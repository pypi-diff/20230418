# Comparing `tmp/scenariogeneration-0.9.2.tar.gz` & `tmp/scenariogeneration-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenariogeneration-0.9.2.tar", last modified: Fri Oct 14 12:36:42 2022, max compression
+gzip compressed data, was "scenariogeneration-0.9.3.tar", last modified: Thu Oct 20 12:39:14 2022, max compression
```

## Comparing `scenariogeneration-0.9.2.tar` & `scenariogeneration-0.9.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-14 12:36:42.584364 scenariogeneration-0.9.2/
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    16776 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/LICENSE
--rw-rw-r--   0 mander76  (1000) mander76  (1000)       15 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/MANIFEST.in
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     4441 2022-10-14 12:36:42.584364 scenariogeneration-0.9.2/PKG-INFO
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     3612 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/README.md
-drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-14 12:36:42.576364 scenariogeneration-0.9.2/examples/
--rw-rw-r--   0 mander76  (1000) mander76  (1000)      389 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/examples/__init__.py
-drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-14 12:36:42.576364 scenariogeneration-0.9.2/scenariogeneration/
--rw-rw-r--   0 mander76  (1000) mander76  (1000)      245 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/__init__.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     6748 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/esmini_runner.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     3405 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/helpers.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    11499 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/scenario_generator.py
-drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-14 12:36:42.580364 scenariogeneration-0.9.2/scenariogeneration/xodr/
--rw-rw-r--   0 mander76  (1000) mander76  (1000)      353 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/__init__.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     7169 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/elevation.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     3901 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/enumerations.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     1503 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/exceptions.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    43288 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/generators.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    30962 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/geometry.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    40119 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/junction_creator.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    25918 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/lane.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    36367 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/links.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    41821 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/opendrive.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    34784 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/signals_objects.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     1358 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xodr/utils.py
-drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-14 12:36:42.580364 scenariogeneration-0.9.2/scenariogeneration/xosc/
--rw-rw-r--   0 mander76  (1000) mander76  (1000)      595 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/__init__.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)   141164 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/actions.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    45185 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/entities.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    12005 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/enumerations.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     1085 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/exceptions.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    42189 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/parameters.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    78812 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/position.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    12673 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/scenario.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    37096 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/storyboard.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    90984 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/triggers.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)   121524 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/utils.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     8780 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/scenariogeneration/xosc/xosc_reader.py
-drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-14 12:36:42.576364 scenariogeneration-0.9.2/scenariogeneration.egg-info/
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     4441 2022-10-14 12:36:42.000000 scenariogeneration-0.9.2/scenariogeneration.egg-info/PKG-INFO
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     1753 2022-10-14 12:36:42.000000 scenariogeneration-0.9.2/scenariogeneration.egg-info/SOURCES.txt
--rw-rw-r--   0 mander76  (1000) mander76  (1000)        1 2022-10-14 12:36:42.000000 scenariogeneration-0.9.2/scenariogeneration.egg-info/dependency_links.txt
--rw-rw-r--   0 mander76  (1000) mander76  (1000)       24 2022-10-14 12:36:42.000000 scenariogeneration-0.9.2/scenariogeneration.egg-info/requires.txt
--rw-rw-r--   0 mander76  (1000) mander76  (1000)       34 2022-10-14 12:36:42.000000 scenariogeneration-0.9.2/scenariogeneration.egg-info/top_level.txt
--rw-rw-r--   0 mander76  (1000) mander76  (1000)      102 2022-10-14 12:36:42.584364 scenariogeneration-0.9.2/setup.cfg
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     1122 2022-10-14 12:32:45.000000 scenariogeneration-0.9.2/setup.py
-drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-14 12:36:42.584364 scenariogeneration-0.9.2/tests/
--rw-rw-r--   0 mander76  (1000) mander76  (1000)        0 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/__init__.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    25413 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_actions.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     1186 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_catalog.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     2613 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_elevation.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     8866 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_entities.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    13085 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_geometry.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    33455 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_junction_creator.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     5744 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_lane.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    21571 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_links.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     6099 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_opendrive.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     9647 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_parameters.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    12244 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_position.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    10466 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_reader.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     4827 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_scenario.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     5866 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_scenario_generator.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)     5660 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_signals_objects.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    14444 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_storyboard.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    17515 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_triggers.py
--rw-rw-r--   0 mander76  (1000) mander76  (1000)    21135 2022-10-03 07:31:44.000000 scenariogeneration-0.9.2/tests/test_utils.py
+drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-20 12:39:14.475206 scenariogeneration-0.9.3/
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    16776 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/LICENSE
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)       15 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/MANIFEST.in
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     4441 2022-10-20 12:39:14.475206 scenariogeneration-0.9.3/PKG-INFO
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     3612 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/README.md
+drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-20 12:39:14.471207 scenariogeneration-0.9.3/examples/
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)      389 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/examples/__init__.py
+drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-20 12:39:14.471207 scenariogeneration-0.9.3/scenariogeneration/
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)      245 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/__init__.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     6748 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/esmini_runner.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     3405 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/helpers.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    11523 2022-10-20 12:33:12.000000 scenariogeneration-0.9.3/scenariogeneration/scenario_generator.py
+drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-20 12:39:14.471207 scenariogeneration-0.9.3/scenariogeneration/xodr/
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)      353 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/__init__.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     7169 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/elevation.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     3901 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/enumerations.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     1503 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/exceptions.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    43288 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/generators.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    30962 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/geometry.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    40119 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/junction_creator.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    25918 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/lane.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    36367 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/links.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    41821 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/opendrive.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    34784 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/signals_objects.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     1358 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xodr/utils.py
+drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-20 12:39:14.471207 scenariogeneration-0.9.3/scenariogeneration/xosc/
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)      595 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/__init__.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)   141164 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/actions.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    45185 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/entities.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    12005 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/enumerations.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     1085 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/exceptions.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    42189 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/parameters.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    78812 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/position.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    12673 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/scenario.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    37096 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/storyboard.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    90984 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/triggers.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)   121524 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/utils.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     8780 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/scenariogeneration/xosc/xosc_reader.py
+drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-20 12:39:14.471207 scenariogeneration-0.9.3/scenariogeneration.egg-info/
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     4441 2022-10-20 12:39:14.000000 scenariogeneration-0.9.3/scenariogeneration.egg-info/PKG-INFO
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     1753 2022-10-20 12:39:14.000000 scenariogeneration-0.9.3/scenariogeneration.egg-info/SOURCES.txt
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)        1 2022-10-20 12:39:14.000000 scenariogeneration-0.9.3/scenariogeneration.egg-info/dependency_links.txt
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)       24 2022-10-20 12:39:14.000000 scenariogeneration-0.9.3/scenariogeneration.egg-info/requires.txt
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)       34 2022-10-20 12:39:14.000000 scenariogeneration-0.9.3/scenariogeneration.egg-info/top_level.txt
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)      102 2022-10-20 12:39:14.475206 scenariogeneration-0.9.3/setup.cfg
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     1122 2022-10-20 12:38:07.000000 scenariogeneration-0.9.3/setup.py
+drwxrwxr-x   0 mander76  (1000) mander76  (1000)        0 2022-10-20 12:39:14.475206 scenariogeneration-0.9.3/tests/
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)        0 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/__init__.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    25413 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_actions.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     1186 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_catalog.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     2613 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_elevation.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     8866 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_entities.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    13085 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_geometry.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    33455 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_junction_creator.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     5744 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_lane.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    21571 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_links.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     6099 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_opendrive.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     9647 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_parameters.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    12244 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_position.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    10466 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_reader.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     4827 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_scenario.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     5866 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_scenario_generator.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)     5660 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_signals_objects.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    14444 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_storyboard.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    17515 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_triggers.py
+-rw-rw-r--   0 mander76  (1000) mander76  (1000)    21135 2022-10-03 07:31:44.000000 scenariogeneration-0.9.3/tests/test_utils.py
```

### Comparing `scenariogeneration-0.9.2/LICENSE` & `scenariogeneration-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/PKG-INFO` & `scenariogeneration-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scenariogeneration
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generation of OpenSCENARIO and OpenDRIVE xml files
 Home-page: https://github.com/pyoscx/scenariogeneration
 Author: Mikael Andersson, Irene Natale, Andreas Tingberg
 Author-email: andmika@gmail.com
 License: MPL-2.0
-Download-URL: https://github.com/pyoscx/scenariogeneration/archive/v0.9.2.tar.gz
+Download-URL: https://github.com/pyoscx/scenariogeneration/archive/v0.9.3.tar.gz
 Keywords: OpenDRIVE,OpenSCENARIO,xml
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `scenariogeneration-0.9.2/README.md` & `scenariogeneration-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/esmini_runner.py` & `scenariogeneration-0.9.3/scenariogeneration/esmini_runner.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/helpers.py` & `scenariogeneration-0.9.3/scenariogeneration/helpers.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/scenario_generator.py` & `scenariogeneration-0.9.3/scenariogeneration/scenario_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
   scenariogeneration
   https://github.com/pyoscx/scenariogeneration
- 
+
   This Source Code Form is subject to the terms of the Mozilla Public
   License, v. 2.0. If a copy of the MPL was not distributed with this
   file, You can obtain one at https://mozilla.org/MPL/2.0/.
- 
+
   Copyright (c) 2022 The scenariogeneration Authors.
 
 """
 import itertools
 import os
 import numpy as np
 import sys
@@ -245,14 +245,15 @@
                 it = 0
             elif order == "middle":
                 it = int(np.floor(len(self.all_permutations) / 2))
             elif order == "random":
                 it = int(np.floor(np.random.rand() * len(self.all_permutations)))
         else:
             it = order
+            self._it = it
         osc, odr = self._generate_road_and_scenario(self.all_permutations[it])
         self._reset_name_counter()
         return osc, odr
 
     def generate(
         self,
         generation_folder,
```

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/elevation.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/elevation.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/enumerations.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/enumerations.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/exceptions.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/exceptions.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/generators.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/generators.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/geometry.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/geometry.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/junction_creator.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/junction_creator.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/lane.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/lane.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/links.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/links.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/opendrive.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/opendrive.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/signals_objects.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/signals_objects.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xodr/utils.py` & `scenariogeneration-0.9.3/scenariogeneration/xodr/utils.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/__init__.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/__init__.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/actions.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/actions.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/entities.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/entities.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/enumerations.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/enumerations.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/exceptions.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/exceptions.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/parameters.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/parameters.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/position.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/position.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/scenario.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/scenario.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/storyboard.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/storyboard.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/triggers.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/triggers.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/utils.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/utils.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration/xosc/xosc_reader.py` & `scenariogeneration-0.9.3/scenariogeneration/xosc/xosc_reader.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/scenariogeneration.egg-info/PKG-INFO` & `scenariogeneration-0.9.3/scenariogeneration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scenariogeneration
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generation of OpenSCENARIO and OpenDRIVE xml files
 Home-page: https://github.com/pyoscx/scenariogeneration
 Author: Mikael Andersson, Irene Natale, Andreas Tingberg
 Author-email: andmika@gmail.com
 License: MPL-2.0
-Download-URL: https://github.com/pyoscx/scenariogeneration/archive/v0.9.2.tar.gz
+Download-URL: https://github.com/pyoscx/scenariogeneration/archive/v0.9.3.tar.gz
 Keywords: OpenDRIVE,OpenSCENARIO,xml
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `scenariogeneration-0.9.2/scenariogeneration.egg-info/SOURCES.txt` & `scenariogeneration-0.9.3/scenariogeneration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/setup.py` & `scenariogeneration-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scenariogeneration",
-    version="0.9.2",
+    version="0.9.3",
     license="MPL-2.0",
     author="Mikael Andersson, Irene Natale, Andreas Tingberg",
     author_email="andmika@gmail.com",
     description="Generation of OpenSCENARIO and OpenDRIVE xml files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pyoscx/scenariogeneration",
-    download_url="https://github.com/pyoscx/scenariogeneration/archive/v0.9.2.tar.gz",
+    download_url="https://github.com/pyoscx/scenariogeneration/archive/v0.9.3.tar.gz",
     packages=setuptools.find_packages(),
     keywords=["OpenDRIVE", "OpenSCENARIO", "xml"],
     install_requires=["numpy", "scipy", "pyclothoids"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

### Comparing `scenariogeneration-0.9.2/tests/test_actions.py` & `scenariogeneration-0.9.3/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_catalog.py` & `scenariogeneration-0.9.3/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_elevation.py` & `scenariogeneration-0.9.3/tests/test_elevation.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_entities.py` & `scenariogeneration-0.9.3/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_geometry.py` & `scenariogeneration-0.9.3/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_junction_creator.py` & `scenariogeneration-0.9.3/tests/test_junction_creator.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_lane.py` & `scenariogeneration-0.9.3/tests/test_lane.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_links.py` & `scenariogeneration-0.9.3/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_opendrive.py` & `scenariogeneration-0.9.3/tests/test_opendrive.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_parameters.py` & `scenariogeneration-0.9.3/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_position.py` & `scenariogeneration-0.9.3/tests/test_position.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_reader.py` & `scenariogeneration-0.9.3/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_scenario.py` & `scenariogeneration-0.9.3/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_scenario_generator.py` & `scenariogeneration-0.9.3/tests/test_scenario_generator.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_signals_objects.py` & `scenariogeneration-0.9.3/tests/test_signals_objects.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_storyboard.py` & `scenariogeneration-0.9.3/tests/test_storyboard.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_triggers.py` & `scenariogeneration-0.9.3/tests/test_triggers.py`

 * *Files identical despite different names*

### Comparing `scenariogeneration-0.9.2/tests/test_utils.py` & `scenariogeneration-0.9.3/tests/test_utils.py`

 * *Files identical despite different names*

