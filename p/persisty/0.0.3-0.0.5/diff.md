# Comparing `tmp/persisty-0.0.3.tar.gz` & `tmp/persisty-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/persisty-0.0.3.tar", last modified: Thu Apr  6 02:44:43 2023, max compression
+gzip compressed data, was "dist/persisty-0.0.5.tar", last modified: Tue Apr 18 03:27:27 2023, max compression
```

## Comparing `persisty-0.0.3.tar` & `persisty-0.0.5.tar`

### file list

```diff
@@ -1,192 +1,196 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/
--rw-r--r--   0 tofarr     (501) staff       (20)     3951 2023-04-06 02:44:43.000000 persisty-0.0.3/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     3529 2023-03-29 23:11:13.000000 persisty-0.0.3/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:42.000000 persisty-0.0.3/marshy_config_persisty/
--rw-r--r--   0 tofarr     (501) staff       (20)     5418 2023-04-06 02:36:13.000000 persisty-0.0.3/marshy_config_persisty/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1670 2023-01-17 18:43:12.000000 persisty-0.0.3/marshy_config_persisty/sqlalchemy_config.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 11:54:34.000000 persisty-0.0.3/persisty/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-06 02:36:13.000000 persisty-0.0.3/persisty/__version__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty/attr/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2170 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/attr/attr.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2033 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/attr/attr_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2499 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/attr/attr_filter_op.py
--rw-r--r--   0 tofarr     (501) staff       (20)      868 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/attr/attr_type.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/attr/generator/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/generator/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      168 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/generator/attr_value_generator_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      375 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/generator/default_value_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1203 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/generator/defaults.py
--rw-r--r--   0 tofarr     (501) staff       (20)      749 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/attr/generator/int_sequence_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)      798 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/generator/str_sequence_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)      382 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/generator/timestamp_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)      328 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/attr/generator/uuid_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1304 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/batch_edit.py
--rw-r--r--   0 tofarr     (501) staff       (20)      983 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/batch_edit_result.py
--rw-r--r--   0 tofarr     (501) staff       (20)       41 2023-01-12 05:23:25.000000 persisty-0.0.3/persisty/errors.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      625 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/factory/default_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1725 2023-03-30 15:13:54.000000 persisty-0.0.3/persisty/factory/owned_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3275 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/factory/store_factory_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/finder/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 19:31:01.000000 persisty-0.0.3/persisty/finder/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1776 2023-03-30 17:29:52.000000 persisty-0.0.3/persisty/finder/module_store_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1134 2023-03-30 21:59:07.000000 persisty-0.0.3/persisty/finder/store_finder_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/impl/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/impl/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-03-30 21:09:21.000000 persisty-0.0.3/persisty/impl/default_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/impl/dynamodb/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/impl/dynamodb/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2160 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/impl/dynamodb/dynamodb_index.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/dynamodb/dynamodb_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6350 2023-03-30 20:08:04.000000 persisty-0.0.3/persisty/impl/dynamodb/dynamodb_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)    17382 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/dynamodb/dynamodb_table_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/impl/mem/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/impl/mem/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3951 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/impl/mem/mem_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-30 15:48:00.000000 persisty-0.0.3/persisty/impl/mem/mem_store_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/impl/sqlalchemy/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/impl/sqlalchemy/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2162 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      607 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/include_all_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      845 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1015 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      677 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1362 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3648 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1353 2023-03-30 17:49:46.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1394 2023-03-30 20:09:21.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1088 2023-03-30 20:09:02.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      894 2023-03-30 02:34:01.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2117 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)    18083 2023-03-30 20:51:33.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_table_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1189 2023-03-30 15:48:06.000000 persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      142 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/index.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/io/
--rw-r--r--   0 tofarr     (501) staff       (20)     3200 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/io/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1290 2023-03-30 21:14:52.000000 persisty-0.0.3/persisty/io/seed.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/key_config/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/key_config/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2041 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/key_config/attr_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1265 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/key_config/composite_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      777 2023-03-24 21:18:32.000000 persisty-0.0.3/persisty/key_config/key_config_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/link/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 12:25:11.000000 persisty-0.0.3/persisty/link/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2958 2023-03-30 22:16:51.000000 persisty-0.0.3/persisty/link/belongs_to.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/link/has_count.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2250 2023-03-30 22:18:04.000000 persisty-0.0.3/persisty/link/has_many.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1125 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/link/link_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1681 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/link/linked_store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      114 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/link/on_delete.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/migration/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 00:58:05.000000 persisty-0.0.3/persisty/migration/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1229 2023-03-30 21:59:55.000000 persisty-0.0.3/persisty/migration/alembic.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/migration/serverless/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 01:07:24.000000 persisty-0.0.3/persisty/migration/serverless/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3762 2023-04-06 01:19:27.000000 persisty-0.0.3/persisty/migration/serverless/dynamodb_yml_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      569 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/result_set.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/search_filter/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/search_filter/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2703 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_filter/and_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/search_filter/exclude_all.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_filter/filter_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      624 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/search_filter/include_all.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1032 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_filter/not_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2323 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_filter/or_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1908 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_filter/query_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1631 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_filter/search_filter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2003 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/search_filter/search_filter_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/search_order/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/search_order/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      919 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_order/search_order.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1097 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/search_order/search_order_attr.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1178 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/search_order/search_order_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/servey/
--rw-r--r--   0 tofarr     (501) staff       (20)      540 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/servey/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)    10128 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/servey/actions.py
--rw-r--r--   0 tofarr     (501) staff       (20)       87 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/servey/generated.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/store/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1483 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/filtered_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     8672 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/filtered_store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      379 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/logging_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6401 2023-03-30 15:14:07.000000 persisty-0.0.3/persisty/store/owned_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5020 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/restrict_access_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2609 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/schema_validating_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     8608 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5537 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store/ttl_cache_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3218 2023-03-30 20:08:05.000000 persisty-0.0.3/persisty/store/unique_index_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2371 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/store/wrapper_store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1074 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/store_access.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6990 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/store_meta.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6107 2023-03-19 15:06:43.000000 persisty-0.0.3/persisty/stored.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/trigger/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-07 17:19:03.000000 persisty-0.0.3/persisty/trigger/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/after_create_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/after_delete_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/after_update_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2334 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/asyncio_trigger_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)      985 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/celery_store_trigger_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2553 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/celery_trigger_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3164 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/dynamodb_post_process_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1504 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/serverless_trigger_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3287 2023-03-30 15:47:07.000000 persisty-0.0.3/persisty/trigger/store_triggers.py
--rw-r--r--   0 tofarr     (501) staff       (20)      638 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/trigger/wrapper.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/persisty/util/
--rw-r--r--   0 tofarr     (501) staff       (20)     2023 2023-01-11 03:09:38.000000 persisty-0.0.3/persisty/util/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1094 2023-01-05 17:22:52.000000 persisty-0.0.3/persisty/util/encrypt_at_rest.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1866 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/util/logify.py
--rw-r--r--   0 tofarr     (501) staff       (20)      754 2023-01-17 18:43:12.000000 persisty-0.0.3/persisty/util/undefined.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)     3951 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     5680 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       48 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-06 02:44:42.000000 persisty-0.0.3/persisty.egg-info/top_level.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-06 02:44:43.000000 persisty-0.0.3/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      946 2023-04-05 22:25:24.000000 persisty-0.0.3/setup.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:42.000000 persisty-0.0.3/tests/
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/attr/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/attr/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/attr/generator/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/attr/generator/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      636 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/attr/generator/test_defaults.py
--rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/attr/test_attr.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2492 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/attr/test_attr_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1321 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/attr/test_attr_filter_op.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      664 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/factory/test_default_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2252 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/factory/test_owned_store_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/finder/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/finder/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      361 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/finder/fixtures.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/finder/test_module_store_finder.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/fixtures/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-19 13:13:59.000000 persisty-0.0.3/tests/fixtures/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1406 2023-01-17 18:43:12.000000 persisty-0.0.3/tests/fixtures/number_name.py
--rw-r--r--   0 tofarr     (501) staff       (20)    21310 2023-01-17 18:43:12.000000 persisty-0.0.3/tests/fixtures/storage_tst_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)    14030 2023-01-17 18:43:12.000000 persisty-0.0.3/tests/fixtures/super_bowl_results.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/impl/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:20:56.000000 persisty-0.0.3/tests/impl/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/impl/dynamodb/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 16:41:50.000000 persisty-0.0.3/tests/impl/dynamodb/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6057 2023-01-17 18:43:12.000000 persisty-0.0.3/tests/impl/dynamodb/test_dynamodb_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/impl/mem/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:33:37.000000 persisty-0.0.3/tests/impl/mem/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3478 2023-01-17 18:43:12.000000 persisty-0.0.3/tests/impl/mem/test_mem_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/impl/sqlalchemy/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:22:30.000000 persisty-0.0.3/tests/impl/sqlalchemy/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4970 2023-01-17 18:43:12.000000 persisty-0.0.3/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-06 02:44:43.000000 persisty-0.0.3/tests/util/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:34:03.000000 persisty-0.0.3/tests/util/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      595 2022-07-21 04:14:28.000000 persisty-0.0.3/tests/util/test_encrypt_at_rest.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3262 2023-03-19 15:06:43.000000 persisty-0.0.3/tests/util/test_logify.py
--rw-r--r--   0 tofarr     (501) staff       (20)      377 2022-07-20 14:03:55.000000 persisty-0.0.3/tests/util/test_undefined.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1368 2022-07-21 04:14:28.000000 persisty-0.0.3/tests/util/test_util.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/
+-rw-r--r--   0 tofarr     (501) staff       (20)     4051 2023-04-18 03:27:27.000000 persisty-0.0.5/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     3629 2023-04-16 16:31:32.000000 persisty-0.0.5/README.md
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/marshy_config_persisty/
+-rw-r--r--   0 tofarr     (501) staff       (20)     5933 2023-04-18 00:07:16.000000 persisty-0.0.5/marshy_config_persisty/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1670 2023-01-17 18:43:12.000000 persisty-0.0.5/marshy_config_persisty/sqlalchemy_config.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 11:54:34.000000 persisty-0.0.5/persisty/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-17 23:02:01.000000 persisty-0.0.5/persisty/__version__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/attr/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2170 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/attr/attr.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2033 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/attr/attr_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2499 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/attr/attr_filter_op.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      868 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/attr/attr_type.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/attr/generator/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/generator/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      168 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/generator/attr_value_generator_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      375 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/generator/default_value_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1203 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/generator/defaults.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      749 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/attr/generator/int_sequence_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      798 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/generator/str_sequence_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      382 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/generator/timestamp_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      328 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/attr/generator/uuid_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1304 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/batch_edit.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      983 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/batch_edit_result.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       41 2023-01-12 05:23:25.000000 persisty-0.0.5/persisty/errors.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      625 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/factory/default_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1725 2023-03-30 15:13:54.000000 persisty-0.0.5/persisty/factory/owned_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3275 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/factory/store_factory_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/finder/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 19:31:01.000000 persisty-0.0.5/persisty/finder/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1776 2023-03-30 17:29:52.000000 persisty-0.0.5/persisty/finder/module_store_finder.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1134 2023-03-30 21:59:07.000000 persisty-0.0.5/persisty/finder/store_finder_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/impl/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/impl/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-03-30 21:09:21.000000 persisty-0.0.5/persisty/impl/default_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/impl/dynamodb/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/impl/dynamodb/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/dynamodb/dynamodb_key_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6672 2023-04-18 00:07:16.000000 persisty-0.0.5/persisty/impl/dynamodb/dynamodb_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    17588 2023-04-18 00:07:16.000000 persisty-0.0.5/persisty/impl/dynamodb/dynamodb_table_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2423 2023-04-18 00:06:51.000000 persisty-0.0.5/persisty/impl/dynamodb/partition_sort_index.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty/impl/mem/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/impl/mem/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3951 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/impl/mem/mem_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-30 15:48:00.000000 persisty-0.0.5/persisty/impl/mem/mem_store_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/impl/sqlalchemy/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/impl/sqlalchemy/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2162 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      607 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/include_all_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      845 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1015 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      677 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1362 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3648 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1353 2023-03-30 17:49:46.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1394 2023-03-30 20:09:21.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_context.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1088 2023-03-30 20:09:02.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      894 2023-03-30 02:34:01.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2529 2023-04-17 22:52:15.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    18019 2023-04-17 21:07:20.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_table_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1189 2023-03-30 15:48:06.000000 persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/index/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-17 20:43:57.000000 persisty-0.0.5/persisty/index/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      259 2023-04-17 20:40:30.000000 persisty-0.0.5/persisty/index/attr_index.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       52 2023-04-17 20:39:42.000000 persisty-0.0.5/persisty/index/index_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      271 2023-04-17 20:41:37.000000 persisty-0.0.5/persisty/index/unique_index.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/io/
+-rw-r--r--   0 tofarr     (501) staff       (20)     3200 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/io/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1290 2023-03-30 21:14:52.000000 persisty-0.0.5/persisty/io/seed.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/key_config/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/key_config/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2041 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/key_config/attr_key_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1265 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/key_config/composite_key_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      777 2023-03-24 21:18:32.000000 persisty-0.0.5/persisty/key_config/key_config_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/link/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 12:25:11.000000 persisty-0.0.5/persisty/link/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2958 2023-03-30 22:16:51.000000 persisty-0.0.5/persisty/link/belongs_to.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/link/has_count.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2250 2023-03-30 22:18:04.000000 persisty-0.0.5/persisty/link/has_many.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1125 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/link/link_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1681 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/link/linked_store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      114 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/link/on_delete.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/migration/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 00:58:05.000000 persisty-0.0.5/persisty/migration/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1229 2023-03-30 21:59:55.000000 persisty-0.0.5/persisty/migration/alembic.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/migration/serverless/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 01:07:24.000000 persisty-0.0.5/persisty/migration/serverless/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4126 2023-04-06 13:26:22.000000 persisty-0.0.5/persisty/migration/serverless/dynamodb_yml_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      569 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/result_set.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/search_filter/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/search_filter/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2703 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/search_filter/and_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/search_filter/exclude_all.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/search_filter/filter_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      624 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/search_filter/include_all.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1032 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/search_filter/not_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2323 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/search_filter/or_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1908 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/search_filter/query_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1631 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/search_filter/search_filter_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2003 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/search_filter/search_filter_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/search_order/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/search_order/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      919 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/search_order/search_order.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1112 2023-04-17 14:04:58.000000 persisty-0.0.5/persisty/search_order/search_order_attr.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1178 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/search_order/search_order_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/servey/
+-rw-r--r--   0 tofarr     (501) staff       (20)      540 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/servey/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    10722 2023-04-17 19:54:17.000000 persisty-0.0.5/persisty/servey/actions.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       87 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/servey/generated.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/store/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1483 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/filtered_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     8672 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/filtered_store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      379 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/logging_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6401 2023-03-30 15:14:07.000000 persisty-0.0.5/persisty/store/owned_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5020 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/restrict_access_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2609 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/schema_validating_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     8608 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5537 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store/ttl_cache_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3261 2023-04-17 21:34:03.000000 persisty-0.0.5/persisty/store/unique_index_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2371 2023-03-19 15:06:43.000000 persisty-0.0.5/persisty/store/wrapper_store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1074 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/store_access.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6996 2023-04-17 21:07:20.000000 persisty-0.0.5/persisty/store_meta.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6186 2023-04-18 03:14:40.000000 persisty-0.0.5/persisty/stored.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/trigger/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-07 17:19:03.000000 persisty-0.0.5/persisty/trigger/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/after_create_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/after_delete_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/after_update_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2334 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/asyncio_trigger_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      985 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/celery_store_trigger_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2553 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/celery_trigger_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3164 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/dynamodb_post_process_event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1504 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/serverless_trigger_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3287 2023-03-30 15:47:07.000000 persisty-0.0.5/persisty/trigger/store_triggers.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      638 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/trigger/wrapper.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/persisty/util/
+-rw-r--r--   0 tofarr     (501) staff       (20)     2023 2023-01-11 03:09:38.000000 persisty-0.0.5/persisty/util/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1094 2023-01-05 17:22:52.000000 persisty-0.0.5/persisty/util/encrypt_at_rest.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1866 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/util/logify.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      754 2023-01-17 18:43:12.000000 persisty-0.0.5/persisty/util/undefined.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty.egg-info/
+-rw-r--r--   0 tofarr     (501) staff       (20)     4051 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty.egg-info/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     5783 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty.egg-info/SOURCES.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty.egg-info/dependency_links.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       48 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty.egg-info/requires.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 03:27:26.000000 persisty-0.0.5/persisty.egg-info/top_level.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 03:27:27.000000 persisty-0.0.5/setup.cfg
+-rw-r--r--   0 tofarr     (501) staff       (20)      946 2023-04-13 14:34:44.000000 persisty-0.0.5/setup.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:26.000000 persisty-0.0.5/tests/
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/attr/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/attr/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/attr/generator/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/attr/generator/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      636 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/attr/generator/test_defaults.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/attr/test_attr.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2492 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/attr/test_attr_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1321 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/attr/test_attr_filter_op.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      664 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/factory/test_default_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2439 2023-04-17 21:46:14.000000 persisty-0.0.5/tests/factory/test_owned_store_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/finder/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/finder/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      361 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/finder/fixtures.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/finder/test_module_store_finder.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/fixtures/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-19 13:13:59.000000 persisty-0.0.5/tests/fixtures/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1464 2023-04-18 03:18:56.000000 persisty-0.0.5/tests/fixtures/number_name.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    21310 2023-01-17 18:43:12.000000 persisty-0.0.5/tests/fixtures/storage_tst_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    14045 2023-04-17 22:14:54.000000 persisty-0.0.5/tests/fixtures/super_bowl_results.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/impl/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:20:56.000000 persisty-0.0.5/tests/impl/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/impl/dynamodb/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 16:41:50.000000 persisty-0.0.5/tests/impl/dynamodb/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6078 2023-04-18 00:07:16.000000 persisty-0.0.5/tests/impl/dynamodb/test_dynamodb_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/impl/mem/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:33:37.000000 persisty-0.0.5/tests/impl/mem/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3478 2023-01-17 18:43:12.000000 persisty-0.0.5/tests/impl/mem/test_mem_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/impl/sqlalchemy/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:22:30.000000 persisty-0.0.5/tests/impl/sqlalchemy/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4970 2023-01-17 18:43:12.000000 persisty-0.0.5/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 03:27:27.000000 persisty-0.0.5/tests/util/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:34:03.000000 persisty-0.0.5/tests/util/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      595 2022-07-21 04:14:28.000000 persisty-0.0.5/tests/util/test_encrypt_at_rest.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3262 2023-03-19 15:06:43.000000 persisty-0.0.5/tests/util/test_logify.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      377 2022-07-20 14:03:55.000000 persisty-0.0.5/tests/util/test_undefined.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1368 2022-07-21 04:14:28.000000 persisty-0.0.5/tests/util/test_util.py
```

### Comparing `persisty-0.0.3/PKG-INFO` & `persisty-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: persisty
-Version: 0.0.3
+Version: 0.0.5
 Summary: A better persistence layer for python
 Home-page: https://github.com/tofarr/lambsync
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
+* Appsync is slow. Maybe look at batch processors from API gateway?
+* Check out ordering on search
+
 # Persisty - a better persistence Layer for Python
 
 The objective of this project is to provide a resource oriented approach
 accommodating both security and caching rich enough to handle most use
 cases while still being independant of the underlying persistence 
 mechanism.
```

### Comparing `persisty-0.0.3/README.md` & `persisty-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+* Appsync is slow. Maybe look at batch processors from API gateway?
+* Check out ordering on search
+
 # Persisty - a better persistence Layer for Python
 
 The objective of this project is to provide a resource oriented approach
 accommodating both security and caching rich enough to handle most use
 cases while still being independant of the underlying persistence 
 mechanism.
```

### Comparing `persisty-0.0.3/marshy_config_persisty/__init__.py` & `persisty-0.0.5/marshy_config_persisty/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from persisty.attr.attr_filter import AttrFilter
 from persisty.attr.generator.attr_value_generator_abc import AttrValueGeneratorABC
 from persisty.attr.generator.default_value_generator import DefaultValueGenerator
 from persisty.attr.generator.timestamp_generator import TimestampGenerator
 from persisty.attr.generator.uuid_generator import UuidGenerator
 from persisty.finder.module_store_finder import ModuleStoreFinder
 from persisty.finder.store_finder_abc import StoreFactoryFinderABC
+from persisty.index.attr_index import AttrIndex
+from persisty.index.index_abc import IndexABC
+from persisty.index.unique_index import UniqueIndex
 from persisty.key_config.attr_key_config import AttrKeyConfig
 from persisty.key_config.composite_key_config import CompositeKeyConfig
 from persisty.key_config.key_config_abc import KeyConfigABC
 from persisty.link.belongs_to import BelongsTo
 from persisty.link.has_count import HasCount
 from persisty.link.has_many import HasMany
 from persisty.link.link_abc import LinkABC
@@ -43,14 +46,15 @@
     AttrConfig.filter_dumped_values = (UNDEFINED,)
     PropertyConfig.filter_dumped_values = (UNDEFINED,)
 
     configure_search_filters(context)
     configure_key_configs(context)
     configure_attr_value_generator(context)
     configure_cache_control(context)
+    configure_indexes(context)
     configure_links(context)
     configure_finders(context)
 
     configure_sqlalchemy(context)
     configure_celery(context)
     configure_serverless(context)
 
@@ -80,28 +84,38 @@
 
 def configure_cache_control(context: MarshallerContext):
     register_impl(CacheControlABC, SecureHashCacheControl, context)
     register_impl(CacheControlABC, TimestampCacheControl, context)
     register_impl(CacheControlABC, TtlCacheControl, context)
 
 
+def configure_indexes(context: MarshallerContext):
+    register_impl(IndexABC, AttrIndex, context)
+    register_impl(IndexABC, UniqueIndex, context)
+    try:
+        from persisty.impl.dynamodb.partition_sort_index import PartitionSortIndex
+        register_impl(IndexABC, PartitionSortIndex, context)
+    except ImportError as e:
+        raise_non_ignored(e)
+
+
 def configure_links(context: MarshallerContext):
     register_impl(LinkABC, BelongsTo, context)
     register_impl(LinkABC, HasMany, context)
     register_impl(LinkABC, HasCount, context)
 
 
 def configure_sqlalchemy(context: MarshallerContext):
     try:
         # Local import in case sqlalchemy is not included (Optional extra)
         from marshy_config_persisty import sqlalchemy_config
 
         sqlalchemy_config.configure_converters(context)
         sqlalchemy_config.configure_sqlalchemy_context(context)
-    except ModuleNotFoundError as e:
+    except ImportError as e:
         msg = str(e)
         if msg.startswith("No module named '"):
             module_name = msg[len("No module named '"):-1]
             if module_name == 'sqlalchemy':
                 return
         raise_non_ignored(e)
 
@@ -114,19 +128,19 @@
     try:
         from servey.servey_celery.celery_config.celery_config_abc import CeleryConfigABC
         from persisty.trigger.celery_store_trigger_config import (
             CeleryStoreTriggerConfig,
         )
 
         register_impl(CeleryConfigABC, CeleryStoreTriggerConfig, context)
-    except ModuleNotFoundError as e:
+    except ImportError as e:
         raise_non_ignored(e)
 
 
 def configure_serverless(context: MarshallerContext):
     try:
         from servey.servey_aws.serverless.yml_config.yml_config_abc import YmlConfigABC
         from persisty.migration.serverless.dynamodb_yml_config import DynamodbYmlConfig
 
         register_impl(YmlConfigABC, DynamodbYmlConfig, context)
-    except ModuleNotFoundError as e:
+    except ImportError as e:
         raise_non_ignored(e)
```

### Comparing `persisty-0.0.3/marshy_config_persisty/sqlalchemy_config.py` & `persisty-0.0.5/marshy_config_persisty/sqlalchemy_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/attr/attr.py` & `persisty-0.0.5/persisty/attr/attr.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/attr/attr_filter.py` & `persisty-0.0.5/persisty/attr/attr_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/attr/attr_filter_op.py` & `persisty-0.0.5/persisty/attr/attr_filter_op.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/attr/attr_type.py` & `persisty-0.0.5/persisty/attr/attr_type.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/attr/generator/defaults.py` & `persisty-0.0.5/persisty/attr/generator/defaults.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/attr/generator/int_sequence_generator.py` & `persisty-0.0.5/persisty/attr/generator/int_sequence_generator.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/attr/generator/str_sequence_generator.py` & `persisty-0.0.5/persisty/attr/generator/str_sequence_generator.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/batch_edit.py` & `persisty-0.0.5/persisty/batch_edit.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/batch_edit_result.py` & `persisty-0.0.5/persisty/batch_edit_result.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/factory/default_store_factory.py` & `persisty-0.0.5/persisty/factory/default_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/factory/owned_store_factory.py` & `persisty-0.0.5/persisty/factory/owned_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/factory/store_factory_abc.py` & `persisty-0.0.5/persisty/factory/store_factory_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/finder/module_store_finder.py` & `persisty-0.0.5/persisty/finder/module_store_finder.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/finder/store_finder_abc.py` & `persisty-0.0.5/persisty/finder/store_finder_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/default_store.py` & `persisty-0.0.5/persisty/impl/default_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/dynamodb/dynamodb_index.py` & `persisty-0.0.5/persisty/impl/dynamodb/partition_sort_index.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 from typing import List, Dict, Iterable, Optional
 
 from boto3.dynamodb.conditions import Key, And as DynAnd
 from marshy.types import ExternalItemType
 
 from persisty.attr.attr import Attr
 from persisty.impl.dynamodb.dynamodb_key_config import DynamodbKeyConfig
+from persisty.index.index_abc import IndexABC
 from persisty.key_config.attr_key_config import AttrKeyConfig
 
 
 @dataclass(frozen=True)
-class DynamodbIndex:
+class PartitionSortIndex(IndexABC):
+    """
+    Index which functions similarly to an AttrIndex, but has an optional sort key (Useful for dynamodb)
+    Sql tables treat this as an attr index
+    """
     pk: str
     sk: Optional[str] = None
+    descending: bool = False
 
     def to_schema(self):
         schema = [dict(AttributeName=self.pk, KeyType="HASH")]
         if self.sk:
             schema.append(dict(AttributeName=self.sk, KeyType="RANGE"))
         return schema
 
@@ -48,15 +54,15 @@
             return pk_attr
         sk_attr = next(a for a in configs if a.attr_name == self.sk)
         return DynamodbKeyConfig(pk_attr, sk_attr)
 
 
 def from_schema(schema: List[Dict]):
     assert len(schema) == 1 or len(schema) == 2
-    index = DynamodbIndex(
+    index = PartitionSortIndex(
         pk=next(a["AttributeName"] for a in schema if a["KeyType"] == "HASH"),
         sk=next((a["AttributeName"] for a in schema if a["KeyType"] == "RANGE"), None),
     )
     return index
 
 
-ID_INDEX = DynamodbIndex("id")
+ID_INDEX = PartitionSortIndex("id")
```

### Comparing `persisty-0.0.3/persisty/impl/dynamodb/dynamodb_key_config.py` & `persisty-0.0.5/persisty/impl/dynamodb/dynamodb_key_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/dynamodb/dynamodb_store_factory.py` & `persisty-0.0.5/persisty/impl/dynamodb/dynamodb_store_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import boto3
 from schemey import schema_from_type
 
 from persisty.attr.attr import Attr
 from persisty.attr.attr_filter_op import TYPE_FILTER_OPS
 from persisty.attr.attr_type import attr_type, AttrType
 from persisty.errors import PersistyError
-from persisty.impl.dynamodb.dynamodb_index import DynamodbIndex, from_schema
+from persisty.impl.dynamodb.partition_sort_index import PartitionSortIndex, from_schema
 from persisty.impl.dynamodb.dynamodb_table_store import DynamodbTableStore
+from persisty.index.attr_index import AttrIndex
 from persisty.key_config.attr_key_config import AttrKeyConfig
 from persisty.key_config.composite_key_config import CompositeKeyConfig
 from persisty.key_config.key_config_abc import KeyConfigABC
 from persisty.store.restrict_access_store import restrict_access_store
 from persisty.store.schema_validating_store import SchemaValidatingStore
 from persisty.store.store_abc import StoreABC
 from persisty.store.unique_index_store import unique_index_store
@@ -23,16 +24,16 @@
 
 @dataclass
 class DynamodbStoreFactory:
     meta: Optional[StoreMeta] = None
     aws_profile_name: Optional[str] = None
     region_name: Optional[str] = None
     table_name: Optional[str] = None
-    index: Optional[DynamodbIndex] = None
-    global_secondary_indexes: Optional[Dict[str, DynamodbIndex]] = None
+    index: Optional[PartitionSortIndex] = None
+    global_secondary_indexes: Optional[Dict[str, PartitionSortIndex]] = None
 
     def get_meta(self) -> StoreMeta:
         return self.meta
 
     def create(self) -> Optional[StoreABC]:
         store = DynamodbTableStore(
             meta=self.meta,
@@ -50,21 +51,25 @@
     def derive_from_meta(self):
         meta = self.meta
         if self.table_name is None:
             self.table_name = meta.name
         if self.index is None:
             key_config = meta.key_config
             key_config_attrs = list(_get_attrs_from_key(key_config))
-            self.index = DynamodbIndex(*key_config_attrs)
+            self.index = PartitionSortIndex(*key_config_attrs)
         if self.global_secondary_indexes is None:
-            self.global_secondary_indexes = {
-                f"gix__{'__'.join(index.attr_names)}": DynamodbIndex(*index.attr_names)
-                for index in meta.indexes
-            }
-            # Dynamodb doesn't support unique indexes on gsis, so if these are specified we'll have to check in edit
+            self.global_secondary_indexes = {}
+            for index in meta.indexes:
+                if isinstance(index, AttrIndex):
+                    self.global_secondary_indexes[f"gix__{index.attr_name}"] = PartitionSortIndex(index.attr_name)
+                elif isinstance(index, PartitionSortIndex):
+                    if index.sk:
+                        self.global_secondary_indexes[f"gix__{index.pk}__{index.sk}"] = index
+                    else:
+                        self.global_secondary_indexes[f"gix__{index.pk}"] = index
 
     def get_session(self):
         kwargs = filter_none(
             dict(profile_name=self.aws_profile_name, region_name=self.region_name)
         )
         session = boto3.Session(**kwargs)
         return session
@@ -117,27 +122,27 @@
                 "IndexName": k,
                 "KeySchema": i.to_schema(),
                 "Projection": {"ProjectionType": "ALL"},
             }
             for k, i in (self.global_secondary_indexes or {}).items()
         ]
 
-    def _attrs(self, index: DynamodbIndex, attrs: Dict):
+    def _attrs(self, index: PartitionSortIndex, attrs: Dict):
         attrs[index.pk] = self._attr(index.pk)
         if index.sk:
             attrs[index.sk] = self._attr(index.sk)
 
     def _attr(self, name: str):
         attr = next(a for a in self.meta.attrs if a.name == name)
         return dict(
             AttributeName=name, AttributeType=_FIELD_TYPE_2_DYNAMODB[attr.attr_type]
         )
 
 
-def _remove_index(indexed_attrs: Set[str], index: DynamodbIndex):
+def _remove_index(indexed_attrs: Set[str], index: PartitionSortIndex):
     indexed_attrs.remove(index.pk)
     if index.sk:
         indexed_attrs.remove(index.sk)
 
 
 _DYNAMODB_2_PYTHON = {
     "B": bytearray,
```

### Comparing `persisty-0.0.3/persisty/impl/dynamodb/dynamodb_table_store.py` & `persisty-0.0.5/persisty/impl/dynamodb/dynamodb_table_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from boto3.dynamodb.conditions import Not as DynNot, ConditionBase, Key
 from botocore.exceptions import ClientError
 from marshy.types import ExternalItemType
 
 from persisty.attr.attr import Attr
 from persisty.attr.generator.attr_value_generator_abc import AttrValueGeneratorABC
 from persisty.errors import PersistyError
-from persisty.impl.dynamodb.dynamodb_index import DynamodbIndex
+from persisty.impl.dynamodb.partition_sort_index import PartitionSortIndex
 from persisty.search_filter.and_filter import And
 from persisty.search_filter.exclude_all import EXCLUDE_ALL
 from persisty.search_filter.search_filter_abc import SearchFilterABC
 from persisty.attr.attr_filter import AttrFilter, AttrFilterOp
 from persisty.batch_edit import BatchEdit
 from persisty.batch_edit_result import BatchEditResult
 from persisty.result_set import ResultSet
@@ -42,16 +42,16 @@
 
 @dataclass(frozen=True)
 class DynamodbTableStore(StoreABC[T]):
     """Store backed by a dynamodb table. Does not do single table design or anything of that nature."""
 
     meta: StoreMeta
     table_name: str
-    index: DynamodbIndex
-    global_secondary_indexes: Dict[str, DynamodbIndex] = field(default_factory=dict)
+    index: PartitionSortIndex
+    global_secondary_indexes: Dict[str, PartitionSortIndex] = field(default_factory=dict)
     aws_profile_name: Optional[str] = None
     region_name: Optional[str] = None
     decimal_format: str = "%.9f"
 
     def get_meta(self) -> StoreMeta:
         return self.meta
 
@@ -159,29 +159,31 @@
             limit = self.meta.batch_size
         assert limit <= self.meta.batch_size
         search_filter = search_filter.lock_attrs(self.meta.attrs)
         if search_order:
             search_order.validate_for_attrs(self.meta.attrs)
         if search_filter is EXCLUDE_ALL:
             return ResultSet([])
-        index_name, condition, filter_expression, handled = self.to_dynamodb_filter(
+        index_name, condition, filter_expression, handled, descending = self.to_dynamodb_filter(
             search_filter
         )
         query_args = filter_none(
             {
                 "KeyConditionExpression": condition,
                 "IndexName": index_name,
                 "Select": "SPECIFIC_ATTRIBUTES",
                 "ProjectionExpression": ",".join(
                     a.name for a in self.meta.attrs if a.readable
                 ),
                 "FilterExpression": filter_expression,
                 "Limit": limit,
             }
         )
+        if descending:
+            query_args["ScanIndexForward"] = False
         if page_key:
             query_args["ExclusiveStartKey"] = self.meta.key_config.to_key_dict(page_key)
         table = self._dynamodb_table()
         results = []
         while True:
             if condition:
                 response = table.query(**query_args)
@@ -204,15 +206,15 @@
             query_args["ExclusiveStartKey"] = last_evaluated_key
 
     @catch_client_error
     def count(self, search_filter: SearchFilterABC = INCLUDE_ALL) -> int:
         search_filter = search_filter.lock_attrs(self.meta.attrs)
         if search_filter is EXCLUDE_ALL:
             return 0
-        index_name, condition, filter_expression, handled = self.to_dynamodb_filter(
+        index_name, condition, filter_expression, handled, _ = self.to_dynamodb_filter(
             search_filter
         )
         if not handled:
             logger.warning(f"search_filter_not_handled_by_dynamodb:{search_filter}")
             count = sum(1 for _ in self.search_all(search_filter))
             return count
         kwargs = filter_none(
@@ -352,50 +354,52 @@
                 return int_val
             else:
                 return Decimal(self.decimal_format % item)
         else:
             return item
 
     def to_dynamodb_filter(
-        self, search_filter: SearchFilterABC
-    ) -> Tuple[Optional[str], Optional[ConditionBase], Optional[ConditionBase], bool]:
+        self,
+        search_filter: SearchFilterABC,
+    ) -> Tuple[Optional[str], Optional[ConditionBase], Optional[ConditionBase], bool, bool]:
         eq_filters = _get_top_level_eq_filters(search_filter)
         if not eq_filters:
             filter_expression, handled = search_filter.build_filter_expression(
                 self.meta.attrs
             )
-            return None, None, filter_expression, handled
+            return None, None, filter_expression, handled, False
         index_name, index = self.get_index_for_eq_filters(eq_filters)
         filter_expression = None
         handled = False
         if index:
-            index_condition, search_filter, index_handled = _separate_index_filters(
+            index_condition, search_filter, index_handled, reverse = _separate_index_filters(
                 index, eq_filters
             )
             if search_filter:
                 filter_expression, handled = search_filter.build_filter_expression(
                     self.meta.attrs
                 )
             else:
                 handled = True
             return (
                 index_name,
                 index_condition,
                 filter_expression,
                 handled and index_handled,
+                reverse
             )
         if search_filter:
             filter_expression, handled = search_filter.build_filter_expression(
                 self.meta.attrs
             )
-        return None, None, filter_expression, handled
+        return None, None, filter_expression, handled, False
 
     def get_index_for_eq_filters(
         self, eq_filters: List[AttrFilter]
-    ) -> Tuple[Optional[str], Optional[DynamodbIndex]]:
+    ) -> Tuple[Optional[str], Optional[PartitionSortIndex]]:
         attr_names = {f.name for f in eq_filters}
         if self.index.pk in attr_names:
             return None, self.index
         for name, index in self.global_secondary_indexes.items():
             if index.pk in attr_names:
                 return name, index
         return None, None
@@ -443,20 +447,20 @@
 
 
 def _is_eq_filter(search_filter: SearchFilterABC) -> bool:
     return isinstance(search_filter, AttrFilter) and search_filter.op == AttrFilterOp.eq
 
 
 def _separate_index_filters(
-    index: DynamodbIndex, eq_filters: List[AttrFilter]
-) -> Tuple[ConditionBase, SearchFilterABC, bool]:
+    index: PartitionSortIndex, eq_filters: List[AttrFilter]
+) -> Tuple[ConditionBase, SearchFilterABC, bool, bool]:
     index_filters = [f for f in eq_filters if f.name == index.pk]
     value = index_filters[0].value
     if value.__class__ not in (str, int, float, bool):
         value = marshy.dump(value)
     condition = Key(index.pk).eq(value)
     non_index_filters = tuple(f for f in eq_filters if f.name != index.pk)
     non_index_filter = None
     if non_index_filters:
         non_index_filter = And(non_index_filters)
     handled = len(index_filters) == 1
-    return condition, non_index_filter, handled
+    return condition, non_index_filter, handled, index.descending
```

### Comparing `persisty-0.0.3/persisty/impl/mem/mem_store.py` & `persisty-0.0.5/persisty/impl/mem/mem_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/mem/mem_store_factory.py` & `persisty-0.0.5/persisty/impl/mem/mem_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/include_all_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/include_all_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_context.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_context.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from persisty.impl.sqlalchemy.sqlalchemy_column_converter import (
     SqlalchemyColumnConverter,
 )
 from persisty.impl.sqlalchemy.sqlalchemy_constraint_converter import (
     SqlalchemyConstraintConverter,
 )
+from persisty.index.attr_index import AttrIndex
+from persisty.index.unique_index import UniqueIndex
 from persisty.store_meta import StoreMeta
 
 
 @dataclass
 class SqlalchemyTableConverter:
     """Converter for storemeta to / from sqlalchemy tables"""
 
@@ -35,21 +37,29 @@
         columns_by_name = {}
         indexes = []
         for attr_ in store_meta.attrs:
             column = column_factory.create_column(attr_)
             columns_by_name[attr_.name] = column
             args.append(column)
         for index in store_meta.indexes:
-            name = f"idx_{'__'.join(index.attr_names)}"
+            if isinstance(index, AttrIndex):
+                name = f"idx_{index.attr_name}"
+                index_cols = [columns_by_name[index.attr_name]]
+                unique = False
+            elif isinstance(index, UniqueIndex):
+                name = f"idx_{'__'.join(index.attr_names)}"
+                index_cols = [columns_by_name[a] for a in index.attr_names]
+                unique = True
+            else:
+                continue
             if len(name) > 62:
                 name = base64.b64decode(hashlib.md5(name.encode("UTF-8"))).decode(
                     "UTF-8"
                 )
-            index_cols = [columns_by_name[a] for a in index.attr_names]
-            index_obj = Index(name, *index_cols, unique=index.unique)
+            index_obj = Index(name, *index_cols, unique=unique)
             indexes.append(index_obj)
 
         constraint_factory = SqlalchemyConstraintConverter(self.schema)
         args.extend(constraint_factory.get_foreign_key_constraints(store_meta))
         table = Table(*args)
         return table, indexes
```

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_table_store.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_table_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         if row:
             item = self._load_row(row)
             return item
 
     def read_batch(self, keys: List[str]) -> List[Optional[T]]:
         with self.engine.begin() as connection:
             key_config = self.meta.key_config
-            stored_dataclass = self.meta.get_stored_dataclass()
             key_objs = [key_config.to_key_dict(key) for key in keys]
             items = self._read_batch(connection, key_objs)
             items_by_key = {key_config.to_key_str(item): item for item in items}
             items = [items_by_key.get(k) for k in keys]
             return items
 
     def _read_batch(
```

### Comparing `persisty-0.0.3/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py` & `persisty-0.0.5/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/io/__init__.py` & `persisty-0.0.5/persisty/io/__init__.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/io/seed.py` & `persisty-0.0.5/persisty/io/seed.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/key_config/attr_key_config.py` & `persisty-0.0.5/persisty/key_config/attr_key_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/key_config/composite_key_config.py` & `persisty-0.0.5/persisty/key_config/composite_key_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/key_config/key_config_abc.py` & `persisty-0.0.5/persisty/key_config/key_config_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/link/belongs_to.py` & `persisty-0.0.5/persisty/link/belongs_to.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/link/has_count.py` & `persisty-0.0.5/persisty/link/has_count.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/link/has_many.py` & `persisty-0.0.5/persisty/link/has_many.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/link/link_abc.py` & `persisty-0.0.5/persisty/link/link_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/link/linked_store_abc.py` & `persisty-0.0.5/persisty/link/linked_store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/migration/alembic.py` & `persisty-0.0.5/persisty/migration/alembic.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/migration/serverless/dynamodb_yml_config.py` & `persisty-0.0.5/persisty/migration/serverless/dynamodb_yml_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,24 +56,38 @@
                 }
             }
         return {
             "Resources": resources
         }
 
     def build_dynamodb_role_statement_yml(self) -> ExternalItemType:
-        iam_role_statements = []
+        resources = []
         for factory in self.get_dynamodb_store_factories():
             resource_name = factory.table_name.title().replace('_', '')
-            iam_role_statements.append(self._iam_role_statement({"Fn::GetAtt": [resource_name, "Arn"]}))
+            resources.append({"Fn::GetAtt": [resource_name, "Arn"]})
             for index_name, index in factory.global_secondary_indexes.items():
-                iam_role_statements.append(self._iam_role_statement({
+                resources.append({
                     "Fn::Join": ["/", [{"Fn::GetAtt": [resource_name, "Arn"]}, "index", index_name]]
-                }))
+                })
+        iam_role_statement = {
+            "Effect": "Allow",
+            "Action": [
+                "dynamodb:DescribeTable",
+                "dynamodb:Query",
+                "dynamodb:Scan",
+                "dynamodb:BatchGetItem",
+                "dynamodb:GetItem",
+                "dynamodb:PutItem",
+                "dynamodb:UpdateItem",
+                "dynamodb:DeleteItem",
+            ],
+            "Resource": resources
+        }
         return {
-            "iamRoleStatements": iam_role_statements
+            "iamRoleStatements": [iam_role_statement]
         }
 
     @staticmethod
     def _iam_role_statement(resource):
         result = {
             "Effect": "Allow",
             "Action": [
```

### Comparing `persisty-0.0.3/persisty/result_set.py` & `persisty-0.0.5/persisty/result_set.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/and_filter.py` & `persisty-0.0.5/persisty/search_filter/and_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/exclude_all.py` & `persisty-0.0.5/persisty/search_filter/exclude_all.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/filter_factory.py` & `persisty-0.0.5/persisty/search_filter/filter_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/include_all.py` & `persisty-0.0.5/persisty/search_filter/include_all.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/not_filter.py` & `persisty-0.0.5/persisty/search_filter/not_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/or_filter.py` & `persisty-0.0.5/persisty/search_filter/or_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/query_filter.py` & `persisty-0.0.5/persisty/search_filter/query_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/search_filter_abc.py` & `persisty-0.0.5/persisty/search_filter/search_filter_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_filter/search_filter_factory.py` & `persisty-0.0.5/persisty/search_filter/search_filter_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_order/search_order.py` & `persisty-0.0.5/persisty/search_order/search_order.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/search_order/search_order_attr.py` & `persisty-0.0.5/persisty/search_order/search_order_attr.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 @dataclass(frozen=True)
 class SearchOrderAttr(Generic[T]):
     attr: str
     desc: bool = False
 
     def validate_for_attrs(self, attrs: Tuple[Attr, ...]):
-        for f in attrs:
-            if f.name == self.attr:
+        for a in attrs:
+            if a.name == self.attr and a.sortable:
                 return
         raise ValueError(f"search_order_invalid:{self.attr}")
 
     def sort(self, items: Iterator[T]) -> Iterator[T]:
         items = sorted(items, key=self.key, reverse=self.desc)
         return items
```

### Comparing `persisty-0.0.3/persisty/search_order/search_order_factory.py` & `persisty-0.0.5/persisty/search_order/search_order_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/servey/__init__.py` & `persisty-0.0.5/persisty/servey/__init__.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/servey/actions.py` & `persisty-0.0.5/persisty/servey/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import dataclasses
+import inspect
+from inspect import Signature
 from typing import Type, Optional, List
 
 from servey.action.action import Action, action, get_action
 from servey.action.batch_invoker import BatchInvoker
 from servey.security.authorization import Authorization
 from servey.trigger.web_trigger import WebTrigger, WebTriggerMethod
 
@@ -120,15 +122,15 @@
 
     return get_action(delete)
 
 
 def action_for_search(
     store_factory: StoreFactoryABC,
     item_type: Type,
-    search_filter_type: Type[SearchFilterFactoryABC],
+    search_filter_type: Optional[Type[SearchFilterFactoryABC]],
     search_order_type: Type[SearchOrderFactoryABC],
 ) -> Action:
     store_meta = store_factory.get_meta()
     # noinspection PyTypeChecker
     result_set_type = result_set_dataclass_for(item_type)
     setattr(generated, result_set_type.__name__, result_set_type)
 
@@ -167,14 +169,31 @@
         # noinspection PyArgumentList
         result_set = result_set_type(
             results=result_set.results,
             next_page_key=result_set.next_page_key,
         )
         return result_set
 
+    if search_order_type is None:
+        sig = inspect.signature(search)
+        sig = sig.replace(parameters=[p for p in sig.parameters.values() if p.name != 'search_order'])
+        search.__signature__ = sig
+
+    search = action(
+        fn=search,
+        name=f"{store_meta.name}_search",
+        description=f"Run a search in {store_meta.name}",
+        triggers=(
+            WebTrigger(
+                WebTriggerMethod.GET,
+                f"/actions/{store_meta.name.replace('_', '-')}-search",
+            ),
+        ),
+    )
+
     return get_action(search)
 
 
 def action_for_count(
     store_factory: StoreFactoryABC,
     search_filter_type: Type[SearchFilterFactoryABC],
 ) -> Action:
```

### Comparing `persisty-0.0.3/persisty/store/filtered_store.py` & `persisty-0.0.5/persisty/store/filtered_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store/filtered_store_abc.py` & `persisty-0.0.5/persisty/store/filtered_store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store/owned_store.py` & `persisty-0.0.5/persisty/store/owned_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store/restrict_access_store.py` & `persisty-0.0.5/persisty/store/restrict_access_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store/schema_validating_store.py` & `persisty-0.0.5/persisty/store/schema_validating_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store/store_abc.py` & `persisty-0.0.5/persisty/store/store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store/ttl_cache_store.py` & `persisty-0.0.5/persisty/store/ttl_cache_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store/unique_index_store.py` & `persisty-0.0.5/persisty/store/unique_index_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from typing import Optional, List, Dict, Tuple
 
 from persisty.attr.attr_filter import AttrFilter
 from persisty.attr.attr_filter_op import AttrFilterOp
 from persisty.batch_edit import BatchEdit
 from persisty.batch_edit_result import BatchEditResult
 from persisty.errors import PersistyError
-from persisty.index import Index
+from persisty.index.unique_index import UniqueIndex
 from persisty.search_filter.and_filter import And
 from persisty.store.store_abc import StoreABC, T
 from persisty.store.wrapper_store_abc import WrapperStoreABC
 from persisty.util import UNDEFINED
 
 
 @dataclass
 class UniqueIndexStore(WrapperStoreABC[T]):
     store: StoreABC[T]
-    unique_indexes: Tuple[Index, ...]
+    unique_indexes: Tuple[UniqueIndex, ...]
 
     def get_store(self) -> StoreABC[T]:
         return self.store
 
     def create(self, item: T) -> T:
         self._check_create(item)
         return self.get_store().create(item)
@@ -74,11 +74,11 @@
             item = next(results, None)
             if item:
                 raise PersistyError('non_unique_item')
 
 
 def unique_index_store(store: StoreABC):
     meta = store.get_meta()
-    unique_indexes = tuple(i for i in meta.indexes if i.unique)
+    unique_indexes = tuple(i for i in meta.indexes if isinstance(i, UniqueIndex))
     if unique_indexes:
         return UniqueIndexStore(store, unique_indexes)
     return store
```

### Comparing `persisty-0.0.3/persisty/store/wrapper_store_abc.py` & `persisty-0.0.5/persisty/store/wrapper_store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store_access.py` & `persisty-0.0.5/persisty/store_access.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/store_meta.py` & `persisty-0.0.5/persisty/store_meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from marshy.factory.dataclass_marshaller_factory import dataclass_marshaller
 from marshy.marshaller_context import MarshallerContext
 from schemey import SchemaContext, Schema
 from servey.cache_control.cache_control_abc import CacheControlABC
 from servey.cache_control.secure_hash_cache_control import SecureHashCacheControl
 
 from persisty.attr.attr import Attr
-from persisty.index import Index
+from persisty.index.index_abc import IndexABC
 from persisty.key_config.attr_key_config import ATTR_KEY_CONFIG
 from persisty.key_config.key_config_abc import KeyConfigABC
 from persisty.link.link_abc import LinkABC
 from persisty.store_access import StoreAccess, ALL_ACCESS
 
 from persisty.util import to_camel_case
 from persisty.util.undefined import UNDEFINED
@@ -32,15 +32,15 @@
     attrs: Tuple[Attr, ...]
     key_config: KeyConfigABC = ATTR_KEY_CONFIG
     store_access: StoreAccess = ALL_ACCESS
     cache_control: CacheControlABC = SecureHashCacheControl()
     batch_size: int = 100
     description: Optional[str] = None
     links: Tuple[LinkABC, ...] = tuple()
-    indexes: Tuple[Index, ...] = tuple()
+    indexes: Tuple[IndexABC, ...] = tuple()
 
     def get_stored_dataclass(self) -> Type:
         return self._get_dataclass(
             "_stored_dataclass",
             self.name.title().replace("_", ""),
             iter(self.attrs),
             self.links,
@@ -52,23 +52,23 @@
             "_read_dataclass", self.name.title().replace("_", ""), attrs, self.links
         )
 
     def get_create_dataclass(self) -> Type:
         attrs = (a for a in self.attrs if a.creatable)
         return self._get_dataclass(
             "_create_dataclass",
-            self.name.title().replace("_", "") + "CreateInput",
+            self.name.title().replace("_", "") + "Create",
             attrs,
         )
 
     def get_update_dataclass(self) -> Type:
         attrs = (a for a in self.attrs if a.updatable)
         return self._get_dataclass(
             "_update_dataclass",
-            self.name.title().replace("_", "") + "UpdateInput",
+            self.name.title().replace("_", "") + "Update",
             attrs,
         )
 
     def get_search_filter_factory_dataclass(self) -> Optional[Type]:
         search_filter_factory_dataclass = getattr(
             self, "_search_filter_factory_dataclass", UNDEFINED
         )
```

### Comparing `persisty-0.0.3/persisty/stored.py` & `persisty-0.0.5/persisty/stored.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from dataclasses import Field, MISSING
 from typing import Optional, Tuple
 
 from schemey import SchemaContext, get_default_schema_context
 
 from servey.cache_control.cache_control_abc import CacheControlABC
 from servey.cache_control.secure_hash_cache_control import SecureHashCacheControl
@@ -11,15 +12,15 @@
 from persisty.attr.attr_type import attr_type
 from persisty.attr.generator.default_value_generator import DefaultValueGenerator
 from persisty.attr.generator.defaults import (
     get_default_generator_for_create,
     get_default_generator_for_update,
 )
 from persisty.errors import PersistyError
-from persisty.index import Index
+from persisty.index.index_abc import IndexABC
 from persisty.key_config.attr_key_config import AttrKeyConfig
 from persisty.key_config.key_config_abc import KeyConfigABC
 from persisty.link.link_abc import LinkABC
 from persisty.store_meta import StoreMeta
 from persisty.util import to_snake_case
 from persisty.util.undefined import UNDEFINED
 
@@ -27,15 +28,15 @@
 def stored(
     cls=None,
     *,
     key_config: Optional[KeyConfigABC] = None,
     cache_control: Optional[CacheControlABC] = None,
     batch_size: int = 100,
     schema_context: Optional[SchemaContext] = None,
-    indexes: Tuple[Index, ...] = tuple(),
+    indexes: Tuple[IndexABC, ...] = tuple(),
 ):
     """Decorator inspired by dataclasses, containing stored meta."""
     if schema_context is None:
         schema_context = get_default_schema_context()
 
     def wrapper(cls_):
         nonlocal key_config, cache_control, batch_size, indexes
@@ -109,15 +110,15 @@
             )
             attr = Attr(
                 name=name,
                 attr_type=db_type,
                 schema=schema,
                 creatable=creatable,
                 updatable=updatable,
-                sortable=db_type in SORTABLE_TYPES,
+                sortable=os.environ.get('PERSISTY_ATTRS_SORTABLE') == '1' and db_type in SORTABLE_TYPES,
                 create_generator=create_generator,
                 update_generator=update_generator,
                 permitted_filter_ops=permitted_filter_ops,
             )
             attrs_by_name[name] = attr
 
         # Check that all attributes required by the key actually exist...
```

### Comparing `persisty-0.0.3/persisty/trigger/asyncio_trigger_store.py` & `persisty-0.0.5/persisty/trigger/asyncio_trigger_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/trigger/celery_store_trigger_config.py` & `persisty-0.0.5/persisty/trigger/celery_store_trigger_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/trigger/celery_trigger_store.py` & `persisty-0.0.5/persisty/trigger/celery_trigger_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/trigger/dynamodb_post_process_event_handler.py` & `persisty-0.0.5/persisty/trigger/dynamodb_post_process_event_handler.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/trigger/serverless_trigger_handler.py` & `persisty-0.0.5/persisty/trigger/serverless_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/trigger/store_triggers.py` & `persisty-0.0.5/persisty/trigger/store_triggers.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/trigger/wrapper.py` & `persisty-0.0.5/persisty/trigger/wrapper.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/util/__init__.py` & `persisty-0.0.5/persisty/util/__init__.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/util/encrypt_at_rest.py` & `persisty-0.0.5/persisty/util/encrypt_at_rest.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/util/logify.py` & `persisty-0.0.5/persisty/util/logify.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty/util/undefined.py` & `persisty-0.0.5/persisty/util/undefined.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/persisty.egg-info/PKG-INFO` & `persisty-0.0.5/persisty.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: persisty
-Version: 0.0.3
+Version: 0.0.5
 Summary: A better persistence layer for python
 Home-page: https://github.com/tofarr/lambsync
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
+* Appsync is slow. Maybe look at batch processors from API gateway?
+* Check out ordering on search
+
 # Persisty - a better persistence Layer for Python
 
 The objective of this project is to provide a resource oriented approach
 accommodating both security and caching rich enough to handle most use
 cases while still being independant of the underlying persistence 
 mechanism.
```

### Comparing `persisty-0.0.3/persisty.egg-info/SOURCES.txt` & `persisty-0.0.5/persisty.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 marshy_config_persisty/__init__.py
 marshy_config_persisty/sqlalchemy_config.py
 persisty/__init__.py
 persisty/__version__.py
 persisty/batch_edit.py
 persisty/batch_edit_result.py
 persisty/errors.py
-persisty/index.py
 persisty/result_set.py
 persisty/store_access.py
 persisty/store_meta.py
 persisty/stored.py
 persisty.egg-info/PKG-INFO
 persisty.egg-info/SOURCES.txt
 persisty.egg-info/dependency_links.txt
@@ -36,18 +35,18 @@
 persisty/factory/store_factory_abc.py
 persisty/finder/__init__.py
 persisty/finder/module_store_finder.py
 persisty/finder/store_finder_abc.py
 persisty/impl/__init__.py
 persisty/impl/default_store.py
 persisty/impl/dynamodb/__init__.py
-persisty/impl/dynamodb/dynamodb_index.py
 persisty/impl/dynamodb/dynamodb_key_config.py
 persisty/impl/dynamodb/dynamodb_store_factory.py
 persisty/impl/dynamodb/dynamodb_table_store.py
+persisty/impl/dynamodb/partition_sort_index.py
 persisty/impl/mem/__init__.py
 persisty/impl/mem/mem_store.py
 persisty/impl/mem/mem_store_factory.py
 persisty/impl/sqlalchemy/__init__.py
 persisty/impl/sqlalchemy/sqlalchemy_column_converter.py
 persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py
 persisty/impl/sqlalchemy/sqlalchemy_context.py
@@ -61,14 +60,18 @@
 persisty/impl/sqlalchemy/search_filter/field_filter_converter.py
 persisty/impl/sqlalchemy/search_filter/include_all_converter.py
 persisty/impl/sqlalchemy/search_filter/not_filter_converter.py
 persisty/impl/sqlalchemy/search_filter/or_filter_converter.py
 persisty/impl/sqlalchemy/search_filter/query_filter_converter.py
 persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py
 persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py
+persisty/index/__init__.py
+persisty/index/attr_index.py
+persisty/index/index_abc.py
+persisty/index/unique_index.py
 persisty/io/__init__.py
 persisty/io/seed.py
 persisty/key_config/__init__.py
 persisty/key_config/attr_key_config.py
 persisty/key_config/composite_key_config.py
 persisty/key_config/key_config_abc.py
 persisty/link/__init__.py
```

### Comparing `persisty-0.0.3/setup.py` & `persisty-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from persisty.__version__ import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 extras_require = {
     "sql": ["SQLAlchemy~=1.4"],
-    "server": ["servey[server]~=2.6"],
-    "serverless": ["servey[serverless]~=2.6"]
+    "server": ["servey[server]~=2.7"],
+    "serverless": ["servey[serverless]~=2.7"]
 }
 
 setuptools.setup(
     name="persisty",
     version=__version__,
     author="Tim O'Farrell",
     author_email="tofarr@gmail.com",
@@ -21,15 +21,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/tofarr/lambsync",
     packages=setuptools.find_packages(exclude=("tests",)),
     install_requires=[
         "marshy~=3.0",
         "pyaes~=1.6",
         "schemey~=5.7",
-        "servey~=2.6",
+        "servey~=2.7",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `persisty-0.0.3/tests/attr/generator/test_defaults.py` & `persisty-0.0.5/tests/attr/generator/test_defaults.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/attr/test_attr.py` & `persisty-0.0.5/tests/attr/test_attr.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/attr/test_attr_filter.py` & `persisty-0.0.5/tests/attr/test_attr_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/attr/test_attr_filter_op.py` & `persisty-0.0.5/tests/attr/test_attr_filter_op.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/factory/test_default_store_factory.py` & `persisty-0.0.5/tests/factory/test_default_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/factory/test_owned_store_factory.py` & `persisty-0.0.5/tests/factory/test_owned_store_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+import dataclasses
 from unittest import TestCase
 from uuid import UUID
 
 from servey.security.authorization import Authorization
 
 from persisty.factory.default_store_factory import DefaultStoreFactory
 from persisty.factory.owned_store_factory import OwnedStoreFactory
@@ -18,14 +18,19 @@
     text: str
 
 
 class TestOwnedStoreFactory(TestCase):
     def test_getters(self):
         meta = get_meta(Message)
         store = MemStore(meta)
+        meta = dataclasses.replace(meta, attrs=[
+            meta.attrs[0],
+            dataclasses.replace(meta.attrs[1], creatable=False, updatable=False),
+            meta.attrs[2],
+        ])
         factory = OwnedStoreFactory(DefaultStoreFactory(store), "owner")
         self.assertEqual(meta, factory.get_meta())
         subject_1 = Authorization("subject-1", frozenset(), None, None)
         subject_2 = Authorization("subject-2", frozenset(), None, None)
         subject_1_store = factory.create(subject_1)
         subject_2_store = factory.create(subject_2)
         msg_1 = subject_1_store.create(
```

### Comparing `persisty-0.0.3/tests/finder/test_module_store_finder.py` & `persisty-0.0.5/tests/finder/test_module_store_finder.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/fixtures/number_name.py` & `persisty-0.0.5/tests/fixtures/number_name.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from uuid import UUID
 from datetime import datetime, timezone
 
 from marshy import dump
 
+from persisty.attr.attr import Attr
 from persisty.stored import stored
 
 
 @stored(batch_size=10)
 class NumberName:
     """Item linking a string representing a number with an integer value. Also has a uuid, and timestamps."""
 
     id: UUID
     title: str
-    value: int
+    value: int = Attr(sortable=True)
     created_at: datetime
     updated_at: datetime
 
 
 _num2words = {
     1: "One",
     2: "Two",
```

### Comparing `persisty-0.0.3/tests/fixtures/storage_tst_abc.py` & `persisty-0.0.5/tests/fixtures/storage_tst_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/fixtures/super_bowl_results.py` & `persisty-0.0.5/tests/fixtures/super_bowl_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,15 @@
     },
 ]
 
 
 @stored(key_config=AttrKeyConfig("code", AttrType.STR))
 class SuperBowlResult:
     code: str = Attr()
-    year: int = Attr(schema=int_schema(minimum=1967))
+    year: int = Attr(schema=int_schema(minimum=1967), sortable=True)
     date: datetime
     winner_code: str
     runner_up_code: str
     winner_score: int
     runner_up_score: int
```

### Comparing `persisty-0.0.3/tests/impl/dynamodb/test_dynamodb_store.py` & `persisty-0.0.5/tests/impl/dynamodb/test_dynamodb_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from marshy import dump
 from marshy.types import ExternalItemType
 
 from persisty.attr.attr import Attr
 from persisty.attr.attr_type import AttrType
 from persisty.attr.generator.default_value_generator import DefaultValueGenerator
-from persisty.impl.dynamodb.dynamodb_index import DynamodbIndex
+from persisty.impl.dynamodb.partition_sort_index import PartitionSortIndex
 from persisty.impl.dynamodb.dynamodb_store_factory import DynamodbStoreFactory
 from persisty.key_config.attr_key_config import AttrKeyConfig
 from persisty.key_config.composite_key_config import CompositeKeyConfig
 from persisty.result_set import ResultSet
 
 from persisty.search_filter.exclude_all import EXCLUDE_ALL
 from persisty.search_filter.filter_factory import filter_factory
@@ -130,16 +130,16 @@
     def test_dammit(self):
         self.test_create_with_float()
 
     def new_tag_store(self) -> StoreABC:
         store_meta = get_meta(Tag)
         store_factory = DynamodbStoreFactory(
             meta=store_meta,
-            index=DynamodbIndex("pk", "sk"),
-            global_secondary_indexes=dict(gix__sk__pk=DynamodbIndex("sk", "pk")),
+            index=PartitionSortIndex("pk", "sk"),
+            global_secondary_indexes=dict(gix__sk__pk=PartitionSortIndex("sk", "pk")),
         )
         tags = list(
             dump(
                 Tag(
                     int(i / 100),
                     i % 100,
                     str(i),
```

### Comparing `persisty-0.0.3/tests/impl/mem/test_mem_store.py` & `persisty-0.0.5/tests/impl/mem/test_mem_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py` & `persisty-0.0.5/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/util/test_encrypt_at_rest.py` & `persisty-0.0.5/tests/util/test_encrypt_at_rest.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/util/test_logify.py` & `persisty-0.0.5/tests/util/test_logify.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.3/tests/util/test_util.py` & `persisty-0.0.5/tests/util/test_util.py`

 * *Files identical despite different names*

