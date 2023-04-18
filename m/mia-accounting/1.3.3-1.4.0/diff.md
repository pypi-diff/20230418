# Comparing `tmp/mia-accounting-1.3.3.tar.gz` & `tmp/mia-accounting-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.3.3.tar", last modified: Thu Apr 13 01:57:14 2023, max compression
+gzip compressed data, was "mia-accounting-1.4.0.tar", last modified: Tue Apr 18 01:34:36 2023, max compression
```

## Comparing `mia-accounting-1.3.3.tar` & `mia-accounting-1.4.0.tar`

### file list

```diff
@@ -1,308 +1,304 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.120142 mia-accounting-1.3.3/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.3/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.3/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-13 01:57:14.120142 mia-accounting-1.3.3/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.3.3/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.3/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.3/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.3/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.3/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.3/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.3/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.3/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.unmatched_offset.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-13 01:56:16.000000 mia-accounting-1.3.3/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.3/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.3/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.3/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.3.3/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.3/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-13 01:56:16.000000 mia-accounting-1.3.3/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-13 01:57:14.120142 mia-accounting-1.3.3/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.3/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.3/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3283 2023-04-11 16:41:29.000000 mia-accounting-1.3.3/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.3/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.3/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.3/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.3/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.3/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.3/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.3/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.3/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.3/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.3/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3103 2023-04-10 23:49:07.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.984145 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/unapplied.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.984145 mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/dashboard.html
--rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.040144 mia-accounting-1.3.3/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.3/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.3/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.068143 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.108142 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.108142 mia-accounting-1.3.3/src/accounting/unmatched_offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/unmatched_offset/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/unmatched_offset/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/unmatched_offset/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.112142 mia-accounting-1.3.3/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.3/src/accounting/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.112142 mia-accounting-1.3.3/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11477 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.3.3/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.3.3/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    15396 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-13 00:49:22.000000 mia-accounting-1.3.3/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3898 2023-04-13 01:52:58.000000 mia-accounting-1.3.3/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    13223 2023-04-13 01:30:40.000000 mia-accounting-1.3.3/tests/test_site/lib.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.3/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    13048 2023-04-13 01:52:58.000000 mia-accounting-1.3.3/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.3/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.3.3/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.3.3/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.3.3/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.3.3/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.3/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.3.3/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    27896 2023-04-13 01:30:40.000000 mia-accounting-1.3.3/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     5169 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.947525 mia-accounting-1.4.0/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.4.0/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.4.0/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-18 01:34:36.947525 mia-accounting-1.4.0/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.4.0/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.4.0/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.4.0/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.799528 mia-accounting-1.4.0/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.799528 mia-accounting-1.4.0/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.4.0/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.799528 mia-accounting-1.4.0/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.4.0/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.4.0/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.4.0/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.4.0/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.4.0/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.4.0/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-18 01:33:35.000000 mia-accounting-1.4.0/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.4.0/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.4.0/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.4.0/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.4.0/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.4.0/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-18 01:33:35.000000 mia-accounting-1.4.0/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-18 01:34:36.947525 mia-accounting-1.4.0/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.803527 mia-accounting-1.4.0/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     2995 2023-04-17 15:07:31.000000 mia-accounting-1.4.0/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.803527 mia-accounting-1.4.0/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.4.0/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.4.0/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.803527 mia-accounting-1.4.0/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.4.0/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.4.0/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.803527 mia-accounting-1.4.0/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.4.0/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.4.0/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.803527 mia-accounting-1.4.0/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.4.0/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.4.0/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.4.0/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.803527 mia-accounting-1.4.0/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3283 2023-04-11 16:41:29.000000 mia-accounting-1.4.0/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.807527 mia-accounting-1.4.0/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.4.0/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.4.0/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.4.0/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19883 2023-04-17 23:32:14.000000 mia-accounting-1.4.0/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.4.0/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.807527 mia-accounting-1.4.0/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.4.0/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.4.0/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12987 2023-04-17 23:42:37.000000 mia-accounting-1.4.0/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.4.0/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.4.0/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.4.0/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    33510 2023-04-18 00:13:36.000000 mia-accounting-1.4.0/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.807527 mia-accounting-1.4.0/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.4.0/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.4.0/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.807527 mia-accounting-1.4.0/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.4.0/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.4.0/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.807527 mia-accounting-1.4.0/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.4.0/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.4.0/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.4.0/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.4.0/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.811527 mia-accounting-1.4.0/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.4.0/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.4.0/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.4.0/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.4.0/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.4.0/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.4.0/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.4.0/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8094 2023-04-18 01:09:36.000000 mia-accounting-1.4.0/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5212 2023-04-18 01:09:36.000000 mia-accounting-1.4.0/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8164 2023-04-18 01:14:44.000000 mia-accounting-1.4.0/src/accounting/report/reports/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5193 2023-04-18 01:09:36.000000 mia-accounting-1.4.0/src/accounting/report/reports/unmatched_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.4.0/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.811527 mia-accounting-1.4.0/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.4.0/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.4.0/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7369 2023-04-18 01:18:28.000000 mia-accounting-1.4.0/src/accounting/report/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.4.0/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7865 2023-04-18 01:17:12.000000 mia-accounting-1.4.0/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.4.0/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4472 2023-04-18 01:14:44.000000 mia-accounting-1.4.0/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2262 2023-04-18 01:14:44.000000 mia-accounting-1.4.0/src/accounting/report/utils/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.4.0/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.4.0/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.811527 mia-accounting-1.4.0/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.4.0/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.815527 mia-accounting-1.4.0/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.4.0/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.4.0/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.4.0/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19881 2023-04-17 23:40:32.000000 mia-accounting-1.4.0/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.4.0/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.4.0/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.4.0/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.815527 mia-accounting-1.4.0/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.815527 mia-accounting-1.4.0/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.815527 mia-accounting-1.4.0/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.847527 mia-accounting-1.4.0/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.847527 mia-accounting-1.4.0/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.847527 mia-accounting-1.4.0/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.847527 mia-accounting-1.4.0/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.847527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.847527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.847527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.851527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14492 2023-04-17 23:42:37.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.851527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.851527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.851527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.851527 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.851527 mia-accounting-1.4.0/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.851527 mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.855527 mia-accounting-1.4.0/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.855527 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5600 2023-04-18 00:10:33.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/unapplied.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/unmatched-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.4.0/src/accounting/templates/accounting/report/unmatched.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.855527 mia-accounting-1.4.0/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.4.0/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.4.0/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.855527 mia-accounting-1.4.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.4.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.4.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.855527 mia-accounting-1.4.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.4.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.4.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.859526 mia-accounting-1.4.0/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.4.0/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.4.0/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.4.0/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.4.0/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.4.0/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.4.0/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.4.0/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.4.0/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.4.0/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.859526 mia-accounting-1.4.0/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-18 01:34:36.000000 mia-accounting-1.4.0/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11408 2023-04-18 01:34:36.000000 mia-accounting-1.4.0/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-18 01:34:36.000000 mia-accounting-1.4.0/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-18 01:34:36.000000 mia-accounting-1.4.0/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-18 01:34:36.000000 mia-accounting-1.4.0/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.859526 mia-accounting-1.4.0/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.4.0/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.4.0/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.4.0/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-13 01:09:51.000000 mia-accounting-1.4.0/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-13 01:09:51.000000 mia-accounting-1.4.0/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.4.0/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-13 01:09:51.000000 mia-accounting-1.4.0/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17862 2023-04-18 01:19:22.000000 mia-accounting-1.4.0/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.863526 mia-accounting-1.4.0/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-13 00:49:22.000000 mia-accounting-1.4.0/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3898 2023-04-13 01:52:58.000000 mia-accounting-1.4.0/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13223 2023-04-13 01:30:40.000000 mia-accounting-1.4.0/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.4.0/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13048 2023-04-13 01:52:58.000000 mia-accounting-1.4.0/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.863526 mia-accounting-1.4.0/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.4.0/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.863526 mia-accounting-1.4.0/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.4.0/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.4.0/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.4.0/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.4.0/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.863526 mia-accounting-1.4.0/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.4.0/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.4.0/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.915526 mia-accounting-1.4.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.4.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.4.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.795528 mia-accounting-1.4.0/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-18 01:34:36.947525 mia-accounting-1.4.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.4.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.4.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.4.0/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.4.0/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5169 2023-04-13 01:09:51.000000 mia-accounting-1.4.0/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-13 01:09:51.000000 mia-accounting-1.4.0/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.3.3/LICENSE` & `mia-accounting-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/MANIFEST.in` & `mia-accounting-1.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/PKG-INFO` & `mia-accounting-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.3
+Version: 1.4.0
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.3.3/README.rst` & `mia-accounting-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/Makefile` & `mia-accounting-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/make.bat` & `mia-accounting-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.account.rst` & `mia-accounting-1.4.0/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.base_account.rst` & `mia-accounting-1.4.0/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.currency.rst` & `mia-accounting-1.4.0/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.4.0/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.4.0/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.4.0/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.option.rst` & `mia-accounting-1.4.0/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.report.period.rst` & `mia-accounting-1.4.0/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.report.reports.rst` & `mia-accounting-1.4.0/docs/source/accounting.report.reports.rst`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,30 @@
 ----------------------------------------------------
 
 .. automodule:: accounting.report.reports.unapplied_accounts
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.report.reports.unmatched module
+------------------------------------------
+
+.. automodule:: accounting.report.reports.unmatched
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+accounting.report.reports.unmatched\_accounts module
+----------------------------------------------------
+
+.. automodule:: accounting.report.reports.unmatched_accounts
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: accounting.report.reports
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.3.3/docs/source/accounting.report.rst` & `mia-accounting-1.4.0/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/accounting.report.utils.rst` & `mia-accounting-1.4.0/docs/source/accounting.report.utils.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 ------------------------------------------
 
 .. automodule:: accounting.report.utils.csv_export
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.report.utils.offset\_matcher module
+----------------------------------------------
+
+.. automodule:: accounting.report.utils.offset_matcher
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 accounting.report.utils.option\_link module
 -------------------------------------------
 
 .. automodule:: accounting.report.utils.option_link
    :members:
    :undoc-members:
    :show-inheritance:
@@ -56,14 +64,22 @@
 ----------------------------------------
 
 .. automodule:: accounting.report.utils.unapplied
    :members:
    :undoc-members:
    :show-inheritance:
 
+accounting.report.utils.unmatched module
+----------------------------------------
+
+.. automodule:: accounting.report.utils.unmatched
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 accounting.report.utils.urls module
 -----------------------------------
 
 .. automodule:: accounting.report.utils.urls
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.3.3/docs/source/accounting.rst` & `mia-accounting-1.4.0/docs/source/accounting.rst`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
    accounting.account
    accounting.base_account
    accounting.currency
    accounting.journal_entry
    accounting.option
    accounting.report
-   accounting.unmatched_offset
    accounting.utils
 
 Submodules
 ----------
 
 accounting.commands module
 --------------------------
```

### Comparing `mia-accounting-1.3.3/docs/source/accounting.utils.rst` & `mia-accounting-1.4.0/docs/source/accounting.utils.rst`

 * *Files 6% similar despite different names*

```diff
@@ -48,22 +48,14 @@
 -------------------------------------
 
 .. automodule:: accounting.utils.offset_alias
    :members:
    :undoc-members:
    :show-inheritance:
 
-accounting.utils.offset\_matcher module
----------------------------------------
-
-.. automodule:: accounting.utils.offset_matcher
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 accounting.utils.options module
 -------------------------------
 
 .. automodule:: accounting.utils.options
    :members:
    :undoc-members:
    :show-inheritance:
@@ -104,22 +96,14 @@
 -----------------------------------
 
 .. automodule:: accounting.utils.strip_text
    :members:
    :undoc-members:
    :show-inheritance:
 
-accounting.utils.unapplied module
----------------------------------
-
-.. automodule:: accounting.utils.unapplied
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 accounting.utils.user module
 ----------------------------
 
 .. automodule:: accounting.utils.user
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.3.3/docs/source/conf.py` & `mia-accounting-1.4.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.3.3'
+release = '1.4.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.3.3/docs/source/examples.rst` & `mia-accounting-1.4.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/history.rst` & `mia-accounting-1.4.0/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/docs/source/intro.rst` & `mia-accounting-1.4.0/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/pyproject.toml` & `mia-accounting-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.3.3"
+version = "1.4.0"
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
```

### Comparing `mia-accounting-1.3.3/src/accounting/__init__.py` & `mia-accounting-1.4.0/src/accounting/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,11 +87,8 @@
 
     from . import report
     report.init_app(app, url_prefix)
 
     from . import option
     option.init_app(bp)
 
-    from . import unmatched_offset
-    unmatched_offset.init_app(bp)
-
     app.register_blueprint(bp, url_prefix=url_prefix)
```

### Comparing `mia-accounting-1.3.3/src/accounting/account/__init__.py` & `mia-accounting-1.4.0/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/account/commands.py` & `mia-accounting-1.4.0/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/account/converters.py` & `mia-accounting-1.4.0/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/account/forms.py` & `mia-accounting-1.4.0/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/account/queries.py` & `mia-accounting-1.4.0/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/account/views.py` & `mia-accounting-1.4.0/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/base_account/__init__.py` & `mia-accounting-1.4.0/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/base_account/commands.py` & `mia-accounting-1.4.0/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/base_account/converters.py` & `mia-accounting-1.4.0/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/base_account/queries.py` & `mia-accounting-1.4.0/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/base_account/views.py` & `mia-accounting-1.4.0/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/commands.py` & `mia-accounting-1.4.0/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/currency/__init__.py` & `mia-accounting-1.4.0/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/currency/commands.py` & `mia-accounting-1.4.0/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/currency/converters.py` & `mia-accounting-1.4.0/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/currency/forms.py` & `mia-accounting-1.4.0/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/currency/queries.py` & `mia-accounting-1.4.0/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/currency/views.py` & `mia-accounting-1.4.0/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/data/base_accounts.csv` & `mia-accounting-1.4.0/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/forms.py` & `mia-accounting-1.4.0/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/converters.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/forms/line_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,14 +264,27 @@
         """
         super().__init__(*args, **kwargs)
         from .journal_entry import JournalEntryForm
         self.journal_entry_form: JournalEntryForm | None = None
         """The source journal entry form."""
 
     @property
+    def account_title(self) -> str:
+        """Returns the title of the account.
+
+        :return: The title of the account.
+        """
+        if self.account_code.data is None:
+            return ""
+        account: Account | None = Account.find_by_code(self.account_code.data)
+        if account is None:
+            return ""
+        return account.title
+
+    @property
     def account_text(self) -> str:
         """Returns the text representation of the account.
 
         :return: The text representation of the account.
         """
         if self.account_code.data is None:
             return ""
```

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/utils/account_option.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
         :param account: The account.
         """
         self.id: str = account.id
         """The account ID."""
         self.code: str = account.code
         """The account code."""
+        self.title: str = account.title
+        """The account title."""
         self.query_values: list[str] = account.query_values
         """The values to be queried."""
         self.__str: str = str(account)
         """The string representation of the account option."""
         self.is_in_use: bool = False
         """True if this account is in use, or False otherwise."""
         self.is_need_offset: bool = account.is_need_offset
```

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/utils/description_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,22 @@
     def __str__(self) -> str:
         """Returns the string representation of the account.
 
         :return: The string representation of the account.
         """
         return str(self.__account)
 
+    @property
+    def title(self) -> str:
+        """Returns the account title.
+
+        :return: The account title.
+        """
+        return self.__account.title
+
     def add_freq(self, freq: int) -> None:
         """Adds the frequency of an account.
 
         :param freq: The frequency of the tag name with the account.
         :return: None.
         """
         self.freq = self.freq + freq
```

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/journal_entry/views.py` & `mia-accounting-1.4.0/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/locale.py` & `mia-accounting-1.4.0/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/models.py` & `mia-accounting-1.4.0/src/accounting/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -738,23 +738,45 @@
 
     @property
     def debit(self) -> Decimal | None:
         """Returns the debit amount.
 
         :return: The debit amount, or None if this is not a debit line item.
         """
-        return self.amount if self.is_debit else None
+        if not hasattr(self, "__debit"):
+            setattr(self, "__debit", self.amount if self.is_debit else None)
+        return getattr(self, "__debit")
+
+    @debit.setter
+    def debit(self, debit: Decimal | None) -> None:
+        """Sets the debit amount.
+
+        :param debit: The debit amount.
+        :return: None.
+        """
+        setattr(self, "__debit", debit)
 
     @property
     def credit(self) -> Decimal | None:
         """Returns the credit amount.
 
         :return: The credit amount, or None if this is not a credit line item.
         """
-        return None if self.is_debit else self.amount
+        if not hasattr(self, "__credit"):
+            setattr(self, "__credit", None if self.is_debit else self.amount)
+        return getattr(self, "__credit")
+
+    @credit.setter
+    def credit(self, credit: Decimal | None) -> None:
+        """Sets the credit amount.
+
+        :param credit: The credit amount.
+        :return: None.
+        """
+        setattr(self, "__credit", credit)
 
     @property
     def net_balance(self) -> Decimal:
         """Returns the net balance.
 
         :return: The net balance.
         """
@@ -770,14 +792,33 @@
 
         :param net_balance: The net balance.
         :return: None.
         """
         setattr(self, "__net_balance", net_balance)
 
     @property
+    def balance(self) -> Decimal:
+        """Returns the net balance.
+
+        :return: The net balance.
+        """
+        if not hasattr(self, "__balance"):
+            setattr(self, "__balance", Decimal("0"))
+        return getattr(self, "__balance")
+
+    @balance.setter
+    def balance(self, balance: Decimal) -> None:
+        """Sets the net balance.
+
+        :param balance: The net balance.
+        :return: None.
+        """
+        setattr(self, "__balance", balance)
+
+    @property
     def offsets(self) -> list[t.Self]:
         """Returns the offset items.
 
         :return: The offset items.
         """
         if not hasattr(self, "__offsets"):
             cls: t.Type[t.Self] = self.__class__
@@ -785,14 +826,34 @@
                 .filter(JournalEntryLineItem.original_line_item_id == self.id)\
                 .order_by(JournalEntry.date, JournalEntry.no,
                           cls.is_debit, cls.no).all()
             setattr(self, "__offsets", offsets)
         return getattr(self, "__offsets")
 
     @property
+    def is_offset(self) -> bool:
+        """Returns whether the line item is an offset.
+
+        :return: True if the line item is an offset, or False otherwise.
+        """
+        if not hasattr(self, "__is_offset"):
+            setattr(self, "__is_offset", False)
+        return getattr(self, "__is_offset")
+
+    @is_offset.setter
+    def is_offset(self, is_offset: bool) -> None:
+        """Sets whether the line item is an offset.
+
+        :param is_offset: True if the line item is an offset, or False
+            otherwise.
+        :return: None.
+        """
+        setattr(self, "__is_offset", is_offset)
+
+    @property
     def match(self) -> t.Self | None:
         """Returns the match of the line item.
 
         :return: The match of the line item.
         """
         if not hasattr(self, "__match"):
             setattr(self, "__match", None)
@@ -818,14 +879,15 @@
             frac: Decimal = (value - whole).normalize()
             return str(whole) + str(abs(frac))[1:]
 
         return ["{}/{}/{}".format(self.journal_entry.date.year,
                                   self.journal_entry.date.month,
                                   self.journal_entry.date.day),
                 "" if self.description is None else self.description,
+                str(self.account),
                 format_amount(self.amount)]
 
 
 class Option(db.Model):
     """An option."""
     __tablename__ = "accounting_options"
     """The table name."""
```

### Comparing `mia-accounting-1.3.3/src/accounting/option/__init__.py` & `mia-accounting-1.4.0/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/option/forms.py` & `mia-accounting-1.4.0/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/option/views.py` & `mia-accounting-1.4.0/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/__init__.py` & `mia-accounting-1.4.0/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/converters.py` & `mia-accounting-1.4.0/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/__init__.py` & `mia-accounting-1.4.0/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/chooser.py` & `mia-accounting-1.4.0/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/description.py` & `mia-accounting-1.4.0/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/month_end.py` & `mia-accounting-1.4.0/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/parser.py` & `mia-accounting-1.4.0/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/period.py` & `mia-accounting-1.4.0/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.4.0/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/period/specification.py` & `mia-accounting-1.4.0/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/__init__.py` & `mia-accounting-1.4.0/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.4.0/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.4.0/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.4.0/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/journal.py` & `mia-accounting-1.4.0/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/ledger.py` & `mia-accounting-1.4.0/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/search.py` & `mia-accounting-1.4.0/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.4.0/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.4.0/src/accounting/report/reports/unmatched.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,114 @@
 # The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/7
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/17
 
 #  Copyright (c) 2023 imacat.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The unapplied original line items.
+"""The unmatched offsets.
 
 """
 from datetime import date
 from decimal import Decimal
 
 from flask import render_template, Response
+from flask_babel import LazyString
 
 from accounting.locale import gettext
-from accounting.models import Account, JournalEntryLineItem
+from accounting.models import Currency, Account, JournalEntryLineItem
 from accounting.report.utils.base_page_params import BasePageParams
 from accounting.report.utils.base_report import BaseReport
 from accounting.report.utils.csv_export import BaseCSVRow, csv_download
+from accounting.report.utils.offset_matcher import OffsetMatcher, OffsetPair
 from accounting.report.utils.option_link import OptionLink
 from accounting.report.utils.report_chooser import ReportChooser
 from accounting.report.utils.report_type import ReportType
-from accounting.report.utils.unapplied import get_accounts_with_unapplied
-from accounting.report.utils.urls import unapplied_url
-from accounting.utils.offset_matcher import OffsetMatcher
+from accounting.report.utils.unmatched import get_accounts_with_unmatched
+from accounting.report.utils.urls import unmatched_url
 from accounting.utils.pagination import Pagination
-from accounting.utils.permission import can_edit
 
 
 class CSVRow(BaseCSVRow):
     """A row in the CSV."""
 
     def __init__(self, journal_entry_date: str | date, currency: str,
-                 description: str | None, amount: str | Decimal,
-                 net_balance: str | Decimal):
+                 description: str | None, debit: str | Decimal,
+                 credit: str | Decimal, balance: str | Decimal):
         """Constructs a row in the CSV.
 
         :param journal_entry_date: The journal entry date.
         :param currency: The currency.
         :param description: The description.
-        :param amount: The amount.
-        :param net_balance: The net balance.
+        :param debit: The debit amount.
+        :param credit: The credit amount.
+        :param balance: The balance.
         """
         self.date: str | date = journal_entry_date
         """The date."""
         self.currency: str = currency
         """The currency."""
         self.description: str | None = description
         """The description."""
-        self.amount: str | Decimal = amount
-        """The amount."""
-        self.net_balance: str | Decimal = net_balance
-        """The net balance."""
+        self.debit: str | Decimal | None = debit
+        """The debit amount."""
+        self.credit: str | Decimal | None = credit
+        """The credit amount."""
+        self.balance: str | Decimal = balance
+        """The balance."""
 
     @property
     def values(self) -> list[str | date | Decimal | None]:
         """Returns the values of the row.
 
         :return: The values of the row.
         """
-        return [self.date, self.currency, self.description, self.amount,
-                self.net_balance]
+        return [self.date, self.currency, self.description, self.debit,
+                self.credit, self.balance]
 
 
 class PageParams(BasePageParams):
     """The HTML page parameters."""
 
-    def __init__(self, account: Account,
-                 is_mark_matches: bool,
+    def __init__(self, currency: Currency,
+                 account: Account,
+                 match_status: str | LazyString,
+                 matched_pairs: list[OffsetPair],
                  pagination: Pagination[JournalEntryLineItem],
                  line_items: list[JournalEntryLineItem]):
         """Constructs the HTML page parameters.
 
+        :param currency: The currency.
         :param account: The account.
-        :param is_mark_matches: Whether to mark the matched offsets.
+        :param match_status: The match status message.
+        :param matched_pairs: A list of matched pairs.
         :param pagination: The pagination.
         :param line_items: The line items.
         """
+        self.currency: Currency = currency
+        """The currency."""
         self.account: Account = account
         """The account."""
+        self.match_status: str | LazyString = match_status
+        """The match status message."""
+        self.matched_pairs: list[OffsetPair] = matched_pairs
+        """A list of matched pairs."""
         self.pagination: Pagination[JournalEntryLineItem] = pagination
         """The pagination."""
         self.line_items: list[JournalEntryLineItem] = line_items
         """The line items."""
-        self.is_mark_matches: bool = is_mark_matches
-        """Whether to mark the matched offsets."""
 
     @property
     def has_data(self) -> bool:
         """Returns whether there is any data on the page.
 
         :return: True if there is any data, or False otherwise.
         """
@@ -105,81 +116,99 @@
 
     @property
     def report_chooser(self) -> ReportChooser:
         """Returns the report chooser.
 
         :return: The report chooser.
         """
-        return ReportChooser(ReportType.UNAPPLIED,
+        return ReportChooser(ReportType.UNMATCHED, currency=self.currency,
                              account=self.account)
 
     @property
+    def currency_options(self) -> list[OptionLink]:
+        """Returns the currency options.
+
+        :return: The currency options.
+        """
+        return self._get_currency_options(
+            lambda x: unmatched_url(x, self.account), self.currency)
+
+    @property
     def account_options(self) -> list[OptionLink]:
         """Returns the account options.
 
         :return: The account options.
         """
-        options: list[OptionLink] = [OptionLink(gettext("Accounts"),
-                                                unapplied_url(None),
-                                                False)]
-        options.extend([OptionLink(str(x),
-                                   unapplied_url(x),
-                                   x.id == self.account.id)
-                        for x in get_accounts_with_unapplied()])
+        options: list[OptionLink] \
+            = [OptionLink(gettext("Accounts"),
+                          unmatched_url(self.currency, None),
+                          False)]
+        options.extend(
+            [OptionLink(str(x), unmatched_url(self.currency, x),
+                        x.id == self.account.id)
+             for x in get_accounts_with_unmatched(self.currency)])
         return options
 
 
 def get_csv_rows(line_items: list[JournalEntryLineItem]) -> list[CSVRow]:
     """Composes and returns the CSV rows from the line items.
 
     :param line_items: The line items.
     :return: The CSV rows.
     """
     rows: list[CSVRow] = [CSVRow(gettext("Date"), gettext("Currency"),
-                                 gettext("Description"), gettext("Amount"),
-                                 gettext("Net Balance"))]
+                                 gettext("Description"), gettext("Debit"),
+                                 gettext("Credit"), gettext("Balance"))]
     rows.extend([CSVRow(x.journal_entry.date, x.currency.code,
-                        x.description, x.amount, x.net_balance)
+                        x.description, x.debit, x.credit, x.balance)
                  for x in line_items])
     return rows
 
 
-class UnappliedOriginalLineItems(BaseReport):
-    """The unapplied original line items."""
+class UnmatchedOffsets(BaseReport):
+    """The unmatched offsets."""
 
-    def __init__(self, account: Account):
-        """Constructs the unapplied original line items.
+    def __init__(self, currency: Currency, account: Account):
+        """Constructs the unmatched offsets.
 
+        :param currency: The currency.
         :param account: The account.
         """
+        self.__currency: Currency = currency
+        """The currency."""
         self.__account: Account = account
         """The account."""
-        offset_matcher: OffsetMatcher = OffsetMatcher(self.__account)
+        offset_matcher: OffsetMatcher \
+            = OffsetMatcher(self.__currency, self.__account)
         self.__line_items: list[JournalEntryLineItem] \
-            = offset_matcher.unapplied
+            = offset_matcher.line_items
         """The line items."""
-        self.__is_mark_matches: bool \
-            = can_edit() and len(offset_matcher.unmatched_offsets) > 0
-        """Whether to mark the matched offsets."""
+        self.__match_status: str | LazyString = offset_matcher.status
+        """The match status message."""
+        self.__matched_pairs: list[OffsetPair] = offset_matcher.matched_pairs
+        """A list of matched pairs."""
 
     def csv(self) -> Response:
         """Returns the report as CSV for download.
 
         :return: The response of the report for download.
         """
-        filename: str = f"unapplied-{self.__account.code}.csv"
+        filename: str = "unmatched-{currency}-{account}.csv"\
+            .format(currency=self.__currency.code, account=self.__account.code)
         return csv_download(filename, get_csv_rows(self.__line_items))
 
     def html(self) -> str:
         """Composes and returns the report as HTML.
 
         :return: The report as HTML.
         """
         pagination: Pagination[JournalEntryLineItem] \
             = Pagination[JournalEntryLineItem](self.__line_items,
                                                is_reversed=True)
-        params: PageParams = PageParams(account=self.__account,
-                                        is_mark_matches=self.__is_mark_matches,
+        params: PageParams = PageParams(currency=self.__currency,
+                                        account=self.__account,
+                                        match_status=self.__match_status,
+                                        matched_pairs=self.__matched_pairs,
                                         pagination=pagination,
                                         line_items=pagination.list)
-        return render_template("accounting/report/unapplied.html",
+        return render_template("accounting/report/unmatched.html",
                                report=params)
```

### Comparing `mia-accounting-1.3.3/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.4.0/src/accounting/report/reports/unapplied_accounts.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 from datetime import date
 from decimal import Decimal
 
 from flask import render_template, Response
 
 from accounting.locale import gettext
-from accounting.models import Account
+from accounting.models import Currency, Account
 from accounting.report.utils.base_page_params import BasePageParams
 from accounting.report.utils.base_report import BaseReport
 from accounting.report.utils.csv_export import BaseCSVRow, csv_download
 from accounting.report.utils.option_link import OptionLink
 from accounting.report.utils.report_chooser import ReportChooser
 from accounting.report.utils.report_type import ReportType
 from accounting.report.utils.unapplied import get_accounts_with_unapplied
@@ -56,19 +56,22 @@
         """
         return [self.account, self.count]
 
 
 class PageParams(BasePageParams):
     """The HTML page parameters."""
 
-    def __init__(self, accounts: list[Account]):
+    def __init__(self, currency: Currency, accounts: list[Account]):
         """Constructs the HTML page parameters.
 
+        :param currency: The currency.
         :param accounts: The accounts.
         """
+        self.currency: Currency = currency
+        """The currency."""
         self.accounts: list[Account] = accounts
         """The accounts."""
 
     @property
     def has_data(self) -> bool:
         """Returns whether there is any data on the page.
 
@@ -78,29 +81,39 @@
 
     @property
     def report_chooser(self) -> ReportChooser:
         """Returns the report chooser.
 
         :return: The report chooser.
         """
-        return ReportChooser(ReportType.UNAPPLIED)
+        return ReportChooser(ReportType.UNAPPLIED, currency=self.currency,
+                             account=None)
+
+    @property
+    def currency_options(self) -> list[OptionLink]:
+        """Returns the currency options.
+
+        :return: The currency options.
+        """
+        return self._get_currency_options(lambda x: unapplied_url(x, None),
+                                          self.currency)
 
     @property
     def account_options(self) -> list[OptionLink]:
         """Returns the account options.
 
         :return: The account options.
         """
-        options: list[OptionLink] = [OptionLink(gettext("Accounts"),
-                                                unapplied_url(None),
-                                                True)]
-        options.extend([OptionLink(str(x),
-                                   unapplied_url(x),
-                                   False)
-                        for x in self.accounts])
+        options: list[OptionLink] \
+            = [OptionLink(gettext("Accounts"),
+                          unapplied_url(self.currency, None),
+                          True)]
+        options.extend(
+            [OptionLink(str(x), unapplied_url(self.currency, x), False)
+             for x in self.accounts])
         return options
 
 
 def get_csv_rows(accounts: list[Account]) -> list[CSVRow]:
     """Composes and returns the CSV rows from the line items.
 
     :param accounts: The accounts.
@@ -111,17 +124,22 @@
                  for x in accounts])
     return rows
 
 
 class AccountsWithUnappliedOriginalLineItems(BaseReport):
     """The accounts with unapplied original line items."""
 
-    def __init__(self):
-        """Constructs the outstanding balances."""
-        self.__accounts: list[Account] = get_accounts_with_unapplied()
+    def __init__(self, currency: Currency):
+        """Constructs the outstanding balances.
+
+        :param currency: The currency.
+        """
+        self.__currency: Currency = currency
+        """The currency."""
+        self.__accounts: list[Account] = get_accounts_with_unapplied(currency)
         """The accounts."""
 
     def csv(self) -> Response:
         """Returns the report as CSV for download.
 
         :return: The response of the report for download.
         """
@@ -130,8 +148,9 @@
 
     def html(self) -> str:
         """Composes and returns the report as HTML.
 
         :return: The report as HTML.
         """
         return render_template("accounting/report/unapplied-accounts.html",
-                               report=PageParams(accounts=self.__accounts))
+                               report=PageParams(currency=self.__currency,
+                                                 accounts=self.__accounts))
```

### Comparing `mia-accounting-1.3.3/src/accounting/report/template_filters.py` & `mia-accounting-1.4.0/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/__init__.py` & `mia-accounting-1.4.0/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.4.0/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/base_report.py` & `mia-accounting-1.4.0/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.4.0/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/option_link.py` & `mia-accounting-1.4.0/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.4.0/src/accounting/report/utils/report_chooser.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 
 from accounting import db
 from accounting.locale import gettext
 from accounting.models import Currency, Account
 from accounting.report.period import Period, get_period
 from accounting.template_globals import default_currency_code
 from accounting.utils.current_account import CurrentAccount
+from accounting.utils.permission import can_edit
 from .option_link import OptionLink
 from .report_type import ReportType
 from .urls import journal_url, ledger_url, income_expenses_url, \
-    trial_balance_url, income_statement_url, balance_sheet_url, unapplied_url
+    trial_balance_url, income_statement_url, balance_sheet_url, \
+    unapplied_url, unmatched_url
 
 
 class ReportChooser:
     """The report chooser."""
 
     def __init__(self, active_report: ReportType,
                  period: Period | None = None,
@@ -71,14 +73,16 @@
         self.__reports.append(self.__income_expenses)
         self.__reports.append(self.__ledger)
         self.__reports.append(self.__journal)
         self.__reports.append(self.__trial_balance)
         self.__reports.append(self.__income_statement)
         self.__reports.append(self.__balance_sheet)
         self.__reports.append(self.__unapplied)
+        if can_edit():
+            self.__reports.append(self.__unmatched)
         for report in self.__reports:
             if report.is_active:
                 self.current_report = report.title
         if self.is_search:
             self.current_report = gettext("Search")
 
     @property
@@ -156,22 +160,39 @@
     def __unapplied(self) -> OptionLink:
         """Returns the unapplied original line items.
 
         :return: The unapplied original line items.
         """
         account: Account = self.__account
         if not account.is_need_offset:
-            return OptionLink(gettext("Unapplied Original Line Items"),
-                              unapplied_url(None),
+            return OptionLink(gettext("Unapplied Items"),
+                              unapplied_url(self.__currency, None),
                               self.__active_report == ReportType.UNAPPLIED,
                               fa_icon="fa-solid fa-link-slash")
-        return OptionLink(gettext("Unapplied Original Line Items"),
-                          unapplied_url(account),
+        return OptionLink(gettext("Unapplied Items"),
+                          unapplied_url(self.__currency, self.__account),
                           self.__active_report == ReportType.UNAPPLIED,
                           fa_icon="fa-solid fa-link-slash")
 
+    @property
+    def __unmatched(self) -> OptionLink:
+        """Returns the unmatched offsets.
+
+        :return: The unmatched offsets.
+        """
+        account: Account = self.__account
+        if not account.is_need_offset:
+            return OptionLink(gettext("Unmatched Offsets"),
+                              unmatched_url(self.__currency, None),
+                              self.__active_report == ReportType.UNMATCHED,
+                              fa_icon="fa-solid fa-file-circle-question")
+        return OptionLink(gettext("Unmatched Offsets"),
+                          unmatched_url(self.__currency, self.__account),
+                          self.__active_report == ReportType.UNMATCHED,
+                          fa_icon="fa-solid fa-file-circle-question")
+
     def __iter__(self) -> t.Iterator[OptionLink]:
         """Returns the iteration of the reports.
 
         :return: The iteration of the reports.
         """
         return iter(self.__reports)
```

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/report_type.py` & `mia-accounting-1.4.0/src/accounting/report/utils/report_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,9 +32,11 @@
     """The trial balance."""
     INCOME_STATEMENT: str = "income-statement"
     """The income statement."""
     BALANCE_SHEET: str = "balance-sheet"
     """The balance sheet."""
     UNAPPLIED: str = "unapplied"
     """The unapplied original line items."""
+    UNMATCHED: str = "unmatched"
+    """The unmatched offsets."""
     SEARCH: str = "search"
     """The search."""
```

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.4.0/src/accounting/report/utils/unmatched.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,53 @@
 # The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/7
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/8
 
 #  Copyright (c) 2023 imacat.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The unapplied original line item utilities.
+"""The unmatched offset utilities.
 
 """
 import sqlalchemy as sa
 
 from accounting import db
-from accounting.models import Account, JournalEntryLineItem
+from accounting.models import Currency, Account, JournalEntry, \
+    JournalEntryLineItem
 from accounting.utils.cast import be
-from accounting.utils.offset_alias import offset_alias
 
 
-def get_accounts_with_unapplied() -> list[Account]:
-    """Returns the accounts with unapplied original line items.
+def get_accounts_with_unmatched(currency: Currency) -> list[Account]:
+    """Returns the accounts with unmatched offsets.
 
-    :return: The accounts with unapplied original line items.
+    :param currency: The currency.
+    :return: The accounts with unmatched offsets, with the "count" property set
+        to the number of unmatched offsets.
     """
-    offset: sa.Alias = offset_alias()
-    net_balance: sa.Label \
-        = (JournalEntryLineItem.amount
-           + sa.func.sum(sa.case(
-                (be(offset.c.is_debit == JournalEntryLineItem.is_debit),
-                 offset.c.amount),
-                else_=-offset.c.amount))).label("net_balance")
-    select_unapplied: sa.Select \
-        = sa.select(JournalEntryLineItem.id)\
-        .join(Account)\
-        .join(offset, be(JournalEntryLineItem.id
-                         == offset.c.original_line_item_id),
-              isouter=True)\
-        .filter(Account.is_need_offset,
-                sa.or_(sa.and_(Account.base_code.startswith("2"),
-                               sa.not_(JournalEntryLineItem.is_debit)),
-                       sa.and_(Account.base_code.startswith("1"),
-                               JournalEntryLineItem.is_debit)))\
-        .group_by(JournalEntryLineItem.id)\
-        .having(sa.or_(sa.func.count(offset.c.id) == 0, net_balance != 0))
-
     count_func: sa.Label \
         = sa.func.count(JournalEntryLineItem.id).label("count")
     select: sa.Select = sa.select(Account.id, count_func)\
-        .join(JournalEntryLineItem, isouter=True)\
-        .filter(JournalEntryLineItem.id.in_(select_unapplied))\
+        .select_from(Account)\
+        .join(JournalEntryLineItem, isouter=True).join(JournalEntry)\
+        .filter(Account.is_need_offset,
+                be(JournalEntryLineItem.currency_code == currency.code),
+                JournalEntryLineItem.original_line_item_id.is_(None),
+                sa.or_(sa.and_(Account.base_code.startswith("2"),
+                               JournalEntryLineItem.is_debit),
+                       sa.and_(Account.base_code.startswith("1"),
+                               sa.not_(JournalEntryLineItem.is_debit))))\
         .group_by(Account.id)\
         .having(count_func > 0)
     counts: dict[int, int] \
         = {x.id: x.count for x in db.session.execute(select)}
     accounts: list[Account] = Account.query.filter(Account.id.in_(counts))\
         .order_by(Account.base_code, Account.no).all()
     for account in accounts:
```

### Comparing `mia-accounting-1.3.3/src/accounting/report/utils/urls.py` & `mia-accounting-1.4.0/src/accounting/report/utils/urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -109,17 +109,39 @@
     """
     if currency.code == default_currency_code() and period.is_default:
         return url_for("accounting-report.balance-sheet-default")
     return url_for("accounting-report.balance-sheet",
                    currency=currency, period=period)
 
 
-def unapplied_url(account: Account | None) -> str:
+def unapplied_url(currency: Currency, account: Account | None) -> str:
     """Returns the URL of the unapplied original line items.
 
+    :param currency: The currency.
     :param account: The account, or None to list the accounts with unapplied
         original line items.
     :return: The URL of the unapplied original line items.
     """
     if account is None:
-        return url_for("accounting-report.unapplied-default")
-    return url_for("accounting-report.unapplied", account=account)
+        if currency.code == default_currency_code():
+            return url_for("accounting-report.unapplied-accounts-default")
+        return url_for("accounting-report.unapplied-accounts",
+                       currency=currency)
+    return url_for("accounting-report.unapplied",
+                   currency=currency, account=account)
+
+
+def unmatched_url(currency: Currency, account: Account | None) -> str:
+    """Returns the URL of the unmatched offset line items.
+
+    :param currency: The currency.
+    :param account: The account, or None to list the accounts with unmatched
+        offset line items.
+    :return: The URL of the unmatched offset line items.
+    """
+    if account is None:
+        if currency.code == default_currency_code():
+            return url_for("accounting-report.unmatched-accounts-default")
+        return url_for("accounting-report.unmatched-accounts",
+                       currency=currency)
+    return url_for("accounting-report.unmatched",
+                   currency=currency, account=account)
```

### Comparing `mia-accounting-1.3.3/src/accounting/static/css/style.css` & `mia-accounting-1.4.0/src/accounting/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,18 @@
     background-color: #e9ecef;
 }
 
 /** The toolbar */
 .accounting-toolbar {
     display: flex;
 }
+.accounting-toolbar-accounts {
+    max-height: 20rem;
+    overflow-y: scroll;
+}
 .accounting-toolbar .input-group > .input-group-text {
     padding: 0;
     background-color: transparent;
     color: inherit;
     border: 0;
 }
 .accounting-toolbar .input-group > .input-group-text > button {
@@ -318,23 +322,33 @@
 .accounting-balance-sheet-account {
     margin-left: 0.5rem;
 }
 .accounting-balance-sheet-total .accounting-amount, .accounting-balance-sheet-subtotal, .accounting-amount {
     font-style: italic;
 }
 .accounting-unapplied-table .accounting-report-table-row {
-    grid-template-columns: 1fr 1fr 5fr 1fr 1fr;
+    grid-template-columns: 1fr 5fr 1fr 1fr;
 }
 .accounting-unapplied-account-table .accounting-report-table-row {
     display: flex;
     justify-content: space-between;
 }
 .accounting-unapplied-account-table .accounting-report-table-header .accounting-report-table-row {
     display: block;
 }
+.accounting-unmatched-table .accounting-report-table-row {
+    grid-template-columns: 1fr 5fr 1fr 1fr 1fr;
+}
+.accounting-unmatched-account-table .accounting-report-table-row {
+    display: flex;
+    justify-content: space-between;
+}
+.accounting-unmatched-account-table .accounting-report-table-header .accounting-report-table-row {
+    display: block;
+}
 
 /* The accounting report */
 .accounting-mobile-journal-credit {
     padding-left: 1rem;
 }
 
 /* The description editor */
```

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/account-form.js` & `mia-accounting-1.4.0/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/account-order.js` & `mia-accounting-1.4.0/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/currency-form.js` & `mia-accounting-1.4.0/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/description-editor.js` & `mia-accounting-1.4.0/src/accounting/static/js/description-editor.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -360,20 +360,21 @@
     isConfirmedAccount = false;
 
     /**
      * Constructs an account option in the description editor.
      *
      * @param editor {DescriptionEditor} the description editor
      * @param code {string} the account code
+     * @param title {string} the account title
      * @param text {string} the account text
      * @param isNeedOffset {boolean} true if the line items in the account needs offset, or false otherwise
      * @param button {HTMLButtonElement} the account button
      */
-    constructor(editor, code, text, isNeedOffset, button) {
-        super(code, text, isNeedOffset);
+    constructor(editor, code, title, text, isNeedOffset, button) {
+        super(code, title, text, isNeedOffset);
         this.#element = button;
         this.#element.onclick = () => editor.selectAccount(this);
     }
 
     /**
      * Sets whether the option is shown.
      *
@@ -420,15 +421,15 @@
     /**
      * Constructs a suggested account.
      *
      * @param editor {DescriptionEditor} the description editor
      * @param button {HTMLButtonElement} the account button
      */
     constructor(editor, button) {
-        super(editor, button.dataset.code, button.dataset.text, button.classList.contains("accounting-account-is-need-offset"), button);
+        super(editor, button.dataset.code, button.dataset.title, button.dataset.text, button.classList.contains("accounting-account-is-need-offset"), button);
     }
 }
 
 /**
  * The account option that is specified or confirmed by the user.
  *
  */
@@ -437,15 +438,15 @@
     /**
      * Constructs the account option that is specified or confirmed by the user.
      *
      * @param editor {DescriptionEditor} the description editor
      * @param button {HTMLButtonElement} the account button
      */
     constructor(editor, button) {
-        super(editor, "", "", false, button);
+        super(editor, "", "", "", false, button);
         this.isConfirmedAccount = true;
     }
 
     /**
      * Initializes the confirmed account from the line item editor.
      *
      * @param account {JournalEntryAccount} the confirmed account from the line item editor
```

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.4.0/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.4.0/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -199,14 +199,20 @@
     /**
      * The account code
      * @type {string}
      */
     code;
 
     /**
+     * The account title
+     * @type {string}
+     */
+    title;
+
+    /**
      * The account text
      * @type {string}
      */
     text;
 
     /**
      * Whether the account is in use
@@ -231,14 +237,15 @@
      *
      * @param selector {JournalEntryAccountSelector} the account selector
      * @param element {HTMLLIElement} the element
      */
     constructor(selector, element) {
         this.#element = element;
         this.code = element.dataset.code;
+        this.title = element.dataset.title;
         this.text = element.dataset.text;
         this.#isInUse = element.classList.contains("accounting-account-is-in-use");
         this.isNeedOffset = element.classList.contains("accounting-account-is-need-offset");
         this.#queryValues = JSON.parse(element.dataset.queryValues);
 
         this.#element.onclick = () => selector.lineItemEditor.saveAccount(this);
     }
```

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.4.0/src/accounting/static/js/journal-entry-form.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -788,14 +788,20 @@
     /**
      * The account code
      * @type {string}
      */
     code;
 
     /**
+     * The account title
+     * @type {string}
+     */
+    title;
+
+    /**
      * The account text
      * @type {string}
      */
     text;
 
     /**
      * Whether the line items in the account needs offset
@@ -803,30 +809,32 @@
      */
     isNeedOffset;
 
     /**
      * Constructs a journal entry account.
      *
      * @param code {string} the account code
+     * @param title {string} the account title
      * @param text {string} the account text
      * @param isNeedOffset {boolean} true if the line items in the account needs offset, or false otherwise
      */
-    constructor(code, text, isNeedOffset) {
+    constructor(code, title, text, isNeedOffset) {
         this.code = code;
+        this.title = title;
         this.text = text;
         this.isNeedOffset = isNeedOffset;
     }
 
     /**
      * Returns a copy of the account.
      *
      * @return {JournalEntryAccount} the copy of the account
      */
     copy() {
-        return new JournalEntryAccount(this.code, this.text, this.isNeedOffset);
+        return new JournalEntryAccount(this.code, this.title, this.text, this.isNeedOffset);
     }
 }
 
 /**
  * The line item sub-form.
  *
  */
@@ -883,18 +891,24 @@
     /**
      * The account code
      * @type {HTMLInputElement}
      */
     #accountCode;
 
     /**
-     * The text display of the account
-     * @type {HTMLDivElement}
+     * The code part of the text display of the account
+     * @type {HTMLSpanElement}
+     */
+    #accountTextCode;
+
+    /**
+     * The title part of the text display of the account
+     * @type {HTMLSpanElement}
      */
-    #accountText;
+    #accountTextTitle;
 
     /**
      * The description
      * @type {HTMLInputElement}
      */
     #description;
 
@@ -953,15 +967,16 @@
         this.index = parseInt(element.dataset.lineItemIndex);
         this.isMatched = element.classList.contains("accounting-matched-line-item");
         const prefix = `accounting-currency-${element.dataset.currencyIndex}-${this.debitCredit}-${String(this.index)}`;
         this.#control = document.getElementById(`${prefix}-control`);
         this.#error = document.getElementById(`${prefix}-error`);
         this.#no = document.getElementById(`${prefix}-no`);
         this.#accountCode = document.getElementById(`${prefix}-account-code`);
-        this.#accountText = document.getElementById(`${prefix}-account-text`);
+        this.#accountTextCode = document.getElementById(`${prefix}-account-text-code`);
+        this.#accountTextTitle = document.getElementById(`${prefix}-account-text-title`);
         this.#description = document.getElementById(`${prefix}-description`);
         this.#descriptionText = document.getElementById(`${prefix}-description-text`);
         this.#originalLineItemId = document.getElementById(`${prefix}-original-line-item-id`);
         this.#originalLineItemText = document.getElementById(`${prefix}-original-line-item-text`);
         this.#offsets = document.getElementById(`${prefix}-offsets`);
         this.#amount = document.getElementById(`${prefix}-amount`);
         this.#amountText = document.getElementById(`${prefix}-amount-text`);
@@ -1020,15 +1035,15 @@
 
     /**
      * Returns the account.
      *
      * @return {JournalEntryAccount|null} the account
      */
     get account() {
-        return this.#accountCode.value === null ? null : new JournalEntryAccount(this.#accountCode.value, this.#accountCode.dataset.text, this.#accountCode.classList.contains("accounting-account-is-need-offset"));
+        return this.#accountCode.value === null ? null : new JournalEntryAccount(this.#accountCode.value, this.#accountCode.dataset.title, this.#accountCode.dataset.text, this.#accountCode.classList.contains("accounting-account-is-need-offset"));
     }
 
     /**
      * Returns the amount.
      *
      * @return {Decimal|null} the amount
      */
@@ -1090,21 +1105,23 @@
             this.#originalLineItemText.innerText = "";
         } else {
             this.#originalLineItemText.innerText = A_("Offset %(item)s", {
                 item: editor.originalLineItemText
             });
         }
         this.#accountCode.value = editor.account.code;
+        this.#accountCode.dataset.title = editor.account.title;
         this.#accountCode.dataset.text = editor.account.text;
         if (editor.account.isNeedOffset) {
             this.#accountCode.classList.add("accounting-account-is-need-offset");
         } else {
             this.#accountCode.classList.remove("accounting-account-is-need-offset");
         }
-        this.#accountText.innerText = editor.account.text;
+        this.#accountTextCode.innerText = editor.account.code
+        this.#accountTextTitle.innerText = editor.account.title
         this.#description.value = editor.description === null ? "" : editor.description;
         this.#descriptionText.innerText = editor.description === null ? "" : editor.description;
         this.#amount.value = editor.amount;
         this.#amountText.innerText = formatDecimal(new Decimal(editor.amount));
         this.validate();
         this.debitCreditSubForm.updateTotal();
         this.debitCreditSubForm.currency.updateCodeSelectorStatus();
```

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.4.0/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -352,15 +352,15 @@
     /**
      * Saves the selected account.
      *
      * @param account {JournalEntryAccountOption} the selected account
      */
     saveAccount(account) {
         this.#accountControl.classList.add("accounting-not-empty");
-        this.account = new JournalEntryAccount(account.code, account.text, account.isNeedOffset);
+        this.account = new JournalEntryAccount(account.code, account.title, account.text, account.isNeedOffset);
         this.isAccountConfirmed = true;
         this.#accountText.innerText = account.text;
         this.#validateAccount();
     }
 
     /**
      * Validates the form.
```

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.4.0/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.4.0/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/option-form.js` & `mia-accounting-1.4.0/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.4.0/src/accounting/static/js/original-line-item-selector.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -280,15 +280,15 @@
     constructor(selector, element) {
         this.#form = selector.lineItemEditor.form;
         this.#element = element;
         this.id = element.dataset.id;
         this.date = element.dataset.date;
         this.#debitCredit = element.dataset.debitCredit;
         this.#currencyCode = element.dataset.currencyCode;
-        this.account = new JournalEntryAccount(element.dataset.accountCode, element.dataset.accountText, false);
+        this.account = new JournalEntryAccount(element.dataset.accountCode, element.dataset.accountTitle, element.dataset.accountText, false);
         this.description = element.dataset.description;
         this.bareNetBalance = new Decimal(element.dataset.netBalance);
         this.netBalance = this.bareNetBalance;
         this.netBalanceText = document.getElementById(`accounting-original-line-item-selector-option-${this.id}-net-balance`);
         this.text = element.dataset.text;
         this.#queryValues = JSON.parse(element.dataset.queryValues);
         this.#element.onclick = () => selector.lineItemEditor.saveOriginalLineItem(this);
```

### Comparing `mia-accounting-1.3.3/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.4.0/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/template_filters.py` & `mia-accounting-1.4.0/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/template_globals.py` & `mia-accounting-1.4.0/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/base.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/include/nav.html`

 * *Files 8% similar despite different names*

```diff
@@ -47,22 +47,14 @@
       </li>
       <li>
         <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.currency.") %} active {% endif %}" href="{{ url_for("accounting.currency.list") }}">
           <i class="fa-solid fa-money-bill-wave"></i>
           {{ A_("Currencies") }}
         </a>
       </li>
-      {% if accounting_can_edit() %}
-        <li>
-          <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.unmatched-offset.") %} active {% endif %}" href="{{ url_for("accounting.unmatched-offset.dashboard") }}">
-            <i class="fa-solid fa-link-slash"></i>
-            {{ A_("Unmatched Offsets") }}
-          </a>
-        </li>
-      {% endif %}
       {% if accounting_can_admin() %}
         <li>
           <a class="dropdown-item {% if request.endpoint and request.endpoint.startswith("accounting.option.") %} active {% endif %}" href="{{ url_for("accounting.option.detail") }}">
             <i class="fa-solid fa-gear"></i>
             {{ A_("Settings") }}
           </a>
         </li>
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             <i class="fa-solid fa-magnifying-glass"></i>
             {{ A_("Search") }}
           </label>
         </div>
 
         <ul id="accounting-account-selector-{{ debit_credit }}-option-list" class="list-group accounting-selector-list">
           {% for account in account_options %}
-            <li id="accounting-account-selector-{{ debit_credit }}-option-{{ account.code }}" class="list-group-item accounting-clickable accounting-account-selector-{{ debit_credit }}-option {% if account.is_in_use %} accounting-account-is-in-use {% endif %} {% if account.is_need_offset %} accounting-account-is-need-offset {% endif %}" data-code="{{ account.code }}" data-text="{{ account }}" data-query-values="{{ account.query_values|tojson|forceescape }}" data-bs-toggle="modal" data-bs-target="#accounting-line-item-editor-modal">
+            <li id="accounting-account-selector-{{ debit_credit }}-option-{{ account.code }}" class="list-group-item accounting-clickable accounting-account-selector-{{ debit_credit }}-option {% if account.is_in_use %} accounting-account-is-in-use {% endif %} {% if account.is_need_offset %} accounting-account-is-need-offset {% endif %}" data-code="{{ account.code }}" data-title="{{ account.title }}" data-text="{{ account }}" data-query-values="{{ account.query_values|tojson|forceescape }}" data-bs-toggle="modal" data-bs-target="#accounting-line-item-editor-modal">
               {{ account }}
             </li>
           {% endfor %}
           <li id="accounting-account-selector-{{ debit_credit }}-more" class="list-group-item accounting-clickable">{{ A_("More…") }}</li>
         </ul>
         <p id="accounting-account-selector-{{ debit_credit }}-option-no-result" class="d-none">{{ A_("There is no data.") }}</p>
       </div>
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             </div>
           </div>
 
           {# The suggested accounts #}
           <div class="mt-3 accounting-description-editor-buttons">
             <button id="accounting-description-editor-{{ description_editor.debit_credit }}-account-confirmed" class="btn btn-primary mb-1 d-none" type="button"></button>
             {% for account in description_editor.accounts %}
-              <button class="btn btn-outline-primary d-none accounting-description-editor-{{ description_editor.debit_credit }}-account {% if account.is_need_offset %} accounting-account-is-need-offset {% endif %}" type="button" data-code="{{ account.code }}" data-text="{{ account }}">
+              <button class="btn btn-outline-primary d-none accounting-description-editor-{{ description_editor.debit_credit }}-account {% if account.is_need_offset %} accounting-account-is-need-offset {% endif %}" type="button" data-code="{{ account.code }}" data-title="{{ account.title }}" data-text="{{ account }}">
                 {{ account }}
               </button>
             {% endfor %}
           </div>
         </div>
         <div class="modal-footer">
           <button class="btn btn-secondary" type="button" data-bs-toggle="modal" data-bs-target="#accounting-line-item-editor-modal">{{ A_("Cancel") }}</button>
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 First written: 2023/3/14
 #}
 {# <ul> For SonarQube not to complain about incorrect HTML #}
 {% for line_item in line_items %}
   <li class="list-group-item accounting-journal-entry-line-item">
     <div class="d-flex justify-content-between">
       <div>
-        <div class="small">{{ line_item.account }}</div>
+        <div class="small">
+          <span class="d-none d-md-inline">{{ line_item.account.code }}</span>
+          {{ line_item.account.title|title }}
+        </div>
         {% if line_item.description is not none %}
           <div>{{ line_item.description }}</div>
         {% endif %}
         {% if line_item.original_line_item %}
           <div class="fst-italic small accounting-original-line-item">
             <a href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.original_line_item.journal_entry)|accounting_append_next }}">
               {{ A_("Offset %(item)s", item=line_item.original_line_item) }}
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 implied. See the License for the specific language governing permissions and
 limitations under the License. Author: imacat@mail.imacat.idv.tw (imacat) First
 written: 2023/3/14 #} {#
     * For SonarQube not to complain about incorrect HTML #} {% for line_item in
       line_items %}
-    * {{ line_item.account }}
+    * {{ line_item.account.code }} {{ line_item.account.title|title }}
       {% if line_item.description is not none %}
       {{ line_item.description }}
       {% endif %} {% if line_item.original_line_item %}
       journal-entry.detail",
       journal_entry=line_item.original_line_item.journal_entry)|accounting_append_next
       }}"> {{ A_("Offset %(item)s", item=line_item.original_line_item) }}
 {% endif %} {% if line_item.is_need_offset %}
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,24 @@
 {# <ul> For SonarQube not to complain about incorrect HTML #}
 <li id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}" class="list-group-item list-group-item-action d-flex justify-content-between accounting-currency-{{ currency_index }}-{{ debit_credit }} {% if form.offsets %} accounting-matched-line-item {% endif %}" data-currency-index="{{ currency_index }}" data-debit-credit="{{ debit_credit }}" data-line-item-index="{{ line_item_index }}">
   {% if form.id.data %}
     <input type="hidden" name="currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-id" value="{{ form.id.data }}">
   {% endif %}
   <input id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-no" type="hidden" name="currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-no" value="{{ line_item_index }}">
   <input id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-original-line-item-id" class="accounting-original-line-item-id" type="hidden" name="currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-original_line_item_id" value="{{ form.original_line_item_id.data|accounting_default }}" data-date="{{ form.original_line_item_date|accounting_default }}" data-text="{{ form.original_line_item_text|accounting_default }}">
-  <input id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-account-code" class="{% if form.is_need_offset %} accounting-account-is-need-offset {% endif %}" type="hidden" name="currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-account_code" value="{{ form.account_code.data|accounting_default }}" data-text="{{ form.account_text }}">
+  <input id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-account-code" class="{% if form.is_need_offset %} accounting-account-is-need-offset {% endif %}" type="hidden" name="currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-account_code" value="{{ form.account_code.data|accounting_default }}" data-title="{{ form.account_title }}" data-text="{{ form.account_text }}">
   <input id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-description" type="hidden" name="currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-description" value="{{ form.description.data|accounting_default }}">
   <input id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-amount" type="hidden" name="currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-amount" value="{{ form.amount.data|accounting_journal_entry_format_amount_input }}" data-min="{{ form.offset_total|accounting_default("0") }}">
   <div class="accounting-line-item-content">
     <div id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-control" class="form-control clickable d-flex justify-content-between {% if form.all_errors %} is-invalid {% endif %}" data-bs-toggle="modal" data-bs-target="#accounting-line-item-editor-modal">
       <div>
-        <div id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-account-text" class="small">{{ form.account_text }}</div>
+        <div class="small">
+          <span id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-account-text-code" class="d-none d-md-inline">{{ form.account_code.data|accounting_default }}</span>
+          <span id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-account-text-title">{{ form.account_title }}</span>
+        </div>
         <div id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-description-text">{{ form.description.data|accounting_default }}</div>
         <div id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-original-line-item-text" class="fst-italic small accounting-original-line-item {% if not form.original_line_item_id.data %} d-none {% endif %}">
           {% if form.original_line_item_id.data %}{{ A_("Offset %(item)s", item=form.original_line_item_text|accounting_default) }}{% endif %}
         </div>
         <div id="accounting-currency-{{ currency_index }}-{{ debit_credit }}-{{ line_item_index }}-offsets" class="fst-italic small accounting-offset-line-items {% if not form.is_need_offset %} d-none {% endif %}">
           {% if form.offsets %}
             <div class="d-flex justify-content-between {% if not form.offsets %} d-none {% endif %}">
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,23 @@
             <i class="fa-solid fa-magnifying-glass"></i>
             {{ A_("Search") }}
           </label>
         </div>
 
         <ul id="accounting-original-line-item-selector-option-list" class="list-group accounting-selector-list">
           {% for line_item in form.original_line_item_options %}
-            <li id="accounting-original-line-item-selector-option-{{ line_item.id }}" class="list-group-item d-flex justify-content-between accounting-clickable accounting-original-line-item-selector-option" data-id="{{ line_item.id }}" data-date="{{ line_item.journal_entry.date }}" data-debit-credit="{{ "debit" if line_item.is_debit else "credit" }}" data-currency-code="{{ line_item.currency.code }}" data-account-code="{{ line_item.account_code }}" data-account-text="{{ line_item.account }}" data-description="{{ line_item.description|accounting_default }}" data-net-balance="{{ line_item.net_balance|accounting_journal_entry_format_amount_input }}" data-text="{{ line_item }}" data-query-values="{{ line_item.query_values|tojson|forceescape }}" data-bs-toggle="modal" data-bs-target="#accounting-line-item-editor-modal">
-              <div>{{ line_item.journal_entry.date|accounting_format_date }} {{ line_item.description|accounting_default }}</div>
+            <li id="accounting-original-line-item-selector-option-{{ line_item.id }}" class="list-group-item d-flex justify-content-between accounting-clickable accounting-original-line-item-selector-option" data-id="{{ line_item.id }}" data-date="{{ line_item.journal_entry.date }}" data-debit-credit="{{ "debit" if line_item.is_debit else "credit" }}" data-currency-code="{{ line_item.currency.code }}" data-account-code="{{ line_item.account_code }}" data-account-title="{{ line_item.account.title }}" data-account-text="{{ line_item.account }}" data-description="{{ line_item.description|accounting_default }}" data-net-balance="{{ line_item.net_balance|accounting_journal_entry_format_amount_input }}" data-text="{{ line_item }}" data-query-values="{{ line_item.query_values|tojson|forceescape }}" data-bs-toggle="modal" data-bs-target="#accounting-line-item-editor-modal">
+              <div>
+                <div class="small">
+                  {{ line_item.journal_entry.date|accounting_format_date }}
+                  <span class="d-none d-md-inline">{{ line_item.account.code }}</span>
+                  {{ line_item.account.title|title }}
+                </div>
+                {{ line_item.description|accounting_default }}
+              </div>
               <div>
                 <span class="badge bg-primary rounded-pill">
                   <span id="accounting-original-line-item-selector-option-{{ line_item.id }}-net-balance">{{ line_item.net_balance|accounting_format_amount }}</span>
                   / {{ line_item.amount|accounting_format_amount }}
                 </span>
               </div>
             </li>
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{{ A_("Balance Sheet of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Balance Sheet %(period)s", period=report.period.desc|title) }}{% else %}{{ A_("Balance Sheet of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_period_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
@@ -42,15 +42,21 @@
 {% include "accounting/report/include/period-chooser.html" %}
 
 {% include "accounting/report/include/search-modal.html" %}
 
 {% if report.has_data %}
   <div class="accounting-sheet">
     <div class="d-none d-sm-flex justify-content-center mb-3">
-      <h2 class="text-center">{{ A_("Balance Sheet of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}</h2>
+      <h2 class="text-center">
+        {% if report.currency.code == accounting_default_currency_code() %}
+          {{ A_("Balance Sheet %(period)s", period=report.period.desc|title) }}
+        {% else %}
+          {{ A_("Balance Sheet of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}
+        {% endif %}
+      </h2>
     </div>
 
     <div class="row accounting-report-table accounting-balance-sheet-table">
       <div class="col-sm-6">
         {% if report.assets.subsections %}
           {% with section = report.assets %}
             {% include "accounting/report/include/balance-sheet-section.html" %}
```

#### html2text {}

```diff
@@ -6,25 +6,30 @@
 distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 License for the specific language governing permissions and limitations under
 the License. Author: imacat@mail.imacat.idv.tw (imacat) First written: 2023/3/
 7 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
-{% endblock %} {% block header %}{% block title %}{{ A_("Balance Sheet of %
+{% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
+accounting_default_currency_code() %}{{ A_("Balance Sheet %(period)s",
+period=report.period.desc|title) }}{% else %}{{ A_("Balance Sheet of %
 (currency)s %(period)s", currency=report.currency.name|title,
-period=report.period.desc|title) }}{% endblock %}{% endblock %} {% block
-content %}
+period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %} {%
+block content %}
 {% with use_currency_chooser = true, use_period_chooser = true %} {% include
 "accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/period-chooser.html" %} {% include
 "accounting/report/include/search-modal.html" %} {% if report.has_data %}
-***** {{ A_("Balance Sheet of %(currency)s %(period)s",
-currency=report.currency.name|title, period=report.period.desc|title) }} *****
+***** {% if report.currency.code == accounting_default_currency_code() %} {{ A_
+("Balance Sheet %(period)s", period=report.period.desc|title) }} {% else %} {
+{ A_("Balance Sheet of %(currency)s %(period)s",
+currency=report.currency.name|title, period=report.period.desc|title) }} {%
+endif %} *****
 {% if report.assets.subsections %} {% with section = report.assets %} {%
 include "accounting/report/include/balance-sheet-section.html" %} {% endwith %}
 {{ A_("Total") }}
 {{ report.assets.total|accounting_report_format_amount }}
 {% endif %}
 {% if report.liabilities.subsections %} {% with section = report.liabilities %}
 {% include "accounting/report/include/balance-sheet-section.html" %} {% endwith
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 {% endif %}
 {% if use_account_chooser %}
   <div class="btn-group" role="group">
     <button id="accounting-choose-account" class="btn btn-primary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
       <i class="fa-solid fa-clipboard"></i>
       <span class="d-none d-md-inline">{{ A_("Account") }}</span>
     </button>
-    <ul class="dropdown-menu" aria-labelledby="accounting-choose-account">
+    <ul class="dropdown-menu accounting-toolbar-accounts" aria-labelledby="accounting-choose-account">
       {% for account in report.account_options %}
         <li>
           <a class="dropdown-item {% if account.is_active %} active {% endif %}" href="{{ account.url }}">
             {{ account.title|title }}
           </a>
         </li>
       {% endfor %}
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{{ A_("Income and Expenses Log of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title|title, period=report.period.desc|title) }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Income and Expenses Log of %(account)s %(period)s", account=report.account.title|title, period=report.period.desc|title) }}{% else %}{{ A_("Income and Expenses Log of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title|title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true,
           use_period_chooser = true %}
```

#### html2text {}

```diff
@@ -6,19 +6,21 @@
 software distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
 the License for the specific language governing permissions and limitations
 under the License. Author: imacat@mail.imacat.idv.tw (imacat) First written:
 2023/3/5 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
-{% endblock %} {% block header %}{% block title %}{{ A_("Income and Expenses
-Log of %(account)s in %(currency)s %(period)s",
-currency=report.currency.name|title, account=report.account.title|title,
-period=report.period.desc|title) }}{% endblock %}{% endblock %} {% block
-content %}
+{% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
+accounting_default_currency_code() %}{{ A_("Income and Expenses Log of %
+(account)s %(period)s", account=report.account.title|title,
+period=report.period.desc|title) }}{% else %}{{ A_("Income and Expenses Log of
+%(account)s in %(currency)s %(period)s", currency=report.currency.name|title,
+account=report.account.title|title, period=report.period.desc|title) }}{% endif
+%}{% endblock %}{% endblock %} {% block content %}
 {% with use_currency_chooser = true, use_account_chooser = true,
 use_period_chooser = true %} {% include "accounting/report/include/toolbar-
 buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/period-chooser.html" %} {% include
 "accounting/report/include/search-modal.html" %} {% if report.has_data %} {%
 with pagination = report.pagination %} {% include "accounting/include/
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/income-statement.html`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{{ A_("Income Statement of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Income Statement %(period)s", period=report.period.desc|title) }}{% else %}{{ A_("Income Statement of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_period_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
@@ -42,15 +42,21 @@
 {% include "accounting/report/include/period-chooser.html" %}
 
 {% include "accounting/report/include/search-modal.html" %}
 
 {% if report.has_data %}
   <div class="accounting-sheet">
     <div class="d-none d-sm-flex justify-content-center mb-3">
-      <h2 class="text-center">{{ A_("Income Statement of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}</h2>
+      <h2 class="text-center">
+        {% if report.currency.code == accounting_default_currency_code() %}
+          {{ A_("Income Statement %(period)s", period=report.period.desc|title) }}
+        {% else %}
+          {{ A_("Income Statement of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}
+        {% endif %}
+      </h2>
     </div>
 
     <div class="accounting-report-table accounting-income-statement-table">
       <div class="accounting-report-table-header">
         <div class="accounting-report-table-row">
           <div class="accounting-amount">{{ A_("Amount") }}</div>
         </div>
```

#### html2text {}

```diff
@@ -6,25 +6,30 @@
 distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 License for the specific language governing permissions and limitations under
 the License. Author: imacat@mail.imacat.idv.tw (imacat) First written: 2023/3/
 7 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
-{% endblock %} {% block header %}{% block title %}{{ A_("Income Statement of %
+{% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
+accounting_default_currency_code() %}{{ A_("Income Statement %(period)s",
+period=report.period.desc|title) }}{% else %}{{ A_("Income Statement of %
 (currency)s %(period)s", currency=report.currency.name|title,
-period=report.period.desc|title) }}{% endblock %}{% endblock %} {% block
-content %}
+period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %} {%
+block content %}
 {% with use_currency_chooser = true, use_period_chooser = true %} {% include
 "accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/period-chooser.html" %} {% include
 "accounting/report/include/search-modal.html" %} {% if report.has_data %}
-***** {{ A_("Income Statement of %(currency)s %(period)s",
-currency=report.currency.name|title, period=report.period.desc|title) }} *****
+***** {% if report.currency.code == accounting_default_currency_code() %} {{ A_
+("Income Statement %(period)s", period=report.period.desc|title) }} {% else %}
+{{ A_("Income Statement of %(currency)s %(period)s",
+currency=report.currency.name|title, period=report.period.desc|title) }} {%
+endif %} *****
 {{ A_("Amount") }}
 {% for section in report.sections %}
 {{ section.title.code }} {{ section.title.title|title }}
 {% for subsection in section.subsections %}
 {{ subsection.title.code }} {{ subsection.title.title|title }}
 {% for account in subsection.accounts %}
 {{_account.account.code_}}_{{_account.account.title|title_}}
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/ledger.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{{ A_("Ledger of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title|title, period=report.period.desc|title) }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Ledger of %(account)s %(period)s", account=report.account.title|title, period=report.period.desc|title) }}{% else %}{{ A_("Ledger of %(account)s in %(currency)s %(period)s", currency=report.currency.name|title, account=report.account.title|title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_account_chooser = true,
           use_period_chooser = true %}
```

#### html2text {}

```diff
@@ -6,18 +6,21 @@
 is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied. See the License for the specific language
 governing permissions and limitations under the License. Author:
 imacat@mail.imacat.idv.tw (imacat) First written: 2023/3/5 #} {% extends
 "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
-{% endblock %} {% block header %}{% block title %}{{ A_("Ledger of %(account)s
-in %(currency)s %(period)s", currency=report.currency.name|title,
-account=report.account.title|title, period=report.period.desc|title) }}{%
-endblock %}{% endblock %} {% block content %}
+{% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
+accounting_default_currency_code() %}{{ A_("Ledger of %(account)s %(period)s",
+account=report.account.title|title, period=report.period.desc|title) }}{% else
+%}{{ A_("Ledger of %(account)s in %(currency)s %(period)s",
+currency=report.currency.name|title, account=report.account.title|title,
+period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %} {%
+block content %}
 {% with use_currency_chooser = true, use_account_chooser = true,
 use_period_chooser = true %} {% include "accounting/report/include/toolbar-
 buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/period-chooser.html" %} {% include
 "accounting/report/include/search-modal.html" %} {% if report.has_data %} {%
 with pagination = report.pagination %} {% include "accounting/include/
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
   <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{{ A_("Trial Balance of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Trial Balance %(period)s", period=report.period.desc|title) }}{% else %}{{ A_("Trial Balance of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
   {% with use_currency_chooser = true,
           use_period_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
@@ -42,15 +42,21 @@
 {% include "accounting/report/include/period-chooser.html" %}
 
 {% include "accounting/report/include/search-modal.html" %}
 
 {% if report.has_data %}
   <div class="accounting-sheet">
     <div class="d-none d-sm-flex justify-content-center mb-3">
-      <h2 class="text-center">{{ A_("Trial Balance of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}</h2>
+      <h2 class="text-center">
+        {% if report.currency.code == accounting_default_currency_code() %}
+          {{ A_("Trial Balance %(period)s", period=report.period.desc|title) }}
+        {% else %}
+          {{ A_("Trial Balance of %(currency)s %(period)s", currency=report.currency.name|title, period=report.period.desc|title) }}
+        {% endif %}
+      </h2>
     </div>
 
     <div class="accounting-report-table accounting-trial-balance-table">
       <div class="accounting-report-table-header">
         <div class="accounting-report-table-row">
           <div>{{ A_("Account") }}</div>
           <div class="accounting-amount">{{ A_("Debit") }}</div>
```

#### html2text {}

```diff
@@ -6,25 +6,30 @@
 distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 License for the specific language governing permissions and limitations under
 the License. Author: imacat@mail.imacat.idv.tw (imacat) First written: 2023/3/
 5 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
 static", filename="js/period-chooser.js") }}">
-{% endblock %} {% block header %}{% block title %}{{ A_("Trial Balance of %
+{% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
+accounting_default_currency_code() %}{{ A_("Trial Balance %(period)s",
+period=report.period.desc|title) }}{% else %}{{ A_("Trial Balance of %
 (currency)s %(period)s", currency=report.currency.name|title,
-period=report.period.desc|title) }}{% endblock %}{% endblock %} {% block
-content %}
+period=report.period.desc|title) }}{% endif %}{% endblock %}{% endblock %} {%
+block content %}
 {% with use_currency_chooser = true, use_period_chooser = true %} {% include
 "accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/period-chooser.html" %} {% include
 "accounting/report/include/search-modal.html" %} {% if report.has_data %}
-***** {{ A_("Trial Balance of %(currency)s %(period)s",
-currency=report.currency.name|title, period=report.period.desc|title) }} *****
+***** {% if report.currency.code == accounting_default_currency_code() %} {{ A_
+("Trial Balance %(period)s", period=report.period.desc|title) }} {% else %} {
+{ A_("Trial Balance of %(currency)s %(period)s",
+currency=report.currency.name|title, period=report.period.desc|title) }} {%
+endif %} *****
 {{ A_("Account") }}
 {{ A_("Debit") }}
 {{ A_("Credit") }}
 {% for account in report.accounts %}
 {{_account.account.code_}}_{{_account.account.title|title_}}
 {{_account.debit|accounting_format_amount|accounting_default_}}
 {{_account.credit|accounting_format_amount|accounting_default_}}
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.4.0/src/accounting/templates/accounting/report/unapplied.html`

 * *Files 8% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/4/7
 #}
 {% extends "accounting/base.html" %}
 
 {% block accounting_scripts %}
   <script src="{{ url_for("accounting.static", filename="js/material-fab-speed-dial.js") }}"></script>
+  <script src="{{ url_for("accounting.static", filename="js/period-chooser.js") }}"></script>
 {% endblock %}
 
-{% block header %}{% block title %}{{ A_("Unapplied Original Line Items of %(account)s", account=report.account.title|title) }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{% if report.currency.code == accounting_default_currency_code() %}{{ A_("Unapplied Items of %(account)s", account=report.account.title|title) }}{% else %}{{ A_("Unapplied Items of %(account)s in %(currency)s", currency=report.currency.name|title, account=report.account.title|title) }}{% endif %}{% endblock %}{% endblock %}
 
 {% block content %}
 
 <div class="mb-3 accounting-toolbar">
-  {% with use_account_chooser = true %}
+  {% with use_currency_chooser = true,
+          use_account_chooser = true %}
     {% include "accounting/report/include/toolbar-buttons.html" %}
   {% endwith %}
 </div>
 
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 
 {% include "accounting/report/include/search-modal.html" %}
@@ -44,47 +46,37 @@
     {% include "accounting/include/pagination.html" %}
   {% endwith %}
 
   <div class="d-none d-md-block accounting-report-table accounting-unapplied-table">
     <div class="accounting-report-table-header">
       <div class="accounting-report-table-row">
         <div>{{ A_("Date") }}</div>
-        <div>{{ A_("Currency") }}</div>
         <div>{{ A_("Description") }}</div>
         <div class="accounting-amount">{{ A_("Amount") }}</div>
         <div class="accounting-amount">{{ A_("Net Balance") }}</div>
       </div>
     </div>
     <div class="accounting-report-table-body">
       {% for line_item in report.line_items %}
-        <a class="accounting-report-table-row {% if report.is_mark_matches and not line_item.match %} accounting-report-table-row-danger {% endif %}" href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.journal_entry)|accounting_append_next }}">
+        <a class="accounting-report-table-row" href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.journal_entry)|accounting_append_next }}">
           <div>{{ line_item.journal_entry.date|accounting_format_date }}</div>
-          <div>{{ line_item.currency.name }}</div>
-          <div>
-            {{ line_item.description|accounting_default }}
-            {% if report.is_mark_matches and line_item.match %}
-              <div>{{ A_("Can match %(offset)s", offset=line_item.match) }}</div>
-            {% endif %}
-          </div>
+          <div>{{ line_item.description|accounting_default }}</div>
           <div class="accounting-amount">{{ line_item.amount|accounting_format_amount }}</div>
           <div class="accounting-amount">{{ line_item.net_balance|accounting_format_amount }}</div>
         </a>
       {% endfor %}
     </div>
   </div>
 
   <div class="list-group d-md-none">
   {% for line_item in report.line_items %}
     <a class="list-group-item list-group-item-action d-flex justify-content-between" href="{{ url_for("accounting.journal-entry.detail", journal_entry=line_item.journal_entry)|accounting_append_next }}">
       <div>
         <div class="text-muted small">
           {{ line_item.journal_entry.date|accounting_format_date }}
-          {% if line_item.currency.code != accounting_default_currency_code() %}
-            <span class="badge rounded-pill bg-info">{{ line_item.currency.code }}</span>
-          {% endif %}
         </div>
         {% if line_item.description is not none %}
           <div>{{ line_item.description }}</div>
         {% endif %}
       </div>
 
       <div>
```

#### html2text {}

```diff
@@ -5,46 +5,43 @@
 licenses/LICENSE-2.0 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
 the License for the specific language governing permissions and limitations
 under the License. Author: imacat@mail.imacat.idv.tw (imacat) First written:
 2023/4/7 #} {% extends "accounting/base.html" %} {% block accounting_scripts %}
 static", filename="js/material-fab-speed-dial.js") }}">
-{% endblock %} {% block header %}{% block title %}{{ A_("Unapplied Original
-Line Items of %(account)s", account=report.account.title|title) }}{% endblock
-%}{% endblock %} {% block content %}
-{% with use_account_chooser = true %} {% include "accounting/report/include/
-toolbar-buttons.html" %} {% endwith %}
+static", filename="js/period-chooser.js") }}">
+{% endblock %} {% block header %}{% block title %}{% if report.currency.code ==
+accounting_default_currency_code() %}{{ A_("Unapplied Items of %(account)s",
+account=report.account.title|title) }}{% else %}{{ A_("Unapplied Items of %
+(account)s in %(currency)s", currency=report.currency.name|title,
+account=report.account.title|title) }}{% endif %}{% endblock %}{% endblock %}
+{% block content %}
+{% with use_currency_chooser = true, use_account_chooser = true %} {% include
+"accounting/report/include/toolbar-buttons.html" %} {% endwith %}
 {% include "accounting/report/include/add-journal-entry-material-fab.html" %}
 {% include "accounting/report/include/search-modal.html" %} {% if
 report.has_data %} {% with pagination = report.pagination %} {% include
 "accounting/include/pagination.html" %} {% endwith %}
 {{ A_("Date") }}
-{{ A_("Currency") }}
 {{ A_("Description") }}
 {{ A_("Amount") }}
 {{ A_("Net Balance") }}
 {% for line_item in report.line_items %}
 journal-entry.detail",
 journal_entry=line_item.journal_entry)|accounting_append_next }}">
 {{ line_item.journal_entry.date|accounting_format_date }}
-{{ line_item.currency.name }}
-{{ line_item.description|accounting_default }} {% if report.is_mark_matches and
-line_item.match %}
-{{ A_("Can match %(offset)s", offset=line_item.match) }}
-{% endif %}
+{{ line_item.description|accounting_default }}
 {{ line_item.amount|accounting_format_amount }}
 {{ line_item.net_balance|accounting_format_amount }}
  {% endfor %}
 {% for line_item in report.line_items %}
 journal-entry.detail",
 journal_entry=line_item.journal_entry)|accounting_append_next }}">
-{{ line_item.journal_entry.date|accounting_format_date }} {% if
-line_item.currency.code != accounting_default_currency_code() %} {
-{ line_item.currency.code }} {% endif %}
+{{ line_item.journal_entry.date|accounting_format_date }}
 {% if line_item.description is not none %}
 {{ line_item.description }}
 {% endif %}
 {{ line_item.amount|accounting_format_amount }} {
 { line_item.net_balance|accounting_format_amount }}
  {% endfor %}
 {% else %}
```

### Comparing `mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/dashboard.html` & `mia-accounting-1.4.0/tests/test_site/templates/home.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 00000000: 7b23 0a54 6865 204d 6961 2120 4163 636f  {#.The Mia! Acco
-00000010: 756e 7469 6e67 2050 726f 6a65 6374 0a64  unting Project.d
-00000020: 6173 6862 6f61 7264 2e68 746d 6c3a 2054  ashboard.html: T
-00000030: 6865 2061 6363 6f75 6e74 206c 6973 7420  he account list 
-00000040: 7769 7468 2075 6e6d 6174 6368 6564 206f  with unmatched o
-00000050: 6666 7365 7473 0a0a 2043 6f70 7972 6967  ffsets.. Copyrig
-00000060: 6874 2028 6329 2032 3032 3320 696d 6163  ht (c) 2023 imac
-00000070: 6174 2e0a 0a20 4c69 6365 6e73 6564 2075  at... Licensed u
-00000080: 6e64 6572 2074 6865 2041 7061 6368 6520  nder the Apache 
-00000090: 4c69 6365 6e73 652c 2056 6572 7369 6f6e  License, Version
-000000a0: 2032 2e30 2028 7468 6520 224c 6963 656e   2.0 (the "Licen
-000000b0: 7365 2229 3b0a 2079 6f75 206d 6179 206e  se");. you may n
-000000c0: 6f74 2075 7365 2074 6869 7320 6669 6c65  ot use this file
-000000d0: 2065 7863 6570 7420 696e 2063 6f6d 706c   except in compl
-000000e0: 6961 6e63 6520 7769 7468 2074 6865 204c  iance with the L
-000000f0: 6963 656e 7365 2e0a 2059 6f75 206d 6179  icense.. You may
-00000100: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
-00000110: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
-00000120: 0a0a 2020 2020 2068 7474 703a 2f2f 7777  ..     http://ww
-00000130: 772e 6170 6163 6865 2e6f 7267 2f6c 6963  w.apache.org/lic
-00000140: 656e 7365 732f 4c49 4345 4e53 452d 322e  enses/LICENSE-2.
-00000150: 300a 0a20 556e 6c65 7373 2072 6571 7569  0.. Unless requi
-00000160: 7265 6420 6279 2061 7070 6c69 6361 626c  red by applicabl
-00000170: 6520 6c61 7720 6f72 2061 6772 6565 6420  e law or agreed 
-00000180: 746f 2069 6e20 7772 6974 696e 672c 2073  to in writing, s
-00000190: 6f66 7477 6172 650a 2064 6973 7472 6962  oftware. distrib
-000001a0: 7574 6564 2075 6e64 6572 2074 6865 204c  uted under the L
-000001b0: 6963 656e 7365 2069 7320 6469 7374 7269  icense is distri
-000001c0: 6275 7465 6420 6f6e 2061 6e20 2241 5320  buted on an "AS 
-000001d0: 4953 2220 4241 5349 532c 0a20 5749 5448  IS" BASIS,. WITH
-000001e0: 4f55 5420 5741 5252 414e 5449 4553 204f  OUT WARRANTIES O
-000001f0: 5220 434f 4e44 4954 494f 4e53 204f 4620  R CONDITIONS OF 
-00000200: 414e 5920 4b49 4e44 2c20 6569 7468 6572  ANY KIND, either
-00000210: 2065 7870 7265 7373 206f 7220 696d 706c   express or impl
-00000220: 6965 642e 0a20 5365 6520 7468 6520 4c69  ied.. See the Li
-00000230: 6365 6e73 6520 666f 7220 7468 6520 7370  cense for the sp
-00000240: 6563 6966 6963 206c 616e 6775 6167 6520  ecific language 
-00000250: 676f 7665 726e 696e 6720 7065 726d 6973  governing permis
-00000260: 7369 6f6e 7320 616e 640a 206c 696d 6974  sions and. limit
-00000270: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
-00000280: 204c 6963 656e 7365 2e0a 0a41 7574 686f   License...Autho
-00000290: 723a 2069 6d61 6361 7440 6d61 696c 2e69  r: imacat@mail.i
-000002a0: 6d61 6361 742e 6964 762e 7477 2028 696d  macat.idv.tw (im
-000002b0: 6163 6174 290a 4669 7273 7420 7772 6974  acat).First writ
-000002c0: 7465 6e3a 2032 3032 332f 342f 380a 237d  ten: 2023/4/8.#}
-000002d0: 0a7b 2520 6578 7465 6e64 7320 2261 6363  .{% extends "acc
-000002e0: 6f75 6e74 696e 672f 6261 7365 2e68 746d  ounting/base.htm
-000002f0: 6c22 2025 7d0a 0a7b 2520 626c 6f63 6b20  l" %}..{% block 
-00000300: 6865 6164 6572 2025 7d7b 2520 626c 6f63  header %}{% bloc
-00000310: 6b20 7469 746c 6520 257d 7b7b 2041 5f28  k title %}{{ A_(
-00000320: 2255 6e6d 6174 6368 6564 204f 6666 7365  "Unmatched Offse
-00000330: 7473 2229 207d 7d7b 2520 656e 6462 6c6f  ts") }}{% endblo
-00000340: 636b 2025 7d7b 2520 656e 6462 6c6f 636b  ck %}{% endblock
-00000350: 2025 7d0a 0a7b 2520 626c 6f63 6b20 636f   %}..{% block co
-00000360: 6e74 656e 7420 257d 0a0a 7b25 2069 6620  ntent %}..{% if 
-00000370: 6c69 7374 2025 7d0a 2020 3c64 6976 3e0a  list %}.  <div>.
-00000380: 2020 2020 7b25 2066 6f72 2061 6363 6f75      {% for accou
-00000390: 6e74 2069 6e20 6c69 7374 2025 7d0a 2020  nt in list %}.  
-000003a0: 2020 2020 3c61 2063 6c61 7373 3d22 6274      <a class="bt
-000003b0: 6e20 6274 6e2d 7072 696d 6172 7920 6d62  n btn-primary mb
-000003c0: 2d31 2220 726f 6c65 3d22 6275 7474 6f6e  -1" role="button
-000003d0: 2220 6872 6566 3d22 7b7b 2075 726c 5f66  " href="{{ url_f
-000003e0: 6f72 2822 6163 636f 756e 7469 6e67 2e75  or("accounting.u
-000003f0: 6e6d 6174 6368 6564 2d6f 6666 7365 742e  nmatched-offset.
-00000400: 6c69 7374 222c 2061 6363 6f75 6e74 3d61  list", account=a
-00000410: 6363 6f75 6e74 2920 7d7d 223e 0a20 2020  ccount) }}">.   
-00000420: 2020 2020 207b 7b20 6163 636f 756e 7420       {{ account 
-00000430: 7d7d 2028 7b7b 2061 6363 6f75 6e74 2e63  }} ({{ account.c
-00000440: 6f75 6e74 207d 7d29 0a20 2020 2020 203c  ount }}).      <
-00000450: 2f61 3e0a 2020 2020 7b25 2065 6e64 666f  /a>.    {% endfo
-00000460: 7220 257d 0a20 203c 2f64 6976 3e0a 7b25  r %}.  </div>.{%
-00000470: 2065 6c73 6520 257d 0a20 203c 703e 7b7b   else %}.  <p>{{
-00000480: 2041 5f28 2254 6865 7265 2069 7320 6e6f   A_("There is no
-00000490: 2064 6174 612e 2229 207d 7d3c 2f70 3e0a   data.") }}</p>.
-000004a0: 7b25 2065 6e64 6966 2025 7d0a 0a7b 2520  {% endif %}..{% 
-000004b0: 656e 6462 6c6f 636b 2025 7d0a            endblock %}.
+00000010: 756e 7469 6e67 2044 656d 6f6e 7374 7261  unting Demonstra
+00000020: 7469 6f6e 2057 6562 7369 7465 0a68 6f6d  tion Website.hom
+00000030: 652e 6874 6d6c 3a20 5468 6520 686f 6d65  e.html: The home
+00000040: 2070 6167 652e 0a0a 2043 6f70 7972 6967   page... Copyrig
+00000050: 6874 2028 6329 2032 3032 3320 696d 6163  ht (c) 2023 imac
+00000060: 6174 2e0a 0a20 4c69 6365 6e73 6564 2075  at... Licensed u
+00000070: 6e64 6572 2074 6865 2041 7061 6368 6520  nder the Apache 
+00000080: 4c69 6365 6e73 652c 2056 6572 7369 6f6e  License, Version
+00000090: 2032 2e30 2028 7468 6520 224c 6963 656e   2.0 (the "Licen
+000000a0: 7365 2229 3b0a 2079 6f75 206d 6179 206e  se");. you may n
+000000b0: 6f74 2075 7365 2074 6869 7320 6669 6c65  ot use this file
+000000c0: 2065 7863 6570 7420 696e 2063 6f6d 706c   except in compl
+000000d0: 6961 6e63 6520 7769 7468 2074 6865 204c  iance with the L
+000000e0: 6963 656e 7365 2e0a 2059 6f75 206d 6179  icense.. You may
+000000f0: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
+00000100: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
+00000110: 0a0a 2020 2020 2068 7474 703a 2f2f 7777  ..     http://ww
+00000120: 772e 6170 6163 6865 2e6f 7267 2f6c 6963  w.apache.org/lic
+00000130: 656e 7365 732f 4c49 4345 4e53 452d 322e  enses/LICENSE-2.
+00000140: 300a 0a20 556e 6c65 7373 2072 6571 7569  0.. Unless requi
+00000150: 7265 6420 6279 2061 7070 6c69 6361 626c  red by applicabl
+00000160: 6520 6c61 7720 6f72 2061 6772 6565 6420  e law or agreed 
+00000170: 746f 2069 6e20 7772 6974 696e 672c 2073  to in writing, s
+00000180: 6f66 7477 6172 650a 2064 6973 7472 6962  oftware. distrib
+00000190: 7574 6564 2075 6e64 6572 2074 6865 204c  uted under the L
+000001a0: 6963 656e 7365 2069 7320 6469 7374 7269  icense is distri
+000001b0: 6275 7465 6420 6f6e 2061 6e20 2241 5320  buted on an "AS 
+000001c0: 4953 2220 4241 5349 532c 0a20 5749 5448  IS" BASIS,. WITH
+000001d0: 4f55 5420 5741 5252 414e 5449 4553 204f  OUT WARRANTIES O
+000001e0: 5220 434f 4e44 4954 494f 4e53 204f 4620  R CONDITIONS OF 
+000001f0: 414e 5920 4b49 4e44 2c20 6569 7468 6572  ANY KIND, either
+00000200: 2065 7870 7265 7373 206f 7220 696d 706c   express or impl
+00000210: 6965 642e 0a20 5365 6520 7468 6520 4c69  ied.. See the Li
+00000220: 6365 6e73 6520 666f 7220 7468 6520 7370  cense for the sp
+00000230: 6563 6966 6963 206c 616e 6775 6167 6520  ecific language 
+00000240: 676f 7665 726e 696e 6720 7065 726d 6973  governing permis
+00000250: 7369 6f6e 7320 616e 640a 206c 696d 6974  sions and. limit
+00000260: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
+00000270: 204c 6963 656e 7365 2e0a 0a41 7574 686f   License...Autho
+00000280: 723a 2069 6d61 6361 7440 6d61 696c 2e69  r: imacat@mail.i
+00000290: 6d61 6361 742e 6964 762e 7477 2028 696d  macat.idv.tw (im
+000002a0: 6163 6174 290a 4669 7273 7420 7772 6974  acat).First writ
+000002b0: 7465 6e3a 2032 3032 332f 312f 3237 0a23  ten: 2023/1/27.#
+000002c0: 7d0a 7b25 2065 7874 656e 6473 2022 6261  }.{% extends "ba
+000002d0: 7365 2e68 746d 6c22 2025 7d0a 0a7b 2520  se.html" %}..{% 
+000002e0: 626c 6f63 6b20 6865 6164 6572 2025 7d7b  block header %}{
+000002f0: 2520 626c 6f63 6b20 7469 746c 6520 257d  % block title %}
+00000300: 7b7b 205f 2822 4d69 6121 2041 6363 6f75  {{ _("Mia! Accou
+00000310: 6e74 696e 6720 4c69 7665 2044 656d 6f6e  nting Live Demon
+00000320: 7374 7261 7469 6f6e 2229 207d 7d7b 2520  stration") }}{% 
+00000330: 656e 6462 6c6f 636b 2025 7d7b 2520 656e  endblock %}{% en
+00000340: 6462 6c6f 636b 2025 7d0a 0a7b 2520 626c  dblock %}..{% bl
+00000350: 6f63 6b20 636f 6e74 656e 7420 257d 0a0a  ock content %}..
+00000360: 3c70 3e7b 7b20 5f28 2254 6869 7320 6973  <p>{{ _("This is
+00000370: 2074 6865 206c 6976 6520 6465 6d6f 6e73   the live demons
+00000380: 7472 6174 696f 6e20 6f66 2074 6865 204d  tration of the M
+00000390: 6961 2120 4163 636f 756e 7469 6e67 2070  ia! Accounting p
+000003a0: 726f 6a65 6374 2e20 2050 6c65 6173 6520  roject.  Please 
+000003b0: 3c61 2068 7265 663d 5c22 2f6c 6f67 696e  <a href=\"/login
+000003c0: 3f6e 6578 743d 2525 3246 6163 636f 756e  ?next=%%2Faccoun
+000003d0: 7469 6e67 5c22 3e6c 6f67 2069 6e3c 2f61  ting\">log in</a
+000003e0: 3e20 746f 2063 6f6e 7469 6e75 652e 2229  > to continue.")
+000003f0: 207d 7d3c 2f70 3e0a 0a3c 703e 7b7b 205f   }}</p>..<p>{{ _
+00000400: 2822 596f 7520 6d61 7920 616c 736f 2077  ("You may also w
+00000410: 616e 7420 746f 2063 6865 636b 2074 6865  ant to check the
+00000420: 203c 6120 6872 6566 3d5c 2268 7474 7073   <a href=\"https
+00000430: 3a2f 2f6d 6961 2d61 6363 6f75 6e74 696e  ://mia-accountin
+00000440: 672e 7265 6164 7468 6564 6f63 732e 696f  g.readthedocs.io
+00000450: 5c22 3e66 756c 6c20 646f 6375 6d65 6e74  \">full document
+00000460: 6174 696f 6e3c 2f61 3e20 616e 6420 7468  ation</a> and th
+00000470: 6520 3c61 2068 7265 663d 5c22 6874 7470  e <a href=\"http
+00000480: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
+00000490: 6d61 6361 742f 6d69 612d 6163 636f 756e  macat/mia-accoun
+000004a0: 7469 6e67 5c22 3e47 6974 6875 6220 7265  ting\">Github re
+000004b0: 706f 7369 746f 7279 3c2f 613e 2e22 2920  pository</a>.") 
+000004c0: 7d7d 3c2f 703e 0a0a 7b25 2065 6e64 626c  }}</p>..{% endbl
+000004d0: 6f63 6b20 257d 0a                        ock %}.
```

### Comparing `mia-accounting-1.3.3/src/accounting/translations/accounting.pot` & `mia-accounting-1.4.0/src/accounting/translations/accounting.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-09 01:41+0800\n"
+"POT-Creation-Date: 2023-04-18 09:32+0800\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: src/accounting/forms.py:33
-#: src/accounting/static/js/journal-entry-form.js:1065
+#: src/accounting/static/js/journal-entry-form.js:1080
 #: src/accounting/static/js/journal-entry-line-item-editor.js:411
 #: src/accounting/static/js/option-form.js:537
 #: src/accounting/static/js/option-form.js:803
 msgid "Please select the account."
 msgstr ""
 
 #: src/accounting/forms.py:44
@@ -296,19 +296,19 @@
 
 #: src/accounting/journal_entry/forms/line_item.py:241
 #: src/accounting/static/js/journal-entry-line-item-editor.js:450
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:413
+#: src/accounting/journal_entry/forms/line_item.py:426
 msgid "This account is not for debit line items."
 msgstr ""
 
-#: src/accounting/journal_entry/forms/line_item.py:465
+#: src/accounting/journal_entry/forms/line_item.py:478
 msgid "This account is not for credit line items."
 msgstr ""
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr ""
 
@@ -348,14 +348,23 @@
 msgid "The settings were not modified."
 msgstr ""
 
 #: src/accounting/option/views.py:82
 msgid "The settings are saved successfully."
 msgstr ""
 
+#: src/accounting/report/views.py:401
+msgid "No more offset to match automatically."
+msgstr ""
+
+#: src/accounting/report/views.py:408
+#, python-format
+msgid "Matched %(matches)s offsets."
+msgstr ""
+
 #: src/accounting/report/period/description.py:33
 msgid "for all time"
 msgstr ""
 
 #: src/accounting/report/period/description.py:67
 #, python-format
 msgid "since %(start)s"
@@ -417,71 +426,76 @@
 #: src/accounting/report/reports/ledger.py:380
 #: src/accounting/report/reports/trial_balance.py:229
 #: src/accounting/templates/accounting/journal-entry/disbursement/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html:38
 #: src/accounting/templates/accounting/journal-entry/receipt/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:39
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:55
-#: src/accounting/templates/accounting/report/balance-sheet.html:59
-#: src/accounting/templates/accounting/report/balance-sheet.html:71
-#: src/accounting/templates/accounting/report/balance-sheet.html:81
+#: src/accounting/templates/accounting/report/balance-sheet.html:65
+#: src/accounting/templates/accounting/report/balance-sheet.html:77
 #: src/accounting/templates/accounting/report/balance-sheet.html:87
-#: src/accounting/templates/accounting/report/balance-sheet.html:96
-#: src/accounting/templates/accounting/report/balance-sheet.html:103
+#: src/accounting/templates/accounting/report/balance-sheet.html:93
+#: src/accounting/templates/accounting/report/balance-sheet.html:102
+#: src/accounting/templates/accounting/report/balance-sheet.html:109
 #: src/accounting/templates/accounting/report/income-expenses.html:81
-#: src/accounting/templates/accounting/report/income-statement.html:83
+#: src/accounting/templates/accounting/report/income-statement.html:89
 #: src/accounting/templates/accounting/report/ledger.html:82
-#: src/accounting/templates/accounting/report/trial-balance.html:74
+#: src/accounting/templates/accounting/report/trial-balance.html:80
 msgid "Total"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:136
 #: src/accounting/report/reports/ledger.py:132
 msgid "Brought forward"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/ledger.py:366
-#: src/accounting/report/reports/unapplied.py:137
+#: src/accounting/report/reports/unapplied.py:148
+#: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
-#: src/accounting/templates/accounting/report/unapplied.html:50
+#: src/accounting/templates/accounting/report/unapplied.html:52
+#: src/accounting/templates/accounting/report/unmatched.html:93
 msgid "Date"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
-#: src/accounting/report/reports/unapplied_accounts.py:109
+#: src/accounting/report/reports/unapplied_accounts.py:122
+#: src/accounting/report/reports/unmatched_accounts.py:122
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
-#: src/accounting/templates/accounting/report/trial-balance.html:55
+#: src/accounting/templates/accounting/report/trial-balance.html:61
 msgid "Account"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/ledger.py:366
-#: src/accounting/report/reports/unapplied.py:138
+#: src/accounting/report/reports/unapplied.py:149
+#: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
-#: src/accounting/templates/accounting/report/unapplied.html:52
+#: src/accounting/templates/accounting/report/unapplied.html:53
+#: src/accounting/templates/accounting/report/unmatched.html:94
 msgid "Description"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr ""
@@ -489,16 +503,18 @@
 #: src/accounting/report/reports/income_expenses.py:409
 #: src/accounting/templates/accounting/report/income-expenses.html:59
 msgid "Expense"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:409
 #: src/accounting/report/reports/ledger.py:368
+#: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
+#: src/accounting/templates/accounting/report/unmatched.html:97
 msgid "Balance"
 msgstr ""
 
 #: src/accounting/report/reports/income_expenses.py:410
 #: src/accounting/report/reports/journal.py:161
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
@@ -527,72 +543,96 @@
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:233
 msgid "net income or loss for current period"
 msgstr ""
 
 #: src/accounting/report/reports/income_statement.py:301
-#: src/accounting/report/reports/unapplied.py:138
+#: src/accounting/report/reports/unapplied.py:149
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
-#: src/accounting/templates/accounting/report/income-statement.html:55
-#: src/accounting/templates/accounting/report/unapplied.html:53
+#: src/accounting/templates/accounting/report/income-statement.html:61
+#: src/accounting/templates/accounting/report/unapplied.html:54
 msgid "Amount"
 msgstr ""
 
 #: src/accounting/report/reports/journal.py:158
-#: src/accounting/report/reports/unapplied.py:137
+#: src/accounting/report/reports/unapplied.py:148
+#: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form-currency.html:33
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
-#: src/accounting/templates/accounting/report/unapplied.html:51
 msgid "Currency"
 msgstr ""
 
 #: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:225
+#: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
-#: src/accounting/templates/accounting/report/trial-balance.html:56
+#: src/accounting/templates/accounting/report/trial-balance.html:62
+#: src/accounting/templates/accounting/report/unmatched.html:95
 msgid "Debit"
 msgstr ""
 
 #: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:226
+#: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
-#: src/accounting/templates/accounting/report/trial-balance.html:57
+#: src/accounting/templates/accounting/report/trial-balance.html:63
+#: src/accounting/templates/accounting/report/unmatched.html:96
 msgid "Credit"
 msgstr ""
 
-#: src/accounting/report/reports/unapplied.py:121
-#: src/accounting/report/reports/unapplied_accounts.py:93
+#: src/accounting/report/reports/unapplied.py:132
+#: src/accounting/report/reports/unapplied_accounts.py:107
+#: src/accounting/report/reports/unmatched.py:142
+#: src/accounting/report/reports/unmatched_accounts.py:107
 #: src/accounting/templates/accounting/include/nav.html:39
 msgid "Accounts"
 msgstr ""
 
-#: src/accounting/report/reports/unapplied.py:139
-#: src/accounting/templates/accounting/report/unapplied.html:54
+#: src/accounting/report/reports/unapplied.py:150
+#: src/accounting/templates/accounting/report/unapplied.html:55
 msgid "Net Balance"
 msgstr ""
 
-#: src/accounting/report/reports/unapplied_accounts.py:109
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:47
+#: src/accounting/report/reports/unapplied_accounts.py:122
+#: src/accounting/report/reports/unmatched_accounts.py:122
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:59
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:59
 msgid "Count"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:82
+#: src/accounting/report/utils/offset_matcher.py:163
+msgid "There is no unmatched offset."
+msgstr ""
+
+#: src/accounting/report/utils/offset_matcher.py:167
+#, python-format
+msgid "%(total)s unmatched offsets without original items."
+msgstr ""
+
+#: src/accounting/report/utils/offset_matcher.py:172
+#, python-format
+msgid ""
+"%(matches)s unmatched offsets out of %(total)s can match with their "
+"original items."
+msgstr ""
+
+#: src/accounting/report/utils/report_chooser.py:86
 #: src/accounting/templates/accounting/account/include/form.html:98
 #: src/accounting/templates/accounting/account/list.html:40
 #: src/accounting/templates/accounting/base-account/list.html:34
 #: src/accounting/templates/accounting/currency/list.html:40
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:34
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:34
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:34
@@ -600,122 +640,127 @@
 #: src/accounting/templates/accounting/report/include/search-modal.html:33
 #: src/accounting/templates/accounting/report/include/search-modal.html:38
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:64
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:126
 msgid "Search"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:93
+#: src/accounting/report/utils/report_chooser.py:97
 msgid "Income and Expenses Log"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:106
+#: src/accounting/report/utils/report_chooser.py:110
 msgid "Ledger"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:118
+#: src/accounting/report/utils/report_chooser.py:122
 msgid "Journal"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:128
+#: src/accounting/report/utils/report_chooser.py:132
 msgid "Trial Balance"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:139
+#: src/accounting/report/utils/report_chooser.py:143
 msgid "Income Statement"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:150
+#: src/accounting/report/utils/report_chooser.py:154
 msgid "Balance Sheet"
 msgstr ""
 
-#: src/accounting/report/utils/report_chooser.py:163
 #: src/accounting/report/utils/report_chooser.py:167
-msgid "Unapplied Original Line Items"
+#: src/accounting/report/utils/report_chooser.py:171
+msgid "Unapplied Items"
+msgstr ""
+
+#: src/accounting/report/utils/report_chooser.py:184
+#: src/accounting/report/utils/report_chooser.py:188
+msgid "Unmatched Offsets"
 msgstr ""
 
 #: src/accounting/static/js/account-form.js:206
 msgid "Please fill in the title."
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:951
-#: src/accounting/static/js/description-editor.js:1129
+#: src/accounting/static/js/description-editor.js:952
+#: src/accounting/static/js/description-editor.js:1130
 msgid "Please fill in the tag."
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:961
-#: src/accounting/static/js/description-editor.js:1149
+#: src/accounting/static/js/description-editor.js:962
+#: src/accounting/static/js/description-editor.js:1150
 msgid "Please fill in the origin."
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:971
-#: src/accounting/static/js/description-editor.js:1159
+#: src/accounting/static/js/description-editor.js:972
+#: src/accounting/static/js/description-editor.js:1160
 msgid "Please fill in the destination."
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1139
+#: src/accounting/static/js/description-editor.js:1140
 msgid "Please fill in the route."
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "January"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "February"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "March"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "April"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "May"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "June"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "July"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "August"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "September"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "October"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "November"
 msgstr ""
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "December"
 msgstr ""
 
-#: src/accounting/static/js/journal-entry-form.js:1070
+#: src/accounting/static/js/journal-entry-form.js:1085
 #: src/accounting/static/js/journal-entry-line-item-editor.js:430
 msgid "Please fill in the amount."
 msgstr ""
 
-#: src/accounting/static/js/journal-entry-form.js:1092
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:34
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:38
+#: src/accounting/static/js/journal-entry-form.js:1107
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:37
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:41
 #, python-format
 msgid "Offset %(item)s"
 msgstr ""
 
 #: src/accounting/static/js/period-chooser.js:270
 msgid "The date is too early."
 msgstr ""
@@ -750,15 +795,14 @@
 #: src/accounting/templates/accounting/base-account/detail.html:31
 #: src/accounting/templates/accounting/currency/detail.html:31
 #: src/accounting/templates/accounting/currency/include/form.html:33
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:31
 #: src/accounting/templates/accounting/journal-entry/include/form.html:38
 #: src/accounting/templates/accounting/journal-entry/order.html:36
 #: src/accounting/templates/accounting/option/form.html:36
-#: src/accounting/templates/accounting/unmatched-offset/list.html:31
 msgid "Back"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:36
 #: src/accounting/templates/accounting/currency/detail.html:36
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:36
 #: src/accounting/templates/accounting/option/detail.html:31
@@ -791,15 +835,15 @@
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
-#: src/accounting/templates/accounting/unmatched-offset/list.html:54
+#: src/accounting/templates/accounting/report/unmatched.html:58
 msgid "Close"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr ""
 
@@ -809,23 +853,23 @@
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
-#: src/accounting/templates/accounting/unmatched-offset/list.html:70
+#: src/accounting/templates/accounting/report/unmatched.html:74
 msgid "Cancel"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:85
 #: src/accounting/templates/accounting/report/include/period-chooser.html:141
-#: src/accounting/templates/accounting/unmatched-offset/list.html:71
+#: src/accounting/templates/accounting/report/unmatched.html:75
 msgid "Confirm"
 msgstr ""
 
 #: src/accounting/templates/accounting/account/detail.html:101
 #: src/accounting/templates/accounting/currency/detail.html:92
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:114
 msgid "Created"
@@ -865,30 +909,30 @@
 
 #: src/accounting/templates/accounting/account/include/form.html:109
 #: src/accounting/templates/accounting/account/list.html:68
 #: src/accounting/templates/accounting/account/order.html:81
 #: src/accounting/templates/accounting/base-account/list.html:51
 #: src/accounting/templates/accounting/currency/list.html:65
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:46
-#: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:51
+#: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:58
 #: src/accounting/templates/accounting/journal-entry/order.html:82
 #: src/accounting/templates/accounting/option/detail.html:67
 #: src/accounting/templates/accounting/option/detail.html:83
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:45
-#: src/accounting/templates/accounting/report/balance-sheet.html:110
+#: src/accounting/templates/accounting/report/balance-sheet.html:116
 #: src/accounting/templates/accounting/report/income-expenses.html:113
-#: src/accounting/templates/accounting/report/income-statement.html:96
+#: src/accounting/templates/accounting/report/income-statement.html:102
 #: src/accounting/templates/accounting/report/journal.html:103
 #: src/accounting/templates/accounting/report/ledger.html:116
 #: src/accounting/templates/accounting/report/search.html:100
-#: src/accounting/templates/accounting/report/trial-balance.html:82
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:61
-#: src/accounting/templates/accounting/report/unapplied.html:98
-#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:37
-#: src/accounting/templates/accounting/unmatched-offset/list.html:104
+#: src/accounting/templates/accounting/report/trial-balance.html:88
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:76
+#: src/accounting/templates/accounting/report/unapplied.html:90
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:76
+#: src/accounting/templates/accounting/report/unmatched.html:147
 msgid "There is no data."
 msgstr ""
 
 #: src/accounting/templates/accounting/account/order.html:29
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr ""
@@ -978,20 +1022,15 @@
 msgid "Base Accounts"
 msgstr ""
 
 #: src/accounting/templates/accounting/include/nav.html:51
 msgid "Currencies"
 msgstr ""
 
-#: src/accounting/templates/accounting/include/nav.html:57
-#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:24
-msgid "Unmatched Offsets"
-msgstr ""
-
-#: src/accounting/templates/accounting/include/nav.html:64
+#: src/accounting/templates/accounting/include/nav.html:58
 #: src/accounting/templates/accounting/option/detail.html:24
 #: src/accounting/templates/accounting/option/detail.html:41
 #: src/accounting/templates/accounting/option/form.html:29
 msgid "Settings"
 msgstr ""
 
 #: src/accounting/templates/accounting/include/pagination.html:23
@@ -1082,31 +1121,31 @@
 msgid "Route"
 msgstr ""
 
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:172
 msgid "The Number of Items"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:42
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:43
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:45
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:46
 msgid "Offsets"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:55
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:54
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:58
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:57
 msgid "Net balance"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:60
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:51
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:63
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:54
 msgid "Fully offset"
 msgstr ""
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:65
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:59
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:68
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:62
 msgid "Unmatched"
 msgstr ""
 
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:77
 msgid "Confirm Delete Journal Entry"
 msgstr ""
 
@@ -1211,151 +1250,167 @@
 msgstr ""
 
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
 msgid "Water bill for {last_bimonthly_name}"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/balance-sheet.html:29
-#: src/accounting/templates/accounting/report/balance-sheet.html:49
+#: src/accounting/templates/accounting/report/balance-sheet.html:51
+#, python-format
+msgid "Balance Sheet %(period)s"
+msgstr ""
+
+#: src/accounting/templates/accounting/report/balance-sheet.html:29
+#: src/accounting/templates/accounting/report/balance-sheet.html:53
 #, python-format
 msgid "Balance Sheet of %(currency)s %(period)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/income-expenses.html:29
 #, python-format
+msgid "Income and Expenses Log of %(account)s %(period)s"
+msgstr ""
+
+#: src/accounting/templates/accounting/report/income-expenses.html:29
+#, python-format
 msgid "Income and Expenses Log of %(account)s in %(currency)s %(period)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/income-statement.html:29
-#: src/accounting/templates/accounting/report/income-statement.html:49
+#: src/accounting/templates/accounting/report/income-statement.html:51
+#, python-format
+msgid "Income Statement %(period)s"
+msgstr ""
+
+#: src/accounting/templates/accounting/report/income-statement.html:29
+#: src/accounting/templates/accounting/report/income-statement.html:53
 #, python-format
 msgid "Income Statement of %(currency)s %(period)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/journal.html:29
 #, python-format
 msgid "Journal %(period)s"
 msgstr ""
 
 #: src/accounting/templates/accounting/report/ledger.html:29
 #, python-format
-msgid "Ledger of %(account)s in %(currency)s %(period)s"
+msgid "Ledger of %(account)s %(period)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/trial-balance.html:29
-#: src/accounting/templates/accounting/report/trial-balance.html:49
+#: src/accounting/templates/accounting/report/ledger.html:29
 #, python-format
-msgid "Trial Balance of %(currency)s %(period)s"
-msgstr ""
-
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:24
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:41
-msgid "Accounts with Unapplied Original Line Items"
+msgid "Ledger of %(account)s in %(currency)s %(period)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/unapplied.html:28
+#: src/accounting/templates/accounting/report/trial-balance.html:29
+#: src/accounting/templates/accounting/report/trial-balance.html:51
 #, python-format
-msgid "Unapplied Original Line Items of %(account)s"
+msgid "Trial Balance %(period)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/unapplied.html:65
+#: src/accounting/templates/accounting/report/trial-balance.html:29
+#: src/accounting/templates/accounting/report/trial-balance.html:53
 #, python-format
-msgid "Can match %(offset)s"
-msgstr ""
-
-#: src/accounting/templates/accounting/report/include/period-chooser.html:26
-msgid "Period Chooser"
-msgstr ""
-
-#: src/accounting/templates/accounting/report/include/period-chooser.html:34
-msgid "Month"
+msgid "Trial Balance of %(currency)s %(period)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/include/period-chooser.html:39
-msgid "Year"
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:29
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:49
+msgid "Accounts with Unapplied Items"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/include/period-chooser.html:44
-msgid "Day"
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:29
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:51
+#, python-format
+msgid "Accounts with Unapplied Items in %(currency)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/include/period-chooser.html:49
-msgid "Custom"
+#: src/accounting/templates/accounting/report/unapplied.html:29
+#, python-format
+msgid "Unapplied Items of %(account)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:50
-msgid "Report"
+#: src/accounting/templates/accounting/report/unapplied.html:29
+#, python-format
+msgid "Unapplied Items of %(account)s in %(currency)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:106
-msgid "Period"
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:29
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:49
+msgid "Accounts with Unmatched Offsets"
 msgstr ""
 
-#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:112
-#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:117
-msgid "Download"
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:29
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:51
+#, python-format
+msgid "Accounts with Unmatched Offsets in %(currency)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:24
+#: src/accounting/templates/accounting/report/unmatched.html:29
 #, python-format
-msgid "Unmatched Offsets in %(account)s"
+msgid "Unmatched Offsets of %(account)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:28
-msgid "Toolbar"
+#: src/accounting/templates/accounting/report/unmatched.html:29
+#, python-format
+msgid "Unmatched Offsets of %(account)s in %(currency)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:36
-#: src/accounting/templates/accounting/unmatched-offset/list.html:41
+#: src/accounting/templates/accounting/report/unmatched.html:47
 msgid "Match"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:53
+#: src/accounting/templates/accounting/report/unmatched.html:57
 msgid "Confirm Match Offsets"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:57
+#: src/accounting/templates/accounting/report/unmatched.html:61
 msgid ""
 "Do you really want to match the following original line items with their "
 "offsets?  This cannot be undone.  Please backup your database first, and "
 "review before you confirm."
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:81
+#: src/accounting/templates/accounting/report/unmatched.html:107
 #, python-format
-msgid ""
-"%(matches)s unapplied original line items out of %(total)s can match with"
-" their offsets."
+msgid "Can match %(item)s"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:83
-#, python-format
-msgid "%(total)s unapplied original line items without matching offsets."
+#: src/accounting/templates/accounting/report/include/period-chooser.html:26
+msgid "Period Chooser"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:85
-msgid "Go to unapplied original line items."
+#: src/accounting/templates/accounting/report/include/period-chooser.html:34
+msgid "Month"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:87
-msgid "All original line items are fully offset."
+#: src/accounting/templates/accounting/report/include/period-chooser.html:39
+msgid "Year"
 msgstr ""
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:98
-#, python-format
-msgid "Can match %(item)s"
+#: src/accounting/templates/accounting/report/include/period-chooser.html:44
+msgid "Day"
 msgstr ""
 
-#: src/accounting/unmatched_offset/views.py:71
-msgid "No more offset to match automatically."
+#: src/accounting/templates/accounting/report/include/period-chooser.html:49
+msgid "Custom"
 msgstr ""
 
-#: src/accounting/unmatched_offset/views.py:77
-#, python-format
-msgid "Matches %(matches)s from %(total)s unapplied line items."
+#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:50
+msgid "Report"
+msgstr ""
+
+#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:106
+msgid "Period"
+msgstr ""
+
+#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:112
+#: src/accounting/templates/accounting/report/include/toolbar-buttons.html:117
+msgid "Download"
 msgstr ""
 
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr ""
 
 #: src/accounting/utils/pagination.py:206
```

### Comparing `mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.4.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.1\n"
+"Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 01:41+0800\n"
-"PO-Revision-Date: 2023-04-09 01:41+0800\n"
+"POT-Creation-Date: 2023-04-18 09:32+0800\n"
+"PO-Revision-Date: 2023-04-18 09:32+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -19,20 +19,20 @@
 msgid "%(currency)s Settings"
 msgstr "%(currency)s设置"
 
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
 msgid ""
-"%(matches)s unapplied original line items out of %(total)s can match with "
-"their offsets."
-msgstr "%(total)s 笔未抵销原始分录中，可配对抵销掉 %(matches)s 笔。"
+"%(matches)s unmatched offsets out of %(total)s can match with their original "
+"items."
+msgstr "%(total)s 笔遗漏的抵销分录中，可配对抵销掉 %(matches)s 笔。"
 
-msgid "%(total)s unapplied original line items without matching offsets."
-msgstr "%(total)s 笔未抵销原始分录，无法自动配对抵销。"
+msgid "%(total)s unmatched offsets without original items."
+msgstr "%(total)s 笔遗漏的抵销分录无法自动抵销。"
 
 msgid "(Unknown)"
 msgstr "（不明）"
 
 msgid "A nominal account does not need offset."
 msgstr "虚科目不需抵销。"
 
@@ -50,16 +50,25 @@
 
 msgid "Accounting"
 msgstr "记帐"
 
 msgid "Accounts"
 msgstr "科目"
 
-msgid "Accounts with Unapplied Original Line Items"
-msgstr "有未抵销原始分录的科目"
+msgid "Accounts with Unapplied Items"
+msgstr "含未抵销项目的科目"
+
+msgid "Accounts with Unapplied Items in %(currency)s"
+msgstr "%(currency)s含未抵销项目的科目"
+
+msgid "Accounts with Unmatched Offsets"
+msgstr "含遗漏抵销项目的科目"
+
+msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgstr "%(currency)s含遗漏抵销项目的科目"
 
 msgid "Add a New Account"
 msgstr "添加科目"
 
 msgid "Add a New Cash Disbursement Journal Entry"
 msgstr "添加现金支出传票"
 
@@ -71,17 +80,14 @@
 
 msgid "Add a New Transfer Journal Entry"
 msgstr "添加转帐传票"
 
 msgid "All"
 msgstr "全部"
 
-msgid "All original line items are fully offset."
-msgstr "原始分录已全部抵销。"
-
 msgid "Amount"
 msgstr "金额"
 
 msgid "Annotation"
 msgstr "注记"
 
 msgid "April"
@@ -101,14 +107,17 @@
 
 msgid "Balance"
 msgstr "余额"
 
 msgid "Balance Sheet"
 msgstr "资产负债表"
 
+msgid "Balance Sheet %(period)s"
+msgstr "%(period)s资产负债表"
+
 msgid "Balance Sheet of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s资产负债表"
 
 msgid "Base Account Managements"
 msgstr "基本科目管理"
 
 msgid "Base Accounts"
@@ -122,17 +131,14 @@
 
 msgid "Bus"
 msgstr "公车"
 
 msgid "Can match %(item)s"
 msgstr "可抵销 %(item)s"
 
-msgid "Can match %(offset)s"
-msgstr "可抵销 %(offset)s"
-
 msgid "Cancel"
 msgstr "取消"
 
 msgid "Cash Disbursement"
 msgstr "现金支出"
 
 msgid "Cash Disbursement Journal Entry#%(id)s"
@@ -265,29 +271,32 @@
 
 msgid "Fully offset"
 msgstr "全部抵销"
 
 msgid "General"
 msgstr "一般"
 
-msgid "Go to unapplied original line items."
-msgstr "查阅未抵销原始分录。"
-
 msgid "Income"
 msgstr "收入"
 
 msgid "Income Statement"
 msgstr "损益表"
 
+msgid "Income Statement %(period)s"
+msgstr "%(period)s损益表"
+
 msgid "Income Statement of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s损益表"
 
 msgid "Income and Expenses Log"
 msgstr "收支帐"
 
+msgid "Income and Expenses Log of %(account)s %(period)s"
+msgstr "%(period)s%(account)s收支帐"
+
 msgid "Income and Expenses Log of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s收支帐"
 
 msgid "January"
 msgstr "一月"
 
 msgid "Journal"
@@ -316,14 +325,17 @@
 
 msgid "Last month, in its name."
 msgstr "上个月的名称。"
 
 msgid "Ledger"
 msgstr "分类帐"
 
+msgid "Ledger of %(account)s %(period)s"
+msgstr "%(period)s%(account)s分类帐"
+
 msgid "Ledger of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s分类帐"
 
 msgid "Line Item Content"
 msgstr "分录内容"
 
 msgid "Line items with offset cannot be deleted."
@@ -331,16 +343,16 @@
 
 msgid "March"
 msgstr "三月"
 
 msgid "Match"
 msgstr "抵销"
 
-msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches)s 笔。"
+msgid "Matched %(matches)s offsets."
+msgstr "抵销了 %(matches)s 笔。"
 
 msgid "May"
 msgstr "五月"
 
 msgid "Month"
 msgstr "月"
 
@@ -659,14 +671,17 @@
 
 msgid "The totals of the debit and credit amounts do not match."
 msgstr "借方贷方合计不符。 "
 
 msgid "There is no data."
 msgstr "没有数据。"
 
+msgid "There is no unmatched offset."
+msgstr "没有遗漏的抵销分录"
+
 msgid "This Month"
 msgstr "这个月"
 
 msgid "This Year"
 msgstr "今年"
 
 msgid "This account is not for credit line items."
@@ -701,17 +716,14 @@
 
 msgid "Today"
 msgstr "今天"
 
 msgid "Tomorrow"
 msgstr "明天"
 
-msgid "Toolbar"
-msgstr "工具列"
-
 msgid "Total"
 msgstr "合计"
 
 msgid "Transfer"
 msgstr "转帐"
 
 msgid "Transfer Journal Entry#%(id)s"
@@ -719,31 +731,40 @@
 
 msgid "Travel"
 msgstr "差旅"
 
 msgid "Trial Balance"
 msgstr "试算表"
 
+msgid "Trial Balance %(period)s"
+msgstr "%(period)s试算表"
+
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s试算表"
 
-msgid "Unapplied Original Line Items"
-msgstr "未抵销原始分录"
+msgid "Unapplied Items"
+msgstr "未抵销项目"
+
+msgid "Unapplied Items of %(account)s"
+msgstr "%(account)s未抵销项目"
 
-msgid "Unapplied Original Line Items of %(account)s"
-msgstr "%(account)s未抵销原始分录"
+msgid "Unapplied Items of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s未抵销项目"
 
 msgid "Unmatched"
 msgstr "未抵销"
 
 msgid "Unmatched Offsets"
-msgstr "遗漏的抵销分录"
+msgstr "遗漏的抵销项目"
+
+msgid "Unmatched Offsets of %(account)s"
+msgstr "%(account)s遗漏的抵销项目"
 
-msgid "Unmatched Offsets in %(account)s"
-msgstr "%(account)s遗漏的抵销分录"
+msgid "Unmatched Offsets of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s遗漏的抵销项目"
 
 msgid "Updated"
 msgstr "更新"
 
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水费{last_bimonthly_number}月"
```

### Comparing `mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.4.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # Copyright (C) 2023 imacat
 # This file is distributed under the same license as the Mia! Accounting
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.1\n"
+"Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 01:41+0800\n"
-"PO-Revision-Date: 2023-04-09 01:41+0800\n"
+"POT-Creation-Date: 2023-04-18 09:32+0800\n"
+"PO-Revision-Date: 2023-04-18 09:32+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hans\n"
 "Language-Team: zh_Hans <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: src/accounting/forms.py:33
-#: src/accounting/static/js/journal-entry-form.js:1065
+#: src/accounting/static/js/journal-entry-form.js:1080
 #: src/accounting/static/js/journal-entry-line-item-editor.js:411
 #: src/accounting/static/js/option-form.js:537
 #: src/accounting/static/js/option-form.js:803
 msgid "Please select the account."
 msgstr "请选择科目。"
 
 #: src/accounting/forms.py:44
@@ -298,19 +298,19 @@
 
 #: src/accounting/journal_entry/forms/line_item.py:241
 #: src/accounting/static/js/journal-entry-line-item-editor.js:450
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr "金额不可低于抵销总额 %(total)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:413
+#: src/accounting/journal_entry/forms/line_item.py:426
 msgid "This account is not for debit line items."
 msgstr "科目不是借方科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:465
+#: src/accounting/journal_entry/forms/line_item.py:478
 msgid "This account is not for credit line items."
 msgstr "科目不是贷方科目。"
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr "这不是流动科目。"
 
@@ -350,14 +350,23 @@
 msgid "The settings were not modified."
 msgstr "设置未异动。"
 
 #: src/accounting/option/views.py:82
 msgid "The settings are saved successfully."
 msgstr "设置存好了。"
 
+#: src/accounting/report/views.py:401
+msgid "No more offset to match automatically."
+msgstr "无法自动配对抵销。"
+
+#: src/accounting/report/views.py:408
+#, python-format
+msgid "Matched %(matches)s offsets."
+msgstr "抵销了 %(matches)s 笔。"
+
 #: src/accounting/report/period/description.py:33
 msgid "for all time"
 msgstr "全部"
 
 #: src/accounting/report/period/description.py:67
 #, python-format
 msgid "since %(start)s"
@@ -419,71 +428,76 @@
 #: src/accounting/report/reports/ledger.py:380
 #: src/accounting/report/reports/trial_balance.py:229
 #: src/accounting/templates/accounting/journal-entry/disbursement/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html:38
 #: src/accounting/templates/accounting/journal-entry/receipt/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:39
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:55
-#: src/accounting/templates/accounting/report/balance-sheet.html:59
-#: src/accounting/templates/accounting/report/balance-sheet.html:71
-#: src/accounting/templates/accounting/report/balance-sheet.html:81
+#: src/accounting/templates/accounting/report/balance-sheet.html:65
+#: src/accounting/templates/accounting/report/balance-sheet.html:77
 #: src/accounting/templates/accounting/report/balance-sheet.html:87
-#: src/accounting/templates/accounting/report/balance-sheet.html:96
-#: src/accounting/templates/accounting/report/balance-sheet.html:103
+#: src/accounting/templates/accounting/report/balance-sheet.html:93
+#: src/accounting/templates/accounting/report/balance-sheet.html:102
+#: src/accounting/templates/accounting/report/balance-sheet.html:109
 #: src/accounting/templates/accounting/report/income-expenses.html:81
-#: src/accounting/templates/accounting/report/income-statement.html:83
+#: src/accounting/templates/accounting/report/income-statement.html:89
 #: src/accounting/templates/accounting/report/ledger.html:82
-#: src/accounting/templates/accounting/report/trial-balance.html:74
+#: src/accounting/templates/accounting/report/trial-balance.html:80
 msgid "Total"
 msgstr "合计"
 
 #: src/accounting/report/reports/income_expenses.py:136
 #: src/accounting/report/reports/ledger.py:132
 msgid "Brought forward"
 msgstr "前期转入"
 
 #: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/ledger.py:366
-#: src/accounting/report/reports/unapplied.py:137
+#: src/accounting/report/reports/unapplied.py:148
+#: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
-#: src/accounting/templates/accounting/report/unapplied.html:50
+#: src/accounting/templates/accounting/report/unapplied.html:52
+#: src/accounting/templates/accounting/report/unmatched.html:93
 msgid "Date"
 msgstr "日期"
 
 #: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
-#: src/accounting/report/reports/unapplied_accounts.py:109
+#: src/accounting/report/reports/unapplied_accounts.py:122
+#: src/accounting/report/reports/unmatched_accounts.py:122
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
-#: src/accounting/templates/accounting/report/trial-balance.html:55
+#: src/accounting/templates/accounting/report/trial-balance.html:61
 msgid "Account"
 msgstr "科目"
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/ledger.py:366
-#: src/accounting/report/reports/unapplied.py:138
+#: src/accounting/report/reports/unapplied.py:149
+#: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
-#: src/accounting/templates/accounting/report/unapplied.html:52
+#: src/accounting/templates/accounting/report/unapplied.html:53
+#: src/accounting/templates/accounting/report/unmatched.html:94
 msgid "Description"
 msgstr "摘要"
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr "收入"
@@ -491,16 +505,18 @@
 #: src/accounting/report/reports/income_expenses.py:409
 #: src/accounting/templates/accounting/report/income-expenses.html:59
 msgid "Expense"
 msgstr "支出"
 
 #: src/accounting/report/reports/income_expenses.py:409
 #: src/accounting/report/reports/ledger.py:368
+#: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
+#: src/accounting/templates/accounting/report/unmatched.html:97
 msgid "Balance"
 msgstr "余额"
 
 #: src/accounting/report/reports/income_expenses.py:410
 #: src/accounting/report/reports/journal.py:161
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
@@ -529,72 +545,96 @@
 msgstr "税后净利"
 
 #: src/accounting/report/reports/income_statement.py:233
 msgid "net income or loss for current period"
 msgstr "本期损益"
 
 #: src/accounting/report/reports/income_statement.py:301
-#: src/accounting/report/reports/unapplied.py:138
+#: src/accounting/report/reports/unapplied.py:149
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
-#: src/accounting/templates/accounting/report/income-statement.html:55
-#: src/accounting/templates/accounting/report/unapplied.html:53
+#: src/accounting/templates/accounting/report/income-statement.html:61
+#: src/accounting/templates/accounting/report/unapplied.html:54
 msgid "Amount"
 msgstr "金额"
 
 #: src/accounting/report/reports/journal.py:158
-#: src/accounting/report/reports/unapplied.py:137
+#: src/accounting/report/reports/unapplied.py:148
+#: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form-currency.html:33
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
-#: src/accounting/templates/accounting/report/unapplied.html:51
 msgid "Currency"
 msgstr "货币"
 
 #: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:225
+#: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
-#: src/accounting/templates/accounting/report/trial-balance.html:56
+#: src/accounting/templates/accounting/report/trial-balance.html:62
+#: src/accounting/templates/accounting/report/unmatched.html:95
 msgid "Debit"
 msgstr "借方"
 
 #: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:226
+#: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
-#: src/accounting/templates/accounting/report/trial-balance.html:57
+#: src/accounting/templates/accounting/report/trial-balance.html:63
+#: src/accounting/templates/accounting/report/unmatched.html:96
 msgid "Credit"
 msgstr "贷方"
 
-#: src/accounting/report/reports/unapplied.py:121
-#: src/accounting/report/reports/unapplied_accounts.py:93
+#: src/accounting/report/reports/unapplied.py:132
+#: src/accounting/report/reports/unapplied_accounts.py:107
+#: src/accounting/report/reports/unmatched.py:142
+#: src/accounting/report/reports/unmatched_accounts.py:107
 #: src/accounting/templates/accounting/include/nav.html:39
 msgid "Accounts"
 msgstr "科目"
 
-#: src/accounting/report/reports/unapplied.py:139
-#: src/accounting/templates/accounting/report/unapplied.html:54
+#: src/accounting/report/reports/unapplied.py:150
+#: src/accounting/templates/accounting/report/unapplied.html:55
 msgid "Net Balance"
 msgstr "净额"
 
-#: src/accounting/report/reports/unapplied_accounts.py:109
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:47
+#: src/accounting/report/reports/unapplied_accounts.py:122
+#: src/accounting/report/reports/unmatched_accounts.py:122
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:59
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:59
 msgid "Count"
 msgstr "数量"
 
-#: src/accounting/report/utils/report_chooser.py:82
+#: src/accounting/report/utils/offset_matcher.py:163
+msgid "There is no unmatched offset."
+msgstr "没有遗漏的抵销分录"
+
+#: src/accounting/report/utils/offset_matcher.py:167
+#, python-format
+msgid "%(total)s unmatched offsets without original items."
+msgstr "%(total)s 笔遗漏的抵销分录无法自动抵销。"
+
+#: src/accounting/report/utils/offset_matcher.py:172
+#, python-format
+msgid ""
+"%(matches)s unmatched offsets out of %(total)s can match with their "
+"original items."
+msgstr "%(total)s 笔遗漏的抵销分录中，可配对抵销掉 %(matches)s 笔。"
+
+#: src/accounting/report/utils/report_chooser.py:86
 #: src/accounting/templates/accounting/account/include/form.html:98
 #: src/accounting/templates/accounting/account/list.html:40
 #: src/accounting/templates/accounting/base-account/list.html:34
 #: src/accounting/templates/accounting/currency/list.html:40
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:34
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:34
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:34
@@ -602,122 +642,127 @@
 #: src/accounting/templates/accounting/report/include/search-modal.html:33
 #: src/accounting/templates/accounting/report/include/search-modal.html:38
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:64
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:126
 msgid "Search"
 msgstr "搜索"
 
-#: src/accounting/report/utils/report_chooser.py:93
+#: src/accounting/report/utils/report_chooser.py:97
 msgid "Income and Expenses Log"
 msgstr "收支帐"
 
-#: src/accounting/report/utils/report_chooser.py:106
+#: src/accounting/report/utils/report_chooser.py:110
 msgid "Ledger"
 msgstr "分类帐"
 
-#: src/accounting/report/utils/report_chooser.py:118
+#: src/accounting/report/utils/report_chooser.py:122
 msgid "Journal"
 msgstr "日记簿"
 
-#: src/accounting/report/utils/report_chooser.py:128
+#: src/accounting/report/utils/report_chooser.py:132
 msgid "Trial Balance"
 msgstr "试算表"
 
-#: src/accounting/report/utils/report_chooser.py:139
+#: src/accounting/report/utils/report_chooser.py:143
 msgid "Income Statement"
 msgstr "损益表"
 
-#: src/accounting/report/utils/report_chooser.py:150
+#: src/accounting/report/utils/report_chooser.py:154
 msgid "Balance Sheet"
 msgstr "资产负债表"
 
-#: src/accounting/report/utils/report_chooser.py:163
 #: src/accounting/report/utils/report_chooser.py:167
-msgid "Unapplied Original Line Items"
-msgstr "未抵销原始分录"
+#: src/accounting/report/utils/report_chooser.py:171
+msgid "Unapplied Items"
+msgstr "未抵销项目"
+
+#: src/accounting/report/utils/report_chooser.py:184
+#: src/accounting/report/utils/report_chooser.py:188
+msgid "Unmatched Offsets"
+msgstr "遗漏的抵销项目"
 
 #: src/accounting/static/js/account-form.js:206
 msgid "Please fill in the title."
 msgstr "请填上标题。"
 
-#: src/accounting/static/js/description-editor.js:951
-#: src/accounting/static/js/description-editor.js:1129
+#: src/accounting/static/js/description-editor.js:952
+#: src/accounting/static/js/description-editor.js:1130
 msgid "Please fill in the tag."
 msgstr "请填上标签。"
 
-#: src/accounting/static/js/description-editor.js:961
-#: src/accounting/static/js/description-editor.js:1149
+#: src/accounting/static/js/description-editor.js:962
+#: src/accounting/static/js/description-editor.js:1150
 msgid "Please fill in the origin."
 msgstr "请填上起点。"
 
-#: src/accounting/static/js/description-editor.js:971
-#: src/accounting/static/js/description-editor.js:1159
+#: src/accounting/static/js/description-editor.js:972
+#: src/accounting/static/js/description-editor.js:1160
 msgid "Please fill in the destination."
 msgstr "请填上终点。"
 
-#: src/accounting/static/js/description-editor.js:1139
+#: src/accounting/static/js/description-editor.js:1140
 msgid "Please fill in the route."
 msgstr "请填上路线名称。"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "January"
 msgstr "一月"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "February"
 msgstr "二月"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "March"
 msgstr "三月"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "April"
 msgstr "四月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "May"
 msgstr "五月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "June"
 msgstr "六月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "July"
 msgstr "七月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "August"
 msgstr "八月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "September"
 msgstr "九月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "October"
 msgstr "十月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "November"
 msgstr "十一月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "December"
 msgstr "十二月"
 
-#: src/accounting/static/js/journal-entry-form.js:1070
+#: src/accounting/static/js/journal-entry-form.js:1085
 #: src/accounting/static/js/journal-entry-line-item-editor.js:430
 msgid "Please fill in the amount."
 msgstr "请填上金额。"
 
-#: src/accounting/static/js/journal-entry-form.js:1092
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:34
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:38
+#: src/accounting/static/js/journal-entry-form.js:1107
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:37
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:41
 #, python-format
 msgid "Offset %(item)s"
 msgstr "抵销 %(item)s"
 
 #: src/accounting/static/js/period-chooser.js:270
 msgid "The date is too early."
 msgstr "日期太早。"
@@ -752,15 +797,14 @@
 #: src/accounting/templates/accounting/base-account/detail.html:31
 #: src/accounting/templates/accounting/currency/detail.html:31
 #: src/accounting/templates/accounting/currency/include/form.html:33
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:31
 #: src/accounting/templates/accounting/journal-entry/include/form.html:38
 #: src/accounting/templates/accounting/journal-entry/order.html:36
 #: src/accounting/templates/accounting/option/form.html:36
-#: src/accounting/templates/accounting/unmatched-offset/list.html:31
 msgid "Back"
 msgstr "回上页"
 
 #: src/accounting/templates/accounting/account/detail.html:36
 #: src/accounting/templates/accounting/currency/detail.html:36
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:36
 #: src/accounting/templates/accounting/option/detail.html:31
@@ -793,15 +837,15 @@
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
-#: src/accounting/templates/accounting/unmatched-offset/list.html:54
+#: src/accounting/templates/accounting/report/unmatched.html:58
 msgid "Close"
 msgstr "关闭"
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr "你确定要删掉这个科目吗？"
 
@@ -811,23 +855,23 @@
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
-#: src/accounting/templates/accounting/unmatched-offset/list.html:70
+#: src/accounting/templates/accounting/report/unmatched.html:74
 msgid "Cancel"
 msgstr "取消"
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:85
 #: src/accounting/templates/accounting/report/include/period-chooser.html:141
-#: src/accounting/templates/accounting/unmatched-offset/list.html:71
+#: src/accounting/templates/accounting/report/unmatched.html:75
 msgid "Confirm"
 msgstr "确定"
 
 #: src/accounting/templates/accounting/account/detail.html:101
 #: src/accounting/templates/accounting/currency/detail.html:92
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:114
 msgid "Created"
@@ -867,30 +911,30 @@
 
 #: src/accounting/templates/accounting/account/include/form.html:109
 #: src/accounting/templates/accounting/account/list.html:68
 #: src/accounting/templates/accounting/account/order.html:81
 #: src/accounting/templates/accounting/base-account/list.html:51
 #: src/accounting/templates/accounting/currency/list.html:65
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:46
-#: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:51
+#: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:58
 #: src/accounting/templates/accounting/journal-entry/order.html:82
 #: src/accounting/templates/accounting/option/detail.html:67
 #: src/accounting/templates/accounting/option/detail.html:83
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:45
-#: src/accounting/templates/accounting/report/balance-sheet.html:110
+#: src/accounting/templates/accounting/report/balance-sheet.html:116
 #: src/accounting/templates/accounting/report/income-expenses.html:113
-#: src/accounting/templates/accounting/report/income-statement.html:96
+#: src/accounting/templates/accounting/report/income-statement.html:102
 #: src/accounting/templates/accounting/report/journal.html:103
 #: src/accounting/templates/accounting/report/ledger.html:116
 #: src/accounting/templates/accounting/report/search.html:100
-#: src/accounting/templates/accounting/report/trial-balance.html:82
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:61
-#: src/accounting/templates/accounting/report/unapplied.html:98
-#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:37
-#: src/accounting/templates/accounting/unmatched-offset/list.html:104
+#: src/accounting/templates/accounting/report/trial-balance.html:88
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:76
+#: src/accounting/templates/accounting/report/unapplied.html:90
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:76
+#: src/accounting/templates/accounting/report/unmatched.html:147
 msgid "There is no data."
 msgstr "没有数据。"
 
 #: src/accounting/templates/accounting/account/order.html:29
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr "%(base)s下的科目"
@@ -980,20 +1024,15 @@
 msgid "Base Accounts"
 msgstr "基本科目"
 
 #: src/accounting/templates/accounting/include/nav.html:51
 msgid "Currencies"
 msgstr "货币"
 
-#: src/accounting/templates/accounting/include/nav.html:57
-#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:24
-msgid "Unmatched Offsets"
-msgstr "遗漏的抵销分录"
-
-#: src/accounting/templates/accounting/include/nav.html:64
+#: src/accounting/templates/accounting/include/nav.html:58
 #: src/accounting/templates/accounting/option/detail.html:24
 #: src/accounting/templates/accounting/option/detail.html:41
 #: src/accounting/templates/accounting/option/form.html:29
 msgid "Settings"
 msgstr "设置"
 
 #: src/accounting/templates/accounting/include/pagination.html:23
@@ -1084,31 +1123,31 @@
 msgid "Route"
 msgstr "路线"
 
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:172
 msgid "The Number of Items"
 msgstr "数量"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:42
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:43
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:45
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:46
 msgid "Offsets"
 msgstr "抵销"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:55
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:54
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:58
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:57
 msgid "Net balance"
 msgstr "净额"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:60
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:51
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:63
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:54
 msgid "Fully offset"
 msgstr "全部抵销"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:65
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:59
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:68
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:62
 msgid "Unmatched"
 msgstr "未抵销"
 
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:77
 msgid "Confirm Delete Journal Entry"
 msgstr "确认删除传票"
 
@@ -1213,60 +1252,135 @@
 msgstr "范例："
 
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水费{last_bimonthly_number}月"
 
 #: src/accounting/templates/accounting/report/balance-sheet.html:29
-#: src/accounting/templates/accounting/report/balance-sheet.html:49
+#: src/accounting/templates/accounting/report/balance-sheet.html:51
+#, python-format
+msgid "Balance Sheet %(period)s"
+msgstr "%(period)s资产负债表"
+
+#: src/accounting/templates/accounting/report/balance-sheet.html:29
+#: src/accounting/templates/accounting/report/balance-sheet.html:53
 #, python-format
 msgid "Balance Sheet of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s资产负债表"
 
 #: src/accounting/templates/accounting/report/income-expenses.html:29
 #, python-format
+msgid "Income and Expenses Log of %(account)s %(period)s"
+msgstr "%(period)s%(account)s收支帐"
+
+#: src/accounting/templates/accounting/report/income-expenses.html:29
+#, python-format
 msgid "Income and Expenses Log of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s收支帐"
 
 #: src/accounting/templates/accounting/report/income-statement.html:29
-#: src/accounting/templates/accounting/report/income-statement.html:49
+#: src/accounting/templates/accounting/report/income-statement.html:51
+#, python-format
+msgid "Income Statement %(period)s"
+msgstr "%(period)s损益表"
+
+#: src/accounting/templates/accounting/report/income-statement.html:29
+#: src/accounting/templates/accounting/report/income-statement.html:53
 #, python-format
 msgid "Income Statement of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s损益表"
 
 #: src/accounting/templates/accounting/report/journal.html:29
 #, python-format
 msgid "Journal %(period)s"
 msgstr "%(period)s日记簿"
 
 #: src/accounting/templates/accounting/report/ledger.html:29
 #, python-format
+msgid "Ledger of %(account)s %(period)s"
+msgstr "%(period)s%(account)s分类帐"
+
+#: src/accounting/templates/accounting/report/ledger.html:29
+#, python-format
 msgid "Ledger of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s分类帐"
 
 #: src/accounting/templates/accounting/report/trial-balance.html:29
-#: src/accounting/templates/accounting/report/trial-balance.html:49
+#: src/accounting/templates/accounting/report/trial-balance.html:51
+#, python-format
+msgid "Trial Balance %(period)s"
+msgstr "%(period)s试算表"
+
+#: src/accounting/templates/accounting/report/trial-balance.html:29
+#: src/accounting/templates/accounting/report/trial-balance.html:53
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s试算表"
 
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:24
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:41
-msgid "Accounts with Unapplied Original Line Items"
-msgstr "有未抵销原始分录的科目"
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:29
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:49
+msgid "Accounts with Unapplied Items"
+msgstr "含未抵销项目的科目"
+
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:29
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:51
+#, python-format
+msgid "Accounts with Unapplied Items in %(currency)s"
+msgstr "%(currency)s含未抵销项目的科目"
+
+#: src/accounting/templates/accounting/report/unapplied.html:29
+#, python-format
+msgid "Unapplied Items of %(account)s"
+msgstr "%(account)s未抵销项目"
+
+#: src/accounting/templates/accounting/report/unapplied.html:29
+#, python-format
+msgid "Unapplied Items of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s未抵销项目"
+
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:29
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:49
+msgid "Accounts with Unmatched Offsets"
+msgstr "含遗漏抵销项目的科目"
+
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:29
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:51
+#, python-format
+msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgstr "%(currency)s含遗漏抵销项目的科目"
+
+#: src/accounting/templates/accounting/report/unmatched.html:29
+#, python-format
+msgid "Unmatched Offsets of %(account)s"
+msgstr "%(account)s遗漏的抵销项目"
 
-#: src/accounting/templates/accounting/report/unapplied.html:28
+#: src/accounting/templates/accounting/report/unmatched.html:29
 #, python-format
-msgid "Unapplied Original Line Items of %(account)s"
-msgstr "%(account)s未抵销原始分录"
+msgid "Unmatched Offsets of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s遗漏的抵销项目"
+
+#: src/accounting/templates/accounting/report/unmatched.html:47
+msgid "Match"
+msgstr "抵销"
+
+#: src/accounting/templates/accounting/report/unmatched.html:57
+msgid "Confirm Match Offsets"
+msgstr "确认抵销"
+
+#: src/accounting/templates/accounting/report/unmatched.html:61
+msgid ""
+"Do you really want to match the following original line items with their "
+"offsets?  This cannot be undone.  Please backup your database first, and "
+"review before you confirm."
+msgstr "你确定要抵销下列原始分录与抵销分录吗？结果无法复原。请先备份数据库，并仔细核对抵销分录是否正确。"
 
-#: src/accounting/templates/accounting/report/unapplied.html:65
+#: src/accounting/templates/accounting/report/unmatched.html:107
 #, python-format
-msgid "Can match %(offset)s"
-msgstr "可抵销 %(offset)s"
+msgid "Can match %(item)s"
+msgstr "可抵销 %(item)s"
 
 #: src/accounting/templates/accounting/report/include/period-chooser.html:26
 msgid "Period Chooser"
 msgstr "选择日期范围"
 
 #: src/accounting/templates/accounting/report/include/period-chooser.html:34
 msgid "Month"
@@ -1293,73 +1407,14 @@
 msgstr "期间"
 
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:112
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:117
 msgid "Download"
 msgstr "下载"
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:24
-#, python-format
-msgid "Unmatched Offsets in %(account)s"
-msgstr "%(account)s遗漏的抵销分录"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:28
-msgid "Toolbar"
-msgstr "工具列"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:36
-#: src/accounting/templates/accounting/unmatched-offset/list.html:41
-msgid "Match"
-msgstr "抵销"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:53
-msgid "Confirm Match Offsets"
-msgstr "确认抵销"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:57
-msgid ""
-"Do you really want to match the following original line items with their "
-"offsets?  This cannot be undone.  Please backup your database first, and "
-"review before you confirm."
-msgstr "你确定要抵销下列原始分录与抵销分录吗？结果无法复原。请先备份数据库，并仔细核对抵销分录是否正确。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:81
-#, python-format
-msgid ""
-"%(matches)s unapplied original line items out of %(total)s can match with"
-" their offsets."
-msgstr "%(total)s 笔未抵销原始分录中，可配对抵销掉 %(matches)s 笔。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:83
-#, python-format
-msgid "%(total)s unapplied original line items without matching offsets."
-msgstr "%(total)s 笔未抵销原始分录，无法自动配对抵销。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:85
-msgid "Go to unapplied original line items."
-msgstr "查阅未抵销原始分录。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:87
-msgid "All original line items are fully offset."
-msgstr "原始分录已全部抵销。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:98
-#, python-format
-msgid "Can match %(item)s"
-msgstr "可抵销 %(item)s"
-
-#: src/accounting/unmatched_offset/views.py:71
-msgid "No more offset to match automatically."
-msgstr "无法自动配对抵销。"
-
-#: src/accounting/unmatched_offset/views.py:77
-#, python-format
-msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 笔未抵销原始分录中，配对抵销掉 %(matches)s 笔。"
-
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流动资产与负债"
 
 #: src/accounting/utils/pagination.py:206
 msgctxt "Pagination|"
 msgid "Previous"
```

### Comparing `mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.4.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.1\n"
+"Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 01:41+0800\n"
-"PO-Revision-Date: 2023-04-09 01:41+0800\n"
+"POT-Creation-Date: 2023-04-18 09:32+0800\n"
+"PO-Revision-Date: 2023-04-18 09:32+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -19,20 +19,20 @@
 msgid "%(currency)s Settings"
 msgstr "%(currency)s設定"
 
 msgid "%(date)s %(description)s %(amount)s"
 msgstr "%(date)s %(description)s %(amount)s"
 
 msgid ""
-"%(matches)s unapplied original line items out of %(total)s can match with "
-"their offsets."
-msgstr "%(total)s 筆未抵銷原始分錄中，可配對抵銷掉 %(matches)s 筆。"
+"%(matches)s unmatched offsets out of %(total)s can match with their original "
+"items."
+msgstr "%(total)s 筆遺漏的抵銷分錄中，可配對抵銷掉 %(matches)s 筆。"
 
-msgid "%(total)s unapplied original line items without matching offsets."
-msgstr "%(total)s 筆未抵銷原始分錄，無法自動配對抵銷。"
+msgid "%(total)s unmatched offsets without original items."
+msgstr "%(total)s 筆遺漏的抵銷分錄無法自動抵銷。"
 
 msgid "(Unknown)"
 msgstr "（不明）"
 
 msgid "A nominal account does not need offset."
 msgstr "虛科目不需抵銷。"
 
@@ -50,16 +50,25 @@
 
 msgid "Accounting"
 msgstr "記帳"
 
 msgid "Accounts"
 msgstr "科目"
 
-msgid "Accounts with Unapplied Original Line Items"
-msgstr "有未抵銷原始分錄的科目"
+msgid "Accounts with Unapplied Items"
+msgstr "含未抵銷項目的科目"
+
+msgid "Accounts with Unapplied Items in %(currency)s"
+msgstr "%(currency)s含未抵銷項目的科目"
+
+msgid "Accounts with Unmatched Offsets"
+msgstr "含遺漏抵銷項目的科目"
+
+msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgstr "%(currency)s含遺漏抵銷項目的科目"
 
 msgid "Add a New Account"
 msgstr "新增科目"
 
 msgid "Add a New Cash Disbursement Journal Entry"
 msgstr "新增現金支出傳票"
 
@@ -71,17 +80,14 @@
 
 msgid "Add a New Transfer Journal Entry"
 msgstr "新增轉帳傳票"
 
 msgid "All"
 msgstr "全部"
 
-msgid "All original line items are fully offset."
-msgstr "原始分錄已全部抵銷。"
-
 msgid "Amount"
 msgstr "金額"
 
 msgid "Annotation"
 msgstr "註記"
 
 msgid "April"
@@ -101,14 +107,17 @@
 
 msgid "Balance"
 msgstr "餘額"
 
 msgid "Balance Sheet"
 msgstr "資產負債表"
 
+msgid "Balance Sheet %(period)s"
+msgstr "%(period)s資產負債表"
+
 msgid "Balance Sheet of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s資產負債表"
 
 msgid "Base Account Managements"
 msgstr "基本科目管理"
 
 msgid "Base Accounts"
@@ -122,17 +131,14 @@
 
 msgid "Bus"
 msgstr "公車"
 
 msgid "Can match %(item)s"
 msgstr "可抵銷 %(item)s"
 
-msgid "Can match %(offset)s"
-msgstr "可抵銷 %(offset)s"
-
 msgid "Cancel"
 msgstr "取消"
 
 msgid "Cash Disbursement"
 msgstr "現金支出"
 
 msgid "Cash Disbursement Journal Entry#%(id)s"
@@ -265,29 +271,32 @@
 
 msgid "Fully offset"
 msgstr "全部抵銷"
 
 msgid "General"
 msgstr "一般"
 
-msgid "Go to unapplied original line items."
-msgstr "查閱未抵銷原始分錄。"
-
 msgid "Income"
 msgstr "收入"
 
 msgid "Income Statement"
 msgstr "損益表"
 
+msgid "Income Statement %(period)s"
+msgstr "%(period)s損益表"
+
 msgid "Income Statement of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s損益表"
 
 msgid "Income and Expenses Log"
 msgstr "收支帳"
 
+msgid "Income and Expenses Log of %(account)s %(period)s"
+msgstr "%(period)s%(account)s收支帳"
+
 msgid "Income and Expenses Log of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s收支帳"
 
 msgid "January"
 msgstr "一月"
 
 msgid "Journal"
@@ -316,14 +325,17 @@
 
 msgid "Last month, in its name."
 msgstr "上個月的名稱。"
 
 msgid "Ledger"
 msgstr "分類帳"
 
+msgid "Ledger of %(account)s %(period)s"
+msgstr "%(period)s%(account)s分類帳"
+
 msgid "Ledger of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s分類帳"
 
 msgid "Line Item Content"
 msgstr "分錄內容"
 
 msgid "Line items with offset cannot be deleted."
@@ -331,16 +343,16 @@
 
 msgid "March"
 msgstr "三月"
 
 msgid "Match"
 msgstr "抵銷"
 
-msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches)s 筆。"
+msgid "Matched %(matches)s offsets."
+msgstr "抵銷了 %(matches)s 筆。"
 
 msgid "May"
 msgstr "五月"
 
 msgid "Month"
 msgstr "月"
 
@@ -659,14 +671,17 @@
 
 msgid "The totals of the debit and credit amounts do not match."
 msgstr "借方貸方合計不符。 "
 
 msgid "There is no data."
 msgstr "沒有資料。"
 
+msgid "There is no unmatched offset."
+msgstr "沒有遺漏的抵銷分錄"
+
 msgid "This Month"
 msgstr "這個月"
 
 msgid "This Year"
 msgstr "今年"
 
 msgid "This account is not for credit line items."
@@ -701,17 +716,14 @@
 
 msgid "Today"
 msgstr "今天"
 
 msgid "Tomorrow"
 msgstr "明天"
 
-msgid "Toolbar"
-msgstr "工具列"
-
 msgid "Total"
 msgstr "合計"
 
 msgid "Transfer"
 msgstr "轉帳"
 
 msgid "Transfer Journal Entry#%(id)s"
@@ -719,31 +731,40 @@
 
 msgid "Travel"
 msgstr "差旅"
 
 msgid "Trial Balance"
 msgstr "試算表"
 
+msgid "Trial Balance %(period)s"
+msgstr "%(period)s試算表"
+
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s試算表"
 
-msgid "Unapplied Original Line Items"
-msgstr "未抵銷原始分錄"
+msgid "Unapplied Items"
+msgstr "未抵銷項目"
+
+msgid "Unapplied Items of %(account)s"
+msgstr "%(account)s未抵銷項目"
 
-msgid "Unapplied Original Line Items of %(account)s"
-msgstr "%(account)s未抵銷原始分錄"
+msgid "Unapplied Items of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s未抵銷項目"
 
 msgid "Unmatched"
 msgstr "未抵銷"
 
 msgid "Unmatched Offsets"
-msgstr "遺漏的抵銷分錄"
+msgstr "遺漏的抵銷項目"
+
+msgid "Unmatched Offsets of %(account)s"
+msgstr "%(account)s遺漏的抵銷項目"
 
-msgid "Unmatched Offsets in %(account)s"
-msgstr "%(account)s遺漏的抵銷分錄"
+msgid "Unmatched Offsets of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s遺漏的抵銷項目"
 
 msgid "Updated"
 msgstr "更新"
 
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水費{last_bimonthly_number}月"
```

### Comparing `mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.4.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # Copyright (C) 2023 imacat
 # This file is distributed under the same license as the Mia! Accounting
 # project.
 # imacat <imacat@mail.imacat.idv.tw>, 2023.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: mia-accounting 1.1.1\n"
+"Project-Id-Version: mia-accounting 1.4.0\n"
 "Report-Msgid-Bugs-To: imacat@mail.imacat.idv.tw\n"
-"POT-Creation-Date: 2023-04-09 01:41+0800\n"
-"PO-Revision-Date: 2023-04-09 01:41+0800\n"
+"POT-Creation-Date: 2023-04-18 09:32+0800\n"
+"PO-Revision-Date: 2023-04-18 09:32+0800\n"
 "Last-Translator: imacat <imacat@mail.imacat.idv.tw>\n"
 "Language: zh_Hant\n"
 "Language-Team: zh_Hant <imacat@mail.imacat.idv.tw>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 #: src/accounting/forms.py:33
-#: src/accounting/static/js/journal-entry-form.js:1065
+#: src/accounting/static/js/journal-entry-form.js:1080
 #: src/accounting/static/js/journal-entry-line-item-editor.js:411
 #: src/accounting/static/js/option-form.js:537
 #: src/accounting/static/js/option-form.js:803
 msgid "Please select the account."
 msgstr "請選擇科目。"
 
 #: src/accounting/forms.py:44
@@ -298,19 +298,19 @@
 
 #: src/accounting/journal_entry/forms/line_item.py:241
 #: src/accounting/static/js/journal-entry-line-item-editor.js:450
 #, python-format
 msgid "The amount must not be less than the offset total %(total)s."
 msgstr "金額不可低於抵銷總額 %(total)s 。"
 
-#: src/accounting/journal_entry/forms/line_item.py:413
+#: src/accounting/journal_entry/forms/line_item.py:426
 msgid "This account is not for debit line items."
 msgstr "科目不是借方科目。"
 
-#: src/accounting/journal_entry/forms/line_item.py:465
+#: src/accounting/journal_entry/forms/line_item.py:478
 msgid "This account is not for credit line items."
 msgstr "科目不是貸方科目。"
 
 #: src/accounting/option/forms.py:53
 msgid "This is not a current account."
 msgstr "這不是流動科目。"
 
@@ -350,14 +350,23 @@
 msgid "The settings were not modified."
 msgstr "設定未異動。"
 
 #: src/accounting/option/views.py:82
 msgid "The settings are saved successfully."
 msgstr "設定存好了。"
 
+#: src/accounting/report/views.py:401
+msgid "No more offset to match automatically."
+msgstr "無法自動配對抵銷。"
+
+#: src/accounting/report/views.py:408
+#, python-format
+msgid "Matched %(matches)s offsets."
+msgstr "抵銷了 %(matches)s 筆。"
+
 #: src/accounting/report/period/description.py:33
 msgid "for all time"
 msgstr "全部"
 
 #: src/accounting/report/period/description.py:67
 #, python-format
 msgid "since %(start)s"
@@ -419,71 +428,76 @@
 #: src/accounting/report/reports/ledger.py:380
 #: src/accounting/report/reports/trial_balance.py:229
 #: src/accounting/templates/accounting/journal-entry/disbursement/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html:38
 #: src/accounting/templates/accounting/journal-entry/receipt/detail.html:43
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:39
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:55
-#: src/accounting/templates/accounting/report/balance-sheet.html:59
-#: src/accounting/templates/accounting/report/balance-sheet.html:71
-#: src/accounting/templates/accounting/report/balance-sheet.html:81
+#: src/accounting/templates/accounting/report/balance-sheet.html:65
+#: src/accounting/templates/accounting/report/balance-sheet.html:77
 #: src/accounting/templates/accounting/report/balance-sheet.html:87
-#: src/accounting/templates/accounting/report/balance-sheet.html:96
-#: src/accounting/templates/accounting/report/balance-sheet.html:103
+#: src/accounting/templates/accounting/report/balance-sheet.html:93
+#: src/accounting/templates/accounting/report/balance-sheet.html:102
+#: src/accounting/templates/accounting/report/balance-sheet.html:109
 #: src/accounting/templates/accounting/report/income-expenses.html:81
-#: src/accounting/templates/accounting/report/income-statement.html:83
+#: src/accounting/templates/accounting/report/income-statement.html:89
 #: src/accounting/templates/accounting/report/ledger.html:82
-#: src/accounting/templates/accounting/report/trial-balance.html:74
+#: src/accounting/templates/accounting/report/trial-balance.html:80
 msgid "Total"
 msgstr "合計"
 
 #: src/accounting/report/reports/income_expenses.py:136
 #: src/accounting/report/reports/ledger.py:132
 msgid "Brought forward"
 msgstr "前期轉入"
 
 #: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:158
 #: src/accounting/report/reports/ledger.py:366
-#: src/accounting/report/reports/unapplied.py:137
+#: src/accounting/report/reports/unapplied.py:148
+#: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form.html:50
 #: src/accounting/templates/accounting/report/include/period-chooser.html:111
 #: src/accounting/templates/accounting/report/income-expenses.html:55
 #: src/accounting/templates/accounting/report/journal.html:53
 #: src/accounting/templates/accounting/report/ledger.html:55
 #: src/accounting/templates/accounting/report/search.html:50
-#: src/accounting/templates/accounting/report/unapplied.html:50
+#: src/accounting/templates/accounting/report/unapplied.html:52
+#: src/accounting/templates/accounting/report/unmatched.html:93
 msgid "Date"
 msgstr "日期"
 
 #: src/accounting/report/reports/income_expenses.py:407
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/trial_balance.py:225
-#: src/accounting/report/reports/unapplied_accounts.py:109
+#: src/accounting/report/reports/unapplied_accounts.py:122
+#: src/accounting/report/reports/unmatched_accounts.py:122
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:57
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:39
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:90
 #: src/accounting/templates/accounting/report/income-expenses.html:56
 #: src/accounting/templates/accounting/report/journal.html:55
 #: src/accounting/templates/accounting/report/search.html:52
-#: src/accounting/templates/accounting/report/trial-balance.html:55
+#: src/accounting/templates/accounting/report/trial-balance.html:61
 msgid "Account"
 msgstr "科目"
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/report/reports/journal.py:159
 #: src/accounting/report/reports/ledger.py:366
-#: src/accounting/report/reports/unapplied.py:138
+#: src/accounting/report/reports/unapplied.py:149
+#: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:49
 #: src/accounting/templates/accounting/report/income-expenses.html:57
 #: src/accounting/templates/accounting/report/journal.html:56
 #: src/accounting/templates/accounting/report/ledger.html:56
 #: src/accounting/templates/accounting/report/search.html:53
-#: src/accounting/templates/accounting/report/unapplied.html:52
+#: src/accounting/templates/accounting/report/unapplied.html:53
+#: src/accounting/templates/accounting/report/unmatched.html:94
 msgid "Description"
 msgstr "摘要"
 
 #: src/accounting/report/reports/income_expenses.py:408
 #: src/accounting/templates/accounting/report/income-expenses.html:58
 msgid "Income"
 msgstr "收入"
@@ -491,16 +505,18 @@
 #: src/accounting/report/reports/income_expenses.py:409
 #: src/accounting/templates/accounting/report/income-expenses.html:59
 msgid "Expense"
 msgstr "支出"
 
 #: src/accounting/report/reports/income_expenses.py:409
 #: src/accounting/report/reports/ledger.py:368
+#: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/report/income-expenses.html:60
 #: src/accounting/templates/accounting/report/ledger.html:60
+#: src/accounting/templates/accounting/report/unmatched.html:97
 msgid "Balance"
 msgstr "餘額"
 
 #: src/accounting/report/reports/income_expenses.py:410
 #: src/accounting/report/reports/journal.py:161
 #: src/accounting/report/reports/ledger.py:368
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:178
@@ -529,72 +545,96 @@
 msgstr "稅後淨利"
 
 #: src/accounting/report/reports/income_statement.py:233
 msgid "net income or loss for current period"
 msgstr "本期損益"
 
 #: src/accounting/report/reports/income_statement.py:301
-#: src/accounting/report/reports/unapplied.py:138
+#: src/accounting/report/reports/unapplied.py:149
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:65
-#: src/accounting/templates/accounting/report/income-statement.html:55
-#: src/accounting/templates/accounting/report/unapplied.html:53
+#: src/accounting/templates/accounting/report/income-statement.html:61
+#: src/accounting/templates/accounting/report/unapplied.html:54
 msgid "Amount"
 msgstr "金額"
 
 #: src/accounting/report/reports/journal.py:158
-#: src/accounting/report/reports/unapplied.py:137
+#: src/accounting/report/reports/unapplied.py:148
+#: src/accounting/report/reports/unmatched.py:158
 #: src/accounting/templates/accounting/journal-entry/include/form-currency.html:33
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:73
 #: src/accounting/templates/accounting/report/journal.html:54
 #: src/accounting/templates/accounting/report/search.html:51
-#: src/accounting/templates/accounting/report/unapplied.html:51
 msgid "Currency"
 msgstr "貨幣"
 
 #: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:225
+#: src/accounting/report/reports/unmatched.py:159
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:33
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:30
 #: src/accounting/templates/accounting/report/journal.html:57
 #: src/accounting/templates/accounting/report/ledger.html:57
 #: src/accounting/templates/accounting/report/search.html:54
-#: src/accounting/templates/accounting/report/trial-balance.html:56
+#: src/accounting/templates/accounting/report/trial-balance.html:62
+#: src/accounting/templates/accounting/report/unmatched.html:95
 msgid "Debit"
 msgstr "借方"
 
 #: src/accounting/report/reports/journal.py:160
 #: src/accounting/report/reports/ledger.py:367
 #: src/accounting/report/reports/trial_balance.py:226
+#: src/accounting/report/reports/unmatched.py:160
 #: src/accounting/templates/accounting/journal-entry/transfer/detail.html:49
 #: src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html:41
 #: src/accounting/templates/accounting/report/journal.html:58
 #: src/accounting/templates/accounting/report/ledger.html:58
 #: src/accounting/templates/accounting/report/search.html:55
-#: src/accounting/templates/accounting/report/trial-balance.html:57
+#: src/accounting/templates/accounting/report/trial-balance.html:63
+#: src/accounting/templates/accounting/report/unmatched.html:96
 msgid "Credit"
 msgstr "貸方"
 
-#: src/accounting/report/reports/unapplied.py:121
-#: src/accounting/report/reports/unapplied_accounts.py:93
+#: src/accounting/report/reports/unapplied.py:132
+#: src/accounting/report/reports/unapplied_accounts.py:107
+#: src/accounting/report/reports/unmatched.py:142
+#: src/accounting/report/reports/unmatched_accounts.py:107
 #: src/accounting/templates/accounting/include/nav.html:39
 msgid "Accounts"
 msgstr "科目"
 
-#: src/accounting/report/reports/unapplied.py:139
-#: src/accounting/templates/accounting/report/unapplied.html:54
+#: src/accounting/report/reports/unapplied.py:150
+#: src/accounting/templates/accounting/report/unapplied.html:55
 msgid "Net Balance"
 msgstr "淨額"
 
-#: src/accounting/report/reports/unapplied_accounts.py:109
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:47
+#: src/accounting/report/reports/unapplied_accounts.py:122
+#: src/accounting/report/reports/unmatched_accounts.py:122
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:59
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:59
 msgid "Count"
 msgstr "數量"
 
-#: src/accounting/report/utils/report_chooser.py:82
+#: src/accounting/report/utils/offset_matcher.py:163
+msgid "There is no unmatched offset."
+msgstr "沒有遺漏的抵銷分錄"
+
+#: src/accounting/report/utils/offset_matcher.py:167
+#, python-format
+msgid "%(total)s unmatched offsets without original items."
+msgstr "%(total)s 筆遺漏的抵銷分錄無法自動抵銷。"
+
+#: src/accounting/report/utils/offset_matcher.py:172
+#, python-format
+msgid ""
+"%(matches)s unmatched offsets out of %(total)s can match with their "
+"original items."
+msgstr "%(total)s 筆遺漏的抵銷分錄中，可配對抵銷掉 %(matches)s 筆。"
+
+#: src/accounting/report/utils/report_chooser.py:86
 #: src/accounting/templates/accounting/account/include/form.html:98
 #: src/accounting/templates/accounting/account/list.html:40
 #: src/accounting/templates/accounting/base-account/list.html:34
 #: src/accounting/templates/accounting/currency/list.html:40
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:34
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:34
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:34
@@ -602,122 +642,127 @@
 #: src/accounting/templates/accounting/report/include/search-modal.html:33
 #: src/accounting/templates/accounting/report/include/search-modal.html:38
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:64
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:126
 msgid "Search"
 msgstr "搜尋"
 
-#: src/accounting/report/utils/report_chooser.py:93
+#: src/accounting/report/utils/report_chooser.py:97
 msgid "Income and Expenses Log"
 msgstr "收支帳"
 
-#: src/accounting/report/utils/report_chooser.py:106
+#: src/accounting/report/utils/report_chooser.py:110
 msgid "Ledger"
 msgstr "分類帳"
 
-#: src/accounting/report/utils/report_chooser.py:118
+#: src/accounting/report/utils/report_chooser.py:122
 msgid "Journal"
 msgstr "日記簿"
 
-#: src/accounting/report/utils/report_chooser.py:128
+#: src/accounting/report/utils/report_chooser.py:132
 msgid "Trial Balance"
 msgstr "試算表"
 
-#: src/accounting/report/utils/report_chooser.py:139
+#: src/accounting/report/utils/report_chooser.py:143
 msgid "Income Statement"
 msgstr "損益表"
 
-#: src/accounting/report/utils/report_chooser.py:150
+#: src/accounting/report/utils/report_chooser.py:154
 msgid "Balance Sheet"
 msgstr "資產負債表"
 
-#: src/accounting/report/utils/report_chooser.py:163
 #: src/accounting/report/utils/report_chooser.py:167
-msgid "Unapplied Original Line Items"
-msgstr "未抵銷原始分錄"
+#: src/accounting/report/utils/report_chooser.py:171
+msgid "Unapplied Items"
+msgstr "未抵銷項目"
+
+#: src/accounting/report/utils/report_chooser.py:184
+#: src/accounting/report/utils/report_chooser.py:188
+msgid "Unmatched Offsets"
+msgstr "遺漏的抵銷項目"
 
 #: src/accounting/static/js/account-form.js:206
 msgid "Please fill in the title."
 msgstr "請填上標題。"
 
-#: src/accounting/static/js/description-editor.js:951
-#: src/accounting/static/js/description-editor.js:1129
+#: src/accounting/static/js/description-editor.js:952
+#: src/accounting/static/js/description-editor.js:1130
 msgid "Please fill in the tag."
 msgstr "請填上標籤。"
 
-#: src/accounting/static/js/description-editor.js:961
-#: src/accounting/static/js/description-editor.js:1149
+#: src/accounting/static/js/description-editor.js:962
+#: src/accounting/static/js/description-editor.js:1150
 msgid "Please fill in the origin."
 msgstr "請填上起點。"
 
-#: src/accounting/static/js/description-editor.js:971
-#: src/accounting/static/js/description-editor.js:1159
+#: src/accounting/static/js/description-editor.js:972
+#: src/accounting/static/js/description-editor.js:1160
 msgid "Please fill in the destination."
 msgstr "請填上終點。"
 
-#: src/accounting/static/js/description-editor.js:1139
+#: src/accounting/static/js/description-editor.js:1140
 msgid "Please fill in the route."
 msgstr "請填上路線名稱。"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "January"
 msgstr "一月"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "February"
 msgstr "二月"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "March"
 msgstr "三月"
 
-#: src/accounting/static/js/description-editor.js:1192
+#: src/accounting/static/js/description-editor.js:1193
 msgid "April"
 msgstr "四月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "May"
 msgstr "五月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "June"
 msgstr "六月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "July"
 msgstr "七月"
 
-#: src/accounting/static/js/description-editor.js:1193
+#: src/accounting/static/js/description-editor.js:1194
 msgid "August"
 msgstr "八月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "September"
 msgstr "九月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "October"
 msgstr "十月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "November"
 msgstr "十一月"
 
-#: src/accounting/static/js/description-editor.js:1194
+#: src/accounting/static/js/description-editor.js:1195
 msgid "December"
 msgstr "十二月"
 
-#: src/accounting/static/js/journal-entry-form.js:1070
+#: src/accounting/static/js/journal-entry-form.js:1085
 #: src/accounting/static/js/journal-entry-line-item-editor.js:430
 msgid "Please fill in the amount."
 msgstr "請填上金額。"
 
-#: src/accounting/static/js/journal-entry-form.js:1092
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:34
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:38
+#: src/accounting/static/js/journal-entry-form.js:1107
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:37
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:41
 #, python-format
 msgid "Offset %(item)s"
 msgstr "抵銷 %(item)s"
 
 #: src/accounting/static/js/period-chooser.js:270
 msgid "The date is too early."
 msgstr "日期太早。"
@@ -752,15 +797,14 @@
 #: src/accounting/templates/accounting/base-account/detail.html:31
 #: src/accounting/templates/accounting/currency/detail.html:31
 #: src/accounting/templates/accounting/currency/include/form.html:33
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:31
 #: src/accounting/templates/accounting/journal-entry/include/form.html:38
 #: src/accounting/templates/accounting/journal-entry/order.html:36
 #: src/accounting/templates/accounting/option/form.html:36
-#: src/accounting/templates/accounting/unmatched-offset/list.html:31
 msgid "Back"
 msgstr "回上頁"
 
 #: src/accounting/templates/accounting/account/detail.html:36
 #: src/accounting/templates/accounting/currency/detail.html:36
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:36
 #: src/accounting/templates/accounting/option/detail.html:31
@@ -793,15 +837,15 @@
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:78
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:28
 #: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:27
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:28
 #: src/accounting/templates/accounting/report/include/period-chooser.html:27
 #: src/accounting/templates/accounting/report/include/search-modal.html:28
-#: src/accounting/templates/accounting/unmatched-offset/list.html:54
+#: src/accounting/templates/accounting/report/unmatched.html:58
 msgid "Close"
 msgstr "關閉"
 
 #: src/accounting/templates/accounting/account/detail.html:80
 msgid "Do you really want to delete this account?"
 msgstr "你確定要刪掉這個科目嗎？"
 
@@ -811,23 +855,23 @@
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:49
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:194
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:84
 #: src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html:70
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:48
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:65
 #: src/accounting/templates/accounting/report/include/search-modal.html:37
-#: src/accounting/templates/accounting/unmatched-offset/list.html:70
+#: src/accounting/templates/accounting/report/unmatched.html:74
 msgid "Cancel"
 msgstr "取消"
 
 #: src/accounting/templates/accounting/account/detail.html:84
 #: src/accounting/templates/accounting/currency/detail.html:80
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:85
 #: src/accounting/templates/accounting/report/include/period-chooser.html:141
-#: src/accounting/templates/accounting/unmatched-offset/list.html:71
+#: src/accounting/templates/accounting/report/unmatched.html:75
 msgid "Confirm"
 msgstr "確定"
 
 #: src/accounting/templates/accounting/account/detail.html:101
 #: src/accounting/templates/accounting/currency/detail.html:92
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:114
 msgid "Created"
@@ -867,30 +911,30 @@
 
 #: src/accounting/templates/accounting/account/include/form.html:109
 #: src/accounting/templates/accounting/account/list.html:68
 #: src/accounting/templates/accounting/account/order.html:81
 #: src/accounting/templates/accounting/base-account/list.html:51
 #: src/accounting/templates/accounting/currency/list.html:65
 #: src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html:46
-#: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:51
+#: src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html:58
 #: src/accounting/templates/accounting/journal-entry/order.html:82
 #: src/accounting/templates/accounting/option/detail.html:67
 #: src/accounting/templates/accounting/option/detail.html:83
 #: src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html:45
-#: src/accounting/templates/accounting/report/balance-sheet.html:110
+#: src/accounting/templates/accounting/report/balance-sheet.html:116
 #: src/accounting/templates/accounting/report/income-expenses.html:113
-#: src/accounting/templates/accounting/report/income-statement.html:96
+#: src/accounting/templates/accounting/report/income-statement.html:102
 #: src/accounting/templates/accounting/report/journal.html:103
 #: src/accounting/templates/accounting/report/ledger.html:116
 #: src/accounting/templates/accounting/report/search.html:100
-#: src/accounting/templates/accounting/report/trial-balance.html:82
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:61
-#: src/accounting/templates/accounting/report/unapplied.html:98
-#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:37
-#: src/accounting/templates/accounting/unmatched-offset/list.html:104
+#: src/accounting/templates/accounting/report/trial-balance.html:88
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:76
+#: src/accounting/templates/accounting/report/unapplied.html:90
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:76
+#: src/accounting/templates/accounting/report/unmatched.html:147
 msgid "There is no data."
 msgstr "沒有資料。"
 
 #: src/accounting/templates/accounting/account/order.html:29
 #, python-format
 msgid "The Accounts of %(base)s"
 msgstr "%(base)s下的科目"
@@ -980,20 +1024,15 @@
 msgid "Base Accounts"
 msgstr "基本科目"
 
 #: src/accounting/templates/accounting/include/nav.html:51
 msgid "Currencies"
 msgstr "貨幣"
 
-#: src/accounting/templates/accounting/include/nav.html:57
-#: src/accounting/templates/accounting/unmatched-offset/dashboard.html:24
-msgid "Unmatched Offsets"
-msgstr "遺漏的抵銷分錄"
-
-#: src/accounting/templates/accounting/include/nav.html:64
+#: src/accounting/templates/accounting/include/nav.html:58
 #: src/accounting/templates/accounting/option/detail.html:24
 #: src/accounting/templates/accounting/option/detail.html:41
 #: src/accounting/templates/accounting/option/form.html:29
 msgid "Settings"
 msgstr "設定"
 
 #: src/accounting/templates/accounting/include/pagination.html:23
@@ -1084,31 +1123,31 @@
 msgid "Route"
 msgstr "路線"
 
 #: src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html:172
 msgid "The Number of Items"
 msgstr "數量"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:42
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:43
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:45
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:46
 msgid "Offsets"
 msgstr "抵銷"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:55
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:54
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:58
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:57
 msgid "Net balance"
 msgstr "淨額"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:60
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:51
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:63
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:54
 msgid "Fully offset"
 msgstr "全部抵銷"
 
-#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:65
-#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:59
+#: src/accounting/templates/accounting/journal-entry/include/detail-line-items.html:68
+#: src/accounting/templates/accounting/journal-entry/include/form-line-item.html:62
 msgid "Unmatched"
 msgstr "未抵銷"
 
 #: src/accounting/templates/accounting/journal-entry/include/detail.html:77
 msgid "Confirm Delete Journal Entry"
 msgstr "確認刪除傳票"
 
@@ -1213,60 +1252,135 @@
 msgstr "範例："
 
 #: src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html:61
 msgid "Water bill for {last_bimonthly_name}"
 msgstr "水費{last_bimonthly_number}月"
 
 #: src/accounting/templates/accounting/report/balance-sheet.html:29
-#: src/accounting/templates/accounting/report/balance-sheet.html:49
+#: src/accounting/templates/accounting/report/balance-sheet.html:51
+#, python-format
+msgid "Balance Sheet %(period)s"
+msgstr "%(period)s資產負債表"
+
+#: src/accounting/templates/accounting/report/balance-sheet.html:29
+#: src/accounting/templates/accounting/report/balance-sheet.html:53
 #, python-format
 msgid "Balance Sheet of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s資產負債表"
 
 #: src/accounting/templates/accounting/report/income-expenses.html:29
 #, python-format
+msgid "Income and Expenses Log of %(account)s %(period)s"
+msgstr "%(period)s%(account)s收支帳"
+
+#: src/accounting/templates/accounting/report/income-expenses.html:29
+#, python-format
 msgid "Income and Expenses Log of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s收支帳"
 
 #: src/accounting/templates/accounting/report/income-statement.html:29
-#: src/accounting/templates/accounting/report/income-statement.html:49
+#: src/accounting/templates/accounting/report/income-statement.html:51
+#, python-format
+msgid "Income Statement %(period)s"
+msgstr "%(period)s損益表"
+
+#: src/accounting/templates/accounting/report/income-statement.html:29
+#: src/accounting/templates/accounting/report/income-statement.html:53
 #, python-format
 msgid "Income Statement of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s損益表"
 
 #: src/accounting/templates/accounting/report/journal.html:29
 #, python-format
 msgid "Journal %(period)s"
 msgstr "%(period)s日記簿"
 
 #: src/accounting/templates/accounting/report/ledger.html:29
 #, python-format
+msgid "Ledger of %(account)s %(period)s"
+msgstr "%(period)s%(account)s分類帳"
+
+#: src/accounting/templates/accounting/report/ledger.html:29
+#, python-format
 msgid "Ledger of %(account)s in %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s%(account)s分類帳"
 
 #: src/accounting/templates/accounting/report/trial-balance.html:29
-#: src/accounting/templates/accounting/report/trial-balance.html:49
+#: src/accounting/templates/accounting/report/trial-balance.html:51
+#, python-format
+msgid "Trial Balance %(period)s"
+msgstr "%(period)s試算表"
+
+#: src/accounting/templates/accounting/report/trial-balance.html:29
+#: src/accounting/templates/accounting/report/trial-balance.html:53
 #, python-format
 msgid "Trial Balance of %(currency)s %(period)s"
 msgstr "%(period)s%(currency)s試算表"
 
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:24
-#: src/accounting/templates/accounting/report/unapplied-accounts.html:41
-msgid "Accounts with Unapplied Original Line Items"
-msgstr "有未抵銷原始分錄的科目"
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:29
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:49
+msgid "Accounts with Unapplied Items"
+msgstr "含未抵銷項目的科目"
+
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:29
+#: src/accounting/templates/accounting/report/unapplied-accounts.html:51
+#, python-format
+msgid "Accounts with Unapplied Items in %(currency)s"
+msgstr "%(currency)s含未抵銷項目的科目"
+
+#: src/accounting/templates/accounting/report/unapplied.html:29
+#, python-format
+msgid "Unapplied Items of %(account)s"
+msgstr "%(account)s未抵銷項目"
+
+#: src/accounting/templates/accounting/report/unapplied.html:29
+#, python-format
+msgid "Unapplied Items of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s未抵銷項目"
+
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:29
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:49
+msgid "Accounts with Unmatched Offsets"
+msgstr "含遺漏抵銷項目的科目"
+
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:29
+#: src/accounting/templates/accounting/report/unmatched-accounts.html:51
+#, python-format
+msgid "Accounts with Unmatched Offsets in %(currency)s"
+msgstr "%(currency)s含遺漏抵銷項目的科目"
+
+#: src/accounting/templates/accounting/report/unmatched.html:29
+#, python-format
+msgid "Unmatched Offsets of %(account)s"
+msgstr "%(account)s遺漏的抵銷項目"
 
-#: src/accounting/templates/accounting/report/unapplied.html:28
+#: src/accounting/templates/accounting/report/unmatched.html:29
 #, python-format
-msgid "Unapplied Original Line Items of %(account)s"
-msgstr "%(account)s未抵銷原始分錄"
+msgid "Unmatched Offsets of %(account)s in %(currency)s"
+msgstr "%(currency)s%(account)s遺漏的抵銷項目"
+
+#: src/accounting/templates/accounting/report/unmatched.html:47
+msgid "Match"
+msgstr "抵銷"
+
+#: src/accounting/templates/accounting/report/unmatched.html:57
+msgid "Confirm Match Offsets"
+msgstr "確認抵銷"
+
+#: src/accounting/templates/accounting/report/unmatched.html:61
+msgid ""
+"Do you really want to match the following original line items with their "
+"offsets?  This cannot be undone.  Please backup your database first, and "
+"review before you confirm."
+msgstr "你確定要抵銷下列原始分錄與抵銷分錄嗎？結果無法復原。請先備份資料庫，並仔細核對抵銷分錄是否正確。"
 
-#: src/accounting/templates/accounting/report/unapplied.html:65
+#: src/accounting/templates/accounting/report/unmatched.html:107
 #, python-format
-msgid "Can match %(offset)s"
-msgstr "可抵銷 %(offset)s"
+msgid "Can match %(item)s"
+msgstr "可抵銷 %(item)s"
 
 #: src/accounting/templates/accounting/report/include/period-chooser.html:26
 msgid "Period Chooser"
 msgstr "選擇日期範圍"
 
 #: src/accounting/templates/accounting/report/include/period-chooser.html:34
 msgid "Month"
@@ -1293,73 +1407,14 @@
 msgstr "期間"
 
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:112
 #: src/accounting/templates/accounting/report/include/toolbar-buttons.html:117
 msgid "Download"
 msgstr "下載"
 
-#: src/accounting/templates/accounting/unmatched-offset/list.html:24
-#, python-format
-msgid "Unmatched Offsets in %(account)s"
-msgstr "%(account)s遺漏的抵銷分錄"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:28
-msgid "Toolbar"
-msgstr "工具列"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:36
-#: src/accounting/templates/accounting/unmatched-offset/list.html:41
-msgid "Match"
-msgstr "抵銷"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:53
-msgid "Confirm Match Offsets"
-msgstr "確認抵銷"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:57
-msgid ""
-"Do you really want to match the following original line items with their "
-"offsets?  This cannot be undone.  Please backup your database first, and "
-"review before you confirm."
-msgstr "你確定要抵銷下列原始分錄與抵銷分錄嗎？結果無法復原。請先備份資料庫，並仔細核對抵銷分錄是否正確。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:81
-#, python-format
-msgid ""
-"%(matches)s unapplied original line items out of %(total)s can match with"
-" their offsets."
-msgstr "%(total)s 筆未抵銷原始分錄中，可配對抵銷掉 %(matches)s 筆。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:83
-#, python-format
-msgid "%(total)s unapplied original line items without matching offsets."
-msgstr "%(total)s 筆未抵銷原始分錄，無法自動配對抵銷。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:85
-msgid "Go to unapplied original line items."
-msgstr "查閱未抵銷原始分錄。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:87
-msgid "All original line items are fully offset."
-msgstr "原始分錄已全部抵銷。"
-
-#: src/accounting/templates/accounting/unmatched-offset/list.html:98
-#, python-format
-msgid "Can match %(item)s"
-msgstr "可抵銷 %(item)s"
-
-#: src/accounting/unmatched_offset/views.py:71
-msgid "No more offset to match automatically."
-msgstr "無法自動配對抵銷。"
-
-#: src/accounting/unmatched_offset/views.py:77
-#, python-format
-msgid "Matches %(matches)s from %(total)s unapplied line items."
-msgstr "%(total)s 筆未抵銷原始分錄中，配對抵銷掉 %(matches)s 筆。"
-
 #: src/accounting/utils/current_account.py:65
 msgid "current assets and liabilities"
 msgstr "流動資產與負債"
 
 #: src/accounting/utils/pagination.py:206
 msgctxt "Pagination|"
 msgid "Previous"
```

### Comparing `mia-accounting-1.3.3/src/accounting/unmatched_offset/__init__.py` & `mia-accounting-1.4.0/src/accounting/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 # The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/8
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/1/25
 
 #  Copyright (c) 2023 imacat.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The unmatched offset management.
-
-"""
-from flask import Blueprint
+"""The independent utilities.
 
+This module should not import any other module from the application.
 
-def init_app(bp: Blueprint) -> None:
-    """Initialize the application.
-
-    :param bp: The blueprint of the accounting application.
-    :return: None.
-    """
-    from .views import bp as unmatched_offset_bp
-    bp.register_blueprint(unmatched_offset_bp, url_prefix="/unmatched-offsets")
+"""
```

### Comparing `mia-accounting-1.3.3/src/accounting/utils/cast.py` & `mia-accounting-1.4.0/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/current_account.py` & `mia-accounting-1.4.0/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/flash_errors.py` & `mia-accounting-1.4.0/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.4.0/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/next_uri.py` & `mia-accounting-1.4.0/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/offset_alias.py` & `mia-accounting-1.4.0/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/options.py` & `mia-accounting-1.4.0/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/pagination.py` & `mia-accounting-1.4.0/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/permission.py` & `mia-accounting-1.4.0/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/query.py` & `mia-accounting-1.4.0/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/random_id.py` & `mia-accounting-1.4.0/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/strip_text.py` & `mia-accounting-1.4.0/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/accounting/utils/unapplied.py` & `mia-accounting-1.4.0/src/accounting/report/utils/unapplied.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/8
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/7
 
 #  Copyright (c) 2023 imacat.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
@@ -16,57 +16,90 @@
 #  limitations under the License.
 """The unapplied original line item utilities.
 
 """
 from decimal import Decimal
 
 import sqlalchemy as sa
-from sqlalchemy.orm import selectinload
 
 from accounting import db
-from accounting.models import Account, JournalEntry, JournalEntryLineItem
+from accounting.models import Currency, Account, JournalEntry, \
+    JournalEntryLineItem
 from accounting.utils.cast import be
 from accounting.utils.offset_alias import offset_alias
 
 
-def get_unapplied_original_line_items(account: Account) \
-        -> list[JournalEntryLineItem]:
-    """Queries and returns the unapplied original line items in an account.
+def get_accounts_with_unapplied(currency: Currency) -> list[Account]:
+    """Returns the accounts with unapplied original line items.
 
+    :param currency: The currency.
+    :return: The accounts with unapplied original line items.
+    """
+    offset: sa.Alias = offset_alias()
+    net_balance: sa.Label \
+        = (JournalEntryLineItem.amount
+           + sa.func.sum(sa.case(
+                (be(offset.c.is_debit == JournalEntryLineItem.is_debit),
+                 offset.c.amount),
+                else_=-offset.c.amount))).label("net_balance")
+    select_unapplied: sa.Select \
+        = sa.select(JournalEntryLineItem.id)\
+        .join(JournalEntry).join(Account)\
+        .join(offset, be(JournalEntryLineItem.id
+                         == offset.c.original_line_item_id),
+              isouter=True)\
+        .filter(Account.is_need_offset,
+                be(JournalEntryLineItem.currency_code == currency.code),
+                sa.or_(sa.and_(Account.base_code.startswith("2"),
+                               sa.not_(JournalEntryLineItem.is_debit)),
+                       sa.and_(Account.base_code.startswith("1"),
+                               JournalEntryLineItem.is_debit)))\
+        .group_by(JournalEntryLineItem.id)\
+        .having(sa.or_(sa.func.count(offset.c.id) == 0, net_balance != 0))
+
+    count_func: sa.Label \
+        = sa.func.count(JournalEntryLineItem.id).label("count")
+    select: sa.Select = sa.select(Account.id, count_func)\
+        .join(JournalEntryLineItem, isouter=True)\
+        .filter(JournalEntryLineItem.id.in_(select_unapplied))\
+        .group_by(Account.id)\
+        .having(count_func > 0)
+    counts: dict[int, int] \
+        = {x.id: x.count for x in db.session.execute(select)}
+    accounts: list[Account] = Account.query.filter(Account.id.in_(counts))\
+        .order_by(Account.base_code, Account.no).all()
+    for account in accounts:
+        account.count = counts[account.id]
+    return accounts
+
+
+def get_net_balances(currency: Currency, account: Account) \
+        -> dict[int, Decimal | None]:
+    """Returns the net balances of the unapplied line items of the account.
+
+    :param currency: The currency.
     :param account: The account.
-    :return: The unapplied original line items in the account.
+    :return: The net balances of the unapplied line items of the account.
     """
     offset: sa.Alias = offset_alias()
     net_balance: sa.Label \
         = (JournalEntryLineItem.amount
            + sa.func.sum(sa.case(
                 (be(offset.c.is_debit == JournalEntryLineItem.is_debit),
                  offset.c.amount),
                 else_=-offset.c.amount))).label("net_balance")
     select_net_balances: sa.Select \
         = sa.select(JournalEntryLineItem.id, net_balance) \
-        .join(Account) \
+        .join(JournalEntry).join(Account) \
         .join(offset, be(JournalEntryLineItem.id
                          == offset.c.original_line_item_id),
               isouter=True) \
         .filter(be(Account.id == account.id),
+                be(JournalEntryLineItem.currency_code == currency.code),
                 sa.or_(sa.and_(Account.base_code.startswith("2"),
                                sa.not_(JournalEntryLineItem.is_debit)),
                        sa.and_(Account.base_code.startswith("1"),
                                JournalEntryLineItem.is_debit))) \
         .group_by(JournalEntryLineItem.id) \
         .having(sa.or_(sa.func.count(offset.c.id) == 0, net_balance != 0))
-    net_balances: dict[int, Decimal] \
-        = {x.id: x.net_balance
-           for x in db.session.execute(select_net_balances).all()}
-    line_items: list[JournalEntryLineItem] = JournalEntryLineItem.query \
-        .filter(JournalEntryLineItem.id.in_({x for x in net_balances})) \
-        .join(JournalEntry) \
-        .order_by(JournalEntry.date, JournalEntry.no,
-                  JournalEntryLineItem.is_debit, JournalEntryLineItem.no) \
-        .options(selectinload(JournalEntryLineItem.currency),
-                 selectinload(JournalEntryLineItem.journal_entry)).all()
-    for line_item in line_items:
-        line_item.net_balance = line_item.amount \
-            if net_balances[line_item.id] is None \
-            else net_balances[line_item.id]
-    return line_items
+    return {x.id: x.net_balance
+            for x in db.session.execute(select_net_balances).all()}
```

### Comparing `mia-accounting-1.3.3/src/accounting/utils/user.py` & `mia-accounting-1.4.0/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.4.0/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.3
+Version: 1.4.0
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.3.3/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.4.0/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 docs/source/accounting.journal_entry.utils.rst
 docs/source/accounting.option.rst
 docs/source/accounting.report.period.rst
 docs/source/accounting.report.reports.rst
 docs/source/accounting.report.rst
 docs/source/accounting.report.utils.rst
 docs/source/accounting.rst
-docs/source/accounting.unmatched_offset.rst
 docs/source/accounting.utils.rst
 docs/source/conf.py
 docs/source/examples.rst
 docs/source/history.rst
 docs/source/index.rst
 docs/source/intro.rst
 docs/source/modules.rst
@@ -87,22 +86,26 @@
 src/accounting/report/reports/income_statement.py
 src/accounting/report/reports/journal.py
 src/accounting/report/reports/ledger.py
 src/accounting/report/reports/search.py
 src/accounting/report/reports/trial_balance.py
 src/accounting/report/reports/unapplied.py
 src/accounting/report/reports/unapplied_accounts.py
+src/accounting/report/reports/unmatched.py
+src/accounting/report/reports/unmatched_accounts.py
 src/accounting/report/utils/__init__.py
 src/accounting/report/utils/base_page_params.py
 src/accounting/report/utils/base_report.py
 src/accounting/report/utils/csv_export.py
+src/accounting/report/utils/offset_matcher.py
 src/accounting/report/utils/option_link.py
 src/accounting/report/utils/report_chooser.py
 src/accounting/report/utils/report_type.py
 src/accounting/report/utils/unapplied.py
+src/accounting/report/utils/unmatched.py
 src/accounting/report/utils/urls.py
 src/accounting/static/css/style.css
 src/accounting/static/js/account-form.js
 src/accounting/static/js/account-order.js
 src/accounting/static/js/currency-form.js
 src/accounting/static/js/description-editor.js
 src/accounting/static/js/drag-and-drop-reorder.js
@@ -168,49 +171,44 @@
 src/accounting/templates/accounting/report/income-statement.html
 src/accounting/templates/accounting/report/journal.html
 src/accounting/templates/accounting/report/ledger.html
 src/accounting/templates/accounting/report/search.html
 src/accounting/templates/accounting/report/trial-balance.html
 src/accounting/templates/accounting/report/unapplied-accounts.html
 src/accounting/templates/accounting/report/unapplied.html
+src/accounting/templates/accounting/report/unmatched-accounts.html
+src/accounting/templates/accounting/report/unmatched.html
 src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
 src/accounting/templates/accounting/report/include/balance-sheet-section.html
 src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
 src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
 src/accounting/templates/accounting/report/include/ledger-row-desktop.html
 src/accounting/templates/accounting/report/include/ledger-row-mobile.html
 src/accounting/templates/accounting/report/include/period-chooser.html
 src/accounting/templates/accounting/report/include/search-modal.html
 src/accounting/templates/accounting/report/include/toolbar-buttons.html
-src/accounting/templates/accounting/unmatched-offset/dashboard.html
-src/accounting/templates/accounting/unmatched-offset/list.html
 src/accounting/translations/accounting.pot
 src/accounting/translations/babel.cfg
 src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
 src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
 src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
 src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-src/accounting/unmatched_offset/__init__.py
-src/accounting/unmatched_offset/queries.py
-src/accounting/unmatched_offset/views.py
 src/accounting/utils/__init__.py
 src/accounting/utils/cast.py
 src/accounting/utils/current_account.py
 src/accounting/utils/flash_errors.py
 src/accounting/utils/journal_entry_types.py
 src/accounting/utils/next_uri.py
 src/accounting/utils/offset_alias.py
-src/accounting/utils/offset_matcher.py
 src/accounting/utils/options.py
 src/accounting/utils/pagination.py
 src/accounting/utils/permission.py
 src/accounting/utils/query.py
 src/accounting/utils/random_id.py
 src/accounting/utils/strip_text.py
-src/accounting/utils/unapplied.py
 src/accounting/utils/user.py
 src/mia_accounting.egg-info/PKG-INFO
 src/mia_accounting.egg-info/SOURCES.txt
 src/mia_accounting.egg-info/dependency_links.txt
 src/mia_accounting.egg-info/requires.txt
 src/mia_accounting.egg-info/top_level.txt
 tests/babel-utils-test-site.py
```

### Comparing `mia-accounting-1.3.3/tests/babel-utils-test-site.py` & `mia-accounting-1.4.0/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/babel-utils.py` & `mia-accounting-1.4.0/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_account.py` & `mia-accounting-1.4.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_base_account.py` & `mia-accounting-1.4.0/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_commands.py` & `mia-accounting-1.4.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_currency.py` & `mia-accounting-1.4.0/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_description_editor.py` & `mia-accounting-1.4.0/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_journal_entry.py` & `mia-accounting-1.4.0/tests/test_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_offset.py` & `mia-accounting-1.4.0/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_option.py` & `mia-accounting-1.4.0/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_report.py` & `mia-accounting-1.4.0/tests/test_report.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,18 +103,34 @@
 
         response = client.get(f"{PREFIX}/unapplied")
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/unapplied?as=csv")
         self.assertEqual(response.status_code, 403)
 
-        response = client.get(f"{PREFIX}/unapplied/{Accounts.PAYABLE}")
+        response = client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 403)
 
-        response = client.get(f"{PREFIX}/unapplied/{Accounts.PAYABLE}?as=csv")
+        response = client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}?as=csv")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(f"{PREFIX}/unmatched")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(f"{PREFIX}/unmatched?as=csv")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/search?q=Salary")
         self.assertEqual(response.status_code, 403)
 
         response = client.get(f"{PREFIX}/search?q=Salary&as=csv")
         self.assertEqual(response.status_code, 403)
@@ -186,21 +202,37 @@
         response = client.get(f"{PREFIX}/unapplied")
         self.assertEqual(response.status_code, 200)
 
         response = client.get(f"{PREFIX}/unapplied?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = client.get(f"{PREFIX}/unapplied/{Accounts.PAYABLE}")
+        response = client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 200)
 
-        response = client.get(f"{PREFIX}/unapplied/{Accounts.PAYABLE}?as=csv")
+        response = client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
+        response = client.get(f"{PREFIX}/unmatched")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(f"{PREFIX}/unmatched?as=csv")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 403)
+
+        response = client.get(
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}?as=csv")
+        self.assertEqual(response.status_code, 403)
+
         response = client.get(f"{PREFIX}/search?q=Salary")
         self.assertEqual(response.status_code, 200)
 
         response = client.get(f"{PREFIX}/search?q=Salary&as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
@@ -271,19 +303,36 @@
         response = self.client.get(f"{PREFIX}/unapplied")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(f"{PREFIX}/unapplied?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/unapplied/{Accounts.PAYABLE}")
+        response = self.client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}?as=csv")
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.headers["Content-Type"], CSV_MIME)
+
+        response = self.client.get(f"{PREFIX}/unmatched")
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.get(f"{PREFIX}/unmatched?as=csv")
         self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
         response = self.client.get(
-            f"{PREFIX}/unapplied/{Accounts.PAYABLE}?as=csv")
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.get(
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
         response = self.client.get(f"{PREFIX}/search?q=Salary")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(f"{PREFIX}/search?q=Salary&as=csv")
@@ -356,19 +405,36 @@
         response = self.client.get(f"{PREFIX}/unapplied")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(f"{PREFIX}/unapplied?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
-        response = self.client.get(f"{PREFIX}/unapplied/{Accounts.PAYABLE}")
+        response = self.client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}")
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.get(
+            f"{PREFIX}/unapplied/USD/{Accounts.PAYABLE}?as=csv")
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.headers["Content-Type"], CSV_MIME)
+
+        response = self.client.get(f"{PREFIX}/unmatched")
+        self.assertEqual(response.status_code, 200)
+
+        response = self.client.get(f"{PREFIX}/unmatched?as=csv")
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.headers["Content-Type"], CSV_MIME)
+
+        response = self.client.get(
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(
-            f"{PREFIX}/unapplied/{Accounts.PAYABLE}?as=csv")
+            f"{PREFIX}/unmatched/USD/{Accounts.PAYABLE}?as=csv")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.headers["Content-Type"], CSV_MIME)
 
         response = self.client.get(f"{PREFIX}/search?q=Salary")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(f"{PREFIX}/search?q=Salary&as=csv")
```

### Comparing `mia-accounting-1.3.3/tests/test_site/__init__.py` & `mia-accounting-1.4.0/tests/test_site/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/auth.py` & `mia-accounting-1.4.0/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/lib.py` & `mia-accounting-1.4.0/tests/test_site/lib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/locale.py` & `mia-accounting-1.4.0/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/reset.py` & `mia-accounting-1.4.0/tests/test_site/reset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/static/favicon.svg` & `mia-accounting-1.4.0/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/templates/base.html` & `mia-accounting-1.4.0/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/templates/login.html` & `mia-accounting-1.4.0/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/templates/reset.html` & `mia-accounting-1.4.0/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/translations/messages.pot` & `mia-accounting-1.4.0/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.4.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.4.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.4.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.4.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/test_unmatched_offset.py` & `mia-accounting-1.4.0/tests/test_unmatched_offset.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 import httpx
 from flask import Flask
 
 from test_site import db
 from test_site.lib import JournalEntryCurrencyData, JournalEntryData, \
     BaseTestData
-from testlib import create_test_app, get_client, Accounts
+from testlib import NEXT_URI, create_test_app, get_client, Accounts
 
-PREFIX: str = "/accounting/unmatched-offsets"
+PREFIX: str = "/accounting/match-offsets/USD"
 """The URL prefix for the unmatched offset management."""
 
 
 class UnmatchedOffsetTestCase(unittest.TestCase):
     """The unmatched offset test case."""
 
     def setUp(self) -> None:
@@ -54,188 +54,171 @@
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "nobody")
         DifferentTestData(self.app, "nobody").populate()
         response: httpx.Response
 
-        response = client.get(PREFIX)
-        self.assertEqual(response.status_code, 403)
-
-        response = client.get(f"{PREFIX}/{Accounts.PAYABLE}")
-        self.assertEqual(response.status_code, 403)
-
         response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
-                               data={"csrf_token": csrf_token})
+                               data={"csrf_token": csrf_token,
+                                     "next": NEXT_URI})
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "viewer")
         DifferentTestData(self.app, "viewer").populate()
         response: httpx.Response
 
-        response = client.get(PREFIX)
-        self.assertEqual(response.status_code, 403)
-
-        response = client.get(f"{PREFIX}/{Accounts.PAYABLE}")
-        self.assertEqual(response.status_code, 403)
-
         response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
-                               data={"csrf_token": csrf_token})
+                               data={"csrf_token": csrf_token,
+                                     "next": NEXT_URI})
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
         DifferentTestData(self.app, "editor").populate()
         response: httpx.Response
 
-        response = self.client.get(PREFIX)
-        self.assertEqual(response.status_code, 200)
-
-        response = self.client.get(f"{PREFIX}/{Accounts.PAYABLE}")
-        self.assertEqual(response.status_code, 200)
-
         response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
-                                    data={"csrf_token": self.csrf_token})
+                                    data={"csrf_token": self.csrf_token,
+                                          "next": NEXT_URI})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{Accounts.PAYABLE}")
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_empty_db(self) -> None:
         """Test the empty database.
 
         :return: None.
         """
         response: httpx.Response
 
-        response = self.client.get(PREFIX)
-        self.assertEqual(response.status_code, 200)
-
-        response = self.client.get(f"{PREFIX}/{Accounts.PAYABLE}")
-        self.assertEqual(response.status_code, 200)
-
         response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
-                                    data={"csrf_token": self.csrf_token})
+                                    data={"csrf_token": self.csrf_token,
+                                          "next": NEXT_URI})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{Accounts.PAYABLE}")
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_different(self) -> None:
         """Tests to match against different descriptions and amounts.
 
         :return: None.
         """
-        from accounting.models import Account, JournalEntryLineItem
-        from accounting.utils.offset_matcher import OffsetMatcher
+        from accounting.models import Currency, Account, JournalEntryLineItem
+        from accounting.report.utils.offset_matcher import OffsetMatcher
+        from accounting.template_globals import default_currency_code
         data: DifferentTestData = DifferentTestData(self.app, "editor")
         data.populate()
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
-        list_uri: str
         match_uri: str
         response: httpx.Response
 
+        with self.app.app_context():
+            currency: Currency | None \
+                = db.session.get(Currency, default_currency_code())
+            assert currency is not None
+
         # The receivables
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or1d.id, data.l_r_or2d.id,
                               data.l_r_or3d.id, data.l_r_or4d.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_r_of1c.id, data.l_r_of2c.id,
                               data.l_r_of3c.id, data.l_r_of4c.id,
                               data.l_r_of5c.id})
             self.assertEqual({(x.original_line_item.id, x.offset.id)
                               for x in matcher.matched_pairs},
                              {(data.l_r_or4d.id, data.l_r_of5c.id)})
             for line_item_id in {data.l_r_of1c.id, data.l_r_of2c.id,
                                  data.l_r_of3c.id, data.l_r_of4c.id,
                                  data.l_r_of5c.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
-        list_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
         match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
         response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token})
+                                    data={"csrf_token": self.csrf_token,
+                                          "next": NEXT_URI})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], list_uri)
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or1d.id, data.l_r_or2d.id,
                               data.l_r_or3d.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_r_of1c.id, data.l_r_of2c.id,
                               data.l_r_of3c.id, data.l_r_of4c.id})
-            self.assertEqual(matcher.matches, 0)
+            self.assertEqual(len(matcher.matched_pairs), 0)
             for line_item_id in {data.l_r_of1c.id, data.l_r_of2c.id,
                                  data.l_r_of3c.id, data.l_r_of4c.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_r_of5c.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or4d.id)
 
         # The payables
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or1c.id, data.l_p_or2c.id,
                               data.l_p_or3c.id, data.l_p_or4c.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_p_of1d.id, data.l_p_of2d.id,
                               data.l_p_of3d.id, data.l_p_of4d.id,
                               data.l_p_of5d.id})
             self.assertEqual({(x.original_line_item.id, x.offset.id)
                               for x in matcher.matched_pairs},
                              {(data.l_p_or4c.id, data.l_p_of5d.id)})
             for line_item_id in {data.l_p_of1d.id, data.l_p_of2d.id,
                                  data.l_p_of3d.id, data.l_p_of4d.id,
                                  data.l_p_of5d.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
-        list_uri = f"{PREFIX}/{Accounts.PAYABLE}"
         match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
         response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token})
+                                    data={"csrf_token": self.csrf_token,
+                                          "next": NEXT_URI})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], list_uri)
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or1c.id, data.l_p_or2c.id,
                               data.l_p_or3c.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_p_of1d.id, data.l_p_of2d.id,
                               data.l_p_of3d.id, data.l_p_of4d.id})
-            self.assertEqual(matcher.matches, 0)
+            self.assertEqual(len(matcher.matched_pairs), 0)
             for line_item_id in {data.l_p_of1d.id, data.l_p_of2d.id,
                                  data.l_p_of3d.id, data.l_p_of4d.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_p_of5d.id)
             self.assertIsNotNone(line_item)
@@ -243,35 +226,40 @@
             self.assertEqual(line_item.original_line_item_id, data.l_p_or4c.id)
 
     def test_same(self) -> None:
         """Tests to match against same descriptions and amounts.
 
         :return: None.
         """
-        from accounting.models import Account, JournalEntryLineItem
-        from accounting.utils.offset_matcher import OffsetMatcher
+        from accounting.models import Currency, Account, JournalEntryLineItem
+        from accounting.report.utils.offset_matcher import OffsetMatcher
+        from accounting.template_globals import default_currency_code
         data: SameTestData = SameTestData(self.app, "editor")
         data.populate()
         account: Account | None
         line_item: JournalEntryLineItem | None
         matcher: OffsetMatcher
-        list_uri: str
         match_uri: str
         response: httpx.Response
 
+        with self.app.app_context():
+            currency: Currency | None \
+                = db.session.get(Currency, default_currency_code())
+            assert currency is not None
+
         # The receivables
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or1d.id, data.l_r_or3d.id,
                               data.l_r_or4d.id, data.l_r_or5d.id,
                               data.l_r_or6d.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_r_of1c.id, data.l_r_of2c.id,
                               data.l_r_of4c.id, data.l_r_of5c.id,
                               data.l_r_of6c.id})
             self.assertEqual({(x.original_line_item.id, x.offset.id)
                               for x in matcher.matched_pairs},
                              {(data.l_r_or1d.id, data.l_r_of2c.id),
                               (data.l_r_or3d.id, data.l_r_of4c.id),
@@ -283,30 +271,30 @@
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_r_of3c.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or2d.id)
 
-        list_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
         match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
         response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token})
+                                    data={"csrf_token": self.csrf_token,
+                                          "next": NEXT_URI})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], list_uri)
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_r_or5d.id, data.l_r_or6d.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_r_of1c.id, data.l_r_of5c.id})
-            self.assertEqual(matcher.matches, 0)
+            self.assertEqual(len(matcher.matched_pairs), 0)
             for line_item_id in {data.l_r_of1c.id, data.l_r_of5c.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_r_of2c.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
@@ -324,20 +312,20 @@
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or4d.id)
 
         # The payables
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or1c.id, data.l_p_or3c.id,
                               data.l_p_or4c.id, data.l_p_or5c.id,
                               data.l_p_or6c.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_p_of1d.id, data.l_p_of2d.id,
                               data.l_p_of4d.id, data.l_p_of5d.id,
                               data.l_p_of6d.id})
             self.assertEqual({(x.original_line_item.id, x.offset.id)
                               for x in matcher.matched_pairs},
                              {(data.l_p_or1c.id, data.l_p_of2d.id),
                               (data.l_p_or3c.id, data.l_p_of4d.id),
@@ -349,30 +337,30 @@
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_p_of3d.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_p_or2c.id)
 
-        list_uri = f"{PREFIX}/{Accounts.PAYABLE}"
         match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
         response = self.client.post(match_uri,
-                                    data={"csrf_token": self.csrf_token})
+                                    data={"csrf_token": self.csrf_token,
+                                          "next": NEXT_URI})
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], list_uri)
+        self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
-            matcher = OffsetMatcher(account)
+            matcher = OffsetMatcher(currency, account)
             self.assertEqual({x.id for x in matcher.unapplied},
                              {data.l_p_or5c.id, data.l_p_or6c.id})
-            self.assertEqual({x.id for x in matcher.unmatched_offsets},
+            self.assertEqual({x.id for x in matcher.unmatched},
                              {data.l_p_of1d.id, data.l_p_of5d.id})
-            self.assertEqual(matcher.matches, 0)
+            self.assertEqual(len(matcher.matched_pairs), 0)
             for line_item_id in {data.l_p_of1d.id, data.l_p_of5d.id}:
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
             line_item = db.session.get(JournalEntryLineItem, data.l_p_of2d.id)
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
```

### Comparing `mia-accounting-1.3.3/tests/test_utils.py` & `mia-accounting-1.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/testlib.py` & `mia-accounting-1.4.0/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.3/tests/testlib_journal_entry.py` & `mia-accounting-1.4.0/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

