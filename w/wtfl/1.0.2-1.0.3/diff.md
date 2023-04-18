# Comparing `tmp/wtfl-1.0.2.tar.gz` & `tmp/wtfl-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtfl-1.0.2.tar", max compression
+gzip compressed data, was "wtfl-1.0.3.tar", max compression
```

## Comparing `wtfl-1.0.2.tar` & `wtfl-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-04-18 11:20:11.431147 wtfl-1.0.2/LICENSE
--rw-r--r--   0        0        0      381 2023-04-18 11:20:11.431147 wtfl-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-18 11:20:11.431147 wtfl-1.0.2/wtfl/__init__.py
--rw-r--r--   0        0        0     4607 2023-04-18 11:20:11.431147 wtfl-1.0.2/wtfl/grammar.py
--rw-r--r--   0        0        0     2720 2023-04-18 11:20:11.431147 wtfl-1.0.2/wtfl/internal_types.py
--rw-r--r--   0        0        0     4519 2023-04-18 11:20:11.431147 wtfl-1.0.2/wtfl/parser.py
--rw-r--r--   0        0        0     5233 2023-04-18 11:20:11.431147 wtfl-1.0.2/wtfl/reader.py
--rw-r--r--   0        0        0     1798 2023-04-18 11:20:11.431147 wtfl-1.0.2/wtfl/writer.py
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 wtfl-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-18 11:26:56.748016 wtfl-1.0.3/LICENSE
+-rw-r--r--   0        0        0     8723 2023-04-18 11:26:56.748016 wtfl-1.0.3/README.md
+-rw-r--r--   0        0        0      578 2023-04-18 11:26:56.748016 wtfl-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/__init__.py
+-rw-r--r--   0        0        0     4607 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/grammar.py
+-rw-r--r--   0        0        0     2720 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/internal_types.py
+-rw-r--r--   0        0        0     4519 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/parser.py
+-rw-r--r--   0        0        0     5233 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/reader.py
+-rw-r--r--   0        0        0     1798 2023-04-18 11:26:56.748016 wtfl-1.0.3/wtfl/writer.py
+-rw-r--r--   0        0        0     9562 1970-01-01 00:00:00.000000 wtfl-1.0.3/PKG-INFO
```

### Comparing `wtfl-1.0.2/LICENSE` & `wtfl-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.2/wtfl/grammar.py` & `wtfl-1.0.3/wtfl/grammar.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.2/wtfl/internal_types.py` & `wtfl-1.0.3/wtfl/internal_types.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.2/wtfl/parser.py` & `wtfl-1.0.3/wtfl/parser.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.2/wtfl/reader.py` & `wtfl-1.0.3/wtfl/reader.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.0.2/wtfl/writer.py` & `wtfl-1.0.3/wtfl/writer.py`

 * *Files identical despite different names*

