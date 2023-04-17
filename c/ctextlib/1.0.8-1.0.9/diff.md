# Comparing `tmp/ctextlib-1.0.8.tar.gz` & `tmp/ctextlib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ctextlib-1.0.8.tar", last modified: Mon Dec 23 02:04:18 2019, max compression
+gzip compressed data, was "dist\ctextlib-1.0.9.tar", last modified: Sun Jan  5 13:44:10 2020, max compression
```

## Comparing `ctextlib-1.0.8.tar` & `ctextlib-1.0.9.tar`

### file list

```diff
@@ -1,74 +1,78 @@
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/
--rw-rw-rw-   0        0        0      130 2019-12-19 09:37:24.000000 ctextlib-1.0.8/CMakeLists.txt
--rw-rw-rw-   0        0        0     2182 2017-08-31 18:59:27.000000 ctextlib-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      127 2017-08-31 18:59:27.000000 ctextlib-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    39660 2019-12-23 02:04:18.000000 ctextlib-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    26517 2019-12-23 02:02:39.000000 ctextlib-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/ctextlib.egg-info/
--rw-rw-rw-   0        0        0    39660 2019-12-23 02:04:17.000000 ctextlib-1.0.8/ctextlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2019-12-23 02:04:17.000000 ctextlib-1.0.8/ctextlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-12-23 02:04:17.000000 ctextlib-1.0.8/ctextlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-12-19 09:43:44.000000 ctextlib-1.0.8/ctextlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2019-12-23 02:04:17.000000 ctextlib-1.0.8/ctextlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/
--rw-rw-rw-   0        0        0     6507 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/include/
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    19063 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     4326 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    89703 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     7701 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      120 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2001 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    25044 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    37278 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     3566 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    16322 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    15073 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0     1450 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    29043 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0     7731 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     3865 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     3599 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     5655 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    67677 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0     8749 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2031 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0    97575 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    58356 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/pytypes.h
--rw-rw-rw-   0        0        0    14029 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    23134 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/include/pybind11/stl_bind.h
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/
--rw-rw-rw-   0        0        0     9502 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/
--rw-rw-rw-   0        0        0     2042 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-rw-   0        0        0      686 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-rw-   0        0        0      474 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-rw-   0        0        0     1056 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-rw-   0        0        0      852 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-rw-   0        0        0      373 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-rw-   0        0        0      695 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tests/test_embed/
--rw-rw-rw-   0        0        0     1527 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tests/test_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/pybind11/tools/
--rw-rw-rw-   0        0        0     2100 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tools/FindCatch.cmake
--rw-rw-rw-   0        0        0     2995 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tools/FindEigen3.cmake
--rw-rw-rw-   0        0        0     8360 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-rw-   0        0        0     9597 2019-10-14 23:57:24.000000 ctextlib-1.0.8/pybind11/tools/pybind11Tools.cmake
--rw-rw-rw-   0        0        0       42 2019-12-23 02:04:18.000000 ctextlib-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3088 2019-12-23 02:04:10.000000 ctextlib-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2019-12-23 02:04:18.000000 ctextlib-1.0.8/src/
--rw-rw-rw-   0        0        0      204 2019-12-03 11:42:17.000000 ctextlib-1.0.8/src/CText.h
--rw-rw-rw-   0        0        0     6692 2019-12-04 17:43:06.000000 ctextlib-1.0.8/src/CTextA.h
--rw-rw-rw-   0        0        0    50990 2019-12-22 16:34:09.000000 ctextlib-1.0.8/src/CTextT.h
--rw-rw-rw-   0        0        0   166491 2019-12-22 11:06:53.000000 ctextlib-1.0.8/src/CTextT.inl
--rw-rw-rw-   0        0        0     6207 2019-12-04 17:29:41.000000 ctextlib-1.0.8/src/CTextU.h
--rw-rw-rw-   0        0        0     3248 2019-12-22 11:03:16.000000 ctextlib-1.0.8/src/CharTrie.h
--rw-rw-rw-   0        0        0    27069 2019-12-22 16:42:00.000000 ctextlib-1.0.8/src/module.cpp
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/
+-rw-rw-rw-   0        0        0      130 2019-12-19 09:37:24.000000 ctextlib-1.0.9/CMakeLists.txt
+-rw-rw-rw-   0        0        0     2182 2017-08-31 18:59:27.000000 ctextlib-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      127 2017-08-31 18:59:27.000000 ctextlib-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    39660 2020-01-05 13:44:10.000000 ctextlib-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    26517 2019-12-23 02:02:39.000000 ctextlib-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1760 2020-01-05 12:05:12.000000 ctextlib-1.0.9/cmake_install.cmake
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/ctextlib.egg-info/
+-rw-rw-rw-   0        0        0    39660 2020-01-05 13:44:10.000000 ctextlib-1.0.9/ctextlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2020-01-05 13:44:10.000000 ctextlib-1.0.9/ctextlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-01-05 13:44:10.000000 ctextlib-1.0.9/ctextlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-12-23 21:34:06.000000 ctextlib-1.0.9/ctextlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2020-01-05 13:44:10.000000 ctextlib-1.0.9/ctextlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/CMakeFiles/
+-rw-rw-rw-   0        0        0      692 2020-01-05 12:05:12.000000 ctextlib-1.0.9/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-rw-   0        0        0     6507 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1157 2020-01-05 12:05:12.000000 ctextlib-1.0.9/pybind11/cmake_install.cmake
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/include/
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    19063 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     4326 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    89703 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     7701 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      120 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2001 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    25044 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    37278 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     3566 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    16322 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    15073 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0     1450 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-rw-   0        0        0    29043 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0     7731 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     3865 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     3599 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     5655 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    67677 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0     8749 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2031 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0    97575 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0    58356 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/pytypes.h
+-rw-rw-rw-   0        0        0    14029 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    23134 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/include/pybind11/stl_bind.h
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/
+-rw-rw-rw-   0        0        0     9502 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/
+-rw-rw-rw-   0        0        0     2042 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-rw-   0        0        0      686 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-rw-   0        0        0      474 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-rw-   0        0        0     1056 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-rw-   0        0        0      852 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-rw-   0        0        0      373 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-rw-   0        0        0      695 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tests/test_embed/
+-rw-rw-rw-   0        0        0     1527 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tests/test_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/pybind11/tools/
+-rw-rw-rw-   0        0        0     2100 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tools/FindCatch.cmake
+-rw-rw-rw-   0        0        0     2995 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tools/FindEigen3.cmake
+-rw-rw-rw-   0        0        0     8360 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-rw-   0        0        0     9597 2019-10-14 23:57:24.000000 ctextlib-1.0.9/pybind11/tools/pybind11Tools.cmake
+-rw-rw-rw-   0        0        0       42 2020-01-05 13:44:10.000000 ctextlib-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3088 2020-01-05 13:44:07.000000 ctextlib-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-01-05 13:44:10.000000 ctextlib-1.0.9/src/
+-rw-rw-rw-   0        0        0      204 2019-12-03 11:42:17.000000 ctextlib-1.0.9/src/CText.h
+-rw-rw-rw-   0        0        0     6692 2019-12-04 17:43:06.000000 ctextlib-1.0.9/src/CTextA.h
+-rw-rw-rw-   0        0        0    50990 2019-12-22 16:34:09.000000 ctextlib-1.0.9/src/CTextT.h
+-rw-rw-rw-   0        0        0   166491 2019-12-22 11:06:53.000000 ctextlib-1.0.9/src/CTextT.inl
+-rw-rw-rw-   0        0        0     6207 2019-12-04 17:29:41.000000 ctextlib-1.0.9/src/CTextU.h
+-rw-rw-rw-   0        0        0     3248 2019-12-22 11:03:16.000000 ctextlib-1.0.9/src/CharTrie.h
+-rw-rw-rw-   0        0        0    27069 2019-12-22 16:42:00.000000 ctextlib-1.0.9/src/module.cpp
```

### Comparing `ctextlib-1.0.8/LICENSE` & `ctextlib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/PKG-INFO` & `ctextlib-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctextlib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package with CText C++ extension
 Home-page: https://github.com/antonmilev/CText
 Author: Anton Milev
 Author-email: baj.mile@abv.bg
 License: UNKNOWN
 Description: # CText
         # Modern C++ text processing library
```

### Comparing `ctextlib-1.0.8/README.md` & `ctextlib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/ctextlib.egg-info/PKG-INFO` & `ctextlib-1.0.9/ctextlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctextlib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package with CText C++ extension
 Home-page: https://github.com/antonmilev/CText
 Author: Anton Milev
 Author-email: baj.mile@abv.bg
 License: UNKNOWN
 Description: # CText
         # Modern C++ text processing library
```

### Comparing `ctextlib-1.0.8/ctextlib.egg-info/SOURCES.txt` & `ctextlib-1.0.9/ctextlib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
+cmake_install.cmake
 setup.py
 ctextlib.egg-info/PKG-INFO
 ctextlib.egg-info/SOURCES.txt
 ctextlib.egg-info/dependency_links.txt
 ctextlib.egg-info/not-zip-safe
 ctextlib.egg-info/top_level.txt
 pybind11/CMakeLists.txt
+pybind11/cmake_install.cmake
+pybind11/CMakeFiles/CMakeDirectoryInformation.cmake
 pybind11/include/pybind11/attr.h
 pybind11/include/pybind11/buffer_info.h
 pybind11/include/pybind11/cast.h
 pybind11/include/pybind11/chrono.h
 pybind11/include/pybind11/common.h
 pybind11/include/pybind11/complex.h
 pybind11/include/pybind11/eigen.h
```

### Comparing `ctextlib-1.0.8/pybind11/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/attr.h` & `ctextlib-1.0.9/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/buffer_info.h` & `ctextlib-1.0.9/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/cast.h` & `ctextlib-1.0.9/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/chrono.h` & `ctextlib-1.0.9/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/complex.h` & `ctextlib-1.0.9/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/detail/class.h` & `ctextlib-1.0.9/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/detail/common.h` & `ctextlib-1.0.9/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/detail/descr.h` & `ctextlib-1.0.9/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/detail/init.h` & `ctextlib-1.0.9/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/detail/internals.h` & `ctextlib-1.0.9/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/detail/typeid.h` & `ctextlib-1.0.9/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/eigen.h` & `ctextlib-1.0.9/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/embed.h` & `ctextlib-1.0.9/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/eval.h` & `ctextlib-1.0.9/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/functional.h` & `ctextlib-1.0.9/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/iostream.h` & `ctextlib-1.0.9/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/numpy.h` & `ctextlib-1.0.9/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/operators.h` & `ctextlib-1.0.9/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/options.h` & `ctextlib-1.0.9/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/pybind11.h` & `ctextlib-1.0.9/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/pytypes.h` & `ctextlib-1.0.9/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/stl.h` & `ctextlib-1.0.9/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/include/pybind11/stl_bind.h` & `ctextlib-1.0.9/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tests/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tests/test_cmake_build/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tests/test_embed/CMakeLists.txt` & `ctextlib-1.0.9/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tools/FindCatch.cmake` & `ctextlib-1.0.9/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tools/FindEigen3.cmake` & `ctextlib-1.0.9/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tools/FindPythonLibsNew.cmake` & `ctextlib-1.0.9/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/pybind11/tools/pybind11Tools.cmake` & `ctextlib-1.0.9/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/setup.py` & `ctextlib-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=self.build_temp)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='ctextlib',
-    version='1.0.8',
+    version='1.0.9',
     author='Anton Milev',
     author_email='baj.mile@abv.bg',
     description='Python package with CText C++ extension',
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension('cmake_example_median')],
     cmdclass=dict(build_ext=CMakeBuild),
```

### Comparing `ctextlib-1.0.8/src/CTextA.h` & `ctextlib-1.0.9/src/CTextA.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/src/CTextT.h` & `ctextlib-1.0.9/src/CTextT.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/src/CTextT.inl` & `ctextlib-1.0.9/src/CTextT.inl`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/src/CTextU.h` & `ctextlib-1.0.9/src/CTextU.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/src/CharTrie.h` & `ctextlib-1.0.9/src/CharTrie.h`

 * *Files identical despite different names*

### Comparing `ctextlib-1.0.8/src/module.cpp` & `ctextlib-1.0.9/src/module.cpp`

 * *Files identical despite different names*

