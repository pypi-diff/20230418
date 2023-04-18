# Comparing `tmp/Avlos-0.5.2.tar.gz` & `tmp/Avlos-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Avlos-0.5.2.tar", last modified: Wed Mar 22 13:51:19 2023, max compression
+gzip compressed data, was "Avlos-0.5.4.tar", last modified: Tue Apr 18 14:55:49 2023, max compression
```

## Comparing `Avlos-0.5.2.tar` & `Avlos-0.5.4.tar`

### file list

```diff
@@ -1,84 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.905857 Avlos-0.5.2/
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.705381 Avlos-0.5.2/Avlos.egg-info/
--rw-rw-rw-   0        0        0      304 2023-03-22 13:51:18.000000 Avlos-0.5.2/Avlos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2023-03-22 13:51:19.000000 Avlos-0.5.2/Avlos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 13:51:18.000000 Avlos-0.5.2/Avlos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-22 13:51:19.000000 Avlos-0.5.2/Avlos.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-03-22 13:51:19.000000 Avlos-0.5.2/Avlos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-22 13:51:19.000000 Avlos-0.5.2/Avlos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5352 2022-06-27 08:09:00.000000 Avlos-0.5.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1075 2022-06-20 08:46:17.000000 Avlos-0.5.2/LICENSE
--rw-rw-rw-   0        0        0      256 2022-11-07 08:58:34.000000 Avlos-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-03-22 13:51:19.905857 Avlos-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     5693 2023-03-22 13:25:50.000000 Avlos-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.724672 Avlos-0.5.2/avlos/
--rw-rw-rw-   0        0        0       41 2022-08-30 06:44:33.000000 Avlos-0.5.2/avlos/__init__.py
--rw-rw-rw-   0        0        0      680 2022-12-02 14:51:25.000000 Avlos-0.5.2/avlos/bitmask_field.py
--rw-rw-rw-   0        0        0     1987 2022-09-27 12:00:42.000000 Avlos-0.5.2/avlos/channel.py
--rw-rw-rw-   0        0        0     1542 2022-07-18 09:26:40.000000 Avlos-0.5.2/avlos/cli.py
--rw-rw-rw-   0        0        0      741 2023-01-12 09:42:33.000000 Avlos-0.5.2/avlos/counter.py
--rw-rw-rw-   0        0        0     2779 2023-01-05 11:19:17.000000 Avlos-0.5.2/avlos/datatypes.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.736670 Avlos-0.5.2/avlos/definitions/
--rw-rw-rw-   0        0        0      423 2022-12-02 14:43:51.000000 Avlos-0.5.2/avlos/definitions/__init__.py
--rw-rw-rw-   0        0        0     1905 2023-01-09 09:55:03.000000 Avlos-0.5.2/avlos/definitions/remote_attribute.py
--rw-rw-rw-   0        0        0     2030 2023-01-04 12:38:53.000000 Avlos-0.5.2/avlos/definitions/remote_bitmask.py
--rw-rw-rw-   0        0        0     1963 2023-01-04 12:38:53.000000 Avlos-0.5.2/avlos/definitions/remote_enum.py
--rw-rw-rw-   0        0        0     2588 2022-11-29 14:20:16.000000 Avlos-0.5.2/avlos/definitions/remote_function.py
--rw-rw-rw-   0        0        0     5620 2023-01-04 12:38:53.000000 Avlos-0.5.2/avlos/definitions/remote_node.py
--rw-rw-rw-   0        0        0      858 2023-01-04 12:38:53.000000 Avlos-0.5.2/avlos/definitions/remote_root_node.py
--rw-rw-rw-   0        0        0      701 2022-06-14 06:41:54.000000 Avlos-0.5.2/avlos/deserializer.py
--rw-rw-rw-   0        0        0      670 2023-01-16 12:29:28.000000 Avlos-0.5.2/avlos/enum_field.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.746621 Avlos-0.5.2/avlos/generators/
--rw-rw-rw-   0        0        0        0 2022-05-26 11:40:29.000000 Avlos-0.5.2/avlos/generators/__init__.py
--rw-rw-rw-   0        0        0     1796 2023-01-16 12:29:28.000000 Avlos-0.5.2/avlos/generators/filters.py
--rw-rw-rw-   0        0        0     1386 2023-01-16 12:29:28.000000 Avlos-0.5.2/avlos/generators/generator_c.py
--rw-rw-rw-   0        0        0     4056 2023-02-08 14:20:24.000000 Avlos-0.5.2/avlos/generators/generator_cpp.py
--rw-rw-rw-   0        0        0      610 2022-11-29 14:21:07.000000 Avlos-0.5.2/avlos/generators/generator_dbc.py
--rw-rw-rw-   0        0        0      608 2022-11-29 14:21:14.000000 Avlos-0.5.2/avlos/generators/generator_rst.py
--rw-rw-rw-   0        0        0      341 2023-01-04 12:38:53.000000 Avlos-0.5.2/avlos/json_codec.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.767623 Avlos-0.5.2/avlos/mixins/
--rw-rw-rw-   0        0        0        0 2022-05-26 11:40:29.000000 Avlos-0.5.2/avlos/mixins/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-04 12:38:53.000000 Avlos-0.5.2/avlos/mixins/comm_node.py
--rw-rw-rw-   0        0        0     1087 2023-01-04 12:38:53.000000 Avlos-0.5.2/avlos/mixins/impex_node.py
--rw-rw-rw-   0        0        0      158 2022-11-29 14:21:03.000000 Avlos-0.5.2/avlos/mixins/meta_node.py
--rw-rw-rw-   0        0        0      640 2022-11-29 14:21:43.000000 Avlos-0.5.2/avlos/mixins/named_node.py
--rw-rw-rw-   0        0        0     1800 2022-07-18 09:26:40.000000 Avlos-0.5.2/avlos/processor.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.816619 Avlos-0.5.2/avlos/templates/
--rw-rw-rw-   0        0        0     2670 2023-01-13 14:05:01.000000 Avlos-0.5.2/avlos/templates/device.cpp.jinja
--rw-rw-rw-   0        0        0     1171 2022-12-19 14:46:36.000000 Avlos-0.5.2/avlos/templates/device.dbc.jinja
--rw-rw-rw-   0        0        0     3011 2023-01-16 12:35:23.000000 Avlos-0.5.2/avlos/templates/device.hpp.jinja
--rw-rw-rw-   0        0        0     1175 2023-03-22 13:49:03.000000 Avlos-0.5.2/avlos/templates/docs.rst.jinja
--rw-rw-rw-   0        0        0     3221 2023-01-05 14:32:35.000000 Avlos-0.5.2/avlos/templates/fw_endpoints.c.jinja
--rw-rw-rw-   0        0        0     1724 2023-01-16 12:29:28.000000 Avlos-0.5.2/avlos/templates/fw_endpoints.h.jinja
--rw-rw-rw-   0        0        0     7188 2023-03-22 13:49:03.000000 Avlos-0.5.2/avlos/templates/helpers.hpp.jinja
--rw-rw-rw-   0        0        0     3129 2023-02-08 15:01:02.000000 Avlos-0.5.2/avlos/templates/remote_object.cpp.jinja
--rw-rw-rw-   0        0        0     2117 2023-01-16 12:35:16.000000 Avlos-0.5.2/avlos/templates/remote_object.hpp.jinja
--rw-rw-rw-   0        0        0      877 2022-06-20 07:37:33.000000 Avlos-0.5.2/avlos/unit_field.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.834652 Avlos-0.5.2/example/
--rw-rw-rw-   0        0        0      153 2022-06-20 09:08:12.000000 Avlos-0.5.2/example/README.md
--rw-rw-rw-   0        0        0      341 2022-06-20 09:06:51.000000 Avlos-0.5.2/example/avlos_config.yaml
--rw-rw-rw-   0        0        0      556 2022-07-22 12:21:54.000000 Avlos-0.5.2/example/device.yaml
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.841661 Avlos-0.5.2/example/docs/
--rw-rw-rw-   0        0        0        0 2022-06-20 09:09:01.000000 Avlos-0.5.2/example/docs/index.rst
--rw-rw-rw-   0        0        0      558 2022-06-20 11:55:24.000000 Avlos-0.5.2/example/docs/protocol.rst
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.872391 Avlos-0.5.2/example/fw/
--rw-rw-rw-   0        0        0        0 2022-06-20 09:08:56.000000 Avlos-0.5.2/example/fw/main.c
--rw-rw-rw-   0        0        0     1693 2022-06-20 11:55:24.000000 Avlos-0.5.2/example/fw/protocol.c
--rw-rw-rw-   0        0        0       42 2023-03-22 13:51:19.906867 Avlos-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-03-22 13:49:03.000000 Avlos-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.894774 Avlos-0.5.2/tests/
--rw-rw-rw-   0        0        0        0 2022-06-14 06:41:54.000000 Avlos-0.5.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:51:19.904060 Avlos-0.5.2/tests/definition/
--rw-rw-rw-   0        0        0      725 2023-01-13 11:43:49.000000 Avlos-0.5.2/tests/definition/avlos_config.yaml
--rw-rw-rw-   0        0        0      413 2022-07-22 12:21:15.000000 Avlos-0.5.2/tests/definition/bad_device_bitmask.yaml
--rw-rw-rw-   0        0        0     2116 2022-07-25 07:28:21.000000 Avlos-0.5.2/tests/definition/bad_device_missing_version.yaml
--rw-rw-rw-   0        0        0      170 2022-07-22 12:21:15.000000 Avlos-0.5.2/tests/definition/bad_device_name.yaml
--rw-rw-rw-   0        0        0      303 2022-07-22 12:21:15.000000 Avlos-0.5.2/tests/definition/bad_device_unit.yaml
--rw-rw-rw-   0        0        0     2663 2023-01-16 12:29:28.000000 Avlos-0.5.2/tests/definition/good_device.yaml
--rw-rw-rw-   0        0        0      749 2022-12-19 14:46:36.000000 Avlos-0.5.2/tests/dummy_channel.py
--rw-rw-rw-   0        0        0      955 2023-01-12 09:42:06.000000 Avlos-0.5.2/tests/test_counter.py
--rw-rw-rw-   0        0        0     3007 2022-12-02 14:11:27.000000 Avlos-0.5.2/tests/test_deserialization.py
--rw-rw-rw-   0        0        0      607 2023-01-13 11:26:15.000000 Avlos-0.5.2/tests/test_functions.py
--rw-rw-rw-   0        0        0     4257 2023-01-05 10:57:25.000000 Avlos-0.5.2/tests/test_generation.py
--rw-rw-rw-   0        0        0     1030 2023-01-04 12:38:53.000000 Avlos-0.5.2/tests/test_impex.py
--rw-rw-rw-   0        0        0     3709 2023-01-16 12:29:28.000000 Avlos-0.5.2/tests/test_remote_objects.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.270426 Avlos-0.5.4/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.257436 Avlos-0.5.4/Avlos.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)      245 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1857 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       44 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       47 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        6 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/top_level.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)     5224 2022-06-25 18:06:56.000000 Avlos-0.5.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 yanconst   (501) staff       (20)     1067 2022-06-25 18:06:56.000000 Avlos-0.5.4/LICENSE
+-rw-r--r--   0 yanconst   (501) staff       (20)      247 2022-11-12 18:59:54.000000 Avlos-0.5.4/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)      245 2023-04-18 14:55:49.270274 Avlos-0.5.4/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     5674 2023-03-30 21:32:01.000000 Avlos-0.5.4/README.md
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.259503 Avlos-0.5.4/avlos/
+-rw-r--r--   0 yanconst   (501) staff       (20)       41 2022-09-09 17:01:49.000000 Avlos-0.5.4/avlos/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      656 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/bitmask_field.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1920 2022-10-02 15:27:43.000000 Avlos-0.5.4/avlos/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1490 2022-09-09 17:01:49.000000 Avlos-0.5.4/avlos/cli.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      699 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/counter.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2656 2023-01-05 20:43:17.000000 Avlos-0.5.4/avlos/datatypes.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.260681 Avlos-0.5.4/avlos/definitions/
+-rw-r--r--   0 yanconst   (501) staff       (20)      417 2022-12-03 10:33:47.000000 Avlos-0.5.4/avlos/definitions/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1842 2023-01-01 23:15:33.000000 Avlos-0.5.4/avlos/definitions/remote_attribute.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1955 2022-12-25 09:07:18.000000 Avlos-0.5.4/avlos/definitions/remote_bitmask.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1891 2023-01-13 21:25:11.000000 Avlos-0.5.4/avlos/definitions/remote_enum.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2493 2023-01-01 21:13:12.000000 Avlos-0.5.4/avlos/definitions/remote_function.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     5450 2022-12-25 09:07:04.000000 Avlos-0.5.4/avlos/definitions/remote_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      821 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/definitions/remote_root_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      679 2022-06-11 09:57:19.000000 Avlos-0.5.4/avlos/deserializer.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      649 2023-01-13 21:06:58.000000 Avlos-0.5.4/avlos/enum_field.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.261618 Avlos-0.5.4/avlos/generators/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-05-24 22:21:47.000000 Avlos-0.5.4/avlos/generators/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1730 2023-01-13 21:33:59.000000 Avlos-0.5.4/avlos/generators/filters.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1345 2023-01-13 21:34:39.000000 Avlos-0.5.4/avlos/generators/generator_c.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3945 2023-03-19 14:59:37.000000 Avlos-0.5.4/avlos/generators/generator_cpp.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      593 2022-06-14 22:21:34.000000 Avlos-0.5.4/avlos/generators/generator_dbc.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      591 2022-06-14 22:21:34.000000 Avlos-0.5.4/avlos/generators/generator_rst.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      327 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/json_codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.262635 Avlos-0.5.4/avlos/mixins/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-05-24 22:21:47.000000 Avlos-0.5.4/avlos/mixins/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      514 2023-01-01 00:32:03.000000 Avlos-0.5.4/avlos/mixins/comm_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1057 2023-01-02 13:54:26.000000 Avlos-0.5.4/avlos/mixins/impex_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      151 2022-12-03 10:33:47.000000 Avlos-0.5.4/avlos/mixins/meta_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      618 2022-10-02 15:27:43.000000 Avlos-0.5.4/avlos/mixins/named_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1757 2022-09-09 17:01:49.000000 Avlos-0.5.4/avlos/processor.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.266466 Avlos-0.5.4/avlos/templates/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2580 2023-01-13 20:26:34.000000 Avlos-0.5.4/avlos/templates/device.cpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     1147 2022-12-15 21:27:06.000000 Avlos-0.5.4/avlos/templates/device.dbc.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     2979 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/templates/device.hpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     1133 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/templates/docs.rst.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     3114 2023-01-05 20:43:17.000000 Avlos-0.5.4/avlos/templates/fw_endpoints.c.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     1657 2023-01-13 21:37:06.000000 Avlos-0.5.4/avlos/templates/fw_endpoints.h.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     7421 2023-04-18 14:43:38.000000 Avlos-0.5.4/avlos/templates/helpers.hpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     3024 2023-03-19 14:59:37.000000 Avlos-0.5.4/avlos/templates/remote_object.cpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     2115 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/templates/remote_object.hpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)      844 2022-06-25 18:06:56.000000 Avlos-0.5.4/avlos/unit_field.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.267198 Avlos-0.5.4/example/
+-rw-r--r--   0 yanconst   (501) staff       (20)      145 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/README.md
+-rw-r--r--   0 yanconst   (501) staff       (20)      328 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/avlos_config.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      536 2022-09-09 17:01:49.000000 Avlos-0.5.4/example/device.yaml
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.267353 Avlos-0.5.4/example/docs/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/docs/index.rst
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.267462 Avlos-0.5.4/example/fw/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/fw/main.c
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-18 14:55:49.270468 Avlos-0.5.4/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)      725 2023-04-18 14:43:38.000000 Avlos-0.5.4/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.269067 Avlos-0.5.4/tests/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-11 10:04:29.000000 Avlos-0.5.4/tests/__init__.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.270064 Avlos-0.5.4/tests/definition/
+-rw-r--r--   0 yanconst   (501) staff       (20)      692 2023-01-13 20:26:34.000000 Avlos-0.5.4/tests/definition/avlos_config.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      396 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_bitmask.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     2042 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_missing_version.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      162 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_name.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      290 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_unit.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     2570 2023-01-13 20:57:07.000000 Avlos-0.5.4/tests/definition/good_device.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      709 2022-12-13 21:19:54.000000 Avlos-0.5.4/tests/dummy_channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      926 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_counter.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2899 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_deserialization.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      589 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_functions.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4138 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_generation.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      977 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_impex.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3611 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_remote_objects.py
```

### Comparing `Avlos-0.5.2/Avlos.egg-info/SOURCES.txt` & `Avlos-0.5.4/Avlos.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -47,17 +47,15 @@
 avlos/templates/helpers.hpp.jinja
 avlos/templates/remote_object.cpp.jinja
 avlos/templates/remote_object.hpp.jinja
 example/README.md
 example/avlos_config.yaml
 example/device.yaml
 example/docs/index.rst
-example/docs/protocol.rst
 example/fw/main.c
-example/fw/protocol.c
 tests/__init__.py
 tests/dummy_channel.py
 tests/test_counter.py
 tests/test_deserialization.py
 tests/test_functions.py
 tests/test_generation.py
 tests/test_impex.py
```

### Comparing `Avlos-0.5.2/CODE_OF_CONDUCT.md` & `Avlos-0.5.4/CODE_OF_CONDUCT.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-# Contributor Covenant Code of Conduct
-
-## Our Pledge
-
-We as members, contributors, and leaders pledge to make participation in our
-community a harassment-free experience for everyone, regardless of age, body
-size, visible or invisible disability, ethnicity, sex characteristics, gender
-identity and expression, level of experience, education, socio-economic status,
-nationality, personal appearance, race, religion, or sexual identity
-and orientation.
-
-We pledge to act and interact in ways that contribute to an open, welcoming,
-diverse, inclusive, and healthy community.
-
-## Our Standards
-
-Examples of behavior that contributes to a positive environment for our
-community include:
-
-* Demonstrating empathy and kindness toward other people
-* Being respectful of differing opinions, viewpoints, and experiences
-* Giving and gracefully accepting constructive feedback
-* Accepting responsibility and apologizing to those affected by our mistakes,
-  and learning from the experience
-* Focusing on what is best not just for us as individuals, but for the
-  overall community
-
-Examples of unacceptable behavior include:
-
-* The use of sexualized language or imagery, and sexual attention or
-  advances of any kind
-* Trolling, insulting or derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or email
-  address, without their explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
-  professional setting
-
-## Enforcement Responsibilities
-
-Community leaders are responsible for clarifying and enforcing our standards of
-acceptable behavior and will take appropriate and fair corrective action in
-response to any behavior that they deem inappropriate, threatening, offensive,
-or harmful.
-
-Community leaders have the right and responsibility to remove, edit, or reject
-comments, commits, code, wiki edits, issues, and other contributions that are
-not aligned to this Code of Conduct, and will communicate reasons for moderation
-decisions when appropriate.
-
-## Scope
-
-This Code of Conduct applies within all community spaces, and also applies when
-an individual is officially representing the community in public spaces.
-Examples of representing our community include using an official e-mail address,
-posting via an official social media account, or acting as an appointed
-representative at an online or offline event.
-
-## Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported to the community leaders responsible for enforcement at
-community@tinymovr.com.
-All complaints will be reviewed and investigated promptly and fairly.
-
-All community leaders are obligated to respect the privacy and security of the
-reporter of any incident.
-
-## Enforcement Guidelines
-
-Community leaders will follow these Community Impact Guidelines in determining
-the consequences for any action they deem in violation of this Code of Conduct:
-
-### 1. Correction
-
-**Community Impact**: Use of inappropriate language or other behavior deemed
-unprofessional or unwelcome in the community.
-
-**Consequence**: A private, written warning from community leaders, providing
-clarity around the nature of the violation and an explanation of why the
-behavior was inappropriate. A public apology may be requested.
-
-### 2. Warning
-
-**Community Impact**: A violation through a single incident or series
-of actions.
-
-**Consequence**: A warning with consequences for continued behavior. No
-interaction with the people involved, including unsolicited interaction with
-those enforcing the Code of Conduct, for a specified period of time. This
-includes avoiding interactions in community spaces as well as external channels
-like social media. Violating these terms may lead to a temporary or
-permanent ban.
-
-### 3. Temporary Ban
-
-**Community Impact**: A serious violation of community standards, including
-sustained inappropriate behavior.
-
-**Consequence**: A temporary ban from any sort of interaction or public
-communication with the community for a specified period of time. No public or
-private interaction with the people involved, including unsolicited interaction
-with those enforcing the Code of Conduct, is allowed during this period.
-Violating these terms may lead to a permanent ban.
-
-### 4. Permanent Ban
-
-**Community Impact**: Demonstrating a pattern of violation of community
-standards, including sustained inappropriate behavior,  harassment of an
-individual, or aggression toward or disparagement of classes of individuals.
-
-**Consequence**: A permanent ban from any sort of public interaction within
-the community.
-
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage],
-version 2.0, available at
-https://www.contributor-covenant.org/version/2/0/code_of_conduct.html.
-
-Community Impact Guidelines were inspired by [Mozilla's code of conduct
-enforcement ladder](https://github.com/mozilla/diversity).
-
-[homepage]: https://www.contributor-covenant.org
-
-For answers to common questions about this code of conduct, see the FAQ at
-https://www.contributor-covenant.org/faq. Translations are available at
-https://www.contributor-covenant.org/translations.
+# Contributor Covenant Code of Conduct
+
+## Our Pledge
+
+We as members, contributors, and leaders pledge to make participation in our
+community a harassment-free experience for everyone, regardless of age, body
+size, visible or invisible disability, ethnicity, sex characteristics, gender
+identity and expression, level of experience, education, socio-economic status,
+nationality, personal appearance, race, religion, or sexual identity
+and orientation.
+
+We pledge to act and interact in ways that contribute to an open, welcoming,
+diverse, inclusive, and healthy community.
+
+## Our Standards
+
+Examples of behavior that contributes to a positive environment for our
+community include:
+
+* Demonstrating empathy and kindness toward other people
+* Being respectful of differing opinions, viewpoints, and experiences
+* Giving and gracefully accepting constructive feedback
+* Accepting responsibility and apologizing to those affected by our mistakes,
+  and learning from the experience
+* Focusing on what is best not just for us as individuals, but for the
+  overall community
+
+Examples of unacceptable behavior include:
+
+* The use of sexualized language or imagery, and sexual attention or
+  advances of any kind
+* Trolling, insulting or derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or email
+  address, without their explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+  professional setting
+
+## Enforcement Responsibilities
+
+Community leaders are responsible for clarifying and enforcing our standards of
+acceptable behavior and will take appropriate and fair corrective action in
+response to any behavior that they deem inappropriate, threatening, offensive,
+or harmful.
+
+Community leaders have the right and responsibility to remove, edit, or reject
+comments, commits, code, wiki edits, issues, and other contributions that are
+not aligned to this Code of Conduct, and will communicate reasons for moderation
+decisions when appropriate.
+
+## Scope
+
+This Code of Conduct applies within all community spaces, and also applies when
+an individual is officially representing the community in public spaces.
+Examples of representing our community include using an official e-mail address,
+posting via an official social media account, or acting as an appointed
+representative at an online or offline event.
+
+## Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behavior may be
+reported to the community leaders responsible for enforcement at
+community@tinymovr.com.
+All complaints will be reviewed and investigated promptly and fairly.
+
+All community leaders are obligated to respect the privacy and security of the
+reporter of any incident.
+
+## Enforcement Guidelines
+
+Community leaders will follow these Community Impact Guidelines in determining
+the consequences for any action they deem in violation of this Code of Conduct:
+
+### 1. Correction
+
+**Community Impact**: Use of inappropriate language or other behavior deemed
+unprofessional or unwelcome in the community.
+
+**Consequence**: A private, written warning from community leaders, providing
+clarity around the nature of the violation and an explanation of why the
+behavior was inappropriate. A public apology may be requested.
+
+### 2. Warning
+
+**Community Impact**: A violation through a single incident or series
+of actions.
+
+**Consequence**: A warning with consequences for continued behavior. No
+interaction with the people involved, including unsolicited interaction with
+those enforcing the Code of Conduct, for a specified period of time. This
+includes avoiding interactions in community spaces as well as external channels
+like social media. Violating these terms may lead to a temporary or
+permanent ban.
+
+### 3. Temporary Ban
+
+**Community Impact**: A serious violation of community standards, including
+sustained inappropriate behavior.
+
+**Consequence**: A temporary ban from any sort of interaction or public
+communication with the community for a specified period of time. No public or
+private interaction with the people involved, including unsolicited interaction
+with those enforcing the Code of Conduct, is allowed during this period.
+Violating these terms may lead to a permanent ban.
+
+### 4. Permanent Ban
+
+**Community Impact**: Demonstrating a pattern of violation of community
+standards, including sustained inappropriate behavior,  harassment of an
+individual, or aggression toward or disparagement of classes of individuals.
+
+**Consequence**: A permanent ban from any sort of public interaction within
+the community.
+
+## Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage],
+version 2.0, available at
+https://www.contributor-covenant.org/version/2/0/code_of_conduct.html.
+
+Community Impact Guidelines were inspired by [Mozilla's code of conduct
+enforcement ladder](https://github.com/mozilla/diversity).
+
+[homepage]: https://www.contributor-covenant.org
+
+For answers to common questions about this code of conduct, see the FAQ at
+https://www.contributor-covenant.org/faq. Translations are available at
+https://www.contributor-covenant.org/translations.
```

### Comparing `Avlos-0.5.2/LICENSE` & `Avlos-0.5.4/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 Ioannis Chatzikonstantinou
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+Copyright 2022 Ioannis Chatzikonstantinou
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
```

### Comparing `Avlos-0.5.2/README.md` & `Avlos-0.5.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-<p align="center">
-<img src="avlos_logo.png" width="160"/>
-</p>
-
-![main lint and test](https://github.com/tinymovr/avlos/actions/workflows/ci.yml/badge.svg) ![docs build](https://github.com/tinymovr/avlos/actions/workflows/docs.yml/badge.svg) [![Discord](https://img.shields.io/discord/742400176664084535)](https://discord.gg/CzcCaXbU)
-
-[Αυλός (Avlόs)](https://en.wikipedia.org/wiki/Aulos), _flute_, also _channel_.
-
-Avlos makes it easy to create protocol implementations to communicate with remote embedded devices.
-
-Given a remote embedded device, a client that wants to talk with the device, and a YAML file that represents the remote device structure that we want exposed to the client (the spec), Avlos will generate a protocol implementation based on the spec. It will also generate documentation and more. 
-
-<p align="center">
-<img src="docs/diagram.png" width="800"/>
-</p>
-
-Avlos has been originally developed as a communication layer for [Tinymovr](https://tinymovr.com)
-
-## :bulb: Illustrative Use Case
-
-Let's make a protocol to control a toaster. First we generate a spec file containing the structure we want the toaster to expose:
-
-    name: toaster
-    version: "1.0"
-    remote_attributes:
-    - name: sn
-        dtype: uint32
-        getter_name: toaster_get_sn
-        summary: The unique device serial number.
-    - name: heater
-      remote_attributes:
-      - name: temperature
-          dtype: float
-          unit: celsius
-          getter_name: toaster_get_heater_temp
-          summary: The toaster heater temperature.
-    - name: relay
-      remote_attributes:
-      - name: relay_state
-          dtype: bool
-          getter_name: toaster_get_relay_state
-          setter_name: toaster_set_relay_state
-          summary: The toaster heating relay element state.
-
-Given the above, Avlos can generate the following:
-
-- C implementation of the spec, to be included in the device firmware. The implementation offers data validation, (de-)serialization, getter/setter function calls, and a entry function to call with channel data. The actual comms channel implementation is left to the user.
-
-- A Python object reflecting the spec, to be used in the client. The object includes data validation, (de-)serialization, units integration and pretty presentation. The root node needs a comms channel to realize communication with a remote device.
-
-- RestructuredText-based documentation for each endpoint.
-
-- [CAN DBC file](https://www.csselectronics.com/pages/can-dbc-file-database-intro) (CAN database), for every endpoint, for use with CAN-based comm channels.
-
-In addition, Avlos will compute a checksum for the spec and add it as a variable to the implementation so that it can be retrieved by the client for comparing client and device specs. 
-
-The output location, as well as many other attributes of the files are flexible and easily configurable.
-
-## :gift: Installation
-
-    pip install avlos
-
-## :gear: Project Configuration
-
-### Device Spec
-
-The Device Spec is a YAML file that defines how the device is structured. It consists of a tree-like structure. For an example of Spec file see the [tests/definition/good_device.yaml](./tests/definition/good_device.yaml) file.
-
-### Output Config
-
-The output config defines the output modules that will be used and their options. Example, showing C code generation for embedded devices:
-
-    generators:
-        generator_c:
-            enabled: true
-            paths:
-                output_header: outputs/header.h
-                output_impl: outputs/header.c
-            header_includes:
-            - src/header.h
-            impl_includes:
-            - src/test.h
-
-## :zap: Usage
-
-Ensure a device spec and an output config exist in the current folder.
-
-    avlos from file device.yaml
-
-This will generate the outputs according to the configuration in the output config file.
-
-## Example Project
-
-A complete project example using Avlos is available at [example/](./example). Note that all the output paths defined in the output config are relative to that file. In contrast, includes are parsed as is.
-
-## :gem: Available Generators
-
-- __generator_c__: C Embedded Code
-- __generator_cpp__: C++ Client Code
-- __generator_rst__: RST-based Docs
-- __generator_dbc__: CAN Bus Database Format
-
-In addition, the object resulting from the deserialization of the spec can be used as a Python object for RPC, by supplying a channel as follows:
-
-    import yaml
-    from avlos import deserialize
-    from myProject import myChannel # update this
-    
-    device_description = ...
-    obj = deserialize(yaml.safe_load(device_description))
-    obj.set_channel(myChannel)
-
-## :memo: Various Notes
-
-### Avlos offers:
-
-- A simple straightforward tree structure description, sufficient for most device types out there
-- A flexible templating system with several built-in generators, and a simple unassuming system to extend
-- Tight integration with physical units through the Pint module.
-
-### Avlos does not offer:
-
-- An implementation of the comms channel, this is left to the user.
-- Segmentation of data into packets (this is planned)
-
-- The Avlos_Command enum is structured so as to be compatible with CAN bus RTR field (i.e. 0 -> write, 1 -> read)
-- Even though Avlos generators generate a protocol hash for both device-side (as a variable) and client-side implementations (as an object attribute), the way the hash is retrieved/checked/enforced is not included. This is due to the fact that each comms channel may implement different means of performing the above.
-
-## :key: License
-
-MIT
-
+<p align="center">
+<img src="avlos_logo.png" width="160"/>
+</p>
+
+![main lint and test](https://github.com/tinymovr/avlos/actions/workflows/ci.yml/badge.svg) ![docs build](https://github.com/tinymovr/avlos/actions/workflows/docs.yml/badge.svg) [![Discord](https://img.shields.io/discord/742400176664084535)](https://discord.gg/CzcCaXbU) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[Αυλός (Avlόs)](https://en.wikipedia.org/wiki/Aulos), _flute_, also _channel_.
+
+Avlos makes it easy to create protocol implementations to communicate with remote embedded devices.
+
+Given a remote embedded device, a client that wants to talk with the device, and a YAML file that represents the remote device structure that we want exposed to the client (the spec), Avlos will generate a protocol implementation based on the spec. It will also generate documentation and more. 
+
+<p align="center">
+<img src="docs/diagram.png" width="800"/>
+</p>
+
+Avlos has been originally developed as a communication layer for [Tinymovr](https://tinymovr.com)
+
+## :bulb: Illustrative Use Case
+
+Let's make a protocol to control a toaster. First we generate a spec file containing the structure we want the toaster to expose:
+
+    name: toaster
+    version: "1.0"
+    remote_attributes:
+    - name: sn
+        dtype: uint32
+        getter_name: toaster_get_sn
+        summary: The unique device serial number.
+    - name: heater
+      remote_attributes:
+      - name: temperature
+          dtype: float
+          unit: celsius
+          getter_name: toaster_get_heater_temp
+          summary: The toaster heater temperature.
+    - name: relay
+      remote_attributes:
+      - name: relay_state
+          dtype: bool
+          getter_name: toaster_get_relay_state
+          setter_name: toaster_set_relay_state
+          summary: The toaster heating relay element state.
+
+Given the above, Avlos can generate the following:
+
+- C implementation of the spec, to be included in the device firmware. The implementation offers data validation, (de-)serialization, getter/setter function calls, and a entry function to call with channel data. The actual comms channel implementation is left to the user.
+
+- A Python object reflecting the spec, to be used in the client. The object includes data validation, (de-)serialization, units integration and pretty presentation. The root node needs a comms channel to realize communication with a remote device.
+
+- RestructuredText-based documentation for each endpoint.
+
+- [CAN DBC file](https://www.csselectronics.com/pages/can-dbc-file-database-intro) (CAN database), for every endpoint, for use with CAN-based comm channels.
+
+In addition, Avlos will compute a checksum for the spec and add it as a variable to the implementation so that it can be retrieved by the client for comparing client and device specs. 
+
+The output location, as well as many other attributes of the files are flexible and easily configurable.
+
+## :gift: Installation
+
+    pip install avlos
+
+## :gear: Project Configuration
+
+### Device Spec
+
+The Device Spec is a YAML file that defines how the device is structured. It consists of a tree-like structure. For an example of Spec file see the [tests/definition/good_device.yaml](./tests/definition/good_device.yaml) file.
+
+### Output Config
+
+The output config defines the output modules that will be used and their options. Example, showing C code generation for embedded devices:
+
+    generators:
+        generator_c:
+            enabled: true
+            paths:
+                output_header: outputs/header.h
+                output_impl: outputs/header.c
+            header_includes:
+            - src/header.h
+            impl_includes:
+            - src/test.h
+
+## :zap: Usage
+
+Ensure a device spec and an output config exist in the current folder.
+
+    avlos from file device.yaml
+
+This will generate the outputs according to the configuration in the output config file.
+
+## Example Project
+
+A complete project example using Avlos is available at [example/](./example). Note that all the output paths defined in the output config are relative to that file. In contrast, includes are parsed as is.
+
+## :gem: Available Generators
+
+- __generator_c__: C Embedded Code
+- __generator_cpp__: C++ Client Code
+- __generator_rst__: RST-based Docs
+- __generator_dbc__: CAN Bus Database Format
+
+In addition, the object resulting from the deserialization of the spec can be used as a Python object for RPC, by supplying a channel as follows:
+
+    import yaml
+    from avlos import deserialize
+    from myProject import myChannel # update this
+    
+    device_description = ...
+    obj = deserialize(yaml.safe_load(device_description))
+    obj.set_channel(myChannel)
+
+## :memo: Various Notes
+
+### Avlos offers:
+
+- A simple straightforward tree structure description, sufficient for most device types out there
+- A flexible templating system with several built-in generators, and a simple unassuming system to extend
+- Tight integration with physical units through the Pint module.
+
+### Avlos does not offer:
+
+- An implementation of the comms channel, this is left to the user.
+- Segmentation of data into packets (this is planned)
+
+- The Avlos_Command enum is structured so as to be compatible with CAN bus RTR field (i.e. 0 -> write, 1 -> read)
+- Even though Avlos generators generate a protocol hash for both device-side (as a variable) and client-side implementations (as an object attribute), the way the hash is retrieved/checked/enforced is not included. This is due to the fact that each comms channel may implement different means of performing the above.
+
+## :key: License
+
+MIT
+
```

### Comparing `Avlos-0.5.2/avlos/bitmask_field.py` & `Avlos-0.5.4/avlos/bitmask_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-
-import enum
-from marshmallow import fields, ValidationError
-
-
-class BitmaskField(fields.Field):
-    """
-    Marshmallow Field that serializes to a string
-    and deserializes to a bitmask of flags.
-    """
-
-    def _serialize(self, value, attr, obj, **kwargs):
-        return NotImplementedError
-
-    def _deserialize(self, value, attr, data, **kwargs):
-        try:
-            assert(len(value) > 0)
-            return enum.IntFlag(attr, value)
-        except ValueError as error:
-            raise ValidationError("Invalid flags list.") from error
-        except AssertionError as error:
-            raise ValidationError("Empty flags list.") from error
+import enum
+from marshmallow import fields, ValidationError
+
+
+class BitmaskField(fields.Field):
+    """
+    Marshmallow Field that serializes to a string
+    and deserializes to a bitmask of flags.
+    """
+
+    def _serialize(self, value, attr, obj, **kwargs):
+        return NotImplementedError
+
+    def _deserialize(self, value, attr, data, **kwargs):
+        try:
+            assert len(value) > 0
+            return enum.IntFlag(attr, value)
+        except ValueError as error:
+            raise ValidationError("Invalid flags list.") from error
+        except AssertionError as error:
+            raise ValidationError("Empty flags list.") from error
```

### Comparing `Avlos-0.5.2/avlos/channel.py` & `Avlos-0.5.4/avlos/channel.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from functools import cached_property
-
-
-class BaseChannel:
-    """
-    Base Channel class to be implemented by
-    the client.
-    """
-
-    def send(self, data, ep_id):
-        """
-        Send data to endpoint ep_id. Implement this to
-        send data contained in the data byte array, to
-        the endpoint with id ep_id
-        Arguments:
-            data: a bytearray containing the data to
-                  be sent
-            ep_id: an integer representing the endpoint
-                   ID to send to
-        """
-        raise NotImplementedError
-
-    def recv(self, ep_id, timeout=0.1):
-        """
-        Receive data from endpoint ep_id. Implement this
-        to receive data from endpoint with id ep_id. The
-        implementation should timeout after a period equal
-        to timeout has elapsed.
-        Arguments:
-            ep_id: an integer representing the endpoint ID
-                   to listen to for data
-            timeout: an integer indicating a timeout for
-                     receiving any data
-        Returns:
-            A bytearray containing the received data
-        """
-        raise NotImplementedError
-
-    @cached_property
-    def max_ep_id(self):
-        """
-        Get the max value that the endpoint can get for
-        this channel.
-        Returns:
-            An integer representing the max endpoint ID
-            value
-        """
-        raise NotImplementedError
-
-    @cached_property
-    def max_packet_size(self):
-        """
-        Get the max size in bytes of the packet that this
-        channel can transmit/receive.
-        Returns:
-            An integer representing the max packet size
-        """
-        raise NotImplementedError
-
-    @cached_property
-    def serializer(self):
-        """
-        Return a data codec appropriate for this channel.
-        Returns:
-            The data codec instance
-        """
-        raise NotImplementedError
+from functools import cached_property
+
+
+class BaseChannel:
+    """
+    Base Channel class to be implemented by
+    the client.
+    """
+
+    def send(self, data, ep_id):
+        """
+        Send data to endpoint ep_id. Implement this to
+        send data contained in the data byte array, to
+        the endpoint with id ep_id
+        Arguments:
+            data: a bytearray containing the data to
+                  be sent
+            ep_id: an integer representing the endpoint
+                   ID to send to
+        """
+        raise NotImplementedError
+
+    def recv(self, ep_id, timeout=0.1):
+        """
+        Receive data from endpoint ep_id. Implement this
+        to receive data from endpoint with id ep_id. The
+        implementation should timeout after a period equal
+        to timeout has elapsed.
+        Arguments:
+            ep_id: an integer representing the endpoint ID
+                   to listen to for data
+            timeout: an integer indicating a timeout for
+                     receiving any data
+        Returns:
+            A bytearray containing the received data
+        """
+        raise NotImplementedError
+
+    @cached_property
+    def max_ep_id(self):
+        """
+        Get the max value that the endpoint can get for
+        this channel.
+        Returns:
+            An integer representing the max endpoint ID
+            value
+        """
+        raise NotImplementedError
+
+    @cached_property
+    def max_packet_size(self):
+        """
+        Get the max size in bytes of the packet that this
+        channel can transmit/receive.
+        Returns:
+            An integer representing the max packet size
+        """
+        raise NotImplementedError
+
+    @cached_property
+    def serializer(self):
+        """
+        Return a data codec appropriate for this channel.
+        Returns:
+            The data codec instance
+        """
+        raise NotImplementedError
```

### Comparing `Avlos-0.5.2/avlos/definitions/remote_attribute.py` & `Avlos-0.5.4/avlos/definitions/remote_function.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,95 @@
-from avlos import get_registry
-from avlos.mixins.comm_node import CommNode
-from avlos.mixins.named_node import NamedNode
-from avlos.mixins.meta_node import MetaNode
-from avlos.mixins.impex_node import ImpexNode
-
-
-class RemoteAttribute(CommNode, NamedNode, MetaNode, ImpexNode):
-    """
-    Remote Endpoint with a value, parent and a comms channel
-    """
-
-    def __init__(
-        self,
-        name,
-        summary,
-        dtype,
-        getter_name=None,
-        setter_name=None,
-        unit=None,
-        rst_target=None,
-        ep_id=-1,
-        meta={},
-    ):
-        CommNode.__init__(self)
-        NamedNode.__init__(self, name)
-        MetaNode.__init__(self, meta_dict=meta)
-        self.summary = summary
-        self.dtype = dtype
-        self.unit = unit
-        self.getter_name = getter_name
-        self.setter_name = setter_name
-        self.rst_target = rst_target
-        self.ep_id = ep_id
-
-    def get_value(self):
-        assert self.getter_name, "No getter function available"
-        self.channel.send([], self.ep_id)
-        data = self.channel.recv(self.ep_id)
-        value, *_ = self.channel.serializer.deserialize(data, self.dtype)
-        try:
-            return value * self.unit
-        except TypeError:
-            return value
-
-    def set_value(self, val):
-        assert self.setter_name, "No setter function available"
-        try:
-            val = val.to(self.unit).magnitude
-        except AttributeError:
-            pass
-        data = self.channel.serializer.serialize([val], self.dtype)
-        self.channel.send(data, self.ep_id)
-
-    def set_value_with_string(self, str_val):
-        self.set_value(get_registry()(str_val))
-
-    def str_dump(self):
-        return "{0} [{1}]: {2:.6g}".format(
-            self.name,
-            self.dtype.nickname,
-            self.get_value(),
-        )
+from marshmallow import (
+    Schema,
+    fields,
+    post_load,
+)
+from avlos.unit_field import UnitField
+from avlos.datatypes import DataTypeField
+from avlos.mixins.comm_node import CommNode
+from avlos.mixins.named_node import NamedNode
+from avlos.mixins.meta_node import MetaNode
+
+
+class RemoteFunction(CommNode, NamedNode, MetaNode):
+    """
+    Remote Function with zero or more arguments, return
+    type, parent and a comms channel
+    """
+
+    def __init__(
+        self,
+        name,
+        summary,
+        caller_name,
+        arguments,
+        dtype=None,
+        unit=None,
+        rst_target=None,
+        ep_id=-1,
+        meta={},
+    ):
+        CommNode.__init__(self)
+        NamedNode.__init__(self, name)
+        MetaNode.__init__(self, meta_dict=meta)
+        self.summary = summary
+        self.dtype = dtype
+        self.unit = unit
+        self.caller_name = caller_name
+        self.arguments = arguments
+        self.rst_target = rst_target
+        self.ep_id = ep_id
+
+    def __call__(self, *args):
+        data = self.channel.serializer.serialize(
+            args, *[arg.dtype for arg in self.arguments]
+        )
+        self.channel.send(data, self.ep_id)
+        if not self.dtype.is_void:
+            data = self.channel.recv(self.ep_id)
+            value, *_ = self.channel.serializer.deserialize(data, self.dtype)
+            try:
+                return value * self.unit
+            except TypeError:
+                pass
+            return value
+
+    def str_dump(self):
+        return "{}({}) -> {}".format(
+            self.name,
+            ", ".join([arg.as_function_argument for arg in self.arguments]),
+            self.dtype.nickname,
+        )
+
+
+class RemoteArgument:
+    """
+    Class representing a RemoteFunction argument
+    """
+
+    def __init__(self, name, dtype, unit=None, summary=None):
+        self.name = name
+        self.dtype = dtype
+        self.unit = unit
+        self.summary = summary
+
+    @property
+    def as_function_argument(self):
+        return " ".join([self.dtype.nickname, self.name])
+
+
+class RemoteArgumentSchema(Schema):
+    """
+    Custom Marshmallow schema for generating RemoteFunction
+    arguments
+    """
+
+    name = fields.String(
+        required=True, error_messages={"required": "Name is required."}
+    )
+    summary = fields.String()
+    dtype = DataTypeField(required=True)
+    unit = UnitField()
+
+    @post_load
+    def make_remote_argument(self, data, **kwargs):
+        return RemoteArgument(**data)
```

### Comparing `Avlos-0.5.2/avlos/definitions/remote_node.py` & `Avlos-0.5.4/avlos/definitions/remote_node.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-from collections import OrderedDict
-from marshmallow import (
-    Schema,
-    fields,
-    post_load,
-    validates_schema,
-    ValidationError,
-)
-from avlos.unit_field import UnitField
-from avlos.bitmask_field import BitmaskField
-from avlos.enum_field import EnumField
-from avlos.counter import get_counter
-from avlos.datatypes import DataTypeField
-from avlos.mixins.comm_node import CommNode
-from avlos.mixins.named_node import NamedNode
-from avlos.mixins.impex_node import ImpexNode
-from avlos.definitions import (
-    RemoteAttribute,
-    RemoteFunction,
-    RemoteArgumentSchema,
-    RemoteBitmask,
-    RemoteEnum,
-)
-
-
-class RemoteNode(CommNode, NamedNode, ImpexNode):
-    """
-    Remote node with parent, children and a comms channel
-    """
-
-    def __init__(self, remote_attributes, name, summary=None):
-        od = OrderedDict()
-        for attrib in remote_attributes:
-            od[attrib.name] = attrib
-        super().__setattr__("remote_attributes", od)
-        CommNode.__init__(self)
-        NamedNode.__init__(self, name)
-        self.summary = summary
-
-    def __getattr__(self, __name):
-        try:
-            attr = self.remote_attributes[__name]
-            try:
-                return attr.get_value()
-            except AttributeError:
-                return attr
-        except KeyError:
-            raise AttributeError(__name)
-
-    def __setattr__(self, __name, __value):
-        try:
-            attr = self.remote_attributes[__name]
-            if isinstance(attr, RemoteAttribute):
-                return attr.set_value(__value)
-        except KeyError:
-            super().__setattr__(__name, __value)
-
-    def export_flags(self, namespace):
-        """
-        Recurse children and export bitmask to
-        indicated namespace
-        """
-        for child in self.remote_attributes:
-            try:
-                child.export_flags(namespace)
-            except AttributeError:
-                pass
-
-    def str_dump(self, indent, depth):
-        if depth <= 0:
-            return "..."
-        lines = []
-        for key, val in self.remote_attributes.items():
-            if isinstance(val, RemoteNode):
-                val_str = (
-                    indent
-                    + key
-                    + (": " if depth == 1 else ":\n")
-                    + val.str_dump(indent + "  ", depth - 1)
-                )
-            else:
-                val_str = indent + val.str_dump()
-            lines.append(val_str)
-        return "\n".join(lines)
-
-    def __str__(self):
-        return self.str_dump("", depth=2)
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __dir__(self):
-        return self.remote_attributes.keys()
-
-
-class RemoteNodeSchema(Schema):
-    """
-    Custom Marshmallow schema for generating RemoteNode,
-    RemoteAttribute, RemoteBitmask and RemoteFunction classes
-    """
-
-    name = fields.String(
-        required=True, error_messages={"required": "Name is required."}
-    )
-    summary = fields.String()
-    remote_attributes = fields.List(fields.Nested(lambda: RemoteNodeSchema()))
-    dtype = DataTypeField()
-    flags = BitmaskField()
-    options = EnumField()
-    unit = UnitField()
-    getter_name = fields.String()
-    setter_name = fields.String()
-    caller_name = fields.String()
-    arguments = fields.List(fields.Nested(lambda: RemoteArgumentSchema()))
-    export = fields.Bool(default=False)
-    rst_target = fields.String()
-    ep_id = fields.Integer(default=-1)
-    meta = fields.Dict(default={})
-
-    def __init__(self, *args, **kwargs):
-        self.counter = get_counter()
-        super().__init__(*args, **kwargs)
-
-    @post_load
-    def make_remote_node(self, data, **kwargs):
-        """
-        Decide on which type of object to instantiate
-        based on the initialization data available.
-        Overrides the post_load hook.
-        """
-        if "remote_attributes" in data:
-            node = RemoteNode(**data)
-            for child in node.remote_attributes.values():
-                child._parent = node
-            return node
-        elif "caller_name" in data:
-            data["ep_id"] = self.counter.next()
-            return RemoteFunction(**data)
-        elif "dtype" in data:
-            data["ep_id"] = self.counter.next()
-            return RemoteAttribute(**data)
-        elif "flags" in data:
-            data["ep_id"] = self.counter.next()
-            return RemoteBitmask(**data)
-        elif "options" in data:
-            data["ep_id"] = self.counter.next()
-            return RemoteEnum(**data)
-
-    @validates_schema
-    def validate_schema(self, data, **kwargs):
-        if (
-            "remote_attributes" not in data
-            and "getter_name" not in data
-            and "setter_name" not in data
-            and "caller_name" not in data
-        ):
-            raise ValidationError(
-                "Either a getter, setter, caller or remote attributes list is required"
-            )
-        if "getter_name" in data and "setter_name" in data and "caller_name" in data:
-            raise ValidationError(
-                "A getter, setter, and caller cannot coexist in a single endpoint"
-            )
-        if (
-            ("getter_name" in data or "setter_name" in data or "caller_name" in data)
-            and "dtype" not in data
-            and "flags" not in data
-            and "options" not in data
-        ):
-            raise ValidationError("Data type, flags or options field is required")
+from collections import OrderedDict
+from marshmallow import (
+    Schema,
+    fields,
+    post_load,
+    validates_schema,
+    ValidationError,
+)
+from avlos.unit_field import UnitField
+from avlos.bitmask_field import BitmaskField
+from avlos.enum_field import EnumField
+from avlos.counter import get_counter
+from avlos.datatypes import DataTypeField
+from avlos.mixins.comm_node import CommNode
+from avlos.mixins.named_node import NamedNode
+from avlos.mixins.impex_node import ImpexNode
+from avlos.definitions import (
+    RemoteAttribute,
+    RemoteFunction,
+    RemoteArgumentSchema,
+    RemoteBitmask,
+    RemoteEnum,
+)
+
+
+class RemoteNode(CommNode, NamedNode, ImpexNode):
+    """
+    Remote node with parent, children and a comms channel
+    """
+
+    def __init__(self, remote_attributes, name, summary=None):
+        od = OrderedDict()
+        for attrib in remote_attributes:
+            od[attrib.name] = attrib
+        super().__setattr__("remote_attributes", od)
+        CommNode.__init__(self)
+        NamedNode.__init__(self, name)
+        self.summary = summary
+
+    def __getattr__(self, __name):
+        try:
+            attr = self.remote_attributes[__name]
+            try:
+                return attr.get_value()
+            except AttributeError:
+                return attr
+        except KeyError:
+            raise AttributeError(__name)
+
+    def __setattr__(self, __name, __value):
+        try:
+            attr = self.remote_attributes[__name]
+            if isinstance(attr, RemoteAttribute):
+                return attr.set_value(__value)
+        except KeyError:
+            super().__setattr__(__name, __value)
+
+    def export_flags(self, namespace):
+        """
+        Recurse children and export bitmask to
+        indicated namespace
+        """
+        for child in self.remote_attributes:
+            try:
+                child.export_flags(namespace)
+            except AttributeError:
+                pass
+
+    def str_dump(self, indent, depth):
+        if depth <= 0:
+            return "..."
+        lines = []
+        for key, val in self.remote_attributes.items():
+            if isinstance(val, RemoteNode):
+                val_str = (
+                    indent
+                    + key
+                    + (": " if depth == 1 else ":\n")
+                    + val.str_dump(indent + "  ", depth - 1)
+                )
+            else:
+                val_str = indent + val.str_dump()
+            lines.append(val_str)
+        return "\n".join(lines)
+
+    def __str__(self):
+        return self.str_dump("", depth=2)
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __dir__(self):
+        return self.remote_attributes.keys()
+
+
+class RemoteNodeSchema(Schema):
+    """
+    Custom Marshmallow schema for generating RemoteNode,
+    RemoteAttribute, RemoteBitmask and RemoteFunction classes
+    """
+
+    name = fields.String(
+        required=True, error_messages={"required": "Name is required."}
+    )
+    summary = fields.String()
+    remote_attributes = fields.List(fields.Nested(lambda: RemoteNodeSchema()))
+    dtype = DataTypeField()
+    flags = BitmaskField()
+    options = EnumField()
+    unit = UnitField()
+    getter_name = fields.String()
+    setter_name = fields.String()
+    caller_name = fields.String()
+    arguments = fields.List(fields.Nested(lambda: RemoteArgumentSchema()))
+    export = fields.Bool(default=False)
+    rst_target = fields.String()
+    ep_id = fields.Integer(default=-1)
+    meta = fields.Dict(default={})
+
+    def __init__(self, *args, **kwargs):
+        self.counter = get_counter()
+        super().__init__(*args, **kwargs)
+
+    @post_load
+    def make_remote_node(self, data, **kwargs):
+        """
+        Decide on which type of object to instantiate
+        based on the initialization data available.
+        Overrides the post_load hook.
+        """
+        if "remote_attributes" in data:
+            node = RemoteNode(**data)
+            for child in node.remote_attributes.values():
+                child._parent = node
+            return node
+        elif "caller_name" in data:
+            data["ep_id"] = self.counter.next()
+            return RemoteFunction(**data)
+        elif "dtype" in data:
+            data["ep_id"] = self.counter.next()
+            return RemoteAttribute(**data)
+        elif "flags" in data:
+            data["ep_id"] = self.counter.next()
+            return RemoteBitmask(**data)
+        elif "options" in data:
+            data["ep_id"] = self.counter.next()
+            return RemoteEnum(**data)
+
+    @validates_schema
+    def validate_schema(self, data, **kwargs):
+        if (
+            "remote_attributes" not in data
+            and "getter_name" not in data
+            and "setter_name" not in data
+            and "caller_name" not in data
+        ):
+            raise ValidationError(
+                "Either a getter, setter, caller or remote attributes list is required"
+            )
+        if "getter_name" in data and "setter_name" in data and "caller_name" in data:
+            raise ValidationError(
+                "A getter, setter, and caller cannot coexist in a single endpoint"
+            )
+        if (
+            ("getter_name" in data or "setter_name" in data or "caller_name" in data)
+            and "dtype" not in data
+            and "flags" not in data
+            and "options" not in data
+        ):
+            raise ValidationError("Data type, flags or options field is required")
```

### Comparing `Avlos-0.5.2/avlos/definitions/remote_root_node.py` & `Avlos-0.5.4/avlos/definitions/remote_root_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from functools import cached_property
-from marshmallow import fields, post_load
-from avlos.definitions import RemoteNode, RemoteNodeSchema
-
-
-class RootNode(RemoteNode):
-    """
-    Remote root node with a few additional attributes
-    """
-
-    def __init__(self, version, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.version = version
-    
-    @cached_property
-    def root(self):
-        return self
-
-
-class RootNodeSchema(RemoteNodeSchema):
-    """
-    Custom Marshmallow schema for the root node
-    """
-
-    version = fields.String()
-
-    @post_load
-    def make_remote_node(self, data, **kwargs):
-        if "remote_attributes" in data:
-            node = RootNode(**data)
-            for child in node.remote_attributes.values():
-                child._parent = node
-            return node
+from functools import cached_property
+from marshmallow import fields, post_load
+from avlos.definitions import RemoteNode, RemoteNodeSchema
+
+
+class RootNode(RemoteNode):
+    """
+    Remote root node with a few additional attributes
+    """
+
+    def __init__(self, version, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.version = version
+
+    @cached_property
+    def root(self):
+        return self
+
+
+class RootNodeSchema(RemoteNodeSchema):
+    """
+    Custom Marshmallow schema for the root node
+    """
+
+    version = fields.String()
+
+    @post_load
+    def make_remote_node(self, data, **kwargs):
+        if "remote_attributes" in data:
+            node = RootNode(**data)
+            for child in node.remote_attributes.values():
+                child._parent = node
+            return node
```

### Comparing `Avlos-0.5.2/avlos/deserializer.py` & `Avlos-0.5.4/avlos/deserializer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import json
-import hashlib
-from avlos.definitions import RootNodeSchema
-from avlos.counter import make_counter
-
-
-def deserialize(device_description):
-    make_counter()
-    device_schema = RootNodeSchema()
-    device_obj = device_schema.load(device_description)
-    dev_desc = json.dumps(device_description)
-    device_obj.hash_string = hash_string_from_string(dev_desc)
-    device_obj.hash_uint32 = hash_int_from_string(dev_desc)
-    return device_obj
-
-
-def hash_string_from_string(input_string):
-    return hex(hash_int_from_string(input_string))
-
-
-def hash_int_from_string(input_string):
-    return int.from_bytes(hashlib.sha256(input_string.encode()).digest()[:4], "little")
+import json
+import hashlib
+from avlos.definitions import RootNodeSchema
+from avlos.counter import make_counter
+
+
+def deserialize(device_description):
+    make_counter()
+    device_schema = RootNodeSchema()
+    device_obj = device_schema.load(device_description)
+    dev_desc = json.dumps(device_description)
+    device_obj.hash_string = hash_string_from_string(dev_desc)
+    device_obj.hash_uint32 = hash_int_from_string(dev_desc)
+    return device_obj
+
+
+def hash_string_from_string(input_string):
+    return hex(hash_int_from_string(input_string))
+
+
+def hash_int_from_string(input_string):
+    return int.from_bytes(hashlib.sha256(input_string.encode()).digest()[:4], "little")
```

### Comparing `Avlos-0.5.2/avlos/enum_field.py` & `Avlos-0.5.4/avlos/enum_field.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import enum
-from marshmallow import fields, ValidationError
-
-
-class EnumField(fields.Field):
-    """
-    Marshmallow Field that serializes to a string
-    and deserializes to an enum.
-    """
-
-    def _serialize(self, value, attr, obj, **kwargs):
-        return NotImplementedError
-
-    def _deserialize(self, value, attr, data, **kwargs):
-        try:
-            assert len(value) > 0
-            return enum.IntEnum(attr, value, start=0)
-        except ValueError as error:
-            raise ValidationError("Invalid enum list.") from error
-        except AssertionError as error:
-            raise ValidationError("Empty enum list.") from error
+import enum
+from marshmallow import fields, ValidationError
+
+
+class EnumField(fields.Field):
+    """
+    Marshmallow Field that serializes to a string
+    and deserializes to an enum.
+    """
+
+    def _serialize(self, value, attr, obj, **kwargs):
+        return NotImplementedError
+
+    def _deserialize(self, value, attr, data, **kwargs):
+        try:
+            assert len(value) > 0
+            return enum.IntEnum(attr, value, start=0)
+        except ValueError as error:
+            raise ValidationError("Invalid enum list.") from error
+        except AssertionError as error:
+            raise ValidationError("Empty enum list.") from error
```

### Comparing `Avlos-0.5.2/avlos/generators/filters.py` & `Avlos-0.5.4/avlos/generators/filters.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import os
-from copy import copy
-
-
-def avlos_endpoints(input):
-    """
-    Traverse remote dictionary and return list
-    of remote endpoints
-    """
-
-    def traverse_endpoint_list(ep_list, ep_out_list):
-        for ep in ep_list:
-            if (
-                hasattr(ep, "getter_name")
-                or hasattr(ep, "setter_name")
-                or hasattr(ep, "caller_name")
-            ):
-                ep_out_list.append(ep)
-            elif hasattr(ep, "remote_attributes"):
-                traverse_endpoint_list(ep.remote_attributes.values(), ep_out_list)
-
-    ep_out_list = []
-    if hasattr(input, "remote_attributes"):
-        traverse_endpoint_list(input.remote_attributes.values(), ep_out_list)
-    return ep_out_list
-
-
-def avlos_enum_eps(input):
-    """
-    Traverse remote dictionary and return a list of enum type endpoints
-    """
-    return [ep for ep in avlos_endpoints(input) if hasattr(ep, "options")]
-
-
-def avlos_bitmask_eps(input):
-    """
-    Traverse remote dictionary and return a list of bitmask type endpoints
-    """
-    return [ep for ep in avlos_endpoints(input) if hasattr(ep, "bitmask")]
-
-
-def as_include(input):
-    """
-    Render a string as a C include, with opening
-    and closing braces or quotation marks
-    """
-    if input.startswith('"') and input.endswith('"'):
-        return input
-    elif input.startswith("<") and input.endswith(">"):
-        return input
-    return "<" + input + ">"
-
-
-def file_from_path(input):
-    """
-    Get the file string from a path string
-    """
-    return os.path.basename(input)
-
-
-def capitalize_first(input):
-    """
-    Capitalize the first character of a
-    string, leaving the rest unchanged
-    """
-    return input[0].upper() + input[1:]
+import os
+from copy import copy
+
+
+def avlos_endpoints(input):
+    """
+    Traverse remote dictionary and return list
+    of remote endpoints
+    """
+
+    def traverse_endpoint_list(ep_list, ep_out_list):
+        for ep in ep_list:
+            if (
+                hasattr(ep, "getter_name")
+                or hasattr(ep, "setter_name")
+                or hasattr(ep, "caller_name")
+            ):
+                ep_out_list.append(ep)
+            elif hasattr(ep, "remote_attributes"):
+                traverse_endpoint_list(ep.remote_attributes.values(), ep_out_list)
+
+    ep_out_list = []
+    if hasattr(input, "remote_attributes"):
+        traverse_endpoint_list(input.remote_attributes.values(), ep_out_list)
+    return ep_out_list
+
+
+def avlos_enum_eps(input):
+    """
+    Traverse remote dictionary and return a list of enum type endpoints
+    """
+    return [ep for ep in avlos_endpoints(input) if hasattr(ep, "options")]
+
+
+def avlos_bitmask_eps(input):
+    """
+    Traverse remote dictionary and return a list of bitmask type endpoints
+    """
+    return [ep for ep in avlos_endpoints(input) if hasattr(ep, "bitmask")]
+
+
+def as_include(input):
+    """
+    Render a string as a C include, with opening
+    and closing braces or quotation marks
+    """
+    if input.startswith('"') and input.endswith('"'):
+        return input
+    elif input.startswith("<") and input.endswith(">"):
+        return input
+    return "<" + input + ">"
+
+
+def file_from_path(input):
+    """
+    Get the file string from a path string
+    """
+    return os.path.basename(input)
+
+
+def capitalize_first(input):
+    """
+    Capitalize the first character of a
+    string, leaving the rest unchanged
+    """
+    return input[0].upper() + input[1:]
```

### Comparing `Avlos-0.5.2/avlos/generators/generator_c.py` & `Avlos-0.5.4/avlos/generators/generator_c.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import os
-from jinja2 import Environment, PackageLoader, select_autoescape
-from avlos.generators.filters import (
-    avlos_endpoints,
-    avlos_enum_eps,
-    avlos_bitmask_eps,
-    as_include,
-)
-
-env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
-
-
-def process(instance, config):
-    env.filters["endpoints"] = avlos_endpoints
-    env.filters["enum_eps"] = avlos_enum_eps
-    env.filters["bitmask_eps"] = avlos_bitmask_eps
-    env.filters["as_include"] = as_include
-
-    template = env.get_template("fw_endpoints.h.jinja")
-    try:
-        includes = config["header_includes"]
-    except KeyError:
-        includes = []
-    os.makedirs(os.path.dirname(config["paths"]["output_header"]), exist_ok=True)
-    with open(config["paths"]["output_header"], "w") as output_file:
-        print(
-            template.render(instance=instance, includes=includes),
-            file=output_file,
-        )
-
-    template = env.get_template("fw_endpoints.c.jinja")
-    try:
-        includes = config["impl_includes"]
-    except KeyError:
-        includes = []
-    os.makedirs(os.path.dirname(config["paths"]["output_impl"]), exist_ok=True)
-    with open(config["paths"]["output_impl"], "w") as output_file:
-        print(
-            template.render(instance=instance, includes=includes),
-            file=output_file,
-        )
+import os
+from jinja2 import Environment, PackageLoader, select_autoescape
+from avlos.generators.filters import (
+    avlos_endpoints,
+    avlos_enum_eps,
+    avlos_bitmask_eps,
+    as_include,
+)
+
+env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
+
+
+def process(instance, config):
+    env.filters["endpoints"] = avlos_endpoints
+    env.filters["enum_eps"] = avlos_enum_eps
+    env.filters["bitmask_eps"] = avlos_bitmask_eps
+    env.filters["as_include"] = as_include
+
+    template = env.get_template("fw_endpoints.h.jinja")
+    try:
+        includes = config["header_includes"]
+    except KeyError:
+        includes = []
+    os.makedirs(os.path.dirname(config["paths"]["output_header"]), exist_ok=True)
+    with open(config["paths"]["output_header"], "w") as output_file:
+        print(
+            template.render(instance=instance, includes=includes),
+            file=output_file,
+        )
+
+    template = env.get_template("fw_endpoints.c.jinja")
+    try:
+        includes = config["impl_includes"]
+    except KeyError:
+        includes = []
+    os.makedirs(os.path.dirname(config["paths"]["output_impl"]), exist_ok=True)
+    with open(config["paths"]["output_impl"], "w") as output_file:
+        print(
+            template.render(instance=instance, includes=includes),
+            file=output_file,
+        )
```

### Comparing `Avlos-0.5.2/avlos/generators/generator_cpp.py` & `Avlos-0.5.4/avlos/generators/generator_cpp.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import os
-from pathlib import Path
-from jinja2 import Environment, PackageLoader, select_autoescape
-from avlos.generators.filters import (
-    avlos_enum_eps,
-    avlos_bitmask_eps,
-    file_from_path,
-    capitalize_first,
-)
-
-env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
-
-
-def process(instance, config):
-    env.filters["enum_eps"] = avlos_enum_eps
-    env.filters["bitmask_eps"] = avlos_bitmask_eps
-    env.filters["file_from_path"] = file_from_path
-    env.filters["capitalize_first"] = capitalize_first
-    process_helpers(instance, config)
-    process_header(instance, config)
-    process_impl(instance, config)
-
-
-def process_helpers(instance, config):
-    template = env.get_template("helpers.hpp.jinja")
-    file_path = config["paths"]["output_helpers"]
-    os.makedirs(os.path.dirname(config["paths"]["output_helpers"]), exist_ok=True)
-    with open(file_path, "w") as output_file:
-        print(
-            template.render(instance=instance),
-            file=output_file,
-        )
-
-
-def process_header(instance, config):
-    template = env.get_template("device.hpp.jinja")
-    file_path = config["paths"]["output_header"]
-    helper_file = config["paths"]["output_helpers"]
-    try:
-        includes = config["header_includes"]
-    except KeyError:
-        includes = []
-    os.makedirs(os.path.dirname(config["paths"]["output_header"]), exist_ok=True)
-    with open(file_path, "w") as output_file:
-        print(
-            template.render(
-                instance=instance,
-                includes=includes,
-                helper_file=helper_file,
-                device_name=Path(config["paths"]["output_header"]).stem,
-            ),
-            file=output_file,
-        )
-    for attr in instance.remote_attributes.values():
-        if hasattr(attr, "remote_attributes"):
-            recurse_header(attr, config)
-
-
-def recurse_header(remote_object, config):
-    template = env.get_template("remote_object.hpp.jinja")
-    file_path = os.path.join(
-        os.path.dirname(config["paths"]["output_header"]),
-        remote_object.name + ".hpp",
-    )
-    helper_file = config["paths"]["output_helpers"]
-    os.makedirs(os.path.dirname(config["paths"]["output_header"]), exist_ok=True)
-    with open(file_path, "w") as output_file:
-        print(
-            template.render(instance=remote_object, helper_file=helper_file),
-            file=output_file,
-        )
-    for attr in remote_object.remote_attributes.values():
-        if hasattr(attr, "remote_attributes"):
-            recurse_header(attr, config)
-
-
-def process_impl(instance, config):
-    template = env.get_template("device.cpp.jinja")
-    file_path = config["paths"]["output_impl"]
-    try:
-        includes = config["impl_includes"]
-    except KeyError:
-        includes = []
-    includes.append(Path(config["paths"]["output_header"]).name)
-    os.makedirs(os.path.dirname(config["paths"]["output_impl"]), exist_ok=True)
-    with open(file_path, "w") as output_file:
-        print(
-            template.render(
-                instance=instance,
-                includes=includes,
-                device_name=Path(config["paths"]["output_header"]).stem,
-            ),
-            file=output_file,
-        )
-    for attr in instance.remote_attributes.values():
-        if hasattr(attr, "remote_attributes"):
-            recurse_impl(attr, config)
-
-
-def recurse_impl(remote_object, config):
-    template = env.get_template("remote_object.cpp.jinja")
-    file_path = os.path.join(
-        os.path.dirname(config["paths"]["output_impl"]),
-        remote_object.name + ".cpp",
-    )
-    os.makedirs(os.path.dirname(config["paths"]["output_impl"]), exist_ok=True)
-    with open(file_path, "w") as output_file:
-        print(template.render(instance=remote_object), file=output_file)
-    for attr in remote_object.remote_attributes.values():
-        if hasattr(attr, "remote_attributes"):
-            recurse_impl(attr, config)
+import os
+from pathlib import Path
+from jinja2 import Environment, PackageLoader, select_autoescape
+from avlos.generators.filters import (
+    avlos_enum_eps,
+    avlos_bitmask_eps,
+    file_from_path,
+    capitalize_first,
+)
+
+env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
+
+
+def process(instance, config):
+    env.filters["enum_eps"] = avlos_enum_eps
+    env.filters["bitmask_eps"] = avlos_bitmask_eps
+    env.filters["file_from_path"] = file_from_path
+    env.filters["capitalize_first"] = capitalize_first
+    process_helpers(instance, config)
+    process_header(instance, config)
+    process_impl(instance, config)
+
+
+def process_helpers(instance, config):
+    template = env.get_template("helpers.hpp.jinja")
+    file_path = config["paths"]["output_helpers"]
+    os.makedirs(os.path.dirname(config["paths"]["output_helpers"]), exist_ok=True)
+    with open(file_path, "w") as output_file:
+        print(
+            template.render(instance=instance),
+            file=output_file,
+        )
+
+
+def process_header(instance, config):
+    template = env.get_template("device.hpp.jinja")
+    file_path = config["paths"]["output_header"]
+    helper_file = config["paths"]["output_helpers"]
+    try:
+        includes = config["header_includes"]
+    except KeyError:
+        includes = []
+    os.makedirs(os.path.dirname(config["paths"]["output_header"]), exist_ok=True)
+    with open(file_path, "w") as output_file:
+        print(
+            template.render(
+                instance=instance,
+                includes=includes,
+                helper_file=helper_file,
+                device_name=Path(config["paths"]["output_header"]).stem,
+            ),
+            file=output_file,
+        )
+    for attr in instance.remote_attributes.values():
+        if hasattr(attr, "remote_attributes"):
+            recurse_header(attr, config)
+
+
+def recurse_header(remote_object, config):
+    template = env.get_template("remote_object.hpp.jinja")
+    file_path = os.path.join(
+        os.path.dirname(config["paths"]["output_header"]),
+        remote_object.name + ".hpp",
+    )
+    helper_file = config["paths"]["output_helpers"]
+    os.makedirs(os.path.dirname(config["paths"]["output_header"]), exist_ok=True)
+    with open(file_path, "w") as output_file:
+        print(
+            template.render(instance=remote_object, helper_file=helper_file),
+            file=output_file,
+        )
+    for attr in remote_object.remote_attributes.values():
+        if hasattr(attr, "remote_attributes"):
+            recurse_header(attr, config)
+
+
+def process_impl(instance, config):
+    template = env.get_template("device.cpp.jinja")
+    file_path = config["paths"]["output_impl"]
+    try:
+        includes = config["impl_includes"]
+    except KeyError:
+        includes = []
+    includes.append(Path(config["paths"]["output_header"]).name)
+    os.makedirs(os.path.dirname(config["paths"]["output_impl"]), exist_ok=True)
+    with open(file_path, "w") as output_file:
+        print(
+            template.render(
+                instance=instance,
+                includes=includes,
+                device_name=Path(config["paths"]["output_header"]).stem,
+            ),
+            file=output_file,
+        )
+    for attr in instance.remote_attributes.values():
+        if hasattr(attr, "remote_attributes"):
+            recurse_impl(attr, config)
+
+
+def recurse_impl(remote_object, config):
+    template = env.get_template("remote_object.cpp.jinja")
+    file_path = os.path.join(
+        os.path.dirname(config["paths"]["output_impl"]),
+        remote_object.name + ".cpp",
+    )
+    os.makedirs(os.path.dirname(config["paths"]["output_impl"]), exist_ok=True)
+    with open(file_path, "w") as output_file:
+        print(template.render(instance=remote_object), file=output_file)
+    for attr in remote_object.remote_attributes.values():
+        if hasattr(attr, "remote_attributes"):
+            recurse_impl(attr, config)
```

### Comparing `Avlos-0.5.2/avlos/generators/generator_dbc.py` & `Avlos-0.5.4/avlos/generators/generator_dbc.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os
-from jinja2 import Environment, PackageLoader, select_autoescape
-from avlos.generators.filters import avlos_endpoints
-
-env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
-
-
-def process(instance, config):
-    env.filters["endpoints"] = avlos_endpoints
-
-    template = env.get_template("device.dbc.jinja")
-    os.makedirs(os.path.dirname(config["paths"]["output_file"]), exist_ok=True)
-    with open(config["paths"]["output_file"], "w") as output_file:
-        print(
-            template.render(instance=instance),
-            file=output_file,
-        )
+import os
+from jinja2 import Environment, PackageLoader, select_autoescape
+from avlos.generators.filters import avlos_endpoints
+
+env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
+
+
+def process(instance, config):
+    env.filters["endpoints"] = avlos_endpoints
+
+    template = env.get_template("device.dbc.jinja")
+    os.makedirs(os.path.dirname(config["paths"]["output_file"]), exist_ok=True)
+    with open(config["paths"]["output_file"], "w") as output_file:
+        print(
+            template.render(instance=instance),
+            file=output_file,
+        )
```

### Comparing `Avlos-0.5.2/avlos/generators/generator_rst.py` & `Avlos-0.5.4/avlos/generators/generator_rst.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os
-from jinja2 import Environment, PackageLoader, select_autoescape
-from avlos.generators.filters import avlos_endpoints
-
-env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
-
-
-def process(instance, config):
-    env.filters["endpoints"] = avlos_endpoints
-
-    template = env.get_template("docs.rst.jinja")
-    os.makedirs(os.path.dirname(config["paths"]["output_file"]), exist_ok=True)
-    with open(config["paths"]["output_file"], "w") as output_file:
-        print(
-            template.render(instance=instance),
-            file=output_file,
-        )
+import os
+from jinja2 import Environment, PackageLoader, select_autoescape
+from avlos.generators.filters import avlos_endpoints
+
+env = Environment(loader=PackageLoader("avlos"), autoescape=select_autoescape())
+
+
+def process(instance, config):
+    env.filters["endpoints"] = avlos_endpoints
+
+    template = env.get_template("docs.rst.jinja")
+    os.makedirs(os.path.dirname(config["paths"]["output_file"]), exist_ok=True)
+    with open(config["paths"]["output_file"], "w") as output_file:
+        print(
+            template.render(instance=instance),
+            file=output_file,
+        )
```

### Comparing `Avlos-0.5.2/avlos/mixins/comm_node.py` & `Avlos-0.5.4/avlos/mixins/comm_node.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from functools import cached_property
-
-
-class CommNode:
-    def __init__(self):
-        self._parent = None
-        self._channel = None
-
-    @cached_property
-    def parent(self):
-        return self._parent
-
-    @cached_property
-    def root(self):
-        return self._parent.root
-
-    @cached_property
-    def channel(self):
-        try:
-            return self.parent.channel
-        except AttributeError:
-            return self._channel
-
-    def set_channel(self, channel):
-        self._channel = channel
+from functools import cached_property
+
+
+class CommNode:
+    def __init__(self):
+        self._parent = None
+        self._channel = None
+
+    @cached_property
+    def parent(self):
+        return self._parent
+
+    @cached_property
+    def root(self):
+        return self._parent.root
+
+    @cached_property
+    def channel(self):
+        try:
+            return self.parent.channel
+        except AttributeError:
+            return self._channel
+
+    def set_channel(self, channel):
+        self._channel = channel
```

### Comparing `Avlos-0.5.2/avlos/mixins/impex_node.py` & `Avlos-0.5.4/avlos/mixins/impex_node.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-class ImpexNode:
-    def import_values(self, data):
-        # TODO: Assert correct type
-        try:
-            if "export" in self.meta and self.meta["export"] == True:
-                self.set_value_with_string(data)
-        except AttributeError:
-            for name, attr in self.remote_attributes.items():
-                try:
-                    if name in data:
-                        attr.import_values(data[name])
-                except AttributeError:
-                    pass
-
-    def export_values(self):
-        try:
-            if "export" in self.meta and self.meta["export"] == True:
-                return self.get_value()
-        except AttributeError:
-            values = {}
-            for name, node in self.remote_attributes.items():
-                try:
-                    val = node.export_values()
-                    if val != None:
-                        values[name] = val
-                except AttributeError:
-                    pass
-            if len(values) > 0:
-                return values
-            return None
+class ImpexNode:
+    def import_values(self, data):
+        # TODO: Assert correct type
+        try:
+            if "export" in self.meta and self.meta["export"] == True:
+                self.set_value_with_string(data)
+        except AttributeError:
+            for name, attr in self.remote_attributes.items():
+                try:
+                    if name in data:
+                        attr.import_values(data[name])
+                except AttributeError:
+                    pass
+
+    def export_values(self):
+        try:
+            if "export" in self.meta and self.meta["export"] == True:
+                return self.get_value()
+        except AttributeError:
+            values = {}
+            for name, node in self.remote_attributes.items():
+                try:
+                    val = node.export_values()
+                    if val != None:
+                        values[name] = val
+                except AttributeError:
+                    pass
+            if len(values) > 0:
+                return values
+            return None
```

### Comparing `Avlos-0.5.2/avlos/mixins/named_node.py` & `Avlos-0.5.4/avlos/mixins/named_node.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from functools import cached_property
-
-
-class NamedNode:
-    def __init__(self, name, include_base_name=False):
-        self._parent = None
-        self.name = name
-        self.include_base_name = include_base_name
-
-    # this kinda stinks, cause it is implemented elsewhere
-    # @cached_property
-    # def parent(self):
-    #     return self._parent
-
-    @cached_property
-    def full_name(self):
-        try:
-            return "{}.{}".format(self._parent.full_name, self.name).strip(".")
-        except AttributeError:
-            if self.include_base_name:
-                return self.name
-            return ""
+from functools import cached_property
+
+
+class NamedNode:
+    def __init__(self, name, include_base_name=False):
+        self._parent = None
+        self.name = name
+        self.include_base_name = include_base_name
+
+    # this kinda stinks, cause it is implemented elsewhere
+    # @cached_property
+    # def parent(self):
+    #     return self._parent
+
+    @cached_property
+    def full_name(self):
+        try:
+            return "{}.{}".format(self._parent.full_name, self.name).strip(".")
+        except AttributeError:
+            if self.include_base_name:
+                return self.name
+            return ""
```

### Comparing `Avlos-0.5.2/avlos/processor.py` & `Avlos-0.5.4/avlos/processor.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from os.path import join, dirname, basename, realpath
-import yaml
-from importlib import import_module
-
-
-def process_with_config_file(device_instance, avlos_config_path, traverse_path=False):
-    """
-    Process a device spec using an output config path.
-    """
-    real_path = realpath(avlos_config_path)
-    avlos_config = None
-    while not avlos_config:
-        try:
-            with open(real_path) as avlos_config_stream:
-                avlos_config = yaml.safe_load(avlos_config_stream)
-        except FileNotFoundError as e:
-            if traverse_path:
-                # traverse path backwards
-                new_config_path = join(dirname(real_path), "..", basename(real_path))
-                if new_config_path == real_path:
-                    # we're at the root, and have not found the file
-                    raise FileNotFoundError from e
-                real_path = new_config_path
-            else:
-                raise e
-
-    for module_config in avlos_config["generators"].values():
-        # Convert all paths to absolute using the base path
-        for path_name, path in module_config["paths"].items():
-            module_config["paths"][path_name] = realpath(join(dirname(real_path), path))
-    process_with_config_object(device_instance, avlos_config)
-
-
-def process_with_config_object(device_instance, avlos_config):
-    """
-    Process a device spec using an output config object.
-    """
-    for module_name, module_config in avlos_config["generators"].items():
-        if "enabled" in module_config and True == module_config["enabled"]:
-            generator = import_module(
-                ".generators.{}".format(module_name), package="avlos"
-            )
-            generator.process(device_instance, module_config)
+from os.path import join, dirname, basename, realpath
+import yaml
+from importlib import import_module
+
+
+def process_with_config_file(device_instance, avlos_config_path, traverse_path=False):
+    """
+    Process a device spec using an output config path.
+    """
+    real_path = realpath(avlos_config_path)
+    avlos_config = None
+    while not avlos_config:
+        try:
+            with open(real_path) as avlos_config_stream:
+                avlos_config = yaml.safe_load(avlos_config_stream)
+        except FileNotFoundError as e:
+            if traverse_path:
+                # traverse path backwards
+                new_config_path = join(dirname(real_path), "..", basename(real_path))
+                if new_config_path == real_path:
+                    # we're at the root, and have not found the file
+                    raise FileNotFoundError from e
+                real_path = new_config_path
+            else:
+                raise e
+
+    for module_config in avlos_config["generators"].values():
+        # Convert all paths to absolute using the base path
+        for path_name, path in module_config["paths"].items():
+            module_config["paths"][path_name] = realpath(join(dirname(real_path), path))
+    process_with_config_object(device_instance, avlos_config)
+
+
+def process_with_config_object(device_instance, avlos_config):
+    """
+    Process a device spec using an output config object.
+    """
+    for module_name, module_config in avlos_config["generators"].items():
+        if "enabled" in module_config and True == module_config["enabled"]:
+            generator = import_module(
+                ".generators.{}".format(module_name), package="avlos"
+            )
+            generator.process(device_instance, module_config)
```

### Comparing `Avlos-0.5.2/avlos/templates/device.cpp.jinja` & `Avlos-0.5.4/avlos/templates/device.cpp.jinja`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-/*
-* This file was automatically generated using Avlos.
-* https://github.com/tinymovr/avlos
-*
-* Any changes to this file will be overwritten when
-* content is regenerated.
-*/
-
-{%- macro getter_byval(attr) -%}
-{{attr.dtype.c_name}} {{ device_name | capitalize_first }}::get_{{attr.name}}(void)
-{
-    {{attr.dtype.c_name}} value = 0;
-    this->send({{attr.ep_id}}, this->_data, 0, true);
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
-    {
-        read_le(&value, this->_data);
-    }
-    return value;
-}
-{%- endmacro %}
-
-{%- macro getter_char(attr) -%}
-void {{ device_name | capitalize_first }}::get_{{attr.name}}(char out_value[])
-{
-    this->send({{attr.ep_id}}, this->_data, 0, true);
-    this->_dlc = 0;
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
-    {
-        memcpy(out_value, this->_data, this->_dlc);
-    }
-}
-{%- endmacro %}
-
-{%- macro setter_byval(attr) -%}
-void {{ device_name | capitalize_first }}::set_{{attr.name}}({{attr.dtype.c_name}} value)
-{
-    this->send({{attr.ep_id}}, this->_data, 0, false);
-}
-{%- endmacro %}
-
-{%- macro setter_char(attr) -%}
-void {{ device_name | capitalize_first }}::set_{{attr.name}}(char value[])
-{
-    memcpy(this->_data, value, sizeof(value));
-    this->send({{attr.ep_id}}, this->_data, sizeof(value), false);
-}
-{%- endmacro %}
-
-{%- for include in includes %}
-#include <{{ include }}>
-{%- endfor %}
-
-{%- if instance.remote_attributes %}
-    {%- for attr in instance.remote_attributes.values() %}
-        {%- if attr.remote_attributes %}
-        {%- else %}
-            {%- if attr.getter_name %}
-
-                {%- if attr.dtype.c_name == "char[]" %}
-{{ getter_char(attr) }}
-                {%- else %}
-{{ getter_byval(attr) }}
-                {%- endif %}
-
-            {%- endif %}
-            {%- if attr.setter_name %}
-
-                {%- if attr.dtype.c_name == "char[]" %}
-{{ setter_char(attr) }}
-                {%- else %}
-{{ setter_byval(attr) }}
-                {%- endif %}
-
-            {%- endif %}
-            {%- if attr.caller_name %}
-                {%- set comma = joiner(", ") %}
-
-{{attr.dtype.c_name}} {{ device_name | capitalize_first }}::{{attr.name}}({%- for arg in attr.arguments %}{{ comma() }}{{arg.dtype.c_name}} {{ arg.name }} {%- endfor %})
-{
-    {%- if attr.dtype.c_name == "void" %}
-    this->send({{attr.ep_id}}, this->_data, 0, true);
-    {%- else %}
-    this->send({{attr.ep_id}}, this->_data, sizeof({{attr.dtype.c_name}}), false);
-    {%- endif %}
-}
-            {%- endif %}
-        {%- endif %}
-    {%- endfor %}
-{%- endif %}
-
+/*
+* This file was automatically generated using Avlos.
+* https://github.com/tinymovr/avlos
+*
+* Any changes to this file will be overwritten when
+* content is regenerated.
+*/
+
+{%- macro getter_byval(attr) -%}
+{{attr.dtype.c_name}} {{ device_name | capitalize_first }}::get_{{attr.name}}(void)
+{
+    {{attr.dtype.c_name}} value = 0;
+    this->send({{attr.ep_id}}, this->_data, 0, true);
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    {
+        read_le(&value, this->_data);
+    }
+    return value;
+}
+{%- endmacro %}
+
+{%- macro getter_char(attr) -%}
+void {{ device_name | capitalize_first }}::get_{{attr.name}}(char out_value[])
+{
+    this->send({{attr.ep_id}}, this->_data, 0, true);
+    this->_dlc = 0;
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    {
+        memcpy(out_value, this->_data, this->_dlc);
+    }
+}
+{%- endmacro %}
+
+{%- macro setter_byval(attr) -%}
+void {{ device_name | capitalize_first }}::set_{{attr.name}}({{attr.dtype.c_name}} value)
+{
+    this->send({{attr.ep_id}}, this->_data, 0, false);
+}
+{%- endmacro %}
+
+{%- macro setter_char(attr) -%}
+void {{ device_name | capitalize_first }}::set_{{attr.name}}(char value[])
+{
+    memcpy(this->_data, value, sizeof(value));
+    this->send({{attr.ep_id}}, this->_data, sizeof(value), false);
+}
+{%- endmacro %}
+
+{%- for include in includes %}
+#include <{{ include }}>
+{%- endfor %}
+
+{%- if instance.remote_attributes %}
+    {%- for attr in instance.remote_attributes.values() %}
+        {%- if attr.remote_attributes %}
+        {%- else %}
+            {%- if attr.getter_name %}
+
+                {%- if attr.dtype.c_name == "char[]" %}
+{{ getter_char(attr) }}
+                {%- else %}
+{{ getter_byval(attr) }}
+                {%- endif %}
+
+            {%- endif %}
+            {%- if attr.setter_name %}
+
+                {%- if attr.dtype.c_name == "char[]" %}
+{{ setter_char(attr) }}
+                {%- else %}
+{{ setter_byval(attr) }}
+                {%- endif %}
+
+            {%- endif %}
+            {%- if attr.caller_name %}
+                {%- set comma = joiner(", ") %}
+
+{{attr.dtype.c_name}} {{ device_name | capitalize_first }}::{{attr.name}}({%- for arg in attr.arguments %}{{ comma() }}{{arg.dtype.c_name}} {{ arg.name }} {%- endfor %})
+{
+    {%- if attr.dtype.c_name == "void" %}
+    this->send({{attr.ep_id}}, this->_data, 0, true);
+    {%- else %}
+    this->send({{attr.ep_id}}, this->_data, sizeof({{attr.dtype.c_name}}), false);
+    {%- endif %}
+}
+            {%- endif %}
+        {%- endif %}
+    {%- endfor %}
+{%- endif %}
+
```

### Comparing `Avlos-0.5.2/avlos/templates/device.dbc.jinja` & `Avlos-0.5.4/avlos/templates/device.dbc.jinja`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-
-VERSION "{{instance.version}}"
-
-{% for attr in instance | endpoints %}
-  {%- if attr.getter_name or attr.setter_name %}
-    {%- if attr.getter_name %}
-BO_ {{attr.ep_id}} {{attr.getter_name}}: {{[attr.dtype.size, 1]|max}} Vector__XXX
-  SG_ {{attr.name}} : 0|{{[attr.dtype.size, 1]|max}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
-    {%- endif %}
-    {%- if attr.setter_name %}
-BO_ {{attr.ep_id}} {{attr.setter_name}}: {{[attr.dtype.size, 1]|max}} Vector__XXX
-  SG_ {{attr.name}} : 0|{{[attr.dtype.size, 1]|max}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
-    {%- endif %}
-  {%- elif attr.caller_name %}
-BO_ {{attr.ep_id}} {{attr.caller_name}}: {{[attr.arguments|length, 1]|max}} Vector__XXX
-    {%- if attr.arguments|length == 0%}
-  SG_ {{attr.name}} : 0|{{[attr.dtype.size, 1]|max}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
-    {%- endif %}
-    {%- set count = [0] %}
-    {%- for arg in attr.arguments %}
-  SG_ {{arg.name}} : {{count[0]}}|{{arg.dtype.size}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
-      {%- if count.append(count.pop() + arg.dtype.size) %}{% endif %} {# increment count by 1 #}
-    {%- endfor %}
-  {%- endif %}
+
+VERSION "{{instance.version}}"
+
+{% for attr in instance | endpoints %}
+  {%- if attr.getter_name or attr.setter_name %}
+    {%- if attr.getter_name %}
+BO_ {{attr.ep_id}} {{attr.getter_name}}: {{[attr.dtype.size, 1]|max}} Vector__XXX
+  SG_ {{attr.name}} : 0|{{[attr.dtype.size, 1]|max}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
+    {%- endif %}
+    {%- if attr.setter_name %}
+BO_ {{attr.ep_id}} {{attr.setter_name}}: {{[attr.dtype.size, 1]|max}} Vector__XXX
+  SG_ {{attr.name}} : 0|{{[attr.dtype.size, 1]|max}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
+    {%- endif %}
+  {%- elif attr.caller_name %}
+BO_ {{attr.ep_id}} {{attr.caller_name}}: {{[attr.arguments|length, 1]|max}} Vector__XXX
+    {%- if attr.arguments|length == 0%}
+  SG_ {{attr.name}} : 0|{{[attr.dtype.size, 1]|max}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
+    {%- endif %}
+    {%- set count = [0] %}
+    {%- for arg in attr.arguments %}
+  SG_ {{arg.name}} : {{count[0]}}|{{arg.dtype.size}}@1+ (1,0) [0|0] "{{attr.unit}}" Vector__XXX
+      {%- if count.append(count.pop() + arg.dtype.size) %}{% endif %} {# increment count by 1 #}
+    {%- endfor %}
+  {%- endif %}
 {% endfor %}
```

### Comparing `Avlos-0.5.2/avlos/templates/device.hpp.jinja` & `Avlos-0.5.4/avlos/templates/fw_endpoints.c.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,107 @@
-/*
-* This file was automatically generated using Avlos.
-* https://github.com/tinymovr/avlos
-*
-* Any changes to this file will be overwritten when
-* content is regenerated.
-*/
-
-#pragma once
-
-#include <{{ helper_file | file_from_path }}>
-{%- for include in includes %}
-#include <{{ include }}>
-{%- endfor %}
-
-{%- if instance.remote_attributes %}
-    {%- for attr in instance.remote_attributes.values() %}
-        {%- if attr.remote_attributes %}
-#include <{{attr.name}}.hpp>
-        {%- endif %}
-    {%- endfor %}
-{%- endif %}
-
-static uint32_t avlos_proto_hash = {{ instance.hash_uint32 }};
-
-{%- for ep in instance | bitmask_eps %}
-
-enum {{ ep.full_name | replace(".", "_") }}_flags
-{
-    {%- set comma = joiner(", ") %}
-    {{ ep.full_name | replace(".", "_") | upper }}_NONE = 0,
-    {%- for flag in ep.bitmask %}{{ comma() }}
-    {{ ep.full_name | replace(".", "_") | upper }}_{{ flag.name }} = (1 << {{ loop.index0 }})
-    {%- endfor %}
-};
-{%- endfor %}
-
-{%- for ep in instance | enum_eps %}
-
-enum {{ ep.full_name | replace(".", "_") }}_options
-{
-    {%- set comma = joiner(", ") %}
-    {%- for option in ep.options %}{{ comma() }}
-    {{ ep.full_name | replace(".", "_") | upper }}_{{ option.name }} = {{ loop.index0 }}
-    {%- endfor %}
-};
-{%- endfor %}
-
-class {{ device_name | capitalize_first }} : Node
-{
-    public:
-
-        {{ device_name | capitalize_first }}(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb):
-            Node(_can_node_id, _send_cb, _recv_cb) 
-{%- if instance.remote_attributes %}
-    {%- for attr in instance.remote_attributes.values() %}
-        {%- if attr.remote_attributes %}
-            , {{attr.name}}(_can_node_id, _send_cb, _recv_cb)
-        {%- endif %}
-    {%- endfor %}
-{%- endif %} {};
-
-    {%- if instance.remote_attributes %}
-        {%- for attr in instance.remote_attributes.values() %}
-            {%- if attr.remote_attributes %}
-        {{attr.name | capitalize_first}}_ {{attr.name}};
-
-            {%- else %}
-                {%- if attr.getter_name %}
-                    {%- if attr.dtype.c_name == "char[]" %}
-        void get_{{attr.name}}(char out_value[]);
-                    {%- else %}
-        {{attr.dtype.c_name}} get_{{attr.name}}(void);
-                    {%- endif %}
-                {%- endif %}
-                {%- if attr.setter_name %}
-                    {%- if attr.dtype.c_name == "char[]" %}
-        void set_{{attr.name}}(char value[]);
-                    {%- else %}
-        void set_{{attr.name}}({{attr.dtype.c_name}} value);
-                    {%- endif %}
-                {%- endif %}
-                {%- if attr.caller_name %}
-                    {%- set comma = joiner(", ") %}
-        {{attr.dtype.c_name}} {{attr.name}}({%- for arg in attr.arguments %}{{ comma() }}{{arg.dtype.c_name}} {{ arg.name }} {%- endfor %});
-                {%- endif %}
-
-            {%- endif %}
-        {%- endfor %}
-    {%- endif %}
-
-};
+/*
+* This file was automatically generated using Avlos.
+* https://github.com/tinymovr/avlos
+*
+* Any changes to this file will be overwritten when
+* content is regenerated.
+*/
+
+{%- macro getter_byval(attr) -%}
+    if (AVLOS_CMD_READ == cmd) {
+        {{attr.dtype.c_name}} v;
+        v = {{ attr.getter_name }}();
+        *buffer_len = sizeof(v);
+        memcpy(buffer, &v, sizeof(v));
+        return AVLOS_RET_READ;
+    }
+{%- endmacro %}
+
+{%- macro getter_char(attr) -%}
+    if (AVLOS_CMD_READ == cmd) {
+        {{attr.dtype.c_name}} v;
+        v = {{ attr.getter_name }}();
+        *buffer_len = sizeof(v);
+        memcpy(buffer, &v, sizeof(v));
+        return AVLOS_RET_READ;
+    }
+{%- endmacro %}
+
+{%- macro setter_byval(attr) -%}
+    {% if attr.getter_name %}else {% endif %}if (AVLOS_CMD_WRITE == cmd) {
+        {{attr.dtype.c_name}} v;
+        memcpy(&v, buffer, sizeof(v));
+        {{ attr.setter_name }}(v);
+        return AVLOS_RET_WRITE;
+    }
+{%- endmacro %}
+
+{%- macro setter_char(attr) -%}
+    {% if attr.getter_name %}else {% endif %}if (AVLOS_CMD_WRITE == cmd) {
+        {{attr.dtype.c_name}} v;
+        memcpy(&v, buffer, sizeof(v));
+        {{ attr.setter_name }}(v);
+        return AVLOS_RET_WRITE;
+    }
+{%- endmacro %}
+
+{%- for include in includes %}
+#include {{ include | as_include }}
+{%- endfor %}
+
+{% set comma = joiner(", ") %}
+uint8_t (*avlos_endpoints[{{ instance | endpoints | length }}])(uint8_t * buffer, uint8_t * buffer_len, Avlos_Command cmd) = { {%- for attr in instance | endpoints %}{{ comma() }}&avlos_{{attr.full_name | replace(".", "_") }}{%- endfor %} };
+uint32_t avlos_proto_hash = {{ instance.hash_uint32 }};
+
+uint32_t _avlos_get_proto_hash(void)
+{
+    return avlos_proto_hash;
+}
+
+{%- for attr in instance | endpoints %}
+
+uint8_t avlos_{{attr.full_name | replace(".", "_") }}(uint8_t * buffer, uint8_t * buffer_len, Avlos_Command cmd)
+{
+    {%- if attr.getter_name %}
+
+        {%- if attr.dtype.c_name == "char[]" %}
+{{ getter_char(attr) }}
+        {%- else %}
+{{ getter_byval(attr) }}
+        {%- endif %}
+
+    {%- endif %}
+    {%- if attr.setter_name %}
+
+        {%- if attr.dtype.c_name == "char[]" %}
+{{ setter_char(attr) }}
+        {%- else %}
+{{ setter_byval(attr) }}
+        {%- endif %}
+
+    {%- endif %}
+    {%- if attr.caller_name %}
+        {%- if attr.arguments | length > 0 %}
+    uint8_t offset = 0;
+        {%- endif %}
+    {%- for arg in attr.arguments %}
+    {{ arg.dtype.c_name }} {{arg.name}};
+    memcpy(&{{arg.name}}, buffer+offset, sizeof({{arg.name}}));
+    offset += sizeof({{arg.name}});
+    {%- endfor %}
+
+    {%- set comma = joiner(", ") %}
+    {%- if attr.dtype.c_name != "void" %}
+    {{attr.dtype.c_name}} ret_val = {{ attr.caller_name }}({%- for arg in attr.arguments %}{{ comma() }}{{ arg.name }} {%- endfor %});
+    memcpy(buffer, &ret_val, sizeof(ret_val));
+    *buffer_len = sizeof(ret_val);
+    {%- else %}
+    {{ attr.caller_name }}({%- for arg in attr.arguments %}{{ comma() }}{{ arg.name }} {%- endfor %});
+    {%- endif %}
+
+    return AVLOS_RET_CALL;
+    {%- else %}
+    return AVLOS_RET_NOACTION;
+    {%- endif %}
+}
+
+{%- endfor %}
```

### Comparing `Avlos-0.5.2/avlos/templates/docs.rst.jinja` & `Avlos-0.5.4/avlos/templates/docs.rst.jinja`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-
-.. _api-reference:
-
-API REFERENCE
-=============
-
-Spec version {{ instance.version }}
-
-{% for attr in instance | endpoints %}
-{%- if attr.rst_target %}
-.. _{{attr.rst_target}}:
-{% endif %}
-    {%- if attr.getter_name or attr.setter_name %}
-{{ attr.full_name }}
--------------------------------------------------------------------
-
-ID: {{ attr.ep_id }}
-Type: {{ attr.dtype.nickname }}
-{% if None != attr.unit %}Units: {{attr.unit}} {%- endif %}
-
-{{ attr.summary }}
-
-{% if attr.bitmask %}Flags: {% for flag in attr.bitmask %}
-- {{ flag.name }}
-{%- endfor %}{%- endif %}
-{%- if attr.options %}Options: {% for flag in attr.options %}
-- {{ flag.name }}
-{%- endfor %}{%- endif %}
-
-    {%- elif attr.caller_name %}
-        {%- set comma = joiner(", ") %}
-{{ attr.name }}({%- for arg in attr.arguments %}{{ comma() }}{{ arg.name }} {%- endfor %}) -> {{ attr.dtype.nickname }}
--------------------------------------------------------------------
-
-ID: {{ attr.ep_id }}
-{% if attr.dtype %}Return Type: {{ attr.dtype.nickname }} {%- endif %}
-{% if attr.unit %}Units: {{ attr.unit }} {%- endif %}
-
-{{ attr.summary }}
-
-    {%- endif %}
-
+
+.. _api-reference:
+
+API REFERENCE
+=============
+
+Spec version {{ instance.version }}
+
+{% for attr in instance | endpoints %}
+{%- if attr.rst_target %}
+.. _{{attr.rst_target}}:
+{% endif %}
+    {%- if attr.getter_name or attr.setter_name %}
+{{ attr.full_name }}
+-------------------------------------------------------------------
+
+ID: {{ attr.ep_id }}
+Type: {{ attr.dtype.nickname }}
+{% if None != attr.unit %}Units: {{attr.unit}} {%- endif %}
+
+{{ attr.summary }}
+
+{% if attr.bitmask %}Flags: {% for flag in attr.bitmask %}
+- {{ flag.name }}
+{%- endfor %}{%- endif %}
+{%- if attr.options %}Options: {% for flag in attr.options %}
+- {{ flag.name }}
+{%- endfor %}{%- endif %}
+
+    {%- elif attr.caller_name %}
+        {%- set comma = joiner(", ") %}
+{{ attr.name }}({%- for arg in attr.arguments %}{{ comma() }}{{ arg.name }} {%- endfor %}) -> {{ attr.dtype.nickname }}
+-------------------------------------------------------------------
+
+ID: {{ attr.ep_id }}
+{% if attr.dtype %}Return Type: {{ attr.dtype.nickname }} {%- endif %}
+{% if attr.unit %}Units: {{ attr.unit }} {%- endif %}
+
+{{ attr.summary }}
+
+    {%- endif %}
+
 {% endfor %}
```

### Comparing `Avlos-0.5.2/avlos/templates/fw_endpoints.h.jinja` & `Avlos-0.5.4/avlos/templates/fw_endpoints.h.jinja`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-/*
-* This file was automatically generated using Avlos.
-* https://github.com/tinymovr/avlos
-*
-* Any changes to this file will be overwritten when
-* content is regenerated.
-*/
-
-#pragma once
-
-{%- for include in includes %}
-#include {{ include | as_include }}
-{%- endfor %}
-
-typedef enum
-{
-    AVLOS_RET_NOACTION,
-    AVLOS_RET_READ = 1,
-    AVLOS_RET_WRITE = 2,
-    AVLOS_RET_CALL = 3
-} Avlos_Return;
-
-typedef enum
-{
-    AVLOS_CMD_WRITE,
-    AVLOS_CMD_READ = 1
-} Avlos_Command;
-
-{%- for ep in instance | bitmask_eps %}
-
-typedef enum
-{
-    {%- set comma = joiner(", ") %}
-    {{ ep.full_name | replace(".", "_") | upper }}_NONE = 0,
-    {%- for flag in ep.bitmask %}{{ comma() }}
-    {{ ep.full_name | replace(".", "_") | upper }}_{{ flag.name }} = (1 << {{ loop.index0 }})
-    {%- endfor %}
-} {{ ep.full_name | replace(".", "_") }}_flags;
-{%- endfor %}
-
-{%- for ep in instance | enum_eps %}
-
-typedef enum
-{
-    {%- set comma = joiner(", ") %}
-    {%- for option in ep.options %}{{ comma() }}
-    {{ ep.full_name | replace(".", "_") | upper }}_{{ option.name }} = {{ loop.index0 }}
-    {%- endfor %}
-} {{ ep.full_name | replace(".", "_") }}_options;
-{%- endfor %}
-
-extern uint32_t avlos_proto_hash;
-extern uint8_t (*avlos_endpoints[{{ instance | endpoints | length }}])(uint8_t * buffer, uint8_t * buffer_len, Avlos_Command cmd);
-extern uint32_t _avlos_get_proto_hash(void);
-
-{%- for attr in instance | endpoints %}
-
-/*
-* avlos_{{attr.full_name | replace(".", "_") }}
-*
-* {{ attr.summary }}
-*
-* @param buffer
-* @param buffer_len
-*/
-uint8_t avlos_{{attr.full_name | replace(".", "_") }}(uint8_t * buffer, uint8_t * buffer_len, Avlos_Command cmd);
-
+/*
+* This file was automatically generated using Avlos.
+* https://github.com/tinymovr/avlos
+*
+* Any changes to this file will be overwritten when
+* content is regenerated.
+*/
+
+#pragma once
+
+{%- for include in includes %}
+#include {{ include | as_include }}
+{%- endfor %}
+
+typedef enum
+{
+    AVLOS_RET_NOACTION,
+    AVLOS_RET_READ = 1,
+    AVLOS_RET_WRITE = 2,
+    AVLOS_RET_CALL = 3
+} Avlos_Return;
+
+typedef enum
+{
+    AVLOS_CMD_WRITE,
+    AVLOS_CMD_READ = 1
+} Avlos_Command;
+
+{%- for ep in instance | bitmask_eps %}
+
+typedef enum
+{
+    {%- set comma = joiner(", ") %}
+    {{ ep.full_name | replace(".", "_") | upper }}_NONE = 0,
+    {%- for flag in ep.bitmask %}{{ comma() }}
+    {{ ep.full_name | replace(".", "_") | upper }}_{{ flag.name }} = (1 << {{ loop.index0 }})
+    {%- endfor %}
+} {{ ep.full_name | replace(".", "_") }}_flags;
+{%- endfor %}
+
+{%- for ep in instance | enum_eps %}
+
+typedef enum
+{
+    {%- set comma = joiner(", ") %}
+    {%- for option in ep.options %}{{ comma() }}
+    {{ ep.full_name | replace(".", "_") | upper }}_{{ option.name }} = {{ loop.index0 }}
+    {%- endfor %}
+} {{ ep.full_name | replace(".", "_") }}_options;
+{%- endfor %}
+
+extern uint32_t avlos_proto_hash;
+extern uint8_t (*avlos_endpoints[{{ instance | endpoints | length }}])(uint8_t * buffer, uint8_t * buffer_len, Avlos_Command cmd);
+extern uint32_t _avlos_get_proto_hash(void);
+
+{%- for attr in instance | endpoints %}
+
+/*
+* avlos_{{attr.full_name | replace(".", "_") }}
+*
+* {{ attr.summary }}
+*
+* @param buffer
+* @param buffer_len
+*/
+uint8_t avlos_{{attr.full_name | replace(".", "_") }}(uint8_t * buffer, uint8_t * buffer_len, Avlos_Command cmd);
+
 {%- endfor %}
```

### Comparing `Avlos-0.5.2/avlos/templates/helpers.hpp.jinja` & `Avlos-0.5.4/avlos/templates/helpers.hpp.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -1,237 +1,242 @@
-/*
-* This file was automatically generated using Avlos.
-* https://github.com/tinymovr/avlos
-*
-* Any changes to this file will be overwritten when
-* content is regenerated.
-*/
-
-#pragma once
-
-#if defined ARDUINO || __cplusplus < 201103L
-#include <stdint.h>
-#include <stddef.h>
-#else
-#include <cstdint>
-#include <cstddef>
-#endif
-
-#if defined ARDUINO
-#include "Arduino.h"
-#endif
-
-#define EP_BITS (6)
-#define RECV_DELAY_US (160.0f)
-
-enum recv_result {
-    RECV_OK = 0,
-    RECV_ERROR_ARB_ID = (1 << 0), 
-    RECV_ERROR_TIMEOUT = (1 << 1)
-};
-
-typedef void (*send_callback)(uint32_t arbitration_id, uint8_t *data, uint8_t dlc, bool rtr);
-typedef recv_result (*recv_callback)(uint32_t arbitration_id, uint8_t *data, uint8_t *dlc);
-
-class Node {
-    public:
-
-    Node(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb):
-        can_node_id(_can_node_id), send_cb(_send_cb), recv_cb(_recv_cb) {}
-
-    protected:
-    uint8_t can_node_id;
-    send_callback send_cb;
-    recv_callback recv_cb;
-    uint8_t _data[8];
-    uint8_t _dlc;
-    uint8_t get_arbitration_id(uint8_t cmd_id) {
-        return this->can_node_id << EP_BITS | cmd_id;
-    }
-    void send(uint8_t cmd_id, uint8_t *data, uint8_t data_size, bool rtr)
-    {
-        const uint8_t arb_id = this->get_arbitration_id(cmd_id);
-        this->send_cb(arb_id, data, data_size, rtr);
-    }
-
-    bool recv(uint8_t cmd_id, uint8_t *data, uint8_t *data_size, uint16_t delay_us)
-    {
-#if defined ARDUINO
-        // A delay of a few 100s of us needs to be inserted
-        // to ensure the response has been transmitted.
-        // TODO: Better handle this using an interrupt.
-        if (delay_us > 0)
-        {
-            delayMicroseconds(delay_us);
-        }
-#endif
-        const uint8_t arb_id = this->get_arbitration_id(cmd_id);
-        recv_result r;
-        do {
-            r = this->recv_cb(arb_id, data, data_size);
-        } while (r == RECV_ERROR_ARB_ID);
-        if (RECV_OK == r)
-        {
-            return true;
-        }
-        return false;
-    }
-};
-
-template<typename T>
-inline size_t write_le(T value, uint8_t* buffer);
-
-template<typename T>
-inline size_t read_le(T* value, const uint8_t* buffer);
-
-template<>
-inline size_t write_le<bool>(bool value, uint8_t* buffer) {
-    buffer[0] = value ? 1 : 0;
-    return 1;
-}
-
-template<>
-inline size_t write_le<uint8_t>(uint8_t value, uint8_t* buffer) {
-    buffer[0] = value;
-    return 1;
-}
-
-template<>
-inline size_t write_le<int8_t>(int8_t value, uint8_t* buffer) {
-    buffer[0] = value;
-    return 1;
-}
-
-template<>
-inline size_t write_le<uint16_t>(uint16_t value, uint8_t* buffer) {
-    buffer[0] = (value >> 0) & 0xff;
-    buffer[1] = (value >> 8) & 0xff;
-    return 2;
-}
-
-template<>
-inline size_t write_le<int16_t>(int16_t value, uint8_t* buffer) {
-    buffer[0] = (value >> 0) & 0xff;
-    buffer[1] = (value >> 8) & 0xff;
-    return 2;
-}
-
-template<>
-inline size_t write_le<uint32_t>(uint32_t value, uint8_t* buffer) {
-    buffer[0] = (value >> 0) & 0xff;
-    buffer[1] = (value >> 8) & 0xff;
-    buffer[2] = (value >> 16) & 0xff;
-    buffer[3] = (value >> 24) & 0xff;
-    return 4;
-}
-
-template<>
-inline size_t write_le<int32_t>(int32_t value, uint8_t* buffer) {
-    buffer[0] = (value >> 0) & 0xff;
-    buffer[1] = (value >> 8) & 0xff;
-    buffer[2] = (value >> 16) & 0xff;
-    buffer[3] = (value >> 24) & 0xff;
-    return 4;
-}
-
-template<>
-inline size_t write_le<uint64_t>(uint64_t value, uint8_t* buffer) {
-    buffer[0] = (value >> 0) & 0xff;
-    buffer[1] = (value >> 8) & 0xff;
-    buffer[2] = (value >> 16) & 0xff;
-    buffer[3] = (value >> 24) & 0xff;
-    buffer[4] = (value >> 32) & 0xff;
-    buffer[5] = (value >> 40) & 0xff;
-    buffer[6] = (value >> 48) & 0xff;
-    buffer[7] = (value >> 56) & 0xff;
-    return 8;
-}
-
-template<>
-inline size_t write_le<float>(float value, uint8_t* buffer) {
-    //static_assert(CHAR_BIT * sizeof(float) == 32, "32 bit floating point expected");
-    //static_assert(std::numeric_limits<float>::is_iec559, "IEEE 754 floating point expected");
-    const uint32_t * value_as_uint32 = reinterpret_cast<const uint32_t*>(&value);
-    return write_le<uint32_t>(*value_as_uint32, buffer);
-}
-
-template<>
-inline size_t read_le<bool>(bool* value, const uint8_t* buffer) {
-    *value = buffer[0];
-    return 1;
-}
-
-template<>
-inline size_t read_le<uint8_t>(uint8_t* value, const uint8_t* buffer) {
-    *value = buffer[0];
-    return 1;
-}
-
-template<>
-inline size_t read_le<int8_t>(int8_t* value, const uint8_t* buffer) {
-    *value = buffer[0];
-    return 1;
-}
-
-template<>
-inline size_t read_le<uint16_t>(uint16_t* value, const uint8_t* buffer) {
-    *value = (static_cast<uint16_t>(buffer[0]) << 0) |
-             (static_cast<uint16_t>(buffer[1]) << 8);
-    return 2;
-}
-
-template<>
-inline size_t read_le<int16_t>(int16_t* value, const uint8_t* buffer) {
-    *value = (static_cast<uint16_t>(buffer[0]) << 0) |
-             (static_cast<uint16_t>(buffer[1]) << 8);
-    return 2;
-}
-
-template<>
-inline size_t read_le<int32_t>(int32_t* value, const uint8_t* buffer) {
-    *value = (static_cast<int32_t>(buffer[0]) << 0) |
-             (static_cast<int32_t>(buffer[1]) << 8) |
-             (static_cast<int32_t>(buffer[2]) << 16) |
-             (static_cast<int32_t>(buffer[3]) << 24);
-    return 4;
-}
-
-template<>
-inline size_t read_le<uint32_t>(uint32_t* value, const uint8_t* buffer) {
-    *value = (static_cast<uint32_t>(buffer[0]) << 0) |
-             (static_cast<uint32_t>(buffer[1]) << 8) |
-             (static_cast<uint32_t>(buffer[2]) << 16) |
-             (static_cast<uint32_t>(buffer[3]) << 24);
-    return 4;
-}
-
-template<>
-inline size_t read_le<uint64_t>(uint64_t* value, const uint8_t* buffer) {
-    *value = (static_cast<uint64_t>(buffer[0]) << 0) |
-             (static_cast<uint64_t>(buffer[1]) << 8) |
-             (static_cast<uint64_t>(buffer[2]) << 16) |
-             (static_cast<uint64_t>(buffer[3]) << 24) |
-             (static_cast<uint64_t>(buffer[4]) << 32) |
-             (static_cast<uint64_t>(buffer[5]) << 40) |
-             (static_cast<uint64_t>(buffer[6]) << 48) |
-             (static_cast<uint64_t>(buffer[7]) << 56);
-    return 8;
-}
-
-template<>
-inline size_t read_le<float>(float* value, const uint8_t* buffer) {
-    //static_assert(CHAR_BIT * sizeof(float) == 32, "32 bit floating point expected");
-    //static_assert(std::numeric_limits<float>::is_iec559, "IEEE 754 floating point expected");
-    return read_le(reinterpret_cast<uint32_t*>(value), buffer);
-}
-
-// @brief Reads a value of type T from the buffer.
-// @param buffer    Pointer to the buffer to be read. The pointer is updated by the number of bytes that were read.
-// @param length    The number of available bytes in buffer. This value is updated to subtract the bytes that were read.
-template<typename T>
-static inline T read_le(const uint8_t** buffer, size_t* length) {
-    T result;
-    size_t cnt = read_le(&result, *buffer);
-    *buffer += cnt;
-    *length -= cnt;
-    return result;
-}
+/*
+* This file was automatically generated using Avlos.
+* https://github.com/tinymovr/avlos
+*
+* Any changes to this file will be overwritten when
+* content is regenerated.
+*/
+
+#pragma once
+
+#if defined ARDUINO || __cplusplus < 201103L
+#include <stdint.h>
+#include <stddef.h>
+#else
+#include <cstdint>
+#include <cstddef>
+#endif
+
+#if defined ARDUINO
+#include "Arduino.h"
+#endif
+
+#define CAN_EP_SIZE (12)
+#define CAN_EP_MASK ((1 << CAN_EP_SIZE) - 1)
+#define CAN_SEQ_SIZE (9)
+#define CAN_SEQ_MASK (((1 << CAN_SEQ_SIZE) - 1) << CAN_EP_SIZE)
+#define CAN_DEV_SIZE (8)
+#define CAN_DEV_MASK (((1 << CAN_DEV_SIZE) - 1) << (CAN_EP_SIZE + CAN_SEQ_SIZE))
+
+#define RECV_DELAY_US (160.0f)
+
+typedef void (*send_callback)(uint32_t arbitration_id, uint8_t *data, uint8_t dlc, bool rtr);
+typedef bool (*recv_callback)(uint32_t *arbitration_id, uint8_t *data, uint8_t *dlc);
+typedef void (*delay_us_callback)(uint32_t us);
+
+class Node {
+    public:
+
+    Node(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb):
+        can_node_id(_can_node_id), send_cb(_send_cb), recv_cb(_recv_cb), delay_us_cb(_delay_us_cb) {}
+
+    protected:
+    uint8_t can_node_id;
+    send_callback send_cb;
+    recv_callback recv_cb;
+    delay_us_callback delay_us_cb;
+    uint8_t _data[8];
+    uint8_t _dlc;
+    uint32_t get_arbitration_id(uint32_t cmd_id)
+    {
+        return ((this->can_node_id << (CAN_EP_SIZE + CAN_SEQ_SIZE)) & CAN_DEV_MASK) | (cmd_id & CAN_EP_MASK);
+    }
+    void send(uint8_t cmd_id, uint8_t *data, uint8_t data_size, bool rtr)
+    {
+        const uint32_t arb_id = this->get_arbitration_id(cmd_id);
+        this->send_cb(arb_id, data, data_size, rtr);
+    }
+
+    bool recv(uint8_t cmd_id, uint8_t *data, uint8_t *data_size, uint16_t delay_us)
+    {
+        uint32_t _arbitration_id;
+        uint8_t _data[8];
+        uint8_t _data_size;
+        // A delay of a few 100s of us needs to be inserted
+        // to ensure the response has been transmitted.
+        // TODO: Better handle this using an interrupt.
+        if (delay_us > 0)
+        {
+           this->delay_us_cb(delay_us);
+        }
+        const uint32_t arb_id = this->get_arbitration_id(cmd_id);
+        while (this->recv_cb(&_arbitration_id, _data, &_data_size))
+        {
+            if (_arbitration_id == arb_id)
+            {
+                memcpy(data, _data, _data_size);
+                *data_size = _data_size;
+                return true;
+            }
+        }
+        return false;
+    }
+};
+
+template<typename T>
+inline size_t write_le(T value, uint8_t* buffer);
+
+template<typename T>
+inline size_t read_le(T* value, const uint8_t* buffer);
+
+template<>
+inline size_t write_le<bool>(bool value, uint8_t* buffer) {
+    buffer[0] = value ? 1 : 0;
+    return 1;
+}
+
+template<>
+inline size_t write_le<uint8_t>(uint8_t value, uint8_t* buffer) {
+    buffer[0] = value;
+    return 1;
+}
+
+template<>
+inline size_t write_le<int8_t>(int8_t value, uint8_t* buffer) {
+    buffer[0] = value;
+    return 1;
+}
+
+template<>
+inline size_t write_le<uint16_t>(uint16_t value, uint8_t* buffer) {
+    buffer[0] = (value >> 0) & 0xff;
+    buffer[1] = (value >> 8) & 0xff;
+    return 2;
+}
+
+template<>
+inline size_t write_le<int16_t>(int16_t value, uint8_t* buffer) {
+    buffer[0] = (value >> 0) & 0xff;
+    buffer[1] = (value >> 8) & 0xff;
+    return 2;
+}
+
+template<>
+inline size_t write_le<uint32_t>(uint32_t value, uint8_t* buffer) {
+    buffer[0] = (value >> 0) & 0xff;
+    buffer[1] = (value >> 8) & 0xff;
+    buffer[2] = (value >> 16) & 0xff;
+    buffer[3] = (value >> 24) & 0xff;
+    return 4;
+}
+
+template<>
+inline size_t write_le<int32_t>(int32_t value, uint8_t* buffer) {
+    buffer[0] = (value >> 0) & 0xff;
+    buffer[1] = (value >> 8) & 0xff;
+    buffer[2] = (value >> 16) & 0xff;
+    buffer[3] = (value >> 24) & 0xff;
+    return 4;
+}
+
+template<>
+inline size_t write_le<uint64_t>(uint64_t value, uint8_t* buffer) {
+    buffer[0] = (value >> 0) & 0xff;
+    buffer[1] = (value >> 8) & 0xff;
+    buffer[2] = (value >> 16) & 0xff;
+    buffer[3] = (value >> 24) & 0xff;
+    buffer[4] = (value >> 32) & 0xff;
+    buffer[5] = (value >> 40) & 0xff;
+    buffer[6] = (value >> 48) & 0xff;
+    buffer[7] = (value >> 56) & 0xff;
+    return 8;
+}
+
+template<>
+inline size_t write_le<float>(float value, uint8_t* buffer) {
+    //static_assert(CHAR_BIT * sizeof(float) == 32, "32 bit floating point expected");
+    //static_assert(std::numeric_limits<float>::is_iec559, "IEEE 754 floating point expected");
+    const uint32_t * value_as_uint32 = reinterpret_cast<const uint32_t*>(&value);
+    return write_le<uint32_t>(*value_as_uint32, buffer);
+}
+
+template<>
+inline size_t read_le<bool>(bool* value, const uint8_t* buffer) {
+    *value = buffer[0];
+    return 1;
+}
+
+template<>
+inline size_t read_le<uint8_t>(uint8_t* value, const uint8_t* buffer) {
+    *value = buffer[0];
+    return 1;
+}
+
+template<>
+inline size_t read_le<int8_t>(int8_t* value, const uint8_t* buffer) {
+    *value = buffer[0];
+    return 1;
+}
+
+template<>
+inline size_t read_le<uint16_t>(uint16_t* value, const uint8_t* buffer) {
+    *value = (static_cast<uint16_t>(buffer[0]) << 0) |
+             (static_cast<uint16_t>(buffer[1]) << 8);
+    return 2;
+}
+
+template<>
+inline size_t read_le<int16_t>(int16_t* value, const uint8_t* buffer) {
+    *value = (static_cast<uint16_t>(buffer[0]) << 0) |
+             (static_cast<uint16_t>(buffer[1]) << 8);
+    return 2;
+}
+
+template<>
+inline size_t read_le<int32_t>(int32_t* value, const uint8_t* buffer) {
+    *value = (static_cast<int32_t>(buffer[0]) << 0) |
+             (static_cast<int32_t>(buffer[1]) << 8) |
+             (static_cast<int32_t>(buffer[2]) << 16) |
+             (static_cast<int32_t>(buffer[3]) << 24);
+    return 4;
+}
+
+template<>
+inline size_t read_le<uint32_t>(uint32_t* value, const uint8_t* buffer) {
+    *value = (static_cast<uint32_t>(buffer[0]) << 0) |
+             (static_cast<uint32_t>(buffer[1]) << 8) |
+             (static_cast<uint32_t>(buffer[2]) << 16) |
+             (static_cast<uint32_t>(buffer[3]) << 24);
+    return 4;
+}
+
+template<>
+inline size_t read_le<uint64_t>(uint64_t* value, const uint8_t* buffer) {
+    *value = (static_cast<uint64_t>(buffer[0]) << 0) |
+             (static_cast<uint64_t>(buffer[1]) << 8) |
+             (static_cast<uint64_t>(buffer[2]) << 16) |
+             (static_cast<uint64_t>(buffer[3]) << 24) |
+             (static_cast<uint64_t>(buffer[4]) << 32) |
+             (static_cast<uint64_t>(buffer[5]) << 40) |
+             (static_cast<uint64_t>(buffer[6]) << 48) |
+             (static_cast<uint64_t>(buffer[7]) << 56);
+    return 8;
+}
+
+template<>
+inline size_t read_le<float>(float* value, const uint8_t* buffer) {
+    //static_assert(CHAR_BIT * sizeof(float) == 32, "32 bit floating point expected");
+    //static_assert(std::numeric_limits<float>::is_iec559, "IEEE 754 floating point expected");
+    return read_le(reinterpret_cast<uint32_t*>(value), buffer);
+}
+
+// @brief Reads a value of type T from the buffer.
+// @param buffer    Pointer to the buffer to be read. The pointer is updated by the number of bytes that were read.
+// @param length    The number of available bytes in buffer. This value is updated to subtract the bytes that were read.
+template<typename T>
+static inline T read_le(const uint8_t** buffer, size_t* length) {
+    T result;
+    size_t cnt = read_le(&result, *buffer);
+    *buffer += cnt;
+    *length -= cnt;
+    return result;
+}
```

### Comparing `Avlos-0.5.2/avlos/templates/remote_object.cpp.jinja` & `Avlos-0.5.4/avlos/templates/remote_object.cpp.jinja`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-/*
-* This file was automatically generated using Avlos.
-* https://github.com/tinymovr/avlos
-*
-* Any changes to this file will be overwritten when
-* content is regenerated.
-*/
-
-{%- macro getter_byval(attr) -%}
-{{attr.dtype.c_name}} {{ instance.name | capitalize_first }}_::get_{{attr.name}}(void)
-{
-    {{attr.dtype.c_name}} value = 0;
-    this->send({{attr.ep_id}}, this->_data, 0, true);
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
-    {
-        read_le(&value, this->_data);
-    }
-    return value;
-}
-{%- endmacro %}
-
-{%- macro getter_char(attr) -%}
-void {{ instance.name | capitalize_first }}_::get_{{attr.name}}(char out_value[])
-{
-    this->send({{attr.ep_id}}, this->_data, 0, true);
-    this->_dlc = 0;
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
-    {
-        memcpy(out_value, this->_data, this->_dlc);
-    }
-}
-{%- endmacro %}
-
-{%- macro setter_byval(attr) -%}
-void {{ instance.name | capitalize_first }}_::set_{{attr.name}}({{attr.dtype.c_name}} value)
-{
-    write_le(value, this->_data);
-    this->send({{attr.ep_id}}, this->_data, sizeof({{attr.dtype.c_name}}), false);
-}
-{%- endmacro %}
-
-{%- macro setter_char(attr) -%}
-void {{ instance.name | capitalize_first }}_::set_{{attr.name}}(char value[])
-{
-    memcpy(this->_data, value, sizeof(value));
-    this->send({{attr.ep_id}}, this->_data, sizeof(value), false);
-}
-{%- endmacro %}
-
-#include <{{ instance.name }}.hpp>
-{% if instance.remote_attributes %}
-    {%- for attr in instance.remote_attributes.values() %}
-        {%- if attr.remote_attributes %}
-        {%- else %}
-            {%- if attr.getter_name %}
-
-                {%- if attr.dtype.c_name == "char[]" %}
-{{ getter_char(attr) }}
-                {%- else %}
-{{ getter_byval(attr) }}
-{% endif %}
-
-            {%- endif %}
-            {%- if attr.setter_name %}
-
-                {%- if attr.dtype.c_name == "char[]" %}
-{{ setter_char(attr) }}
-                {%- else %}
-{{ setter_byval(attr) }}
-{% endif %}
-
-            {%- endif %}
-            {%- if attr.caller_name %}
-                {%- set comma = joiner(", ") %}
-
-{{attr.dtype.c_name}} {{ instance.name | capitalize_first }}_::{{attr.name}}({%- for arg in attr.arguments %}{{ comma() }}{{arg.dtype.c_name}} {{ arg.name }} {%- endfor %})
-{
-    {%- if attr.arguments|length == 0 %}
-    this->send({{attr.ep_id}}, this->_data, 0, true);
-    {%- else %}
-    uint8_t data_len = 0;
-        {%- for arg in attr.arguments %}
-    write_le({{ arg.name }}, this->_data + data_len);
-    data_len += sizeof({{ arg.name }});
-        {%- endfor %}
-
-    this->send({{attr.ep_id}}, this->_data, data_len, false);
-    {%- endif %}
-
-    {%- if attr.dtype.c_name != "void" %}
-    {{attr.dtype.c_name}} value = 0;
-    this->send(17, this->_data, 0, true);
-    if (this->recv(17, this->_data, &(this->_dlc), RECV_DELAY_US)) 
-    {
-        read_le(&value, this->_data);
-    }
-    return value;
-    {%- endif %}
-}
-            {%- endif %}
-        {%- endif %}
-    {%- endfor %}
-{%- endif %}
-
-
+/*
+* This file was automatically generated using Avlos.
+* https://github.com/tinymovr/avlos
+*
+* Any changes to this file will be overwritten when
+* content is regenerated.
+*/
+
+{%- macro getter_byval(attr) -%}
+{{attr.dtype.c_name}} {{ instance.name | capitalize_first }}_::get_{{attr.name}}(void)
+{
+    {{attr.dtype.c_name}} value = 0;
+    this->send({{attr.ep_id}}, this->_data, 0, true);
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    {
+        read_le(&value, this->_data);
+    }
+    return value;
+}
+{%- endmacro %}
+
+{%- macro getter_char(attr) -%}
+void {{ instance.name | capitalize_first }}_::get_{{attr.name}}(char out_value[])
+{
+    this->send({{attr.ep_id}}, this->_data, 0, true);
+    this->_dlc = 0;
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    {
+        memcpy(out_value, this->_data, this->_dlc);
+    }
+}
+{%- endmacro %}
+
+{%- macro setter_byval(attr) -%}
+void {{ instance.name | capitalize_first }}_::set_{{attr.name}}({{attr.dtype.c_name}} value)
+{
+    write_le(value, this->_data);
+    this->send({{attr.ep_id}}, this->_data, sizeof({{attr.dtype.c_name}}), false);
+}
+{%- endmacro %}
+
+{%- macro setter_char(attr) -%}
+void {{ instance.name | capitalize_first }}_::set_{{attr.name}}(char value[])
+{
+    memcpy(this->_data, value, sizeof(value));
+    this->send({{attr.ep_id}}, this->_data, sizeof(value), false);
+}
+{%- endmacro %}
+
+#include <{{ instance.name }}.hpp>
+{% if instance.remote_attributes %}
+    {%- for attr in instance.remote_attributes.values() %}
+        {%- if attr.remote_attributes %}
+        {%- else %}
+            {%- if attr.getter_name %}
+
+                {%- if attr.dtype.c_name == "char[]" %}
+{{ getter_char(attr) }}
+                {%- else %}
+{{ getter_byval(attr) }}
+{% endif %}
+
+            {%- endif %}
+            {%- if attr.setter_name %}
+
+                {%- if attr.dtype.c_name == "char[]" %}
+{{ setter_char(attr) }}
+                {%- else %}
+{{ setter_byval(attr) }}
+{% endif %}
+
+            {%- endif %}
+            {%- if attr.caller_name %}
+                {%- set comma = joiner(", ") %}
+
+{{attr.dtype.c_name}} {{ instance.name | capitalize_first }}_::{{attr.name}}({%- for arg in attr.arguments %}{{ comma() }}{{arg.dtype.c_name}} {{ arg.name }} {%- endfor %})
+{
+    {%- if attr.arguments|length == 0 %}
+    this->send({{attr.ep_id}}, this->_data, 0, true);
+    {%- else %}
+    uint8_t data_len = 0;
+        {%- for arg in attr.arguments %}
+    write_le({{ arg.name }}, this->_data + data_len);
+    data_len += sizeof({{ arg.name }});
+        {%- endfor %}
+
+    this->send({{attr.ep_id}}, this->_data, data_len, false);
+    {%- endif %}
+
+    {%- if attr.dtype.c_name != "void" %}
+    {{attr.dtype.c_name}} value = 0;
+    this->send(17, this->_data, 0, true);
+    if (this->recv(17, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    {
+        read_le(&value, this->_data);
+    }
+    return value;
+    {%- endif %}
+}
+            {%- endif %}
+        {%- endif %}
+    {%- endfor %}
+{%- endif %}
+
+
```

### Comparing `Avlos-0.5.2/avlos/templates/remote_object.hpp.jinja` & `Avlos-0.5.4/avlos/templates/device.hpp.jinja`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,92 @@
-/*
-* This file was automatically generated using Avlos.
-* https://github.com/tinymovr/avlos
-*
-* Any changes to this file will be overwritten when
-* content is regenerated.
-*/
-
-#pragma once
-
-#include <{{ helper_file | file_from_path }}>
-
-{%- if instance.remote_attributes %}
-    {%- for attr in instance.remote_attributes.values() %}
-        {%- if attr.remote_attributes %}
-#include <{{attr.name}}.hpp>
-        {%- endif %}
-    {%- endfor %}
-{%- endif %}
-
-class {{ instance.name | capitalize_first }}_ : Node
-{
-    public:
-
-        {{ instance.name | capitalize_first }}_(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb):
-            Node(_can_node_id, _send_cb, _recv_cb) 
-{%- if instance.remote_attributes %}
-    {%- for attr in instance.remote_attributes.values() %}
-        {%- if attr.remote_attributes %}
-            , {{attr.name}}(_can_node_id, _send_cb, _recv_cb)
-        {%- endif %}
-    {%- endfor %}
-{%- endif %} {};
-
-    {%- if instance.remote_attributes %}
-        {%- for attr in instance.remote_attributes.values() %}
-            {%- if attr.remote_attributes %}
-        {{attr.name | capitalize_first}}_ {{attr.name}};
-
-            {%- elif attr.getter_name %}
-                    {%- if attr.dtype.c_name == "char[]" %}
-        void get_{{attr.name}}(char out_value[]);
-                    {%- else %}
-        {{attr.dtype.c_name}} get_{{attr.name}}(void);
-                    {%- endif %}
-            {%- endif %}
-            {%- if attr.setter_name %}
-                    {%- if attr.dtype.c_name == "char[]" %}
-        void set_{{attr.name}}(char value[]);
-                    {%- else %}
-        void set_{{attr.name}}({{attr.dtype.c_name}} value);
-                    {%- endif %}
-            {%- endif %}
-            {%- if attr.caller_name %}
-                {%- set comma = joiner(", ") %}
-        {{attr.dtype.c_name}} {{attr.name}}({%- for arg in attr.arguments %}{{ comma() }}{{arg.dtype.c_name}} {{ arg.name }} {%- endfor %});
-            {%- endif %}
-        
-        {%- endfor %}
-    {%- endif %}
-
-};
+/*
+* This file was automatically generated using Avlos.
+* https://github.com/tinymovr/avlos
+*
+* Any changes to this file will be overwritten when
+* content is regenerated.
+*/
+
+#pragma once
+
+#include <{{ helper_file | file_from_path }}>
+{%- for include in includes %}
+#include <{{ include }}>
+{%- endfor %}
+
+{%- if instance.remote_attributes %}
+    {%- for attr in instance.remote_attributes.values() %}
+        {%- if attr.remote_attributes %}
+#include <{{attr.name}}.hpp>
+        {%- endif %}
+    {%- endfor %}
+{%- endif %}
+
+static uint32_t avlos_proto_hash = {{ instance.hash_uint32 }};
+
+{%- for ep in instance | bitmask_eps %}
+
+enum {{ ep.full_name | replace(".", "_") }}_flags
+{
+    {%- set comma = joiner(", ") %}
+    {{ ep.full_name | replace(".", "_") | upper }}_NONE = 0,
+    {%- for flag in ep.bitmask %}{{ comma() }}
+    {{ ep.full_name | replace(".", "_") | upper }}_{{ flag.name }} = (1 << {{ loop.index0 }})
+    {%- endfor %}
+};
+{%- endfor %}
+
+{%- for ep in instance | enum_eps %}
+
+enum {{ ep.full_name | replace(".", "_") }}_options
+{
+    {%- set comma = joiner(", ") %}
+    {%- for option in ep.options %}{{ comma() }}
+    {{ ep.full_name | replace(".", "_") | upper }}_{{ option.name }} = {{ loop.index0 }}
+    {%- endfor %}
+};
+{%- endfor %}
+
+class {{ device_name | capitalize_first }} : Node
+{
+    public:
+
+        {{ device_name | capitalize_first }}(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb):
+            Node(_can_node_id, _send_cb, _recv_cb, _delay_us_cb) 
+{%- if instance.remote_attributes %}
+    {%- for attr in instance.remote_attributes.values() %}
+        {%- if attr.remote_attributes %}
+            , {{attr.name}}(_can_node_id, _send_cb, _recv_cb, _delay_us_cb)
+        {%- endif %}
+    {%- endfor %}
+{%- endif %} {};
+
+    {%- if instance.remote_attributes %}
+        {%- for attr in instance.remote_attributes.values() %}
+            {%- if attr.remote_attributes %}
+        {{attr.name | capitalize_first}}_ {{attr.name}};
+
+            {%- else %}
+                {%- if attr.getter_name %}
+                    {%- if attr.dtype.c_name == "char[]" %}
+        void get_{{attr.name}}(char out_value[]);
+                    {%- else %}
+        {{attr.dtype.c_name}} get_{{attr.name}}(void);
+                    {%- endif %}
+                {%- endif %}
+                {%- if attr.setter_name %}
+                    {%- if attr.dtype.c_name == "char[]" %}
+        void set_{{attr.name}}(char value[]);
+                    {%- else %}
+        void set_{{attr.name}}({{attr.dtype.c_name}} value);
+                    {%- endif %}
+                {%- endif %}
+                {%- if attr.caller_name %}
+                    {%- set comma = joiner(", ") %}
+        {{attr.dtype.c_name}} {{attr.name}}({%- for arg in attr.arguments %}{{ comma() }}{{arg.dtype.c_name}} {{ arg.name }} {%- endfor %});
+                {%- endif %}
+
+            {%- endif %}
+        {%- endfor %}
+    {%- endif %}
+
+};
```

### Comparing `Avlos-0.5.2/avlos/unit_field.py` & `Avlos-0.5.4/avlos/unit_field.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from marshmallow import fields, ValidationError
-import pint
-
-_registry = None
-
-
-def get_registry():
-    """
-    Get or create a Pint unit registry with custom units
-    """
-    global _registry
-    if not _registry:
-        _registry = pint.UnitRegistry(autoconvert_offset_to_baseunit=True)
-        _registry.define("tick = turn / 8192")
-    return _registry
-
-
-class UnitField(fields.Field):
-    """
-    Marshmallow Field that serializes to a string
-    and deserializes to a Pint unit.
-    """
-
-    def _serialize(self, value, attr, obj, **kwargs):
-        if value is None:
-            return ""
-        return str(value)
-
-    def _deserialize(self, value, attr, data, **kwargs):
-        try:
-            return get_registry().Unit(value)
-        except ValueError as error:
-            raise ValidationError("Invalid Pint unit.") from error
+from marshmallow import fields, ValidationError
+import pint
+
+_registry = None
+
+
+def get_registry():
+    """
+    Get or create a Pint unit registry with custom units
+    """
+    global _registry
+    if not _registry:
+        _registry = pint.UnitRegistry(autoconvert_offset_to_baseunit=True)
+        _registry.define("tick = turn / 8192")
+    return _registry
+
+
+class UnitField(fields.Field):
+    """
+    Marshmallow Field that serializes to a string
+    and deserializes to a Pint unit.
+    """
+
+    def _serialize(self, value, attr, obj, **kwargs):
+        if value is None:
+            return ""
+        return str(value)
+
+    def _deserialize(self, value, attr, data, **kwargs):
+        try:
+            return get_registry().Unit(value)
+        except ValueError as error:
+            raise ValidationError("Invalid Pint unit.") from error
```

### Comparing `Avlos-0.5.2/example/device.yaml` & `Avlos-0.5.4/example/device.yaml`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-name: toaster
-version: "1.0"
-remote_attributes:
-- name: sn
-  dtype: uint32
-  getter_name: toaster_get_sn
-  summary: The unique device serial number.
-- name: heater
-  remote_attributes:
-  - name: temperature
-    dtype: float
-    unit: celsius
-    getter_name: toaster_get_heater_temp
-    summary: The toaster heater temperature.
-- name: relay
-  remote_attributes:
-  - name: relay_state
-    dtype: bool
-    getter_name: toaster_get_relay_state
-    setter_name: toaster_set_relay_state
+name: toaster
+version: "1.0"
+remote_attributes:
+- name: sn
+  dtype: uint32
+  getter_name: toaster_get_sn
+  summary: The unique device serial number.
+- name: heater
+  remote_attributes:
+  - name: temperature
+    dtype: float
+    unit: celsius
+    getter_name: toaster_get_heater_temp
+    summary: The toaster heater temperature.
+- name: relay
+  remote_attributes:
+  - name: relay_state
+    dtype: bool
+    getter_name: toaster_get_relay_state
+    setter_name: toaster_set_relay_state
     summary: The toaster heating relay element state.
```

### Comparing `Avlos-0.5.2/tests/definition/bad_device_missing_version.yaml` & `Avlos-0.5.4/tests/definition/good_device.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,93 @@
-# missing version in root node
-
-name: tm
-remote_attributes:
-  - name: sn
-    dtype: uint32
-    getter_name: system_get_sn
-    summary: Retrieve the unique device serial number.
-  - name: errors
-    flags: [NONE, UNDERVOLTAGE]
-    getter_name: system_get_error
-    summary: Retrieve any device errors.
-  - name: Vbus
-    dtype: float
-    unit: volt
-    getter_name: system_get_vbus
-    summary: Retrieve the bus voltage.
-  - name: reset
-    summary: Reset the device.
-    caller_name: system_reset
-    dtype: void
-    arguments: []
-  - name: move_to
-    summary: Move to
-    caller_name: move_to
-    dtype: void
-    arguments: 
-      - name: position
-        dtype: float
-      - name: max_vel
-        dtype: float
-  - name: controller
-    remote_attributes:
-      - name: set_pos_vel_setpoints
-        summary: Set position and velocity setpoints.
-        caller_name: controller_set_pos_vel_setpoints
-        dtype: void
-        arguments:
-          - name: pos_setpoint
-            dtype: float
-          - name: vel_setpoint
-            dtype: float
-  - name: motor
-    remote_attributes:
-      - name: R
-        dtype: float
-        unit: ohm
-        getter_name: motor_get_R
-        setter_name: motor_set_R
-        summary: Access the motor Resistance value.
-      - name: L
-        dtype: float
-        unit: henry
-        getter_name: motor_get_L
-        setter_name: motor_set_L
-        summary: Access the motor Inductance value.
-      - name: errors
-        flags: [NONE, R_OUT_OF_RANGE, L_OUT_OF_RANGE, INVALID_POLE_PAIRS]
-        getter_name: system_get_error
-        summary: Retrieve any motor errors.
-  - name: encoder
-    remote_attributes:
-      - name: position_estimate
-        dtype: float
-        unit: ticks
-        getter_name: encoder_get_pos_estimate
-        summary: Retrieve the encoder position estimate.
-      - name: bandwidth
-        dtype: float
-        unit: rad/s
-        getter_name: encoder_get_bandwidth
-        setter_name: encoder_set_bandwidth
-        summary: Access the encoder observer bandwidth.
-
+
+name: tm
+version: "0.1"
+remote_attributes:
+  - name: nickname
+    dtype: string
+    getter_name: system_get_name
+    setter_name: system_set_name 
+    summary: Retrieve the device name
+  - name: sn
+    dtype: uint32
+    getter_name: system_get_sn
+    summary: Retrieve the unique device serial number.
+  - name: errors
+    flags: [UNDERVOLTAGE]
+    meta: {dynamic: True}
+    getter_name: system_get_error
+    summary: Retrieve any device errors.
+    meta: {"lalala": "ok"}
+  - name: Vbus
+    dtype: float
+    unit: volt
+    meta: {dynamic: True}
+    getter_name: system_get_vbus
+    summary: Retrieve the bus voltage.
+  - name: reset
+    summary: Reset the device.
+    caller_name: system_reset
+    dtype: void
+    arguments: []
+    meta: {reload_data: True}
+  - name: move_to
+    summary: Move to
+    caller_name: move_to
+    dtype: void
+    arguments: 
+      - name: position
+        dtype: float
+      - name: max_vel
+        dtype: float
+  - name: controller
+    remote_attributes:
+      - name: set_pos_vel_setpoints
+        summary: Set position and velocity setpoints.
+        caller_name: set_position_velocity_setpoints
+        dtype: float
+        unit: ticks
+        arguments:
+          - name: pos_setpoint
+            dtype: float
+          - name: vel_setpoint
+            dtype: float
+      - name: mode
+        summary: Control mode
+        getter_name: controller_get_mode
+        setter_name: controller_set_mode
+        options: [IDLE, CLOSED_LOOP]
+  - name: motor
+    remote_attributes:
+      - name: R
+        dtype: float
+        unit: ohm
+        getter_name: motor_get_R
+        setter_name: motor_set_R
+        meta: {export: True}
+        summary: Access the motor Resistance value.
+      - name: L
+        dtype: float
+        unit: henry
+        getter_name: motor_get_L
+        setter_name: motor_set_L
+        meta: {export: True}
+        summary: Access the motor Inductance value.
+      - name: errors
+        flags: [R_OUT_OF_RANGE, L_OUT_OF_RANGE, INVALID_POLE_PAIRS]
+        getter_name: system_get_error
+        summary: Retrieve any motor errors.
+  - name: encoder
+    remote_attributes:
+      - name: position_estimate
+        dtype: float
+        unit: ticks
+        meta: {dynamic: True}
+        getter_name: encoder_get_pos_estimate
+        summary: Retrieve the encoder position estimate.
+      - name: bandwidth
+        dtype: float
+        unit: rad/s
+        meta: {export: True}
+        getter_name: encoder_get_bandwidth
+        setter_name: encoder_set_bandwidth
+        summary: Access the encoder observer bandwidth.
+
```

### Comparing `Avlos-0.5.2/tests/definition/good_device.yaml` & `Avlos-0.5.4/tests/definition/bad_device_missing_version.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,74 @@
-
-name: tm
-version: "0.1"
-remote_attributes:
-  - name: nickname
-    dtype: string
-    getter_name: system_get_name
-    setter_name: system_set_name 
-    summary: Retrieve the device name
-  - name: sn
-    dtype: uint32
-    getter_name: system_get_sn
-    summary: Retrieve the unique device serial number.
-  - name: errors
-    flags: [UNDERVOLTAGE]
-    meta: {dynamic: True}
-    getter_name: system_get_error
-    summary: Retrieve any device errors.
-    meta: {"lalala": "ok"}
-  - name: Vbus
-    dtype: float
-    unit: volt
-    meta: {dynamic: True}
-    getter_name: system_get_vbus
-    summary: Retrieve the bus voltage.
-  - name: reset
-    summary: Reset the device.
-    caller_name: system_reset
-    dtype: void
-    arguments: []
-    meta: {reload_data: True}
-  - name: move_to
-    summary: Move to
-    caller_name: move_to
-    dtype: void
-    arguments: 
-      - name: position
-        dtype: float
-      - name: max_vel
-        dtype: float
-  - name: controller
-    remote_attributes:
-      - name: set_pos_vel_setpoints
-        summary: Set position and velocity setpoints.
-        caller_name: set_position_velocity_setpoints
-        dtype: float
-        unit: ticks
-        arguments:
-          - name: pos_setpoint
-            dtype: float
-          - name: vel_setpoint
-            dtype: float
-      - name: mode
-        summary: Control mode
-        getter_name: controller_get_mode
-        setter_name: controller_set_mode
-        options: [IDLE, CLOSED_LOOP]
-  - name: motor
-    remote_attributes:
-      - name: R
-        dtype: float
-        unit: ohm
-        getter_name: motor_get_R
-        setter_name: motor_set_R
-        meta: {export: True}
-        summary: Access the motor Resistance value.
-      - name: L
-        dtype: float
-        unit: henry
-        getter_name: motor_get_L
-        setter_name: motor_set_L
-        meta: {export: True}
-        summary: Access the motor Inductance value.
-      - name: errors
-        flags: [R_OUT_OF_RANGE, L_OUT_OF_RANGE, INVALID_POLE_PAIRS]
-        getter_name: system_get_error
-        summary: Retrieve any motor errors.
-  - name: encoder
-    remote_attributes:
-      - name: position_estimate
-        dtype: float
-        unit: ticks
-        meta: {dynamic: True}
-        getter_name: encoder_get_pos_estimate
-        summary: Retrieve the encoder position estimate.
-      - name: bandwidth
-        dtype: float
-        unit: rad/s
-        meta: {export: True}
-        getter_name: encoder_get_bandwidth
-        setter_name: encoder_set_bandwidth
-        summary: Access the encoder observer bandwidth.
-
+# missing version in root node
+
+name: tm
+remote_attributes:
+  - name: sn
+    dtype: uint32
+    getter_name: system_get_sn
+    summary: Retrieve the unique device serial number.
+  - name: errors
+    flags: [NONE, UNDERVOLTAGE]
+    getter_name: system_get_error
+    summary: Retrieve any device errors.
+  - name: Vbus
+    dtype: float
+    unit: volt
+    getter_name: system_get_vbus
+    summary: Retrieve the bus voltage.
+  - name: reset
+    summary: Reset the device.
+    caller_name: system_reset
+    dtype: void
+    arguments: []
+  - name: move_to
+    summary: Move to
+    caller_name: move_to
+    dtype: void
+    arguments: 
+      - name: position
+        dtype: float
+      - name: max_vel
+        dtype: float
+  - name: controller
+    remote_attributes:
+      - name: set_pos_vel_setpoints
+        summary: Set position and velocity setpoints.
+        caller_name: controller_set_pos_vel_setpoints
+        dtype: void
+        arguments:
+          - name: pos_setpoint
+            dtype: float
+          - name: vel_setpoint
+            dtype: float
+  - name: motor
+    remote_attributes:
+      - name: R
+        dtype: float
+        unit: ohm
+        getter_name: motor_get_R
+        setter_name: motor_set_R
+        summary: Access the motor Resistance value.
+      - name: L
+        dtype: float
+        unit: henry
+        getter_name: motor_get_L
+        setter_name: motor_set_L
+        summary: Access the motor Inductance value.
+      - name: errors
+        flags: [NONE, R_OUT_OF_RANGE, L_OUT_OF_RANGE, INVALID_POLE_PAIRS]
+        getter_name: system_get_error
+        summary: Retrieve any motor errors.
+  - name: encoder
+    remote_attributes:
+      - name: position_estimate
+        dtype: float
+        unit: ticks
+        getter_name: encoder_get_pos_estimate
+        summary: Retrieve the encoder position estimate.
+      - name: bandwidth
+        dtype: float
+        unit: rad/s
+        getter_name: encoder_get_bandwidth
+        setter_name: encoder_set_bandwidth
+        summary: Access the encoder observer bandwidth.
+
```

### Comparing `Avlos-0.5.2/tests/dummy_channel.py` & `Avlos-0.5.4/tests/dummy_channel.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-class DummyChannel:
-    """
-    Dummy channel class
-    """
-
-    def __init__(self, value=0):
-        self.value = value
-        self.write = False
-
-    def send(self, data, ep_id):
-        if self.write:
-            self.value = data
-
-    def recv(self, ep_id):
-        return [self.value]
-
-    def set_value(self, value):
-        self.value = value
-
-    def write_on(self):
-        self.write = True
-
-    def write_off(self):
-        self.write = False
-
-    @property
-    def serializer(self):
-        return DummyCodec()
-
-
-class DummyCodec:
-    """
-    Dummy CODEC class
-    """
-
-    def serialize(self, values, *args):
-        return values[0]
-
-    def deserialize(self, data, *args):
-        return data
+class DummyChannel:
+    """
+    Dummy channel class
+    """
+
+    def __init__(self, value=0):
+        self.value = value
+        self.write = False
+
+    def send(self, data, ep_id):
+        if self.write:
+            self.value = data
+
+    def recv(self, ep_id):
+        return [self.value]
+
+    def set_value(self, value):
+        self.value = value
+
+    def write_on(self):
+        self.write = True
+
+    def write_off(self):
+        self.write = False
+
+    @property
+    def serializer(self):
+        return DummyCodec()
+
+
+class DummyCodec:
+    """
+    Dummy CODEC class
+    """
+
+    def serialize(self, values, *args):
+        return values[0]
+
+    def deserialize(self, data, *args):
+        return data
```

### Comparing `Avlos-0.5.2/tests/test_counter.py` & `Avlos-0.5.4/tests/test_counter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from avlos.counter import get_counter, make_counter, delete_counter
-
-import unittest
-
-
-class TestCounter(unittest.TestCase):
-
-    def test_make_counter_return(self):
-        self.assertIsNone(make_counter())
-
-    def test_get_counter(self):
-        delete_counter()
-        self.assertIsNone(get_counter())
-        make_counter()
-        self.assertIsNotNone(get_counter())
-
-    def test_make_counter(self):
-        make_counter()
-        counter1 = get_counter()
-        counter2 = get_counter()
-        make_counter()
-        counter3 = make_counter()
-        self.assertEqual(counter1, counter2)
-        self.assertNotEqual(counter1, counter3)
-
-    def test_counter_next(self):
-        make_counter()
-        counter = get_counter()
-        self.assertEqual(0, counter.count)
-        self.assertEqual(0, counter.next())
-        self.assertEqual(1, counter.next())
-        self.assertEqual(counter.next()+1, counter.count)
+from avlos.counter import get_counter, make_counter, delete_counter
+
+import unittest
+
+
+class TestCounter(unittest.TestCase):
+    def test_make_counter_return(self):
+        self.assertIsNone(make_counter())
+
+    def test_get_counter(self):
+        delete_counter()
+        self.assertIsNone(get_counter())
+        make_counter()
+        self.assertIsNotNone(get_counter())
+
+    def test_make_counter(self):
+        make_counter()
+        counter1 = get_counter()
+        counter2 = get_counter()
+        make_counter()
+        counter3 = make_counter()
+        self.assertEqual(counter1, counter2)
+        self.assertNotEqual(counter1, counter3)
+
+    def test_counter_next(self):
+        make_counter()
+        counter = get_counter()
+        self.assertEqual(0, counter.count)
+        self.assertEqual(0, counter.next())
+        self.assertEqual(1, counter.next())
+        self.assertEqual(counter.next() + 1, counter.count)
```

### Comparing `Avlos-0.5.2/tests/test_functions.py` & `Avlos-0.5.4/tests/test_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from avlos.generators.filters import as_include, file_from_path, capitalize_first
-import unittest
-
-
-class TestFunctions(unittest.TestCase):
-
-    def test_file_from_path_filter(self):
-         self.assertEqual("test_functions.py", file_from_path(__file__))
-
-    def test_jinja_as_include_filter(self):
-        self.assertEqual("<test.h>", as_include("test.h"))
-        self.assertEqual("<test.h>", as_include("<test.h>"))
-        self.assertEqual('"test.h"', as_include('"test.h"'))
-
-    def test_capitalize_first(self):
-        self.assertEqual(capitalize_first("bob Meadow"), "Bob Meadow")
+from avlos.generators.filters import as_include, file_from_path, capitalize_first
+import unittest
+
+
+class TestFunctions(unittest.TestCase):
+    def test_file_from_path_filter(self):
+        self.assertEqual("test_functions.py", file_from_path(__file__))
+
+    def test_jinja_as_include_filter(self):
+        self.assertEqual("<test.h>", as_include("test.h"))
+        self.assertEqual("<test.h>", as_include("<test.h>"))
+        self.assertEqual('"test.h"', as_include('"test.h"'))
+
+    def test_capitalize_first(self):
+        self.assertEqual(capitalize_first("bob Meadow"), "Bob Meadow")
```

### Comparing `Avlos-0.5.2/tests/test_generation.py` & `Avlos-0.5.4/tests/test_generation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import yaml
-import subprocess
-from pathlib import Path
-import importlib.resources
-from avlos.deserializer import deserialize
-from avlos.processor import process_with_config_file
-import avlos.generators.generator_c as generator_c
-import avlos.generators.generator_cpp as generator_cpp
-import avlos.generators.generator_rst as generator_rst
-from rstcheck_core import _extras, config as config_mod, runner
-import unittest
-
-
-class TestGeneration(unittest.TestCase):
-    def test_c_output_manual(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        header_path_str = str(
-            importlib.resources.files("tests").joinpath("outputs/test.h")
-        )
-        impl_path_str = str(
-            importlib.resources.files("tests").joinpath("outputs/test.c")
-        )
-        with open(def_path_str) as device_desc_stream:
-            obj = deserialize(yaml.safe_load(device_desc_stream))
-            config = {
-                "hash_string": "0x9e8dc7ac",
-                "paths": {
-                    "output_header": header_path_str,
-                    "output_impl": impl_path_str,
-                },
-                "c_includes": {"src/common.h"},
-            }
-            generator_c.process(obj, config)
-
-            result = subprocess.run(
-                ["cppcheck", "--error-exitcode=1", header_path_str, impl_path_str],
-                stdout=subprocess.DEVNULL,
-            )
-            self.assertEqual(result.returncode, 0)
-
-    def test_cpp_output_manual(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        helper_path_str = str(
-            importlib.resources.files("tests").joinpath("outputs/helpers.hpp")
-        )
-        header_path_str = str(
-            importlib.resources.files("tests").joinpath("outputs/base_device.hpp")
-        )
-        impl_path_str = str(
-            importlib.resources.files("tests").joinpath("outputs/base_device.cpp")
-        )
-        with open(def_path_str) as device_desc_stream:
-            obj = deserialize(yaml.safe_load(device_desc_stream))
-            config = {
-                "hash_string": "0x9e8dc7ac",
-                "paths": {
-                    "output_helpers": helper_path_str,
-                    "output_header": header_path_str,
-                    "output_impl": impl_path_str,
-                },
-                "header_includes": {"string"},
-            }
-            generator_cpp.process(obj, config)
-
-            result = subprocess.run(
-                ["cppcheck", "--error-exitcode=1", header_path_str, impl_path_str],
-                stdout=subprocess.DEVNULL,
-            )
-            self.assertEqual(result.returncode, 0)
-
-    def test_rst_output_manual(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        out_path_str = str(
-            importlib.resources.files("tests").joinpath("outputs/test.rst")
-        )
-        with open(def_path_str) as device_desc_stream:
-            obj = deserialize(yaml.safe_load(device_desc_stream))
-            config = {
-                "hash_string": "0x9e8dc7ac",
-                "paths": {"output_file": out_path_str},
-            }
-            generator_rst.process(obj, config)
-
-        rstcheck_config = config_mod.RstcheckConfig()
-        path = Path(out_path_str)
-        _runner = runner.RstcheckMainRunner(
-            check_paths=[path], rstcheck_config=rstcheck_config, overwrite_config=False
-        )
-        _runner.check()
-        _runner.print_result()
-            
-    def test_avlos_config(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        config_file_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/avlos_config.yaml")
-        )
-        with open(def_path_str) as device_desc_stream:
-            obj = deserialize(yaml.safe_load(device_desc_stream))
-            process_with_config_file(obj, config_file_path_str)
+import yaml
+import subprocess
+from pathlib import Path
+import importlib.resources
+from avlos.deserializer import deserialize
+from avlos.processor import process_with_config_file
+import avlos.generators.generator_c as generator_c
+import avlos.generators.generator_cpp as generator_cpp
+import avlos.generators.generator_rst as generator_rst
+from rstcheck_core import _extras, config as config_mod, runner
+import unittest
+
+
+class TestGeneration(unittest.TestCase):
+    def test_c_output_manual(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        header_path_str = str(
+            importlib.resources.files("tests").joinpath("outputs/test.h")
+        )
+        impl_path_str = str(
+            importlib.resources.files("tests").joinpath("outputs/test.c")
+        )
+        with open(def_path_str) as device_desc_stream:
+            obj = deserialize(yaml.safe_load(device_desc_stream))
+            config = {
+                "hash_string": "0x9e8dc7ac",
+                "paths": {
+                    "output_header": header_path_str,
+                    "output_impl": impl_path_str,
+                },
+                "c_includes": {"src/common.h"},
+            }
+            generator_c.process(obj, config)
+
+            result = subprocess.run(
+                ["cppcheck", "--error-exitcode=1", header_path_str, impl_path_str],
+                stdout=subprocess.DEVNULL,
+            )
+            self.assertEqual(result.returncode, 0)
+
+    def test_cpp_output_manual(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        helper_path_str = str(
+            importlib.resources.files("tests").joinpath("outputs/helpers.hpp")
+        )
+        header_path_str = str(
+            importlib.resources.files("tests").joinpath("outputs/base_device.hpp")
+        )
+        impl_path_str = str(
+            importlib.resources.files("tests").joinpath("outputs/base_device.cpp")
+        )
+        with open(def_path_str) as device_desc_stream:
+            obj = deserialize(yaml.safe_load(device_desc_stream))
+            config = {
+                "hash_string": "0x9e8dc7ac",
+                "paths": {
+                    "output_helpers": helper_path_str,
+                    "output_header": header_path_str,
+                    "output_impl": impl_path_str,
+                },
+                "header_includes": {"string"},
+            }
+            generator_cpp.process(obj, config)
+
+            result = subprocess.run(
+                ["cppcheck", "--error-exitcode=1", header_path_str, impl_path_str],
+                stdout=subprocess.DEVNULL,
+            )
+            self.assertEqual(result.returncode, 0)
+
+    def test_rst_output_manual(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        out_path_str = str(
+            importlib.resources.files("tests").joinpath("outputs/test.rst")
+        )
+        with open(def_path_str) as device_desc_stream:
+            obj = deserialize(yaml.safe_load(device_desc_stream))
+            config = {
+                "hash_string": "0x9e8dc7ac",
+                "paths": {"output_file": out_path_str},
+            }
+            generator_rst.process(obj, config)
+
+        rstcheck_config = config_mod.RstcheckConfig()
+        path = Path(out_path_str)
+        _runner = runner.RstcheckMainRunner(
+            check_paths=[path], rstcheck_config=rstcheck_config, overwrite_config=False
+        )
+        _runner.check()
+        _runner.print_result()
+
+    def test_avlos_config(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        config_file_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/avlos_config.yaml")
+        )
+        with open(def_path_str) as device_desc_stream:
+            obj = deserialize(yaml.safe_load(device_desc_stream))
+            process_with_config_file(obj, config_file_path_str)
```

### Comparing `Avlos-0.5.2/tests/test_impex.py` & `Avlos-0.5.4/tests/test_impex.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-import json
-import yaml
-import importlib.resources
-from avlos.deserializer import deserialize
-from avlos.unit_field import get_registry
-from avlos.json_codec import AvlosEncoder
-import unittest
-from tests.dummy_channel import DummyChannel
-
-
-class TestImpex(unittest.TestCase):
-    
-    def test_import_export_root_object(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        with open(def_path_str) as device_description:
-            obj = deserialize(yaml.safe_load(device_description))
-            obj._channel = DummyChannel()
-            obj._channel.set_value(0)
-            func = obj.motor.remote_attributes["R"]
-            root = func.root
-            self.assertEqual(obj, root)
-            values = root.export_values()
-            json_string = json.dumps(values, cls=AvlosEncoder)
-            imported_values = json.loads(json_string)
-            root.import_values(imported_values)
-
-
-            
- 
+import json
+import yaml
+import importlib.resources
+from avlos.deserializer import deserialize
+from avlos.unit_field import get_registry
+from avlos.json_codec import AvlosEncoder
+import unittest
+from tests.dummy_channel import DummyChannel
+
+
+class TestImpex(unittest.TestCase):
+    def test_import_export_root_object(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        with open(def_path_str) as device_description:
+            obj = deserialize(yaml.safe_load(device_description))
+            obj._channel = DummyChannel()
+            obj._channel.set_value(0)
+            func = obj.motor.remote_attributes["R"]
+            root = func.root
+            self.assertEqual(obj, root)
+            values = root.export_values()
+            json_string = json.dumps(values, cls=AvlosEncoder)
+            imported_values = json.loads(json_string)
+            root.import_values(imported_values)
```

### Comparing `Avlos-0.5.2/tests/test_remote_objects.py` & `Avlos-0.5.4/tests/test_remote_objects.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,92 @@
-import yaml
-import importlib.resources
-from avlos.deserializer import deserialize
-from avlos.unit_field import get_registry
-import unittest
-from tests.dummy_channel import DummyChannel
-
-_reg = get_registry()
-
-
-class TestRemoteObjects(unittest.TestCase):
-    
-    def test_read_remote_properties(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        with open(def_path_str) as device_description:
-
-            obj = deserialize(yaml.safe_load(device_description))
-            obj._channel = DummyChannel()
-
-            self.assertEqual(0, obj.Vbus)
-            obj._channel.set_value(12.0)
-            self.assertEqual(12.0 * _reg("volt"), obj.Vbus)
-            obj._channel.set_value(24.0)
-            self.assertEqual(24.0 * _reg("volt"), obj.Vbus)
-
-            obj._channel.set_value(0.1)
-            self.assertEqual(0.1 * _reg("ohm"), obj.motor.R)
-
-            obj.channel.set_value("lalala")
-            self.assertEqual(obj.nickname, "lalala")
-
-            obj.controller.set_pos_vel_setpoints(0, 0)
-
-            obj._channel.write_on()
-            obj.nickname = "other"
-            obj._channel.write_off()
-            self.assertEqual(obj.nickname, "other")
-
-    def test_remote_enum(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        with open(def_path_str) as device_description:
-
-            obj = deserialize(yaml.safe_load(device_description))
-            obj._channel = DummyChannel()
-            modes = obj.controller.remote_attributes["mode"].options
-            obj._channel.set_value(0)
-            self.assertEqual(obj.controller.mode, modes.IDLE)
-            obj._channel.set_value(1)
-            self.assertEqual(obj.controller.mode, modes.CLOSED_LOOP)
-
-    def test_remote_function_call(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        with open(def_path_str) as device_description:
-            obj = deserialize(yaml.safe_load(device_description))
-            obj._channel = DummyChannel()
-
-        self.assertEqual(0, obj.controller.set_pos_vel_setpoints(1, 2))
-        obj._channel.set_value(100.0)
-        self.assertEqual(100 * _reg("tick"), obj.controller.set_pos_vel_setpoints(0, 0))
-
-    def test_non_existent_remote_attributes_fail(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        with open(def_path_str) as device_description:
-            obj = deserialize(yaml.safe_load(device_description))
-            obj._channel = DummyChannel()
-            with self.assertRaises(AttributeError):
-                val = obj.foo
-                print(val)
-            with self.assertRaises(AttributeError):
-                val = obj.controller.bar
-                print(val)
-
-    def test_meta_dictionary(self):
-        def_path_str = str(
-            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
-        )
-        with open(def_path_str) as device_description:
-            obj = deserialize(yaml.safe_load(device_description))
-            self.assertEqual(1, len(obj.errors.meta))
-            self.assertEqual("ok", obj.errors.meta["lalala"])
-            self.assertEqual(1, len(obj.reset.meta))
-            self.assertEqual(True, obj.reset.meta["reload_data"])
-            self.assertEqual(0, len(obj.sn.meta))
-            with self.assertRaises(KeyError):
-                d = obj.sn.meta["reload_data"]
+import yaml
+import importlib.resources
+from avlos.deserializer import deserialize
+from avlos.unit_field import get_registry
+import unittest
+from tests.dummy_channel import DummyChannel
+
+_reg = get_registry()
+
+
+class TestRemoteObjects(unittest.TestCase):
+    def test_read_remote_properties(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        with open(def_path_str) as device_description:
+
+            obj = deserialize(yaml.safe_load(device_description))
+            obj._channel = DummyChannel()
+
+            self.assertEqual(0, obj.Vbus)
+            obj._channel.set_value(12.0)
+            self.assertEqual(12.0 * _reg("volt"), obj.Vbus)
+            obj._channel.set_value(24.0)
+            self.assertEqual(24.0 * _reg("volt"), obj.Vbus)
+
+            obj._channel.set_value(0.1)
+            self.assertEqual(0.1 * _reg("ohm"), obj.motor.R)
+
+            obj.channel.set_value("lalala")
+            self.assertEqual(obj.nickname, "lalala")
+
+            obj.controller.set_pos_vel_setpoints(0, 0)
+
+            obj._channel.write_on()
+            obj.nickname = "other"
+            obj._channel.write_off()
+            self.assertEqual(obj.nickname, "other")
+
+    def test_remote_enum(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        with open(def_path_str) as device_description:
+
+            obj = deserialize(yaml.safe_load(device_description))
+            obj._channel = DummyChannel()
+            modes = obj.controller.remote_attributes["mode"].options
+            obj._channel.set_value(0)
+            self.assertEqual(obj.controller.mode, modes.IDLE)
+            obj._channel.set_value(1)
+            self.assertEqual(obj.controller.mode, modes.CLOSED_LOOP)
+
+    def test_remote_function_call(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        with open(def_path_str) as device_description:
+            obj = deserialize(yaml.safe_load(device_description))
+            obj._channel = DummyChannel()
+
+        self.assertEqual(0, obj.controller.set_pos_vel_setpoints(1, 2))
+        obj._channel.set_value(100.0)
+        self.assertEqual(100 * _reg("tick"), obj.controller.set_pos_vel_setpoints(0, 0))
+
+    def test_non_existent_remote_attributes_fail(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        with open(def_path_str) as device_description:
+            obj = deserialize(yaml.safe_load(device_description))
+            obj._channel = DummyChannel()
+            with self.assertRaises(AttributeError):
+                val = obj.foo
+                print(val)
+            with self.assertRaises(AttributeError):
+                val = obj.controller.bar
+                print(val)
+
+    def test_meta_dictionary(self):
+        def_path_str = str(
+            importlib.resources.files("tests").joinpath("definition/good_device.yaml")
+        )
+        with open(def_path_str) as device_description:
+            obj = deserialize(yaml.safe_load(device_description))
+            self.assertEqual(1, len(obj.errors.meta))
+            self.assertEqual("ok", obj.errors.meta["lalala"])
+            self.assertEqual(1, len(obj.reset.meta))
+            self.assertEqual(True, obj.reset.meta["reload_data"])
+            self.assertEqual(0, len(obj.sn.meta))
+            with self.assertRaises(KeyError):
+                d = obj.sn.meta["reload_data"]
```

