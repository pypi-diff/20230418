# Comparing `tmp/sqlparse-0.4.3.tar.gz` & `tmp/sqlparse-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlparse-0.4.3.tar", last modified: Fri Sep 23 18:40:44 2022, max compression
+gzip compressed data, was "sqlparse-0.4.4.tar", last modified: Tue Apr 18 08:30:17 2023, max compression
```

## Comparing `sqlparse-0.4.3.tar` & `sqlparse-0.4.4.tar`

### file list

```diff
@@ -1,84 +1,69 @@
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.459500 sqlparse-0.4.3/
--rw-r--r--   0 a.albrecht   (502) staff       (20)     3105 2022-09-06 19:32:40.000000 sqlparse-0.4.3/AUTHORS
--rw-r--r--   0 a.albrecht   (502) staff       (20)    18655 2022-09-23 18:30:49.000000 sqlparse-0.4.3/CHANGELOG
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1537 2019-10-09 08:03:19.000000 sqlparse-0.4.3/LICENSE
--rw-r--r--   0 a.albrecht   (502) staff       (20)      228 2019-10-09 08:03:19.000000 sqlparse-0.4.3/MANIFEST.in
--rw-r--r--   0 a.albrecht   (502) staff       (20)      506 2022-09-06 19:32:40.000000 sqlparse-0.4.3/Makefile
--rw-r--r--   0 a.albrecht   (502) staff       (20)     3740 2022-09-23 18:40:44.459821 sqlparse-0.4.3/PKG-INFO
--rw-r--r--   0 a.albrecht   (502) staff       (20)     2317 2022-09-06 19:32:40.000000 sqlparse-0.4.3/README.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)      290 2019-10-09 08:03:19.000000 sqlparse-0.4.3/TODO
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.408364 sqlparse-0.4.3/docs/
--rw-r--r--   0 a.albrecht   (502) staff       (20)     2994 2019-10-09 08:03:19.000000 sqlparse-0.4.3/docs/Makefile
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.411485 sqlparse-0.4.3/docs/source/
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1361 2019-10-09 08:03:19.000000 sqlparse-0.4.3/docs/source/analyzing.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)     2060 2022-09-06 19:32:40.000000 sqlparse-0.4.3/docs/source/api.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)      311 2019-10-09 08:03:19.000000 sqlparse-0.4.3/docs/source/changes.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)     6608 2022-09-06 19:32:40.000000 sqlparse-0.4.3/docs/source/conf.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)      696 2022-09-06 19:32:40.000000 sqlparse-0.4.3/docs/source/index.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)       92 2019-10-09 08:03:19.000000 sqlparse-0.4.3/docs/source/indices.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)     4290 2022-09-06 19:32:40.000000 sqlparse-0.4.3/docs/source/intro.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)       43 2022-09-06 19:32:40.000000 sqlparse-0.4.3/docs/source/license.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)      559 2019-10-09 08:03:19.000000 sqlparse-0.4.3/docs/source/ui.rst
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1792 2019-10-09 08:03:19.000000 sqlparse-0.4.3/docs/sqlformat.1
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1546 2022-09-23 18:40:44.461999 sqlparse-0.4.3/setup.cfg
--rw-r--r--   0 a.albrecht   (502) staff       (20)      284 2022-09-06 19:32:40.000000 sqlparse-0.4.3/setup.py
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.416221 sqlparse-0.4.3/sqlparse/
--rw-r--r--   0 a.albrecht   (502) staff       (20)     2180 2022-09-23 18:29:53.000000 sqlparse-0.4.3/sqlparse/__init__.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)      610 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/__main__.py
--rwxr-xr-x   0 a.albrecht   (502) staff       (20)     5712 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/cli.py
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.420461 sqlparse-0.4.3/sqlparse/engine/
--rw-r--r--   0 a.albrecht   (502) staff       (20)      447 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/engine/__init__.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1193 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/engine/filter_stack.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)    13826 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/engine/grouping.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     3758 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/engine/statement_splitter.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)      342 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/exceptions.py
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.443370 sqlparse-0.4.3/sqlparse/filters/
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1242 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/filters/__init__.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     5110 2022-09-10 08:36:58.000000 sqlparse-0.4.3/sqlparse/filters/aligned_indent.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     5180 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/filters/others.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     4001 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/filters/output.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     9549 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/filters/reindent.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1543 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/filters/right_margin.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1553 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/filters/tokens.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     7566 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/formatter.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)    30162 2022-09-10 08:36:58.000000 sqlparse-0.4.3/sqlparse/keywords.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     2453 2022-09-10 08:29:34.000000 sqlparse-0.4.3/sqlparse/lexer.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)    20398 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/sql.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1661 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/tokens.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     3446 2022-09-06 19:32:40.000000 sqlparse-0.4.3/sqlparse/utils.py
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.418474 sqlparse-0.4.3/sqlparse.egg-info/
--rw-r--r--   0 a.albrecht   (502) staff       (20)     3740 2022-09-23 18:40:44.000000 sqlparse-0.4.3/sqlparse.egg-info/PKG-INFO
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1704 2022-09-23 18:40:44.000000 sqlparse-0.4.3/sqlparse.egg-info/SOURCES.txt
--rw-r--r--   0 a.albrecht   (502) staff       (20)        1 2022-09-23 18:40:44.000000 sqlparse-0.4.3/sqlparse.egg-info/dependency_links.txt
--rw-r--r--   0 a.albrecht   (502) staff       (20)       53 2022-09-23 18:40:44.000000 sqlparse-0.4.3/sqlparse.egg-info/entry_points.txt
--rw-r--r--   0 a.albrecht   (502) staff       (20)        9 2022-09-23 18:40:44.000000 sqlparse-0.4.3/sqlparse.egg-info/top_level.txt
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.449352 sqlparse-0.4.3/tests/
--rw-r--r--   0 a.albrecht   (502) staff       (20)        0 2020-10-07 06:28:34.000000 sqlparse-0.4.3/tests/__init__.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     1571 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/conftest.py
-drwxr-xr-x   0 a.albrecht   (502) staff       (20)        0 2022-09-23 18:40:44.459059 sqlparse-0.4.3/tests/files/
--rw-r--r--   0 a.albrecht   (502) staff       (20)      109 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/_Make_DirEntry.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)       45 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/begintag.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)      357 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/begintag_2.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)      150 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/files/casewhen_procedure.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)       88 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/dashcomment.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)       50 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/encoding_gbk.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)       76 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/encoding_utf8.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)      187 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/function.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)     3066 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/function_psql.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)      177 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/function_psql2.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)      171 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/function_psql3.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)      221 2020-09-30 07:12:29.000000 sqlparse-0.4.3/tests/files/function_psql4.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)     9434 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/huge_select.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)      134 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/files/mysql_handler.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)       44 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/stream.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)       49 2019-10-09 08:03:19.000000 sqlparse-0.4.3/tests/files/test_cp1251.sql
--rw-r--r--   0 a.albrecht   (502) staff       (20)     3533 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_cli.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)    26231 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_format.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)    22932 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_grouping.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)      424 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_keywords.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)    15265 2022-09-10 08:05:08.000000 sqlparse-0.4.3/tests/test_parse.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)    14010 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_regressions.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     4798 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_split.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)     6248 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_tokenize.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)      268 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tests/test_utils.py
--rw-r--r--   0 a.albrecht   (502) staff       (20)      303 2022-09-06 19:32:40.000000 sqlparse-0.4.3/tox.ini
+-rw-r--r--   0        0        0     3105 2022-12-30 11:03:50.592785 sqlparse-0.4.4/AUTHORS
+-rw-r--r--   0        0        0    19534 2023-04-18 08:27:22.670305 sqlparse-0.4.4/CHANGELOG
+-rw-r--r--   0        0        0     1537 2022-12-30 11:03:50.593383 sqlparse-0.4.4/LICENSE
+-rw-r--r--   0        0        0      488 2022-12-30 15:04:41.268404 sqlparse-0.4.4/Makefile
+-rw-r--r--   0        0        0     2317 2022-12-30 11:03:50.594170 sqlparse-0.4.4/README.rst
+-rw-r--r--   0        0        0      290 2022-12-30 11:03:50.594411 sqlparse-0.4.4/TODO
+-rw-r--r--   0        0        0     2994 2019-10-09 08:03:19.949045 sqlparse-0.4.4/docs/Makefile
+-rw-r--r--   0        0        0     1361 2022-12-30 11:03:50.594700 sqlparse-0.4.4/docs/source/analyzing.rst
+-rw-r--r--   0        0        0     2060 2022-12-30 11:03:50.595020 sqlparse-0.4.4/docs/source/api.rst
+-rw-r--r--   0        0        0      311 2022-12-30 11:03:50.595314 sqlparse-0.4.4/docs/source/changes.rst
+-rw-r--r--   0        0        0     6608 2022-12-30 11:03:50.595671 sqlparse-0.4.4/docs/source/conf.py
+-rw-r--r--   0        0        0     3025 2023-03-20 07:41:41.863353 sqlparse-0.4.4/docs/source/extending.rst
+-rw-r--r--   0        0        0      709 2023-03-20 07:41:41.866786 sqlparse-0.4.4/docs/source/index.rst
+-rw-r--r--   0        0        0       92 2022-12-30 11:03:50.596110 sqlparse-0.4.4/docs/source/indices.rst
+-rw-r--r--   0        0        0     4290 2022-12-30 11:03:50.596439 sqlparse-0.4.4/docs/source/intro.rst
+-rw-r--r--   0        0        0       43 2022-12-30 11:03:50.596585 sqlparse-0.4.4/docs/source/license.rst
+-rw-r--r--   0        0        0      559 2022-12-30 11:03:50.596890 sqlparse-0.4.4/docs/source/ui.rst
+-rw-r--r--   0        0        0     1792 2022-12-30 11:03:50.597052 sqlparse-0.4.4/docs/sqlformat.1
+-rw-r--r--   0        0        0     1867 2022-12-30 15:04:41.268766 sqlparse-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2180 2023-04-18 08:24:53.735503 sqlparse-0.4.4/sqlparse/__init__.py
+-rw-r--r--   0        0        0      610 2022-12-30 11:03:50.598850 sqlparse-0.4.4/sqlparse/__main__.py
+-rwxr-xr-x   0        0        0     5712 2022-12-30 11:03:50.599187 sqlparse-0.4.4/sqlparse/cli.py
+-rw-r--r--   0        0        0      447 2022-12-30 11:03:50.599833 sqlparse-0.4.4/sqlparse/engine/__init__.py
+-rw-r--r--   0        0        0     1193 2022-12-30 11:03:50.600246 sqlparse-0.4.4/sqlparse/engine/filter_stack.py
+-rw-r--r--   0        0        0    13826 2022-12-30 11:03:50.601055 sqlparse-0.4.4/sqlparse/engine/grouping.py
+-rw-r--r--   0        0        0     3758 2022-12-30 11:03:50.601699 sqlparse-0.4.4/sqlparse/engine/statement_splitter.py
+-rw-r--r--   0        0        0      342 2022-12-30 11:03:50.602233 sqlparse-0.4.4/sqlparse/exceptions.py
+-rw-r--r--   0        0        0     1242 2022-12-30 11:03:50.602661 sqlparse-0.4.4/sqlparse/filters/__init__.py
+-rw-r--r--   0        0        0     5110 2022-12-30 11:03:50.603097 sqlparse-0.4.4/sqlparse/filters/aligned_indent.py
+-rw-r--r--   0        0        0     5180 2022-12-30 11:03:50.603659 sqlparse-0.4.4/sqlparse/filters/others.py
+-rw-r--r--   0        0        0     4001 2022-12-30 11:03:50.604079 sqlparse-0.4.4/sqlparse/filters/output.py
+-rw-r--r--   0        0        0     9549 2022-12-30 11:03:50.604431 sqlparse-0.4.4/sqlparse/filters/reindent.py
+-rw-r--r--   0        0        0     1543 2022-12-30 11:03:50.604681 sqlparse-0.4.4/sqlparse/filters/right_margin.py
+-rw-r--r--   0        0        0     1553 2022-12-30 11:03:50.604914 sqlparse-0.4.4/sqlparse/filters/tokens.py
+-rw-r--r--   0        0        0     7566 2022-12-30 11:03:50.605285 sqlparse-0.4.4/sqlparse/formatter.py
+-rw-r--r--   0        0        0    29445 2023-04-18 08:23:13.328575 sqlparse-0.4.4/sqlparse/keywords.py
+-rw-r--r--   0        0        0     5786 2023-03-20 07:41:41.867994 sqlparse-0.4.4/sqlparse/lexer.py
+-rw-r--r--   0        0        0    20401 2023-03-20 07:41:41.868462 sqlparse-0.4.4/sqlparse/sql.py
+-rw-r--r--   0        0        0     1661 2022-12-30 11:03:50.607236 sqlparse-0.4.4/sqlparse/tokens.py
+-rw-r--r--   0        0        0     3446 2022-12-30 11:03:50.607533 sqlparse-0.4.4/sqlparse/utils.py
+-rw-r--r--   0        0        0        0 2020-10-07 06:28:34.767618 sqlparse-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     1571 2022-12-30 11:03:50.607837 sqlparse-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0      109 2022-12-30 11:03:50.608055 sqlparse-0.4.4/tests/files/_Make_DirEntry.sql
+-rw-r--r--   0        0        0       45 2019-10-09 08:03:19.956406 sqlparse-0.4.4/tests/files/begintag.sql
+-rw-r--r--   0        0        0      357 2022-12-30 11:03:50.608241 sqlparse-0.4.4/tests/files/begintag_2.sql
+-rw-r--r--   0        0        0      150 2022-12-30 11:03:50.608470 sqlparse-0.4.4/tests/files/casewhen_procedure.sql
+-rw-r--r--   0        0        0       88 2019-10-09 08:03:19.956774 sqlparse-0.4.4/tests/files/dashcomment.sql
+-rw-r--r--   0        0        0       50 2022-12-30 11:03:50.608804 sqlparse-0.4.4/tests/files/encoding_gbk.sql
+-rw-r--r--   0        0        0       76 2022-12-30 11:03:50.609010 sqlparse-0.4.4/tests/files/encoding_utf8.sql
+-rw-r--r--   0        0        0      187 2019-10-09 08:03:19.957228 sqlparse-0.4.4/tests/files/function.sql
+-rw-r--r--   0        0        0     3066 2019-10-09 08:03:19.957352 sqlparse-0.4.4/tests/files/function_psql.sql
+-rw-r--r--   0        0        0      177 2019-10-09 08:03:19.957478 sqlparse-0.4.4/tests/files/function_psql2.sql
+-rw-r--r--   0        0        0      171 2019-10-09 08:03:19.957598 sqlparse-0.4.4/tests/files/function_psql3.sql
+-rw-r--r--   0        0        0      221 2022-12-30 11:03:50.609266 sqlparse-0.4.4/tests/files/function_psql4.sql
+-rw-r--r--   0        0        0     9434 2022-12-30 11:03:50.609519 sqlparse-0.4.4/tests/files/huge_select.sql
+-rw-r--r--   0        0        0      134 2022-12-30 11:03:50.609857 sqlparse-0.4.4/tests/files/mysql_handler.sql
+-rw-r--r--   0        0        0       44 2022-12-30 11:03:50.610224 sqlparse-0.4.4/tests/files/stream.sql
+-rw-r--r--   0        0        0       49 2022-12-30 11:03:50.610491 sqlparse-0.4.4/tests/files/test_cp1251.sql
+-rw-r--r--   0        0        0     3533 2022-12-30 11:03:50.610816 sqlparse-0.4.4/tests/test_cli.py
+-rw-r--r--   0        0        0    26231 2022-12-30 11:03:50.611319 sqlparse-0.4.4/tests/test_format.py
+-rw-r--r--   0        0        0    22636 2022-12-30 11:03:50.611888 sqlparse-0.4.4/tests/test_grouping.py
+-rw-r--r--   0        0        0      447 2023-03-20 07:41:41.869629 sqlparse-0.4.4/tests/test_keywords.py
+-rw-r--r--   0        0        0    17510 2023-03-20 07:41:41.870118 sqlparse-0.4.4/tests/test_parse.py
+-rw-r--r--   0        0        0    14249 2023-03-20 07:41:41.870934 sqlparse-0.4.4/tests/test_regressions.py
+-rw-r--r--   0        0        0     4781 2023-04-18 08:23:13.329035 sqlparse-0.4.4/tests/test_split.py
+-rw-r--r--   0        0        0     6248 2022-12-30 11:03:50.613845 sqlparse-0.4.4/tests/test_tokenize.py
+-rw-r--r--   0        0        0      268 2022-12-30 11:03:50.614084 sqlparse-0.4.4/tests/test_utils.py
+-rw-r--r--   0        0        0      303 2022-12-30 11:03:50.614336 sqlparse-0.4.4/tox.ini
+-rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 sqlparse-0.4.4/PKG-INFO
```

### Comparing `sqlparse-0.4.3/AUTHORS` & `sqlparse-0.4.4/AUTHORS`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/CHANGELOG` & `sqlparse-0.4.4/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Release 0.4.4 (Apr 18, 2023)
+----------------------------
+
+Notable Changes
+
+* IMPORTANT: This release fixes a security vulnerability in the
+  parser where a regular expression vulnerable to ReDOS (Regular
+  Expression Denial of Service) was used. See the security advisory
+  for details: https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-rrm6-wvj7-cwh2
+  The vulnerability was discovered by @erik-krogh from GitHub
+  Security Lab (GHSL). Thanks for reporting!
+
+Bug Fixes
+
+* Revert a change from 0.4.0 that changed IN to be a comparison (issue694).
+  The primary expectation is that IN is treated as a keyword and not as a
+  comparison operator. That also follows the definition of reserved keywords
+  for the major SQL syntax definitions.
+* Fix regular expressions for string parsing.
+
+Other
+
+* sqlparse now uses pyproject.toml instead of setup.cfg (issue685).
+
+
 Release 0.4.3 (Sep 23, 2022)
 ----------------------------
 
 Enhancements
 
 * Add support for DIV operator (pr664, by chezou).
 * Add support for additional SPARK keywords (pr643, by mrmasterplan).
```

### Comparing `sqlparse-0.4.3/LICENSE` & `sqlparse-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/PKG-INFO` & `sqlparse-0.4.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Metadata-Version: 2.1
 Name: sqlparse
-Version: 0.4.3
+Version: 0.4.4
 Summary: A non-validating SQL parser.
-Home-page: https://github.com/andialbrecht/sqlparse
-Author: Andi Albrecht
-Author-email: albrecht.andi@gmail.com
-License: BSD-3-Clause
-Project-URL: Documentation, https://sqlparse.readthedocs.io/
-Project-URL: Release Notes, https://sqlparse.readthedocs.io/en/latest/changes/
-Project-URL: Source, https://github.com/andialbrecht/sqlparse
-Project-URL: Tracker, https://github.com/andialbrecht/sqlparse/issues
+Author-email: Andi Albrecht <albrecht.andi@gmail.com>
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -23,17 +18,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
-Requires-Python: >=3.5
-License-File: LICENSE
-License-File: AUTHORS
+Requires-Dist: flake8 ; extra == "dev"
+Requires-Dist: build ; extra == "dev"
+Requires-Dist: sphinx ; extra == "doc"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Project-URL: Documentation, https://sqlparse.readthedocs.io/
+Project-URL: Home, https://github.com/andialbrecht/sqlparse
+Project-URL: Release Notes, https://sqlparse.readthedocs.io/en/latest/changes/
+Project-URL: Source, https://github.com/andialbrecht/sqlparse
+Project-URL: Tracker, https://github.com/andialbrecht/sqlparse/issues
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: test
 
 python-sqlparse - Parse SQL statements
 ======================================
 
 |buildstatus|_
 |coverage|_
 |docs|_
@@ -105,7 +110,8 @@
 .. _buildstatus: https://github.com/andialbrecht/sqlparse/actions/workflows/python-app.yml
 .. |coverage| image:: https://codecov.io/gh/andialbrecht/sqlparse/branch/master/graph/badge.svg
 .. _coverage: https://codecov.io/gh/andialbrecht/sqlparse
 .. |docs| image:: https://readthedocs.org/projects/sqlparse/badge/?version=latest
 .. _docs: https://sqlparse.readthedocs.io/en/latest/?badge=latest
 .. |packageversion| image:: https://img.shields.io/pypi/v/sqlparse?color=%2334D058&label=pypi%20package
 .. _packageversion: https://pypi.org/project/sqlparse
+
```

### Comparing `sqlparse-0.4.3/README.rst` & `sqlparse-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/docs/Makefile` & `sqlparse-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/docs/source/analyzing.rst` & `sqlparse-0.4.4/docs/source/analyzing.rst`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/docs/source/api.rst` & `sqlparse-0.4.4/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/docs/source/conf.py` & `sqlparse-0.4.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/docs/source/intro.rst` & `sqlparse-0.4.4/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/docs/source/ui.rst` & `sqlparse-0.4.4/docs/source/ui.rst`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/docs/sqlformat.1` & `sqlparse-0.4.4/docs/sqlformat.1`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/__init__.py` & `sqlparse-0.4.4/sqlparse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sqlparse import cli
 from sqlparse import engine
 from sqlparse import tokens
 from sqlparse import filters
 from sqlparse import formatter
 
 
-__version__ = '0.4.3'
+__version__ = '0.4.4'
 __all__ = ['engine', 'filters', 'formatter', 'sql', 'tokens', 'cli']
 
 
 def parse(sql, encoding=None):
     """Parse sql and return a list of statements.
 
     :param sql: A string containing one or more SQL statements.
```

### Comparing `sqlparse-0.4.3/sqlparse/__main__.py` & `sqlparse-0.4.4/sqlparse/__main__.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/cli.py` & `sqlparse-0.4.4/sqlparse/cli.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/engine/filter_stack.py` & `sqlparse-0.4.4/sqlparse/engine/filter_stack.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/engine/grouping.py` & `sqlparse-0.4.4/sqlparse/engine/grouping.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/engine/statement_splitter.py` & `sqlparse-0.4.4/sqlparse/engine/statement_splitter.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/filters/__init__.py` & `sqlparse-0.4.4/sqlparse/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/filters/aligned_indent.py` & `sqlparse-0.4.4/sqlparse/filters/aligned_indent.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/filters/others.py` & `sqlparse-0.4.4/sqlparse/filters/others.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/filters/output.py` & `sqlparse-0.4.4/sqlparse/filters/output.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/filters/reindent.py` & `sqlparse-0.4.4/sqlparse/filters/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/filters/right_margin.py` & `sqlparse-0.4.4/sqlparse/filters/right_margin.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/filters/tokens.py` & `sqlparse-0.4.4/sqlparse/filters/tokens.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/formatter.py` & `sqlparse-0.4.4/sqlparse/formatter.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/keywords.py` & `sqlparse-0.4.4/sqlparse/keywords.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,116 +1,100 @@
 #
 # Copyright (C) 2009-2020 the sqlparse authors and contributors
 # <see AUTHORS file>
 #
 # This module is part of python-sqlparse and is released under
 # the BSD License: https://opensource.org/licenses/BSD-3-Clause
 
-import re
-
 from sqlparse import tokens
 
-
-def is_keyword(value):
-    """Checks for a keyword.
-
-    If the given value is in one of the KEYWORDS_* dictionary
-    it's considered a keyword. Otherwise tokens.Name is returned.
-    """
-    val = value.upper()
-    return (KEYWORDS_COMMON.get(val)
-            or KEYWORDS_ORACLE.get(val)
-            or KEYWORDS_PLPGSQL.get(val)
-            or KEYWORDS_HQL.get(val)
-            or KEYWORDS_MSACCESS.get(val)
-            or KEYWORDS.get(val, tokens.Name)), value
-
-
-SQL_REGEX = {
-    'root': [
-        (r'(--|# )\+.*?(\r\n|\r|\n|$)', tokens.Comment.Single.Hint),
-        (r'/\*\+[\s\S]*?\*/', tokens.Comment.Multiline.Hint),
-
-        (r'(--|# ).*?(\r\n|\r|\n|$)', tokens.Comment.Single),
-        (r'/\*[\s\S]*?\*/', tokens.Comment.Multiline),
-
-        (r'(\r\n|\r|\n)', tokens.Newline),
-        (r'\s+?', tokens.Whitespace),
-
-        (r':=', tokens.Assignment),
-        (r'::', tokens.Punctuation),
-
-        (r'\*', tokens.Wildcard),
-
-        (r"`(``|[^`])*`", tokens.Name),
-        (r"´(´´|[^´])*´", tokens.Name),
-        (r'((?<!\S)\$(?:[_A-ZÀ-Ü]\w*)?\$)[\s\S]*?\1', tokens.Literal),
-
-        (r'\?', tokens.Name.Placeholder),
-        (r'%(\(\w+\))?s', tokens.Name.Placeholder),
-        (r'(?<!\w)[$:?]\w+', tokens.Name.Placeholder),
-
-        (r'\\\w+', tokens.Command),
-        (r'(NOT\s+)?(IN)\b', tokens.Operator.Comparison),
-        # FIXME(andi): VALUES shouldn't be listed here
-        # see https://github.com/andialbrecht/sqlparse/pull/64
-        # AS and IN are special, it may be followed by a parenthesis, but
-        # are never functions, see issue183 and issue507
-        (r'(CASE|IN|VALUES|USING|FROM|AS)\b', tokens.Keyword),
-
-        (r'(@|##|#)[A-ZÀ-Ü]\w+', tokens.Name),
-
-        # see issue #39
-        # Spaces around period `schema . name` are valid identifier
-        # TODO: Spaces before period not implemented
-        (r'[A-ZÀ-Ü]\w*(?=\s*\.)', tokens.Name),  # 'Name'.
-        # FIXME(atronah): never match,
-        # because `re.match` doesn't work with look-behind regexp feature
-        (r'(?<=\.)[A-ZÀ-Ü]\w*', tokens.Name),  # .'Name'
-        (r'[A-ZÀ-Ü]\w*(?=\()', tokens.Name),  # side effect: change kw to func
-        (r'-?0x[\dA-F]+', tokens.Number.Hexadecimal),
-        (r'-?\d+(\.\d+)?E-?\d+', tokens.Number.Float),
-        (r'(?![_A-ZÀ-Ü])-?(\d+(\.\d*)|\.\d+)(?![_A-ZÀ-Ü])',
-         tokens.Number.Float),
-        (r'(?![_A-ZÀ-Ü])-?\d+(?![_A-ZÀ-Ü])', tokens.Number.Integer),
-        (r"'(''|\\\\|\\'|[^'])*'", tokens.String.Single),
-        # not a real string literal in ANSI SQL:
-        (r'"(""|\\\\|\\"|[^"])*"', tokens.String.Symbol),
-        (r'(""|".*?[^\\]")', tokens.String.Symbol),
-        # sqlite names can be escaped with [square brackets]. left bracket
-        # cannot be preceded by word character or a right bracket --
-        # otherwise it's probably an array index
-        (r'(?<![\w\])])(\[[^\]\[]+\])', tokens.Name),
-        (r'((LEFT\s+|RIGHT\s+|FULL\s+)?(INNER\s+|OUTER\s+|STRAIGHT\s+)?'
-         r'|(CROSS\s+|NATURAL\s+)?)?JOIN\b', tokens.Keyword),
-        (r'END(\s+IF|\s+LOOP|\s+WHILE)?\b', tokens.Keyword),
-        (r'NOT\s+NULL\b', tokens.Keyword),
-        (r'NULLS\s+(FIRST|LAST)\b', tokens.Keyword),
-        (r'UNION\s+ALL\b', tokens.Keyword),
-        (r'CREATE(\s+OR\s+REPLACE)?\b', tokens.Keyword.DDL),
-        (r'DOUBLE\s+PRECISION\b', tokens.Name.Builtin),
-        (r'GROUP\s+BY\b', tokens.Keyword),
-        (r'ORDER\s+BY\b', tokens.Keyword),
-        (r'HANDLER\s+FOR\b', tokens.Keyword),
-        (r'(LATERAL\s+VIEW\s+)'
-         r'(EXPLODE|INLINE|PARSE_URL_TUPLE|POSEXPLODE|STACK)\b',
-         tokens.Keyword),
-        (r"(AT|WITH')\s+TIME\s+ZONE\s+'[^']+'", tokens.Keyword.TZCast),
-        (r'(NOT\s+)?(LIKE|ILIKE|RLIKE)\b', tokens.Operator.Comparison),
-        (r'(NOT\s+)?(REGEXP)\b', tokens.Operator.Comparison),
-        # Check for keywords, also returns tokens.Name if regex matches
-        # but the match isn't a keyword.
-        (r'[0-9_\w][_$#\w]*', is_keyword),
-        (r'[;:()\[\],\.]', tokens.Punctuation),
-        (r'[<>=~!]+', tokens.Operator.Comparison),
-        (r'[+/@#%^&|^-]+', tokens.Operator),
-    ]}
-
-FLAGS = re.IGNORECASE | re.UNICODE
-SQL_REGEX = [(re.compile(rx, FLAGS).match, tt) for rx, tt in SQL_REGEX['root']]
+# object() only supports "is" and is useful as a marker
+# use this marker to specify that the given regex in SQL_REGEX
+# shall be processed further through a lookup in the KEYWORDS dictionaries
+PROCESS_AS_KEYWORD = object()
+
+
+SQL_REGEX = [
+    (r'(--|# )\+.*?(\r\n|\r|\n|$)', tokens.Comment.Single.Hint),
+    (r'/\*\+[\s\S]*?\*/', tokens.Comment.Multiline.Hint),
+
+    (r'(--|# ).*?(\r\n|\r|\n|$)', tokens.Comment.Single),
+    (r'/\*[\s\S]*?\*/', tokens.Comment.Multiline),
+
+    (r'(\r\n|\r|\n)', tokens.Newline),
+    (r'\s+?', tokens.Whitespace),
+
+    (r':=', tokens.Assignment),
+    (r'::', tokens.Punctuation),
+
+    (r'\*', tokens.Wildcard),
+
+    (r"`(``|[^`])*`", tokens.Name),
+    (r"´(´´|[^´])*´", tokens.Name),
+    (r'((?<!\S)\$(?:[_A-ZÀ-Ü]\w*)?\$)[\s\S]*?\1', tokens.Literal),
+
+    (r'\?', tokens.Name.Placeholder),
+    (r'%(\(\w+\))?s', tokens.Name.Placeholder),
+    (r'(?<!\w)[$:?]\w+', tokens.Name.Placeholder),
+
+    (r'\\\w+', tokens.Command),
+
+    # FIXME(andi): VALUES shouldn't be listed here
+    # see https://github.com/andialbrecht/sqlparse/pull/64
+    # AS and IN are special, it may be followed by a parenthesis, but
+    # are never functions, see issue183 and issue507
+    (r'(CASE|IN|VALUES|USING|FROM|AS)\b', tokens.Keyword),
+
+    (r'(@|##|#)[A-ZÀ-Ü]\w+', tokens.Name),
+
+    # see issue #39
+    # Spaces around period `schema . name` are valid identifier
+    # TODO: Spaces before period not implemented
+    (r'[A-ZÀ-Ü]\w*(?=\s*\.)', tokens.Name),  # 'Name'.
+    # FIXME(atronah): never match,
+    # because `re.match` doesn't work with look-behind regexp feature
+    (r'(?<=\.)[A-ZÀ-Ü]\w*', tokens.Name),  # .'Name'
+    (r'[A-ZÀ-Ü]\w*(?=\()', tokens.Name),  # side effect: change kw to func
+    (r'-?0x[\dA-F]+', tokens.Number.Hexadecimal),
+    (r'-?\d+(\.\d+)?E-?\d+', tokens.Number.Float),
+    (r'(?![_A-ZÀ-Ü])-?(\d+(\.\d*)|\.\d+)(?![_A-ZÀ-Ü])',
+     tokens.Number.Float),
+    (r'(?![_A-ZÀ-Ü])-?\d+(?![_A-ZÀ-Ü])', tokens.Number.Integer),
+    (r"'(''|\\'|[^'])*'", tokens.String.Single),
+    # not a real string literal in ANSI SQL:
+    (r'"(""|\\"|[^"])*"', tokens.String.Symbol),
+    (r'(""|".*?[^\\]")', tokens.String.Symbol),
+    # sqlite names can be escaped with [square brackets]. left bracket
+    # cannot be preceded by word character or a right bracket --
+    # otherwise it's probably an array index
+    (r'(?<![\w\])])(\[[^\]\[]+\])', tokens.Name),
+    (r'((LEFT\s+|RIGHT\s+|FULL\s+)?(INNER\s+|OUTER\s+|STRAIGHT\s+)?'
+     r'|(CROSS\s+|NATURAL\s+)?)?JOIN\b', tokens.Keyword),
+    (r'END(\s+IF|\s+LOOP|\s+WHILE)?\b', tokens.Keyword),
+    (r'NOT\s+NULL\b', tokens.Keyword),
+    (r'NULLS\s+(FIRST|LAST)\b', tokens.Keyword),
+    (r'UNION\s+ALL\b', tokens.Keyword),
+    (r'CREATE(\s+OR\s+REPLACE)?\b', tokens.Keyword.DDL),
+    (r'DOUBLE\s+PRECISION\b', tokens.Name.Builtin),
+    (r'GROUP\s+BY\b', tokens.Keyword),
+    (r'ORDER\s+BY\b', tokens.Keyword),
+    (r'HANDLER\s+FOR\b', tokens.Keyword),
+    (r'(LATERAL\s+VIEW\s+)'
+     r'(EXPLODE|INLINE|PARSE_URL_TUPLE|POSEXPLODE|STACK)\b',
+     tokens.Keyword),
+    (r"(AT|WITH')\s+TIME\s+ZONE\s+'[^']+'", tokens.Keyword.TZCast),
+    (r'(NOT\s+)?(LIKE|ILIKE|RLIKE)\b', tokens.Operator.Comparison),
+    (r'(NOT\s+)?(REGEXP)\b', tokens.Operator.Comparison),
+    # Check for keywords, also returns tokens.Name if regex matches
+    # but the match isn't a keyword.
+    (r'\w[$#\w]*', PROCESS_AS_KEYWORD),
+    (r'[;:()\[\],\.]', tokens.Punctuation),
+    (r'[<>=~!]+', tokens.Operator.Comparison),
+    (r'[+/@#%^&|^-]+', tokens.Operator),
+]
 
 KEYWORDS = {
     'ABORT': tokens.Keyword,
     'ABS': tokens.Keyword,
     'ABSOLUTE': tokens.Keyword,
     'ACCESS': tokens.Keyword,
     'ADA': tokens.Keyword,
```

### Comparing `sqlparse-0.4.3/sqlparse/sql.py` & `sqlparse-0.4.4/sqlparse/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,35 +409,36 @@
         The returned value is a string holding an upper-cased reprint of
         the first DML or DDL keyword. If the first token in this group
         isn't a DML or DDL keyword "UNKNOWN" is returned.
 
         Whitespaces and comments at the beginning of the statement
         are ignored.
         """
-        first_token = self.token_first(skip_cm=True)
-        if first_token is None:
+        token = self.token_first(skip_cm=True)
+        if token is None:
             # An "empty" statement that either has not tokens at all
             # or only whitespace tokens.
             return 'UNKNOWN'
 
-        elif first_token.ttype in (T.Keyword.DML, T.Keyword.DDL):
-            return first_token.normalized
+        elif token.ttype in (T.Keyword.DML, T.Keyword.DDL):
+            return token.normalized
 
-        elif first_token.ttype == T.Keyword.CTE:
+        elif token.ttype == T.Keyword.CTE:
             # The WITH keyword should be followed by either an Identifier or
             # an IdentifierList containing the CTE definitions;  the actual
             # DML keyword (e.g. SELECT, INSERT) will follow next.
-            fidx = self.token_index(first_token)
-            tidx, token = self.token_next(fidx, skip_ws=True)
-            if isinstance(token, (Identifier, IdentifierList)):
-                _, dml_keyword = self.token_next(tidx, skip_ws=True)
-
-                if dml_keyword is not None \
-                        and dml_keyword.ttype == T.Keyword.DML:
-                    return dml_keyword.normalized
+            tidx = self.token_index(token)
+            while tidx is not None:
+                tidx, token = self.token_next(tidx, skip_ws=True)
+                if isinstance(token, (Identifier, IdentifierList)):
+                    tidx, token = self.token_next(tidx, skip_ws=True)
+
+                    if token is not None \
+                            and token.ttype == T.Keyword.DML:
+                        return token.normalized
 
         # Hmm, probably invalid syntax, so return unknown.
         return 'UNKNOWN'
 
 
 class Identifier(NameAliasMixin, TokenList):
     """Represents an identifier.
```

### Comparing `sqlparse-0.4.3/sqlparse/tokens.py` & `sqlparse-0.4.4/sqlparse/tokens.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/sqlparse/utils.py` & `sqlparse-0.4.4/sqlparse/utils.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/tests/conftest.py` & `sqlparse-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/tests/files/function_psql.sql` & `sqlparse-0.4.4/tests/files/function_psql.sql`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/tests/files/huge_select.sql` & `sqlparse-0.4.4/tests/files/huge_select.sql`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/tests/test_cli.py` & `sqlparse-0.4.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/tests/test_format.py` & `sqlparse-0.4.4/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `sqlparse-0.4.3/tests/test_grouping.py` & `sqlparse-0.4.4/tests/test_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,28 +372,18 @@
     assert len(list(p.tokens[0].get_parameters())) == 2
 
 
 def test_grouping_function_not_in():
     # issue183
     p = sqlparse.parse('in(1, 2)')[0]
     assert len(p.tokens) == 2
-    assert p.tokens[0].ttype == T.Comparison
+    assert p.tokens[0].ttype == T.Keyword
     assert isinstance(p.tokens[1], sql.Parenthesis)
 
 
-def test_in_comparison():
-    # issue566
-    p = sqlparse.parse('a in (1, 2)')[0]
-    assert len(p.tokens) == 1
-    assert isinstance(p.tokens[0], sql.Comparison)
-    assert len(p.tokens[0].tokens) == 5
-    assert p.tokens[0].left.value == 'a'
-    assert p.tokens[0].right.value == '(1, 2)'
-
-
 def test_grouping_varchar():
     p = sqlparse.parse('"text" Varchar(50) NOT NULL')[0]
     assert isinstance(p.tokens[2], sql.Function)
 
 
 def test_statement_get_type():
     def f(sql):
```

### Comparing `sqlparse-0.4.3/tests/test_parse.py` & `sqlparse-0.4.4/tests/test_parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests sqlparse.parse()."""
 from io import StringIO
 
 import pytest
 
 import sqlparse
-from sqlparse import sql, tokens as T
+from sqlparse import sql, tokens as T, keywords
+from sqlparse.lexer import Lexer
 
 
 def test_parse_tokenize():
     s = 'select * from foo;'
     stmts = sqlparse.parse(s)
     assert len(stmts) == 1
     assert str(stmts[0]) == s
@@ -485,7 +486,83 @@
                                                     T.Newline,
                                                     T.Whitespace,
                                                     T.Number.Integer,
                                                     T.Whitespace,
                                                     T.Newline,
                                                     T.Newline,
                                                     T.Punctuation]
+
+
+def test_configurable_keywords():
+    sql = """select * from foo BACON SPAM EGGS;"""
+    tokens = sqlparse.parse(sql)[0]
+
+    assert list(
+        (t.ttype, t.value)
+        for t in tokens
+        if t.ttype not in sqlparse.tokens.Whitespace
+    ) == [
+        (sqlparse.tokens.Keyword.DML, "select"),
+        (sqlparse.tokens.Wildcard, "*"),
+        (sqlparse.tokens.Keyword, "from"),
+        (None, "foo BACON"),
+        (None, "SPAM EGGS"),
+        (sqlparse.tokens.Punctuation, ";"),
+    ]
+
+    Lexer.get_default_instance().add_keywords(
+        {
+            "BACON": sqlparse.tokens.Name.Builtin,
+            "SPAM": sqlparse.tokens.Keyword,
+            "EGGS": sqlparse.tokens.Keyword,
+        }
+    )
+
+    tokens = sqlparse.parse(sql)[0]
+
+    # reset the syntax for later tests.
+    Lexer.get_default_instance().default_initialization()
+
+    assert list(
+        (t.ttype, t.value)
+        for t in tokens
+        if t.ttype not in sqlparse.tokens.Whitespace
+    ) == [
+        (sqlparse.tokens.Keyword.DML, "select"),
+        (sqlparse.tokens.Wildcard, "*"),
+        (sqlparse.tokens.Keyword, "from"),
+        (None, "foo"),
+        (sqlparse.tokens.Name.Builtin, "BACON"),
+        (sqlparse.tokens.Keyword, "SPAM"),
+        (sqlparse.tokens.Keyword, "EGGS"),
+        (sqlparse.tokens.Punctuation, ";"),
+    ]
+
+
+def test_configurable_regex():
+    lex = Lexer.get_default_instance()
+    lex.clear()
+
+    my_regex = (r"ZORDER\s+BY\b", sqlparse.tokens.Keyword)
+
+    lex.set_SQL_REGEX(
+        keywords.SQL_REGEX[:38]
+        + [my_regex]
+        + keywords.SQL_REGEX[38:]
+    )
+    lex.add_keywords(keywords.KEYWORDS_COMMON)
+    lex.add_keywords(keywords.KEYWORDS_ORACLE)
+    lex.add_keywords(keywords.KEYWORDS_PLPGSQL)
+    lex.add_keywords(keywords.KEYWORDS_HQL)
+    lex.add_keywords(keywords.KEYWORDS_MSACCESS)
+    lex.add_keywords(keywords.KEYWORDS)
+
+    tokens = sqlparse.parse("select * from foo zorder by bar;")[0]
+
+    # reset the syntax for later tests.
+    Lexer.get_default_instance().default_initialization()
+
+    assert list(
+        (t.ttype, t.value)
+        for t in tokens
+        if t.ttype not in sqlparse.tokens.Whitespace
+    )[4] == (sqlparse.tokens.Keyword, "zorder by")
```

### Comparing `sqlparse-0.4.3/tests/test_regressions.py` & `sqlparse-0.4.4/tests/test_regressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -869,8 +869,23 @@
 00003640: 603b 2067 7261 6e74 2062 6172 2074 6f20  `; grant bar to 
 00003650: 7573 6572 3140 606d 7968 6f73 7460 3b27  user1@`myhost`;'
 00003660: 290a 2020 2020 6173 7365 7274 206c 656e  ).    assert len
 00003670: 2873 706c 6974 7465 6429 203d 3d20 320a  (splitted) == 2.
 00003680: 2020 2020 6173 7365 7274 2073 706c 6974      assert split
 00003690: 7465 645b 2d31 5d20 3d3d 2027 6772 616e  ted[-1] == 'gran
 000036a0: 7420 6261 7220 746f 2075 7365 7231 4060  t bar to user1@`
-000036b0: 6d79 686f 7374 603b 270a                 myhost`;'.
+000036b0: 6d79 686f 7374 603b 270a 0a0a 6465 6620  myhost`;'...def 
+000036c0: 7465 7374 5f63 6f6d 6d65 6e74 5f62 6574  test_comment_bet
+000036d0: 7765 656e 5f63 7465 5f63 6c61 7573 6573  ween_cte_clauses
+000036e0: 5f69 7373 7565 3633 3228 293a 0a20 2020  _issue632():.   
+000036f0: 2070 2c20 3d20 7371 6c70 6172 7365 2e70   p, = sqlparse.p
+00003700: 6172 7365 2822 2222 0a20 2020 2020 2020  arse(""".       
+00003710: 2057 4954 4820 666f 6f20 4153 2028 292c   WITH foo AS (),
+00003720: 0a20 2020 2020 2020 2020 2020 2020 2d2d  .             --
+00003730: 2041 2063 6f6d 6d65 6e74 2062 6566 6f72   A comment befor
+00003740: 6520 6261 7a20 7375 6271 7565 7279 0a20  e baz subquery. 
+00003750: 2020 2020 2020 2020 2020 2020 6261 7a20              baz 
+00003760: 4153 2028 290a 2020 2020 2020 2020 5345  AS ().        SE
+00003770: 4c45 4354 202a 2046 524f 4d20 6261 7a3b  LECT * FROM baz;
+00003780: 2222 2229 0a20 2020 2061 7373 6572 7420  """).    assert 
+00003790: 702e 6765 745f 7479 7065 2829 203d 3d20  p.get_type() == 
+000037a0: 2253 454c 4543 5422 0a                   "SELECT".
```

### Comparing `sqlparse-0.4.3/tests/test_split.py` & `sqlparse-0.4.4/tests/test_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     stmts = sqlparse.parse(''.join([sql1, sql2]))
     assert len(stmts) == 2
     assert str(stmts[0]) == sql1
     assert str(stmts[1]) == sql2
 
 
 def test_split_backslash():
-    stmts = sqlparse.parse(r"select '\\'; select '\''; select '\\\'';")
-    assert len(stmts) == 3
+    stmts = sqlparse.parse("select '\'; select '\'';")
+    assert len(stmts) == 2
 
 
 @pytest.mark.parametrize('fn', ['function.sql',
                                 'function_psql.sql',
                                 'function_psql2.sql',
                                 'function_psql3.sql',
                                 'function_psql4.sql'])
```

### Comparing `sqlparse-0.4.3/tests/test_tokenize.py` & `sqlparse-0.4.4/tests/test_tokenize.py`

 * *Files identical despite different names*

