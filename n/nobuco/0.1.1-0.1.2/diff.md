# Comparing `tmp/nobuco-0.1.1.tar.gz` & `tmp/nobuco-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.1.1.tar", last modified: Sun Apr 16 17:34:39 2023, max compression
+gzip compressed data, was "nobuco-0.1.2.tar", last modified: Tue Apr 18 07:52:41 2023, max compression
```

## Comparing `nobuco-0.1.1.tar` & `nobuco-0.1.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.031311 nobuco-0.1.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.1.1/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.1.1/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    17729 2023-04-16 17:34:39.031311 nobuco-0.1.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    15895 2023-04-16 17:33:51.000000 nobuco-0.1.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.1.1/docs/channel_ordering.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.1.1/docs/channel_ordering_forced.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    70703 2023-03-24 09:18:07.000000 nobuco-0.1.1/docs/control_if.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.1.1/docs/converter_inside_converter1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.1.1/docs/converter_inside_converter1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.1.1/docs/converter_inside_converter2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.1.1/docs/converter_inside_converter2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.1.1/docs/essentials1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.1.1/docs/essentials1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.1.1/docs/essentials2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.1.1/docs/essentials2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.1.1/docs/essentials3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.1.1/docs/essentials3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.1.1/docs/inplace1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.1.1/docs/inplace1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.1.1/docs/inplace2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.1.1/docs/inplace2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.1.1/docs/inplace3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.1.1/docs/inplace3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.1.1/docs/inplace_empty.png
--rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.1.1/docs/nobuco.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.1.1/docs/tutorial.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2021-06-04 16:18:38.000000 nobuco-0.1.1/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.1.1/nobuco/commons.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/convert/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:30:24.000000 nobuco-0.1.1/nobuco/convert/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    12608 2023-03-13 12:38:17.000000 nobuco-0.1.1/nobuco/convert/converter.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/convert/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.1.1/nobuco/convert/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.1.1/nobuco/convert/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2023-03-07 15:12:41.000000 nobuco-0.1.1/nobuco/convert/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.1.1/nobuco/convert/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      918 2023-03-08 10:08:07.000000 nobuco-0.1.1/nobuco/convert/layers/weight.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.1.1/nobuco/convert/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.1.1/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2049 2023-03-06 15:27:24.000000 nobuco-0.1.1/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    71864 2023-04-16 17:28:21.000000 nobuco-0.1.1/nobuco/converters/impl.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2459 2023-03-13 12:32:55.000000 nobuco-0.1.1/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      384 2022-12-21 13:41:52.000000 nobuco-0.1.1/nobuco/converters/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2002 2023-03-03 18:45:12.000000 nobuco-0.1.1/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.1.1/nobuco/converters/type_cast.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.1.1/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3152 2023-03-03 13:25:51.000000 nobuco-0.1.1/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13052 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-03-03 13:30:15.000000 nobuco-0.1.1/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.031311 nobuco-0.1.1/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.1.1/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9354 2023-03-10 20:01:46.000000 nobuco-0.1.1/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2632 2023-03-10 22:18:16.000000 nobuco-0.1.1/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.031311 nobuco-0.1.1/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.1.1/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1952 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3172 2023-03-10 22:09:16.000000 nobuco-0.1.1/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-16 17:34:39.027311 nobuco-0.1.1/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    17729 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1489 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-16 17:34:39.000000 nobuco-0.1.1/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-16 17:34:03.000000 nobuco-0.1.1/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-16 17:34:39.031311 nobuco-0.1.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.964064 nobuco-0.1.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.1.2/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.1.2/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 07:52:41.964064 nobuco-0.1.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15947 2023-04-18 07:49:16.000000 nobuco-0.1.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/docs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.1.2/docs/channel_ordering.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.1.2/docs/channel_ordering_forced.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    70703 2023-03-24 09:18:07.000000 nobuco-0.1.2/docs/control_if.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.1.2/docs/converter_inside_converter1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.1.2/docs/converter_inside_converter1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.1.2/docs/converter_inside_converter2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.1.2/docs/converter_inside_converter2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.1.2/docs/essentials1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.1.2/docs/essentials1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.1.2/docs/essentials2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.1.2/docs/essentials2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.1.2/docs/essentials3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.1.2/docs/essentials3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.1.2/docs/inplace1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.1.2/docs/inplace1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.1.2/docs/inplace2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.1.2/docs/inplace2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.1.2/docs/inplace3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.1.2/docs/inplace3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.1.2/docs/inplace_empty.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.1.2/docs/nobuco.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.1.2/docs/tutorial.png
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2021-06-04 16:18:38.000000 nobuco-0.1.2/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.1.2/nobuco/commons.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/nobuco/convert/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:30:24.000000 nobuco-0.1.2/nobuco/convert/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    12608 2023-03-13 12:38:17.000000 nobuco-0.1.2/nobuco/convert/converter.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/nobuco/convert/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.1.2/nobuco/convert/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.1.2/nobuco/convert/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2023-03-07 15:12:41.000000 nobuco-0.1.2/nobuco/convert/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.1.2/nobuco/convert/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      918 2023-03-08 10:08:07.000000 nobuco-0.1.2/nobuco/convert/layers/weight.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.1.2/nobuco/convert/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.1.2/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2049 2023-03-06 15:27:24.000000 nobuco-0.1.2/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    74100 2023-04-18 07:47:56.000000 nobuco-0.1.2/nobuco/converters/impl.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2459 2023-03-13 12:32:55.000000 nobuco-0.1.2/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      384 2022-12-21 13:41:52.000000 nobuco-0.1.2/nobuco/converters/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2002 2023-03-03 18:45:12.000000 nobuco-0.1.2/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.1.2/nobuco/converters/type_cast.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.1.2/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3152 2023-03-03 13:25:51.000000 nobuco-0.1.2/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13052 2023-03-10 22:09:16.000000 nobuco-0.1.2/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-03-03 13:30:15.000000 nobuco-0.1.2/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.1.2/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.1.2/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9354 2023-03-10 20:01:46.000000 nobuco-0.1.2/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2632 2023-03-10 22:18:16.000000 nobuco-0.1.2/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.964064 nobuco-0.1.2/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.1.2/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1952 2023-03-10 22:09:16.000000 nobuco-0.1.2/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3172 2023-03-10 22:09:16.000000 nobuco-0.1.2/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 07:52:41.960064 nobuco-0.1.2/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 07:52:41.000000 nobuco-0.1.2/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1489 2023-04-18 07:52:41.000000 nobuco-0.1.2/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-18 07:52:41.000000 nobuco-0.1.2/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-18 07:52:41.000000 nobuco-0.1.2/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-18 07:52:41.000000 nobuco-0.1.2/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-18 07:49:28.000000 nobuco-0.1.2/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-18 07:52:41.964064 nobuco-0.1.2/setup.cfg
```

### Comparing `nobuco-0.1.1/LICENSE` & `nobuco-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/PKG-INFO` & `nobuco-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -146,15 +146,15 @@
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
 Transposing tensors between the two layouts incurs non-trivial overhead as generally, tensor data must be physically rearranged.
 In an effort to keep that overhead to the minimum, Nobuco does layout coercions _lazily_. 
 A couple of things are needed to make it possible:
 
-- Tensorflow tensors are augmented with an additional property which stores their channel order.
+- Tensorflow tensors are augmented with an additional property which stores their channel order, either pytorch (channel first) or tensorflow (channel last) style.
 - Node converters have requirements on what channel order their inputs must have. Said requirements are expressed with `channel_ordering_strategy` argument. 
 
 Channel ordering strategies are
 - `FORCE_TENSORFLOW_ORDER`
   - Input tensors will be coerced to tensorflow channel order.
   - Convenient for converting channel-aware operations (convolution, batchnorm).
 - `FORCE_PYTORCH_ORDER`
@@ -416,15 +416,15 @@
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
     # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
-    tf_rep: TensorflowRep = prepare(onnx_model)
+    tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
```

### Comparing `nobuco-0.1.1/README.md` & `nobuco-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
 Transposing tensors between the two layouts incurs non-trivial overhead as generally, tensor data must be physically rearranged.
 In an effort to keep that overhead to the minimum, Nobuco does layout coercions _lazily_. 
 A couple of things are needed to make it possible:
 
-- Tensorflow tensors are augmented with an additional property which stores their channel order.
+- Tensorflow tensors are augmented with an additional property which stores their channel order, either pytorch (channel first) or tensorflow (channel last) style.
 - Node converters have requirements on what channel order their inputs must have. Said requirements are expressed with `channel_ordering_strategy` argument. 
 
 Channel ordering strategies are
 - `FORCE_TENSORFLOW_ORDER`
   - Input tensors will be coerced to tensorflow channel order.
   - Convenient for converting channel-aware operations (convolution, batchnorm).
 - `FORCE_PYTORCH_ORDER`
@@ -380,15 +380,15 @@
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
     # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
-    tf_rep: TensorflowRep = prepare(onnx_model)
+    tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
```

### Comparing `nobuco-0.1.1/docs/channel_ordering.png` & `nobuco-0.1.2/docs/channel_ordering.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/channel_ordering_forced.png` & `nobuco-0.1.2/docs/channel_ordering_forced.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/control_if.png` & `nobuco-0.1.2/docs/control_if.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/converter_inside_converter1.html` & `nobuco-0.1.2/docs/converter_inside_converter1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/converter_inside_converter1.svg` & `nobuco-0.1.2/docs/converter_inside_converter1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/converter_inside_converter2.html` & `nobuco-0.1.2/docs/converter_inside_converter2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/converter_inside_converter2.svg` & `nobuco-0.1.2/docs/converter_inside_converter2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/essentials1.html` & `nobuco-0.1.2/docs/essentials1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/essentials1.svg` & `nobuco-0.1.2/docs/essentials1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/essentials2.html` & `nobuco-0.1.2/docs/essentials2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/essentials2.svg` & `nobuco-0.1.2/docs/essentials2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/essentials3.html` & `nobuco-0.1.2/docs/essentials3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/essentials3.svg` & `nobuco-0.1.2/docs/essentials3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/inplace1.html` & `nobuco-0.1.2/docs/inplace1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/inplace1.svg` & `nobuco-0.1.2/docs/inplace1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/inplace2.html` & `nobuco-0.1.2/docs/inplace2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/inplace2.svg` & `nobuco-0.1.2/docs/inplace2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/inplace3.html` & `nobuco-0.1.2/docs/inplace3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/inplace3.svg` & `nobuco-0.1.2/docs/inplace3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/inplace_empty.png` & `nobuco-0.1.2/docs/inplace_empty.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/nobuco.png` & `nobuco-0.1.2/docs/nobuco.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/docs/tutorial.png` & `nobuco-0.1.2/docs/tutorial.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/commons.py` & `nobuco-0.1.2/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/convert/converter.py` & `nobuco-0.1.2/nobuco/convert/converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/convert/layers/channel_order.py` & `nobuco-0.1.2/nobuco/convert/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/convert/layers/container.py` & `nobuco-0.1.2/nobuco/convert/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/convert/layers/weight.py` & `nobuco-0.1.2/nobuco/convert/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/convert/validation.py` & `nobuco-0.1.2/nobuco/convert/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/converters/channel_ordering.py` & `nobuco-0.1.2/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/converters/impl.py` & `nobuco-0.1.2/nobuco/converters/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     groups = self.groups
     padding = self.padding
     stride = self.stride
     dilation = self.dilation
 
     out_filters, in_filters, kw = weight.shape
     weights = weight.detach().numpy()
-    weights = weights.transpose((2, 1, 0))
+    weights = weights.transpose((2, 0, 1))
 
     if bias is not None:
         biases = bias.detach().numpy()
         params = [weights, biases]
         use_bias = True
     else:
         params = [weights]
@@ -385,45 +385,84 @@
         if pad_layer is not None:
             input = pad_layer(input)
         output = conv(input)
         return output
     return func
 
 
-# @converter(F.conv1d)
-# def conv1d(input: Tensor, weight: Tensor, bias: Optional[Tensor]=None, stride: Union[_int, _size]=1, padding: str="valid", dilation: Union[_int, _size]=1, groups: _int=1):
-#     out_filters, in_filters, kw = weight.shape
-#     weights = weight.detach().numpy()
-#     weights = weights.transpose((2, 1, 0))
-#
-#     if bias is not None:
-#         biases = bias.detach().numpy()
-#         params = [weights, biases]
-#         use_bias = True
-#     else:
-#         params = [weights]
-#         use_bias = False
-#
-#     if padding != 0:
-#         pad_layer = keras.layers.ZeroPadding1D(padding)
-#     else:
-#         pad_layer = None
-#
-#     conv = keras.layers.Conv1D(out_filters, kernel_size=kw,
-#                          strides=stride, padding='valid',
-#                          # dilation_rate=dilations, groups=groups,
-#                          use_bias=use_bias,
-#                          weights=params
-#                          )
-#
-#     def func(input, *args, **kwargs):
-#         if pad_layer is not None:
-#             input = pad_layer(input)
-#         return conv(input)
-#     return func
+@converter(F.conv1d)
+def conv1d(input: Tensor, weight: Tensor, bias: Optional[Tensor]=None, stride: Union[_int, _size]=1, padding: str="valid", dilation: Union[_int, _size]=1, groups: _int=1):
+    out_filters, in_filters, kw = weight.shape
+    weights = weight.detach().numpy()
+    weights = weights.transpose((2, 0, 1))
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
+    def func(input, *args, **kwargs):
+        if pad_layer is not None:
+            input = pad_layer(input)
+        output = conv(input)
+        return output
+    return func
 
 
 @converter(nn.Conv2d)
 def conv2d(self, input: Tensor):
     weight = self.weight
     bias = self.bias
     groups = self.groups
@@ -1432,15 +1471,16 @@
         return tf.reshape(input, shape)
     return func
 
 
 @converter(torch.masked_select, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def masked_select(input: Tensor, mask: Tensor, *, out: Optional[Tensor]=None):
     def func(input, mask, *, out=None):
-        return tf.boolean_mask(input, mask)
+        # return tf.boolean_mask(input, mask)
+        return input[mask]
     return func
 
 
 @converter(torch.masked_fill, torch.Tensor.masked_fill, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def masked_fill(input: Tensor, mask: Tensor, value: Number):
     def func(input, mask, value):
         value = tf.convert_to_tensor(value, dtype=input.dtype)
@@ -1865,14 +1905,28 @@
         x, _ = tf.unique(input)
         if sorted:
             x = tf.sort(x)
         return x
     return func
 
 
+@converter(torch.isnan, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def isnan(input: Tensor):
+    def func(input):
+        return tf.math.is_nan(input)
+    return func
+
+
+@converter(torch.Tensor.__invert__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def invert(input: Tensor):
+    def func(input):
+        return tf.math.logical_not(input)
+    return func
+
+
 @converter(torch.clone, torch.Tensor.clone, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def clone(input: Tensor, *, memory_format=None):
     def func(input: Tensor, *, memory_format=None):
         return tf.identity(input)
     return func
```

### Comparing `nobuco-0.1.1/nobuco/converters/node_converter.py` & `nobuco-0.1.2/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/converters/tensor.py` & `nobuco-0.1.2/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/converters/type_cast.py` & `nobuco-0.1.2/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/entity/keras.py` & `nobuco-0.1.2/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/entity/pytorch.py` & `nobuco-0.1.2/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/trace/tensor_storage.py` & `nobuco-0.1.2/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/trace/trace.py` & `nobuco-0.1.2/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/util.py` & `nobuco-0.1.2/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/vis/console_stylizer.py` & `nobuco-0.1.2/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco/vis/html_stylizer.py` & `nobuco-0.1.2/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/nobuco.egg-info/PKG-INFO` & `nobuco-0.1.2/nobuco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -146,15 +146,15 @@
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
 Transposing tensors between the two layouts incurs non-trivial overhead as generally, tensor data must be physically rearranged.
 In an effort to keep that overhead to the minimum, Nobuco does layout coercions _lazily_. 
 A couple of things are needed to make it possible:
 
-- Tensorflow tensors are augmented with an additional property which stores their channel order.
+- Tensorflow tensors are augmented with an additional property which stores their channel order, either pytorch (channel first) or tensorflow (channel last) style.
 - Node converters have requirements on what channel order their inputs must have. Said requirements are expressed with `channel_ordering_strategy` argument. 
 
 Channel ordering strategies are
 - `FORCE_TENSORFLOW_ORDER`
   - Input tensors will be coerced to tensorflow channel order.
   - Convenient for converting channel-aware operations (convolution, batchnorm).
 - `FORCE_PYTORCH_ORDER`
@@ -416,15 +416,15 @@
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
     # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
-    tf_rep: TensorflowRep = prepare(onnx_model)
+    tf_rep = prepare(onnx_model)
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
```

### Comparing `nobuco-0.1.1/nobuco.egg-info/SOURCES.txt` & `nobuco-0.1.2/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.1/pyproject.toml` & `nobuco-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

