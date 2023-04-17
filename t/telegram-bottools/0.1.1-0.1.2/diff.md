# Comparing `tmp/telegram_bottools-0.1.1.tar.gz` & `tmp/telegram_bottools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_bottools-0.1.1.tar", max compression
+gzip compressed data, was "telegram_bottools-0.1.2.tar", max compression
```

## Comparing `telegram_bottools-0.1.1.tar` & `telegram_bottools-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      320 2023-04-17 19:52:59.957392 telegram_bottools-0.1.1/README.md
--rw-r--r--   0        0        0      365 2023-04-17 21:45:11.612006 telegram_bottools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 19:19:57.449184 telegram_bottools-0.1.1/telegram_bottools/__init__.py
--rw-r--r--   0        0        0     1760 2023-04-17 19:24:04.692427 telegram_bottools-0.1.1/telegram_bottools/telegram_bottools.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 telegram_bottools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-04-17 21:59:33.128358 telegram_bottools-0.1.2/README.md
+-rw-r--r--   0        0        0      383 2023-04-17 22:03:53.531996 telegram_bottools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 21:59:34.629363 telegram_bottools-0.1.2/telegram_bottools/__init__.py
+-rw-r--r--   0        0        0     1760 2023-04-17 21:59:34.632511 telegram_bottools-0.1.2/telegram_bottools/telegram_bottools.py
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 telegram_bottools-0.1.2/PKG-INFO
```

### Comparing `telegram_bottools-0.1.1/telegram_bottools/telegram_bottools.py` & `telegram_bottools-0.1.2/telegram_bottools/telegram_bottools.py`

 * *Files identical despite different names*

