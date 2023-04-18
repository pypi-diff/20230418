# Comparing `tmp/marshy-3.0.0.tar.gz` & `tmp/marshy-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/marshy-3.0.0.tar", last modified: Wed Nov 30 22:13:50 2022, max compression
+gzip compressed data, was "dist/marshy-4.0.0.tar", last modified: Tue Apr 18 21:22:40 2023, max compression
```

## Comparing `marshy-3.0.0.tar` & `marshy-4.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/
--rw-r--r--   0 tofarr     (501) staff       (20)     1069 2021-09-27 22:36:51.000000 marshy-3.0.0/LICENSE
--rw-r--r--   0 tofarr     (501) staff       (20)     8717 2022-11-30 22:13:50.000000 marshy-3.0.0/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     8251 2022-11-30 22:13:29.000000 marshy-3.0.0/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/marshy/
--rw-r--r--   0 tofarr     (501) staff       (20)     1226 2021-11-14 22:08:58.000000 marshy-3.0.0/marshy/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2022-11-30 22:12:24.000000 marshy-3.0.0/marshy/__version__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       43 2021-09-25 17:26:10.000000 marshy-3.0.0/marshy/errors.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/marshy/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-09-25 22:20:47.000000 marshy-3.0.0/marshy/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4879 2022-11-30 22:09:24.000000 marshy-3.0.0/marshy/factory/dataclass_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      727 2021-09-28 02:53:11.000000 marshy-3.0.0/marshy/factory/enum_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      643 2021-11-05 23:12:05.000000 marshy-3.0.0/marshy/factory/factory_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1848 2022-08-11 16:57:36.000000 marshy-3.0.0/marshy/factory/impl_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1003 2022-11-30 21:49:19.000000 marshy-3.0.0/marshy/factory/list_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      774 2022-01-23 15:06:09.000000 marshy-3.0.0/marshy/factory/marshaller_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1220 2021-09-28 02:53:11.000000 marshy-3.0.0/marshy/factory/optional_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1241 2022-01-24 23:28:38.000000 marshy-3.0.0/marshy/factory/tuple_marshaller_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1082 2021-09-28 02:53:11.000000 marshy-3.0.0/marshy/factory/union_marshaller_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/marshy/marshaller/
--rw-r--r--   0 tofarr     (501) staff       (20)      519 2021-11-03 13:37:59.000000 marshy-3.0.0/marshy/marshaller/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      452 2021-10-09 16:07:39.000000 marshy-3.0.0/marshy/marshaller/as_str_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      464 2022-02-06 00:41:38.000000 marshy-3.0.0/marshy/marshaller/bool_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      518 2021-11-03 13:39:03.000000 marshy-3.0.0/marshy/marshaller/datetime_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      734 2021-09-28 17:30:24.000000 marshy-3.0.0/marshy/marshaller/deferred_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1212 2021-09-28 02:53:11.000000 marshy-3.0.0/marshy/marshaller/enum_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      752 2022-01-24 23:12:00.000000 marshy-3.0.0/marshy/marshaller/iterable_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      518 2021-12-07 14:44:56.000000 marshy-3.0.0/marshy/marshaller/json_str_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      480 2022-02-06 00:41:38.000000 marshy-3.0.0/marshy/marshaller/marshaller_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      352 2021-09-28 02:53:11.000000 marshy-3.0.0/marshy/marshaller/no_op_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1825 2022-07-31 11:30:41.000000 marshy-3.0.0/marshy/marshaller/obj_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      761 2021-09-28 02:53:11.000000 marshy-3.0.0/marshy/marshaller/optional_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      453 2021-09-28 17:30:50.000000 marshy-3.0.0/marshy/marshaller/primitive_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1729 2022-07-31 11:31:15.000000 marshy-3.0.0/marshy/marshaller/property_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      913 2022-02-10 02:40:00.000000 marshy-3.0.0/marshy/marshaller/tuple_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1861 2021-11-17 23:59:03.000000 marshy-3.0.0/marshy/marshaller/type_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1539 2021-11-18 00:03:28.000000 marshy-3.0.0/marshy/marshaller/union_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2141 2022-07-26 13:23:28.000000 marshy-3.0.0/marshy/marshaller_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)      199 2021-12-07 03:19:47.000000 marshy-3.0.0/marshy/types.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1009 2021-10-29 15:31:13.000000 marshy-3.0.0/marshy/utils.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/marshy.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)     8717 2022-11-30 22:13:49.000000 marshy-3.0.0/marshy.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     2192 2022-11-30 22:13:49.000000 marshy-3.0.0/marshy.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2022-11-30 22:13:49.000000 marshy-3.0.0/marshy.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2022-11-30 22:13:49.000000 marshy-3.0.0/marshy.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       34 2022-11-30 22:13:49.000000 marshy-3.0.0/marshy.egg-info/top_level.txt
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/marshy_config_default/
--rw-r--r--   0 tofarr     (501) staff       (20)     1819 2022-01-24 23:05:39.000000 marshy-3.0.0/marshy_config_default/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2022-11-30 22:13:50.000000 marshy-3.0.0/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      753 2021-09-28 02:54:22.000000 marshy-3.0.0/setup.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/test/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-09-26 14:52:20.000000 marshy-3.0.0/test/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2022-11-30 22:13:50.000000 marshy-3.0.0/test/performance/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-10-09 15:23:45.000000 marshy-3.0.0/test/performance/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      716 2021-10-09 15:20:22.000000 marshy-3.0.0/test/performance/fixtures.py
--rw-r--r--   0 tofarr     (501) staff       (20)      316 2021-10-09 15:28:35.000000 marshy-3.0.0/test/performance/marshmallow_performance.py
--rw-r--r--   0 tofarr     (501) staff       (20)      252 2021-10-09 15:28:35.000000 marshy-3.0.0/test/performance/marshy_performance.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4118 2021-12-07 14:44:39.000000 marshy-3.0.0/test/test_custom_marshalling.py
--rw-r--r--   0 tofarr     (501) staff       (20)      625 2022-07-31 11:39:59.000000 marshy-3.0.0/test/test_customize_exclude_dumped_values.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1704 2022-01-23 15:06:09.000000 marshy-3.0.0/test/test_factory_ordering.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1752 2022-07-26 13:42:12.000000 marshy-3.0.0/test/test_futures.py
--rw-r--r--   0 tofarr     (501) staff       (20)      975 2022-01-24 23:31:34.000000 marshy-3.0.0/test/test_immutable.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1612 2022-08-11 16:59:14.000000 marshy-3.0.0/test/test_impl_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      703 2021-09-28 02:53:11.000000 marshy-3.0.0/test/test_marshall_bool.py
--rw-r--r--   0 tofarr     (501) staff       (20)      710 2021-11-03 13:45:28.000000 marshy-3.0.0/test/test_marshall_datetime.py
--rw-r--r--   0 tofarr     (501) staff       (20)      765 2021-09-28 02:53:11.000000 marshy-3.0.0/test/test_marshall_deferred.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1102 2021-09-28 02:53:11.000000 marshy-3.0.0/test/test_marshall_enum.py
--rw-r--r--   0 tofarr     (501) staff       (20)      474 2021-12-07 14:43:04.000000 marshy-3.0.0/test/test_marshall_freeform.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1053 2022-02-02 23:23:37.000000 marshy-3.0.0/test/test_marshall_iterable.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3799 2022-02-09 16:01:32.000000 marshy-3.0.0/test/test_marshall_obj.py
--rw-r--r--   0 tofarr     (501) staff       (20)      368 2021-09-28 02:53:11.000000 marshy-3.0.0/test/test_marshall_optional.py
--rw-r--r--   0 tofarr     (501) staff       (20)      542 2021-09-28 02:53:11.000000 marshy-3.0.0/test/test_marshall_primitive.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3023 2022-11-30 22:11:46.000000 marshy-3.0.0/test/test_marshall_properties.py
--rw-r--r--   0 tofarr     (501) staff       (20)      627 2022-02-10 02:49:32.000000 marshy-3.0.0/test/test_marshall_tuple.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1223 2021-11-18 00:01:20.000000 marshy-3.0.0/test/test_marshall_type.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1898 2021-11-18 00:13:22.000000 marshy-3.0.0/test/test_marshall_union.py
--rw-r--r--   0 tofarr     (501) staff       (20)      355 2021-10-29 15:33:04.000000 marshy-3.0.0/test/test_marshall_uuid.py
--rw-r--r--   0 tofarr     (501) staff       (20)      795 2021-10-09 15:50:08.000000 marshy-3.0.0/test/test_performance.py
--rw-r--r--   0 tofarr     (501) staff       (20)      975 2021-12-07 03:33:25.000000 marshy-3.0.0/test/test_utils.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/
+-rw-r--r--   0 tofarr     (501) staff       (20)     1069 2021-09-27 22:36:51.000000 marshy-4.0.0/LICENSE
+-rw-r--r--   0 tofarr     (501) staff       (20)     8717 2023-04-18 21:22:40.000000 marshy-4.0.0/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     8251 2022-11-30 22:13:29.000000 marshy-4.0.0/README.md
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy/
+-rw-r--r--   0 tofarr     (501) staff       (20)     1226 2021-11-14 22:08:58.000000 marshy-4.0.0/marshy/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:15:19.000000 marshy-4.0.0/marshy/__version__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       43 2021-09-25 17:26:10.000000 marshy-4.0.0/marshy/errors.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy/factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-09-25 22:20:47.000000 marshy-4.0.0/marshy/factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4879 2022-11-30 22:09:24.000000 marshy-4.0.0/marshy/factory/dataclass_marshaller_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      727 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/factory/enum_marshaller_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      643 2021-11-05 23:12:05.000000 marshy-4.0.0/marshy/factory/factory_marshaller_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1848 2022-08-11 16:57:36.000000 marshy-4.0.0/marshy/factory/impl_marshaller_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1003 2022-11-30 21:49:19.000000 marshy-4.0.0/marshy/factory/list_marshaller_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      774 2022-01-23 15:06:09.000000 marshy-4.0.0/marshy/factory/marshaller_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1220 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/factory/optional_marshaller_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1241 2022-01-24 23:28:38.000000 marshy-4.0.0/marshy/factory/tuple_marshaller_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1082 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/factory/union_marshaller_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy/marshaller/
+-rw-r--r--   0 tofarr     (501) staff       (20)      519 2021-11-03 13:37:59.000000 marshy-4.0.0/marshy/marshaller/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      452 2021-10-09 16:07:39.000000 marshy-4.0.0/marshy/marshaller/as_str_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      464 2022-02-06 00:41:38.000000 marshy-4.0.0/marshy/marshaller/bool_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      518 2021-11-03 13:39:03.000000 marshy-4.0.0/marshy/marshaller/datetime_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      734 2021-09-28 17:30:24.000000 marshy-4.0.0/marshy/marshaller/deferred_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1209 2023-04-18 21:16:33.000000 marshy-4.0.0/marshy/marshaller/enum_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      752 2022-01-24 23:12:00.000000 marshy-4.0.0/marshy/marshaller/iterable_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      518 2021-12-07 14:44:56.000000 marshy-4.0.0/marshy/marshaller/json_str_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      480 2022-02-06 00:41:38.000000 marshy-4.0.0/marshy/marshaller/marshaller_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      352 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/marshaller/no_op_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1825 2022-07-31 11:30:41.000000 marshy-4.0.0/marshy/marshaller/obj_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      761 2021-09-28 02:53:11.000000 marshy-4.0.0/marshy/marshaller/optional_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      453 2021-09-28 17:30:50.000000 marshy-4.0.0/marshy/marshaller/primitive_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1729 2022-07-31 11:31:15.000000 marshy-4.0.0/marshy/marshaller/property_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      913 2022-02-10 02:40:00.000000 marshy-4.0.0/marshy/marshaller/tuple_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1861 2021-11-17 23:59:03.000000 marshy-4.0.0/marshy/marshaller/type_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1539 2021-11-18 00:03:28.000000 marshy-4.0.0/marshy/marshaller/union_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2141 2022-07-26 13:23:28.000000 marshy-4.0.0/marshy/marshaller_context.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      199 2021-12-07 03:19:47.000000 marshy-4.0.0/marshy/types.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1009 2021-10-29 15:31:13.000000 marshy-4.0.0/marshy/utils.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy.egg-info/
+-rw-r--r--   0 tofarr     (501) staff       (20)     8717 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     2192 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/SOURCES.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/dependency_links.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/requires.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       34 2023-04-18 21:22:39.000000 marshy-4.0.0/marshy.egg-info/top_level.txt
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/marshy_config_default/
+-rw-r--r--   0 tofarr     (501) staff       (20)     1819 2022-01-24 23:05:39.000000 marshy-4.0.0/marshy_config_default/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 21:22:40.000000 marshy-4.0.0/setup.cfg
+-rw-r--r--   0 tofarr     (501) staff       (20)      753 2021-09-28 02:54:22.000000 marshy-4.0.0/setup.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/test/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-09-26 14:52:20.000000 marshy-4.0.0/test/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:22:40.000000 marshy-4.0.0/test/performance/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-10-09 15:23:45.000000 marshy-4.0.0/test/performance/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      716 2021-10-09 15:20:22.000000 marshy-4.0.0/test/performance/fixtures.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      316 2021-10-09 15:28:35.000000 marshy-4.0.0/test/performance/marshmallow_performance.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      252 2021-10-09 15:28:35.000000 marshy-4.0.0/test/performance/marshy_performance.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4118 2021-12-07 14:44:39.000000 marshy-4.0.0/test/test_custom_marshalling.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      625 2022-07-31 11:39:59.000000 marshy-4.0.0/test/test_customize_exclude_dumped_values.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1704 2022-01-23 15:06:09.000000 marshy-4.0.0/test/test_factory_ordering.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1752 2022-07-26 13:42:12.000000 marshy-4.0.0/test/test_futures.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      975 2022-01-24 23:31:34.000000 marshy-4.0.0/test/test_immutable.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1612 2022-08-11 16:59:14.000000 marshy-4.0.0/test/test_impl_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      703 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_bool.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      710 2021-11-03 13:45:28.000000 marshy-4.0.0/test/test_marshall_datetime.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      765 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_deferred.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1116 2023-04-18 21:21:34.000000 marshy-4.0.0/test/test_marshall_enum.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      474 2021-12-07 14:43:04.000000 marshy-4.0.0/test/test_marshall_freeform.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1053 2022-02-02 23:23:37.000000 marshy-4.0.0/test/test_marshall_iterable.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3799 2022-02-09 16:01:32.000000 marshy-4.0.0/test/test_marshall_obj.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      368 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_optional.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      542 2021-09-28 02:53:11.000000 marshy-4.0.0/test/test_marshall_primitive.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3023 2022-11-30 22:11:46.000000 marshy-4.0.0/test/test_marshall_properties.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      627 2022-02-10 02:49:32.000000 marshy-4.0.0/test/test_marshall_tuple.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1223 2021-11-18 00:01:20.000000 marshy-4.0.0/test/test_marshall_type.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1898 2021-11-18 00:13:22.000000 marshy-4.0.0/test/test_marshall_union.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      355 2021-10-29 15:33:04.000000 marshy-4.0.0/test/test_marshall_uuid.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      795 2021-10-09 15:50:08.000000 marshy-4.0.0/test/test_performance.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      975 2021-12-07 03:33:25.000000 marshy-4.0.0/test/test_utils.py
```

### Comparing `marshy-3.0.0/LICENSE` & `marshy-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/PKG-INFO` & `marshy-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshy
-Version: 3.0.0
+Version: 4.0.0
 Summary: A convention over configuration approach to object marshalling.
 Home-page: https://github.com/tofarr/marshy
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `marshy-3.0.0/README.md` & `marshy-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/__init__.py` & `marshy-4.0.0/marshy/__init__.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/dataclass_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/dataclass_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/enum_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/enum_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/factory_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/factory_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/impl_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/impl_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/list_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/list_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/marshaller_factory_abc.py` & `marshy-4.0.0/marshy/factory/marshaller_factory_abc.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/optional_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/optional_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/tuple_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/tuple_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/factory/union_marshaller_factory.py` & `marshy-4.0.0/marshy/factory/union_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/__init__.py` & `marshy-4.0.0/marshy/marshaller/__init__.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/datetime_marshaller.py` & `marshy-4.0.0/marshy/marshaller/datetime_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/deferred_marshaller.py` & `marshy-4.0.0/marshy/marshaller/deferred_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/enum_marshaller.py` & `marshy-4.0.0/marshy/marshaller/enum_marshaller.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     """
     Marshaller for enums
     """
     allow_unknown: bool = False
 
     def load(self, item: Union[str, int, float]) -> T:
         try:
-            loaded = self.marshalled_type(item)
+            loaded = self.marshalled_type[item]
             return loaded
-        except ValueError as e:
+        except KeyError as e:
             if self.allow_unknown:
                 pseudo_member = generate_pseudo_member(self.marshalled_type, item)
                 return pseudo_member
             raise MarshallError(e)
 
     def dump(self, item: T) -> Union[str, int, float]:
-        dumped = item.value
+        dumped = item.name
         return dumped
 
 
 def generate_pseudo_member(enum: T, value: Union[str, int, float]):
     pseudo_member = object.__new__(enum)
     pseudo_member._name_ = f'{ERROR_PREFIX}{str(value).upper()}'
     pseudo_member._value_ = value
```

### Comparing `marshy-3.0.0/marshy/marshaller/iterable_marshaller.py` & `marshy-4.0.0/marshy/marshaller/iterable_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/json_str_marshaller.py` & `marshy-4.0.0/marshy/marshaller/json_str_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/obj_marshaller.py` & `marshy-4.0.0/marshy/marshaller/obj_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/optional_marshaller.py` & `marshy-4.0.0/marshy/marshaller/optional_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/property_marshaller.py` & `marshy-4.0.0/marshy/marshaller/property_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/tuple_marshaller.py` & `marshy-4.0.0/marshy/marshaller/tuple_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/type_marshaller.py` & `marshy-4.0.0/marshy/marshaller/type_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller/union_marshaller.py` & `marshy-4.0.0/marshy/marshaller/union_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/marshaller_context.py` & `marshy-4.0.0/marshy/marshaller_context.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy/utils.py` & `marshy-4.0.0/marshy/utils.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy.egg-info/PKG-INFO` & `marshy-4.0.0/marshy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshy
-Version: 3.0.0
+Version: 4.0.0
 Summary: A convention over configuration approach to object marshalling.
 Home-page: https://github.com/tofarr/marshy
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `marshy-3.0.0/marshy.egg-info/SOURCES.txt` & `marshy-4.0.0/marshy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/marshy_config_default/__init__.py` & `marshy-4.0.0/marshy_config_default/__init__.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/setup.py` & `marshy-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/performance/fixtures.py` & `marshy-4.0.0/test/performance/fixtures.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_custom_marshalling.py` & `marshy-4.0.0/test/test_custom_marshalling.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_customize_exclude_dumped_values.py` & `marshy-4.0.0/test/test_customize_exclude_dumped_values.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_factory_ordering.py` & `marshy-4.0.0/test/test_factory_ordering.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_futures.py` & `marshy-4.0.0/test/test_futures.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_immutable.py` & `marshy-4.0.0/test/test_immutable.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_impl_marshaller.py` & `marshy-4.0.0/test/test_impl_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_bool.py` & `marshy-4.0.0/test/test_marshall_bool.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_datetime.py` & `marshy-4.0.0/test/test_marshall_datetime.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_deferred.py` & `marshy-4.0.0/test/test_marshall_deferred.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_enum.py` & `marshy-4.0.0/test/test_marshall_enum.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     BIKE = 'bike'
 
 
 class TestMarshallEnum(TestCase):
 
     def test_marshall(self):
         dumped = dump(VehicleTypes.CAR)
-        assert VehicleTypes.CAR.value == dumped
+        assert VehicleTypes.CAR.name == dumped
         loaded = load(VehicleTypes, dumped)
         assert VehicleTypes.CAR == loaded
 
     def test_unknown_value_not_permitted(self):
         with self.assertRaises(MarshallError):
             load(VehicleTypes, 'spaceship')
 
     def test_unknown_value_permitted(self):
         # Allow unknown values to be placed in the enum
         marshaller = EnumMarshallerFactory(allow_unknown=True).create(get_default_context(), VehicleTypes)
         loaded = marshaller.load('spaceship')
         assert loaded.value == 'spaceship'
         assert loaded.__class__ == VehicleTypes
         dumped = marshaller.dump(loaded)
-        assert dumped == 'spaceship'
+        assert dumped == 'INVALID_VALUE__SPACESHIP'
```

### Comparing `marshy-3.0.0/test/test_marshall_iterable.py` & `marshy-4.0.0/test/test_marshall_iterable.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_obj.py` & `marshy-4.0.0/test/test_marshall_obj.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_primitive.py` & `marshy-4.0.0/test/test_marshall_primitive.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_properties.py` & `marshy-4.0.0/test/test_marshall_properties.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_tuple.py` & `marshy-4.0.0/test/test_marshall_tuple.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_type.py` & `marshy-4.0.0/test/test_marshall_type.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_marshall_union.py` & `marshy-4.0.0/test/test_marshall_union.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_performance.py` & `marshy-4.0.0/test/test_performance.py`

 * *Files identical despite different names*

### Comparing `marshy-3.0.0/test/test_utils.py` & `marshy-4.0.0/test/test_utils.py`

 * *Files identical despite different names*

