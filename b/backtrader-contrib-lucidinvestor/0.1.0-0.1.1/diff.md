# Comparing `tmp/backtrader_contrib-lucidinvestor-0.1.0.tar.gz` & `tmp/backtrader_contrib-lucidinvestor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtrader_contrib-lucidinvestor-0.1.0.tar", last modified: Sun Apr 16 14:53:57 2023, max compression
+gzip compressed data, was "backtrader_contrib-lucidinvestor-0.1.1.tar", last modified: Tue Apr 18 11:20:03 2023, max compression
```

## Comparing `backtrader_contrib-lucidinvestor-0.1.0.tar` & `backtrader_contrib-lucidinvestor-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/
--rw-rw-r--   0 flo       (1000) flo       (1000)     2342 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/.gitignore
--rw-rw-r--   0 flo       (1000) flo       (1000)      197 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/LICENSE
--rw-rw-r--   0 flo       (1000) flo       (1000)    11357 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/LICENSE.apache
--rw-rw-r--   0 flo       (1000) flo       (1000)     1464 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/LICENSE.bsd3
--rw-rw-r--   0 flo       (1000) flo       (1000)    35121 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/LICENSE.gplv3
--rw-rw-r--   0 flo       (1000) flo       (1000)     1060 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/LICENSE.mit
--rw-rw-r--   0 flo       (1000) flo       (1000)     1308 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/Makefile
--rw-rw-r--   0 flo       (1000) flo       (1000)     3546 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/PKG-INFO
--rw-rw-r--   0 flo       (1000) flo       (1000)     1971 2023-04-16 14:53:35.000000 backtrader_contrib-lucidinvestor-0.1.0/README.rst
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.219233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/
--rw-rw-r--   0 flo       (1000) flo       (1000)     1645 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.219233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/analyzers/
--rw-rw-r--   0 flo       (1000) flo       (1000)      996 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/analyzers/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.219233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/brokers/
--rw-rw-r--   0 flo       (1000) flo       (1000)      996 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/brokers/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.219233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/commissions/
--rw-rw-r--   0 flo       (1000) flo       (1000)     1002 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/commissions/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.219233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/feeds/
--rw-rw-r--   0 flo       (1000) flo       (1000)      992 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/feeds/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.219233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/filters/
--rw-rw-r--   0 flo       (1000) flo       (1000)      992 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/filters/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.219233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/
--rw-rw-r--   0 flo       (1000) flo       (1000)      997 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/
--rw-rw-r--   0 flo       (1000) flo       (1000)     1485 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/LICENSE.bsd3
--rw-rw-r--   0 flo       (1000) flo       (1000)     2228 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/README.rst
--rw-rw-r--   0 flo       (1000) flo       (1000)      997 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/__init__.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     8383 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/order_management.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     3763 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/portfolio.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     4018 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/strategy_generic.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/utils/
--rw-rw-r--   0 flo       (1000) flo       (1000)     5181 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/utils/analytics.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     4748 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/utils/input_ouput.py
--rw-rw-r--   0 flo       (1000) flo       (1000)    12636 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/utils/run_backtest.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/indicators/
--rw-rw-r--   0 flo       (1000) flo       (1000)      998 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/indicators/__init__.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     2531 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/loadmodule.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/observers/
--rw-rw-r--   0 flo       (1000) flo       (1000)      996 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/observers/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/signals/
--rw-rw-r--   0 flo       (1000) flo       (1000)      992 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/signals/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/sizers/
--rw-rw-r--   0 flo       (1000) flo       (1000)      990 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/sizers/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/stores/
--rw-rw-r--   0 flo       (1000) flo       (1000)      990 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/stores/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/
--rw-rw-r--   0 flo       (1000) flo       (1000)      997 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/
--rw-rw-r--   0 flo       (1000) flo       (1000)     1485 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/LICENSE.bsd3
--rw-rw-r--   0 flo       (1000) flo       (1000)      135 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/README.rst
--rw-rw-r--   0 flo       (1000) flo       (1000)      997 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/strategic_asset_allocation/
--rw-rw-r--   0 flo       (1000) flo       (1000)      190 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/strategic_asset_allocation/60-40.json
--rw-rw-r--   0 flo       (1000) flo       (1000)   252898 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/strategic_asset_allocation/60-40.png
--rw-rw-r--   0 flo       (1000) flo       (1000)        0 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/strategic_asset_allocation/__init__.py
--rw-rw-r--   0 flo       (1000) flo       (1000)    11782 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/strategic_asset_allocation/fixed_target_allocations.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/tactical_asset_allocation/
--rw-rw-r--   0 flo       (1000) flo       (1000)        0 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/tactical_asset_allocation/__init__.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/studies/
--rw-rw-r--   0 flo       (1000) flo       (1000)      995 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/studies/__init.py
--rw-rw-r--   0 flo       (1000) flo       (1000)     1098 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/version.py
-drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/
--rw-rw-r--   0 flo       (1000) flo       (1000)     3546 2023-04-16 14:53:57.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/PKG-INFO
--rw-rw-r--   0 flo       (1000) flo       (1000)     2023 2023-04-16 14:53:57.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/SOURCES.txt
--rw-rw-r--   0 flo       (1000) flo       (1000)        1 2023-04-16 14:53:57.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/dependency_links.txt
--rw-rw-r--   0 flo       (1000) flo       (1000)       25 2023-04-16 14:53:57.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/requires.txt
--rw-rw-r--   0 flo       (1000) flo       (1000)       19 2023-04-16 14:53:57.000000 backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/top_level.txt
--rwxrwxr-x   0 flo       (1000) flo       (1000)      556 2023-04-16 14:50:30.000000 backtrader_contrib-lucidinvestor-0.1.0/pypi.sh
--rw-rw-r--   0 flo       (1000) flo       (1000)      222 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/requirements.txt
--rw-rw-r--   0 flo       (1000) flo       (1000)       80 2023-04-16 14:53:57.223233 backtrader_contrib-lucidinvestor-0.1.0/setup.cfg
--rw-rw-r--   0 flo       (1000) flo       (1000)     5613 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.0/setup.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/
+-rw-rw-r--   0 flo       (1000) flo       (1000)     2342 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/.gitignore
+-rw-rw-r--   0 flo       (1000) flo       (1000)      197 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/LICENSE
+-rw-rw-r--   0 flo       (1000) flo       (1000)    11357 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/LICENSE.apache
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1464 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/LICENSE.bsd3
+-rw-rw-r--   0 flo       (1000) flo       (1000)    35121 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/LICENSE.gplv3
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1060 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/LICENSE.mit
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1308 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/Makefile
+-rw-rw-r--   0 flo       (1000) flo       (1000)     3546 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/PKG-INFO
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1971 2023-04-18 11:07:57.000000 backtrader_contrib-lucidinvestor-0.1.1/README.rst
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1645 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/analyzers/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      996 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/analyzers/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/brokers/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      996 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/brokers/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/commissions/
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1002 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/commissions/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/feeds/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      992 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/feeds/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/filters/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      992 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/filters/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      997 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1485 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/LICENSE.bsd3
+-rw-rw-r--   0 flo       (1000) flo       (1000)     2228 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/README.rst
+-rw-rw-r--   0 flo       (1000) flo       (1000)      997 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/__init__.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)     8383 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/order_management.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)     3763 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/portfolio.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)     4018 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/strategy_generic.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/utils/
+-rw-rw-r--   0 flo       (1000) flo       (1000)     5181 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/utils/analytics.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)     4843 2023-04-18 11:08:01.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/utils/input_ouput.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)    12659 2023-04-18 11:08:01.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/utils/run_backtest.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/indicators/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      998 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/indicators/__init__.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)     2531 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/loadmodule.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.329633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/observers/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      996 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/observers/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/signals/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      992 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/signals/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/sizers/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      990 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/sizers/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/stores/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      990 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/stores/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      997 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1485 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/LICENSE.bsd3
+-rw-rw-r--   0 flo       (1000) flo       (1000)      135 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/README.rst
+-rw-rw-r--   0 flo       (1000) flo       (1000)      997 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/strategic_asset_allocation/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      190 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/strategic_asset_allocation/60-40.json
+-rw-rw-r--   0 flo       (1000) flo       (1000)   252898 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/strategic_asset_allocation/60-40.png
+-rw-rw-r--   0 flo       (1000) flo       (1000)        0 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/strategic_asset_allocation/__init__.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)    11782 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/strategic_asset_allocation/fixed_target_allocations.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/tactical_asset_allocation/
+-rw-rw-r--   0 flo       (1000) flo       (1000)        0 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/tactical_asset_allocation/__init__.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/studies/
+-rw-rw-r--   0 flo       (1000) flo       (1000)      995 2022-12-13 16:21:51.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/studies/__init.py
+-rw-rw-r--   0 flo       (1000) flo       (1000)     1098 2023-04-18 11:08:37.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/version.py
+drwxrwxr-x   0 flo       (1000) flo       (1000)        0 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/
+-rw-rw-r--   0 flo       (1000) flo       (1000)     3546 2023-04-18 11:20:03.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/PKG-INFO
+-rw-rw-r--   0 flo       (1000) flo       (1000)     2023 2023-04-18 11:20:03.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/SOURCES.txt
+-rw-rw-r--   0 flo       (1000) flo       (1000)        1 2023-04-18 11:20:03.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/dependency_links.txt
+-rw-rw-r--   0 flo       (1000) flo       (1000)       25 2023-04-18 11:20:03.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/requires.txt
+-rw-rw-r--   0 flo       (1000) flo       (1000)       19 2023-04-18 11:20:03.000000 backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/top_level.txt
+-rwxrwxr-x   0 flo       (1000) flo       (1000)      552 2023-04-18 11:19:56.000000 backtrader_contrib-lucidinvestor-0.1.1/pypi.sh
+-rw-rw-r--   0 flo       (1000) flo       (1000)      222 2023-04-16 14:46:24.000000 backtrader_contrib-lucidinvestor-0.1.1/requirements.txt
+-rw-rw-r--   0 flo       (1000) flo       (1000)       80 2023-04-18 11:20:03.333633 backtrader_contrib-lucidinvestor-0.1.1/setup.cfg
+-rw-rw-r--   0 flo       (1000) flo       (1000)     5613 2023-04-18 11:14:43.000000 backtrader_contrib-lucidinvestor-0.1.1/setup.py
```

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/.gitignore` & `backtrader_contrib-lucidinvestor-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/LICENSE.apache` & `backtrader_contrib-lucidinvestor-0.1.1/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/LICENSE.bsd3` & `backtrader_contrib-lucidinvestor-0.1.1/LICENSE.bsd3`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/LICENSE.gplv3` & `backtrader_contrib-lucidinvestor-0.1.1/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/LICENSE.mit` & `backtrader_contrib-lucidinvestor-0.1.1/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/Makefile` & `backtrader_contrib-lucidinvestor-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/PKG-INFO` & `backtrader_contrib-lucidinvestor-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: backtrader_contrib-lucidinvestor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Contributions to the Backtrader backtesting engine - maintained by LucidInvestor
 Home-page: https://gitlab.com/algorithmic-trading-library/backtrader_contrib
-Download-URL: https://gitlab.com/algorithmic-trading-library/backtrader_contrib/-/archive/0.1.0/backtrader_contrib-0.1.0.tar.gz
+Download-URL: https://gitlab.com/algorithmic-trading-library/backtrader_contrib/-/archive/0.1.1/backtrader_contrib-0.1.1.tar.gz
 Author: maintainer: LucidInvestor
 Author-email: info@lucidinvestor.ca
 License: GPLv3+
 Keywords: trading,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/README.rst` & `backtrader_contrib-lucidinvestor-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/analyzers/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/brokers/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/commissions/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/commissions/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/feeds/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/feeds/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/filters/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/LICENSE.bsd3` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/LICENSE.bsd3`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/README.rst` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/README.rst`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/order_management.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/order_management.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/portfolio.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/portfolio.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/strategy_generic.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/strategy_generic.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/utils/analytics.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/utils/input_ouput.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/utils/input_ouput.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 import backtrader as bt
 from pandas_datareader import data as pdr
 import yfinance as yf
 
 
 class ImportHistoricalData(object):
 
-    def __init__(self, start_date, end_date, time=9):
+    def __init__(self, start_date, end_date, time=9, tz='America/New_York'):
         self.start_date = start_date
         self.end_date = end_date
         self.time = time
+        self.tz = tz
 
         return
 
     def custom_csv(self, file):
         #######################################################################
         # DATA FORMAT: .csv                                                   #
         # date	close	volume	Open	high	low                           #
@@ -90,14 +91,15 @@
         temp = []
         for i in range(0, len(dataframe.index)):
             temp.append(dataframe.index[i] + pd.DateOffset(hours=9))
 
         # adding the new index in the df, and switching to new index
         dataframe['nysetime'] = pd.Series(temp, index=dataframe.index)
         dataframe.set_index('nysetime', inplace=True)
+        dataframe = dataframe.tz_localize(self.tz)
 
         # reoredering the df chronologically
         data = dataframe.sort_index(ascending=True)
 
         if self.start_date is not None and self.end_date is not None:
             data = data.loc[self.start_date:self.end_date]
         elif self.start_date is not None:
```

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/framework/lucid/utils/run_backtest.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/framework/lucid/utils/run_backtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     cerebro.broker.set_coc(True)  # match a Market order to the closing price of the bar in which the order was issued.
     cerebro.broker.set_checksubmit(checksubmit=True)  # check margin/cash before accepting an order into the system
 
     # get data from csv
     fileDir = os.path.dirname(os.path.abspath(__file__))
     parentDir = os.path.dirname(fileDir)
 
-    historical_data = ImportHistoricalData(start_date, end_date)
+    historical_data = ImportHistoricalData(start_date, end_date, tz='America/New_York')
     for asset in update_target.assets.items():
         symbol = asset[1].symbol.upper()
 
         path = os.path.join(parentDir, datadir, symbol)
         path = path + '.csv'
 
         d1 = None
```

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/indicators/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/loadmodule.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/loadmodule.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/observers/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/observers/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/signals/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/sizers/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/sizers/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/stores/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/LICENSE.bsd3` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/LICENSE.bsd3`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/__init__.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/__init__.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/strategic_asset_allocation/60-40.png` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/strategic_asset_allocation/60-40.png`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/strategies/lucid/strategic_asset_allocation/fixed_target_allocations.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/strategies/lucid/strategic_asset_allocation/fixed_target_allocations.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/studies/__init.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/studies/__init.py`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib/version.py` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 __sversion__ = tuple(int(x) for x in __version__.split('.'))
```

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/PKG-INFO` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: backtrader-contrib-lucidinvestor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Contributions to the Backtrader backtesting engine - maintained by LucidInvestor
 Home-page: https://gitlab.com/algorithmic-trading-library/backtrader_contrib
-Download-URL: https://gitlab.com/algorithmic-trading-library/backtrader_contrib/-/archive/0.1.0/backtrader_contrib-0.1.0.tar.gz
+Download-URL: https://gitlab.com/algorithmic-trading-library/backtrader_contrib/-/archive/0.1.1/backtrader_contrib-0.1.1.tar.gz
 Author: maintainer: LucidInvestor
 Author-email: info@lucidinvestor.ca
 License: GPLv3+
 Keywords: trading,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/backtrader_contrib_lucidinvestor.egg-info/SOURCES.txt` & `backtrader_contrib-lucidinvestor-0.1.1/backtrader_contrib_lucidinvestor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/pypi.sh` & `backtrader_contrib-lucidinvestor-0.1.1/pypi.sh`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sudo apt install twine
 fi
 
 # clean up older versions
 $py_cmd setup.py clean --all
 rm -rf dist
 rm -rf build
-rm -rf *.egg-info
+rm -rf *.egg*
 #
 # Generate pypi wheels universal package and upload
 # in case anything goes wrong use:
 # $twine check dist/*
 $py_cmd setup.py sdist bdist_wheel
 twine check dist/*
 twine upload --config-file ../env_var/secret.pypirc --verbose dist/*
```

### Comparing `backtrader_contrib-lucidinvestor-0.1.0/setup.py` & `backtrader_contrib-lucidinvestor-0.1.1/setup.py`

 * *Files identical despite different names*

