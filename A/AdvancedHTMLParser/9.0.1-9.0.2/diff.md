# Comparing `tmp/AdvancedHTMLParser-9.0.1.tar.gz` & `tmp/AdvancedHTMLParser-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AdvancedHTMLParser-9.0.1.tar", last modified: Wed Feb 12 22:09:49 2020, max compression
+gzip compressed data, was "AdvancedHTMLParser-9.0.2.tar", last modified: Mon Apr 17 23:41:52 2023, max compression
```

## Comparing `AdvancedHTMLParser-9.0.1.tar` & `AdvancedHTMLParser-9.0.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 T S      (197613) None     (197121)        0 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/
-drwxrwxr-x   0 T S      (197613) None     (197121)        0 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/
--rw-rw-r--   0 T S      (197613) None     (197121)       32 2019-08-07 21:48:31.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/.vimrc
--rw-rw-r--   0 T S      (197613) None     (197121)     1906 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/compat.py
--rw-rw-r--   0 T S      (197613) None     (197121)    19658 2019-11-15 02:08:59.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/constants.py
--rw-rw-r--   0 T S      (197613) None     (197121)     8214 2019-11-15 02:08:59.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/conversions.py
--rw-rw-r--   0 T S      (197613) None     (197121)     3345 2019-11-15 02:08:59.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/exceptions.py
--rw-rw-r--   0 T S      (197613) None     (197121)    15146 2019-11-15 02:08:59.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Formatter.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    51906 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Parser.py
--rw-rw-r--   0 T S      (197613) None     (197121)    26377 2019-11-15 02:08:59.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/SpecialAttributes.py
--rw-rw-r--   0 T S      (197613) None     (197121)    97200 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Tags.py
--rw-rw-r--   0 T S      (197613) None     (197121)     3052 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/utils.py
--rw-rw-r--   0 T S      (197613) None     (197121)     2594 2019-11-15 02:09:00.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Validator.py
-drwxrwxr-x   0 T S      (197613) None     (197121)        0 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/
--rw-rw-r--   0 T S      (197613) None     (197121)     1319 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/exceptions.py
--rw-rw-r--   0 T S      (197613) None     (197121)     4780 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/expression.py
--rw-rw-r--   0 T S      (197613) None     (197121)     1121 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/null.py
--rw-rw-r--   0 T S      (197613) None     (197121)     2581 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/operation.py
--rw-rw-r--   0 T S      (197613) None     (197121)     9273 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/parsing.py
--rw-rw-r--   0 T S      (197613) None     (197121)     3283 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_axes.py
--rw-rw-r--   0 T S      (197613) None     (197121)    84083 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_body.py
--rw-rw-r--   0 T S      (197613) None     (197121)     5716 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_cache.py
--rw-rw-r--   0 T S      (197613) None     (197121)     1106 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_debug.py
--rw-rw-r--   0 T S      (197613) None     (197121)    14332 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_filters.py
--rw-rw-r--   0 T S      (197613) None     (197121)      568 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/__init__.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     1740 2020-02-12 22:09:35.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/__init__.py
-drwxrwxr-x   0 T S      (197613) None     (197121)        0 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser.egg-info/
--rw-rw-r--   0 T S      (197613) None     (197121)        1 2020-02-12 22:09:48.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser.egg-info/dependency_links.txt
--rw-rw-r--   0 T S      (197613) None     (197121)    35975 2020-02-12 22:09:48.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser.egg-info/PKG-INFO
--rw-rw-r--   0 T S      (197613) None     (197121)       14 2020-02-12 22:09:48.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser.egg-info/requires.txt
--rw-rw-r--   0 T S      (197613) None     (197121)     3059 2020-02-12 22:09:48.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser.egg-info/SOURCES.txt
--rw-rw-r--   0 T S      (197613) None     (197121)       19 2020-02-12 22:09:48.000000 AdvancedHTMLParser-9.0.1/AdvancedHTMLParser.egg-info/top_level.txt
--rw-rw-r--   0 T S      (197613) None     (197121)    34679 2020-02-12 22:09:35.000000 AdvancedHTMLParser-9.0.1/ChangeLog
-drwxrwxr-x   0 T S      (197613) None     (197121)        0 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/doc/
--rw-rw-r--   0 T S      (197613) None     (197121)    30319 2020-02-12 22:08:49.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.compat.html
--rw-rw-r--   0 T S      (197613) None     (197121)     7423 2020-02-12 22:08:49.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.constants.html
--rw-rw-r--   0 T S      (197613) None     (197121)    10311 2020-02-12 22:08:49.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.conversions.html
--rw-rw-r--   0 T S      (197613) None     (197121)    26626 2020-02-12 22:08:50.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.exceptions.html
--rw-rw-r--   0 T S      (197613) None     (197121)    58963 2020-02-12 22:08:50.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Formatter.html
--rw-rw-r--   0 T S      (197613) None     (197121)   334850 2020-02-12 22:09:35.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.html
--rw-rw-r--   0 T S      (197613) None     (197121)    91284 2020-02-12 22:08:54.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Parser.html
--rw-rw-r--   0 T S      (197613) None     (197121)    42473 2020-02-12 22:08:54.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.SpecialAttributes.html
--rw-rw-r--   0 T S      (197613) None     (197121)   127058 2020-02-12 22:08:55.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Tags.html
--rw-rw-r--   0 T S      (197613) None     (197121)     5135 2020-02-12 22:08:55.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.utils.html
--rw-rw-r--   0 T S      (197613) None     (197121)    61642 2020-02-12 22:08:56.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Validator.html
--rw-rw-r--   0 T S      (197613) None     (197121)    21758 2020-02-12 22:08:58.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.exceptions.html
--rw-rw-r--   0 T S      (197613) None     (197121)     6330 2020-02-12 22:08:58.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.expression.html
--rw-rw-r--   0 T S      (197613) None     (197121)     7246 2020-02-12 22:08:59.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.html
--rw-rw-r--   0 T S      (197613) None     (197121)     4277 2020-02-12 22:08:59.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.null.html
--rw-rw-r--   0 T S      (197613) None     (197121)     6431 2020-02-12 22:08:59.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.operation.html
--rw-rw-r--   0 T S      (197613) None     (197121)     3639 2020-02-12 22:08:59.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.parsing.html
--rw-rw-r--   0 T S      (197613) None     (197121)     2692 2020-02-12 22:08:56.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._axes.html
--rw-rw-r--   0 T S      (197613) None     (197121)    29150 2020-02-12 22:08:57.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._body.html
--rw-rw-r--   0 T S      (197613) None     (197121)     8469 2020-02-12 22:08:57.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._cache.html
--rw-rw-r--   0 T S      (197613) None     (197121)     3197 2020-02-12 22:08:57.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._debug.html
--rw-rw-r--   0 T S      (197613) None     (197121)    14684 2020-02-12 22:08:58.000000 AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._filters.html
--rw-rw-r--   0 T S      (197613) None     (197121)   196090 2019-08-07 21:48:31.000000 AdvancedHTMLParser-9.0.1/doc/exceptions.html
--rw-rw-r--   0 T S      (197613) None     (197121)   334850 2020-02-12 22:09:35.000000 AdvancedHTMLParser-9.0.1/doc/index.html
--rwxrwxr-x   0 T S      (197613) None     (197121)     2369 2019-08-07 21:48:31.000000 AdvancedHTMLParser-9.0.1/example.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     5124 2019-08-07 21:48:31.000000 AdvancedHTMLParser-9.0.1/formatHTML
--rw-rw-r--   0 T S      (197613) None     (197121)     1985 2019-08-07 21:48:31.000000 AdvancedHTMLParser-9.0.1/indexed_example.py
--rw-rw-r--   0 T S      (197613) None     (197121)     7652 2019-08-07 21:48:31.000000 AdvancedHTMLParser-9.0.1/LICENSE
--rw-rw-r--   0 T S      (197613) None     (197121)      340 2020-02-12 22:04:14.000000 AdvancedHTMLParser-9.0.1/MANIFEST.in
--rw-rw-r--   0 T S      (197613) None     (197121)    35975 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/PKG-INFO
--rw-rw-r--   0 T S      (197613) None     (197121)    28595 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/README.md
--rw-rw-r--   0 T S      (197613) None     (197121)    28796 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/README.rst
--rw-rw-r--   0 T S      (197613) None     (197121)       59 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/setup.cfg
--rwxrwxr-x   0 T S      (197613) None     (197121)     5209 2020-02-12 22:09:35.000000 AdvancedHTMLParser-9.0.1/setup.py
-drwxrwxr-x   0 T S      (197613) None     (197121)        0 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/tests/
-drwxrwxr-x   0 T S      (197613) None     (197121)        0 2020-02-12 22:09:49.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/
--rwxrwxr-x   0 T S      (197613) None     (197121)    56489 2019-09-11 23:28:20.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Attributes.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     7848 2019-09-11 23:28:20.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Blocks.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    11443 2019-09-11 23:28:20.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Building.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     3300 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Children.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     7615 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Compare.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    14046 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Conversions.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     4564 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_CustomFilter.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     2548 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_DOMTokenList.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     4973 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Formatting.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    10355 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_General.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    13387 2019-09-11 23:28:21.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Insertions.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     2141 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_InvalidHtml.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     2524 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_ParseMethods.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     2122 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_ParserGetters.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    11744 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Pickle.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     1845 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_RefTag.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    15591 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Style.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    17318 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_TagClass.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     4746 2019-09-11 23:28:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_untaggedText.py
--rwxrwxr-x   0 T S      (197613) None     (197121)     4937 2019-09-11 23:28:23.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_ValidateInvalidHtml.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    26397 2020-01-16 21:41:22.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_XPath.py
--rw-rw-r--   0 T S      (197613) None     (197121)        0 2019-09-11 23:28:20.000000 AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/__init__.py
--rwxrwxr-x   0 T S      (197613) None     (197121)    14990 2019-08-07 21:53:11.000000 AdvancedHTMLParser-9.0.1/tests/runTests.py
+drwxr-xr-x   0 owner    (197609) None     (197121)        0 2023-04-17 23:41:52.817176 AdvancedHTMLParser-9.0.2/
+drwxr-xr-x   0 owner    (197609) None     (197121)        0 2023-04-17 23:41:52.367277 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/
+-rw-r--r--   0 owner    (197609) None     (197121)       32 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/.vimrc
+-rw-r--r--   0 owner    (197609) None     (197121)    15146 2023-04-17 23:27:00.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Formatter.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    51906 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Parser.py
+-rw-r--r--   0 owner    (197609) None     (197121)    26377 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/SpecialAttributes.py
+-rw-r--r--   0 owner    (197609) None     (197121)    97200 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Tags.py
+-rw-r--r--   0 owner    (197609) None     (197121)     2594 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Validator.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     1746 2023-04-17 23:24:43.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/__init__.py
+-rw-r--r--   0 owner    (197609) None     (197121)     1906 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/compat.py
+-rw-r--r--   0 owner    (197609) None     (197121)    19658 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/constants.py
+-rw-r--r--   0 owner    (197609) None     (197121)     8214 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/conversions.py
+-rw-r--r--   0 owner    (197609) None     (197121)     3345 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/exceptions.py
+-rw-r--r--   0 owner    (197609) None     (197121)     3052 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/utils.py
+drwxr-xr-x   0 owner    (197609) None     (197121)        0 2023-04-17 23:41:52.469219 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/
+-rw-r--r--   0 owner    (197609) None     (197121)      568 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/__init__.py
+-rw-r--r--   0 owner    (197609) None     (197121)     3283 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_axes.py
+-rw-r--r--   0 owner    (197609) None     (197121)    84058 2023-04-17 23:13:59.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_body.py
+-rw-r--r--   0 owner    (197609) None     (197121)     5716 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_cache.py
+-rw-r--r--   0 owner    (197609) None     (197121)     1106 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_debug.py
+-rw-r--r--   0 owner    (197609) None     (197121)    14332 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_filters.py
+-rw-r--r--   0 owner    (197609) None     (197121)     1319 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/exceptions.py
+-rw-r--r--   0 owner    (197609) None     (197121)     4780 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/expression.py
+-rw-r--r--   0 owner    (197609) None     (197121)     1121 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/null.py
+-rw-r--r--   0 owner    (197609) None     (197121)     2581 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/operation.py
+-rw-r--r--   0 owner    (197609) None     (197121)     9273 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/parsing.py
+drwxr-xr-x   0 owner    (197609) None     (197121)        0 2023-04-17 23:41:52.407254 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser.egg-info/
+-rw-r--r--   0 owner    (197609) None     (197121)    30420 2023-04-17 23:41:51.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser.egg-info/PKG-INFO
+-rw-r--r--   0 owner    (197609) None     (197121)     3059 2023-04-17 23:41:51.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser.egg-info/SOURCES.txt
+-rw-r--r--   0 owner    (197609) None     (197121)        1 2023-04-17 23:41:51.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser.egg-info/dependency_links.txt
+-rw-r--r--   0 owner    (197609) None     (197121)       14 2023-04-17 23:41:51.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser.egg-info/requires.txt
+-rw-r--r--   0 owner    (197609) None     (197121)       19 2023-04-17 23:41:51.000000 AdvancedHTMLParser-9.0.2/AdvancedHTMLParser.egg-info/top_level.txt
+-rw-r--r--   0 owner    (197609) None     (197121)    34866 2023-04-17 23:41:15.000000 AdvancedHTMLParser-9.0.2/ChangeLog
+-rw-r--r--   0 owner    (197609) None     (197121)     7652 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/LICENSE
+-rw-r--r--   0 owner    (197609) None     (197121)      340 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/MANIFEST.in
+-rw-r--r--   0 owner    (197609) None     (197121)    30420 2023-04-17 23:41:52.818175 AdvancedHTMLParser-9.0.2/PKG-INFO
+-rw-r--r--   0 owner    (197609) None     (197121)    28595 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/README.md
+-rw-r--r--   0 owner    (197609) None     (197121)    28796 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/README.rst
+drwxr-xr-x   0 owner    (197609) None     (197121)        0 2023-04-17 23:41:52.640144 AdvancedHTMLParser-9.0.2/doc/
+-rw-r--r--   0 owner    (197609) None     (197121)    58963 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Formatter.html
+-rw-r--r--   0 owner    (197609) None     (197121)    91284 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Parser.html
+-rw-r--r--   0 owner    (197609) None     (197121)    42473 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.SpecialAttributes.html
+-rw-r--r--   0 owner    (197609) None     (197121)   127058 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Tags.html
+-rw-r--r--   0 owner    (197609) None     (197121)    61642 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Validator.html
+-rw-r--r--   0 owner    (197609) None     (197121)    30319 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.compat.html
+-rw-r--r--   0 owner    (197609) None     (197121)     7423 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.constants.html
+-rw-r--r--   0 owner    (197609) None     (197121)    10311 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.conversions.html
+-rw-r--r--   0 owner    (197609) None     (197121)    26626 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.exceptions.html
+-rw-r--r--   0 owner    (197609) None     (197121)   334850 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.html
+-rw-r--r--   0 owner    (197609) None     (197121)     5135 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.utils.html
+-rw-r--r--   0 owner    (197609) None     (197121)     2692 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._axes.html
+-rw-r--r--   0 owner    (197609) None     (197121)    29150 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._body.html
+-rw-r--r--   0 owner    (197609) None     (197121)     8469 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._cache.html
+-rw-r--r--   0 owner    (197609) None     (197121)     3197 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._debug.html
+-rw-r--r--   0 owner    (197609) None     (197121)    14684 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._filters.html
+-rw-r--r--   0 owner    (197609) None     (197121)    21758 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.exceptions.html
+-rw-r--r--   0 owner    (197609) None     (197121)     6330 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.expression.html
+-rw-r--r--   0 owner    (197609) None     (197121)     7246 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.html
+-rw-r--r--   0 owner    (197609) None     (197121)     4277 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.null.html
+-rw-r--r--   0 owner    (197609) None     (197121)     6431 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.operation.html
+-rw-r--r--   0 owner    (197609) None     (197121)     3639 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.parsing.html
+-rw-r--r--   0 owner    (197609) None     (197121)   196090 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/doc/exceptions.html
+-rw-r--r--   0 owner    (197609) None     (197121)   334850 2023-04-17 23:38:59.000000 AdvancedHTMLParser-9.0.2/doc/index.html
+-rwxr-xr-x   0 owner    (197609) None     (197121)     2369 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/example.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     5124 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/formatHTML
+-rw-r--r--   0 owner    (197609) None     (197121)     1985 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/indexed_example.py
+-rw-r--r--   0 owner    (197609) None     (197121)       59 2023-04-17 23:41:52.820174 AdvancedHTMLParser-9.0.2/setup.cfg
+-rwxr-xr-x   0 owner    (197609) None     (197121)     5416 2023-04-17 23:24:16.000000 AdvancedHTMLParser-9.0.2/setup.py
+drwxr-xr-x   0 owner    (197609) None     (197121)        0 2023-04-17 23:41:52.644142 AdvancedHTMLParser-9.0.2/tests/
+drwxr-xr-x   0 owner    (197609) None     (197121)        0 2023-04-17 23:41:52.814177 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/
+-rw-r--r--   0 owner    (197609) None     (197121)        0 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/__init__.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    56489 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Attributes.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     7848 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Blocks.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    11443 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Building.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     3300 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Children.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     7615 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Compare.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    14046 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Conversions.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     4564 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_CustomFilter.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     2548 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_DOMTokenList.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     4973 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Formatting.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    10515 2023-04-17 23:35:16.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_General.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    13387 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Insertions.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     2141 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_InvalidHtml.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     2524 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_ParseMethods.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     2122 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_ParserGetters.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    11744 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Pickle.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     1845 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_RefTag.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    15591 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Style.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    17318 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_TagClass.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     4937 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_ValidateInvalidHtml.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    26459 2023-04-17 23:30:01.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_XPath.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)     4746 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_untaggedText.py
+-rwxr-xr-x   0 owner    (197609) None     (197121)    14990 2023-04-17 22:40:24.000000 AdvancedHTMLParser-9.0.2/tests/runTests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/compat.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/compat.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/constants.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/constants.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/conversions.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/conversions.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/exceptions.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/exceptions.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Formatter.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         if self.root is None:
             self.root = newTag
         elif len(inTag) > 0:
             inTag[-1].appendChild(newTag)
         else:
             raise MultipleRootNodeException()
 
-        if self.inPreformatted is 0:
+        if self.inPreformatted == 0:
             newTag._indent = self._getIndent()
 
         if tagName in PREFORMATTED_TAGS:
             self.inPreformatted += 1
 
         if isSelfClosing is False:
             inTag.append(newTag)
@@ -402,15 +402,15 @@
     if self.root is None:
         self.root = newTag
     elif len(inTag) > 0:
         inTag[-1].appendChild(newTag)
     else:
         raise MultipleRootNodeException()
 
-    if self.inPreformatted is 0:
+    if self.inPreformatted == 0:
         newTag._indent = self._getIndent()
 
     if tagName in PREFORMATTED_TAGS:
         self.inPreformatted += 1
 
     if isSelfClosing is False:
         inTag.append(newTag)
```

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Parser.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Parser.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/SpecialAttributes.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/SpecialAttributes.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Tags.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Tags.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/utils.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/utils.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/Validator.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/Validator.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/exceptions.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/expression.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/expression.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/null.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/null.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/operation.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/operation.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/parsing.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/parsing.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_axes.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_axes.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_body.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-    Copyright (c) 2019 Timothy Savannah under terms of LGPLv3. All Rights Reserved.
+    Copyright (c) 2019, 2023 Timothy Savannah under terms of LGPLv3. All Rights Reserved.
 
     See LICENSE (https://gnu.org/licenses/lgpl-3.0.txt) for more information.
 
     See: https://github.com/kata198/AdvancedHTMLParser for full information
 
 
     ==INTERNAL==
@@ -124,16 +124,14 @@
     def __iter__(self):
         '''
             __iter__ - Iterate over this object
         '''
         for bodyElement in self.bodyElements:
             yield bodyElement
 
-        raise StopIteration()
-
 
     def evaluateLevelForTag(self, currentTag):
         '''
             evaluateLevelForTag - Shorthand version of "evaluateLevelForTags" but for one tag
```

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_cache.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_cache.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_debug.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_debug.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/_filters.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/_filters.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/xpath/__init__.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/xpath/__init__.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser/__init__.py` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-    Copyright (c) 2015, 2016, 2017, 2018, 2019 Tim Savannah All Rights Rserved under LGPLv3. All Rights Reserved.
+    Copyright (c) 2015, 2016, 2017, 2018, 2019, 2023 Tim Savannah All Rights Rserved under LGPLv3. All Rights Reserved.
 
 
     See LICENSE (https://gnu.org/licenses/lgpl-3.0.txt) for more information.
 
     See: https://github.com/kata198/AdvancedHTMLParser for full information
 '''
 
@@ -14,17 +14,17 @@
 from .Parser import AdvancedHTMLParser, IndexedAdvancedHTMLParser
 from .Tags import AdvancedTag, TagCollection, toggleAttributesDOM, isTextNode, isTagNode
 from .Formatter import AdvancedHTMLFormatter, AdvancedHTMLMiniFormatter, AdvancedHTMLSlimTagFormatter, AdvancedHTMLSlimTagMiniFormatter
 from .Validator import ValidatingAdvancedHTMLParser
 from .exceptions import InvalidCloseException, MissedCloseException, HTMLValidationException, MultipleRootNodeException
 from .SpecialAttributes import StyleAttribute
 
-__version__ = '9.0.1'
-__version_tuple__ = ('9', '0', '1')
-__int_version_tuple__ = (9, 0, 1)
+__version__ = '9.0.2'
+__version_tuple__ = ('9', '0', '2')
+__int_version_tuple__ = (9, 0, 2)
 
 __all__ = ( 'AdvancedHTMLParser', 'IndexedAdvancedHTMLParser', 'AdvancedHTMLFormatter', 'AdvancedTag', 'TagCollection',
     'ValidatingAdvancedHTMLParser', 'MissedCloseException', 'InvalidCloseException', 'HTMLValidationException', 'MultipleRootNodeException',
     'StyleAttribute', 'toggleAttributesDOM', 'isTextNode', 'isTagNode',
     'AdvancedHTMLMiniFormatter', 'AdvancedHTMLSlimTagFormatter', 'AdvancedHTMLSlimTagMiniFormatter' )
 
 #vim: set ts=4 sw=4 expandtab
```

### Comparing `AdvancedHTMLParser-9.0.1/AdvancedHTMLParser.egg-info/SOURCES.txt` & `AdvancedHTMLParser-9.0.2/AdvancedHTMLParser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/ChangeLog` & `AdvancedHTMLParser-9.0.2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+* 9.0.2 - Apr 17 2023
+
+- Fixed a compatibility issue with python 3.9 in xpath
+- Fixed all warnings with python > 3.6
+- Fixed some tests which displayed failure when there was no problem
+
 * 9.0.1 - Feb 12 2020
 
 - Fix installation issue under some conditions
 
 * 9.0.0 - Jan 16 2020
 * (8.9.9 - beta release 1)
```

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.compat.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.compat.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.constants.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.constants.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.conversions.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.conversions.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.exceptions.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.exceptions.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Formatter.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Formatter.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Parser.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Parser.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.SpecialAttributes.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.SpecialAttributes.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Tags.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Tags.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.utils.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.utils.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.Validator.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.Validator.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.exceptions.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.exceptions.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.expression.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.expression.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.null.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.null.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.operation.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.operation.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath.parsing.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath.parsing.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._axes.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._axes.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._body.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._body.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._cache.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._cache.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._debug.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._debug.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/AdvancedHTMLParser.xpath._filters.html` & `AdvancedHTMLParser-9.0.2/doc/AdvancedHTMLParser.xpath._filters.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/exceptions.html` & `AdvancedHTMLParser-9.0.2/doc/exceptions.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/doc/index.html` & `AdvancedHTMLParser-9.0.2/doc/index.html`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/example.py` & `AdvancedHTMLParser-9.0.2/example.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/formatHTML` & `AdvancedHTMLParser-9.0.2/formatHTML`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/indexed_example.py` & `AdvancedHTMLParser-9.0.2/indexed_example.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/LICENSE` & `AdvancedHTMLParser-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/README.md` & `AdvancedHTMLParser-9.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/README.rst` & `AdvancedHTMLParser-9.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/setup.py` & `AdvancedHTMLParser-9.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 '''
-    Copyright (c) 2015, 2016, 2017, 2018, 2019 Timothy Savannah under terms of LGPLv3. All Rights Reserved.
+    Copyright (c) 2015, 2016, 2017, 2018, 2019, 2023 Timothy Savannah under terms of LGPLv3. All Rights Reserved.
 
 
     You should have received a copy of this with this distribution as "LICENSE"
       If you did not, the current license can be found at: https://github.com/kata198/AdvancedHTMLParser/blob/master/LICENSE
 
 
   NOTE: - If you pass --no-deps, you can get a standalone install of AdvancedHTMLParser
@@ -38,15 +38,15 @@
         with open('README.rst', 'rt') as f:
             long_description = f.read()
     except Exception as e:
         sys.stderr.write('Exception when reading long description: %s\n' %(str(e),))
         long_description = summary
 
     setup(name='AdvancedHTMLParser',
-            version='9.0.1',
+            version='9.0.2',
             packages=['AdvancedHTMLParser', 'AdvancedHTMLParser.xpath'],
             scripts=['formatHTML'],
             author='Tim Savannah',
             author_email='kata198@gmail.com',
             maintainer='Tim Savannah',
             requires=requires,
             install_requires=requires,
@@ -63,14 +63,17 @@
                           'Programming Language :: Python :: 2',
                           'Programming Language :: Python :: 2.7',
                           'Programming Language :: Python :: 3',
                           'Programming Language :: Python :: 3.3',
                           'Programming Language :: Python :: 3.4',
                           'Programming Language :: Python :: 3.5',
                           'Programming Language :: Python :: 3.6',
+                          'Programming Language :: Python :: 3.7',
+                          'Programming Language :: Python :: 3.8',
+                          'Programming Language :: Python :: 3.9',
                           'Topic :: Internet :: WWW/HTTP',
                           'Topic :: Text Processing :: Markup :: HTML',
                           'Topic :: Software Development :: Libraries :: Python Modules',
             ]
     )
```

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Attributes.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Attributes.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Blocks.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Blocks.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Building.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Building.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Children.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Children.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Compare.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Compare.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Conversions.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Conversions.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_CustomFilter.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_CustomFilter.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_DOMTokenList.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_DOMTokenList.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Formatting.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Formatting.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_General.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_General.py`

 * *Files 5% similar despite different names*

```diff
@@ -249,17 +249,23 @@
 
         assert formEms[0].id == 'form1' , 'Expected to find form1 first'
         assert formEms[1].id == 'form2' , 'Expected to find form2 second'
 
         assert issubclass(formEms.__class__, AdvancedHTMLParser.TagCollection) , 'Expected result of document.forms to be a TagCollection'
 
         try:
-            assert formEms.filter(id='form1').all() == [formEms[0]] , 'Expected filtering to work on TagCollection returned from document.forms'
+            import QueryableList
+            hasQueryableList = True
         except ImportError:
-            sys.stderr.write('WARNING: .filter is disabled via ImportError. QueryableList not installed?\n\n')
+            hasQueryableList = False
+            sys.stderr.write('WARNING: .filter is disabled via ImportError. Skipping related test. QueryableList not installed?\n\n')
+
+        if hasQueryableList:
+            assert formEms.filter(id='form1').all() == [formEms[0]] , 'Expected filtering to work on TagCollection returned from document.forms'
+
 
     def test_doctype(self):
         '''
             test_doctype - Test doctype stuff
         '''
 
         parser = AdvancedHTMLParser.AdvancedHTMLParser()
```

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Insertions.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Insertions.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_InvalidHtml.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_InvalidHtml.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_ParseMethods.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_ParseMethods.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_ParserGetters.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_ParserGetters.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Pickle.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Pickle.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_RefTag.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_RefTag.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_Style.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_Style.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_TagClass.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_TagClass.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_untaggedText.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_untaggedText.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_ValidateInvalidHtml.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_ValidateInvalidHtml.py`

 * *Files identical despite different names*

### Comparing `AdvancedHTMLParser-9.0.1/tests/AdvancedHTMLParserTests/test_XPath.py` & `AdvancedHTMLParser-9.0.2/tests/AdvancedHTMLParserTests/test_XPath.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,15 +488,16 @@
         XPathExpressionCache.getCachedExpression = oldGetCachedExpression
 
         timeWithoutCache = round(timeWithoutCache, 7)
         timeWithCache = round(timeWithCache, 7)
         print ( "No Cache: %.7f" %( timeWithoutCache, ))
         print ( "W/ Cache: %.7f" %( timeWithCache, ))
 
-        assert timeWithCache < timeWithoutCache , 'Expected compiling XPath strings to be faster when caching the compiled result, but was not.\nTime with cache   : %.7f\nTime without cache: %.7f' %( timeWithCache, timeWithoutCache)
+        # Don't fail the test for this, can be other things
+        # assert timeWithCache < timeWithoutCache , 'Expected compiling XPath strings to be faster when caching the compiled result, but was not.\nTime with cache   : %.7f\nTime without cache: %.7f' %( timeWithCache, timeWithoutCache)
 
 
     def test_xpathCatchMissingCloseParen(self):
         '''
             test_xpathCatchMissingCloseParen - Test that we properly catch missing close parenthesis
         '''
         try:
```

### Comparing `AdvancedHTMLParser-9.0.1/tests/runTests.py` & `AdvancedHTMLParser-9.0.2/tests/runTests.py`

 * *Files identical despite different names*

