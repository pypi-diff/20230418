# Comparing `tmp/pydantic-translations-0.1.0.tar.gz` & `tmp/pydantic-translations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-translations-0.1.0.tar", last modified: Mon Apr  3 10:52:05 2023, max compression
+gzip compressed data, was "pydantic-translations-0.2.0.tar", last modified: Tue Apr 18 09:37:21 2023, max compression
```

## Comparing `pydantic-translations-0.1.0.tar` & `pydantic-translations-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      128 2023-03-31 09:09:46.066607 pydantic-translations-0.1.0/.gitignore
--rw-r--r--   0        0        0      325 2023-03-31 07:34:53.564133 pydantic-translations-0.1.0/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2023-03-31 07:35:20.203909 pydantic-translations-0.1.0/LICENSE
--rw-r--r--   0        0        0     2608 2023-04-03 07:25:48.587993 pydantic-translations-0.1.0/README.md
--rw-r--r--   0        0        0     3967 2023-03-31 10:15:59.804031 pydantic-translations-0.1.0/Taskfile.yml
--rw-r--r--   0        0        0     9846 2023-03-31 12:39:04.197605 pydantic-translations-0.1.0/locales/de.po
--rw-r--r--   0        0        0    13115 2023-03-31 12:39:04.197605 pydantic-translations-0.1.0/locales/en.po
--rw-r--r--   0        0        0     9846 2023-03-31 12:39:04.197605 pydantic-translations-0.1.0/locales/es.po
--rw-r--r--   0        0        0     9845 2023-03-31 12:39:04.197605 pydantic-translations-0.1.0/locales/fr.po
--rw-r--r--   0        0        0     9846 2023-03-31 12:39:04.197605 pydantic-translations-0.1.0/locales/it.po
--rw-r--r--   0        0        0     9846 2023-03-31 12:39:04.197605 pydantic-translations-0.1.0/locales/nl.po
--rw-r--r--   0        0        0    14950 2023-04-03 07:03:56.036022 pydantic-translations-0.1.0/locales/ru.po
--rw-r--r--   0        0        0      126 2023-03-31 07:43:14.479910 pydantic-translations-0.1.0/pydantic_translations/__init__.py
--rw-r--r--   0        0        0      136 2023-03-31 08:42:52.417332 pydantic-translations-0.1.0/pydantic_translations/_constants.py
--rw-r--r--   0        0        0     9016 2023-03-31 10:10:09.219762 pydantic-translations-0.1.0/pydantic_translations/_messages.py
--rw-r--r--   0        0        0     4868 2023-03-31 12:50:11.309343 pydantic-translations-0.1.0/pydantic_translations/_translator.py
--rw-r--r--   0        0        0     1701 2023-03-31 09:09:16.931060 pydantic-translations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-31 07:34:31.548319 pydantic-translations-0.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-30 11:42:57.498741 pydantic-translations-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2126 2023-03-31 07:43:14.475910 pydantic-translations-0.1.0/tests/test_messages.py
--rw-r--r--   0        0        0     1464 2023-03-31 10:12:59.705748 pydantic-translations-0.1.0/tests/test_translate.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 pydantic-translations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-04-03 10:57:30.267939 pydantic-translations-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      128 2023-03-31 09:09:46.066607 pydantic-translations-0.2.0/.gitignore
+-rw-r--r--   0        0        0      325 2023-03-31 07:34:53.564133 pydantic-translations-0.2.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2023-03-31 07:35:20.203909 pydantic-translations-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2679 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/README.md
+-rw-r--r--   0        0        0     3967 2023-03-31 10:15:59.804031 pydantic-translations-0.2.0/Taskfile.yml
+-rw-r--r--   0        0        0    13300 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/locales/de.po
+-rw-r--r--   0        0        0    13115 2023-03-31 12:39:04.197605 pydantic-translations-0.2.0/locales/en.po
+-rw-r--r--   0        0        0    13520 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/locales/es.po
+-rw-r--r--   0        0        0    13769 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/locales/fr.po
+-rw-r--r--   0        0        0    13470 2023-04-18 09:37:06.906758 pydantic-translations-0.2.0/locales/it.po
+-rw-r--r--   0        0        0    13007 2023-04-18 09:37:06.906758 pydantic-translations-0.2.0/locales/nl.po
+-rw-r--r--   0        0        0    14950 2023-04-03 07:03:56.036022 pydantic-translations-0.2.0/locales/ru.po
+-rw-r--r--   0        0        0      126 2023-04-18 09:37:06.906758 pydantic-translations-0.2.0/pydantic_translations/__init__.py
+-rw-r--r--   0        0        0      136 2023-03-31 08:42:52.417332 pydantic-translations-0.2.0/pydantic_translations/_constants.py
+-rw-r--r--   0        0        0     9016 2023-03-31 10:10:09.219762 pydantic-translations-0.2.0/pydantic_translations/_messages.py
+-rw-r--r--   0        0        0     4868 2023-03-31 12:50:11.309343 pydantic-translations-0.2.0/pydantic_translations/_translator.py
+-rw-r--r--   0        0        0     1701 2023-03-31 09:09:16.931060 pydantic-translations-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-31 07:34:31.548319 pydantic-translations-0.2.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-03-30 11:42:57.498741 pydantic-translations-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2126 2023-03-31 07:43:14.475910 pydantic-translations-0.2.0/tests/test_messages.py
+-rw-r--r--   0        0        0     1464 2023-03-31 10:12:59.705748 pydantic-translations-0.2.0/tests/test_translate.py
+-rw-r--r--   0        0        0     3682 1970-01-01 00:00:00.000000 pydantic-translations-0.2.0/PKG-INFO
```

### Comparing `pydantic-translations-0.1.0/LICENSE` & `pydantic-translations-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/README.md` & `pydantic-translations-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 Translations for pydantic errors.
 
 ## Languages
 
 Currently, we have translated pydantic v1.10.2 errors to the following languages:
 
-* `de`: German. 0/87.
-* `es`: Spanish. 0/87.
-* `fr`: French. 0/87.
-* `it`: Italian. 0/87.
-* `nl`: Dutch. 0/87.
+* `de`: German. 87/87.
+* `es`: Spanish. 87/87.
+* `fr`: French. 87/87.
+* `it`: Italian. 87/87.
+* `nl`: Dutch. 87/87.
 * `ru`: Russian. 70/87.
 
 Need more languages? Contributions are welcome!
 
 ## Installation
 
 ```bash
@@ -84,12 +84,12 @@
 locales = Locales()
 locale = locales['ua']
 tr = Translator(locale)
 ```
 
 ## Contributors
 
-1. The original error messages provided by @samuelcolvin and [pydantic contributors](https://github.com/pydantic/pydantic/graphs/contributors).
-1. The Russian translation is provided by @orsinium.
+1. The original error messages provided by [@samuelcolvin](https://github.com/samuelcolvin) and [pydantic contributors](https://github.com/pydantic/pydantic/graphs/contributors).
+1. The Russian translation is provided by [@orsinium](https://github.com/orsinium).
 1. The German, Spanish, French, Italian, and Dutch translations are provided by [Andovar](https://andovar.com/) translation agency.
 
 Minor corrections and improvements are provided by [the project contributors](https://github.com/orsinium-labs/pydantic-translations/graphs/contributors).
```

### Comparing `pydantic-translations-0.1.0/Taskfile.yml` & `pydantic-translations-0.2.0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/locales/en.po` & `pydantic-translations-0.2.0/locales/en.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/locales/ru.po` & `pydantic-translations-0.2.0/locales/ru.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/pydantic_translations/_messages.py` & `pydantic-translations-0.2.0/pydantic_translations/_messages.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/pydantic_translations/_translator.py` & `pydantic-translations-0.2.0/pydantic_translations/_translator.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/pyproject.toml` & `pydantic-translations-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/tests/test_messages.py` & `pydantic-translations-0.2.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/tests/test_translate.py` & `pydantic-translations-0.2.0/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.1.0/PKG-INFO` & `pydantic-translations-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-translations
-Version: 0.1.0
+Version: 0.2.0
 Summary: Translations for pydantic errors.
 Keywords: mypy,typing,annotations,type annotations
 Author-email: Gram <git@orsinium.dev>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,19 +30,19 @@
 
 Translations for pydantic errors.
 
 ## Languages
 
 Currently, we have translated pydantic v1.10.2 errors to the following languages:
 
-* `de`: German. 0/87.
-* `es`: Spanish. 0/87.
-* `fr`: French. 0/87.
-* `it`: Italian. 0/87.
-* `nl`: Dutch. 0/87.
+* `de`: German. 87/87.
+* `es`: Spanish. 87/87.
+* `fr`: French. 87/87.
+* `it`: Italian. 87/87.
+* `nl`: Dutch. 87/87.
 * `ru`: Russian. 70/87.
 
 Need more languages? Contributions are welcome!
 
 ## Installation
 
 ```bash
@@ -112,13 +112,13 @@
 locales = Locales()
 locale = locales['ua']
 tr = Translator(locale)
 ```
 
 ## Contributors
 
-1. The original error messages provided by @samuelcolvin and [pydantic contributors](https://github.com/pydantic/pydantic/graphs/contributors).
-1. The Russian translation is provided by @orsinium.
+1. The original error messages provided by [@samuelcolvin](https://github.com/samuelcolvin) and [pydantic contributors](https://github.com/pydantic/pydantic/graphs/contributors).
+1. The Russian translation is provided by [@orsinium](https://github.com/orsinium).
 1. The German, Spanish, French, Italian, and Dutch translations are provided by [Andovar](https://andovar.com/) translation agency.
 
 Minor corrections and improvements are provided by [the project contributors](https://github.com/orsinium-labs/pydantic-translations/graphs/contributors).
```

