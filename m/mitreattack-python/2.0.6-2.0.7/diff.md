# Comparing `tmp/mitreattack-python-2.0.6.tar.gz` & `tmp/mitreattack-python-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitreattack-python-2.0.6.tar", last modified: Mon Mar 13 18:32:50 2023, max compression
+gzip compressed data, was "mitreattack-python-2.0.7.tar", last modified: Tue Apr 18 21:11:19 2023, max compression
```

## Comparing `mitreattack-python-2.0.6.tar` & `mitreattack-python-2.0.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.816634 mitreattack-python-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-03-13 18:32:50.816634 mitreattack-python-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.804634 mitreattack-python-2.0.6/mitreattack/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.808634 mitreattack-python-2.0.6/mitreattack/attackToExcel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/attackToExcel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/attackToExcel/attackToExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/attackToExcel/stixToDf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.808634 mitreattack-python-2.0.6/mitreattack/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/collections/collection_to_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/collections/index_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/collections/stix_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.808634 mitreattack-python-2.0.6/mitreattack/diffStix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/diffStix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86864 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/diffStix/changelog_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/download_stix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.808634 mitreattack-python-2.0.6/mitreattack/navlayers/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.812634 mitreattack-python-2.0.6/mitreattack/navlayers/core/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/layerobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/legenditem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/objlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/technique.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/core/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.812634 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/excel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.812634 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   358460 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/fonts/monospace.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    85240 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/fonts/serif.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/matrix_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/svg_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/svg_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/to_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/exporters/to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.812634 mitreattack-python-2.0.6/mitreattack/navlayers/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/generators/gen_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/generators/overview_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/generators/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/generators/usage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/layerExporter_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/layerGenerator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.816634 mitreattack-python-2.0.6/mitreattack/navlayers/manipulators/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/manipulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/navlayers/manipulators/layerops.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/release_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.816634 mitreattack-python-2.0.6/mitreattack/stix20/
--rw-r--r--   0 runner    (1001) docker     (123)    61313 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/stix20/MitreAttackData.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/stix20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/mitreattack/stix20/custom_attack_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.816634 mitreattack-python-2.0.6/mitreattack_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-03-13 18:32:50.000000 mitreattack-python-2.0.6/mitreattack_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-13 18:32:50.000000 mitreattack-python-2.0.6/mitreattack_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 18:32:50.000000 mitreattack-python-2.0.6/mitreattack_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-13 18:32:50.000000 mitreattack-python-2.0.6/mitreattack_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-13 18:32:50.000000 mitreattack-python-2.0.6/mitreattack_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-13 18:32:50.000000 mitreattack-python-2.0.6/mitreattack_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 18:32:50.816634 mitreattack-python-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 18:32:50.816634 mitreattack-python-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-13 18:09:03.000000 mitreattack-python-2.0.6/tests/test_to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/attackToExcel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/attackToExcel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/attackToExcel/attackToExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/attackToExcel/stixToDf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/collection_to_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/index_to_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/collections/stix_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/diffStix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/diffStix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87227 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/diffStix/changelog_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/download_stix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.967008 mitreattack-python-2.0.7/mitreattack/navlayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.971008 mitreattack-python-2.0.7/mitreattack/navlayers/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/layerobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/legenditem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/objlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/technique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/core/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.971008 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/excel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   358460 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/monospace.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    85240 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    17843 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/matrix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/navlayers/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/gen_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/overview_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/generators/usage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/layerExporter_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/layerGenerator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/layerops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/release_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack/stix20/
+-rw-r--r--   0 runner    (1001) docker     (123)    61287 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/stix20/MitreAttackData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/stix20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/mitreattack/stix20/custom_attack_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.975008 mitreattack-python-2.0.7/mitreattack_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 21:11:19.000000 mitreattack-python-2.0.7/mitreattack_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:11:19.979008 mitreattack-python-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-18 20:48:09.000000 mitreattack-python-2.0.7/tests/test_to_excel.py
```

### Comparing `mitreattack-python-2.0.6/LICENSE.txt` & `mitreattack-python-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/NOTICE.txt` & `mitreattack-python-2.0.7/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/PKG-INFO` & `mitreattack-python-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 2.0.6
+Version: 2.0.7
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-2.0.6/README.md` & `mitreattack-python-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/attackToExcel/attackToExcel.py` & `mitreattack-python-2.0.7/mitreattack/attackToExcel/attackToExcel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/attackToExcel/stixToDf.py` & `mitreattack-python-2.0.7/mitreattack/attackToExcel/stixToDf.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/collections/collection_to_index.py` & `mitreattack-python-2.0.7/mitreattack/collections/collection_to_index.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/collections/index_to_markdown.py` & `mitreattack-python-2.0.7/mitreattack/collections/index_to_markdown.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/collections/stix_to_collection.py` & `mitreattack-python-2.0.7/mitreattack/collections/stix_to_collection.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/diffStix/changelog_helper.py` & `mitreattack-python-2.0.7/mitreattack/diffStix/changelog_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,35 +100,33 @@
             "campaigns": "Campaigns",
             "mitigations": "Mitigations",
             "datasources": "Data Sources",
             "datacomponents": "Data Components",
         }
 
         self.section_descriptions = {
-            "additions": "ATT&CK objects which are present in the new STIX data but not the old.",
+            "additions": "ATT&CK objects which are only present in the new STIX data.",
             "major_version_changes": "ATT&CK objects that have a major version change. (e.g. 1.0 → 2.0)",
             "minor_version_changes": "ATT&CK objects that have a minor version change. (e.g. 1.0 → 1.1)",
-            "other_version_changes": "ATT&CK objects that have an unexpected version change. (e.g. 1.0 → 1.3)",
-            "metadata_changes": "ATT&CK objects that have at least one field changed, but not the version.",
-            "unknown_changes": "ATT&CK objects that have changed while the modified time stayed the same.",
+            "other_version_changes": "ATT&CK objects that have a version change of any other kind. (e.g. 1.0 → 1.3)",
+            "patches": "ATT&CK objects that have been patched while keeping the version the same.",
             "revocations": "ATT&CK objects which are revoked by a different object.",
             "deprecations": "ATT&CK objects which are deprecated and no longer in use, and not replaced.",
             "deletions": "ATT&CK objects which are no longer found in the STIX data.",
             "unchanged": "ATT&CK objects which did not change between the two versions.",
         }
 
         self.section_headers = {}
         for object_type in self.types:
             self.section_headers[object_type] = {
                 "additions": f"New {self.attack_type_to_title[object_type]}",
                 "major_version_changes": "Major Version Changes",
                 "minor_version_changes": "Minor Version Changes",
                 "other_version_changes": "Other Version Changes",
-                "metadata_changes": "Metadata-only Changes",
-                "unknown_changes": "Unknown Changes",
+                "patches": "Patches",
                 "deprecations": "Deprecations",
                 "revocations": "Revocations",
                 "deletions": "Deletions",
                 "unchanged": "Unchanged",
             }
 
         # will hold information of contributors of the new release {... {"contributor_credit/name_as_key": counter]} ...}
@@ -143,16 +141,15 @@
                 # "technique": {
                 #     "enterprise-attack": {
                 #         "additions": [],
                 #         "deletions": [],
                 #         "major_version_changes": [],
                 #         "minor_version_changes": [],
                 #         "other_version_changes": [],
-                #         "metadata_changes": [],
-                #         "unknown_changes": [],
+                #         "patches": [],
                 #         "revocations": [],
                 #         "deprecations": [],
                 #         "unchanged": [],
                 #     },
                 #     "mobile-attack": {...},
                 # },
                 # "software": {...},
@@ -196,16 +193,15 @@
                 additions = new_attack_objects.keys() - old_attack_objects.keys()
                 deletions = old_attack_objects.keys() - new_attack_objects.keys()
 
                 # sets to store the ids of objects for each section
                 major_version_changes = set()
                 minor_version_changes = set()
                 other_version_changes = set()
-                metadata_changes = set()
-                unknown_changes = set()
+                patches = set()
                 revocations = set()
                 deprecations = set()
                 unchanged = set()
 
                 # find changes, revocations and deprecations
                 for stix_id in intersection:
                     old_stix_obj = old_attack_objects[stix_id]
@@ -255,67 +251,43 @@
                         # Verify if there are new contributors on the object
                         self.update_contributors(old_object=old_stix_obj, new_object=new_stix_obj)
 
                         old_version = get_attack_object_version(old_stix_obj)
                         new_version = get_attack_object_version(new_stix_obj)
                         new_stix_obj["previous_version"] = old_version
 
-                        # Version number didn't change
-                        ##############################
-                        if new_version == old_version:
-                            # check for modification date increase but not version
-                            old_date = dateparser.parse(old_stix_obj["modified"])
-                            new_date = dateparser.parse(new_stix_obj["modified"])
-                            if new_date != old_date:
-                                metadata_changes.add(stix_id)
-                            else:
-                                unchanged.add(stix_id)
-
-                        # Version number changed
-                        ########################
+                        if is_major_version_change(old_version=old_version, new_version=new_version):
+                            major_version_changes.add(stix_id)
+                        elif is_minor_version_change(old_version=old_version, new_version=new_version):
+                            minor_version_changes.add(stix_id)
+                        elif is_other_version_change(old_version=old_version, new_version=new_version):
+                            logger.warning(f"{stix_id} - Unexpected version increase {old_version} → {new_version}. [{attack_id}] {new_stix_obj['name']}")
+                            other_version_changes.add(stix_id)
+                        elif is_patch_change(old_stix_obj=old_stix_obj, new_stix_obj=new_stix_obj):
+                            patches.add(stix_id)
                         else:
-                            if is_major_version_change(old_version=old_version, new_version=new_version):
-                                major_version_changes.add(stix_id)
-                            elif is_minor_version_change(old_version=old_version, new_version=new_version):
-                                minor_version_changes.add(stix_id)
-                            else:
-                                other_version_changes.add(stix_id)
-                                logger.warning(
-                                    f"{stix_id} - Unexpected version increase {old_version} → {new_version}. [{attack_id}] {new_stix_obj['name']}"
-                                )
+                            unchanged.add(stix_id)
 
+                        if new_version != old_version:
                             new_stix_obj["version_change"] = f"{old_version} → {new_version}"
 
                         # Description changes
                         #####################
                         old_lines = old_stix_obj["description"].replace("\n", " ").splitlines()
                         new_lines = new_stix_obj["description"].replace("\n", " ").splitlines()
-
-                        df = [x for x in old_lines if x not in new_lines]
-                        df1 = [x for x in new_lines if x not in old_lines]
-
-                        if df != [] or df1 != []:
-                            if (
-                                (stix_id not in major_version_changes)
-                                and (stix_id not in minor_version_changes)
-                                and (stix_id not in metadata_changes)
-                                and (stix_id not in other_version_changes)
-                            ):
-                                logger.error(
-                                    f"{stix_id} - Somehow {attack_id} has a description change "
-                                    "without the version being incremented or the last modified date changing"
-                                )
-                                unknown_changes.add(stix_id)
-
+                        old_lines_unique = [line for line in old_lines if line not in new_lines]
+                        new_lines_unique = [line for line in new_lines if line not in old_lines]
+                        if old_lines_unique or new_lines_unique:
                             html_diff = difflib.HtmlDiff(wrapcolumn=60)
                             html_diff._legend = ""
-
                             delta = html_diff.make_table(old_lines, new_lines, "Old Description", "New Description")
                             new_stix_obj["description_change_table"] = delta
 
+                        # Relationship changes
+                        ######################
                         if new_stix_obj["type"] == "attack-pattern":
                             self.find_technique_mitigation_changes(new_stix_obj, domain)
                             self.find_technique_detection_changes(new_stix_obj, domain)
 
                 #############
                 # New objects
                 #############
@@ -362,20 +334,16 @@
                         [new_attack_objects[stix_id] for stix_id in minor_version_changes],
                         key=lambda stix_object: stix_object["name"],
                     ),
                     "other_version_changes": sorted(
                         [new_attack_objects[stix_id] for stix_id in other_version_changes],
                         key=lambda stix_object: stix_object["name"],
                     ),
-                    "metadata_changes": sorted(
-                        [new_attack_objects[stix_id] for stix_id in metadata_changes],
-                        key=lambda stix_object: stix_object["name"],
-                    ),
-                    "unknown_changes": sorted(
-                        [new_attack_objects[stix_id] for stix_id in unknown_changes],
+                    "patches": sorted(
+                        [new_attack_objects[stix_id] for stix_id in patches],
                         key=lambda stix_object: stix_object["name"],
                     ),
                     "revocations": sorted(
                         [new_attack_objects[stix_id] for stix_id in revocations],
                         key=lambda stix_object: stix_object["name"],
                     ),
                     "deprecations": sorted(
@@ -922,16 +890,15 @@
             f"""\
             ## Key
 
             * New objects: {self.section_descriptions["additions"]}
             * Major version changes: {self.section_descriptions["major_version_changes"]}
             * Minor version changes: {self.section_descriptions["minor_version_changes"]}
             * Other version changes: {self.section_descriptions["other_version_changes"]}
-            * Metadata changes: {self.section_descriptions["metadata_changes"]}
-            * Unknown changes: {self.section_descriptions["unknown_changes"]}
+            * Patches: {self.section_descriptions["patches"]}
             * Object revocations: {self.section_descriptions["revocations"]}
             * Object deprecations: {self.section_descriptions["deprecations"]}
             * Object deletions: {self.section_descriptions["deletions"]}
             """
         )
 
         return key
@@ -991,16 +958,15 @@
         logger.info("Generating ATT&CK Navigator layers")
 
         colors = {
             "additions": "#a1d99b",  # granny smith apple
             "major_version_changes": "#fcf3a2",  # yellow-ish
             "minor_version_changes": "#c7c4e0",  # light periwinkle
             "other_version_changes": "#B5E5CF",  # mint
-            "metadata_changes": "#B99095",  # mauve
-            "unknown_changes": "#3D5B59",  # teal green
+            "patches": "#B99095",  # mauve
             "deletions": "#ff00e1",  # hot magenta
             "revocations": "#ff9000",  # dark orange
             "deprecations": "#ff6363",  # bittersweet red
             "unchanged": "#ffffff",  # white
         }
 
         layers = {}
@@ -1148,15 +1114,15 @@
         if not version_increment_is_valid(old_version=None, new_version=str(object_version), section=section):
             color = red
 
     elif section == "deletions":
         color = red
 
     # nothing needs to be added to this statement - it just needs to skip the 'else' clause
-    elif section == "metadata_changes":
+    elif section == "patches":
         pass
 
     else:
         # the "previous_version" key was added in the load_data() function
         old_version = stix_object.get("previous_version")
         if not version_increment_is_valid(old_version=old_version, new_version=str(object_version), section=section):
             color = red
@@ -1229,29 +1195,88 @@
 
     if major_change or minor_change:
         return True
     return False
 
 
 def is_major_version_change(old_version: float, new_version: float) -> bool:
-    """Determine if the new version is a major change or not."""
+    """Determine if the new version is a major change."""
     next_major = float(math.floor(old_version + 1))
     if next_major == new_version:
         return True
     return False
 
 
 def is_minor_version_change(old_version: float, new_version: float) -> bool:
-    """Determine if the new version is a minor change or not."""
+    """Determine if the new version is a minor change."""
     diff = round(new_version - old_version, 1)
     if diff == 0.1:
         return True
     return False
 
 
+def is_other_version_change(old_version: float, new_version: float) -> bool:
+    """Determine if the new version is an unexpected change."""
+    next_major = float(math.floor(old_version + 1))
+    diff = round(new_version - old_version, 1)
+
+    # went up by more than 0.1, but not next major version
+    if (diff > 0.1) and (new_version != next_major):
+        return True
+    # version number went down
+    elif diff < 0:
+        return True
+
+    # either stayed the same or was a normal version change
+    return False
+
+
+def is_patch_change(old_stix_obj: dict, new_stix_obj: dict) -> bool:
+    """Determine if ATT&CK Object changes are considered a patch change.
+
+    Parameters
+    ----------
+    old_stix_obj : dict
+        Old ATT&CK STIX Domain Object (SDO).
+    new_stix_obj : dict
+        New ATT&CK STIX Domain Object (SDO).
+
+    Returns
+    -------
+    bool
+        True if the object changed in such a way as to only be considered a patch change.
+    """
+    stix_id = new_stix_obj["id"]
+    attack_id = get_attack_id(new_stix_obj)
+
+    # Version stayed the same, but the modified date changed
+    old_version = get_attack_object_version(old_stix_obj)
+    new_version = get_attack_object_version(new_stix_obj)
+    if new_version == old_version:
+        old_date = dateparser.parse(old_stix_obj["modified"])
+        new_date = dateparser.parse(new_stix_obj["modified"])
+        if new_date != old_date:
+            return True
+
+    # description changed, even though modified date didn't
+    old_lines = old_stix_obj["description"].replace("\n", " ").splitlines()
+    new_lines = new_stix_obj["description"].replace("\n", " ").splitlines()
+    old_lines_unique = [line for line in old_lines if line not in new_lines]
+    new_lines_unique = [line for line in new_lines if line not in old_lines]
+    if old_lines_unique or new_lines_unique:
+        logger.error(
+            f"{stix_id} - Somehow {attack_id} has a description change "
+            "without the version being incremented or the last modified date changing"
+        )
+        return True
+
+    # doesn't meet the definintion of a patch change
+    return False
+
+
 def get_relative_url_from_stix(stix_object: dict) -> Optional[str]:
     """Parse the website url from a stix object.
 
     Parameters
     ----------
     stix_object : dict
         An ATT&CK STIX Domain Object (SDO).
```

### Comparing `mitreattack-python-2.0.6/mitreattack/download_stix.py` & `mitreattack-python-2.0.7/mitreattack/download_stix.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/exceptions.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/filter.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/filter.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/gradient.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/gradient.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/helpers.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/layer.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/layer.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/layerobj.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/layerobj.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/layout.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/layout.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/legenditem.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/legenditem.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/metadata.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/metadata.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/objlink.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/objlink.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/technique.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/technique.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/core/versions.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/core/versions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/excel_templates.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/excel_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/fonts/monospace.ttf` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/monospace.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/fonts/sans-serif.ttf` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/sans-serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/fonts/serif.ttf` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/fonts/serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/matrix_gen.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/matrix_gen.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/svg_objects.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/svg_templates.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/svg_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/to_excel.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_excel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/exporters/to_svg.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/exporters/to_svg.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/generators/gen_helpers.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/generators/gen_helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/generators/overview_generator.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/generators/overview_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/generators/sum_generator.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/generators/sum_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/generators/usage_generator.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/generators/usage_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/layerExporter_cli.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/layerExporter_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/layerGenerator_cli.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/layerGenerator_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/navlayers/manipulators/layerops.py` & `mitreattack-python-2.0.7/mitreattack/navlayers/manipulators/layerops.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/release_info.py` & `mitreattack-python-2.0.7/mitreattack/release_info.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack/stix20/MitreAttackData.py` & `mitreattack-python-2.0.7/mitreattack/stix20/MitreAttackData.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,15 +820,15 @@
         -------
         dict
             a mapping of group_stix_id => [{'object': Software, 'relationship': Relationship}] for each software used by the group and each software used
             by campaigns attributed to the group
         """
         # return data if it has already been fetched
         if self.all_software_used_by_all_groups:
-            return self.get_all_software_used_by_all_groups
+            return self.all_software_used_by_all_groups
 
         # get all software used by groups
         tools_used_by_group = self.get_related("intrusion-set", "uses", "tool")
         malware_used_by_group = self.get_related("intrusion-set", "uses", "malware")
         software_used_by_group = self.merge(
             tools_used_by_group, malware_used_by_group
         )  # group_id -> {software, relationship}
@@ -1613,15 +1613,13 @@
 
         Returns
         -------
         object
             the object that replaced ("revoked") it
         """
         relations = self.src.relationships(revoked_stix_id, "revoked-by", source_only=True)
-        revoked_by = self.src.query(
-            [Filter("id", "in", [r.target_ref for r in relations])]
-        )
+        revoked_by = self.src.query([Filter("id", "in", [r.target_ref for r in relations])])
 
         if not revoked_by:
             return None
 
         return revoked_by[0]
```

### Comparing `mitreattack-python-2.0.6/mitreattack/stix20/custom_attack_objects.py` & `mitreattack-python-2.0.7/mitreattack/stix20/custom_attack_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack_python.egg-info/PKG-INFO` & `mitreattack-python-2.0.7/mitreattack_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 2.0.6
+Version: 2.0.7
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-2.0.6/mitreattack_python.egg-info/SOURCES.txt` & `mitreattack-python-2.0.7/mitreattack_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/mitreattack_python.egg-info/entry_points.txt` & `mitreattack-python-2.0.7/mitreattack_python.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/setup.py` & `mitreattack-python-2.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mitreattack-python",
-    version="2.0.6",
+    version="2.0.7",
     author="MITRE ATT&CK, MITRE Corporation",
     author_email="attack@mitre.org",
     description="MITRE ATT&CK python library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     maintainer="Jared Ondricek",
     maintainer_email="jondricek@mitre.org",
```

### Comparing `mitreattack-python-2.0.6/tests/test_cli.py` & `mitreattack-python-2.0.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/tests/test_collections.py` & `mitreattack-python-2.0.7/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/tests/test_layers.py` & `mitreattack-python-2.0.7/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/tests/test_mass.py` & `mitreattack-python-2.0.7/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-2.0.6/tests/test_to_excel.py` & `mitreattack-python-2.0.7/tests/test_to_excel.py`

 * *Files identical despite different names*

