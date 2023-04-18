# Comparing `tmp/MTGProxyPrinter-0.21.0.tar.gz` & `tmp/MTGProxyPrinter-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MTGProxyPrinter-0.21.0.tar", last modified: Thu Feb  9 09:01:50 2023, max compression
+gzip compressed data, was "MTGProxyPrinter-0.22.0.tar", last modified: Tue Apr 18 18:23:42 2023, max compression
```

## Comparing `MTGProxyPrinter-0.21.0.tar` & `MTGProxyPrinter-0.22.0.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.725671 MTGProxyPrinter-0.21.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.21.0/LICENSE.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.21.0/MANIFEST.in
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.025789 MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9591 2023-02-09 09:01:49.000000 MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13128 2023-02-09 09:01:49.000000 MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-02-09 09:01:49.000000 MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-02-09 09:01:49.000000 MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      115 2023-02-09 09:01:49.000000 MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-02-09 09:01:49.000000 MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9591 2023-02-09 09:01:50.725671 MTGProxyPrinter-0.21.0/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8135 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    27127 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/ThirdPartyLicenses.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.025789 MTGProxyPrinter-0.21.0/doc/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    38622 2023-02-08 13:29:53.000000 MTGProxyPrinter-0.21.0/doc/changelog.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.137770 MTGProxyPrinter-0.21.0/mtg_proxy_printer/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2253 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/__main__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      828 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/app_dirs.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11170 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/application.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/argument_parser.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    31681 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/card_info_downloader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8968 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_downloader.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.145769 MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10048 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/csv_parsers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10903 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/re_parsers.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.157767 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/_interface.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11368 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/card_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/compact_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/edit_document_settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/import_deck_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/load_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/move_cards.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/new_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/page_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/replace_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4094 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/shuffle_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/downloader_base.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/http_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2772 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/logger.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/meta_data.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/metered_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/missing_images_manager.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.245752 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10880 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/card_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    37302 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/carddb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7195 2022-10-04 12:35:01.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/carddb.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    30247 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/carddb_migrations.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v2.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v3.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v4.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v5.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21573 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    27222 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document_loader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1650 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    18932 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/imagedb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/string_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/natsort.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/print.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.245752 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:49.989795 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.257750 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:49.993795 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.325738 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.365731 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.401725 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      481 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.409724 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/index.theme
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:49.993795 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/status/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.417723 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/status/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.417723 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/status/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7125 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/resources.qrc
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.473713 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7266 2022-10-03 10:12:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/about_dialog.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.493710 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6278 2022-04-03 09:13:06.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5746 2022-03-27 19:48:38.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.517706 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3533 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5290 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1119 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.517706 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4127 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3982 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3592 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.537702 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5021 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3115 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    19716 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10907 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/main_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1884 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16376 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/page_config_widget.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.537702 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8075 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8622 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    25603 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16985 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5579 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/sqlite_helpers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/stop_thread.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.537702 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12951 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/add_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20065 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8259 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/central_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3626 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    31138 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/deck_import_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11517 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/dialogs.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.569697 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8278 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/about_dialog.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.653683 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8445 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8009 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.677679 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4488 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5958 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1666 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.697675 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5413 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5140 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4041 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.697675 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6846 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4337 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16841 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14308 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1821 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/page_config_dialog.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16398 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/page_config_widget.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-09 09:01:50.725671 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13255 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11450 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    30085 2023-02-08 13:18:24.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3583 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/item_delegates.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23416 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7234 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/page_config_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    24945 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/page_renderer.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5569 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/printing_filter_widgets.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17050 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2091 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/units_and_sizes.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-02-09 09:01:08.000000 MTGProxyPrinter-0.21.0/mtg_proxy_printer/update_checker.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5010 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-02-09 09:01:50.725671 MTGProxyPrinter-0.21.0/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-02-03 18:03:28.000000 MTGProxyPrinter-0.21.0/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.22.0/LICENSE.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.22.0/MANIFEST.in
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.125462 MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9626 2023-04-18 18:23:42.000000 MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13128 2023-04-18 18:23:42.000000 MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-04-18 18:23:42.000000 MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-04-18 18:23:42.000000 MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      219 2023-04-18 18:23:42.000000 MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-04-18 18:23:42.000000 MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9626 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8170 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/README.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    27127 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/ThirdPartyLicenses.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.129462 MTGProxyPrinter-0.22.0/doc/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    39620 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/doc/changelog.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.129462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3163 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/__main__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      828 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/app_dirs.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11170 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/application.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/argument_parser.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    31505 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/card_info_downloader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16610 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_downloader.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.129462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10420 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/csv_parsers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11291 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/re_parsers.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.129462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/_interface.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11368 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/card_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/compact_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/edit_document_settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/import_deck_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/load_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/move_cards.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/new_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/page_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/replace_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4094 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/shuffle_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/downloader_base.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/http_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2772 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/logger.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-04-18 18:21:05.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/meta_data.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/metered_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/missing_images_manager.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.129462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10880 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/card_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    37302 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/carddb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7195 2022-10-04 12:35:01.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/carddb.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    30247 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/carddb_migrations.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v2.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v3.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v4.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v5.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    21573 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    27307 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document_loader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1650 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    18932 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/imagedb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/string_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/natsort.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/print.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.129462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.125462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.129462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.125462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.133462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.133462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.137462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      481 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.137462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/index.theme
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.125462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/status/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.137462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/status/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.137462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/status/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7125 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/resources.qrc
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.137462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7266 2022-10-03 10:12:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/about_dialog.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.137462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6278 2022-04-03 09:13:06.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5746 2022-03-27 19:48:38.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3533 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5290 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1119 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4127 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3982 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3592 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5018 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3115 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20314 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10907 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/main_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1884 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16376 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/page_config_widget.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8075 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8622 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    25603 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16985 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5579 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/sqlite_helpers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/stop_thread.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12951 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/add_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20065 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8259 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/central_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3626 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    31709 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/deck_import_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11517 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/dialogs.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8278 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/about_dialog.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8445 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8009 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4488 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5958 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1666 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5413 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5140 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4041 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6843 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4337 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17319 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14308 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1821 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/page_config_dialog.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16398 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/page_config_widget.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13255 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11450 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    30085 2023-04-18 18:23:35.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3583 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/item_delegates.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23416 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7234 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/page_config_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    24943 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/page_renderer.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5569 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/printing_filter_widgets.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17050 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2091 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/units_and_sizes.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/mtg_proxy_printer/update_checker.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5555 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-04-18 18:23:42.141462 MTGProxyPrinter-0.22.0/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-04-18 18:20:09.000000 MTGProxyPrinter-0.22.0/setup.py
```

### Comparing `MTGProxyPrinter-0.21.0/LICENSE.md` & `MTGProxyPrinter-0.22.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/PKG-INFO` & `MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.21.0
+Version: 0.22.0
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
@@ -78,14 +78,15 @@
 
 - [Scryfall](https://scryfall.com)
 - [MTGGoldfish](https://www.mtggoldfish.com/)
 - [mtg.wtf](https://mtg.wtf/)
 - [TappedOut](https://tappedout.net/)
 - [Moxfield](https://www.moxfield.com/)
 - [Deckstats](https://deckstats.net/)
+- [MTGDecks](https://mtgdecks.net)
 
 Except for Scryfall, these websites do not offer a stable, public Web API. Support is offered on a
 “best effort” base and may break at any time, if a website decides to re-design their code.
 
 ## Requirements
 
 - Python >= 3.8
```

### Comparing `MTGProxyPrinter-0.21.0/MTGProxyPrinter.egg-info/SOURCES.txt` & `MTGProxyPrinter-0.22.0/MTGProxyPrinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/PKG-INFO` & `MTGProxyPrinter-0.22.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.21.0
+Version: 0.22.0
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
@@ -78,14 +78,15 @@
 
 - [Scryfall](https://scryfall.com)
 - [MTGGoldfish](https://www.mtggoldfish.com/)
 - [mtg.wtf](https://mtg.wtf/)
 - [TappedOut](https://tappedout.net/)
 - [Moxfield](https://www.moxfield.com/)
 - [Deckstats](https://deckstats.net/)
+- [MTGDecks](https://mtgdecks.net)
 
 Except for Scryfall, these websites do not offer a stable, public Web API. Support is offered on a
 “best effort” base and may break at any time, if a website decides to re-design their code.
 
 ## Requirements
 
 - Python >= 3.8
```

### Comparing `MTGProxyPrinter-0.21.0/README.md` & `MTGProxyPrinter-0.22.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 - [Scryfall](https://scryfall.com)
 - [MTGGoldfish](https://www.mtggoldfish.com/)
 - [mtg.wtf](https://mtg.wtf/)
 - [TappedOut](https://tappedout.net/)
 - [Moxfield](https://www.moxfield.com/)
 - [Deckstats](https://deckstats.net/)
+- [MTGDecks](https://mtgdecks.net)
 
 Except for Scryfall, these websites do not offer a stable, public Web API. Support is offered on a
 “best effort” base and may break at any time, if a website decides to re-design their code.
 
 ## Requirements
 
 - Python >= 3.8
```

### Comparing `MTGProxyPrinter-0.21.0/ThirdPartyLicenses.md` & `MTGProxyPrinter-0.22.0/ThirdPartyLicenses.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/doc/changelog.md` & `MTGProxyPrinter-0.22.0/doc/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Changelog
 
+# Version 0.22.0 (2023-04-18)  <a name="v0_22_0"></a>
+
+## New features
+
+- Added support for importing Magic Workstation Deck Data (`.mwDeck`) deck lists
+- Support for direct downloads from additional card list database websites:
+  - MTG Arena Zone ([mtgazone.com](https://mtgazone.com))
+  - MTGTop8 ([mtgtop8.com](http://mtgtop8.com))
+  - MTGDecks ([mtgdecks.net](https://mtgdecks.net/))
+  - Archidekt ([archidekt.com](https://archidekt.com/))
+  - TCGPlayer Infinite ([infinite.tcgplayer.com](https://infinite.tcgplayer.com/magic-the-gathering))
+
+## Changed features
+
+- Drawing sharp card corners is no longer always enabled,
+  when loading documents created with MTGProxyPrinter version 0.18.0 or older.
+  The option now follows the global application settings.
+- The "funny cards" card filter no longer hides tournament-legal cards from Un-sets like Unfinity.
+
+## Fixed issues
+
+- Fixed crash that occurred when compacting the document moved cards from other pages onto the currently shown page.
+
 # Version 0.21.0 (2023-02-08)  <a name="v0_21_0"></a>
 
 ## New features
 
 - Added Undo and Redo actions. It is now possible to undo changes to the document, and also redo undone changes.
   - The undo and redo button tooltip shows a short description
     of the change that is performed when the button is clicked.
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/__init__.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/__main__.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,32 +12,55 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # Import and implicitly load the settings first, before importing any modules that pull in GUI classes.
 import mtg_proxy_printer.settings
 
+import os
+import platform
+
 from PyQt5.QtCore import Qt, QTimer
 from PyQt5.QtWidgets import QApplication
 
 import mtg_proxy_printer.argument_parser
 import mtg_proxy_printer.logger
 import mtg_proxy_printer.application
+import mtg_proxy_printer.natsort
 
 # Workaround that puts the Application instance into the module scope. This prevents issues with the garbage collector
 # when main() is left. Without, the Python GC interferes with Qt’s memory management and may cause segmentation faults
 # on application exit.
 _app = None
 logger = mtg_proxy_printer.logger.get_logger(__name__)
 
 
+def handle_ssl_certificates():
+    """
+    Ensures that HTTPS connections can be established.
+    On Python >= 3.10, use truststore to use the system native certificate store.
+    On Python < 3.10, use certifi to set the CA certificates
+    """
+    if "SSL_CERT_FILE" in os.environ:
+        logger.info("SSL certificate location set in the environment. Using that for HTTPS connections")
+    elif not mtg_proxy_printer.natsort.str_less_than(platform.python_version(), "3.10"):
+        logger.info("Use system-native SSL trust store via the truststore library for HTTPS connections")
+        import truststore
+        truststore.inject_into_ssl()
+    else:
+        import certifi
+        logger.info("Use certifi library as SSL trust store for HTTPS connections")
+        os.environ["SSL_CERT_FILE"] =  certifi.where()
+
+
 def main():
     global _app
     arguments = mtg_proxy_printer.argument_parser.parse_args()
     mtg_proxy_printer.logger.configure_root_logger()
+    handle_ssl_certificates()
     # According to https://doc.qt.io/qt-5/qt.html#ApplicationAttribute-enum,
     # Qt.AA_EnableHighDpiScaling has to be set prior to creating the QApplication instance
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling)
     _app = mtg_proxy_printer.application.Application(arguments)
     if arguments.test_exit_on_launch:
         logger.info("Skipping startup tasks, because immediate application exit was requested.")
         QTimer.singleShot(0, _app.main_window.on_action_quit_triggered)
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/app_dirs.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/app_dirs.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/application.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/application.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/argument_parser.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/argument_parser.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/card_info_downloader.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/card_info_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,16 +305,14 @@
             self._clear_lru_caches()
             logger.info(f"Finished import with {card_count} imported cards.")
 
     def _populate_database(self, card_data: CardStream, *, total_count: int) -> int:
         logger.info(f"About to populate the database with card data. Expected cards: {total_count or 'unknown'}")
         self.model.begin_transaction()
         progress_report_step = total_count // 100
-        # Look up the printing filter ids only once per import
-        printing_filter_ids = self._read_printing_filters_from_db()
         skipped_cards = 0
         index = 0
         face_ids: IntTuples = []
         db: sqlite3.Connection = self.model.db
         # PrintingDisplayFilter will be re-populated while iterating over the card data.
         # Axing the previous data is far cheaper than trying
         # to update it in-place by removing up to number-of-available-filters entries per each individual card,
@@ -337,15 +335,15 @@
                         SET oracle_id = excluded.oracle_id,
                             language = excluded.language
                         WHERE oracle_id <> excluded.oracle_id
                            OR language <> excluded.language
                     ;"""), (card["id"], card["lang"], self._get_oracle_id(card)))
                 continue
             try:
-                face_ids += self._parse_single_printing(card, printing_filter_ids)
+                face_ids += self._parse_single_printing(card)
             except Exception as e:
                 logger.exception(f"Error while parsing card at position {index}. {card=}")
                 raise RuntimeError(f"Error while parsing card at position {index}: {e}")
             if not index % 10000:
                 logger.debug(f"Imported {index} cards.")
             if progress_report_step and not index % progress_report_step:
                 self.download_progress.emit(index)
@@ -364,41 +362,38 @@
             (index,)
         )
         # Populate the sqlite stat tables to give the query optimizer data to work with.
         db.execute("ANALYZE\n")
         db.commit()
         return index
 
+    @functools.lru_cache(maxsize=1)
     def _read_printing_filters_from_db(self) -> typing.Dict[str, int]:
-        return {
-            filter_name: filter_id
-            for filter_name, filter_id
-            in self.model.db.execute("SELECT filter_name, filter_id FROM DisplayFilters").fetchall()
-        }
+        return dict(self.model.db.execute("SELECT filter_name, filter_id FROM DisplayFilters"))
 
-    def _parse_single_printing(self, card: JSONType, printing_filter_ids):
+    def _parse_single_printing(self, card: JSONType):
         language_id = self._insert_language(card["lang"])
         oracle_id = self._get_oracle_id(card)
         card_id = self._insert_card(oracle_id)
         set_id = self.set_code_cache.get(card["set"])
         if not set_id:
             self.set_code_cache[card["set"]] = set_id = self._insert_set(card)
         printing_id = self._insert_printing(card, card_id, set_id)
         filter_data = self._get_card_filter_data(card)
-        self._insert_card_filters(printing_id, filter_data, printing_filter_ids)
+        self._insert_card_filters(printing_id, filter_data)
         new_face_ids = self._insert_card_faces(card, language_id, printing_id)
         return new_face_ids
 
     def _clear_lru_caches(self):
         """
         Clears the lru_cache instances. If the user re-downloads data, the old, cached keys become invalid and break
         the import. This will lead to assignment of wrong data via invalid foreign key relations.
         To prevent these issues, clear the LRU caches. Also frees RAM by purging data that isn’t used anymore.
         """
-        for cache in (self._insert_language, self._insert_card):
+        for cache in (self._insert_language, self._insert_card, self._read_printing_filters_from_db):
             logger.debug(str(cache.cache_info()))
             cache.cache_clear()
         self.set_code_cache.clear()
 
     def _clean_unused_data(self, new_face_ids: IntTuples):
         """Purges all excess data, like printings that are no longer in the import data."""
         db = self.model.db
@@ -554,15 +549,15 @@
             "hide-cards-without-images": card["image_status"] == "placeholder",
             "hide-oversized-cards": card["oversized"],
             # Border filter
             "hide-white-bordered": card["border_color"] == "white",
             "hide-gold-bordered": card["border_color"] == "gold",
             # “Funny” cards, not legal in any constructed format. This includes full-art Contraptions from Unstable and some
             # black-bordered promotional cards, in addition to silver-bordered cards.
-            "hide-funny-cards": card["set_type"] == "funny",
+            "hide-funny-cards": card["set_type"] == "funny" and "legal" not in legalities.values(),
             # Token cards
             "hide-token": card["layout"] == "token",
             "hide-digital-cards": card["digital"],
             # Specific format legality. Use .get() with a default instead of [] to not fail
             # if Scryfall removes one of the listed formats in the future.
             "hide-banned-in-brawl": legalities.get("brawl", "") == "banned",
             "hide-banned-in-commander": legalities.get("commander", "") == "banned",
@@ -593,16 +588,16 @@
         elif card["set_type"] == "promo":
             result = SetWackinessScore.PROMOTIONAL
         else:
             result = SetWackinessScore.REGULAR
         return result
 
     def _insert_card_filters(
-            self, printing_id: int, filter_data: typing.Dict[str, bool],
-            printing_filter_ids: typing.Dict[str, int]):
+            self, printing_id: int, filter_data: typing.Dict[str, bool]):
+        printing_filter_ids = self._read_printing_filters_from_db()
         self.model.db.executemany(
             "INSERT INTO PrintingDisplayFilter (printing_id, filter_id) VALUES (?, ?)\n",
             ((printing_id, printing_filter_ids[filter_name])
              for filter_name, filter_applies in filter_data.items() if filter_applies)
         )
 
     @staticmethod
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/common.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/csv_parsers.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/csv_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,14 @@
     "TappedOutCSVParser",
 ]
 
 
 class BaseCSVParser(ParserBase):
 
     DIALECT_NAME = ""
-
-    SUPPORTED_FILE_TYPES = {
-        "CSV-Document": ["csv"]
-    }
     USED_COLUMNS: typing.Set[str] = {
 
     }
 
     def parse_deck_internal(self, deck_list: str, print_guessing: bool, language_override: str = None) -> ParsedDeck:
         deck = collections.Counter()
         unmatched_lines = []
@@ -81,14 +77,22 @@
         pass
 
     def should_skip_entry(self, line: typing.Dict[str, str]) -> bool:
         return False
 
 
 class ScryfallCSVParser(BaseCSVParser):
+    """
+    This parser handles CSV-based exports from Scryfall.com. It expects a header
+
+    Primary columns used:
+        scryfall_id, count
+    Secondary columns used (in case scryfall_id is unknown or refers to a hidden printing):
+        lang, name, set_code, collector_number
+    """
 
     class Dialect(csv.Dialect):
         '''
         Specifies the CSV dialect used by Scryfall’s CSV deck export function
         The parameters were determined by inspecting exports.
         As a test case, a deck containing "Ach! Hans, Run!" was used.
         (Note that the actual card name contains both a comma and the quotation marks.)
@@ -102,14 +106,18 @@
         quoting = csv.QUOTE_MINIMAL
 
     DIALECT_NAME = "scryfall_com"
     USED_COLUMNS = {
         "scryfall_id", "count", "lang", "name", "set_code", "collector_number",
     }
 
+    SUPPORTED_FILE_TYPES = {
+        "Scryfall CSV export": ["csv"]
+    }
+
     def parse_cards_from_line(self, line: typing.Dict[str, str], guess_printing: bool, language_override: str = None) \
             -> LineParserResult:
         cards = collections.Counter()
         scryfall_id = line["scryfall_id"]
         count = int(line["count"])
         language = line["lang"]
         target_language = language_override or language
@@ -166,14 +174,17 @@
 
     DIALECT_NAME = "tappedout_net"
     USED_COLUMNS = {
         # Does not include the Language column,
         # because there is the fallback to the old "Languange" column.
         "Qty", "Name", "Board", "Printing",
     }
+    SUPPORTED_FILE_TYPES = {
+        "Tappedout CSV export": ["csv"]
+    }
 
     def __init__(self, card_db: CardDatabase, image_db: ImageDatabase,
                  include_maybe_board: bool = False, include_acquire_board: bool = False, parent: QObject = None):
         super(TappedOutCSVParser, self).__init__(card_db, image_db, parent)
         self.allowed_boards = {"main", "side"}
         if include_maybe_board:
             self.allowed_boards.add("maybe")
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/decklist_parser/re_parsers.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/decklist_parser/re_parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 logger = get_logger(__name__)
 del get_logger
 
 MatchType = typing.Dict[str, str]
 
 __all__ = [
     "GenericRegularExpressionDeckParser",
+    "MagicWorkstationDeckDataFormatParser",
     "MTGArenaParser",
     "MTGOnlineParser",
     "XMageParser",
 ]
 
 try:
     # Profiling decorator, injected into globals by line-profiler. Because the injection does funky stuff, this
@@ -58,14 +59,15 @@
     IDENTIFYING_GROUP_COMBINATIONS = frozenset((
         frozenset({"set_code", "collector_number"}),
         frozenset({"scryfall_id"}),
         frozenset({"name"}),
     ))
 
     LINES_TO_SKIP = frozenset()
+    PREFIXES_TO_SKIP = frozenset()
 
     def __init__(
             self, card_db: CardDatabase, image_db: ImageDatabase, regular_expression: typing.Union[re.Pattern, str],
             parent: QObject = None):
         super().__init__(card_db, image_db, parent)
         self.parser = regular_expression \
             if isinstance(regular_expression, re.Pattern) \
@@ -154,22 +156,37 @@
             # Many sources combine both names of split- or flip-cards as "Front // Back". If so, simply remove the
             # second name, as the back, if any, will be added later.
             name = name.split("//")[0].rstrip()
         return name
 
     def line_splitter(self, deck_list: str) -> typing.Generator[str, None, None]:
         """
-        Split the input deck list into individual lines, omitting empty lines.
+        Split the input deck list into individual lines, omitting empty lines,
+        lines that only contain
         Subclasses can overwrite this method to provide custom filtering for unrelated meta-data.
         """
         for line in deck_list.splitlines():
-            if line and line not in self.LINES_TO_SKIP:
+            if line and line not in self.LINES_TO_SKIP and not any(map(line.startswith, self.PREFIXES_TO_SKIP)):
                 yield line
 
 
+class MagicWorkstationDeckDataFormatParser(GenericRegularExpressionDeckParser):
+
+    SUPPORTED_FILE_TYPES = {
+        "Magic Workstation Deck Data Format": ["mwDeck"],
+    }
+    PREFIXES_TO_SKIP = frozenset({"//"})
+
+    def __init__(self, card_db: CardDatabase, image_db: ImageDatabase, parent: QObject = None):
+        super().__init__(
+            card_db, image_db,
+            re.compile(r"(SB: {2})?(?P<copies>\d+) \[(?P<set_code>\w+)?] (?P<name>.+)"), parent
+        )
+
+
 class MTGArenaParser(GenericRegularExpressionDeckParser):
     """
     A parser for MTG Arena deck lists (file extension .mtga). moxfield.com uses this format to export deck lists.
     """
     SUPPORTED_FILE_TYPES = {
         # Magic Arena typically uses the clipboard. Some sites offer downloads with the .txt ending.
         # XMage also lists the .mtga suffix, so add that too.
@@ -223,19 +240,14 @@
     """
     A parser for XMage deck files (file extension ".dck").
     """
 
     SUPPORTED_FILE_TYPES = {
         "XMage Deck file": ["dck"],
     }
+    PREFIXES_TO_SKIP = frozenset(("NAME", "LAYOUT"))
 
     def __init__(self, card_db: CardDatabase, image_db: ImageDatabase, parent: QObject = None):
         super().__init__(
             card_db, image_db,
             re.compile(r"(SB: )?(?P<copies>\d+) \[(?P<set_code>\w+):(?P<collector_number>[^]]+)] (?P<name>.+)"), parent
         )
-
-    def line_splitter(self, deck_list: str) -> typing.Generator[str, None, None]:
-        # Skip the deck name, if set, and the deck/sideboard layout
-        for line in super().line_splitter(deck_list):
-            if not line.startswith("NAME") and not line.startswith("LAYOUT"):
-                yield line
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/_interface.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/_interface.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/card_actions.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/card_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/compact_document.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/compact_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/edit_document_settings.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/edit_document_settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/import_deck_list.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/import_deck_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/load_document.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/load_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/move_cards.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/move_cards.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/new_document.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/new_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/page_actions.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/page_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/replace_card.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/replace_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/document_controller/shuffle_document.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/document_controller/shuffle_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/downloader_base.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/downloader_base.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/http_file.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/http_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/logger.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/logger.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/meta_data.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/meta_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 PROGRAMNAME = "MTGProxyPrinter"
-__version__ = "0.21.0"
+__version__ = "0.22.0"
 COPYRIGHT = "(C) 2019-2023 Thomas Hess"
 HOME_PAGE = "https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter"
 
 DOWNLOAD_WEB_PAGE = f"{HOME_PAGE}/uv/download.html"
 USER_AGENT = f"{PROGRAMNAME}/{__version__} ({HOME_PAGE})"
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/metered_file.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/metered_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/missing_images_manager.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/missing_images_manager.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/card_list.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/card_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/carddb.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/carddb.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/carddb.sql` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/carddb.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/carddb_migrations.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/carddb_migrations.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v2.sql` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v2.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v3.sql` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v3.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v4.sql` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v4.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document-v5.sql` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document-v5.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document_loader.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,20 +378,21 @@
                 ), f"Invalid data found in the save data at row {row_number}. Aborting")
                 page, slot, scryfall_id, is_front = row_data
                 card_data.append((page, slot, scryfall_id, bool(is_front)))
             return card_data
 
         @staticmethod
         def _read_page_layout_data_from_database(db, user_version):
+            default_settings = PageLayoutSettings.create_from_settings()
             if user_version >= 4:
                 document_settings_query = textwrap.dedent(f"""\
                     SELECT page_height, page_width,
                            margin_top, margin_bottom, margin_left, margin_right,
                            image_spacing_horizontal, image_spacing_vertical, draw_cut_markers,
-                           {'1' if user_version == 4 else 'draw_sharp_corners'}
+                           {int(default_settings.draw_sharp_corners) if user_version == 4 else 'draw_sharp_corners'}
                         FROM DocumentSettings
                         WHERE rowid == 1
                     """)
                 assert_that(
                     db.execute("SELECT COUNT(*) FROM DocumentSettings").fetchone(),
                     contains_exactly(1),
                 )
@@ -416,15 +417,15 @@
                     settings.compute_page_card_capacity(),
                     is_(greater_than_or_equal_to(1)),
                     "Document settings invalid: At least one card has to fit on a page."
                 )
                 settings.draw_cut_markers = bool(settings.draw_cut_markers)
                 settings.draw_sharp_corners = bool(settings.draw_sharp_corners)
             else:
-                settings = PageLayoutSettings.create_from_settings()
+                settings = default_settings
             return settings
 
         @staticmethod
         def _validate_database_schema(db_unsafe: sqlite3.Connection) -> int:
             """
             Validates the database schema of the user-provided file against a known-good schema.
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/document_page.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/document_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/imagedb.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/imagedb.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/model/string_list.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/model/string_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/natsort.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/natsort.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/print.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/print.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/index.theme` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/index.theme`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/resources.qrc` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/about_dialog.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui`

```diff
@@ -52,15 +52,15 @@
             <iconset theme="edit-download"/>
           </property>
         </widget>
       </item>
       <item row="2" column="0" colspan="3">
         <widget class="QPushButton" name="deck_list_browse_button">
           <property name="toolTip">
-            <string>Opens a file picker and let’s you load a deck file from disk.</string>
+            <string>Opens a file picker and lets you load a deck file from disk.</string>
           </property>
           <property name="text">
             <string>Select deck list file</string>
           </property>
           <property name="icon">
             <iconset theme="document-open">
               <normaloff>.</normaloff>
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui`

 * *Files 4% similar despite different names*

#### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui`

```diff
@@ -13,31 +13,133 @@
     <property name="title">
       <string>Import a deck list for printing</string>
     </property>
     <property name="subTitle">
       <string>Select which kind of deck list you want to import.</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="5" column="1">
-        <spacer name="tapped_out_board_spacer">
+      <item row="3" column="1" colspan="4">
+        <widget class="QRadioButton" name="select_parser_xmage">
+          <property name="toolTip">
+            <string>Decklist files, stored in XMage’s native format.
+Because XMage closely follows Scryfall regarding Magic sets,
+this should give very accurate results.</string>
+          </property>
+          <property name="text">
+            <string>XMage</string>
+          </property>
+        </widget>
+      </item>
+      <item row="6" column="3">
+        <widget class="QCheckBox" name="tappedout_include_acquire_board">
+          <property name="enabled">
+            <bool>false</bool>
+          </property>
+          <property name="toolTip">
+            <string>This is a Tappedout-specific section of the deck.
+It may contain the decklist author’s buylist or anything else.</string>
+          </property>
+          <property name="text">
+            <string>Include “Acquire-Board”</string>
+          </property>
+        </widget>
+      </item>
+      <item row="1" column="1" colspan="4">
+        <widget class="QRadioButton" name="select_parser_mtg_online">
+          <property name="toolTip">
+            <string>The simplistic format used by Magic Online. It does not specify exact printings, so may not give the best results.</string>
+          </property>
+          <property name="text">
+            <string>Magic Online</string>
+          </property>
+        </widget>
+      </item>
+      <item row="11" column="1">
+        <spacer name="sample_buttons_spacer">
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+          <property name="sizeType">
+            <enum>QSizePolicy::Fixed</enum>
+          </property>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>20</height>
+            </size>
+          </property>
+        </spacer>
+      </item>
+      <item row="9" column="1">
+        <spacer name="custom_re_input_spacer">
           <property name="orientation">
             <enum>Qt::Horizontal</enum>
           </property>
           <property name="sizeType">
             <enum>QSizePolicy::Fixed</enum>
           </property>
           <property name="sizeHint" stdset="0">
             <size>
               <width>20</width>
               <height>20</height>
             </size>
           </property>
         </spacer>
       </item>
-      <item row="10" column="2" colspan="3">
+      <item row="6" column="2">
+        <widget class="QCheckBox" name="tappedout_include_maybe_board">
+          <property name="enabled">
+            <bool>false</bool>
+          </property>
+          <property name="toolTip">
+            <string>This is a Tappedout-specific section of the deck.
+It may contain cards that the decklist creator considers for inclusion, based on the meta
+or any other preference, like card price.</string>
+          </property>
+          <property name="text">
+            <string>Include “Maybe-Board”</string>
+          </property>
+        </widget>
+      </item>
+      <item row="4" column="1" colspan="4">
+        <widget class="QRadioButton" name="select_parser_scryfall_csv">
+          <property name="toolTip">
+            <string>CSV exports from Scryfall’s own deck builder.
+Gives very accurate results, unless the imported deck list contains ignored items
+matching a configured download filter.</string>
+          </property>
+          <property name="text">
+            <string>Scryfall.com deck lists (CSV export)</string>
+          </property>
+        </widget>
+      </item>
+      <item row="14" column="1" colspan="4">
+        <spacer name="verticalSpacer">
+          <property name="orientation">
+            <enum>Qt::Vertical</enum>
+          </property>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>40</height>
+            </size>
+          </property>
+        </spacer>
+      </item>
+      <item row="5" column="1" colspan="4">
+        <widget class="QRadioButton" name="select_parser_tappedout_csv">
+          <property name="toolTip">
+            <string>CSV exports can be downloaded from Tappedout by choosing the appropriate deck export option.</string>
+          </property>
+          <property name="text">
+            <string>tappedout.net deck list (CSV export)</string>
+          </property>
+        </widget>
+      </item>
+      <item row="11" column="2" colspan="3">
         <layout class="QGridLayout" name="sample_buttons_layout">
           <item row="0" column="1">
             <widget class="QPushButton" name="insert_set_code_matcher_sample_button">
               <property name="enabled">
                 <bool>false</bool>
               </property>
               <property name="toolTip">
@@ -115,37 +217,68 @@
               <property name="text">
                 <string>Language matcher</string>
               </property>
             </widget>
           </item>
         </layout>
       </item>
-      <item row="1" column="1" colspan="4">
-        <widget class="QRadioButton" name="select_parser_mtg_online">
+      <item row="8" column="1" colspan="4">
+        <widget class="QRadioButton" name="select_parser_custom_re">
           <property name="toolTip">
-            <string>The simplistic format used by Magic Online. It does not specify exact printings, so may not give the best results.</string>
+            <string>Specify a custom regular expression in the input field below. It will be used to parse each deck list line.
+You can use the buttons below to insert basic building blocks.
+You have to separate them with the “control structures”, like spaces, as used in your deck list.</string>
           </property>
           <property name="text">
-            <string>Magic Online</string>
+            <string>Custom regular expression based parser:</string>
           </property>
         </widget>
       </item>
+      <item row="6" column="1">
+        <spacer name="tapped_out_board_spacer">
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+          <property name="sizeType">
+            <enum>QSizePolicy::Fixed</enum>
+          </property>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>20</height>
+            </size>
+          </property>
+        </spacer>
+      </item>
+      <item row="6" column="4">
+        <spacer name="horizontalSpacer">
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>40</width>
+              <height>20</height>
+            </size>
+          </property>
+        </spacer>
+      </item>
       <item row="0" column="1" colspan="4">
         <widget class="QRadioButton" name="select_parser_mtg_arena">
           <property name="toolTip">
             <string>Magic Arena and exports from compatible websites, like moxfield.com
 Note that this option is not limited to cards in Standard/Historic,
 as the format works for any card.</string>
           </property>
           <property name="text">
             <string>MTG Arena</string>
           </property>
         </widget>
       </item>
-      <item row="8" column="2" colspan="3">
+      <item row="9" column="2" colspan="3">
         <widget class="QLineEdit" name="custom_re_input">
           <property name="enabled">
             <bool>false</bool>
           </property>
           <property name="toolTip">
             <string>Use this regular expression to parse the deck list file. See the context help (?-Button) for more detailes.</string>
           </property>
@@ -170,164 +303,38 @@
             <string>(?P&lt;copies&gt;\w+) (?P&lt;name&gt;.+) \((?P&lt;set_code&gt;\w+)\) (?P&lt;collector_number&gt;\d+)</string>
           </property>
           <property name="clearButtonEnabled">
             <bool>true</bool>
           </property>
         </widget>
       </item>
-      <item row="13" column="1" colspan="4">
-        <spacer name="verticalSpacer">
-          <property name="orientation">
-            <enum>Qt::Vertical</enum>
-          </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>40</height>
-            </size>
-          </property>
-        </spacer>
-      </item>
-      <item row="4" column="1" colspan="4">
-        <widget class="QRadioButton" name="select_parser_tappedout_csv">
-          <property name="toolTip">
-            <string>CSV exports can be downloaded from Tappedout by choosing the appropriate deck export option.</string>
-          </property>
-          <property name="text">
-            <string>tappedout.net deck list (CSV export)</string>
-          </property>
-        </widget>
-      </item>
-      <item row="3" column="1" colspan="4">
-        <widget class="QRadioButton" name="select_parser_scryfall_csv">
-          <property name="toolTip">
-            <string>CSV exports from Scryfall’s own deck builder.
-Gives very accurate results, unless the imported deck list contains ignored items
-matching a configured download filter.</string>
-          </property>
-          <property name="text">
-            <string>Scryfall.com deck lists (CSV export)</string>
-          </property>
-        </widget>
-      </item>
-      <item row="7" column="1" colspan="4">
-        <widget class="QRadioButton" name="select_parser_custom_re">
-          <property name="toolTip">
-            <string>Specify a custom regular expression in the input field below. It will be used to parse each deck list line.
-You can use the buttons below to insert basic building blocks.
-You have to separate them with the “control structures”, like spaces, as used in your deck list.</string>
-          </property>
-          <property name="text">
-            <string>Custom regular expression based parser:</string>
-          </property>
-        </widget>
-      </item>
-      <item row="10" column="1">
-        <spacer name="sample_buttons_spacer">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="sizeType">
-            <enum>QSizePolicy::Fixed</enum>
-          </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>20</height>
-            </size>
-          </property>
-        </spacer>
-      </item>
-      <item row="8" column="1">
-        <spacer name="custom_re_input_spacer">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="sizeType">
-            <enum>QSizePolicy::Fixed</enum>
-          </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>20</height>
-            </size>
-          </property>
-        </spacer>
-      </item>
       <item row="2" column="1" colspan="4">
-        <widget class="QRadioButton" name="select_parser_xmage">
-          <property name="toolTip">
-            <string>Decklist files, stored in XMage’s native format.
-Because XMage closely follows Scryfall regarding Magic sets,
-this should give very accurate results.</string>
-          </property>
-          <property name="text">
-            <string>XMage</string>
-          </property>
-        </widget>
-      </item>
-      <item row="5" column="2">
-        <widget class="QCheckBox" name="tappedout_include_maybe_board">
-          <property name="enabled">
-            <bool>false</bool>
-          </property>
-          <property name="toolTip">
-            <string>This is a Tappedout-specific section of the deck.
-It may contain cards that the decklist creator considers for inclusion, based on the meta
-or any other preference, like card price.</string>
-          </property>
-          <property name="text">
-            <string>Include “Maybe-Board”</string>
-          </property>
-        </widget>
-      </item>
-      <item row="5" column="3">
-        <widget class="QCheckBox" name="tappedout_include_acquire_board">
-          <property name="enabled">
-            <bool>false</bool>
-          </property>
-          <property name="toolTip">
-            <string>This is a Tappedout-specific section of the deck.
-It may contain the decklist author’s buylist or anything else.</string>
-          </property>
+        <widget class="QRadioButton" name="select_parser_magic_workstation">
           <property name="text">
-            <string>Include “Acquire-Board”</string>
+            <string>Magic Workstation Deck Data (mwDeck)</string>
           </property>
         </widget>
       </item>
-      <item row="5" column="4">
-        <spacer name="horizontalSpacer">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>40</width>
-              <height>20</height>
-            </size>
-          </property>
-        </spacer>
-      </item>
     </layout>
   </widget>
   <resources/>
   <connections>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>toggled(bool)</signal>
       <receiver>custom_re_input</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>120</x>
-          <y>188</y>
+          <x>126</x>
+          <y>223</y>
         </hint>
         <hint type="destinationlabel">
-          <x>176</x>
-          <y>225</y>
+          <x>208</x>
+          <y>261</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_mtg_arena</sender>
       <signal>clicked()</signal>
       <receiver>WizardPage</receiver>
@@ -362,210 +369,226 @@
     <connection>
       <sender>select_parser_scryfall_csv</sender>
       <signal>clicked()</signal>
       <receiver>WizardPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>26</x>
-          <y>103</y>
+          <x>32</x>
+          <y>139</y>
         </hint>
         <hint type="destinationlabel">
           <x>20</x>
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>clicked()</signal>
       <receiver>WizardPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>38</x>
-          <y>188</y>
+          <x>44</x>
+          <y>223</y>
         </hint>
         <hint type="destinationlabel">
           <x>20</x>
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_xmage</sender>
       <signal>clicked()</signal>
       <receiver>WizardPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>26</x>
-          <y>77</y>
+          <x>32</x>
+          <y>111</y>
         </hint>
         <hint type="destinationlabel">
           <x>20</x>
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>custom_re_input</sender>
       <signal>textChanged(QString)</signal>
       <receiver>WizardPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>215</x>
-          <y>225</y>
+          <x>247</x>
+          <y>261</y>
         </hint>
         <hint type="destinationlabel">
           <x>145</x>
           <y>114</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_tappedout_csv</sender>
       <signal>clicked()</signal>
       <receiver>WizardPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>139</x>
-          <y>119</y>
+          <x>145</x>
+          <y>167</y>
         </hint>
         <hint type="destinationlabel">
           <x>139</x>
           <y>101</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_tappedout_csv</sender>
       <signal>toggled(bool)</signal>
       <receiver>tappedout_include_maybe_board</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>92</x>
-          <y>134</y>
+          <x>98</x>
+          <y>167</y>
         </hint>
         <hint type="destinationlabel">
-          <x>88</x>
-          <y>154</y>
+          <x>120</x>
+          <y>195</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_tappedout_csv</sender>
       <signal>toggled(bool)</signal>
       <receiver>tappedout_include_acquire_board</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>277</x>
-          <y>134</y>
+          <x>283</x>
+          <y>167</y>
         </hint>
         <hint type="destinationlabel">
-          <x>369</x>
-          <y>157</y>
+          <x>378</x>
+          <y>195</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>toggled(bool)</signal>
       <receiver>insert_name_matcher_sample_button</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>256</x>
-          <y>187</y>
+          <x>262</x>
+          <y>223</y>
         </hint>
         <hint type="destinationlabel">
-          <x>173</x>
-          <y>240</y>
+          <x>206</x>
+          <y>302</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>toggled(bool)</signal>
       <receiver>insert_collector_number_matcher_sample_button</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>390</x>
-          <y>173</y>
+          <x>396</x>
+          <y>223</y>
         </hint>
         <hint type="destinationlabel">
-          <x>750</x>
-          <y>265</y>
+          <x>759</x>
+          <y>302</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>toggled(bool)</signal>
       <receiver>insert_scryfall_id_matcher_sample_button</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>336</x>
-          <y>180</y>
+          <x>342</x>
+          <y>223</y>
         </hint>
         <hint type="destinationlabel">
-          <x>750</x>
-          <y>304</y>
+          <x>759</x>
+          <y>342</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>toggled(bool)</signal>
       <receiver>insert_set_code_matcher_sample_button</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>390</x>
-          <y>181</y>
+          <x>396</x>
+          <y>223</y>
         </hint>
         <hint type="destinationlabel">
-          <x>392</x>
-          <y>257</y>
+          <x>515</x>
+          <y>302</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>toggled(bool)</signal>
       <receiver>insert_copies_matcher_sample_button</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>390</x>
-          <y>181</y>
+          <x>396</x>
+          <y>223</y>
         </hint>
         <hint type="destinationlabel">
-          <x>173</x>
-          <y>283</y>
+          <x>206</x>
+          <y>342</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>toggled(bool)</signal>
       <receiver>insert_language_matcher_sample_button</receiver>
       <slot>setEnabled(bool)</slot>
       <hints>
         <hint type="sourcelabel">
-          <x>446</x>
-          <y>181</y>
+          <x>452</x>
+          <y>223</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>515</x>
+          <y>342</y>
+        </hint>
+      </hints>
+    </connection>
+    <connection>
+      <sender>select_parser_magic_workstation</sender>
+      <signal>clicked()</signal>
+      <receiver>WizardPage</receiver>
+      <slot>isComplete()</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>383</x>
+          <y>72</y>
         </hint>
         <hint type="destinationlabel">
-          <x>448</x>
-          <y>296</y>
+          <x>383</x>
+          <y>297</y>
         </hint>
       </hints>
     </connection>
   </connections>
 </ui>
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/main_window.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/page_config_dialog.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/page_config_widget.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/page_config_widget.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/settings.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/sqlite_helpers.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/sqlite_helpers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/stop_thread.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/stop_thread.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/add_card.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/add_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/central_widget.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/central_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/common.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/deck_import_wizard.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/deck_import_wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,17 @@
                 self, "Select deck file", default_path, file_extension_filter)
             self._load_from_file(selected_file)
 
     @staticmethod
     def get_file_extension_filter() -> str:
         parsers = [
             re_parsers.MTGOnlineParser, re_parsers.MTGArenaParser, re_parsers.XMageParser,
-            csv_parsers.ScryfallCSVParser, csv_parsers.TappedOutCSVParser]
+            re_parsers.MagicWorkstationDeckDataFormatParser,
+            csv_parsers.ScryfallCSVParser, csv_parsers.TappedOutCSVParser,
+        ]
         everything = "All files (*)"
         individual_file_types = list(
             itertools.chain.from_iterable(parser.SUPPORTED_FILE_TYPES.items() for parser in parsers)
         )
         # At this point, the data required (file extension list) is in a list of dict values containing
         # lists of strings. Thus, it requires two levels of iterable unpacking. Because of duplicates in file,
         # extensions across all parsers, de-duplicate and then sort the result.
@@ -280,14 +282,17 @@
         self.ui.insert_language_matcher_sample_button.clicked.connect(
             lambda: self.append_group_to_custom_re_input(r"(?P<language>[a-zA-Z]{2})"))
         self.ui.insert_scryfall_id_matcher_sample_button.clicked.connect(
             lambda: self.append_group_to_custom_re_input(r"(?P<scryfall_id>[a-f\d]{8}(-[a-f\d]{4}){3}-[a-f\d]{12})"))
         self.complete = False
         self.registerField("custom_re", self.ui.custom_re_input)
         self.registerField("selected_parser", self)
+        self.ui.select_parser_magic_workstation.clicked.connect(
+            lambda: setattr(self, "parser_creator", self._create_magic_workstation_parser)
+        )
         self.ui.select_parser_mtg_arena.clicked.connect(
             lambda: setattr(self, "parser_creator", self._create_mtg_arena_parser)
         )
         self.ui.select_parser_mtg_online.clicked.connect(
             lambda: setattr(self, "parser_creator", self._create_mtg_online_parser)
         )
         self.ui.select_parser_xmage.clicked.connect(
@@ -306,24 +311,28 @@
 
     def initializePage(self) -> None:
         super().initializePage()
         used_downloader: str = self.field("deck-list-downloaded")
         if used_downloader:
             parser_to_use = AVAILABLE_DOWNLOADERS[used_downloader].PARSER_CLASS
             {
+                re_parsers.MagicWorkstationDeckDataFormatParser: self.ui.select_parser_magic_workstation,
                 re_parsers.MTGArenaParser: self.ui.select_parser_mtg_arena,
                 re_parsers.MTGOnlineParser: self.ui.select_parser_mtg_online,
                 re_parsers.XMageParser: self.ui.select_parser_xmage,
                 csv_parsers.ScryfallCSVParser: self.ui.select_parser_scryfall_csv,
                 csv_parsers.TappedOutCSVParser: self.ui.select_parser_tappedout_csv,
             }[parser_to_use].click()
 
     def append_group_to_custom_re_input(self, value: str):
         self.ui.custom_re_input.setText(self.ui.custom_re_input.text()+value)
 
+    def _create_magic_workstation_parser(self):
+        self.selected_parser = re_parsers.MagicWorkstationDeckDataFormatParser(self.card_db, self.image_db, self)
+
     def _create_mtg_arena_parser(self):
         self.selected_parser = re_parsers.MTGArenaParser(self.card_db, self.image_db, self)
 
     def _create_mtg_online_parser(self):
         self.selected_parser = re_parsers.MTGOnlineParser(self.card_db, self.image_db, self)
 
     def _create_xmage_parser(self):
@@ -342,14 +351,15 @@
         self.selected_parser = re_parsers.GenericRegularExpressionDeckParser(
             self.card_db, self.image_db, self.field("custom_re"), self
         )
 
     @Slot()
     def isComplete(self) -> bool:
         acceptable = any((
+            self.ui.select_parser_magic_workstation.isChecked(),
             self.ui.select_parser_mtg_arena.isChecked(),
             self.ui.select_parser_mtg_online.isChecked(),
             self.ui.select_parser_xmage.isChecked(),
             self.ui.select_parser_scryfall_csv.isChecked(),
             self.ui.select_parser_tappedout_csv.isChecked(),
         )) or all((
                 self.ui.select_parser_custom_re.isChecked(),
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/dialogs.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/about_dialog.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/about_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def retranslateUi(self, WizardPage):
         _translate = QtCore.QCoreApplication.translate
         WizardPage.setTitle(_translate("WizardPage", "Import a deck list for printing"))
         WizardPage.setSubTitle(_translate("WizardPage", "Load a deck file from disk or paste deck list in the text field below"))
         self.translate_deck_list_enable.setText(_translate("WizardPage", "Translate deck list to:"))
         self.deck_list_download_url_line_edit.setPlaceholderText(_translate("WizardPage", "Paste a link to a deck list here. Hover to see supported sites."))
         self.deck_list_download_button.setText(_translate("WizardPage", "Download"))
-        self.deck_list_browse_button.setToolTip(_translate("WizardPage", "Opens a file picker and let’s you load a deck file from disk."))
+        self.deck_list_browse_button.setToolTip(_translate("WizardPage", "Opens a file picker and lets you load a deck file from disk."))
         self.deck_list_browse_button.setText(_translate("WizardPage", "Select deck list file"))
         self.deck_list.setPlaceholderText(_translate("WizardPage", "Paste your deck list here or select a file using the button above."))
         self.print_guessing_enable.setToolTip(_translate("WizardPage", "If checked, choose an arbitrary printing, if a unique printing is not identified.\n"
 "If unchecked, each ambiguous card is ignored and reported as unrecognized."))
         self.print_guessing_enable.setText(_translate("WizardPage", "Guess printings for ambiguous entries in the deck list"))
         self.print_guessing_prefer_already_downloaded.setToolTip(_translate("WizardPage", "When an exact printing is not determined or card translation is requested, choose a printing that is already downloaded, if possible.\n"
 "Enabling this can potentially save disk space and download volume, based on the images already downloaded."))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,40 @@
 
 class Ui_WizardPage(object):
     def setupUi(self, WizardPage):
         WizardPage.setObjectName("WizardPage")
         WizardPage.resize(767, 596)
         self.gridLayout = QtWidgets.QGridLayout(WizardPage)
         self.gridLayout.setObjectName("gridLayout")
+        self.select_parser_xmage = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_xmage.setObjectName("select_parser_xmage")
+        self.gridLayout.addWidget(self.select_parser_xmage, 3, 1, 1, 4)
+        self.tappedout_include_acquire_board = QtWidgets.QCheckBox(WizardPage)
+        self.tappedout_include_acquire_board.setEnabled(False)
+        self.tappedout_include_acquire_board.setObjectName("tappedout_include_acquire_board")
+        self.gridLayout.addWidget(self.tappedout_include_acquire_board, 6, 3, 1, 1)
+        self.select_parser_mtg_online = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_mtg_online.setObjectName("select_parser_mtg_online")
+        self.gridLayout.addWidget(self.select_parser_mtg_online, 1, 1, 1, 4)
         spacerItem = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
-        self.gridLayout.addItem(spacerItem, 5, 1, 1, 1)
+        self.gridLayout.addItem(spacerItem, 11, 1, 1, 1)
+        spacerItem1 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
+        self.gridLayout.addItem(spacerItem1, 9, 1, 1, 1)
+        self.tappedout_include_maybe_board = QtWidgets.QCheckBox(WizardPage)
+        self.tappedout_include_maybe_board.setEnabled(False)
+        self.tappedout_include_maybe_board.setObjectName("tappedout_include_maybe_board")
+        self.gridLayout.addWidget(self.tappedout_include_maybe_board, 6, 2, 1, 1)
+        self.select_parser_scryfall_csv = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_scryfall_csv.setObjectName("select_parser_scryfall_csv")
+        self.gridLayout.addWidget(self.select_parser_scryfall_csv, 4, 1, 1, 4)
+        spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.gridLayout.addItem(spacerItem2, 14, 1, 1, 4)
+        self.select_parser_tappedout_csv = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_tappedout_csv.setObjectName("select_parser_tappedout_csv")
+        self.gridLayout.addWidget(self.select_parser_tappedout_csv, 5, 1, 1, 4)
         self.sample_buttons_layout = QtWidgets.QGridLayout()
         self.sample_buttons_layout.setObjectName("sample_buttons_layout")
         self.insert_set_code_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
         self.insert_set_code_matcher_sample_button.setEnabled(False)
         self.insert_set_code_matcher_sample_button.setObjectName("insert_set_code_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_set_code_matcher_sample_button, 0, 1, 1, 1)
         self.insert_collector_number_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
@@ -41,54 +65,33 @@
         self.insert_scryfall_id_matcher_sample_button.setEnabled(False)
         self.insert_scryfall_id_matcher_sample_button.setObjectName("insert_scryfall_id_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_scryfall_id_matcher_sample_button, 1, 2, 1, 1)
         self.insert_language_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
         self.insert_language_matcher_sample_button.setEnabled(False)
         self.insert_language_matcher_sample_button.setObjectName("insert_language_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_language_matcher_sample_button, 1, 1, 1, 1)
-        self.gridLayout.addLayout(self.sample_buttons_layout, 10, 2, 1, 3)
-        self.select_parser_mtg_online = QtWidgets.QRadioButton(WizardPage)
-        self.select_parser_mtg_online.setObjectName("select_parser_mtg_online")
-        self.gridLayout.addWidget(self.select_parser_mtg_online, 1, 1, 1, 4)
+        self.gridLayout.addLayout(self.sample_buttons_layout, 11, 2, 1, 3)
+        self.select_parser_custom_re = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_custom_re.setObjectName("select_parser_custom_re")
+        self.gridLayout.addWidget(self.select_parser_custom_re, 8, 1, 1, 4)
+        spacerItem3 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
+        self.gridLayout.addItem(spacerItem3, 6, 1, 1, 1)
+        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.gridLayout.addItem(spacerItem4, 6, 4, 1, 1)
         self.select_parser_mtg_arena = QtWidgets.QRadioButton(WizardPage)
         self.select_parser_mtg_arena.setObjectName("select_parser_mtg_arena")
         self.gridLayout.addWidget(self.select_parser_mtg_arena, 0, 1, 1, 4)
         self.custom_re_input = QtWidgets.QLineEdit(WizardPage)
         self.custom_re_input.setEnabled(False)
         self.custom_re_input.setClearButtonEnabled(True)
         self.custom_re_input.setObjectName("custom_re_input")
-        self.gridLayout.addWidget(self.custom_re_input, 8, 2, 1, 3)
-        spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.gridLayout.addItem(spacerItem1, 13, 1, 1, 4)
-        self.select_parser_tappedout_csv = QtWidgets.QRadioButton(WizardPage)
-        self.select_parser_tappedout_csv.setObjectName("select_parser_tappedout_csv")
-        self.gridLayout.addWidget(self.select_parser_tappedout_csv, 4, 1, 1, 4)
-        self.select_parser_scryfall_csv = QtWidgets.QRadioButton(WizardPage)
-        self.select_parser_scryfall_csv.setObjectName("select_parser_scryfall_csv")
-        self.gridLayout.addWidget(self.select_parser_scryfall_csv, 3, 1, 1, 4)
-        self.select_parser_custom_re = QtWidgets.QRadioButton(WizardPage)
-        self.select_parser_custom_re.setObjectName("select_parser_custom_re")
-        self.gridLayout.addWidget(self.select_parser_custom_re, 7, 1, 1, 4)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
-        self.gridLayout.addItem(spacerItem2, 10, 1, 1, 1)
-        spacerItem3 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
-        self.gridLayout.addItem(spacerItem3, 8, 1, 1, 1)
-        self.select_parser_xmage = QtWidgets.QRadioButton(WizardPage)
-        self.select_parser_xmage.setObjectName("select_parser_xmage")
-        self.gridLayout.addWidget(self.select_parser_xmage, 2, 1, 1, 4)
-        self.tappedout_include_maybe_board = QtWidgets.QCheckBox(WizardPage)
-        self.tappedout_include_maybe_board.setEnabled(False)
-        self.tappedout_include_maybe_board.setObjectName("tappedout_include_maybe_board")
-        self.gridLayout.addWidget(self.tappedout_include_maybe_board, 5, 2, 1, 1)
-        self.tappedout_include_acquire_board = QtWidgets.QCheckBox(WizardPage)
-        self.tappedout_include_acquire_board.setEnabled(False)
-        self.tappedout_include_acquire_board.setObjectName("tappedout_include_acquire_board")
-        self.gridLayout.addWidget(self.tappedout_include_acquire_board, 5, 3, 1, 1)
-        spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.gridLayout.addItem(spacerItem4, 5, 4, 1, 1)
+        self.gridLayout.addWidget(self.custom_re_input, 9, 2, 1, 3)
+        self.select_parser_magic_workstation = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_magic_workstation.setObjectName("select_parser_magic_workstation")
+        self.gridLayout.addWidget(self.select_parser_magic_workstation, 2, 1, 1, 4)
 
         self.retranslateUi(WizardPage)
         self.select_parser_custom_re.toggled['bool'].connect(self.custom_re_input.setEnabled) # type: ignore
         self.select_parser_mtg_arena.clicked.connect(WizardPage.isComplete) # type: ignore
         self.select_parser_mtg_online.clicked.connect(WizardPage.isComplete) # type: ignore
         self.select_parser_scryfall_csv.clicked.connect(WizardPage.isComplete) # type: ignore
         self.select_parser_custom_re.clicked.connect(WizardPage.isComplete) # type: ignore
@@ -99,20 +102,40 @@
         self.select_parser_tappedout_csv.toggled['bool'].connect(self.tappedout_include_acquire_board.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_name_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_collector_number_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_scryfall_id_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_set_code_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_copies_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_language_matcher_sample_button.setEnabled) # type: ignore
+        self.select_parser_magic_workstation.clicked.connect(WizardPage.isComplete) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(WizardPage)
 
     def retranslateUi(self, WizardPage):
         _translate = QtCore.QCoreApplication.translate
         WizardPage.setTitle(_translate("WizardPage", "Import a deck list for printing"))
         WizardPage.setSubTitle(_translate("WizardPage", "Select which kind of deck list you want to import."))
+        self.select_parser_xmage.setToolTip(_translate("WizardPage", "Decklist files, stored in XMage’s native format.\n"
+"Because XMage closely follows Scryfall regarding Magic sets,\n"
+"this should give very accurate results."))
+        self.select_parser_xmage.setText(_translate("WizardPage", "XMage"))
+        self.tappedout_include_acquire_board.setToolTip(_translate("WizardPage", "This is a Tappedout-specific section of the deck.\n"
+"It may contain the decklist author’s buylist or anything else."))
+        self.tappedout_include_acquire_board.setText(_translate("WizardPage", "Include “Acquire-Board”"))
+        self.select_parser_mtg_online.setToolTip(_translate("WizardPage", "The simplistic format used by Magic Online. It does not specify exact printings, so may not give the best results."))
+        self.select_parser_mtg_online.setText(_translate("WizardPage", "Magic Online"))
+        self.tappedout_include_maybe_board.setToolTip(_translate("WizardPage", "This is a Tappedout-specific section of the deck.\n"
+"It may contain cards that the decklist creator considers for inclusion, based on the meta\n"
+"or any other preference, like card price."))
+        self.tappedout_include_maybe_board.setText(_translate("WizardPage", "Include “Maybe-Board”"))
+        self.select_parser_scryfall_csv.setToolTip(_translate("WizardPage", "CSV exports from Scryfall’s own deck builder.\n"
+"Gives very accurate results, unless the imported deck list contains ignored items\n"
+"matching a configured download filter."))
+        self.select_parser_scryfall_csv.setText(_translate("WizardPage", "Scryfall.com deck lists (CSV export)"))
+        self.select_parser_tappedout_csv.setToolTip(_translate("WizardPage", "CSV exports can be downloaded from Tappedout by choosing the appropriate deck export option."))
+        self.select_parser_tappedout_csv.setText(_translate("WizardPage", "tappedout.net deck list (CSV export)"))
         self.insert_set_code_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a sample matcher for a set code to the input field above."))
         self.insert_set_code_matcher_sample_button.setText(_translate("WizardPage", "Set code matcher"))
         self.insert_collector_number_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a sample matcher for a collector number to the input field above"))
         self.insert_collector_number_matcher_sample_button.setText(_translate("WizardPage", "Collector number matcher"))
         self.insert_copies_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a matcher for the number of card copies to the input field above.\n"
 "If a card count field is not present in the deck list, 1 card copy per line is assumed"))
         self.insert_copies_matcher_sample_button.setText(_translate("WizardPage", "Copies matcher"))
@@ -121,16 +144,18 @@
         self.insert_scryfall_id_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a matcher for the Scryfall ID to the input field above.\n"
 "This may be used by deck lists that closely integrate with the Scryfall website.\n"
 "Most deck lists won’t use this."))
         self.insert_scryfall_id_matcher_sample_button.setText(_translate("WizardPage", "Scryfall ID matcher"))
         self.insert_language_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a matcher for the  card language to the input field above.\n"
 "If a language field is not present in the deck list, the card language is guessed."))
         self.insert_language_matcher_sample_button.setText(_translate("WizardPage", "Language matcher"))
-        self.select_parser_mtg_online.setToolTip(_translate("WizardPage", "The simplistic format used by Magic Online. It does not specify exact printings, so may not give the best results."))
-        self.select_parser_mtg_online.setText(_translate("WizardPage", "Magic Online"))
+        self.select_parser_custom_re.setToolTip(_translate("WizardPage", "Specify a custom regular expression in the input field below. It will be used to parse each deck list line.\n"
+"You can use the buttons below to insert basic building blocks.\n"
+"You have to separate them with the “control structures”, like spaces, as used in your deck list."))
+        self.select_parser_custom_re.setText(_translate("WizardPage", "Custom regular expression based parser:"))
         self.select_parser_mtg_arena.setToolTip(_translate("WizardPage", "Magic Arena and exports from compatible websites, like moxfield.com\n"
 "Note that this option is not limited to cards in Standard/Historic,\n"
 "as the format works for any card."))
         self.select_parser_mtg_arena.setText(_translate("WizardPage", "MTG Arena"))
         self.custom_re_input.setToolTip(_translate("WizardPage", "Use this regular expression to parse the deck list file. See the context help (?-Button) for more detailes."))
         self.custom_re_input.setWhatsThis(_translate("WizardPage", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
 "<html><head><meta name=\"qrichtext\" content=\"1\" /><style type=\"text/css\">\n"
@@ -144,28 +169,8 @@
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">set_code</span>: The 3 (or more) letter code identifying the set.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">collector_number</span>: The collector number of the card</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">language</span>: The card language, using a two-letter language code. If not given, the importer tries to determine the language from the card name. Defaults to &quot;en&quot; for English, if not possible.<br /></p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">Not all groups are required for a successful match. For example, <span style=\" font-weight:600;\">set_code</span> and <span style=\" font-weight:600;\">collector_number</span> is sufficient for exact identification most of the time.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">Hint: You may want to use an online Regular Expression editor, like <a href=\"https://regex101.com/\"><span style=\" text-decoration: underline; color:#2980b9;\">https://regex101.com/</span></a>, for example.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><br /></p></body></html>"))
         self.custom_re_input.setPlaceholderText(_translate("WizardPage", "(?P<copies>\\w+) (?P<name>.+) \\((?P<set_code>\\w+)\\) (?P<collector_number>\\d+)"))
-        self.select_parser_tappedout_csv.setToolTip(_translate("WizardPage", "CSV exports can be downloaded from Tappedout by choosing the appropriate deck export option."))
-        self.select_parser_tappedout_csv.setText(_translate("WizardPage", "tappedout.net deck list (CSV export)"))
-        self.select_parser_scryfall_csv.setToolTip(_translate("WizardPage", "CSV exports from Scryfall’s own deck builder.\n"
-"Gives very accurate results, unless the imported deck list contains ignored items\n"
-"matching a configured download filter."))
-        self.select_parser_scryfall_csv.setText(_translate("WizardPage", "Scryfall.com deck lists (CSV export)"))
-        self.select_parser_custom_re.setToolTip(_translate("WizardPage", "Specify a custom regular expression in the input field below. It will be used to parse each deck list line.\n"
-"You can use the buttons below to insert basic building blocks.\n"
-"You have to separate them with the “control structures”, like spaces, as used in your deck list."))
-        self.select_parser_custom_re.setText(_translate("WizardPage", "Custom regular expression based parser:"))
-        self.select_parser_xmage.setToolTip(_translate("WizardPage", "Decklist files, stored in XMage’s native format.\n"
-"Because XMage closely follows Scryfall regarding Magic sets,\n"
-"this should give very accurate results."))
-        self.select_parser_xmage.setText(_translate("WizardPage", "XMage"))
-        self.tappedout_include_maybe_board.setToolTip(_translate("WizardPage", "This is a Tappedout-specific section of the deck.\n"
-"It may contain cards that the decklist creator considers for inclusion, based on the meta\n"
-"or any other preference, like card price."))
-        self.tappedout_include_maybe_board.setText(_translate("WizardPage", "Include “Maybe-Board”"))
-        self.tappedout_include_acquire_board.setToolTip(_translate("WizardPage", "This is a Tappedout-specific section of the deck.\n"
-"It may contain the decklist author’s buylist or anything else."))
-        self.tappedout_include_acquire_board.setText(_translate("WizardPage", "Include “Acquire-Board”"))
+        self.select_parser_magic_workstation.setText(_translate("WizardPage", "Magic Workstation Deck Data (mwDeck)"))
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/main_window.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/main_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/page_config_dialog.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/page_config_dialog.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/page_config_widget.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/page_config_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/item_delegates.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/item_delegates.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/main_window.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/page_config_widget.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/page_config_widget.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/page_renderer.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/page_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         if parent.isValid() and parent.row() == self.selected_page.row():
             # Cards moved away are treated as if they were deleted
             logger.debug("Cards moved away from the currently shown page, calling card removal handler.")
             self.on_rows_removed(parent, start, end)
         if destination.isValid() and destination.row() == self.selected_page.row():
             # Moved in cards are treated as if they were added
             logger.debug("Cards moved onto the currently shown page, calling card insertion handler.")
-            self.on_rows_inserted(destination, row, row+end-start-1)
+            self.on_rows_inserted(destination, row, row+end-start)
 
     @functools.lru_cache
     def _compute_position_for_image(self, index_row: int, page_type: PageType) -> QPointF:
         """Returns the page-absolute position of the top-left pixel of the given image."""
         card_size = CardSizes.for_page_type(page_type)
         card_height: int = card_size.height.magnitude
         card_width: int = card_size.width.magnitude
```

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/printing_filter_widgets.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/printing_filter_widgets.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/ui/settings_window.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/ui/settings_window.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/units_and_sizes.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/units_and_sizes.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/mtg_proxy_printer/update_checker.py` & `MTGProxyPrinter-0.22.0/mtg_proxy_printer/update_checker.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.21.0/pyproject.toml` & `MTGProxyPrinter-0.22.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,21 @@
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
 ]
 # ijson adds full compatibility with Python 3.11 in version 3.2 (3.1 is really slow on Py3.11).
 # Older Python works fine with ijson >= 3.1
 dependencies = [
     "appdirs >= 1.4.3",
     "PyQt5",
-    "ijson >= 3.1.0",
+    "ijson >= 3.1.0; python_version < '3.11'",
     "ijson >= 3.2.0; python_version >= '3.11'",
     "pint",
     "delegateto == 1.5",
     "PyHamcrest >= 1.8.1",
+    "truststore; python_version >= '3.10'",
+    "certifi; python_version < '3.10'",
 ]
 dynamic = [
     "version",
 ]
 
 [project.urls]
 Homepage = "https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index"
@@ -82,33 +84,40 @@
 legacy_tox_ini = """
 [tox]
 minversion = 3.18
 
 envlist = 
     py3-{unit_tests, test_create_bundle}-{windows, linux}
 
+
 [testenv]
 skip_install = True
 
 
 platform =
     linux: linux
 #    macos: darwin
     windows: win32
 
 
+allowlist_externals =
+    windows: {toxinidir}{/}scripts{/}clean_windows_build.bat
+
+
 deps =
     appdirs >= 1.4.3
     build
     PyQt5
-    ijson >= 3.1.0
+    ijson >= 3.1.0; python_version < '3.11'
     ijson >= 3.2.0; python_version >= '3.11'
     pint
     delegateto == 1.5
     PyHamcrest >= 1.8.1
+    truststore; python_version >= '3.10'
+    certifi; python_version < '3.10'
 
 build_deps =
     setuptools>=61
 
 test_deps =
     pytest
     pytest-cov
@@ -167,25 +176,28 @@
 # Let Qt5 render offscreen, so that running tests don’t open windows or try to access the local system’s display
 # This also prevents unwanted user interactions with the widgets under test
 setenv =
     linux: QT_QPA_PLATFORM = offscreen
     PYTHONDEVMODE = 1
 
 commands =
+    python scripts{/}compile_ui_files.py --full --purge-existing
     python setup_cx_freeze.py build_exe --build-exe build{/}bundle_test
     windows: {toxinidir}{/}scripts{/}clean_windows_build.bat build{/}bundle_test
     {toxinidir}{/}build{/}bundle_test{/}MTGProxyPrinter --test-exit-on-launch
+    -python scripts{/}compile_ui_files.py --purge-existing
 
 
 [testenv:py3-package-{windows,linux}]
 
 deps =
     {[testenv]deps}
     cx_Freeze >= 6.11.1
 
 commands =
+    python scripts{/}compile_ui_files.py --full --purge-existing
     python -m build
     python setup_cx_freeze.py build_exe
     windows: {toxinidir}{/}scripts{/}clean_windows_build.bat
     windows: python setup_cx_freeze.py bdist_msi --skip-build
-
+    -python scripts{/}compile_ui_files.py --purge-existing
 """
```

### Comparing `MTGProxyPrinter-0.21.0/setup.py` & `MTGProxyPrinter-0.22.0/setup.py`

 * *Files identical despite different names*

