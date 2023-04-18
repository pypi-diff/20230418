# Comparing `tmp/nobuco-0.1.4.tar.gz` & `tmp/nobuco-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.1.4.tar", last modified: Tue Apr 18 08:15:36 2023, max compression
+gzip compressed data, was "nobuco-0.2.0.tar", last modified: Tue Apr 18 18:55:19 2023, max compression
```

## Comparing `nobuco-0.1.4.tar` & `nobuco-0.2.0.tar`

### file list

```diff
@@ -1,71 +1,87 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.1.4/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.1.4/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 08:15:36.441566 nobuco-0.1.4/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    15947 2023-04-18 07:49:16.000000 nobuco-0.1.4/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.437566 nobuco-0.1.4/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.1.4/docs/channel_ordering.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.1.4/docs/channel_ordering_forced.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    70703 2023-03-24 09:18:07.000000 nobuco-0.1.4/docs/control_if.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.1.4/docs/converter_inside_converter1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.1.4/docs/converter_inside_converter1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.1.4/docs/converter_inside_converter2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.1.4/docs/converter_inside_converter2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.1.4/docs/essentials1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.1.4/docs/essentials1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.1.4/docs/essentials2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.1.4/docs/essentials2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.1.4/docs/essentials3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.1.4/docs/essentials3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.1.4/docs/inplace1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.1.4/docs/inplace1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.1.4/docs/inplace2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.1.4/docs/inplace2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.1.4/docs/inplace3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.1.4/docs/inplace3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.1.4/docs/inplace_empty.png
--rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.1.4/docs/nobuco.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.1.4/docs/tutorial.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.437566 nobuco-0.1.4/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2021-06-04 16:18:38.000000 nobuco-0.1.4/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.1.4/nobuco/commons.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/convert/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:30:24.000000 nobuco-0.1.4/nobuco/convert/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    12608 2023-03-13 12:38:17.000000 nobuco-0.1.4/nobuco/convert/converter.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/convert/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.1.4/nobuco/convert/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.1.4/nobuco/convert/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4894 2023-03-07 15:12:41.000000 nobuco-0.1.4/nobuco/convert/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.1.4/nobuco/convert/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      918 2023-03-08 10:08:07.000000 nobuco-0.1.4/nobuco/convert/layers/weight.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.1.4/nobuco/convert/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.1.4/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2049 2023-03-06 15:27:24.000000 nobuco-0.1.4/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    74178 2023-04-18 08:14:55.000000 nobuco-0.1.4/nobuco/converters/impl.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2459 2023-03-13 12:32:55.000000 nobuco-0.1.4/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      384 2022-12-21 13:41:52.000000 nobuco-0.1.4/nobuco/converters/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2002 2023-03-03 18:45:12.000000 nobuco-0.1.4/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.1.4/nobuco/converters/type_cast.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.1.4/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3152 2023-03-03 13:25:51.000000 nobuco-0.1.4/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13052 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      187 2023-03-03 13:30:15.000000 nobuco-0.1.4/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.1.4/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9354 2023-03-10 20:01:46.000000 nobuco-0.1.4/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2632 2023-03-10 22:18:16.000000 nobuco-0.1.4/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.1.4/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1952 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3172 2023-03-10 22:09:16.000000 nobuco-0.1.4/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 08:15:36.441566 nobuco-0.1.4/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    17781 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1489 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-18 08:15:36.000000 nobuco-0.1.4/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-18 08:15:03.000000 nobuco-0.1.4/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-18 08:15:36.441566 nobuco-0.1.4/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.2.0/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.2.0/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18006 2023-04-18 18:55:19.569498 nobuco-0.2.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16172 2023-04-18 12:28:26.000000 nobuco-0.2.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/docs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.2.0/docs/channel_ordering.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.2.0/docs/channel_ordering_forced.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    67966 2023-04-18 11:28:12.000000 nobuco-0.2.0/docs/control_if.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.2.0/docs/converter_inside_converter1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.2.0/docs/converter_inside_converter1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.2.0/docs/converter_inside_converter2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.2.0/docs/converter_inside_converter2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.2.0/docs/essentials1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.2.0/docs/essentials1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.2.0/docs/essentials2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.2.0/docs/essentials2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.2.0/docs/essentials3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.2.0/docs/essentials3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.2.0/docs/inplace1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.2.0/docs/inplace1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.2.0/docs/inplace2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.2.0/docs/inplace2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.2.0/docs/inplace3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.2.0/docs/inplace3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.2.0/docs/inplace_empty.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.2.0/docs/nobuco.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.2.0/docs/tutorial.png
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      461 2023-04-18 17:44:04.000000 nobuco-0.2.0/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.2.0/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13121 2023-04-18 17:45:07.000000 nobuco-0.2.0/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.2.0/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.2.0/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2455 2023-04-18 11:52:51.000000 nobuco-0.2.0/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.2.0/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.2.0/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.2.0/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.2.0/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3106 2023-04-18 10:12:58.000000 nobuco-0.2.0/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13309 2023-04-18 18:06:08.000000 nobuco-0.2.0/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1275 2023-04-18 18:43:04.000000 nobuco-0.2.0/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.2.0/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.2.0/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4886 2023-04-18 10:06:25.000000 nobuco-0.2.0/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.2.0/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.2.0/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.2.0/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-18 17:59:47.000000 nobuco-0.2.0/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6822 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2863 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.2.0/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.2.0/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.2.0/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9670 2023-04-18 11:49:04.000000 nobuco-0.2.0/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.2.0/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.569498 nobuco-0.2.0/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.2.0/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1943 2023-04-18 10:12:57.000000 nobuco-0.2.0/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3167 2023-04-18 10:12:58.000000 nobuco-0.2.0/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-18 18:55:19.565498 nobuco-0.2.0/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18006 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2055 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-18 18:55:19.000000 nobuco-0.2.0/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-18 10:02:06.000000 nobuco-0.2.0/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-18 18:55:19.569498 nobuco-0.2.0/setup.cfg
```

### Comparing `nobuco-0.1.4/LICENSE` & `nobuco-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/PKG-INFO` & `nobuco-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,27 @@
-Metadata-Version: 2.1
-Name: nobuco
-Version: 0.1.4
-Summary: Pytorch to Tensorflow conversion made somewhat easy
-Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Alexander Lutsenko
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
-Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
-Keywords: pytorch,tensorflow,keras,converter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src="docs/nobuco.png" width="100%">
+<p align="center">
+<img src="docs/nobuco.png">
+</p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
-## Installation
+## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
+
 ```bash
-pip install nobuco
+pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
@@ -78,24 +45,24 @@
         x = 1 - x[:, ::2] * x[:, 1::2]
         return x
 ````
 
 The process is exactly what you would expect. Instantiate the module, create dummy inputs and call the magic function:
 
 ```python
-from nobuco.convert.converter import pytorch_to_keras
-from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
-from nobuco.convert.layers.weight import WeightLayer
+import nobuco
+from nobuco import ChannelOrder, ChannelOrderingStrategy
+from nobuco.layers.weight import WeightLayer
 ```
 
 ````python
 dummy_image = torch.rand(size=(1, 3, 256, 256))
 pytorch_module = MyModule().eval()
 
-keras_model = pytorch_to_keras(
+keras_model = nobuco.pytorch_to_keras(
     pytorch_module,
     args=[dummy_image], kwargs=None,
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW
 )
 ````
 
@@ -107,42 +74,44 @@
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
 Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. A node converter is just a `Callable` that takes in the same arguments as the corresponding node and outputs an equivalent node in tensorflow. The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
 
 This should do the trick:
 
 ````python
-@converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
 ````
 
 <img src="docs/essentials2.svg" width="100%">
 
 It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
 And sure enough, their implementations differ. Have to type in the formula manually, I guess...
 
 ````python
-@converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.clip_by_value(input/6 + 1/2, clip_value_min=0, clip_value_max=1)
 ````
 
 <img src="docs/essentials3.svg" width="100%">
 
 And the happy result:
 
+<p align="center">
 <img src="docs/tutorial.png" width="30%">
+</p>
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
-Reproducing the graph structure is a different matter entirely. Good thing Nobuco has you covered.
+Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
@@ -189,43 +158,47 @@
 
 pytorch_module = MyModule().eval()
 
 inputs = [
     torch.normal(0, 1, size=(1, 12, 32)),
 ]
 
-keras_model = pytorch_to_keras(
+keras_model = nobuco.pytorch_to_keras(
     pytorch_module, inputs,
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
 
+<p align="center">
 <img src="docs/channel_ordering.png" width="30%">
+</p>
 
 For such occasions, there's two brethren functions: `force_tensorflow_order` and `force_pytorch_order`.
 
 ```python
 x, hx = self.gru(x)
-x = force_tensorflow_order(x)
+x = nobuco.force_tensorflow_order(x)
 x1 = self.conv1(x)
 x2 = self.conv2(x)
 ```
 
+<p align="center">
 <img src="docs/channel_ordering_forced.png" width="30%">
+</p>
 
 In case you are curious, the implementation is trivial:
 
 ```python
-@Tracer.traceable()
+@nobuco.traceable
 def force_tensorflow_order(inputs):
     return inputs
 
-@converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
+@nobuco.converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converter_force_tensorflow_order(inputs):
     return lambda inputs: inputs
 ```
 
 `force_pytorch_order` is defined analogously.
 
 ## In-place operations
@@ -255,15 +228,17 @@
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
 As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
+<p align="center">
 <img src="docs/inplace_empty.png" width="30%">
+</p>
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
@@ -273,24 +248,24 @@
 
 <img src="docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
-Stuff like that is way above Nobuco's paygrade, so the module below cannot be properly handled without human intervention.
+Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
 
 ```python
 class ControlIf(nn.Module):
     def __init__(self):
         super().__init__()
-        self.conv_pre = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_true = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_false = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_shared = nn.Conv2d(300, 300, kernel_size=(1, 1))
+        self.conv_pre = nn.Conv2d(3, 16, kernel_size=(1, 1))
+        self.conv_true = nn.Conv2d(16, 32, kernel_size=(1, 1))
+        self.conv_false = nn.Conv2d(16, 32, kernel_size=(1, 1))
+        self.conv_shared = nn.Conv2d(32, 32, kernel_size=(1, 1))
 
     def forward(self, x):
         x = self.conv_pre(x)
         if x.mean() > 0:
             x = self.conv_true(x)
             x = torch.tanh(x)
             x = self.conv_shared(x)
@@ -342,25 +317,30 @@
             x = tf.sigmoid(x)
             x = self.conv_shared(x)
             x = x - 1
         x = self.conv_shared(x)
         return x
 
 
-@converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
+@nobuco.converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converterControlIf(self, x):
     order = ChannelOrder.TENSORFLOW
-    conv_pre = pytorch_to_keras(self.conv_pre, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_true = pytorch_to_keras(self.conv_true, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_false = pytorch_to_keras(self.conv_false, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_shared = pytorch_to_keras(self.conv_shared, [x], inputs_channel_order=order, outputs_channel_order=order)
-    return ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
+    kwargs = {'inputs_channel_order': order, 'outputs_channel_order': order, 'return_outputs_pt': True}
+    
+    conv_pre, out_pre = nobuco.pytorch_to_keras(self.conv_pre, [x], **kwargs)
+    conv_true, out_true = nobuco.pytorch_to_keras(self.conv_true, [out_pre], **kwargs)
+    conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
+    conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
+    layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
+    return layer
 ```
 
+<p align="center">
 <img src="docs/control_if.png" width="30%">
+</p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
@@ -407,16 +387,16 @@
 ```
 
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
-@converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
-def converterAddByMask(self, x, mask):
+@nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
+def converter_AddByMask(self, x, mask):
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
     # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
```

### Comparing `nobuco-0.1.4/README.md` & `nobuco-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,63 @@
-<img src="docs/nobuco.png" width="100%">
+Metadata-Version: 2.1
+Name: nobuco
+Version: 0.2.0
+Summary: Pytorch to Tensorflow conversion made somewhat easy
+Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Alexander Lutsenko
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
+Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
+Keywords: pytorch,tensorflow,keras,converter
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+<img src="docs/nobuco.png">
+</p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
-## Installation
+## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
+
 ```bash
-pip install nobuco
+pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
@@ -42,24 +81,24 @@
         x = 1 - x[:, ::2] * x[:, 1::2]
         return x
 ````
 
 The process is exactly what you would expect. Instantiate the module, create dummy inputs and call the magic function:
 
 ```python
-from nobuco.convert.converter import pytorch_to_keras
-from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
-from nobuco.convert.layers.weight import WeightLayer
+import nobuco
+from nobuco import ChannelOrder, ChannelOrderingStrategy
+from nobuco.layers.weight import WeightLayer
 ```
 
 ````python
 dummy_image = torch.rand(size=(1, 3, 256, 256))
 pytorch_module = MyModule().eval()
 
-keras_model = pytorch_to_keras(
+keras_model = nobuco.pytorch_to_keras(
     pytorch_module,
     args=[dummy_image], kwargs=None,
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW
 )
 ````
 
@@ -71,42 +110,44 @@
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
 Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. A node converter is just a `Callable` that takes in the same arguments as the corresponding node and outputs an equivalent node in tensorflow. The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
 
 This should do the trick:
 
 ````python
-@converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
 ````
 
 <img src="docs/essentials2.svg" width="100%">
 
 It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
 And sure enough, their implementations differ. Have to type in the formula manually, I guess...
 
 ````python
-@converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.clip_by_value(input/6 + 1/2, clip_value_min=0, clip_value_max=1)
 ````
 
 <img src="docs/essentials3.svg" width="100%">
 
 And the happy result:
 
+<p align="center">
 <img src="docs/tutorial.png" width="30%">
+</p>
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
-Reproducing the graph structure is a different matter entirely. Good thing Nobuco has you covered.
+Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
@@ -153,43 +194,47 @@
 
 pytorch_module = MyModule().eval()
 
 inputs = [
     torch.normal(0, 1, size=(1, 12, 32)),
 ]
 
-keras_model = pytorch_to_keras(
+keras_model = nobuco.pytorch_to_keras(
     pytorch_module, inputs,
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
 
+<p align="center">
 <img src="docs/channel_ordering.png" width="30%">
+</p>
 
 For such occasions, there's two brethren functions: `force_tensorflow_order` and `force_pytorch_order`.
 
 ```python
 x, hx = self.gru(x)
-x = force_tensorflow_order(x)
+x = nobuco.force_tensorflow_order(x)
 x1 = self.conv1(x)
 x2 = self.conv2(x)
 ```
 
+<p align="center">
 <img src="docs/channel_ordering_forced.png" width="30%">
+</p>
 
 In case you are curious, the implementation is trivial:
 
 ```python
-@Tracer.traceable()
+@nobuco.traceable
 def force_tensorflow_order(inputs):
     return inputs
 
-@converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
+@nobuco.converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converter_force_tensorflow_order(inputs):
     return lambda inputs: inputs
 ```
 
 `force_pytorch_order` is defined analogously.
 
 ## In-place operations
@@ -219,15 +264,17 @@
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
 As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
+<p align="center">
 <img src="docs/inplace_empty.png" width="30%">
+</p>
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
@@ -237,24 +284,24 @@
 
 <img src="docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
-Stuff like that is way above Nobuco's paygrade, so the module below cannot be properly handled without human intervention.
+Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
 
 ```python
 class ControlIf(nn.Module):
     def __init__(self):
         super().__init__()
-        self.conv_pre = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_true = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_false = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_shared = nn.Conv2d(300, 300, kernel_size=(1, 1))
+        self.conv_pre = nn.Conv2d(3, 16, kernel_size=(1, 1))
+        self.conv_true = nn.Conv2d(16, 32, kernel_size=(1, 1))
+        self.conv_false = nn.Conv2d(16, 32, kernel_size=(1, 1))
+        self.conv_shared = nn.Conv2d(32, 32, kernel_size=(1, 1))
 
     def forward(self, x):
         x = self.conv_pre(x)
         if x.mean() > 0:
             x = self.conv_true(x)
             x = torch.tanh(x)
             x = self.conv_shared(x)
@@ -306,25 +353,30 @@
             x = tf.sigmoid(x)
             x = self.conv_shared(x)
             x = x - 1
         x = self.conv_shared(x)
         return x
 
 
-@converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
+@nobuco.converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converterControlIf(self, x):
     order = ChannelOrder.TENSORFLOW
-    conv_pre = pytorch_to_keras(self.conv_pre, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_true = pytorch_to_keras(self.conv_true, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_false = pytorch_to_keras(self.conv_false, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_shared = pytorch_to_keras(self.conv_shared, [x], inputs_channel_order=order, outputs_channel_order=order)
-    return ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
+    kwargs = {'inputs_channel_order': order, 'outputs_channel_order': order, 'return_outputs_pt': True}
+    
+    conv_pre, out_pre = nobuco.pytorch_to_keras(self.conv_pre, [x], **kwargs)
+    conv_true, out_true = nobuco.pytorch_to_keras(self.conv_true, [out_pre], **kwargs)
+    conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
+    conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
+    layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
+    return layer
 ```
 
+<p align="center">
 <img src="docs/control_if.png" width="30%">
+</p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
@@ -371,16 +423,16 @@
 ```
 
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
-@converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
-def converterAddByMask(self, x, mask):
+@nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
+def converter_AddByMask(self, x, mask):
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
     # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
```

### Comparing `nobuco-0.1.4/docs/channel_ordering.png` & `nobuco-0.2.0/docs/channel_ordering.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/channel_ordering_forced.png` & `nobuco-0.2.0/docs/channel_ordering_forced.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/converter_inside_converter1.html` & `nobuco-0.2.0/docs/converter_inside_converter1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/converter_inside_converter1.svg` & `nobuco-0.2.0/docs/converter_inside_converter1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/converter_inside_converter2.html` & `nobuco-0.2.0/docs/converter_inside_converter2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/converter_inside_converter2.svg` & `nobuco-0.2.0/docs/converter_inside_converter2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/essentials1.html` & `nobuco-0.2.0/docs/essentials1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/essentials1.svg` & `nobuco-0.2.0/docs/essentials1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/essentials2.html` & `nobuco-0.2.0/docs/essentials2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/essentials2.svg` & `nobuco-0.2.0/docs/essentials2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/essentials3.html` & `nobuco-0.2.0/docs/essentials3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/essentials3.svg` & `nobuco-0.2.0/docs/essentials3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/inplace1.html` & `nobuco-0.2.0/docs/inplace1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/inplace1.svg` & `nobuco-0.2.0/docs/inplace1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/inplace2.html` & `nobuco-0.2.0/docs/inplace2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/inplace2.svg` & `nobuco-0.2.0/docs/inplace2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/inplace3.html` & `nobuco-0.2.0/docs/inplace3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/inplace3.svg` & `nobuco-0.2.0/docs/inplace3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/inplace_empty.png` & `nobuco-0.2.0/docs/inplace_empty.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/nobuco.png` & `nobuco-0.2.0/docs/nobuco.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/docs/tutorial.png` & `nobuco-0.2.0/docs/tutorial.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/nobuco/commons.py` & `nobuco-0.2.0/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/nobuco/convert/converter.py` & `nobuco-0.2.0/nobuco/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import random
 import time
 import warnings
 from typing import Callable, Dict, Collection, Optional, List, Union, Tuple
 
 import torch
+from nobuco.converters.tensor import permute_pytorch2keras
 from torch import nn
 import tensorflow as tf
 from tensorflow import keras
 
-from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TF_TENSOR_CLASSES, CONVERTED_OP_DICT
-from nobuco.convert.layers.channel_order import ChangeOrderingLayer, SetOrderLayer
-from nobuco.convert.layers.container import TransientContainer
-from nobuco.convert.layers.stub import UnimplementedOpStub
-from nobuco.converters.channel_ordering import t_pytorch2keras, set_channel_order
-from nobuco.convert.validation import validate, ValidationStatus, ValidationResult, ConversionResult
+from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TF_TENSOR_CLASSES
+from nobuco.converters.channel_ordering import t_pytorch2keras, set_channel_order, t_keras2pytorch
+from nobuco.converters.validation import validate, ValidationResult, ConversionResult
+from nobuco.layers.channel_order import ChangeOrderingLayer
+from nobuco.layers.container import TransientContainer
+from nobuco.layers.stub import UnimplementedOpStub
 from nobuco.util import get_torch_tensor_identifier, collect_recursively, replace_recursively_func, \
     clone_torch_tensors_recursively
 from nobuco.entity.keras import KerasConvertedNode
 from nobuco.entity.pytorch import PytorchNode, PytorchNodeHierarchy
 from nobuco.trace.trace import Tracer
 from nobuco.converters.node_converter import CONVERTER_DICT, Pytorch2KerasNodeConverter
+from nobuco.vis.html_stylizer import HtmlStylizer
 
 # Load default converters
-from nobuco.converters import impl
+# noinspection PyUnresolvedReferences
+from nobuco.node_converters import *
 
 # Trace pytorch ops right away
-from nobuco.vis.html_stylizer import HtmlStylizer
-
 Tracer.decorate_all()
 
 
 def has_converter(node: PytorchNode, converter_dict: Dict[object, Pytorch2KerasNodeConverter]) -> bool:
     return node.get_type() in converter_dict.keys()
 
 
@@ -173,26 +173,35 @@
 def collect_conversion_results(keras_node: KerasConvertedNode) -> Dict[PytorchNode, ConversionResult]:
     conversion_result_dict = {keras_node.pytorch_node: keras_node.conversion_result}
     for child in keras_node.children:
         conversion_result_dict.update(collect_conversion_results(child))
     return conversion_result_dict
 
 
-def prepare_inputs_tf(inputs_pt, inputs_channel_order):
+def prepare_inputs_tf(inputs_pt, inputs_channel_order, input_shapes):
 
     def collect_func(obj):
         return isinstance(obj, torch.Tensor)
 
     def replace_func(obj: torch.Tensor) -> torch.Tensor:
         if isinstance(inputs_channel_order, Dict):
             channel_order = inputs_channel_order.get(obj, ChannelOrder.TENSORFLOW)
         else:
             channel_order = inputs_channel_order
+
         tens = t_pytorch2keras(obj, channel_order=channel_order)
-        return set_channel_order(keras.Input(batch_shape=tens.shape), channel_order)
+
+        if input_shapes is not None and obj in input_shapes:
+            shape = input_shapes.get(obj)
+            if channel_order == ChannelOrder.TENSORFLOW:
+                shape = permute_pytorch2keras(shape)
+        else:
+            shape = tens.shape
+
+        return set_channel_order(keras.Input(batch_shape=shape), channel_order)
 
     return replace_recursively_func(inputs_pt, collect_func, replace_func)
 
 
 def postprocess_outputs_tf(outputs, outputs_channel_order):
     processed = []
     outputs = collect_recursively(outputs, TF_TENSOR_CLASSES)
@@ -217,25 +226,26 @@
     processed = [tf.identity(t) for t in processed]
     return processed
 
 
 def pytorch_to_keras(
         module: nn.Module,
         args=[], kwargs={},
+        input_shapes: Dict[torch.Tensor, Collection[Optional[int]]] = None,
         inputs_channel_order: Union[ChannelOrder, Dict[torch.Tensor, ChannelOrder]] = ChannelOrder.TENSORFLOW,
         outputs_channel_order: Union[ChannelOrder, Dict[int, ChannelOrder]] = None,
         converter_dict=CONVERTER_DICT,
         constants_to_variables: bool = True,
         full_validation: bool = True,
         validation_tolerance=1e-4,
         save_trace_html=False,
-) -> keras.Model:
+        return_outputs_pt=False
+) -> Union[keras.Model, Tuple[keras.Model, object]]:
     start = time.time()
     node_hierarchy = Tracer.trace(module, args, kwargs)
-    # print(node_hierarchy)
 
     keras_converted_node = convert_hierarchy(node_hierarchy, converter_dict,
                                              reuse_layers=True, full_validation=full_validation, constants_to_variables=constants_to_variables,
                                              tolerance=validation_tolerance,
                                              )
 
     validation_result_dict = collect_validation_results(keras_converted_node)
@@ -252,18 +262,22 @@
     if unimplemented_hierarchy is not None:
         print('Unimplemented nodes:')
         print(unimplemented_hierarchy.__str__(validation_result_dict=validation_result_dict, conversion_result_dict=conversion_result_dict))
         raise Exception('Unimplemented nodes')
 
     keras_op = keras_converted_node.keras_op
 
-    args_tf = prepare_inputs_tf(args, inputs_channel_order)
-    kwargs_tf = prepare_inputs_tf(kwargs, inputs_channel_order)
+    args_tf, kwargs_tf = prepare_inputs_tf((args, kwargs), inputs_channel_order, input_shapes)
     outputs_tf = keras_op(*args_tf, **kwargs_tf)
     outputs_tf = postprocess_outputs_tf(outputs_tf, outputs_channel_order)
 
     inputs_tf_flat = collect_recursively((args_tf, kwargs_tf), TF_TENSOR_CLASSES)
     keras_model = keras.Model(inputs_tf_flat, outputs_tf)
 
     elapsed = time.time() - start
     print(f'Conversion complete. Elapsed time: {elapsed:.2f} sec.')
-    return keras_model
+
+    if return_outputs_pt:
+        outputs_pt = node_hierarchy.node.outputs
+        return keras_model, outputs_pt
+    else:
+        return keras_model
```

### Comparing `nobuco-0.1.4/nobuco/convert/layers/channel_order.py` & `nobuco-0.2.0/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/nobuco/convert/layers/container.py` & `nobuco-0.2.0/nobuco/layers/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from nobuco.commons import TF_TENSOR_CLASSES
-from nobuco.convert.layers.weight import WeightLayer
+from nobuco.layers.weight import WeightLayer
 from nobuco.converters.channel_ordering import TensorPlaceholder, template_insert_recursively
 from nobuco.util import collect_recursively
 
 
 class ConnectivityStatus:
     def __init__(self, unused_inputs, unreached_outputs, unused_nodes, unprovided_inputs):
         self.unused_inputs = unused_inputs
```

### Comparing `nobuco-0.1.4/nobuco/convert/layers/weight.py` & `nobuco-0.2.0/nobuco/layers/weight.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 
 from nobuco.commons import ChannelOrderingStrategy
-from nobuco.convert.layers.channel_order import ChangeOrderingLayer
+from nobuco.layers.channel_order import ChangeOrderingLayer
 
 
 class WeightLayer(tf.keras.layers.Layer):
     def __init__(self, weight_shape, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.weight_shape = weight_shape
         self.weight = self.add_weight('weight', shape=weight_shape)
```

### Comparing `nobuco-0.1.4/nobuco/convert/validation.py` & `nobuco-0.2.0/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/nobuco/converters/channel_ordering.py` & `nobuco-0.2.0/nobuco/converters/channel_ordering.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from dataclasses import dataclass
 
 import tensorflow as tf
 import torch
 
-from nobuco.commons import ChannelOrder
+from nobuco.commons import ChannelOrder, TF_TENSOR_CLASSES
 from nobuco.converters.tensor import _permute, perm_pytorch2keras, perm_keras2pytorch
 from nobuco.util import replace_recursively_func
 
 
 def set_channel_order(tensor, channel_order: ChannelOrder):
     tensor.channel_order = channel_order
     return tensor
 
 
 def get_channel_order(tensor) -> ChannelOrder:
     return tensor.channel_order
 
 
 def t_keras2pytorch(tensor_tf, restore_channel_order=False):
-    if restore_channel_order and tensor_tf.channel_order == ChannelOrder.TENSORFLOW:
+    if restore_channel_order and get_channel_order(tensor_tf) == ChannelOrder.TENSORFLOW:
         tensor_tf = _permute(perm_keras2pytorch(len(tensor_tf.shape)))(tensor_tf)
     tensor_pt = torch.as_tensor(tensor_tf.numpy())
     return tensor_pt
 
 
 def t_pytorch2keras(tensor_pt, channel_order=ChannelOrder.PYTORCH):
     tensor_tf = tf.convert_to_tensor(tensor_pt.detach().numpy())
@@ -39,14 +39,25 @@
 
     def replace_func(obj):
         return t_pytorch2keras(obj, channel_order=channel_order)
 
     return replace_recursively_func(obj, collect_func, replace_func)
 
 
+def keras2pytorch_recursively(obj, restore_channel_order=False):
+
+    def collect_func(obj):
+        return isinstance(obj, TF_TENSOR_CLASSES)
+
+    def replace_func(obj):
+        return t_keras2pytorch(obj, restore_channel_order=restore_channel_order)
+
+    return replace_recursively_func(obj, collect_func, replace_func)
+
+
 @dataclass
 class TensorPlaceholder:
     idx: int
 
 
 def make_template_recursively(obj):
     i = 0
```

### Comparing `nobuco-0.1.4/nobuco/converters/node_converter.py` & `nobuco-0.2.0/nobuco/converters/node_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable
 
-from nobuco.convert.layers.channel_order import ChangeOrderingLayer
-from nobuco.convert.validation import validate_diff_default
+from nobuco.converters.validation import validate_diff_default
 from nobuco.commons import ChannelOrderingStrategy
+from nobuco.layers.channel_order import ChangeOrderingLayer
 from nobuco.trace.trace import Tracer
 
 CONVERTER_DICT = {}
 
 
 class Pytorch2KerasNodeConverter:
     def __call__(self, *args, **kwargs):
@@ -62,8 +62,8 @@
 
 def converter_unregister(op, converter_dict=None):
     if converter_dict is None:
         converter_dict = CONVERTER_DICT
 
     op = Tracer.op_unwrap(op)
     if op in converter_dict:
-        del converter_dict[op]
+        del converter_dict[op]
```

### Comparing `nobuco-0.1.4/nobuco/converters/tensor.py` & `nobuco-0.2.0/nobuco/converters/tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 
 def perm_compose(perm_next, perm_prev):
     assert len(perm_next) == len(perm_prev)
     res = [None] * len(perm_prev)
     for i2, i1 in enumerate(perm_next):
         res[i2] = perm_prev[i1]
-
     return res
 
 
 def perm_keras2pytorch(n_dims):
     dims = [i for i in range(n_dims)]
     # Sic!
     return [dim_pytorch2keras(d, n_dims) for d in dims]
@@ -57,14 +56,18 @@
     return [dim_pytorch2keras(d, num_dims) for d in dims]
 
 
 def permute_pytorch2keras(xs):
     return perm_compose(perm_pytorch2keras(len(xs)), xs)
 
 
+def permute_keras2pytorch(xs):
+    return perm_compose(perm_keras2pytorch(len(xs)), xs)
+
+
 def is_identity_perm(perm):
     return all(i == p for i, p in enumerate(perm))
 
 
 # FIXME: find a better place for these
 
 def _permute(perm):
```

### Comparing `nobuco-0.1.4/nobuco/converters/type_cast.py` & `nobuco-0.2.0/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/nobuco/entity/keras.py` & `nobuco-0.2.0/nobuco/entity/keras.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Collection
 
-from nobuco.convert.validation import ValidationResult, ValidationStatus, ConversionResult
+from nobuco.converters.validation import ValidationResult, ConversionResult
 from nobuco.entity.pytorch import PytorchNode
-from sty import bg, ef, fg, rs
 
 
 class KerasConvertedNode:
     def __init__(self, keras_op, pytorch_node: PytorchNode,
                  validation_result: ValidationResult, conversion_result: ConversionResult,
                  input_names: Collection[int], output_names: Collection[int],
                  children: Collection):
```

### Comparing `nobuco-0.1.4/nobuco/entity/pytorch.py` & `nobuco-0.2.0/nobuco/entity/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from typing import Collection, List
 
 import torch
 from torch import nn
 
-from nobuco.convert.validation import ValidationStatus
+from nobuco.converters.validation import ValidationStatus
 
 from nobuco.converters.channel_ordering import make_template_recursively
 from nobuco.util import collect_recursively, get_torch_tensor_identifier
 from nobuco.vis.console_stylizer import ConsoleStylizer
 
 
 class WrappedOp:
@@ -140,15 +140,17 @@
                 dtype = str(obj.dtype).split('.')[-1]
                 return stylizer.stylize(f'{dtype}_{name}' + '<' + ','.join([str(s) for s in obj.shape]) + '>', style)
             elif isinstance(obj, torch.Size):
                 return f'Size{tuple(obj)}'
             elif isinstance(obj, str):
                 return f'"{str(obj)}"'
             elif isinstance(obj, slice):
-                return f"{str(obj.start) if obj.start is not None else ''}:{obj.stop if obj.stop is not None else ''}{f':{obj.step}' if obj.step is not None else ''}"
+                return f"{to_str(obj.start, connectivity_status, parent_connectivity_status, is_input) if obj.start is not None else ''}:" \
+                       f"{to_str(obj.stop, connectivity_status, parent_connectivity_status, is_input) if obj.stop is not None else ''}" \
+                       f"{f':{to_str(obj.step, connectivity_status, parent_connectivity_status, is_input)}' if obj.step is not None else ''}"
             elif isinstance(obj, type(Ellipsis)):
                 return "..."
             elif isinstance(obj, list):
                 return '[' + ', '.join([to_str(el, connectivity_status, parent_connectivity_status, is_input) for el in obj]) + ']'
             elif isinstance(obj, tuple):
                 return '(' + ', '.join([to_str(el, connectivity_status, parent_connectivity_status, is_input) for el in obj]) + ')'
             elif isinstance(obj, dict):
```

### Comparing `nobuco-0.1.4/nobuco/trace/tensor_storage.py` & `nobuco-0.2.0/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.1.4/nobuco/trace/trace.py` & `nobuco-0.2.0/nobuco/trace/trace.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,34 @@
 from torch import nn
 
 from nobuco.entity.pytorch import PytorchNode, WrappedOp, PytorchNodeHierarchy
 from nobuco.trace.tensor_storage import clone_torch_tensors_recursively_with_cache, TensorStorage
 from nobuco.util import collect_recursively
 
 
+# def traceable():
+#     def inner(func_to_trace: Callable) -> Callable:
+#         if Tracer.is_decorated(func_to_trace):
+#             return func_to_trace
+#         else:
+#             module_suffix = func_to_trace.__qualname__
+#             module_suffix = '.'.join(module_suffix.split('.')[:-1])
+#             return Tracer.op_tracing_decorator(func_to_trace, inspect.getmodule(func_to_trace), module_suffix=module_suffix)
+#     return inner
+
+
+def traceable(func_to_trace: Callable):
+    if Tracer.is_decorated(func_to_trace):
+        return func_to_trace
+    else:
+        module_suffix = func_to_trace.__qualname__
+        module_suffix = '.'.join(module_suffix.split('.')[:-1])
+        return Tracer.op_tracing_decorator(func_to_trace, inspect.getmodule(func_to_trace), module_suffix=module_suffix)
+
+
 class Tracer:
     
     op_tracing_classes = [
         torch,
         torch.Tensor,
         torch.linalg,
         torch.nn.functional,
@@ -34,25 +54,14 @@
     _tracing_enabled = False
     _parent_list = []
     _node_list = []
 
     _tensor_storage: TensorStorage = None
 
     @staticmethod
-    def traceable():
-        def inner(func_to_trace: Callable) -> Callable:
-            if Tracer.is_decorated(func_to_trace):
-                return func_to_trace
-            else:
-                module_suffix = func_to_trace.__qualname__
-                module_suffix = '.'.join(module_suffix.split('.')[:-1])
-                return Tracer.op_tracing_decorator(func_to_trace, inspect.getmodule(func_to_trace), module_suffix=module_suffix)
-        return inner
-
-    @staticmethod
     def is_decorated(callable) -> bool:
         return hasattr(callable, '__undecorated_func__')
 
     @staticmethod
     def op_unwrap(callable) -> bool:
         if Tracer.is_decorated(callable):
             return callable.__undecorated_func__
@@ -209,15 +218,15 @@
         Tracer._node_list = []
         Tracer._parent_list = []
         Tracer._tensor_storage = TensorStorage()
 
         if isinstance(module_or_function, nn.Module):
             apply_module_tracing_recursively(module_or_function)
         else:
-            module_or_function = Tracer.traceable()(module_or_function)
+            module_or_function = traceable(module_or_function)
         with torch.no_grad():
             module_or_function(*args, **kwargs)
 
         Tracer._tracing_enabled = False
 
         hierarchy = Tracer.build_hierarchy(Tracer._node_list)
         return hierarchy
```

### Comparing `nobuco-0.1.4/nobuco/util.py` & `nobuco-0.2.0/nobuco/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
             if isinstance(obj, (list, tuple)):
                 for el in obj:
                     collect(el)
             elif isinstance(obj, dict):
                 for k, v in obj.items():
                     collect(k)
                     collect(v)
+            elif isinstance(obj, slice):
+                collect(obj.start)
+                collect(obj.stop)
+                collect(obj.step)
             elif hasattr(obj, '__dict__') and not isinstance(obj, nn.Module):
                 v = vars(obj)
                 collect(v)
 
     collect(obj)
     return collected
```

### Comparing `nobuco-0.1.4/nobuco/vis/console_stylizer.py` & `nobuco-0.2.0/nobuco/vis/console_stylizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from sty import bg, ef, fg, rs
+from sty import ef, fg, rs
 
-from nobuco.convert.layers.container import ConnectivityStatus
-from nobuco.convert.validation import ValidationStatus
+from nobuco.converters.validation import ValidationStatus
+from nobuco.layers.container import ConnectivityStatus
 from nobuco.util import get_torch_tensor_identifier
 
 
 class ConsoleStylizer:
 
     def postprocess(self, text):
         return text
```

### Comparing `nobuco-0.1.4/nobuco/vis/html_stylizer.py` & `nobuco-0.2.0/nobuco/vis/html_stylizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
-from nobuco.convert.layers.container import ConnectivityStatus
-from nobuco.convert.validation import ValidationStatus
+from nobuco.converters.validation import ValidationStatus
+from nobuco.layers.container import ConnectivityStatus
 from nobuco.util import get_torch_tensor_identifier
 
 
 class HtmlStylizer:
 
     def postprocess(self, text):
         text = text.replace('\n', '<br>\n')
```

### Comparing `nobuco-0.1.4/nobuco.egg-info/PKG-INFO` & `nobuco-0.2.0/nobuco.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.1.4
+Version: 0.2.0
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,31 +30,34 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="docs/nobuco.png" width="100%">
+<p align="center">
+<img src="docs/nobuco.png">
+</p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
   - [x] Arbitrary torch functions
 - Simple
 - Flexible
 - Sanity-preserving, with clear mistake messaging
 
 <!-- toc -->
 
-## Installation
+## Installation <img src="https://img.shields.io/pypi/v/nobuco?color=blue&style=flat-square">
+
 ```bash
-pip install nobuco
+pip install -U nobuco
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
@@ -78,24 +81,24 @@
         x = 1 - x[:, ::2] * x[:, 1::2]
         return x
 ````
 
 The process is exactly what you would expect. Instantiate the module, create dummy inputs and call the magic function:
 
 ```python
-from nobuco.convert.converter import pytorch_to_keras
-from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
-from nobuco.convert.layers.weight import WeightLayer
+import nobuco
+from nobuco import ChannelOrder, ChannelOrderingStrategy
+from nobuco.layers.weight import WeightLayer
 ```
 
 ````python
 dummy_image = torch.rand(size=(1, 3, 256, 256))
 pytorch_module = MyModule().eval()
 
-keras_model = pytorch_to_keras(
+keras_model = nobuco.pytorch_to_keras(
     pytorch_module,
     args=[dummy_image], kwargs=None,
     inputs_channel_order=ChannelOrder.TENSORFLOW,
     outputs_channel_order=ChannelOrder.TENSORFLOW
 )
 ````
 
@@ -107,42 +110,44 @@
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
 Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. A node converter is just a `Callable` that takes in the same arguments as the corresponding node and outputs an equivalent node in tensorflow. The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
 
 This should do the trick:
 
 ````python
-@converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
 ````
 
 <img src="docs/essentials2.svg" width="100%">
 
 It works, but the outputs don't quite match. Perhaps we should check on how [pytorch](https://pytorch.org/docs/stable/generated/torch.nn.functional.hardsigmoid.html) and [tensorflow](https://www.tensorflow.org/api_docs/python/tf/keras/activations/hard_sigmoid) define hard sigmoid. 
 And sure enough, their implementations differ. Have to type in the formula manually, I guess...
 
 ````python
-@converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.clip_by_value(input/6 + 1/2, clip_value_min=0, clip_value_max=1)
 ````
 
 <img src="docs/essentials3.svg" width="100%">
 
 And the happy result:
 
+<p align="center">
 <img src="docs/tutorial.png" width="30%">
+</p>
 
 The example above is artificial but it illustrates the point.
 It's not feasible to provide a node converter for every existing pytorch op. There's literally [thousands](https://dev-discuss.pytorch.org/t/where-do-the-2000-pytorch-operators-come-from-more-than-you-wanted-to-know/) of them! 
 Best we can do without the converter constantly lacking essential functionality, being riddled with bugs, doing weird stuff and breaking apart with every other PT/TF release 
 is to keep the tool simple and customizable, make it clear where a problem comes from and let the _user_ sort things out.
 Usually it's easy for a human to translate an isolated operation from one framework to another.
-Reproducing the graph structure is a different matter entirely. Good thing Nobuco has you covered.
+Reproducing the graph structure is a different matter entirely. For that, Nobuco has you covered!
 
 ## Channel order wizardry
 
 Some operations assume its input tensors have a channel dimension. 
 And as you probably know, pytorch and tensorflow do not agree on the layout of such tensors.
 Pytorch adopts channel-first layout (_B**C**H_, _B**C**HW_, etc.) 
 while tensorflow works efficiently with channel-last tensors (_BH**C**_, _BHW**C**_, ...).
@@ -189,43 +194,47 @@
 
 pytorch_module = MyModule().eval()
 
 inputs = [
     torch.normal(0, 1, size=(1, 12, 32)),
 ]
 
-keras_model = pytorch_to_keras(
+keras_model = nobuco.pytorch_to_keras(
     pytorch_module, inputs,
     inputs_channel_order=ChannelOrder.PYTORCH,
 )
 ```
 
 The laziness shoots us in the foot here, and we get not one transpose but two:
 
+<p align="center">
 <img src="docs/channel_ordering.png" width="30%">
+</p>
 
 For such occasions, there's two brethren functions: `force_tensorflow_order` and `force_pytorch_order`.
 
 ```python
 x, hx = self.gru(x)
-x = force_tensorflow_order(x)
+x = nobuco.force_tensorflow_order(x)
 x1 = self.conv1(x)
 x2 = self.conv2(x)
 ```
 
+<p align="center">
 <img src="docs/channel_ordering_forced.png" width="30%">
+</p>
 
 In case you are curious, the implementation is trivial:
 
 ```python
-@Tracer.traceable()
+@nobuco.traceable
 def force_tensorflow_order(inputs):
     return inputs
 
-@converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
+@nobuco.converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converter_force_tensorflow_order(inputs):
     return lambda inputs: inputs
 ```
 
 `force_pytorch_order` is defined analogously.
 
 ## In-place operations
@@ -255,15 +264,17 @@
 
 You see, tensorflow graphs (and many other formats like ONNX) do not support in-place ops.
 So when we take slice (`x[:, 1:2, 16:25, 8::2]`) in TF/ONNX, the result is not a view of the original tensor but a copy. 
 This copy is then passed to `relu` (which is not in-place either), and its result is not used anywhere. 
 As you can see above, the output tensors of `__getitem__` and `relu_` are <span style="color:gray">grayed out</span>, and these operations are excluded from the graph.
 In fact, it's empty:
 
+<p align="center">
 <img src="docs/inplace_empty.png" width="30%">
+</p>
 
 The easiest way of fixing this is to explicitly assign the result to the slice.
 Conveniently enough, most standard in-place operations in pytorch do return their modified arguments as outputs.
 
 ```python
 class MyModule(nn.Module):
     def forward(self, x):
@@ -273,24 +284,24 @@
 
 <img src="docs/inplace3.svg" width="100%">
 
 ## Going dynamic
 
 Introducing python control flow statements into the compute graph is no easy feat.
 Tensorflow can do so via `tf.autograph`, but at a cost of [system's complexity](https://www.youtube.com/watch?v=NIEgzljyDyI) and with some notable [limitations](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/python/autograph/g3doc/reference/control_flow.md).
-Stuff like that is way above Nobuco's paygrade, so the module below cannot be properly handled without human intervention.
+Stuff like that is way above Nobuco's paygrade, so the following module cannot be properly handled without human intervention.
 
 ```python
 class ControlIf(nn.Module):
     def __init__(self):
         super().__init__()
-        self.conv_pre = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_true = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_false = nn.Conv2d(300, 300, kernel_size=(1, 1))
-        self.conv_shared = nn.Conv2d(300, 300, kernel_size=(1, 1))
+        self.conv_pre = nn.Conv2d(3, 16, kernel_size=(1, 1))
+        self.conv_true = nn.Conv2d(16, 32, kernel_size=(1, 1))
+        self.conv_false = nn.Conv2d(16, 32, kernel_size=(1, 1))
+        self.conv_shared = nn.Conv2d(32, 32, kernel_size=(1, 1))
 
     def forward(self, x):
         x = self.conv_pre(x)
         if x.mean() > 0:
             x = self.conv_true(x)
             x = torch.tanh(x)
             x = self.conv_shared(x)
@@ -342,25 +353,30 @@
             x = tf.sigmoid(x)
             x = self.conv_shared(x)
             x = x - 1
         x = self.conv_shared(x)
         return x
 
 
-@converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
+@nobuco.converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converterControlIf(self, x):
     order = ChannelOrder.TENSORFLOW
-    conv_pre = pytorch_to_keras(self.conv_pre, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_true = pytorch_to_keras(self.conv_true, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_false = pytorch_to_keras(self.conv_false, [x], inputs_channel_order=order, outputs_channel_order=order)
-    conv_shared = pytorch_to_keras(self.conv_shared, [x], inputs_channel_order=order, outputs_channel_order=order)
-    return ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
+    kwargs = {'inputs_channel_order': order, 'outputs_channel_order': order, 'return_outputs_pt': True}
+    
+    conv_pre, out_pre = nobuco.pytorch_to_keras(self.conv_pre, [x], **kwargs)
+    conv_true, out_true = nobuco.pytorch_to_keras(self.conv_true, [out_pre], **kwargs)
+    conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
+    conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
+    layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
+    return layer
 ```
 
+<p align="center">
 <img src="docs/control_if.png" width="30%">
+</p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
@@ -407,16 +423,16 @@
 ```
 
 ```python
 import onnx
 from onnx_tf.backend import prepare
 
 
-@converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
-def converterAddByMask(self, x, mask):
+@nobuco.converter(AddByMask, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER, reusable=False)
+def converter_AddByMask(self, x, mask):
     model_path = 'add_by_mask'
     onnx_path = model_path + '.onnx'
 
     # NB: onnx.export in implemented via tracing i.e. it may modify the inputs!
     torch.onnx.export(self, (x, mask), onnx_path, opset_version=12, input_names=['input', 'mask'], dynamic_axes={'input': [0, 1, 2, 3]})
 
     onnx_model = onnx.load(onnx_path)
```

### Comparing `nobuco-0.1.4/nobuco.egg-info/SOURCES.txt` & `nobuco-0.2.0/nobuco.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -22,38 +22,54 @@
 docs/inplace3.html
 docs/inplace3.svg
 docs/inplace_empty.png
 docs/nobuco.png
 docs/tutorial.png
 nobuco/__init__.py
 nobuco/commons.py
+nobuco/convert.py
 nobuco/funcs.py
 nobuco/util.py
 nobuco.egg-info/PKG-INFO
 nobuco.egg-info/SOURCES.txt
 nobuco.egg-info/dependency_links.txt
 nobuco.egg-info/requires.txt
 nobuco.egg-info/top_level.txt
-nobuco/convert/__init__.py
-nobuco/convert/converter.py
-nobuco/convert/validation.py
-nobuco/convert/layers/__init__.py
-nobuco/convert/layers/channel_order.py
-nobuco/convert/layers/container.py
-nobuco/convert/layers/stub.py
-nobuco/convert/layers/weight.py
 nobuco/converters/__init__.py
 nobuco/converters/channel_ordering.py
-nobuco/converters/impl.py
 nobuco/converters/node_converter.py
-nobuco/converters/ops.py
 nobuco/converters/tensor.py
 nobuco/converters/type_cast.py
+nobuco/converters/validation.py
 nobuco/entity/__init__.py
 nobuco/entity/keras.py
 nobuco/entity/pytorch.py
+nobuco/layers/__init__.py
+nobuco/layers/channel_order.py
+nobuco/layers/container.py
+nobuco/layers/stub.py
+nobuco/layers/weight.py
+nobuco/node_converters/__init__.py
+nobuco/node_converters/activation.py
+nobuco/node_converters/boolean.py
+nobuco/node_converters/boolean_mask.py
+nobuco/node_converters/comparison.py
+nobuco/node_converters/convolution.py
+nobuco/node_converters/dropout.py
+nobuco/node_converters/interpolation.py
+nobuco/node_converters/linear.py
+nobuco/node_converters/math.py
+nobuco/node_converters/misc.py
+nobuco/node_converters/normalization.py
+nobuco/node_converters/padding.py
+nobuco/node_converters/pooling.py
+nobuco/node_converters/recurrent.py
+nobuco/node_converters/slice.py
+nobuco/node_converters/tensor_cast.py
+nobuco/node_converters/tensor_creation.py
+nobuco/node_converters/tensor_manipulation.py
 nobuco/trace/__init__.py
 nobuco/trace/tensor_storage.py
 nobuco/trace/trace.py
 nobuco/vis/__init__.py
 nobuco/vis/console_stylizer.py
 nobuco/vis/html_stylizer.py
```

### Comparing `nobuco-0.1.4/pyproject.toml` & `nobuco-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.1.4"
+version = "0.2.0"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

