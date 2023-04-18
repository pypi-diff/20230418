# Comparing `tmp/mimeograph-0.3.0.tar.gz` & `tmp/mimeograph-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.3.0.tar", last modified: Fri Apr 14 08:40:45 2023, max compression
+gzip compressed data, was "mimeograph-0.3.1.tar", last modified: Tue Apr 18 09:44:20 2023, max compression
```

## Comparing `mimeograph-0.3.0.tar` & `mimeograph-0.3.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.3.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       69 2023-03-31 04:40:40.000000 mimeograph-0.3.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    20178 2023-04-14 08:40:45.788154 mimeograph-0.3.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    18221 2023-04-14 08:35:34.000000 mimeograph-0.3.0/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     1422 2023-04-14 08:40:13.000000 mimeograph-0.3.0/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-14 08:40:45.788154 mimeograph-0.3.0/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.780153 mimeograph-0.3.0/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-14 08:40:13.000000 mimeograph-0.3.0/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9013 2023-04-14 08:40:13.000000 mimeograph-0.3.0/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-03-13 09:26:49.000000 mimeograph-0.3.0/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    11602 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-03-27 15:10:13.000000 mimeograph-0.3.0/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-04 09:02:56.000000 mimeograph-0.3.0/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      881 2023-03-20 11:29:27.000000 mimeograph-0.3.0/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-03-11 12:33:58.000000 mimeograph-0.3.0/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/annotations.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4098 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)      109 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      125 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1316 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/database/mimeo_db.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      649 2023-04-03 07:14:05.000000 mimeograph-0.3.0/src/mimeo/exceptions.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5745 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.784153 mimeograph-0.3.0/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.3.0/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)      455 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)      301 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6899 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6555 2023-04-14 08:35:34.000000 mimeograph-0.3.0/src/mimeo/utils/renderer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    20178 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1596 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       91 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-14 08:40:45.000000 mimeograph-0.3.0/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 08:40:45.788154 mimeograph-0.3.0/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)    29774 2023-04-03 07:14:05.000000 mimeograph-0.3.0/tests/test_mimeo_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 08:35:34.000000 mimeograph-0.3.0/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      462 2023-04-14 08:35:34.000000 mimeograph-0.3.0/tests/test_utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.700028 mimeograph-0.3.1/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.3.1/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       69 2023-03-31 04:40:40.000000 mimeograph-0.3.1/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    21308 2023-04-18 09:44:20.700028 mimeograph-0.3.1/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19351 2023-04-18 09:43:35.000000 mimeograph-0.3.1/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1422 2023-04-18 09:43:59.000000 mimeograph-0.3.1/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-18 09:44:20.700028 mimeograph-0.3.1/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-18 09:43:59.000000 mimeograph-0.3.1/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9525 2023-04-18 09:43:59.000000 mimeograph-0.3.1/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-03-13 09:26:49.000000 mimeograph-0.3.1/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11602 2023-04-18 09:21:02.000000 mimeograph-0.3.1/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-03-27 15:10:13.000000 mimeograph-0.3.1/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-18 09:21:02.000000 mimeograph-0.3.1/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      881 2023-04-18 09:21:02.000000 mimeograph-0.3.1/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-03-11 12:33:58.000000 mimeograph-0.3.1/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/annotations.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4098 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      109 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      125 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1316 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/database/mimeo_db.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      649 2023-04-03 07:14:05.000000 mimeograph-0.3.1/src/mimeo/exceptions.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5745 2023-04-14 15:51:40.000000 mimeograph-0.3.1/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)      455 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      301 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6963 2023-04-18 09:43:35.000000 mimeograph-0.3.1/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6555 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/utils/renderer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    21308 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1596 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       91 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    31428 2023-04-14 15:51:40.000000 mimeograph-0.3.1/tests/test_mimeo_cli.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 09:39:06.000000 mimeograph-0.3.1/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      462 2023-04-14 09:39:06.000000 mimeograph-0.3.1/tests/test_utils.py
```

### Comparing `mimeograph-0.3.0/LICENSE` & `mimeograph-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/PKG-INFO` & `mimeograph-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -205,14 +205,51 @@
 | `vars`                          |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `xml_declaration`               |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
 | `_templates_`                   |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                         | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                         | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                       |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
+#### Mimeo Environment
+
+To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
+They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
+- `protocol`
+- `host`
+- `port`
+- `auth`
+- `username`
+- `password`
+
+Example
+```json
+{
+    "local": {
+        "host": "localhost",
+        "port": 8000,
+        "username": "admin",
+        "password": "admin"
+    },
+    "dev": {
+        "protocol": "https",
+        "host": "11.111.11.111",
+        "port": 8000,
+        "auth": "digest",
+        "username": "some-user",
+        "password": "some-password"
+    }
+}
+```
+
+To use a specific Mimeo Environment you can use the following commands:
+```sh
+mimeo SomeEntity-config.json -e dev
+mimeo SomeEntity-config.json -e dev --http-envs-file environments.json
+```
+
 #### Mimeo Vars
 
 Mimeo allows you to define a list of variables.
 You can use them in your Mimeo Config by wrapping them in curly brackets [`{VARIABLE}`].
 
 There are only 2 rules for variable names:
 - Variable name can include upper-cased letters \[`A-Z`\], underscore \[`_`\] and digits \{`0-9`\} only
@@ -318,35 +355,48 @@
     }
   }
 }
 ```
 
 ##### Random Integer
 
-Generates a random integer value.
+Generates a random integer value between `start` and `limit` parameters (inclusive).
 
 ###### Raw
 
-Uses the default limit: 100.
+Uses the default start (1) and limit (100) values.
 
 ```json
 {
   "randominteger": "{random_int}"
 }
 ```
 
 ###### Parametrized
 
 Uses the customized limit.
 
 ```json
 {
-  "randominteger": {
+  "randominteger1": {
+    "_mimeo_util": {
+      "_name": "random_int",
+      "start": 0
+    }
+  },
+  "randominteger2": {
+    "_mimeo_util": {
+      "_name": "random_int",
+      "limit": 5
+    }
+  },
+  "randominteger3": {
     "_mimeo_util": {
       "_name": "random_int",
+      "start": 0,
       "limit": 5
     }
   }
 }
 ```
 
 ##### Random Item
```

### Comparing `mimeograph-0.3.0/README.md` & `mimeograph-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -163,14 +163,51 @@
 | `vars`                          |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `xml_declaration`               |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
 | `_templates_`                   |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                         | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                         | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                       |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
+#### Mimeo Environment
+
+To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
+They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
+- `protocol`
+- `host`
+- `port`
+- `auth`
+- `username`
+- `password`
+
+Example
+```json
+{
+    "local": {
+        "host": "localhost",
+        "port": 8000,
+        "username": "admin",
+        "password": "admin"
+    },
+    "dev": {
+        "protocol": "https",
+        "host": "11.111.11.111",
+        "port": 8000,
+        "auth": "digest",
+        "username": "some-user",
+        "password": "some-password"
+    }
+}
+```
+
+To use a specific Mimeo Environment you can use the following commands:
+```sh
+mimeo SomeEntity-config.json -e dev
+mimeo SomeEntity-config.json -e dev --http-envs-file environments.json
+```
+
 #### Mimeo Vars
 
 Mimeo allows you to define a list of variables.
 You can use them in your Mimeo Config by wrapping them in curly brackets [`{VARIABLE}`].
 
 There are only 2 rules for variable names:
 - Variable name can include upper-cased letters \[`A-Z`\], underscore \[`_`\] and digits \{`0-9`\} only
@@ -276,35 +313,48 @@
     }
   }
 }
 ```
 
 ##### Random Integer
 
-Generates a random integer value.
+Generates a random integer value between `start` and `limit` parameters (inclusive).
 
 ###### Raw
 
-Uses the default limit: 100.
+Uses the default start (1) and limit (100) values.
 
 ```json
 {
   "randominteger": "{random_int}"
 }
 ```
 
 ###### Parametrized
 
 Uses the customized limit.
 
 ```json
 {
-  "randominteger": {
+  "randominteger1": {
+    "_mimeo_util": {
+      "_name": "random_int",
+      "start": 0
+    }
+  },
+  "randominteger2": {
+    "_mimeo_util": {
+      "_name": "random_int",
+      "limit": 5
+    }
+  },
+  "randominteger3": {
     "_mimeo_util": {
       "_name": "random_int",
+      "start": 0,
       "limit": 5
     }
   }
 }
 ```
 
 ##### Random Item
```

### Comparing `mimeograph-0.3.0/pyproject.toml` & `mimeograph-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.3.0"
+version = "0.3.1"
 description = "Generate data based on a simple template"
 readme = "README.md"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
@@ -32,15 +32,15 @@
 [project.optional-dependencies]
 dev = ["bumpver", "build", "twine", "isort", "pytest", "pytest-cov", "responses"]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mimeograph-0.3.0/src/mimeo/__main__.py` & `mimeograph-0.3.1/src/mimeo/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from argparse import ArgumentParser
-from os import path
+from os import path, walk
 
 from mimeo import Mimeograph
 from mimeo.config import MimeoConfig
 from mimeo.context import MimeoContextManager
 from mimeo.exceptions import EnvironmentNotFound, EnvironmentsFileNotFound
 from mimeo.logging import setup_logging
 
@@ -21,15 +21,15 @@
         super().__init__(
             prog="mimeo",
             description="Generate data based on a template")
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.3.0")
+            version="%(prog)s v0.3.1")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configurations")
 
         mimeo_config_args = self.add_argument_group("Mimeo Configuration arguments")
@@ -134,27 +134,44 @@
             action="store_true",
             help="enable FINE mode")
 
 
 def main():
     mimeo_parser = MimeoArgumentParser()
     args = mimeo_parser.parse_args()
+    customize_logging_level(args)
+
+    logger.info("Starting Mimeo job")
+    paths = get_paths(args.paths)
+    for config_path in paths:
+        logger.info(f"Data generation from Mimeo Config: {config_path}")
+        mimeo_config = get_config(config_path, args)
+        with MimeoContextManager(mimeo_config):
+            Mimeograph(mimeo_config).produce()
+
+
+def customize_logging_level(args):
     if args.silent:
         logging.getLogger("mimeo").setLevel(logging.WARNING)
     elif args.debug:
         logging.getLogger("mimeo").setLevel(logging.DEBUG)
     elif args.fine:
         logging.getLogger("mimeo").setLevel(logging.FINE)
 
-    logger.info("Starting Mimeo job")
-    for path in args.paths:
-        logger.info(f"Data generation from Mimeo Config: {path}")
-        mimeo_config = get_config(path, args)
-        with MimeoContextManager(mimeo_config):
-            Mimeograph(mimeo_config).produce()
+
+def get_paths(paths: list) -> list:
+    file_paths = []
+    for file_path in paths:
+        if path.isdir(file_path):
+            for dir_path, _, file_names in walk(file_path):
+                for file_name in file_names:
+                    paths.append(f"{dir_path}/{file_name}")
+        elif path.isfile(file_path):
+            file_paths.append(file_path)
+    return file_paths
 
 
 def get_config(config_path, args):
     with open(config_path) as config_file:
         config = json.load(config_file)
         if args.http_env is not None:
             envs_file = args.http_envs_file if args.http_envs_file is not None else DEFAULT_ENVS_FILE_PATH
```

### Comparing `mimeograph-0.3.0/src/mimeo/config/mimeo_config.py` & `mimeograph-0.3.1/src/mimeo/config/mimeo_config.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/consumers/consumer_factory.py` & `mimeograph-0.3.1/src/mimeo/consumers/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.3.1/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.3.1/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/context/annotations.py` & `mimeograph-0.3.1/src/mimeo/context/annotations.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/context/mimeo_context.py` & `mimeograph-0.3.1/src/mimeo/context/mimeo_context.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-0.3.1/src/mimeo/context/mimeo_context_manager.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/context/mimeo_iteration.py` & `mimeograph-0.3.1/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/database/cities.py` & `mimeograph-0.3.1/src/mimeo/database/cities.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/database/countries.py` & `mimeograph-0.3.1/src/mimeo/database/countries.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/database/mimeo_db.py` & `mimeograph-0.3.1/src/mimeo/database/mimeo_db.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/exceptions.py` & `mimeograph-0.3.1/src/mimeo/exceptions.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/generators/generator.py` & `mimeograph-0.3.1/src/mimeo/generators/generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/generators/generator_factory.py` & `mimeograph-0.3.1/src/mimeo/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/generators/xml_generator.py` & `mimeograph-0.3.1/src/mimeo/generators/xml_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import xml.etree.ElementTree as ElemTree
 from typing import Iterator, List, Union
 from xml.dom import minidom
 
 from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
 from mimeo.context import MimeoContext
-from mimeo.context.annotations import (mimeo_clear_iterations,
+from mimeo.context.annotations import (mimeo_clear_iterations, mimeo_context,
                                        mimeo_context_switch,
-                                       mimeo_next_iteration, mimeo_context)
+                                       mimeo_next_iteration)
 from mimeo.generators import Generator
 from mimeo.utils import MimeoRenderer
 
 logger = logging.getLogger(__name__)
 
 
 class XMLGenerator(Generator):
```

### Comparing `mimeograph-0.3.0/src/mimeo/meta/alive.py` & `mimeograph-0.3.1/src/mimeo/meta/alive.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/mimeo.py` & `mimeograph-0.3.1/src/mimeo/mimeo.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/resources/cities.csv` & `mimeograph-0.3.1/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/resources/countries.csv` & `mimeograph-0.3.1/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/resources/logging.yaml` & `mimeograph-0.3.1/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeo/utils/mimeo_utils.py` & `mimeograph-0.3.1/src/mimeo/utils/mimeo_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,19 @@
 
 
 class RandomIntegerUtil(MimeoUtil):
 
     KEY = "random_int"
 
     def __init__(self, **kwargs):
+        self.__start = kwargs.get("limit", 1)
         self.__limit = kwargs.get("limit", 100)
 
     def render(self):
-        return random.randrange(self.__limit)
+        return random.randrange(self.__start, self.__limit + 1)
 
 
 class RandomItemUtil(MimeoUtil):
 
     KEY = "random_item"
 
     def __init__(self, **kwargs):
```

### Comparing `mimeograph-0.3.0/src/mimeo/utils/renderer.py` & `mimeograph-0.3.1/src/mimeo/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.3.1/src/mimeograph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -205,14 +205,51 @@
 | `vars`                          |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `xml_declaration`               |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
 | `_templates_`                   |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                         | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                         | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                       |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
+#### Mimeo Environment
+
+To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
+They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
+- `protocol`
+- `host`
+- `port`
+- `auth`
+- `username`
+- `password`
+
+Example
+```json
+{
+    "local": {
+        "host": "localhost",
+        "port": 8000,
+        "username": "admin",
+        "password": "admin"
+    },
+    "dev": {
+        "protocol": "https",
+        "host": "11.111.11.111",
+        "port": 8000,
+        "auth": "digest",
+        "username": "some-user",
+        "password": "some-password"
+    }
+}
+```
+
+To use a specific Mimeo Environment you can use the following commands:
+```sh
+mimeo SomeEntity-config.json -e dev
+mimeo SomeEntity-config.json -e dev --http-envs-file environments.json
+```
+
 #### Mimeo Vars
 
 Mimeo allows you to define a list of variables.
 You can use them in your Mimeo Config by wrapping them in curly brackets [`{VARIABLE}`].
 
 There are only 2 rules for variable names:
 - Variable name can include upper-cased letters \[`A-Z`\], underscore \[`_`\] and digits \{`0-9`\} only
@@ -318,35 +355,48 @@
     }
   }
 }
 ```
 
 ##### Random Integer
 
-Generates a random integer value.
+Generates a random integer value between `start` and `limit` parameters (inclusive).
 
 ###### Raw
 
-Uses the default limit: 100.
+Uses the default start (1) and limit (100) values.
 
 ```json
 {
   "randominteger": "{random_int}"
 }
 ```
 
 ###### Parametrized
 
 Uses the customized limit.
 
 ```json
 {
-  "randominteger": {
+  "randominteger1": {
+    "_mimeo_util": {
+      "_name": "random_int",
+      "start": 0
+    }
+  },
+  "randominteger2": {
+    "_mimeo_util": {
+      "_name": "random_int",
+      "limit": 5
+    }
+  },
+  "randominteger3": {
     "_mimeo_util": {
       "_name": "random_int",
+      "start": 0,
       "limit": 5
     }
   }
 }
 ```
 
 ##### Random Item
```

### Comparing `mimeograph-0.3.0/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.3.1/src/mimeograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.0/tests/test_mimeo_cli.py` & `mimeograph-0.3.1/tests/test_mimeo_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,16 @@
 
     # Teardown
     shutil.rmtree("test_mimeo_cli-dir")
     remove("mimeo.envs.json")
     remove("custom-mimeo-envs-file.json")
     for filename in glob("mimeo-output/customized-output-file*"):
         remove(filename)
+    for filename in glob("mimeo-output/mimeo-output*"):
+        remove(filename)
     if path.exists("mimeo-output") and not listdir("mimeo-output"):
         rmdir("mimeo-output")
 
 
 def test_basic_use():
     sys.argv = ["mimeo", "test_mimeo_cli-dir/default-config.json"]
 
@@ -162,14 +164,50 @@
             assert file_content.readline() == '<SomeEntity>\n'
             assert file_content.readline() == '    <ChildNode1>1</ChildNode1>\n'
             assert file_content.readline() == '    <ChildNode2>value-2</ChildNode2>\n'
             assert file_content.readline() == '    <ChildNode3>true</ChildNode3>\n'
             assert file_content.readline() == '</SomeEntity>\n'
 
 
+@responses.activate
+def test_directory_path():
+    sys.argv = ["mimeo", "test_mimeo_cli-dir"]
+
+    responses.add(responses.POST, "http://localhost:8080/document")
+    assert not path.exists("test_mimeo_cli-dir/output")
+    assert not path.exists("mimeo-output")
+
+    MimeoCLI.main()
+
+    assert path.exists("test_mimeo_cli-dir/output")
+    for i in range(1, 11):
+        file_path = f"test_mimeo_cli-dir/output/output-file-{i}.xml"
+        assert path.exists(file_path)
+
+        with open(file_path, "r") as file_content:
+            assert file_content.readline() == '<?xml version="1.0" encoding="utf-8"?>\n'
+            assert file_content.readline() == '<SomeEntity>\n'
+            assert file_content.readline() == '    <ChildNode1>1</ChildNode1>\n'
+            assert file_content.readline() == '    <ChildNode2>value-2</ChildNode2>\n'
+            assert file_content.readline() == '    <ChildNode3>true</ChildNode3>\n'
+            assert file_content.readline() == '</SomeEntity>\n'
+
+    assert path.exists("mimeo-output")
+    for i in range(1, 11):
+        file_path = f"mimeo-output/mimeo-output-{i}.xml"
+        assert path.exists(file_path)
+
+        with open(file_path, "r") as file_content:
+            assert file_content.readline() == '<SomeEntity>' \
+                                              '<ChildNode1>1</ChildNode1>' \
+                                              '<ChildNode2>value-2</ChildNode2>' \
+                                              '<ChildNode3>true</ChildNode3>' \
+                                              '</SomeEntity>' \
+
+
 def test_custom_short_xml_declaration_false():
     sys.argv = ["mimeo", "test_mimeo_cli-dir/default-config.json", "-x", "false"]
 
     assert not path.exists("test_mimeo_cli-dir/output")
 
     MimeoCLI.main()
```

### Comparing `mimeograph-0.3.0/tests/test_mimeograph.py` & `mimeograph-0.3.1/tests/test_mimeograph.py`

 * *Files identical despite different names*

