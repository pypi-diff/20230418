# Comparing `tmp/nobuco-0.1.3.tar.gz` & `tmp/nobuco-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.1.3.tar", last modified: Tue Apr 18 08:13:43 2023, max compression
+gzip compressed data, was "nobuco-0.1.4.tar", last modified: Tue Apr 18 08:15:36 2023, max compression
```

## Comparing `nobuco-0.1.3.tar` & `nobuco-0.1.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.958048 nobuco-0.1.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.1.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.1.3/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 08:13:43.958048 nobuco-0.1.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    15947 2023-04-18 07:49:16.000000 nobuco-0.1.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.954048 nobuco-0.1.3/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.1.3/docs/channel_ordering.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.1.3/docs/channel_ordering_forced.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    70703 2023-03-24 09:18:07.000000 nobuco-0.1.3/docs/control_if.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.1.3/docs/converter_inside_converter1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.1.3/docs/converter_inside_converter1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.1.3/docs/converter_inside_converter2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.1.3/docs/converter_inside_converter2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.1.3/docs/essentials1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.1.3/docs/essentials1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.1.3/docs/essentials2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.1.3/docs/essentials2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.1.3/docs/essentials3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.1.3/docs/essentials3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.1.3/docs/inplace1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.1.3/docs/inplace1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.1.3/docs/inplace2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.1.3/docs/inplace2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.1.3/docs/inplace3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.1.3/docs/inplace3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.1.3/docs/inplace_empty.png
--rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.1.3/docs/nobuco.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.1.3/docs/tutorial.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.954048 nobuco-0.1.3/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2021-06-04 16:18:38.000000 nobuco-0.1.3/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.1.3/nobuco/commons.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.954048 nobuco-0.1.3/nobuco/convert/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:30:24.000000 nobuco-0.1.3/nobuco/convert/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    12608 2023-03-13 12:38:17.000000 nobuco-0.1.3/nobuco/convert/converter.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.954048 nobuco-0.1.3/nobuco/convert/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.1.3/nobuco/convert/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.1.3/nobuco/convert/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2023-03-07 15:12:41.000000 nobuco-0.1.3/nobuco/convert/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.1.3/nobuco/convert/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      918 2023-03-08 10:08:07.000000 nobuco-0.1.3/nobuco/convert/layers/weight.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.1.3/nobuco/convert/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.954048 nobuco-0.1.3/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.1.3/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2049 2023-03-06 15:27:24.000000 nobuco-0.1.3/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    74330 2023-04-18 08:12:46.000000 nobuco-0.1.3/nobuco/converters/impl.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2459 2023-03-13 12:32:55.000000 nobuco-0.1.3/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      384 2022-12-21 13:41:52.000000 nobuco-0.1.3/nobuco/converters/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2002 2023-03-03 18:45:12.000000 nobuco-0.1.3/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.1.3/nobuco/converters/type_cast.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.958048 nobuco-0.1.3/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.1.3/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3152 2023-03-03 13:25:51.000000 nobuco-0.1.3/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13052 2023-03-10 22:09:16.000000 nobuco-0.1.3/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-03-03 13:30:15.000000 nobuco-0.1.3/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.958048 nobuco-0.1.3/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.1.3/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.1.3/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9354 2023-03-10 20:01:46.000000 nobuco-0.1.3/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2632 2023-03-10 22:18:16.000000 nobuco-0.1.3/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.958048 nobuco-0.1.3/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.1.3/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1952 2023-03-10 22:09:16.000000 nobuco-0.1.3/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3172 2023-03-10 22:09:16.000000 nobuco-0.1.3/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:13:43.954048 nobuco-0.1.3/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 08:13:43.000000 nobuco-0.1.3/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1489 2023-04-18 08:13:43.000000 nobuco-0.1.3/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-18 08:13:43.000000 nobuco-0.1.3/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-18 08:13:43.000000 nobuco-0.1.3/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-18 08:13:43.000000 nobuco-0.1.3/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-18 08:13:20.000000 nobuco-0.1.3/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-18 08:13:43.958048 nobuco-0.1.3/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.1.4/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.1.4/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 08:15:36.441566 nobuco-0.1.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15947 2023-04-18 07:49:16.000000 nobuco-0.1.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.437566 nobuco-0.1.4/docs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.1.4/docs/channel_ordering.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.1.4/docs/channel_ordering_forced.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    70703 2023-03-24 09:18:07.000000 nobuco-0.1.4/docs/control_if.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.1.4/docs/converter_inside_converter1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.1.4/docs/converter_inside_converter1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.1.4/docs/converter_inside_converter2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.1.4/docs/converter_inside_converter2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.1.4/docs/essentials1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.1.4/docs/essentials1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.1.4/docs/essentials2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.1.4/docs/essentials2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.1.4/docs/essentials3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.1.4/docs/essentials3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.1.4/docs/inplace1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.1.4/docs/inplace1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.1.4/docs/inplace2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.1.4/docs/inplace2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.1.4/docs/inplace3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.1.4/docs/inplace3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.1.4/docs/inplace_empty.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.1.4/docs/nobuco.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.1.4/docs/tutorial.png
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.437566 nobuco-0.1.4/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2021-06-04 16:18:38.000000 nobuco-0.1.4/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.1.4/nobuco/commons.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/convert/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:30:24.000000 nobuco-0.1.4/nobuco/convert/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    12608 2023-03-13 12:38:17.000000 nobuco-0.1.4/nobuco/convert/converter.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/convert/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.1.4/nobuco/convert/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.1.4/nobuco/convert/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2023-03-07 15:12:41.000000 nobuco-0.1.4/nobuco/convert/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.1.4/nobuco/convert/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      918 2023-03-08 10:08:07.000000 nobuco-0.1.4/nobuco/convert/layers/weight.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.1.4/nobuco/convert/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.1.4/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2049 2023-03-06 15:27:24.000000 nobuco-0.1.4/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    74178 2023-04-18 08:14:55.000000 nobuco-0.1.4/nobuco/converters/impl.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2459 2023-03-13 12:32:55.000000 nobuco-0.1.4/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      384 2022-12-21 13:41:52.000000 nobuco-0.1.4/nobuco/converters/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2002 2023-03-03 18:45:12.000000 nobuco-0.1.4/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.1.4/nobuco/converters/type_cast.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.1.4/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3152 2023-03-03 13:25:51.000000 nobuco-0.1.4/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13052 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-03-03 13:30:15.000000 nobuco-0.1.4/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.1.4/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9354 2023-03-10 20:01:46.000000 nobuco-0.1.4/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2632 2023-03-10 22:18:16.000000 nobuco-0.1.4/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.1.4/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1952 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3172 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1489 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-18 08:15:03.000000 nobuco-0.1.4/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-18 08:15:36.441566 nobuco-0.1.4/setup.cfg
```

### Comparing `nobuco-0.1.3/LICENSE` & `nobuco-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/PKG-INFO` & `nobuco-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.1.3/README.md` & `nobuco-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/channel_ordering.png` & `nobuco-0.1.4/docs/channel_ordering.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/channel_ordering_forced.png` & `nobuco-0.1.4/docs/channel_ordering_forced.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/control_if.png` & `nobuco-0.1.4/docs/control_if.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/converter_inside_converter1.html` & `nobuco-0.1.4/docs/converter_inside_converter1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/converter_inside_converter1.svg` & `nobuco-0.1.4/docs/converter_inside_converter1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/converter_inside_converter2.html` & `nobuco-0.1.4/docs/converter_inside_converter2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/converter_inside_converter2.svg` & `nobuco-0.1.4/docs/converter_inside_converter2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/essentials1.html` & `nobuco-0.1.4/docs/essentials1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/essentials1.svg` & `nobuco-0.1.4/docs/essentials1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/essentials2.html` & `nobuco-0.1.4/docs/essentials2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/essentials2.svg` & `nobuco-0.1.4/docs/essentials2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/essentials3.html` & `nobuco-0.1.4/docs/essentials3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/essentials3.svg` & `nobuco-0.1.4/docs/essentials3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/inplace1.html` & `nobuco-0.1.4/docs/inplace1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/inplace1.svg` & `nobuco-0.1.4/docs/inplace1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/inplace2.html` & `nobuco-0.1.4/docs/inplace2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/inplace2.svg` & `nobuco-0.1.4/docs/inplace2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/inplace3.html` & `nobuco-0.1.4/docs/inplace3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/inplace3.svg` & `nobuco-0.1.4/docs/inplace3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/inplace_empty.png` & `nobuco-0.1.4/docs/inplace_empty.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/nobuco.png` & `nobuco-0.1.4/docs/nobuco.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/docs/tutorial.png` & `nobuco-0.1.4/docs/tutorial.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/commons.py` & `nobuco-0.1.4/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/convert/converter.py` & `nobuco-0.1.4/nobuco/convert/converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/convert/layers/channel_order.py` & `nobuco-0.1.4/nobuco/convert/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/convert/layers/container.py` & `nobuco-0.1.4/nobuco/convert/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/convert/layers/weight.py` & `nobuco-0.1.4/nobuco/convert/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/convert/validation.py` & `nobuco-0.1.4/nobuco/convert/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/converters/channel_ordering.py` & `nobuco-0.1.4/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/converters/impl.py` & `nobuco-0.1.4/nobuco/converters/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,94 +306,94 @@
 @converter(torch.abs, torch.Tensor.abs, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def abs(input: Tensor, *, out: Optional[Tensor]=None):
     def func(input, *, out=None):
         return tf.abs(input)
     return func
 
 
-# @converter(nn.Conv1d)
-# def conv1d(self, input: Tensor):
-#     weight = self.weight
-#     bias = self.bias
-#     groups = self.groups
-#     padding = self.padding
-#     stride = self.stride
-#     dilation = self.dilation
-#
-#     out_filters, in_filters, kw = weight.shape
-#     weights = weight.detach().numpy()
-#     if groups == out_filters and groups != 1:
-#         weights = tf.transpose(weights, (2, 0, 1))
-#     else:
-#         weights = tf.transpose(weights, (2, 1, 0))
-#
-#     if bias is not None:
-#         biases = bias.detach().numpy()
-#         params = [weights, biases]
-#         use_bias = True
-#     else:
-#         params = [weights]
-#         use_bias = False
-#
-#     if isinstance(padding, numbers.Number):
-#         padding = (padding,)
-#     if padding != (0,) and padding != 'valid':
-#         pad_layer = keras.layers.ZeroPadding1D(padding[0])
-#     else:
-#         pad_layer = None
-#
-#     if groups == out_filters and groups != 1:
-#         conv = keras.layers.DepthwiseConv1D(kernel_size=kw,
-#                                       strides=stride,
-#                                       padding='valid',
-#                                       dilation_rate=dilation,
-#                                       groups=groups,
-#                                       use_bias=use_bias,
-#                                       weights=params
-#                                       )
-#     elif groups == 1:
-#         conv = keras.layers.Conv1D(filters=out_filters,
-#                              kernel_size=kw,
-#                              strides=stride,
-#                              padding='valid',
-#                              dilation_rate=dilation,
-#                              groups=groups,
-#                              use_bias=use_bias,
-#                              weights=params
-#                              )
-#     else:
-#         def split_params(params, groups, axis):
-#             params_split = [np.split(p, groups, axis=axis) for p in params]
-#             return list(zip(*params_split))
-#
-#         params_split = split_params(params, groups, axis=-1)
-#
-#         def grouped_conv1d(inputs, filters, kernel_size, strides, groups, dilation=dilation):
-#             splits = tf.split(inputs, groups, axis=-1)
-#             convolved_splits = [
-#                 keras.layers.Conv1D(filters // groups,
-#                                     kernel_size=kernel_size,
-#                                     strides=strides,
-#                                     padding='valid',
-#                                     dilation_rate=dilation,
-#                                     use_bias=use_bias,
-#                                     weights=params_split[i]
-#                                     )(split)
-#                 for i, split in enumerate(splits)
-#             ]
-#             return tf.concat(convolved_splits, -1)
-#
-#         conv = lambda x: grouped_conv1d(x, out_filters, kernel_size=kw, strides=stride, groups=groups, dilation=dilation)
-#
-#     def func(input):
-#         if pad_layer is not None:
-#             input = pad_layer(input)
-#         output = conv(input)
-#         return output
-#     return func
+@converter(nn.Conv1d)
+def conv1d(self, input: Tensor):
+    weight = self.weight
+    bias = self.bias
+    groups = self.groups
+    padding = self.padding
+    stride = self.stride
+    dilation = self.dilation
+
+    out_filters, in_filters, kw = weight.shape
+    weights = weight.detach().numpy()
+    if groups == out_filters and groups != 1:
+        weights = tf.transpose(weights, (2, 0, 1))
+    else:
+        weights = tf.transpose(weights, (2, 1, 0))
+
+    if bias is not None:
+        biases = bias.detach().numpy()
+        params = [weights, biases]
+        use_bias = True
+    else:
+        params = [weights]
+        use_bias = False
+
+    if isinstance(padding, numbers.Number):
+        padding = (padding,)
+    if padding != (0,) and padding != 'valid':
+        pad_layer = keras.layers.ZeroPadding1D(padding[0])
+    else:
+        pad_layer = None
+
+    if groups == out_filters and groups != 1:
+        conv = keras.layers.DepthwiseConv1D(kernel_size=kw,
+                                      strides=stride,
+                                      padding='valid',
+                                      dilation_rate=dilation,
+                                      groups=groups,
+                                      use_bias=use_bias,
+                                      weights=params
+                                      )
+    elif groups == 1:
+        conv = keras.layers.Conv1D(filters=out_filters,
+                             kernel_size=kw,
+                             strides=stride,
+                             padding='valid',
+                             dilation_rate=dilation,
+                             groups=groups,
+                             use_bias=use_bias,
+                             weights=params
+                             )
+    else:
+        def split_params(params, groups, axis):
+            params_split = [np.split(p, groups, axis=axis) for p in params]
+            return list(zip(*params_split))
+
+        params_split = split_params(params, groups, axis=-1)
+
+        def grouped_conv1d(inputs, filters, kernel_size, strides, groups, dilation=dilation):
+            splits = tf.split(inputs, groups, axis=-1)
+            convolved_splits = [
+                keras.layers.Conv1D(filters // groups,
+                                    kernel_size=kernel_size,
+                                    strides=strides,
+                                    padding='valid',
+                                    dilation_rate=dilation,
+                                    use_bias=use_bias,
+                                    weights=params_split[i]
+                                    )(split)
+                for i, split in enumerate(splits)
+            ]
+            return tf.concat(convolved_splits, -1)
+
+        conv = lambda x: grouped_conv1d(x, out_filters, kernel_size=kw, strides=stride, groups=groups, dilation=dilation)
+
+    def func(input):
+        if pad_layer is not None:
+            input = pad_layer(input)
+        output = conv(input)
+        return output
+    return func
 
 
 @converter(F.conv1d)
 def conv1d(input: Tensor, weight: Tensor, bias: Optional[Tensor]=None, stride: Union[_int, _size]=1, padding: str="valid", dilation: Union[_int, _size]=1, groups: _int=1):
     out_filters, in_filters, kw = weight.shape
     weights = weight.detach().numpy()
     if groups == out_filters and groups != 1:
```

### Comparing `nobuco-0.1.3/nobuco/converters/node_converter.py` & `nobuco-0.1.4/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/converters/tensor.py` & `nobuco-0.1.4/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/converters/type_cast.py` & `nobuco-0.1.4/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/entity/keras.py` & `nobuco-0.1.4/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/entity/pytorch.py` & `nobuco-0.1.4/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/trace/tensor_storage.py` & `nobuco-0.1.4/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/trace/trace.py` & `nobuco-0.1.4/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/util.py` & `nobuco-0.1.4/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/vis/console_stylizer.py` & `nobuco-0.1.4/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco/vis/html_stylizer.py` & `nobuco-0.1.4/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/nobuco.egg-info/PKG-INFO` & `nobuco-0.1.4/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.1.3/nobuco.egg-info/SOURCES.txt` & `nobuco-0.1.4/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.3/pyproject.toml` & `nobuco-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.1.3"
+version = "0.1.4"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

