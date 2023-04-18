# Comparing `tmp/pydin-0.0.0.tar.gz` & `tmp/pydin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydin-0.0.0.tar", last modified: Mon May  2 18:38:34 2022, max compression
+gzip compressed data, was "pydin-0.2.0.tar", last modified: Tue Apr 18 20:28:56 2023, max compression
```

## Comparing `pydin-0.0.0.tar` & `pydin-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,37 @@
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2022-05-02 18:38:34.723565 pydin-0.0.0/
--rw-r--r--   0 timur      (501) staff       (20)     1074 2022-05-02 18:19:56.000000 pydin-0.0.0/LICENSE
--rw-r--r--   0 timur      (501) staff       (20)      440 2022-05-02 18:38:34.723446 pydin-0.0.0/PKG-INFO
--rw-r--r--   0 timur      (501) staff       (20)        0 2022-05-02 18:15:08.000000 pydin-0.0.0/README.md
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2022-05-02 18:38:34.721472 pydin-0.0.0/pydin/
--rw-r--r--   0 timur      (501) staff       (20)      254 2022-05-02 18:29:55.000000 pydin-0.0.0/pydin/__init__.py
-drwxr-xr-x   0 timur      (501) staff       (20)        0 2022-05-02 18:38:34.723266 pydin-0.0.0/pydin.egg-info/
--rw-r--r--   0 timur      (501) staff       (20)      440 2022-05-02 18:38:34.000000 pydin-0.0.0/pydin.egg-info/PKG-INFO
--rw-r--r--   0 timur      (501) staff       (20)      160 2022-05-02 18:38:34.000000 pydin-0.0.0/pydin.egg-info/SOURCES.txt
--rw-r--r--   0 timur      (501) staff       (20)        1 2022-05-02 18:38:34.000000 pydin-0.0.0/pydin.egg-info/dependency_links.txt
--rw-r--r--   0 timur      (501) staff       (20)        6 2022-05-02 18:38:34.000000 pydin-0.0.0/pydin.egg-info/top_level.txt
--rw-r--r--   0 timur      (501) staff       (20)       38 2022-05-02 18:38:34.723609 pydin-0.0.0/setup.cfg
--rw-r--r--   0 timur      (501) staff       (20)     1090 2022-05-02 18:30:09.000000 pydin-0.0.0/setup.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-04-18 20:28:56.669298 pydin-0.2.0/
+-rw-r--r--   0 timur      (501) staff       (20)     1093 2020-04-24 13:39:18.000000 pydin-0.2.0/LICENSE
+-rw-r--r--   0 timur      (501) staff       (20)     7795 2023-04-18 20:28:56.669129 pydin-0.2.0/PKG-INFO
+-rw-r--r--   0 timur      (501) staff       (20)     7507 2023-04-18 20:02:20.000000 pydin-0.2.0/README.md
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-04-18 20:28:56.663813 pydin-0.2.0/pydin/
+-rw-r--r--   0 timur      (501) staff       (20)     1359 2023-04-18 20:26:56.000000 pydin-0.2.0/pydin/__init__.py
+-rw-r--r--   0 timur      (501) staff       (20)    23651 2023-04-16 02:41:25.000000 pydin-0.2.0/pydin/api.py
+-rw-r--r--   0 timur      (501) staff       (20)      107 2020-07-20 19:33:48.000000 pydin-0.2.0/pydin/cache.py
+-rw-r--r--   0 timur      (501) staff       (20)    25197 2023-04-15 19:49:51.000000 pydin-0.2.0/pydin/cli.py
+-rw-r--r--   0 timur      (501) staff       (20)     4945 2023-04-18 20:08:58.000000 pydin-0.2.0/pydin/config.py
+-rw-r--r--   0 timur      (501) staff       (20)      230 2023-04-15 19:07:04.000000 pydin-0.2.0/pydin/const.py
+-rw-r--r--   0 timur      (501) staff       (20)   107291 2023-04-16 19:44:39.000000 pydin-0.2.0/pydin/core.py
+-rw-r--r--   0 timur      (501) staff       (20)     9245 2023-04-18 20:09:55.000000 pydin-0.2.0/pydin/db.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-04-18 20:28:56.666706 pydin-0.2.0/pydin/demo/
+-rw-r--r--   0 timur      (501) staff       (20)      996 2022-12-26 20:06:45.000000 pydin-0.2.0/pydin/demo/cli.txt
+-rw-r--r--   0 timur      (501) staff       (20)      482 2022-12-26 20:06:54.000000 pydin-0.2.0/pydin/demo/web.txt
+-rw-r--r--   0 timur      (501) staff       (20)     1800 2023-04-15 19:07:28.000000 pydin-0.2.0/pydin/fields.py
+-rw-r--r--   0 timur      (501) staff       (20)     1344 2023-01-11 22:22:05.000000 pydin-0.2.0/pydin/logger.py
+-rw-r--r--   0 timur      (501) staff       (20)    88015 2023-04-17 07:27:37.000000 pydin-0.2.0/pydin/models.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-04-18 20:28:56.668533 pydin-0.2.0/pydin/samples/
+-rw-r--r--   0 timur      (501) staff       (20)     2135 2020-06-02 18:45:38.000000 pydin-0.2.0/pydin/samples/gitignore.txt
+-rw-r--r--   0 timur      (501) staff       (20)      151 2022-12-15 10:53:53.000000 pydin-0.2.0/pydin/samples/head.txt
+-rw-r--r--   0 timur      (501) staff       (20)       83 2023-01-11 17:51:27.000000 pydin-0.2.0/pydin/samples/job.txt
+-rw-r--r--   0 timur      (501) staff       (20)       70 2023-01-11 17:49:00.000000 pydin-0.2.0/pydin/samples/scheduler.txt
+-rw-r--r--   0 timur      (501) staff       (20)       51 2023-01-11 17:48:21.000000 pydin-0.2.0/pydin/samples/script.txt
+-rw-r--r--   0 timur      (501) staff       (20)     5140 2023-04-15 19:46:58.000000 pydin-0.2.0/pydin/sources.py
+-rw-r--r--   0 timur      (501) staff       (20)    44055 2023-04-18 20:08:51.000000 pydin-0.2.0/pydin/utils.py
+-rw-r--r--   0 timur      (501) staff       (20)     9157 2022-12-27 12:16:07.000000 pydin-0.2.0/pydin/web.py
+-rw-r--r--   0 timur      (501) staff       (20)     1230 2023-04-16 23:02:41.000000 pydin-0.2.0/pydin/wrap.py
+drwxr-xr-x   0 timur      (501) staff       (20)        0 2023-04-18 20:28:56.666239 pydin-0.2.0/pydin.egg-info/
+-rw-r--r--   0 timur      (501) staff       (20)     7795 2023-04-18 20:28:56.000000 pydin-0.2.0/pydin.egg-info/PKG-INFO
+-rw-r--r--   0 timur      (501) staff       (20)      557 2023-04-18 20:28:56.000000 pydin-0.2.0/pydin.egg-info/SOURCES.txt
+-rw-r--r--   0 timur      (501) staff       (20)        1 2023-04-18 20:28:56.000000 pydin-0.2.0/pydin.egg-info/dependency_links.txt
+-rw-r--r--   0 timur      (501) staff       (20)      154 2023-04-18 20:28:56.000000 pydin-0.2.0/pydin.egg-info/requires.txt
+-rw-r--r--   0 timur      (501) staff       (20)        6 2023-04-18 20:28:56.000000 pydin-0.2.0/pydin.egg-info/top_level.txt
+-rw-r--r--   0 timur      (501) staff       (20)       38 2023-04-18 20:28:56.669354 pydin-0.2.0/setup.cfg
+-rw-r--r--   0 timur      (501) staff       (20)     1400 2023-04-18 15:37:09.000000 pydin-0.2.0/setup.py
```

### Comparing `pydin-0.0.0/LICENSE` & `pydin-0.2.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2022 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2020 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

