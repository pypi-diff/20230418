# Comparing `tmp/delphi_utils-0.3.8.tar.gz` & `tmp/delphi_utils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphi_utils-0.3.8.tar", last modified: Mon Jan 30 14:56:22 2023, max compression
+gzip compressed data, was "delphi_utils-0.3.9.tar", last modified: Mon Feb  6 19:28:02 2023, max compression
```

## Comparing `delphi_utils-0.3.8.tar` & `delphi_utils-0.3.9.tar`

### file list

```diff
@@ -1,78 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:22.779257 delphi_utils-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-01-30 14:56:22.779257 delphi_utils-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:22.755256 delphi_utils-0.3.8/delphi_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27067 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:22.751256 delphi_utils-0.3.8/delphi_utils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:22.763256 delphi_utils-0.3.8/delphi_utils/data/2019/
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/fips_hhs_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   147974 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/fips_hrr_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/fips_msa_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38706 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/fips_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69872 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/fips_state_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1438655 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/fips_zip_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/hhs_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)    64764 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/jhu_uid_fips_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/nation_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/state_code_hhs_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/state_codes_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/state_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1019998 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/zip_fips_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   829875 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/zip_hhs_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   403215 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/zip_hrr_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   484155 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/zip_hsa_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   411131 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/zip_msa_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   361441 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/zip_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1416681 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2019/zip_state_code_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:22.775257 delphi_utils-0.3.8/delphi_utils/data/2020/
--rw-r--r--   0 runner    (1001) docker     (123)    26506 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/fips_hhs_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   147974 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/fips_hrr_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/fips_msa_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/fips_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69891 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/fips_state_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1438655 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/fips_zip_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/hhs_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)    64764 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/jhu_uid_fips_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/nation_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/state_code_hhs_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/state_codes_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/state_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1019998 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/zip_fips_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   829875 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/zip_hhs_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   403215 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/zip_hrr_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   484155 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/zip_hsa_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   411131 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/zip_msa_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)   361117 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/zip_pop.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1416681 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/data/2020/zip_state_code_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/geomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/nancodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:22.779257 delphi_utils-0.3.8/delphi_utils/validator/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/datafetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    33192 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19153 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/validator/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/delphi_utils/weekday.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:56:22.755256 delphi_utils-0.3.8/delphi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-01-30 14:56:22.000000 delphi_utils-0.3.8/delphi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-01-30 14:56:22.000000 delphi_utils-0.3.8/delphi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 14:56:22.000000 delphi_utils-0.3.8/delphi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-30 14:56:22.000000 delphi_utils-0.3.8/delphi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-30 14:56:22.000000 delphi_utils-0.3.8/delphi_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 14:56:22.779257 delphi_utils-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-30 14:54:38.000000 delphi_utils-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.085908 delphi_utils-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-02-06 19:28:02.085908 delphi_utils-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.065908 delphi_utils-0.3.9/delphi_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27067 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.061908 delphi_utils-0.3.9/delphi_utils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.073908 delphi_utils-0.3.9/delphi_utils/data/2019/
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/fips_hhs_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   147974 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/fips_hrr_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/fips_msa_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38706 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/fips_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69872 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/fips_state_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1438655 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/fips_zip_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/hhs_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    64764 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/jhu_uid_fips_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/nation_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/state_code_hhs_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/state_codes_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/state_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1019998 2023-02-06 19:26:15.000000 delphi_utils-0.3.9/delphi_utils/data/2019/zip_fips_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   829875 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2019/zip_hhs_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   403215 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2019/zip_hrr_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   484155 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2019/zip_hsa_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   411131 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2019/zip_msa_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   361441 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2019/zip_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1416681 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2019/zip_state_code_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.081908 delphi_utils-0.3.9/delphi_utils/data/2020/
+-rw-r--r--   0 runner    (1001) docker     (123)    26506 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/fips_hhs_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   147974 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/fips_hrr_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/fips_msa_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38715 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/fips_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69891 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/fips_state_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1438655 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/fips_zip_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/hhs_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    64764 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/jhu_uid_fips_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/nation_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/state_code_hhs_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/state_codes_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/state_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1019998 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/zip_fips_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   829875 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/zip_hhs_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   403215 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/zip_hrr_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   484155 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/zip_hsa_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   411131 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/zip_msa_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   361117 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/zip_pop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1416681 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/data/2020/zip_state_code_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.085908 delphi_utils-0.3.9/delphi_utils/flash_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/flash_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/flash_eval/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/flash_eval/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/flash_eval/eval_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/flash_eval/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/geomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/nancodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.085908 delphi_utils-0.3.9/delphi_utils/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/datafetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33192 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19153 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/validator/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/delphi_utils/weekday.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:28:02.065908 delphi_utils-0.3.9/delphi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-02-06 19:28:01.000000 delphi_utils-0.3.9/delphi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-02-06 19:28:01.000000 delphi_utils-0.3.9/delphi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 19:28:01.000000 delphi_utils-0.3.9/delphi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-06 19:28:01.000000 delphi_utils-0.3.9/delphi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-06 19:28:01.000000 delphi_utils-0.3.9/delphi_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 19:28:02.085908 delphi_utils-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-06 19:26:16.000000 delphi_utils-0.3.9/setup.py
```

### Comparing `delphi_utils-0.3.8/LICENSE` & `delphi_utils-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/PKG-INFO` & `delphi_utils-0.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi_utils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Shared Utility Functions for Indicators
 Home-page: https://github.com/cmu-delphi/
 Author: 
 Author-email: 
 License: UNKNOWN
 Description: # Delphi Python Utilities
```

### Comparing `delphi_utils-0.3.8/README.md` & `delphi_utils-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/__init__.py` & `delphi_utils-0.3.9/delphi_utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 from .logger import get_structured_logger
 from .geomap import GeoMapper
 from .smooth import Smoother
 from .signal import add_prefix
 from .nancodes import Nans
 from .weekday import Weekday
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `delphi_utils-0.3.8/delphi_utils/archive.py` & `delphi_utils-0.3.9/delphi_utils/archive.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/fips_hhs_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/fips_hhs_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/fips_hrr_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/fips_hrr_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/fips_msa_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/fips_msa_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/fips_pop.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/fips_pop.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/fips_state_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/fips_state_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/fips_zip_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/fips_zip_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/jhu_uid_fips_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/jhu_uid_fips_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/state_codes_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/state_codes_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/state_pop.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/state_pop.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/zip_fips_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/zip_fips_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/zip_hhs_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/zip_hhs_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/zip_hrr_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/zip_hrr_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/zip_hsa_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/zip_hsa_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/zip_msa_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/zip_msa_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/zip_pop.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/zip_pop.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2019/zip_state_code_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2019/zip_state_code_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/fips_hhs_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/fips_hhs_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/fips_hrr_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/fips_hrr_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/fips_msa_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/fips_msa_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/fips_pop.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/fips_pop.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/fips_state_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/fips_state_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/fips_zip_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/fips_zip_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/jhu_uid_fips_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/jhu_uid_fips_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/state_codes_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/state_codes_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/state_pop.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/state_pop.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/zip_fips_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/zip_fips_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/zip_hhs_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/zip_hhs_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/zip_hrr_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/zip_hrr_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/zip_hsa_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/zip_hsa_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/zip_msa_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/zip_msa_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/zip_pop.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/zip_pop.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/data/2020/zip_state_code_table.csv` & `delphi_utils-0.3.9/delphi_utils/data/2020/zip_state_code_table.csv`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/export.py` & `delphi_utils-0.3.9/delphi_utils/export.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/geomap.py` & `delphi_utils-0.3.9/delphi_utils/geomap.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/logger.py` & `delphi_utils-0.3.9/delphi_utils/logger.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/runner.py` & `delphi_utils-0.3.9/delphi_utils/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 """Indicator running utilities."""
 import argparse as ap
 import importlib
 import os
 from typing import Any, Callable, Dict, Optional
+import threading
 from .archive import ArchiveDiffer, archiver_from_params
 from .logger import get_structured_logger
 from .utils import read_params, transfer_files, delete_move_files
 from .validator.validate import Validator
 from .validator.run import validator_from_params
 
+
 Params = Dict[str, Any]
 
 # Trivial function to use as default value for validator and archive functions.
 NULL_FN = lambda x: None
 
 def run_indicator_pipeline(indicator_fn:  Callable[[Params], None],
+                            flash_fn: Callable[[Params], None] = NULL_FN,
                            validator_fn:  Callable[[Params], Optional[Validator]] = NULL_FN,
-                           archiver_fn:  Callable[[Params], Optional[ArchiveDiffer]] = NULL_FN):
+                           archiver_fn:  Callable[[Params], Optional[ArchiveDiffer]] = NULL_FN,
+                             timer=1):
     """Run an indicator with its optional validation and archiving.
 
     Each argument to this function should itself be a function that will be passed a common set of
-    parameters (see details below).  This parameter dictionary should have four subdictionaries
-    keyed as "indicator", "validation", "archive", and "common" corresponding to parameters to be
-    used in `indicator_fn`, `validator_fn`, `archiver_fn`, and shared across functions,
-    respectively.
+    parameters (see details below).  This parameter dictionary should have five subdictionaries
+    keyed as "indicator", "validation", "archive", "flash", and "common" corresponding to parameters
+    to be used in `indicator_fn`, `validator_fn`, `archiver_fn`, `flash_fn` and shared across
+    functions, respectively.The timer function stops the flash process after a certain time.
 
     Arguments
     ---------
     indicator_fn: Callable[[Params], None]
         function that takes a dictionary of parameters and produces indicator output
+    flash_fn: Callable[[Params], None]
+        function that takes a dictionary of parameters and writes points of interest to the log.
     validator_fn: Callable[[Params], Optional[Validator]]
         function that takes a dictionary of parameters and produces the associated Validator or
         None if no validation should be performed.
     archiver_fn: Callable[[Params], Optional[ArchiveDiffer]]
         function that takes a dictionary of parameters and produces the associated ArchiveDiffer or
         None if no archiving should be performed.
     """
@@ -55,14 +61,24 @@
     #Logging - Starting Indicator
         logger.info(f"Started {ind_name} with covidcast-indicators version {current_version}")
     else: logger.info(f"Started {ind_name} without version.cfg")
 
     indicator_fn(params)
     validator = validator_fn(params)
     archiver = archiver_fn(params)
+
+    if flash_fn:
+        t = threading.Timer(timer, flash_fn(params))
+        t.start()
+        t.join(timer)
+        if t.is_alive():
+            t.cancel()
+            t.join()
+
+
     if validator:
         validation_report = validator.validate()
         validation_report.log(logger)
         # Validators on dry-run always return success
         if not validation_report.success():
             delete_move_files()
     if (not validator or validation_report.success()):
@@ -76,10 +92,14 @@
     parser = ap.ArgumentParser()
     parser.add_argument("indicator_name",
                         type=str,
                         help="Name of the Python package containing the indicator.  This package "
                              "must export a `run.run_module(params)` function.")
     args = parser.parse_args()
     indicator_module = importlib.import_module(args.indicator_name)
+    flash_module = importlib.import_module('delphi_utils.flash_eval.run')
     run_indicator_pipeline(indicator_module.run.run_module,
+                           flash_module.run_module,
                            validator_from_params,
-                           archiver_from_params)
+                           archiver_from_params,
+                           timer=600
+                           )
```

### Comparing `delphi_utils-0.3.8/delphi_utils/signal.py` & `delphi_utils-0.3.9/delphi_utils/signal.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/slack_notifier.py` & `delphi_utils-0.3.9/delphi_utils/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/smooth.py` & `delphi_utils-0.3.9/delphi_utils/smooth.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/utils.py` & `delphi_utils-0.3.9/delphi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/datafetcher.py` & `delphi_utils-0.3.9/delphi_utils/validator/datafetcher.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/dynamic.py` & `delphi_utils-0.3.9/delphi_utils/validator/dynamic.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/errors.py` & `delphi_utils-0.3.9/delphi_utils/validator/errors.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/report.py` & `delphi_utils-0.3.9/delphi_utils/validator/report.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/run.py` & `delphi_utils-0.3.9/delphi_utils/validator/run.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/static.py` & `delphi_utils-0.3.9/delphi_utils/validator/static.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/utils.py` & `delphi_utils-0.3.9/delphi_utils/validator/utils.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils/validator/validate.py` & `delphi_utils-0.3.9/delphi_utils/validator/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,11 @@
         Returns:
             - ValidationReport collating the validation outcomes
         """
         report = ValidationReport(self.suppressed_errors, self.data_source, self.dry_run)
         frames_list = load_all_files(self.export_dir, self.time_window.start_date,
                                      self.time_window.end_date)
         self.static_validation.validate(frames_list, report)
-        # Check if frames_list is empty before calling aggregate_frames
-        if len(frames_list) == 0:
-            all_frames = []
-        else:
-            all_frames = aggregate_frames(frames_list)
-        self.dynamic_validation.validate(all_frames, report)
+        # Dynamic Validation only performed when frames_list is populated
+        if len(frames_list) > 0:
+            self.dynamic_validation.validate(aggregate_frames(frames_list), report)
         return report
```

### Comparing `delphi_utils-0.3.8/delphi_utils/weekday.py` & `delphi_utils-0.3.9/delphi_utils/weekday.py`

 * *Files identical despite different names*

### Comparing `delphi_utils-0.3.8/delphi_utils.egg-info/PKG-INFO` & `delphi_utils-0.3.9/delphi_utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi-utils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Shared Utility Functions for Indicators
 Home-page: https://github.com/cmu-delphi/
 Author: 
 Author-email: 
 License: UNKNOWN
 Description: # Delphi Python Utilities
```

### Comparing `delphi_utils-0.3.8/delphi_utils.egg-info/SOURCES.txt` & `delphi_utils-0.3.9/delphi_utils.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 delphi_utils/data/2020/zip_fips_table.csv
 delphi_utils/data/2020/zip_hhs_table.csv
 delphi_utils/data/2020/zip_hrr_table.csv
 delphi_utils/data/2020/zip_hsa_table.csv
 delphi_utils/data/2020/zip_msa_table.csv
 delphi_utils/data/2020/zip_pop.csv
 delphi_utils/data/2020/zip_state_code_table.csv
+delphi_utils/flash_eval/__init__.py
+delphi_utils/flash_eval/__main__.py
+delphi_utils/flash_eval/constants.py
+delphi_utils/flash_eval/eval_day.py
+delphi_utils/flash_eval/run.py
 delphi_utils/validator/__init__.py
 delphi_utils/validator/__main__.py
 delphi_utils/validator/datafetcher.py
 delphi_utils/validator/dynamic.py
 delphi_utils/validator/errors.py
 delphi_utils/validator/report.py
 delphi_utils/validator/run.py
```

### Comparing `delphi_utils-0.3.8/setup.py` & `delphi_utils-0.3.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "slackclient",
     "structlog",
     "xlrd"
 ]
 
 setup(
     name="delphi_utils",
-    version="0.3.8",
+    version="0.3.9",
     description="Shared Utility Functions for Indicators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="",
     author_email="",
     url="https://github.com/cmu-delphi/",
     install_requires=required,
```

