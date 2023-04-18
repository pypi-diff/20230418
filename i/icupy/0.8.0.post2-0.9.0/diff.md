# Comparing `tmp/icupy-0.8.0.post2.tar.gz` & `tmp/icupy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icupy-0.8.0.post2.tar", last modified: Thu Sep 16 15:51:35 2021, max compression
+gzip compressed data, was "icupy-0.9.0.tar", last modified: Tue Oct  5 11:57:53 2021, max compression
```

## Comparing `icupy-0.8.0.post2.tar` & `icupy-0.9.0.tar`

### file list

```diff
@@ -1,231 +1,245 @@
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:35.078299 icupy-0.8.0.post2/
--rw-r--r--   0 miute     (1000) miute     (1000)     1070 2021-01-15 02:06:18.000000 icupy-0.8.0.post2/LICENSE
--rw-r--r--   0 miute     (1000) miute     (1000)      324 2021-01-29 11:16:43.000000 icupy-0.8.0.post2/MANIFEST.in
--rw-r--r--   0 miute     (1000) miute     (1000)     3155 2021-09-16 15:51:35.080298 icupy-0.8.0.post2/PKG-INFO
--rwxr--r--   0 miute     (1000) miute     (1000)     2060 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/README.md
--rw-r--r--   0 miute     (1000) miute     (1000)     3492 2021-03-12 13:26:57.000000 icupy-0.8.0.post2/_build.py
--rw-r--r--   0 miute     (1000) miute     (1000)      161 2021-01-29 04:19:44.000000 icupy-0.8.0.post2/pyproject.toml
--rwxr--r--   0 miute     (1000) miute     (1000)     1134 2021-09-16 15:51:35.087298 icupy-0.8.0.post2/setup.cfg
--rw-r--r--   0 miute     (1000) miute     (1000)      540 2021-01-27 01:30:12.000000 icupy-0.8.0.post2/setup.py
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:30.553387 icupy-0.8.0.post2/src/
--rwxr--r--   0 miute     (1000) miute     (1000)     3420 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/CMakeLists.txt
--rw-r--r--   0 miute     (1000) miute     (1000)     1593 2021-05-20 16:11:29.000000 icupy-0.8.0.post2/src/appendable.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1235 2021-08-11 13:39:09.000000 icupy-0.8.0.post2/src/char16ptr.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      331 2020-12-25 03:20:14.000000 icupy-0.8.0.post2/src/char16ptr.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3740 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/coleitr.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     8174 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/compactdecimalformat.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     5997 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/currpinf.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)      867 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/currunit.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    15232 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/datefmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     7577 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/dcfmtsym.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    24258 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/decimfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    14906 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/dtfmtsym.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      777 2021-05-20 16:11:29.000000 icupy-0.8.0.post2/src/dtintrv.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    14287 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/dtitvfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     6088 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/dtitvinf.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    16864 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/dtptngen.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     2988 2021-04-14 14:56:37.000000 icupy-0.8.0.post2/src/dtrule.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)      681 2021-08-11 13:39:09.000000 icupy-0.8.0.post2/src/errorcode.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1554 2021-05-20 16:11:29.000000 icupy-0.8.0.post2/src/fieldpos.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     9141 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/fmtable.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3835 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/format.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3067 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/formattedvalue.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      514 2021-05-20 16:11:29.000000 icupy-0.8.0.post2/src/fpositer.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    20499 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/gregocal.cpp
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:30.620387 icupy-0.8.0.post2/src/icupy/
--rwxr--r--   0 miute     (1000) miute     (1000)      244 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/icupy/__init__.py
--rwxr--r--   0 miute     (1000) miute     (1000)       76 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/src/icupy/number.py
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:30.855520 icupy-0.8.0.post2/src/icupy.egg-info/
--rwxr--r--   0 miute     (1000) miute     (1000)     3155 2021-09-16 15:51:20.000000 icupy-0.8.0.post2/src/icupy.egg-info/PKG-INFO
--rwxr--r--   0 miute     (1000) miute     (1000)     5421 2021-09-16 15:51:26.000000 icupy-0.8.0.post2/src/icupy.egg-info/SOURCES.txt
--rwxr--r--   0 miute     (1000) miute     (1000)        1 2021-09-16 15:51:20.000000 icupy-0.8.0.post2/src/icupy.egg-info/dependency_links.txt
--rw-r--r--   0 miute     (1000) miute     (1000)        1 2021-02-07 08:27:48.000000 icupy-0.8.0.post2/src/icupy.egg-info/not-zip-safe
--rwxr--r--   0 miute     (1000) miute     (1000)        6 2021-09-16 15:51:20.000000 icupy-0.8.0.post2/src/icupy.egg-info/top_level.txt
--rwxr--r--   0 miute     (1000) miute     (1000)     7801 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/idna.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3080 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/localebuilder.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    10050 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/localematcher.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    16304 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/locid.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     9562 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/main.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)      858 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/main.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     8378 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/measfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    64809 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/measunit.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     4054 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/measure.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     2383 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/messagepattern.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    21647 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/msgfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     9217 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/normalizer2.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)      400 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/src/nounit.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    20710 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/numberformatter.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     9673 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/numberrangeformatter.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    18001 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/numfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3421 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/numsys.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1039 2020-12-27 23:51:44.000000 icupy-0.8.0.post2/src/parseerr.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1194 2021-05-20 16:11:29.000000 icupy-0.8.0.post2/src/parsepos.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    17898 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/plurfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     6816 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/plurrule.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    12900 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/rbbi.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    27368 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/rbnf.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    31599 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/regex.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     8808 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/resbund.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     7322 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/src/schriter.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     6360 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/selfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    17063 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/smpdtfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1343 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/sortkey.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3338 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/strenum.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    19064 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/stsearch.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    26276 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/tblcoll.cpp
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:26.701562 icupy-0.8.0.post2/src/third_party/
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:30.984517 icupy-0.8.0.post2/src/third_party/pybind11/
--rw-r--r--   0 miute     (1000) miute     (1000)    10364 2021-01-30 10:53:33.000000 icupy-0.8.0.post2/src/third_party/pybind11/CMakeLists.txt
--rw-r--r--   0 miute     (1000) miute     (1000)     1684 2021-01-30 10:53:33.000000 icupy-0.8.0.post2/src/third_party/pybind11/LICENSE
--rw-r--r--   0 miute     (1000) miute     (1000)     8064 2021-01-30 10:53:33.000000 icupy-0.8.0.post2/src/third_party/pybind11/README.rst
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:26.722561 icupy-0.8.0.post2/src/third_party/pybind11/include/
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:32.167832 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/
--rw-r--r--   0 miute     (1000) miute     (1000)    21412 2021-01-30 10:53:33.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/attr.h
--rw-r--r--   0 miute     (1000) miute     (1000)     6118 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 miute     (1000) miute     (1000)    95557 2021-01-30 11:56:48.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/cast.h
--rw-r--r--   0 miute     (1000) miute     (1000)     8185 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 miute     (1000) miute     (1000)      120 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/common.h
--rw-r--r--   0 miute     (1000) miute     (1000)     2037 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:32.598474 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/
--rw-r--r--   0 miute     (1000) miute     (1000)    27823 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 miute     (1000) miute     (1000)    40452 2021-01-30 11:56:48.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 miute     (1000) miute     (1000)     3602 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 miute     (1000) miute     (1000)    16397 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 miute     (1000) miute     (1000)    16375 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 miute     (1000) miute     (1000)     1486 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 miute     (1000) miute     (1000)    29086 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 miute     (1000) miute     (1000)     7843 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/embed.h
--rw-r--r--   0 miute     (1000) miute     (1000)     5079 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/eval.h
--rw-r--r--   0 miute     (1000) miute     (1000)     3709 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/functional.h
--rw-r--r--   0 miute     (1000) miute     (1000)     6084 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 miute     (1000) miute     (1000)    69310 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 miute     (1000) miute     (1000)     9085 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/operators.h
--rw-r--r--   0 miute     (1000) miute     (1000)     2049 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/options.h
--rw-r--r--   0 miute     (1000) miute     (1000)   111558 2021-01-30 11:56:48.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 miute     (1000) miute     (1000)    66118 2021-01-30 11:56:48.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 miute     (1000) miute     (1000)    14136 2021-01-30 11:56:48.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/stl.h
--rw-r--r--   0 miute     (1000) miute     (1000)    23912 2021-01-30 10:53:34.000000 icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:33.363128 icupy-0.8.0.post2/src/third_party/pybind11/tools/
--rw-r--r--   0 miute     (1000) miute     (1000)     2295 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 miute     (1000) miute     (1000)     3105 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 miute     (1000) miute     (1000)     9977 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 miute     (1000) miute     (1000)     1427 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/check-style.sh
--rw-r--r--   0 miute     (1000) miute     (1000)      952 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 miute     (1000) miute     (1000)     1121 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/libsize.py
--rwxr-xr-x   0 miute     (1000) miute     (1000)     1202 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/make_changelog.py
--rw-r--r--   0 miute     (1000) miute     (1000)    14003 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 miute     (1000) miute     (1000)     7010 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 miute     (1000) miute     (1000)     9172 2021-01-30 10:53:35.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 miute     (1000) miute     (1000)     7276 2021-01-30 10:53:36.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 miute     (1000) miute     (1000)       94 2021-01-30 10:53:36.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/pyproject.toml
--rw-r--r--   0 miute     (1000) miute     (1000)     1822 2021-01-30 10:53:36.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/setup_global.py.in
--rw-r--r--   0 miute     (1000) miute     (1000)      915 2021-01-30 10:53:36.000000 icupy-0.8.0.post2/src/third_party/pybind11/tools/setup_main.py.in
--rwxr--r--   0 miute     (1000) miute     (1000)    50449 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/timezone.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1378 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/tmunit.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    16321 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/translit.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    18681 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/tzfmt.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     7483 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/tznames.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)    12672 2021-04-14 14:56:37.000000 icupy-0.8.0.post2/src/tzrule.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1728 2021-05-20 16:11:29.000000 icupy-0.8.0.post2/src/tztrans.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    18622 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ubidi.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1543 2021-03-12 10:41:35.000000 icupy-0.8.0.post2/src/ubidiptr.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1652 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ubrk.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     6249 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucal.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    59776 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uchar.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    17661 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucnv.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1710 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucnv_cb.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     4361 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucnv_err.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     2000 2021-02-27 02:43:02.000000 icupy-0.8.0.post2/src/ucnv_err.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3532 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucol.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     2418 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucpmap.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      929 2021-02-27 02:43:02.000000 icupy-0.8.0.post2/src/ucpmapptr.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     5533 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucsdet.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      788 2021-03-02 13:58:08.000000 icupy-0.8.0.post2/src/ucsdetptr.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1251 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ucurr.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     8835 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/udat.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     2371 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/udatpg.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1954 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/udisplaycontext.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     4011 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uenum.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      477 2021-03-02 13:58:08.000000 icupy-0.8.0.post2/src/uenumptr.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1004 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uformattedvalue.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     2008 2020-12-13 15:19:24.000000 icupy-0.8.0.post2/src/uidna.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     2359 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uloc.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    20562 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uniset.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    49239 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/unistr.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)      580 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/unorm2.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     9587 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/unum.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     3140 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/unumberformatter.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1676 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/unumberrangeformatter.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)      458 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/upluralrules.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     2155 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uregex.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1597 2021-02-27 02:43:02.000000 icupy-0.8.0.post2/src/uregex.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     2191 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/ures.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      372 2020-12-16 15:59:02.000000 icupy-0.8.0.post2/src/uresptr.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)    15410 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uscript.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1247 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/usearch.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1210 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uset.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      504 2020-12-16 16:02:59.000000 icupy-0.8.0.post2/src/usetptr.hpp
--rw-r--r--   0 miute     (1000) miute     (1000)      485 2021-01-02 14:15:00.000000 icupy-0.8.0.post2/src/ustring.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    11522 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/utext.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      653 2021-03-02 13:58:08.000000 icupy-0.8.0.post2/src/utextptr.hpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1024 2021-02-27 02:43:02.000000 icupy-0.8.0.post2/src/utextvec.hpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1093 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/utrans.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)    19706 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/utypes.cpp
--rwxr--r--   0 miute     (1000) miute     (1000)     1708 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/src/uversion.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)     1263 2021-02-27 02:43:02.000000 icupy-0.8.0.post2/src/voidptr.cpp
--rw-r--r--   0 miute     (1000) miute     (1000)      735 2021-03-02 13:58:08.000000 icupy-0.8.0.post2/src/voidptr.hpp
-drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-09-16 15:51:35.044299 icupy-0.8.0.post2/tests/
--rw-r--r--   0 miute     (1000) miute     (1000)      632 2021-01-23 12:06:52.000000 icupy-0.8.0.post2/tests/__init__.py
--rwxr--r--   0 miute     (1000) miute     (1000)     5298 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_coleitr.py
--rwxr--r--   0 miute     (1000) miute     (1000)     8644 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_compactdecimalformat.py
--rwxr--r--   0 miute     (1000) miute     (1000)     3606 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_currpinf.py
--rwxr--r--   0 miute     (1000) miute     (1000)     1846 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_currunit.py
--rwxr--r--   0 miute     (1000) miute     (1000)    18948 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_datefmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)     9015 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_dcfmtsym.py
--rwxr--r--   0 miute     (1000) miute     (1000)    25091 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_decimfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)    19692 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_dtfmtsym.py
--rwxr--r--   0 miute     (1000) miute     (1000)    18682 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_dtitvfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)    13240 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_dtptngen.py
--rwxr--r--   0 miute     (1000) miute     (1000)    10341 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_fmtable.py
--rwxr--r--   0 miute     (1000) miute     (1000)    18924 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_gregocal.py
--rwxr--r--   0 miute     (1000) miute     (1000)     4602 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_icupy.py
--rwxr--r--   0 miute     (1000) miute     (1000)     4952 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_localebuilder.py
--rwxr--r--   0 miute     (1000) miute     (1000)     7663 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_localematcher.py
--rwxr--r--   0 miute     (1000) miute     (1000)    25430 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_locid.py
--rwxr--r--   0 miute     (1000) miute     (1000)    15078 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_measfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)    52611 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_measunit.py
--rwxr--r--   0 miute     (1000) miute     (1000)    19860 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_msgfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)     8888 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_normalizer2.py
--rwxr--r--   0 miute     (1000) miute     (1000)    23925 2021-09-06 13:38:38.000000 icupy-0.8.0.post2/tests/test_numberformatter.py
--rwxr--r--   0 miute     (1000) miute     (1000)    15232 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_numberrangeformatter.py
--rwxr--r--   0 miute     (1000) miute     (1000)     9710 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_numfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)     9809 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_plurfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)     5829 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_plurrule.py
--rwxr--r--   0 miute     (1000) miute     (1000)    19706 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_rbbi.py
--rwxr--r--   0 miute     (1000) miute     (1000)    22355 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_rbnf.py
--rwxr--r--   0 miute     (1000) miute     (1000)    24478 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_regex_matcher.py
--rwxr--r--   0 miute     (1000) miute     (1000)     9918 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_regex_pattern.py
--rwxr--r--   0 miute     (1000) miute     (1000)    14224 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_resbund.py
--rwxr--r--   0 miute     (1000) miute     (1000)     9700 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_schriter.py
--rwxr--r--   0 miute     (1000) miute     (1000)     5959 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_selfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)    17116 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_smpdtfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)     2430 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_sortkey.py
--rwxr--r--   0 miute     (1000) miute     (1000)     4588 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_strenum.py
--rwxr--r--   0 miute     (1000) miute     (1000)    13884 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_stsearch.py
--rwxr--r--   0 miute     (1000) miute     (1000)    23012 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_tblcoll.py
--rwxr--r--   0 miute     (1000) miute     (1000)    60762 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_timezone.py
--rwxr--r--   0 miute     (1000) miute     (1000)     2018 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_tmunit.py
--rwxr--r--   0 miute     (1000) miute     (1000)    17681 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_translit.py
--rwxr--r--   0 miute     (1000) miute     (1000)    19376 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_tzfmt.py
--rwxr--r--   0 miute     (1000) miute     (1000)     6684 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_tznames.py
--rwxr--r--   0 miute     (1000) miute     (1000)    17600 2021-08-11 13:39:10.000000 icupy-0.8.0.post2/tests/test_tzrule.py
--rw-r--r--   0 miute     (1000) miute     (1000)    19793 2021-03-12 10:41:35.000000 icupy-0.8.0.post2/tests/test_ubidi.py
--rwxr--r--   0 miute     (1000) miute     (1000)    10607 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_uchar.py
--rwxr--r--   0 miute     (1000) miute     (1000)    22073 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_ucnv.py
--rw-r--r--   0 miute     (1000) miute     (1000)     3154 2021-03-02 13:58:08.000000 icupy-0.8.0.post2/tests/test_ucsdet.py
--rw-r--r--   0 miute     (1000) miute     (1000)     2575 2021-03-02 13:58:08.000000 icupy-0.8.0.post2/tests/test_uenum.py
--rwxr--r--   0 miute     (1000) miute     (1000)    26580 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_uniset.py
--rwxr--r--   0 miute     (1000) miute     (1000)    66580 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_unistr.py
--rwxr--r--   0 miute     (1000) miute     (1000)     3604 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_uscript.py
--rwxr--r--   0 miute     (1000) miute     (1000)    14888 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_utext.py
--rwxr--r--   0 miute     (1000) miute     (1000)    31008 2021-09-16 14:01:08.000000 icupy-0.8.0.post2/tests/test_uts46.py
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:53.174609 icupy-0.9.0/
+-rw-r--r--   0 miute     (1000) miute     (1000)     1070 2021-01-15 02:06:18.000000 icupy-0.9.0/LICENSE
+-rw-r--r--   0 miute     (1000) miute     (1000)      324 2021-01-29 11:16:43.000000 icupy-0.9.0/MANIFEST.in
+-rw-r--r--   0 miute     (1000) miute     (1000)     3267 2021-10-05 11:57:53.176609 icupy-0.9.0/PKG-INFO
+-rwxr--r--   0 miute     (1000) miute     (1000)     2202 2021-10-05 10:32:06.000000 icupy-0.9.0/README.md
+-rwxr--r--   0 miute     (1000) miute     (1000)     4262 2021-10-01 05:12:37.000000 icupy-0.9.0/_build.py
+-rw-r--r--   0 miute     (1000) miute     (1000)      161 2021-01-29 04:19:44.000000 icupy-0.9.0/pyproject.toml
+-rwxr--r--   0 miute     (1000) miute     (1000)     1122 2021-10-05 11:57:53.184613 icupy-0.9.0/setup.cfg
+-rw-r--r--   0 miute     (1000) miute     (1000)      540 2021-01-27 01:30:12.000000 icupy-0.9.0/setup.py
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:48.535542 icupy-0.9.0/src/
+-rwxr--r--   0 miute     (1000) miute     (1000)     3491 2021-10-05 10:32:06.000000 icupy-0.9.0/src/CMakeLists.txt
+-rwxr--r--   0 miute     (1000) miute     (1000)    13333 2021-10-05 10:32:06.000000 icupy-0.9.0/src/alphaindex.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     1593 2021-05-20 16:11:29.000000 icupy-0.9.0/src/appendable.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1235 2021-08-11 13:39:09.000000 icupy-0.9.0/src/char16ptr.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      331 2020-12-25 03:20:14.000000 icupy-0.9.0/src/char16ptr.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3740 2021-09-16 14:01:08.000000 icupy-0.9.0/src/coleitr.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     8174 2021-09-16 14:01:08.000000 icupy-0.9.0/src/compactdecimalformat.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     5997 2021-09-16 14:01:08.000000 icupy-0.9.0/src/currpinf.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)      867 2021-09-16 14:01:08.000000 icupy-0.9.0/src/currunit.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    15232 2021-09-16 14:01:08.000000 icupy-0.9.0/src/datefmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     7577 2021-09-16 14:01:08.000000 icupy-0.9.0/src/dcfmtsym.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    24258 2021-09-16 14:01:08.000000 icupy-0.9.0/src/decimfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    15072 2021-10-01 05:12:37.000000 icupy-0.9.0/src/dtfmtsym.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      777 2021-05-20 16:11:29.000000 icupy-0.9.0/src/dtintrv.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    14287 2021-09-16 14:01:08.000000 icupy-0.9.0/src/dtitvfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     6088 2021-09-16 14:01:08.000000 icupy-0.9.0/src/dtitvinf.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    16864 2021-09-16 14:01:08.000000 icupy-0.9.0/src/dtptngen.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     2988 2021-04-14 14:56:37.000000 icupy-0.9.0/src/dtrule.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)      681 2021-08-11 13:39:09.000000 icupy-0.9.0/src/errorcode.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     1554 2021-05-20 16:11:29.000000 icupy-0.9.0/src/fieldpos.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     9230 2021-10-01 05:12:37.000000 icupy-0.9.0/src/fmtable.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3835 2021-09-16 14:01:08.000000 icupy-0.9.0/src/format.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3067 2021-09-16 14:01:08.000000 icupy-0.9.0/src/formattedvalue.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      514 2021-05-20 16:11:29.000000 icupy-0.9.0/src/fpositer.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    20502 2021-10-01 05:12:37.000000 icupy-0.9.0/src/gregocal.cpp
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:48.605544 icupy-0.9.0/src/icupy/
+-rwxr--r--   0 miute     (1000) miute     (1000)      244 2021-09-16 14:01:08.000000 icupy-0.9.0/src/icupy/__init__.py
+-rwxr--r--   0 miute     (1000) miute     (1000)       76 2021-08-11 13:39:10.000000 icupy-0.9.0/src/icupy/number.py
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:48.813287 icupy-0.9.0/src/icupy.egg-info/
+-rwxr--r--   0 miute     (1000) miute     (1000)     3267 2021-10-05 11:57:39.000000 icupy-0.9.0/src/icupy.egg-info/PKG-INFO
+-rwxr--r--   0 miute     (1000) miute     (1000)     5838 2021-10-05 11:57:45.000000 icupy-0.9.0/src/icupy.egg-info/SOURCES.txt
+-rwxr--r--   0 miute     (1000) miute     (1000)        1 2021-10-05 11:57:39.000000 icupy-0.9.0/src/icupy.egg-info/dependency_links.txt
+-rw-r--r--   0 miute     (1000) miute     (1000)        1 2021-02-07 08:27:48.000000 icupy-0.9.0/src/icupy.egg-info/not-zip-safe
+-rwxr--r--   0 miute     (1000) miute     (1000)       15 2021-10-05 11:57:39.000000 icupy-0.9.0/src/icupy.egg-info/requires.txt
+-rwxr--r--   0 miute     (1000) miute     (1000)        6 2021-10-05 11:57:39.000000 icupy-0.9.0/src/icupy.egg-info/top_level.txt
+-rwxr--r--   0 miute     (1000) miute     (1000)     7801 2021-09-16 14:01:08.000000 icupy-0.9.0/src/idna.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     5449 2021-10-01 05:12:37.000000 icupy-0.9.0/src/listformatter.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3080 2021-09-16 14:01:08.000000 icupy-0.9.0/src/localebuilder.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    10050 2021-09-16 14:01:08.000000 icupy-0.9.0/src/localematcher.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    16307 2021-10-01 05:12:37.000000 icupy-0.9.0/src/locid.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     9957 2021-10-05 10:32:06.000000 icupy-0.9.0/src/main.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)      882 2021-10-01 05:12:37.000000 icupy-0.9.0/src/main.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     8378 2021-09-16 14:01:08.000000 icupy-0.9.0/src/measfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    64815 2021-10-01 05:12:37.000000 icupy-0.9.0/src/measunit.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     4097 2021-10-01 05:12:37.000000 icupy-0.9.0/src/measure.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    11173 2021-10-01 05:12:37.000000 icupy-0.9.0/src/messagepattern.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    21668 2021-10-01 05:12:37.000000 icupy-0.9.0/src/msgfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     9217 2021-09-16 14:01:08.000000 icupy-0.9.0/src/normalizer2.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)      400 2021-08-11 13:39:10.000000 icupy-0.9.0/src/nounit.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    20710 2021-09-16 14:01:08.000000 icupy-0.9.0/src/numberformatter.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     9673 2021-09-16 14:01:08.000000 icupy-0.9.0/src/numberrangeformatter.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    18001 2021-09-16 14:01:08.000000 icupy-0.9.0/src/numfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3421 2021-09-16 14:01:08.000000 icupy-0.9.0/src/numsys.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     1039 2020-12-27 23:51:44.000000 icupy-0.9.0/src/parseerr.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     1194 2021-05-20 16:11:29.000000 icupy-0.9.0/src/parsepos.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    17898 2021-09-16 14:01:08.000000 icupy-0.9.0/src/plurfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     6822 2021-10-01 05:12:37.000000 icupy-0.9.0/src/plurrule.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    12906 2021-10-01 05:12:37.000000 icupy-0.9.0/src/rbbi.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    27368 2021-09-16 14:01:08.000000 icupy-0.9.0/src/rbnf.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    31635 2021-10-01 05:12:37.000000 icupy-0.9.0/src/regex.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    16726 2021-10-01 05:12:37.000000 icupy-0.9.0/src/reldatefmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     8808 2021-09-16 14:01:08.000000 icupy-0.9.0/src/resbund.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     7322 2021-08-11 13:39:10.000000 icupy-0.9.0/src/schriter.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     6360 2021-09-16 14:01:08.000000 icupy-0.9.0/src/selfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    17063 2021-09-16 14:01:08.000000 icupy-0.9.0/src/smpdtfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1343 2021-09-16 14:01:08.000000 icupy-0.9.0/src/sortkey.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3350 2021-10-01 05:12:37.000000 icupy-0.9.0/src/strenum.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    19064 2021-09-16 14:01:08.000000 icupy-0.9.0/src/stsearch.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    26297 2021-10-01 05:12:37.000000 icupy-0.9.0/src/tblcoll.cpp
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:45.197193 icupy-0.9.0/src/third_party/
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:48.938287 icupy-0.9.0/src/third_party/pybind11/
+-rw-r--r--   0 miute     (1000) miute     (1000)    10692 2021-09-24 16:06:24.000000 icupy-0.9.0/src/third_party/pybind11/CMakeLists.txt
+-rw-r--r--   0 miute     (1000) miute     (1000)     1684 2021-01-30 10:53:33.000000 icupy-0.9.0/src/third_party/pybind11/LICENSE
+-rw-r--r--   0 miute     (1000) miute     (1000)     7434 2021-09-24 16:06:24.000000 icupy-0.9.0/src/third_party/pybind11/README.rst
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:45.216190 icupy-0.9.0/src/third_party/pybind11/include/
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:50.275068 icupy-0.9.0/src/third_party/pybind11/include/pybind11/
+-rw-r--r--   0 miute     (1000) miute     (1000)    21421 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     6131 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    59150 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     8674 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 miute     (1000) miute     (1000)      120 2021-01-30 10:53:34.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/common.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     2037 2021-01-30 10:53:34.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:50.766070 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/
+-rw-r--r--   0 miute     (1000) miute     (1000)    27889 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    43531 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     3602 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    16641 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    16540 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    40845 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     1486 2021-01-30 10:53:34.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    29039 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     7853 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     5143 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     4369 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     6532 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     8756 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    70192 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     9085 2021-01-30 10:53:34.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 miute     (1000) miute     (1000)     2049 2021-01-30 10:53:34.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/options.h
+-rw-r--r--   0 miute     (1000) miute     (1000)   107484 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    69206 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:50.832060 icupy-0.9.0/src/third_party/pybind11/include/pybind11/stl/
+-rw-r--r--   0 miute     (1000) miute     (1000)     3518 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    14357 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 miute     (1000) miute     (1000)    24027 2021-09-24 16:06:25.000000 icupy-0.9.0/src/third_party/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:51.550989 icupy-0.9.0/src/third_party/pybind11/tools/
+-rw-r--r--   0 miute     (1000) miute     (1000)     2295 2021-01-30 10:53:35.000000 icupy-0.9.0/src/third_party/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 miute     (1000) miute     (1000)     3105 2021-01-30 10:53:35.000000 icupy-0.9.0/src/third_party/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 miute     (1000) miute     (1000)     9977 2021-01-30 10:53:35.000000 icupy-0.9.0/src/third_party/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 miute     (1000) miute     (1000)     1423 2021-09-24 16:06:28.000000 icupy-0.9.0/src/third_party/pybind11/tools/check-style.sh
+-rw-r--r--   0 miute     (1000) miute     (1000)      952 2021-01-30 10:53:35.000000 icupy-0.9.0/src/third_party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 miute     (1000) miute     (1000)     1121 2021-01-30 10:53:35.000000 icupy-0.9.0/src/third_party/pybind11/tools/libsize.py
+-rwxr-xr-x   0 miute     (1000) miute     (1000)     1308 2021-09-24 16:06:28.000000 icupy-0.9.0/src/third_party/pybind11/tools/make_changelog.py
+-rw-r--r--   0 miute     (1000) miute     (1000)    14307 2021-09-24 16:06:28.000000 icupy-0.9.0/src/third_party/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 miute     (1000) miute     (1000)     7041 2021-09-24 16:06:28.000000 icupy-0.9.0/src/third_party/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 miute     (1000) miute     (1000)     9173 2021-09-24 16:06:28.000000 icupy-0.9.0/src/third_party/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 miute     (1000) miute     (1000)     7276 2021-01-30 10:53:36.000000 icupy-0.9.0/src/third_party/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 miute     (1000) miute     (1000)       94 2021-01-30 10:53:36.000000 icupy-0.9.0/src/third_party/pybind11/tools/pyproject.toml
+-rw-r--r--   0 miute     (1000) miute     (1000)     1951 2021-09-24 16:06:28.000000 icupy-0.9.0/src/third_party/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 miute     (1000) miute     (1000)     1089 2021-09-24 16:06:28.000000 icupy-0.9.0/src/third_party/pybind11/tools/setup_main.py.in
+-rwxr--r--   0 miute     (1000) miute     (1000)    50464 2021-10-01 05:12:37.000000 icupy-0.9.0/src/timezone.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1378 2021-09-16 14:01:08.000000 icupy-0.9.0/src/tmunit.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    16321 2021-09-16 14:01:08.000000 icupy-0.9.0/src/translit.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    18681 2021-09-16 14:01:08.000000 icupy-0.9.0/src/tzfmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     7483 2021-09-16 14:01:08.000000 icupy-0.9.0/src/tznames.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)    12672 2021-04-14 14:56:37.000000 icupy-0.9.0/src/tzrule.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1740 2021-10-01 05:12:37.000000 icupy-0.9.0/src/tztrans.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    18622 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ubidi.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     1543 2021-03-12 10:41:35.000000 icupy-0.9.0/src/ubidiptr.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1652 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ubrk.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     6249 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ucal.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    59782 2021-10-01 05:12:37.000000 icupy-0.9.0/src/uchar.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    17670 2021-10-01 05:12:37.000000 icupy-0.9.0/src/ucnv.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1710 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ucnv_cb.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     4361 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ucnv_err.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     2000 2021-02-27 02:43:02.000000 icupy-0.9.0/src/ucnv_err.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3532 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ucol.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     2418 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ucpmap.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      929 2021-02-27 02:43:02.000000 icupy-0.9.0/src/ucpmapptr.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     5539 2021-10-01 05:12:37.000000 icupy-0.9.0/src/ucsdet.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      788 2021-03-02 13:58:08.000000 icupy-0.9.0/src/ucsdetptr.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1251 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ucurr.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     8835 2021-09-16 14:01:08.000000 icupy-0.9.0/src/udat.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     2371 2021-09-16 14:01:08.000000 icupy-0.9.0/src/udatpg.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1954 2021-09-16 14:01:08.000000 icupy-0.9.0/src/udisplaycontext.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     4077 2021-10-01 05:12:37.000000 icupy-0.9.0/src/uenum.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      477 2021-03-02 13:58:08.000000 icupy-0.9.0/src/uenumptr.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1004 2021-09-16 14:01:08.000000 icupy-0.9.0/src/uformattedvalue.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     2008 2020-12-13 15:19:24.000000 icupy-0.9.0/src/uidna.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1103 2021-10-01 05:12:37.000000 icupy-0.9.0/src/ulistformatter.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     2359 2021-09-16 14:01:08.000000 icupy-0.9.0/src/uloc.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    20565 2021-10-01 05:12:37.000000 icupy-0.9.0/src/uniset.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    49254 2021-10-01 05:12:37.000000 icupy-0.9.0/src/unistr.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)      580 2021-09-16 14:01:08.000000 icupy-0.9.0/src/unorm2.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     9587 2021-09-16 14:01:08.000000 icupy-0.9.0/src/unum.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     3140 2021-09-16 14:01:08.000000 icupy-0.9.0/src/unumberformatter.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1676 2021-09-16 14:01:08.000000 icupy-0.9.0/src/unumberrangeformatter.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)      458 2021-09-16 14:01:08.000000 icupy-0.9.0/src/upluralrules.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     2155 2021-09-16 14:01:08.000000 icupy-0.9.0/src/uregex.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     1597 2021-02-27 02:43:02.000000 icupy-0.9.0/src/uregex.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     4430 2021-10-01 05:12:37.000000 icupy-0.9.0/src/ureldatefmt.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     2191 2021-09-16 14:01:08.000000 icupy-0.9.0/src/ures.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      372 2020-12-16 15:59:02.000000 icupy-0.9.0/src/uresptr.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    15419 2021-10-01 05:12:37.000000 icupy-0.9.0/src/uscript.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1247 2021-09-16 14:01:08.000000 icupy-0.9.0/src/usearch.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1210 2021-09-16 14:01:08.000000 icupy-0.9.0/src/uset.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      504 2020-12-16 16:02:59.000000 icupy-0.9.0/src/usetptr.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)      488 2021-10-01 05:12:37.000000 icupy-0.9.0/src/ustring.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    11534 2021-10-01 05:12:37.000000 icupy-0.9.0/src/utext.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      653 2021-03-02 13:58:08.000000 icupy-0.9.0/src/utextptr.hpp
+-rw-r--r--   0 miute     (1000) miute     (1000)     1024 2021-02-27 02:43:02.000000 icupy-0.9.0/src/utextvec.hpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1093 2021-09-16 14:01:08.000000 icupy-0.9.0/src/utrans.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)    19706 2021-09-16 14:01:08.000000 icupy-0.9.0/src/utypes.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1708 2021-09-16 14:01:08.000000 icupy-0.9.0/src/uversion.cpp
+-rwxr--r--   0 miute     (1000) miute     (1000)     1318 2021-10-05 10:32:06.000000 icupy-0.9.0/src/voidptr.cpp
+-rw-r--r--   0 miute     (1000) miute     (1000)      735 2021-03-02 13:58:08.000000 icupy-0.9.0/src/voidptr.hpp
+drwxr-xr-x   0 miute     (1000) miute     (1000)        0 2021-10-05 11:57:53.141610 icupy-0.9.0/tests/
+-rw-r--r--   0 miute     (1000) miute     (1000)      632 2021-01-23 12:06:52.000000 icupy-0.9.0/tests/__init__.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    10754 2021-10-05 10:32:06.000000 icupy-0.9.0/tests/test_alphaindex.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     5298 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_coleitr.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     8644 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_compactdecimalformat.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     3606 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_currpinf.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     1846 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_currunit.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    18948 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_datefmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     9015 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_dcfmtsym.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    25091 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_decimfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    19692 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_dtfmtsym.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    18682 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_dtitvfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    13240 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_dtptngen.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    10341 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_fmtable.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    18924 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_gregocal.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     4602 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_icupy.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     6607 2021-10-01 05:12:38.000000 icupy-0.9.0/tests/test_listformatter.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     4952 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_localebuilder.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     7663 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_localematcher.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    25430 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_locid.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    15078 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_measfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    52611 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_measunit.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    11578 2021-10-01 05:12:38.000000 icupy-0.9.0/tests/test_messagepattern.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    19860 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_msgfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     8888 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_normalizer2.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    23925 2021-09-06 13:38:38.000000 icupy-0.9.0/tests/test_numberformatter.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    15232 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_numberrangeformatter.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     9710 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_numfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     9809 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_plurfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     5829 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_plurrule.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    19747 2021-10-01 05:12:38.000000 icupy-0.9.0/tests/test_rbbi.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    22355 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_rbnf.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    24478 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_regex_matcher.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     9918 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_regex_pattern.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    13886 2021-10-01 05:12:38.000000 icupy-0.9.0/tests/test_reldatefmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    14224 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_resbund.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     9700 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_schriter.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     5959 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_selfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    17116 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_smpdtfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     2430 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_sortkey.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     4588 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_strenum.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    13884 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_stsearch.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    23012 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_tblcoll.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    60762 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_timezone.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     2018 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_tmunit.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    17681 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_translit.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    19376 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_tzfmt.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     6684 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_tznames.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    17600 2021-08-11 13:39:10.000000 icupy-0.9.0/tests/test_tzrule.py
+-rw-r--r--   0 miute     (1000) miute     (1000)    19793 2021-03-12 10:41:35.000000 icupy-0.9.0/tests/test_ubidi.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    10607 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_uchar.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    22073 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_ucnv.py
+-rw-r--r--   0 miute     (1000) miute     (1000)     3154 2021-03-02 13:58:08.000000 icupy-0.9.0/tests/test_ucsdet.py
+-rw-r--r--   0 miute     (1000) miute     (1000)     2575 2021-09-23 06:22:12.000000 icupy-0.9.0/tests/test_uenum.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    26580 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_uniset.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    66580 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_unistr.py
+-rwxr--r--   0 miute     (1000) miute     (1000)     3604 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_uscript.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    14888 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_utext.py
+-rwxr--r--   0 miute     (1000) miute     (1000)    31008 2021-09-16 14:01:08.000000 icupy-0.9.0/tests/test_uts46.py
```

### Comparing `icupy-0.8.0.post2/LICENSE` & `icupy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/PKG-INFO` & `icupy-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: icupy
-Version: 0.8.0.post2
+Version: 0.9.0
 Summary: Python bindings for ICU4C
 Home-page: https://github.com/miute/icupy
 Author: Tetsuya Miura
 Author-email: miute.dev@gmail.com
 License: MIT
-Download-URL: https://github.com/miute/icupy
 Keywords: icu4c,binding
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Localization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # icupy
 
 Python bindings for [ICU4C](https://unicode-org.github.io/icu/userguide/icu4c/).
 
 ## Installation
@@ -50,16 +50,22 @@
     ```bash
     pip install icupy
     ```
 
     Alternatively, installing from the git repository:
 
     ```bash
-    git clone --recursive https://github.com/miute/icupy.git
-    pip install ./icupy
+    pip install git+https://github.com/miute/icupy.git
+    ```
+   
+    Optionally, the CMake environment variables are available.
+    e.g., Using the Ninja build system:
+
+    ```bash
+    CMAKE_GENERATOR=Ninja pip install icupy
     ```
 
 ## Changes
 
 - **Naming Rules**
   - Renamed C functions and C++ class methods from mixed case to snake case. (e.g., `findAndReplace()` → `find_and_replace()`)
   - Renamed C++ enumerators to upper snake case without "k" prefix. (e.g., `kDateOffset` → `DATE_OFFSET`)
```

### Comparing `icupy-0.8.0.post2/README.md` & `icupy-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,22 @@
     ```bash
     pip install icupy
     ```
 
     Alternatively, installing from the git repository:
 
     ```bash
-    git clone --recursive https://github.com/miute/icupy.git
-    pip install ./icupy
+    pip install git+https://github.com/miute/icupy.git
+    ```
+   
+    Optionally, the CMake environment variables are available.
+    e.g., Using the Ninja build system:
+
+    ```bash
+    CMAKE_GENERATOR=Ninja pip install icupy
     ```
 
 ## Changes
 
 - **Naming Rules**
   - Renamed C functions and C++ class methods from mixed case to snake case. (e.g., `findAndReplace()` → `find_and_replace()`)
   - Renamed C++ enumerators to upper snake case without "k" prefix. (e.g., `kDateOffset` → `DATE_OFFSET`)
```

### Comparing `icupy-0.8.0.post2/setup.cfg` & `icupy-0.9.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [metadata]
 name = icupy
-version = 0.8.0.post2
+version = 0.9.0
 description = Python bindings for ICU4C
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Tetsuya Miura
 author_email = miute.dev@gmail.com
 url = https://github.com/miute/icupy
-download_url = https://github.com/miute/icupy
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
@@ -37,11 +36,14 @@
 zip_safe = False
 install_requires = 
 python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
+[options.extras_require]
+test = pytest
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `icupy-0.8.0.post2/setup.py` & `icupy-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/CMakeLists.txt` & `icupy-0.9.0/src/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 add_subdirectory(third_party/pybind11)
 
 find_package(ICU REQUIRED COMPONENTS dt i18n io uc)
 
 pybind11_add_module(
     ${PROJECT_NAME}
+    alphaindex.cpp
     appendable.cpp
     char16ptr.cpp
     coleitr.cpp
     compactdecimalformat.cpp
     currpinf.cpp
     currunit.cpp
     datefmt.cpp
@@ -31,14 +32,15 @@
     fieldpos.cpp
     fmtable.cpp
     format.cpp
     formattedvalue.cpp
     fpositer.cpp
     gregocal.cpp
     idna.cpp
+    listformatter.cpp
     localebuilder.cpp
     localematcher.cpp
     locid.cpp
     main.cpp
     measfmt.cpp
     measunit.cpp
     measure.cpp
@@ -53,14 +55,15 @@
     parseerr.cpp
     parsepos.cpp
     plurfmt.cpp
     plurrule.cpp
     rbbi.cpp
     rbnf.cpp
     regex.cpp
+    reldatefmt.cpp
     resbund.cpp
     schriter.cpp
     selfmt.cpp
     smpdtfmt.cpp
     sortkey.cpp
     strenum.cpp
     stsearch.cpp
@@ -85,23 +88,25 @@
     ucurr.cpp
     udat.cpp
     udatpg.cpp
     udisplaycontext.cpp
     uenum.cpp
     uformattedvalue.cpp
     uidna.cpp
+    ulistformatter.cpp
     uloc.cpp
     uniset.cpp
     unistr.cpp
     unorm2.cpp
     unum.cpp
     unumberformatter.cpp
     unumberrangeformatter.cpp
     upluralrules.cpp
     uregex.cpp
+    ureldatefmt.cpp
     ures.cpp
     uscript.cpp
     usearch.cpp
     uset.cpp
     ustring.cpp
     utext.cpp
     utrans.cpp
@@ -157,15 +162,14 @@
     PRIVATE
     ICU::i18n
     ICU::io
     ICU::uc
 )
 
 pybind11_extension(${PROJECT_NAME})
-pybind11_strip(${PROJECT_NAME})
 
 install(
     TARGETS
     ${PROJECT_NAME}
     LIBRARY
     DESTINATION ${DESTDIR}
 )
```

### Comparing `icupy-0.8.0.post2/src/appendable.cpp` & `icupy-0.9.0/src/appendable.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/char16ptr.cpp` & `icupy-0.9.0/src/char16ptr.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/coleitr.cpp` & `icupy-0.9.0/src/coleitr.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/compactdecimalformat.cpp` & `icupy-0.9.0/src/compactdecimalformat.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/currpinf.cpp` & `icupy-0.9.0/src/currpinf.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/currunit.cpp` & `icupy-0.9.0/src/currunit.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/datefmt.cpp` & `icupy-0.9.0/src/datefmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/dcfmtsym.cpp` & `icupy-0.9.0/src/dcfmtsym.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/decimfmt.cpp` & `icupy-0.9.0/src/decimfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/dtfmtsym.cpp` & `icupy-0.9.0/src/dtfmtsym.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #include "main.hpp"
-#include <optional>
 #include <pybind11/operators.h>
 #include <pybind11/stl.h>
 #include <unicode/dtfmtsym.h>
 
 using namespace icu;
 
 void init_dtfmtsym(py::module &m) {
@@ -225,98 +224,122 @@
         }
         return result;
       },
       py::return_value_policy::reference, py::arg("context"), py::arg("width"));
 #endif // (U_ICU_VERSION_MAJOR_NUM >= 54)
   dfs.def(
       "set_am_pm_strings",
-      [](DateFormatSymbols &self, const std::list<UnicodeString> &ampms, std::optional<int32_t> count) {
+      [](DateFormatSymbols &self, const std::list<UnicodeString> &ampms, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)ampms.size();
+        }
         std::vector<UnicodeString> _ampms(std::begin(ampms), std::end(ampms));
-        self.setAmPmStrings(_ampms.data(), count.value_or((int32_t)ampms.size()));
+        self.setAmPmStrings(_ampms.data(), count);
       },
-      py::arg("ampms"), py::arg("count") = std::nullopt);
+      py::arg("ampms"), py::arg("count") = -1);
   dfs.def(
       "set_era_names",
-      [](DateFormatSymbols &self, const std::list<UnicodeString> &era_names, std::optional<int32_t> count) {
+      [](DateFormatSymbols &self, const std::list<UnicodeString> &era_names, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)era_names.size();
+        }
         std::vector<UnicodeString> _era_names(std::begin(era_names), std::end(era_names));
-        self.setEraNames(_era_names.data(), count.value_or((int32_t)era_names.size()));
+        self.setEraNames(_era_names.data(), count);
       },
-      py::arg("era_names"), py::arg("count") = std::nullopt);
+      py::arg("era_names"), py::arg("count") = -1);
   dfs.def(
       "set_eras",
-      [](DateFormatSymbols &self, const std::list<UnicodeString> &eras, std::optional<int32_t> count) {
+      [](DateFormatSymbols &self, const std::list<UnicodeString> &eras, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)eras.size();
+        }
         std::vector<UnicodeString> _eras(std::begin(eras), std::end(eras));
-        self.setEras(_eras.data(), count.value_or((int32_t)eras.size()));
+        self.setEras(_eras.data(), count);
       },
-      py::arg("eras"), py::arg("count") = std::nullopt);
+      py::arg("eras"), py::arg("count") = -1);
   dfs.def("set_local_pattern_chars", &DateFormatSymbols::setLocalPatternChars, py::arg("new_local_pattern_chars"))
       .def(
           // const char16_t *new_local_pattern_chars -> const UnicodeString &new_local_pattern_chars
           "set_local_pattern_chars",
           [](DateFormatSymbols &self, const char16_t *new_local_pattern_chars) {
             self.setLocalPatternChars(new_local_pattern_chars);
           },
           py::arg("new_local_pattern_chars"));
   dfs.def(
          "set_months",
-         [](DateFormatSymbols &self, const std::list<UnicodeString> &months, std::optional<int32_t> count) {
+         [](DateFormatSymbols &self, const std::list<UnicodeString> &months, int32_t count) {
+           if (count == -1) {
+             count = (int32_t)months.size();
+           }
            std::vector<UnicodeString> _months(std::begin(months), std::end(months));
-           self.setMonths(_months.data(), count.value_or((int32_t)months.size()));
+           self.setMonths(_months.data(), count);
          },
-         py::arg("months"), py::arg("count") = std::nullopt)
+         py::arg("months"), py::arg("count") = -1)
       .def(
           "set_months",
           [](DateFormatSymbols &self, const std::list<UnicodeString> &months, int32_t count,
              DateFormatSymbols::DtContextType context, DateFormatSymbols::DtWidthType width) {
             std::vector<UnicodeString> _months(std::begin(months), std::end(months));
             if (count == -1) {
               count = (int32_t)months.size();
             }
             self.setMonths(_months.data(), count, context, width);
           },
           py::arg("months"), py::arg("count"), py::arg("context"), py::arg("width"));
   dfs.def(
       "set_narrow_eras",
-      [](DateFormatSymbols &self, const std::list<UnicodeString> &narrow_eras, std::optional<int32_t> count) {
+      [](DateFormatSymbols &self, const std::list<UnicodeString> &narrow_eras, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)narrow_eras.size();
+        }
         std::vector<UnicodeString> _narrow_eras(std::begin(narrow_eras), std::end(narrow_eras));
-        self.setNarrowEras(_narrow_eras.data(), count.value_or((int32_t)narrow_eras.size()));
+        self.setNarrowEras(_narrow_eras.data(), count);
       },
-      py::arg("narrow_eras"), py::arg("count") = std::nullopt);
+      py::arg("narrow_eras"), py::arg("count") = -1);
   dfs.def(
       "set_quarters",
       [](DateFormatSymbols &self, const std::list<UnicodeString> &quarters, int32_t count,
          DateFormatSymbols::DtContextType context, DateFormatSymbols::DtWidthType width) {
         std::vector<UnicodeString> _quarters(std::begin(quarters), std::end(quarters));
         if (count == -1) {
           count = (int32_t)quarters.size();
         }
         self.setQuarters(_quarters.data(), count, context, width);
       },
       py::arg("quarters"), py::arg("count"), py::arg("context"), py::arg("width"));
   dfs.def(
       "set_short_months",
-      [](DateFormatSymbols &self, const std::list<UnicodeString> &short_months, std::optional<int32_t> count) {
+      [](DateFormatSymbols &self, const std::list<UnicodeString> &short_months, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)short_months.size();
+        }
         std::vector<UnicodeString> _short_months(std::begin(short_months), std::end(short_months));
-        self.setShortMonths(_short_months.data(), count.value_or((int32_t)short_months.size()));
+        self.setShortMonths(_short_months.data(), count);
       },
-      py::arg("short_months"), py::arg("count") = std::nullopt);
+      py::arg("short_months"), py::arg("count") = -1);
   dfs.def(
       "set_short_weekdays",
-      [](DateFormatSymbols &self, const std::list<UnicodeString> &abbrev_weekdays, std::optional<int32_t> count) {
+      [](DateFormatSymbols &self, const std::list<UnicodeString> &abbrev_weekdays, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)abbrev_weekdays.size();
+        }
         std::vector<UnicodeString> _abbrev_weekdays(std::begin(abbrev_weekdays), std::end(abbrev_weekdays));
-        self.setShortWeekdays(_abbrev_weekdays.data(), count.value_or((int32_t)abbrev_weekdays.size()));
+        self.setShortWeekdays(_abbrev_weekdays.data(), count);
       },
-      py::arg("abbrev_weekdays"), py::arg("count") = std::nullopt);
+      py::arg("abbrev_weekdays"), py::arg("count") = -1);
   dfs.def(
          "set_weekdays",
-         [](DateFormatSymbols &self, const std::list<UnicodeString> &weekdays, std::optional<int32_t> count) {
+         [](DateFormatSymbols &self, const std::list<UnicodeString> &weekdays, int32_t count) {
+           if (count == -1) {
+             count = (int32_t)weekdays.size();
+           }
            std::vector<UnicodeString> _weekdays(std::begin(weekdays), std::end(weekdays));
-           self.setWeekdays(_weekdays.data(), count.value_or((int32_t)weekdays.size()));
+           self.setWeekdays(_weekdays.data(), count);
          },
-         py::arg("weekdays"), py::arg("count") = std::nullopt)
+         py::arg("weekdays"), py::arg("count") = -1)
       .def(
           "set_weekdays",
           [](DateFormatSymbols &self, const std::list<UnicodeString> &weekdays, int32_t count,
              DateFormatSymbols::DtContextType context, DateFormatSymbols::DtWidthType width) {
             std::vector<UnicodeString> _weekdays(std::begin(weekdays), std::end(weekdays));
             if (count == -1) {
               count = (int32_t)weekdays.size();
```

### Comparing `icupy-0.8.0.post2/src/dtintrv.cpp` & `icupy-0.9.0/src/dtintrv.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/dtitvfmt.cpp` & `icupy-0.9.0/src/dtitvfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/dtitvinf.cpp` & `icupy-0.9.0/src/dtitvinf.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/dtptngen.cpp` & `icupy-0.9.0/src/dtptngen.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/dtrule.cpp` & `icupy-0.9.0/src/dtrule.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/errorcode.cpp` & `icupy-0.9.0/src/errorcode.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/fieldpos.cpp` & `icupy-0.9.0/src/fieldpos.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/fmtable.cpp` & `icupy-0.9.0/src/fmtable.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #include "main.hpp"
-#include <optional>
 #include <pybind11/operators.h>
 #include <pybind11/stl.h>
 #include <unicode/basictz.h>
 #include <unicode/calendar.h>
 #include <unicode/curramt.h>
 #include <unicode/dtintrv.h>
 #include <unicode/fmtable.h>
@@ -41,32 +40,35 @@
               throw ICUError(error_code);
             }
             return result;
           }),
           py::arg("number"))
       .def(py::init<const UnicodeString &>(), py::arg("str_to_copy"))
       .def(py::init<const Formattable &>(), py::arg("source"))
-      .def(py::init([](const std::vector<Formattable> &array_to_copy, std::optional<int32_t> count) {
-             return std::make_unique<Formattable>(array_to_copy.data(), count.value_or((int32_t)array_to_copy.size()));
+      .def(py::init([](const std::vector<Formattable> &array_to_copy, int32_t count) {
+             if (count == -1) {
+               count = (int32_t)array_to_copy.size();
+             }
+             return std::make_unique<Formattable>(array_to_copy.data(), count);
            }),
-           py::arg("array_to_copy"), py::arg("count") = std::nullopt)
+           py::arg("array_to_copy"), py::arg("count") = -1)
       // FIXME: Implement "icu::Formattable::Formattable(UObject *objectToAdopt)".
       .def(py::init(
-               [](const Calendar &object_to_adopt) { return std::make_unique<Formattable>(object_to_adopt.clone()); }),
-           py::arg("object_to_adopt"))
-      .def(py::init([](const DateInterval &object_to_adopt) {
-             return std::make_unique<Formattable>(object_to_adopt.clone());
+               [](const Calendar *object_to_adopt) { return std::make_unique<Formattable>(object_to_adopt->clone()); }),
+           py::arg("object_to_adopt").none(false))
+      .def(py::init([](const DateInterval *object_to_adopt) {
+             return std::make_unique<Formattable>(object_to_adopt->clone());
            }),
-           py::arg("object_to_adopt"))
+           py::arg("object_to_adopt").none(false))
       .def(py::init(
-               [](const Measure &object_to_adopt) { return std::make_unique<Formattable>(object_to_adopt.clone()); }),
-           py::arg("object_to_adopt"))
+               [](const Measure *object_to_adopt) { return std::make_unique<Formattable>(object_to_adopt->clone()); }),
+           py::arg("object_to_adopt").none(false))
       .def(py::init(
-               [](const TimeZone &object_to_adopt) { return std::make_unique<Formattable>(object_to_adopt.clone()); }),
-           py::arg("object_to_adopt"))
+               [](const TimeZone *object_to_adopt) { return std::make_unique<Formattable>(object_to_adopt->clone()); }),
+           py::arg("object_to_adopt").none(false))
       .def(py::self != py::self, py::arg("other"))
       .def(py::self == py::self, py::arg("other"));
   fmt.def("__copy__", &Formattable::clone)
       .def(
           "__deepcopy__", [](const Formattable &self, py::dict) { return self.clone(); }, py::arg("memo"))
       .def(
           "__getitem__",
@@ -200,18 +202,21 @@
             return value;
           },
           py::arg("result"));
   fmt.def("get_type", &Formattable::getType);
   fmt.def("is_numeric", &Formattable::isNumeric);
   fmt.def(
       "set_array",
-      [](Formattable &self, const std::vector<Formattable> &array, std::optional<int32_t> count) {
-        self.setArray(array.data(), count.value_or((int32_t)array.size()));
+      [](Formattable &self, const std::vector<Formattable> &array, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)array.size();
+        }
+        self.setArray(array.data(), count);
       },
-      py::arg("array"), py::arg("count") = std::nullopt);
+      py::arg("array"), py::arg("count") = -1);
   fmt.def("set_date", &Formattable::setDate, py::arg("d"));
   fmt.def(
       "set_decimal_number",
       [](Formattable &self, const char *number_string) {
         UErrorCode error_code = U_ZERO_ERROR;
         self.setDecimalNumber(number_string, error_code);
         if (U_FAILURE(error_code)) {
```

### Comparing `icupy-0.8.0.post2/src/format.cpp` & `icupy-0.9.0/src/format.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/formattedvalue.cpp` & `icupy-0.9.0/src/formattedvalue.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/fpositer.cpp` & `icupy-0.9.0/src/fpositer.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/gregocal.cpp` & `icupy-0.9.0/src/gregocal.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
           throw ICUError(error_code);
         }
       },
       py::arg("field"), py::arg("amount"));
   // FIXME: Implement "void icu::Calendar::adoptTimeZone(TimeZone *value)".
   /*
   cal.def(
-      "adopt_time_zone", [](Calendar &self, TimeZone *value) { self.adoptTimeZone(value ? value->clone() : NULL); },
+      "adopt_time_zone", [](Calendar &self, TimeZone *value) { self.adoptTimeZone(value ? value->clone() : nullptr); },
       py::arg("value"));
   */
   cal.def(
       "after",
       [](const Calendar &self, const Calendar &when) {
         UErrorCode error_code = U_ZERO_ERROR;
         auto result = self.after(when, error_code);
```

### Comparing `icupy-0.8.0.post2/src/icupy.egg-info/PKG-INFO` & `icupy-0.9.0/src/icupy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: icupy
-Version: 0.8.0.post2
+Version: 0.9.0
 Summary: Python bindings for ICU4C
 Home-page: https://github.com/miute/icupy
 Author: Tetsuya Miura
 Author-email: miute.dev@gmail.com
 License: MIT
-Download-URL: https://github.com/miute/icupy
 Keywords: icu4c,binding
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Localization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # icupy
 
 Python bindings for [ICU4C](https://unicode-org.github.io/icu/userguide/icu4c/).
 
 ## Installation
@@ -50,16 +50,22 @@
     ```bash
     pip install icupy
     ```
 
     Alternatively, installing from the git repository:
 
     ```bash
-    git clone --recursive https://github.com/miute/icupy.git
-    pip install ./icupy
+    pip install git+https://github.com/miute/icupy.git
+    ```
+   
+    Optionally, the CMake environment variables are available.
+    e.g., Using the Ninja build system:
+
+    ```bash
+    CMAKE_GENERATOR=Ninja pip install icupy
     ```
 
 ## Changes
 
 - **Naming Rules**
   - Renamed C functions and C++ class methods from mixed case to snake case. (e.g., `findAndReplace()` → `find_and_replace()`)
   - Renamed C++ enumerators to upper snake case without "k" prefix. (e.g., `kDateOffset` → `DATE_OFFSET`)
```

### Comparing `icupy-0.8.0.post2/src/icupy.egg-info/SOURCES.txt` & `icupy-0.9.0/src/icupy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 _build.py
 pyproject.toml
 setup.cfg
 setup.py
 src/CMakeLists.txt
+src/alphaindex.cpp
 src/appendable.cpp
 src/char16ptr.cpp
 src/char16ptr.hpp
 src/coleitr.cpp
 src/compactdecimalformat.cpp
 src/currpinf.cpp
 src/currunit.cpp
@@ -26,14 +27,15 @@
 src/fieldpos.cpp
 src/fmtable.cpp
 src/format.cpp
 src/formattedvalue.cpp
 src/fpositer.cpp
 src/gregocal.cpp
 src/idna.cpp
+src/listformatter.cpp
 src/localebuilder.cpp
 src/localematcher.cpp
 src/locid.cpp
 src/main.cpp
 src/main.hpp
 src/measfmt.cpp
 src/measunit.cpp
@@ -49,14 +51,15 @@
 src/parseerr.cpp
 src/parsepos.cpp
 src/plurfmt.cpp
 src/plurrule.cpp
 src/rbbi.cpp
 src/rbnf.cpp
 src/regex.cpp
+src/reldatefmt.cpp
 src/resbund.cpp
 src/schriter.cpp
 src/selfmt.cpp
 src/smpdtfmt.cpp
 src/sortkey.cpp
 src/strenum.cpp
 src/stsearch.cpp
@@ -86,24 +89,26 @@
 src/udat.cpp
 src/udatpg.cpp
 src/udisplaycontext.cpp
 src/uenum.cpp
 src/uenumptr.hpp
 src/uformattedvalue.cpp
 src/uidna.cpp
+src/ulistformatter.cpp
 src/uloc.cpp
 src/uniset.cpp
 src/unistr.cpp
 src/unorm2.cpp
 src/unum.cpp
 src/unumberformatter.cpp
 src/unumberrangeformatter.cpp
 src/upluralrules.cpp
 src/uregex.cpp
 src/uregex.hpp
+src/ureldatefmt.cpp
 src/ures.cpp
 src/uresptr.hpp
 src/uscript.cpp
 src/usearch.cpp
 src/uset.cpp
 src/usetptr.hpp
 src/ustring.cpp
@@ -117,42 +122,46 @@
 src/voidptr.hpp
 src/icupy/__init__.py
 src/icupy/number.py
 src/icupy.egg-info/PKG-INFO
 src/icupy.egg-info/SOURCES.txt
 src/icupy.egg-info/dependency_links.txt
 src/icupy.egg-info/not-zip-safe
+src/icupy.egg-info/requires.txt
 src/icupy.egg-info/top_level.txt
 src/third_party/pybind11/CMakeLists.txt
 src/third_party/pybind11/LICENSE
 src/third_party/pybind11/README.rst
 src/third_party/pybind11/include/pybind11/attr.h
 src/third_party/pybind11/include/pybind11/buffer_info.h
 src/third_party/pybind11/include/pybind11/cast.h
 src/third_party/pybind11/include/pybind11/chrono.h
 src/third_party/pybind11/include/pybind11/common.h
 src/third_party/pybind11/include/pybind11/complex.h
 src/third_party/pybind11/include/pybind11/eigen.h
 src/third_party/pybind11/include/pybind11/embed.h
 src/third_party/pybind11/include/pybind11/eval.h
 src/third_party/pybind11/include/pybind11/functional.h
+src/third_party/pybind11/include/pybind11/gil.h
 src/third_party/pybind11/include/pybind11/iostream.h
 src/third_party/pybind11/include/pybind11/numpy.h
 src/third_party/pybind11/include/pybind11/operators.h
 src/third_party/pybind11/include/pybind11/options.h
 src/third_party/pybind11/include/pybind11/pybind11.h
 src/third_party/pybind11/include/pybind11/pytypes.h
 src/third_party/pybind11/include/pybind11/stl.h
 src/third_party/pybind11/include/pybind11/stl_bind.h
 src/third_party/pybind11/include/pybind11/detail/class.h
 src/third_party/pybind11/include/pybind11/detail/common.h
 src/third_party/pybind11/include/pybind11/detail/descr.h
 src/third_party/pybind11/include/pybind11/detail/init.h
 src/third_party/pybind11/include/pybind11/detail/internals.h
+src/third_party/pybind11/include/pybind11/detail/type_caster_base.h
 src/third_party/pybind11/include/pybind11/detail/typeid.h
+src/third_party/pybind11/include/pybind11/stl/filesystem.h
 src/third_party/pybind11/tools/FindCatch.cmake
 src/third_party/pybind11/tools/FindEigen3.cmake
 src/third_party/pybind11/tools/FindPythonLibsNew.cmake
 src/third_party/pybind11/tools/check-style.sh
 src/third_party/pybind11/tools/cmake_uninstall.cmake.in
 src/third_party/pybind11/tools/libsize.py
 src/third_party/pybind11/tools/make_changelog.py
@@ -160,43 +169,47 @@
 src/third_party/pybind11/tools/pybind11Config.cmake.in
 src/third_party/pybind11/tools/pybind11NewTools.cmake
 src/third_party/pybind11/tools/pybind11Tools.cmake
 src/third_party/pybind11/tools/pyproject.toml
 src/third_party/pybind11/tools/setup_global.py.in
 src/third_party/pybind11/tools/setup_main.py.in
 tests/__init__.py
+tests/test_alphaindex.py
 tests/test_coleitr.py
 tests/test_compactdecimalformat.py
 tests/test_currpinf.py
 tests/test_currunit.py
 tests/test_datefmt.py
 tests/test_dcfmtsym.py
 tests/test_decimfmt.py
 tests/test_dtfmtsym.py
 tests/test_dtitvfmt.py
 tests/test_dtptngen.py
 tests/test_fmtable.py
 tests/test_gregocal.py
 tests/test_icupy.py
+tests/test_listformatter.py
 tests/test_localebuilder.py
 tests/test_localematcher.py
 tests/test_locid.py
 tests/test_measfmt.py
 tests/test_measunit.py
+tests/test_messagepattern.py
 tests/test_msgfmt.py
 tests/test_normalizer2.py
 tests/test_numberformatter.py
 tests/test_numberrangeformatter.py
 tests/test_numfmt.py
 tests/test_plurfmt.py
 tests/test_plurrule.py
 tests/test_rbbi.py
 tests/test_rbnf.py
 tests/test_regex_matcher.py
 tests/test_regex_pattern.py
+tests/test_reldatefmt.py
 tests/test_resbund.py
 tests/test_schriter.py
 tests/test_selfmt.py
 tests/test_smpdtfmt.py
 tests/test_sortkey.py
 tests/test_strenum.py
 tests/test_stsearch.py
```

### Comparing `icupy-0.8.0.post2/src/idna.cpp` & `icupy-0.9.0/src/idna.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/localebuilder.cpp` & `icupy-0.9.0/src/localebuilder.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/localematcher.cpp` & `icupy-0.9.0/src/localematcher.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/locid.cpp` & `icupy-0.9.0/src/locid.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
   loc.def(
       "get_keyword_value",
       [](const Locale &self, const char *keyword_name) {
         if (self.isBogus()) {
           throw ICUError(U_ILLEGAL_ARGUMENT_ERROR);
         }
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto length = self.getKeywordValue(keyword_name, NULL, 0, error_code);
+        const auto length = self.getKeywordValue(keyword_name, nullptr, 0, error_code);
         std::string result(length, '\0');
         error_code = U_ZERO_ERROR;
         self.getKeywordValue(keyword_name, result.data(), (int32_t)result.size(), error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
```

### Comparing `icupy-0.8.0.post2/src/main.cpp` & `icupy-0.9.0/src/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 #ifndef MODULE_NAME
 #define MODULE_NAME icu
 #endif // MODULE_NAME
 
 using namespace icu;
 
+void init_alphaindex(py::module &m);
 void init_appendable(py::module &m);
 void init_char16ptr(py::module &m);
 void init_coleitr(py::module &m);
 void init_compactdecimalformat(py::module &m);
 void init_currpinf(py::module &m);
 void init_currunit(py::module &m);
 void init_datefmt(py::module &m);
@@ -30,14 +31,15 @@
 void init_fieldpos(py::module &m);
 void init_fmtable(py::module &m, py::class_<Formattable, UObject> &fmt);
 void init_format(py::module &m);
 void init_formattedvalue(py::module &m);
 void init_fpositer(py::module &m);
 void init_gregocal(py::module &m);
 void init_idna(py::module &m);
+void init_listformatter(py::module &m);
 void init_localebuilder(py::module &m);
 void init_localematcher(py::module &m);
 void init_locid(py::module &m, py::class_<Locale, UObject> &loc);
 void init_measfmt(py::module &m);
 void init_measunit(py::module &m);
 void init_measure(py::module &m);
 void init_messagepattern(py::module &m);
@@ -51,14 +53,15 @@
 void init_parseerr(py::module &m);
 void init_parsepos(py::module &m);
 void init_plurfmt(py::module &m);
 void init_plurrule(py::module &m, py::class_<PluralRules, UObject> &pr);
 void init_rbbi(py::module &m);
 void init_rbnf(py::module &m);
 void init_regex(py::module &m);
+void init_reldatefmt(py::module &m);
 void init_resbund(py::module &m);
 void init_schriter(py::module &m);
 void init_selfmt(py::module &m);
 void init_smpdtfmt(py::module &m);
 void init_sortkey(py::module &m);
 void init_strenum(py::module &m);
 void init_stsearch(py::module &m);
@@ -83,23 +86,25 @@
 void init_ucurr(py::module &m);
 void init_udat(py::module &m);
 void init_udatpg(py::module &m);
 void init_udisplaycontext(py::module &m);
 void init_uenum(py::module &m);
 void init_uformattedvalue(py::module &m);
 void init_uidna(py::module &m);
+void init_ulistformatter(py::module &m);
 void init_uloc(py::module &m);
 void init_uniset(py::module &m);
 void init_unistr(py::module &m, py::class_<Replaceable, UObject> &rep, py::class_<UnicodeString, Replaceable> &us);
 void init_unorm2(py::module &m);
 void init_unum(py::module &m);
 void init_unumberformatter(py::module &m);
 void init_unumberrangeformatter(py::module &m);
 void init_upluralrules(py::module &m);
 void init_uregex(py::module &m);
+void init_ureldatefmt(py::module &m);
 void init_ures(py::module &m);
 void init_uscript(py::module &m);
 void init_usearch(py::module &m);
 void init_uset(py::module &m);
 void init_ustring(py::module &m);
 void init_utext(py::module &m);
 void init_utrans(py::module &m);
@@ -221,28 +226,32 @@
   init_plurfmt(m);                      // icu::PluralFormat
 
   init_schriter(m); // icu::StringCharacterIterator
   init_coleitr(m);  // icu::CollationElementIterator
 
   init_dtptngen(m);      // icu::DateTimePatternGenerator
   init_idna(m);          // icu::IDNA
+  init_listformatter(m); // icu::ListFormatter
   init_localebuilder(m); // icu::LocaleBuilder
   init_localematcher(m); // icu::LocaleMatcher
   init_locid(m, loc);    // icu::Locale
   init_rbbi(m);          // icu::RuleBasedBreakIterator
   init_regex(m);         // icu::RegexPattern, icu::RegexMatcher
+  init_reldatefmt(m);    // icu::RelativeDateTimeFormatter
   init_resbund(m);       // icu::ResourceBundle
   init_sortkey(m);       // icu::CollationKey
 
   init_uniset(m);      // icu::UnicodeSet
   init_normalizer2(m); // icu::Normalizer2, icu::FilteredNormalizer2
   init_tblcoll(m);     // icu::RuleBasedCollator
   init_stsearch(m);    // icu::StringSearch
   init_translit(m);    // icu::Transliterator
 
+  init_alphaindex(m); // icu::AlphabeticIndex
+
   init_unistr(m, rep, us); // icu::UnicodeString
 
   init_ubidi(m);
   init_ubrk(m);
   init_ucal(m);
   init_uchar(m);
   init_ucnv(m);
@@ -254,21 +263,23 @@
   init_ucurr(m);
   init_udat(m);
   init_udatpg(m);
   init_udisplaycontext(m);
   init_uenum(m);
   init_uformattedvalue(m);
   init_uidna(m);
+  init_ulistformatter(m);
   init_uloc(m);
   init_unorm2(m);
   init_unum(m);
   init_unumberformatter(m);
   init_unumberrangeformatter(m);
   init_upluralrules(m);
   init_uregex(m);
+  init_ureldatefmt(m);
   init_ures(m);
   init_uscript(m);
   init_usearch(m);
   init_uset(m);
   init_ustring(m);
   init_utext(m);
   init_utrans(m);
```

### Comparing `icupy-0.8.0.post2/src/main.hpp` & `icupy-0.9.0/src/main.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #ifndef ICUPY_MAIN_HPP
 #define ICUPY_MAIN_HPP
 
 #ifdef _MSC_VER
 #pragma warning(disable : 4819)
+
+#define strdup _strdup
 #endif // _MSC_VER
 
 #include <list>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl_bind.h>
 #include <unicode/unistr.h>
 #include <vector>
```

### Comparing `icupy-0.8.0.post2/src/measfmt.cpp` & `icupy-0.9.0/src/measfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/measunit.cpp` & `icupy-0.9.0/src/measunit.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -434,27 +434,27 @@
     }
     return result;
   });
   mu.def_static(
         "get_available",
         [](const char *type) {
           UErrorCode error_code = U_ZERO_ERROR;
-          int32_t capacity = MeasureUnit::getAvailable(type, NULL, 0, error_code);
+          int32_t capacity = MeasureUnit::getAvailable(type, nullptr, 0, error_code);
           auto result = std::vector<MeasureUnit>(capacity);
           error_code = U_ZERO_ERROR;
           MeasureUnit::getAvailable(type, result.data(), capacity, error_code);
           if (U_FAILURE(error_code)) {
             throw ICUError(error_code);
           }
           return result;
         },
         py::arg("type_"))
       .def_static("get_available", []() {
         UErrorCode error_code = U_ZERO_ERROR;
-        int32_t capacity = MeasureUnit::getAvailable(NULL, 0, error_code);
+        int32_t capacity = MeasureUnit::getAvailable(nullptr, 0, error_code);
         auto result = std::vector<MeasureUnit>(capacity);
         error_code = U_ZERO_ERROR;
         MeasureUnit::getAvailable(result.data(), capacity, error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
```

### Comparing `icupy-0.8.0.post2/src/measure.cpp` & `icupy-0.9.0/src/measure.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 #include <unicode/tmutamt.h>
 
 using namespace icu;
 
 void init_measure(py::module &m) {
   // icu::Measure
   py::class_<Measure, UObject> meas(m, "Measure");
-  meas.def(py::init([](const Formattable &number, const MeasureUnit &adopted_unit) {
+  meas.def(py::init([](const Formattable &number, const MeasureUnit *adopted_unit) {
              UErrorCode error_code = U_ZERO_ERROR;
-             auto result = std::make_unique<Measure>(number, adopted_unit.clone(), error_code);
+             auto result =
+                 std::make_unique<Measure>(number, adopted_unit ? adopted_unit->clone() : nullptr, error_code);
              if (U_FAILURE(error_code)) {
                throw ICUError(error_code);
              }
              return result;
            }),
            py::arg("number"), py::arg("adopted_unit"))
       .def(py::init<const Measure &>(), py::arg("other"))
```

### Comparing `icupy-0.8.0.post2/src/msgfmt.cpp` & `icupy-0.9.0/src/msgfmt.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -490,18 +490,21 @@
           py::arg("format_name"), py::arg("format_"))
       .def(
           // [2] MessageFormat::setFormat
           "set_format", py::overload_cast<int32_t, const Format &>(&MessageFormat::setFormat), py::arg("format_number"),
           py::arg("format_"));
   mf.def(
       "set_formats",
-      [](MessageFormat &self, std::vector<const Format *> &new_formats, std::optional<int32_t> count) {
-        self.setFormats(new_formats.data(), count.value_or((int32_t)new_formats.size()));
+      [](MessageFormat &self, std::vector<const Format *> &new_formats, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)new_formats.size();
+        }
+        self.setFormats(new_formats.data(), count);
       },
-      py::arg("new_formats"), py::arg("count") = std::nullopt);
+      py::arg("new_formats"), py::arg("count") = -1);
   mf.def("set_locale", &MessageFormat::setLocale, py::arg("locale"))
       .def(
           // const char *locale -> const Locale &locale
           "set_locale", [](MessageFormat &self, const char *locale) { self.setLocale(locale); }, py::arg("locale"));
   mf.def("to_pattern", &MessageFormat::toPattern, py::arg("append_to"));
   mf.def("uses_named_arguments", &MessageFormat::usesNamedArguments);
 }
```

### Comparing `icupy-0.8.0.post2/src/normalizer2.cpp` & `icupy-0.9.0/src/normalizer2.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/numberformatter.cpp` & `icupy-0.9.0/src/numberformatter.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/numberrangeformatter.cpp` & `icupy-0.9.0/src/numberrangeformatter.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/numfmt.cpp` & `icupy-0.9.0/src/numfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/numsys.cpp` & `icupy-0.9.0/src/numsys.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/parseerr.cpp` & `icupy-0.9.0/src/parseerr.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/parsepos.cpp` & `icupy-0.9.0/src/parsepos.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/plurfmt.cpp` & `icupy-0.9.0/src/plurfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/plurrule.cpp` & `icupy-0.9.0/src/plurrule.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -119,30 +119,30 @@
     }
     return result;
   });
   pr.def(
         "get_samples",
         [](PluralRules &self, const UnicodeString &keyword) {
           UErrorCode error_code = U_ZERO_ERROR;
-          auto dest_capacity = self.getSamples(keyword, (double *)NULL, 0, error_code);
+          auto dest_capacity = self.getSamples(keyword, (double *)nullptr, 0, error_code);
           std::vector<double> result(dest_capacity);
           error_code = U_ZERO_ERROR;
           self.getSamples(keyword, result.data(), dest_capacity, error_code);
           if (U_FAILURE(error_code)) {
             throw ICUError(error_code);
           }
           return result;
         },
         py::arg("keyword"))
       .def(
           // const char16_t *keyword -> const UnicodeString &keyword
           "get_samples",
           [](PluralRules &self, const char16_t *keyword) {
             UErrorCode error_code = U_ZERO_ERROR;
-            auto dest_capacity = self.getSamples(keyword, (double *)NULL, 0, error_code);
+            auto dest_capacity = self.getSamples(keyword, (double *)nullptr, 0, error_code);
             std::vector<double> result(dest_capacity);
             error_code = U_ZERO_ERROR;
             self.getSamples(keyword, result.data(), dest_capacity, error_code);
             if (U_FAILURE(error_code)) {
               throw ICUError(error_code);
             }
             return result;
```

### Comparing `icupy-0.8.0.post2/src/rbbi.cpp` & `icupy-0.9.0/src/rbbi.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         return result;
       },
       py::arg("type_"));
   bi.def("get_rule_status", &BreakIterator::getRuleStatus);
 #if (U_ICU_VERSION_MAJOR_NUM >= 52)
   bi.def("get_rule_status_vec", [](BreakIterator &self) {
     UErrorCode error_code = U_ZERO_ERROR;
-    std::vector<int32_t> result(self.getRuleStatusVec(NULL, 0, error_code));
+    std::vector<int32_t> result(self.getRuleStatusVec(nullptr, 0, error_code));
     error_code = U_ZERO_ERROR;
     self.getRuleStatusVec(result.data(), (int32_t)result.size(), error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return result;
   });
@@ -269,15 +269,15 @@
             return result;
           }),
           py::arg("compiled_rules"), py::arg("rule_length"))
       .def(py::self != py::self, py::arg("other"))
       .def(py::self == py::self, py::arg("other"));
   rbbi.def(
       "adopt_text",
-      [](RuleBasedBreakIterator &self, CharacterIterator *it) { self.adoptText(it ? it->clone() : NULL); },
+      [](RuleBasedBreakIterator &self, CharacterIterator *it) { self.adoptText(it ? it->clone() : nullptr); },
       py::arg("it"));
   rbbi.def("clone", &RuleBasedBreakIterator::clone);
   rbbi.def("current", &RuleBasedBreakIterator::current);
   rbbi.def("first", &RuleBasedBreakIterator::first);
   rbbi.def("following", &RuleBasedBreakIterator::following, py::arg("offset"));
   rbbi.def("get_binary_rules", [](RuleBasedBreakIterator &self) {
     uint32_t length = 0;
```

### Comparing `icupy-0.8.0.post2/src/rbnf.cpp` & `icupy-0.9.0/src/rbnf.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/regex.cpp` & `icupy-0.9.0/src/regex.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -506,38 +506,42 @@
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
       },
       py::arg("limit"));
   rm.def(
         "split",
-        [](RegexMatcher &self, const UnicodeString &input, _UnicodeStringVector &dest,
-           std::optional<int32_t> dest_capacity) {
+        [](RegexMatcher &self, const UnicodeString &input, _UnicodeStringVector &dest, int32_t dest_capacity) {
+          if (dest_capacity == -1) {
+            dest_capacity = (int32_t)dest.size();
+          }
           UErrorCode error_code = U_ZERO_ERROR;
-          auto result = self.split(input, dest.data(), dest_capacity.value_or((int32_t)dest.size()), error_code);
+          auto result = self.split(input, dest.data(), dest_capacity, error_code);
           if (U_FAILURE(error_code)) {
             throw ICUError(error_code);
           }
           return result;
         },
-        py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = std::nullopt)
+        py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = -1)
       .def(
           "split",
-          [](RegexMatcher &self, _UTextPtr &input, _UTextVector &dest, std::optional<int32_t> dest_capacity) {
+          [](RegexMatcher &self, _UTextPtr &input, _UTextVector &dest, int32_t dest_capacity) {
+            if (dest_capacity == -1) {
+              dest_capacity = (int32_t)dest.size();
+            }
             UErrorCode error_code = U_ZERO_ERROR;
-            const int32_t output_capacity = dest_capacity.value_or((int32_t)dest.size());
-            std::vector<UText *> output(std::max(0, output_capacity));
+            std::vector<UText *> output(std::max(0, dest_capacity));
             std::copy(dest.begin(), dest.begin() + output.size(), output.begin());
-            auto result = self.split(input, output.data(), output_capacity, error_code);
+            auto result = self.split(input, output.data(), dest_capacity, error_code);
             if (U_FAILURE(error_code)) {
               throw ICUError(error_code);
             }
             return result;
           },
-          py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = std::nullopt);
+          py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = -1);
   rm.def(
         "start",
         [](const RegexMatcher &self, int32_t group) {
           UErrorCode error_code = U_ZERO_ERROR;
           auto result = self.start(group, error_code);
           if (U_FAILURE(error_code)) {
             throw ICUError(error_code);
@@ -783,32 +787,36 @@
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return std::make_unique<_UTextPtr>(p);
   });
   rp.def(
         "split",
-        [](const RegexPattern &self, const UnicodeString &input, _UnicodeStringVector &dest,
-           std::optional<int32_t> dest_capacity) {
+        [](const RegexPattern &self, const UnicodeString &input, _UnicodeStringVector &dest, int32_t dest_capacity) {
+          if (dest_capacity == -1) {
+            dest_capacity = (int32_t)dest.size();
+          }
           UErrorCode error_code = U_ZERO_ERROR;
-          auto result = self.split(input, dest.data(), dest_capacity.value_or((int32_t)dest.size()), error_code);
+          auto result = self.split(input, dest.data(), dest_capacity, error_code);
           if (U_FAILURE(error_code)) {
             throw ICUError(error_code);
           }
           return result;
         },
-        py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = std::nullopt)
+        py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = -1)
       .def(
           "split",
-          [](const RegexPattern &self, _UTextPtr &input, _UTextVector &dest, std::optional<int32_t> dest_capacity) {
+          [](const RegexPattern &self, _UTextPtr &input, _UTextVector &dest, int32_t dest_capacity) {
+            if (dest_capacity == -1) {
+              dest_capacity = (int32_t)dest.size();
+            }
             UErrorCode error_code = U_ZERO_ERROR;
-            const int32_t output_capacity = dest_capacity.value_or((int32_t)dest.size());
-            std::vector<UText *> output(std::max(0, output_capacity));
+            std::vector<UText *> output(std::max(0, dest_capacity));
             std::copy(dest.begin(), dest.begin() + output.size(), output.begin());
-            auto result = self.split(input, output.data(), output_capacity, error_code);
+            auto result = self.split(input, output.data(), dest_capacity, error_code);
             if (U_FAILURE(error_code)) {
               throw ICUError(error_code);
             }
             return result;
           },
-          py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = std::nullopt);
+          py::arg("input_"), py::arg("dest"), py::arg("dest_capacity") = -1);
 }
```

### Comparing `icupy-0.8.0.post2/src/resbund.cpp` & `icupy-0.9.0/src/resbund.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/schriter.cpp` & `icupy-0.9.0/src/schriter.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/selfmt.cpp` & `icupy-0.9.0/src/selfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/smpdtfmt.cpp` & `icupy-0.9.0/src/smpdtfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/sortkey.cpp` & `icupy-0.9.0/src/sortkey.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/strenum.cpp` & `icupy-0.9.0/src/strenum.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
              return result;
            })
       .def(
           "__ne__", [](const StringEnumeration &self, const StringEnumeration &other) { return self != other; },
           py::is_operator(), py::arg("other"))
       .def("__next__", [](StringEnumeration &self) {
         UErrorCode error_code = U_ZERO_ERROR;
-        auto result = self.next(NULL, error_code);
+        auto result = self.next(nullptr, error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
-        } else if (result == NULL) {
+        } else if (result == nullptr) {
           throw py::stop_iteration();
         }
         return result;
       });
   se.def("clone", &StringEnumeration::clone);
   se.def("count", [](const StringEnumeration &self) {
     UErrorCode error_code = U_ZERO_ERROR;
@@ -62,15 +62,15 @@
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return result;
   });
   se.def("next", [](StringEnumeration &self) {
     UErrorCode error_code = U_ZERO_ERROR;
-    auto result = self.next(NULL, error_code);
+    auto result = self.next(nullptr, error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return result;
   });
   se.def("reset", [](StringEnumeration &self) {
     UErrorCode error_code = U_ZERO_ERROR;
@@ -88,14 +88,14 @@
           throw ICUError(error_code);
         }
         return result;
       },
       py::return_value_policy::reference);
   se.def("unext", [](StringEnumeration &self) {
     UErrorCode error_code = U_ZERO_ERROR;
-    auto result = self.unext(NULL, error_code);
+    auto result = self.unext(nullptr, error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return result;
   });
 }
```

### Comparing `icupy-0.8.0.post2/src/stsearch.cpp` & `icupy-0.9.0/src/stsearch.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/tblcoll.cpp` & `icupy-0.9.0/src/tblcoll.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
       },
       py::return_value_policy::reference);
   coll.def_static(
       "get_bound",
       [](const std::vector<uint8_t> &source, int32_t source_length, UColBoundMode bound_type, uint32_t no_of_levels) {
         UErrorCode error_code = U_ZERO_ERROR;
         const auto result_length =
-            Collator::getBound(source.data(), source_length, bound_type, no_of_levels, NULL, 0, error_code);
+            Collator::getBound(source.data(), source_length, bound_type, no_of_levels, nullptr, 0, error_code);
         std::vector<uint8_t> result(result_length);
         error_code = U_ZERO_ERROR;
         Collator::getBound(source.data(), source_length, bound_type, no_of_levels, result.data(), result_length,
                            error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
@@ -106,15 +106,15 @@
                   py::arg("object_locale"), py::arg("display_locale"), py::arg("name"))
       .def_static("get_display_name", py::overload_cast<const Locale &, UnicodeString &>(&Collator::getDisplayName),
                   py::arg("object_locale"), py::arg("name"));
   coll.def_static(
       "get_equivalent_reorder_codes",
       [](int32_t reorder_code) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto dest_capacity = Collator::getEquivalentReorderCodes(reorder_code, NULL, 0, error_code);
+        const auto dest_capacity = Collator::getEquivalentReorderCodes(reorder_code, nullptr, 0, error_code);
         std::vector<int32_t> result(dest_capacity);
         error_code = U_ZERO_ERROR;
         Collator::getEquivalentReorderCodes(reorder_code, result.data(), dest_capacity, error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
@@ -317,15 +317,15 @@
       .def(py::self == py::self, py::arg("other"));
   rbc.def("__copy__", &RuleBasedCollator::clone)
       .def(
           "__deepcopy__", [](const RuleBasedCollator &self, py::dict) { return self.clone(); }, py::arg("memo"));
   rbc.def("clone", &RuleBasedCollator::clone);
   rbc.def("clone_binary", [](const RuleBasedCollator &self) {
     UErrorCode error_code = U_ZERO_ERROR;
-    const auto capacity = self.cloneBinary(NULL, 0, error_code);
+    const auto capacity = self.cloneBinary(nullptr, 0, error_code);
     std::vector<uint8_t> result(capacity);
     error_code = U_ZERO_ERROR;
     self.cloneBinary(result.data(), capacity, error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return result;
@@ -513,49 +513,49 @@
           },
           py::arg("source"), py::arg("key"));
 #if (U_ICU_VERSION_MAJOR_NUM >= 53)
   rbc.def("get_max_variable", &RuleBasedCollator::getMaxVariable);
 #endif // (U_ICU_VERSION_MAJOR_NUM >= 53)
   rbc.def("get_reorder_codes", [](const RuleBasedCollator &self) {
     UErrorCode error_code = U_ZERO_ERROR;
-    const auto dest_capacity = self.getReorderCodes(NULL, 0, error_code);
+    const auto dest_capacity = self.getReorderCodes(nullptr, 0, error_code);
     error_code = U_ZERO_ERROR;
     std::vector<int32_t> result(dest_capacity);
     self.getReorderCodes(result.data(), dest_capacity, error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return result;
   });
   rbc.def("get_rules", py::overload_cast<>(&RuleBasedCollator::getRules, py::const_))
       .def("get_rules", py::overload_cast<UColRuleOption, UnicodeString &>(&RuleBasedCollator::getRules, py::const_),
            py::arg("delta"), py::arg("buffer"));
   rbc.def(
          "get_sort_key",
          [](const RuleBasedCollator &self, const char16_t *source, int32_t source_length) {
-           const auto result_length = self.getSortKey(source, source_length, NULL, 0);
+           const auto result_length = self.getSortKey(source, source_length, nullptr, 0);
            std::vector<uint8_t> result(result_length);
            self.getSortKey(source, source_length, result.data(), result_length);
            return result;
          },
          py::arg("source"), py::arg("source_length"))
       .def(
           "get_sort_key",
           [](const RuleBasedCollator &self, const UnicodeString &source) {
-            const auto result_length = self.getSortKey(source, NULL, 0);
+            const auto result_length = self.getSortKey(source, nullptr, 0);
             std::vector<uint8_t> result(result_length);
             self.getSortKey(source, result.data(), result_length);
             return result;
           },
           py::arg("source"))
       .def(
           // const char16_t *source -> const UnicodeString &source
           "get_sort_key",
           [](const RuleBasedCollator &self, const char16_t *source) {
-            const auto result_length = self.getSortKey(source, NULL, 0);
+            const auto result_length = self.getSortKey(source, nullptr, 0);
             std::vector<uint8_t> result(result_length);
             self.getSortKey(source, result.data(), result_length);
             return result;
           },
           py::arg("source"));
   rbc.def("get_tailored_set", [](const RuleBasedCollator &self) {
     UErrorCode error_code = U_ZERO_ERROR;
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/CMakeLists.txt` & `icupy-0.9.0/src/third_party/pybind11/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -101,33 +101,36 @@
 # NB: when adding a header don't forget to also add it to setup.py
 set(PYBIND11_HEADERS
     include/pybind11/detail/class.h
     include/pybind11/detail/common.h
     include/pybind11/detail/descr.h
     include/pybind11/detail/init.h
     include/pybind11/detail/internals.h
+    include/pybind11/detail/type_caster_base.h
     include/pybind11/detail/typeid.h
     include/pybind11/attr.h
     include/pybind11/buffer_info.h
     include/pybind11/cast.h
     include/pybind11/chrono.h
     include/pybind11/common.h
     include/pybind11/complex.h
     include/pybind11/options.h
     include/pybind11/eigen.h
     include/pybind11/embed.h
     include/pybind11/eval.h
+    include/pybind11/gil.h
     include/pybind11/iostream.h
     include/pybind11/functional.h
     include/pybind11/numpy.h
     include/pybind11/operators.h
     include/pybind11/pybind11.h
     include/pybind11/pytypes.h
     include/pybind11/stl.h
-    include/pybind11/stl_bind.h)
+    include/pybind11/stl_bind.h
+    include/pybind11/stl/filesystem.h)
 
 # Compare with grep and warn if mismatched
 if(PYBIND11_MASTER_PROJECT AND NOT CMAKE_VERSION VERSION_LESS 3.12)
   file(
     GLOB_RECURSE _pybind11_header_check
     LIST_DIRECTORIES false
     RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}"
@@ -196,14 +199,20 @@
 
 if(PYBIND11_INSTALL)
   install(DIRECTORY ${pybind11_INCLUDE_DIR}/pybind11 DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
   set(PYBIND11_CMAKECONFIG_INSTALL_DIR
       "${CMAKE_INSTALL_DATAROOTDIR}/cmake/${PROJECT_NAME}"
       CACHE STRING "install path for pybind11Config.cmake")
 
+  if(IS_ABSOLUTE "${CMAKE_INSTALL_INCLUDEDIR}")
+    set(pybind11_INCLUDEDIR "${CMAKE_INSTALL_FULL_INCLUDEDIR}")
+  else()
+    set(pybind11_INCLUDEDIR "\$\{PACKAGE_PREFIX_DIR\}/${CMAKE_INSTALL_INCLUDEDIR}")
+  endif()
+
   configure_package_config_file(
     tools/${PROJECT_NAME}Config.cmake.in "${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake"
     INSTALL_DESTINATION ${PYBIND11_CMAKECONFIG_INSTALL_DIR})
 
   if(CMAKE_VERSION VERSION_LESS 3.14)
     # Remove CMAKE_SIZEOF_VOID_P from ConfigVersion.cmake since the library does
     # not depend on architecture specific settings or libraries.
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/LICENSE` & `icupy-0.9.0/src/third_party/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/README.rst` & `icupy-0.9.0/src/third_party/pybind11/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,14 @@
 
 `Setuptools example <https://github.com/pybind/python_example>`_
 • `Scikit-build example <https://github.com/pybind/scikit_build_example>`_
 • `CMake example <https://github.com/pybind/cmake_example>`_
 
 .. start
 
-.. warning::
-
-   Combining older versions of pybind11 (< 2.6.0) with Python 3.9.0 will
-   trigger undefined behavior that typically manifests as crashes during
-   interpreter shutdown (but could also destroy your data. **You have been
-   warned.**)
-
-   We recommend that you update to the latest patch release of Python (3.9.1),
-   which includes a `fix <https://github.com/python/cpython/pull/22670>`_
-   that resolves this problem. If you do use Python 3.9.0, please update to
-   the latest version of pybind11 (2.6.0 or newer), which includes a temporary
-   workaround specifically when Python 3.9.0 is detected at runtime.
-
 
 **pybind11** is a lightweight header-only library that exposes C++ types
 in Python and vice versa, mainly to create Python bindings of existing
 C++ code. Its goals and syntax are similar to the excellent
 `Boost.Python <http://www.boost.org/doc/libs/1_58_0/libs/python/doc/>`_
 library by David Abrahams: to minimize boilerplate code in traditional
 extension modules by inferring type information using compile-time
@@ -106,15 +93,15 @@
   between C++ matrix classes like Eigen and NumPy without expensive
   copy operations.
 
 - pybind11 can automatically vectorize functions so that they are
   transparently applied to all entries of one or more NumPy array
   arguments.
 
-- Python’s slice-based access and assignment operations can be
+- Python's slice-based access and assignment operations can be
   supported with just a few lines of code.
 
 - Everything is contained in just a few header files; there is no need
   to link against any additional libraries.
 
 - Binaries are generally smaller by a factor of at least 2 compared to
   equivalent bindings generated by Boost.Python. A recent pybind11
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/attr.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/attr.h`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 struct buffer_protocol { };
 
 /// Annotation which requests that a special metaclass is created for a type
 struct metaclass {
     handle value;
 
     PYBIND11_DEPRECATED("py::metaclass() is no longer required. It's turned on by default now.")
-    metaclass() { } // NOLINT(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
+    // NOLINTNEXTLINE(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
+    metaclass() {}
 
     /// Override pybind11's default metaclass
     explicit metaclass(handle value) : value(value) { }
 };
 
 /// Annotation that marks a class as local to the module:
 struct module_local { const bool value; constexpr module_local(bool v = true) : value(v) { } };
@@ -373,15 +374,15 @@
 };
 
 template <> struct process_attribute<is_new_style_constructor> : process_attribute_default<is_new_style_constructor> {
     static void init(const is_new_style_constructor &, function_record *r) { r->is_new_style_constructor = true; }
 };
 
 inline void process_kw_only_arg(const arg &a, function_record *r) {
-    if (!a.name || strlen(a.name) == 0)
+    if (!a.name || a.name[0] == '\0')
         pybind11_fail("arg(): cannot specify an unnamed argument after an kw_only() annotation");
     ++r->nargs_kw_only;
 }
 
 /// Process a keyword argument attribute (*without* a default value)
 template <> struct process_attribute<arg> : process_attribute_default<arg> {
     static void init(const arg &a, function_record *r) {
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/buffer_info.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/buffer_info.h`

 * *Files 4% similar despite different names*

```diff
@@ -79,27 +79,25 @@
             {view->shape, view->shape + view->ndim},
             /* Though buffer::request() requests PyBUF_STRIDES, ctypes objects
              * ignore this flag and return a view with NULL strides.
              * When strides are NULL, build them manually.  */
             view->strides
             ? std::vector<ssize_t>(view->strides, view->strides + view->ndim)
             : detail::c_strides({view->shape, view->shape + view->ndim}, view->itemsize),
-            view->readonly) {
+            (view->readonly != 0)) {
         this->m_view = view;
         this->ownview = ownview;
     }
 
     buffer_info(const buffer_info &) = delete;
     buffer_info& operator=(const buffer_info &) = delete;
 
-    buffer_info(buffer_info &&other) {
-        (*this) = std::move(other);
-    }
+    buffer_info(buffer_info &&other) noexcept { (*this) = std::move(other); }
 
-    buffer_info& operator=(buffer_info &&rhs) {
+    buffer_info &operator=(buffer_info &&rhs) noexcept {
         ptr = rhs.ptr;
         itemsize = rhs.itemsize;
         size = rhs.size;
         format = std::move(rhs.format);
         ndim = rhs.ndim;
         shape = std::move(rhs.shape);
         strides = std::move(rhs.strides);
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/chrono.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/chrono.h`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,22 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
+
+#include <chrono>
 #include <cmath>
 #include <ctime>
-#include <chrono>
+#include <mutex>
+
+#include <time.h>
+
 #include <datetime.h>
 
 // Backport the PyDateTime_DELTA functions from Python3.3 if required
 #ifndef PyDateTime_DELTA_GET_DAYS
 #define PyDateTime_DELTA_GET_DAYS(o)         (((PyDateTime_Delta*)o)->days)
 #endif
 #ifndef PyDateTime_DELTA_GET_SECONDS
@@ -31,15 +36,15 @@
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <typename type> class duration_caster {
 public:
     using rep = typename type::rep;
     using period = typename type::period;
 
-    using days = std::chrono::duration<uint_fast32_t, std::ratio<86400>>;
+    using days = std::chrono::duration<int_least32_t, std::ratio<86400>>; // signed 25 bits required by the standard.
 
     bool load(handle src, bool) {
         using namespace std::chrono;
 
         // Lazy initialise the PyDateTime import
         if (!PyDateTimeAPI) { PyDateTime_IMPORT; }
 
@@ -49,19 +54,19 @@
             value = type(duration_cast<duration<rep, period>>(
                   days(PyDateTime_DELTA_GET_DAYS(src.ptr()))
                 + seconds(PyDateTime_DELTA_GET_SECONDS(src.ptr()))
                 + microseconds(PyDateTime_DELTA_GET_MICROSECONDS(src.ptr()))));
             return true;
         }
         // If invoked with a float we assume it is seconds and convert
-        else if (PyFloat_Check(src.ptr())) {
+        if (PyFloat_Check(src.ptr())) {
             value = type(duration_cast<duration<rep, period>>(duration<double>(PyFloat_AsDouble(src.ptr()))));
             return true;
         }
-        else return false;
+        return false;
     }
 
     // If this is a duration just return it back
     static const std::chrono::duration<rep, period>& get_duration(const std::chrono::duration<rep, period> &src) {
         return src;
     }
 
@@ -91,14 +96,30 @@
         auto us = duration_cast<us_t>(subd - ss);
         return PyDelta_FromDSU(dd.count(), ss.count(), us.count());
     }
 
     PYBIND11_TYPE_CASTER(type, _("datetime.timedelta"));
 };
 
+inline std::tm *localtime_thread_safe(const std::time_t *time, std::tm *buf) {
+#if (defined(__STDC_LIB_EXT1__) && defined(__STDC_WANT_LIB_EXT1__)) || defined(_MSC_VER)
+    if (localtime_s(buf, time))
+        return nullptr;
+    return buf;
+#else
+    static std::mutex mtx;
+    std::lock_guard<std::mutex> lock(mtx);
+    std::tm *tm_ptr = localtime(time);
+    if (tm_ptr != nullptr) {
+        *buf = *tm_ptr;
+    }
+    return tm_ptr;
+#endif
+}
+
 // This is for casting times on the system clock into datetime.datetime instances
 template <typename Duration> class type_caster<std::chrono::time_point<std::chrono::system_clock, Duration>> {
 public:
     using type = std::chrono::time_point<std::chrono::system_clock, Duration>;
     bool load(handle src, bool) {
         using namespace std::chrono;
 
@@ -157,18 +178,19 @@
         if (us.count() < 0)
             us += seconds(1);
 
         // Subtract microseconds BEFORE `system_clock::to_time_t`, because:
         // > If std::time_t has lower precision, it is implementation-defined whether the value is rounded or truncated.
         // (https://en.cppreference.com/w/cpp/chrono/system_clock/to_time_t)
         std::time_t tt = system_clock::to_time_t(time_point_cast<system_clock::duration>(src - us));
-        // this function uses static memory so it's best to copy it out asap just in case
-        // otherwise other code that is using localtime may break this (not just python code)
-        std::tm localtime = *std::localtime(&tt);
 
+        std::tm localtime;
+        std::tm *localtime_ptr = localtime_thread_safe(&tt, &localtime);
+        if (!localtime_ptr)
+            throw cast_error("Unable to represent system_clock in local time");
         return PyDateTime_FromDateAndTime(localtime.tm_year + 1900,
                                           localtime.tm_mon + 1,
                                           localtime.tm_mday,
                                           localtime.tm_hour,
                                           localtime.tm_min,
                                           localtime.tm_sec,
                                           us.count());
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/complex.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/class.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/class.h`

 * *Files 0% similar despite different names*

```diff
@@ -125,16 +125,17 @@
     PyObject *descr = _PyType_Lookup((PyTypeObject *) obj, name);
 
     // The following assignment combinations are possible:
     //   1. `Type.static_prop = value`             --> descr_set: `Type.static_prop.__set__(value)`
     //   2. `Type.static_prop = other_static_prop` --> setattro:  replace existing `static_prop`
     //   3. `Type.regular_attribute = value`       --> setattro:  regular attribute assignment
     const auto static_prop = (PyObject *) get_internals().static_property_type;
-    const auto call_descr_set = descr && value && PyObject_IsInstance(descr, static_prop)
-                                && !PyObject_IsInstance(value, static_prop);
+    const auto call_descr_set = (descr != nullptr) && (value != nullptr)
+                                && (PyObject_IsInstance(descr, static_prop) != 0)
+                                && (PyObject_IsInstance(value, static_prop) == 0);
     if (call_descr_set) {
         // Call `static_property.__set__()` instead of replacing the `static_property`.
 #if !defined(PYPY_VERSION)
         return Py_TYPE(descr)->tp_descr_set(descr, obj, value);
 #else
         if (PyObject *result = PyObject_CallMethod(descr, "__set__", "OO", obj, value)) {
             Py_DECREF(result);
@@ -158,17 +159,15 @@
  */
 extern "C" inline PyObject *pybind11_meta_getattro(PyObject *obj, PyObject *name) {
     PyObject *descr = _PyType_Lookup((PyTypeObject *) obj, name);
     if (descr && PyInstanceMethod_Check(descr)) {
         Py_INCREF(descr);
         return descr;
     }
-    else {
-        return PyType_Type.tp_getattro(obj, name);
-    }
+    return PyType_Type.tp_getattro(obj, name);
 }
 #endif
 
 /// metaclass `__call__` function that is used to create all pybind11 objects.
 extern "C" inline PyObject *pybind11_meta_call(PyObject *type, PyObject *args, PyObject *kwargs) {
 
     // use the default metaclass call to create/initialize the object
@@ -325,15 +324,15 @@
 
 /// Instance creation function for all pybind11 types. It allocates the internal instance layout for
 /// holding C++ objects and holders.  Allocation is done lazily (the first time the instance is cast
 /// to a reference or pointer), and initialization is done by an `__init__` function.
 inline PyObject *make_new_instance(PyTypeObject *type) {
 #if defined(PYPY_VERSION)
     // PyPy gets tp_basicsize wrong (issue 2482) under multiple inheritance when the first inherited
-    // object is a a plain Python type (i.e. not derived from an extension type).  Fix it.
+    // object is a plain Python type (i.e. not derived from an extension type).  Fix it.
     ssize_t instance_size = static_cast<ssize_t>(sizeof(instance));
     if (type->tp_basicsize < instance_size) {
         type->tp_basicsize = instance_size;
     }
 #endif
     PyObject *self = type->tp_alloc(type, 0);
     auto inst = reinterpret_cast<instance *>(self);
@@ -560,15 +559,15 @@
     view->ndim = 1;
     view->internal = info;
     view->buf = info->ptr;
     view->itemsize = info->itemsize;
     view->len = view->itemsize;
     for (auto s : info->shape)
         view->len *= s;
-    view->readonly = info->readonly;
+    view->readonly = static_cast<int>(info->readonly);
     if ((flags & PyBUF_FORMAT) == PyBUF_FORMAT)
         view->format = const_cast<char *>(info->format.c_str());
     if ((flags & PyBUF_STRIDES) == PyBUF_STRIDES) {
         view->ndim = (int) info->ndim;
         view->strides = &info->strides[0];
         view->shape = &info->shape[0];
     }
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/common.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/common.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,20 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
-#define PYBIND11_VERSION_MINOR 6
-#define PYBIND11_VERSION_PATCH 2
+#define PYBIND11_VERSION_MINOR 7
+#define PYBIND11_VERSION_PATCH 1
+
+// Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
+// Additional convention: 0xD = dev
+#define PYBIND11_VERSION_HEX 0x02070100
 
 #define PYBIND11_NAMESPACE_BEGIN(name) namespace name {
 #define PYBIND11_NAMESPACE_END(name) }
 
 // Robust support for some features and loading modules compiled against different pybind versions
 // requires forcing hidden visibility on pybind code, so we enforce this by setting the attribute on
 // the main `pybind11` namespace.
@@ -48,14 +52,17 @@
 // Compiler version assertions
 #if defined(__INTEL_COMPILER)
 #  if __INTEL_COMPILER < 1800
 #    error pybind11 requires Intel C++ compiler v18 or newer
 #  elif __INTEL_COMPILER < 1900 && defined(PYBIND11_CPP14)
 #    error pybind11 supports only C++11 with Intel C++ compiler v18. Use v19 or newer for C++14.
 #  endif
+/* The following pragma cannot be pop'ed:
+   https://community.intel.com/t5/Intel-C-Compiler/Inline-and-no-inline-warning/td-p/1216764 */
+#  pragma warning disable 2196 // warning #2196: routine is both "inline" and "noinline"
 #elif defined(__clang__) && !defined(__apple_build_version__)
 #  if __clang_major__ < 3 || (__clang_major__ == 3 && __clang_minor__ < 3)
 #    error pybind11 requires clang 3.3 or newer
 #  endif
 #elif defined(__clang__)
 // Apple changes clang version macros to its Xcode version; the first Xcode release based on
 // (upstream) clang 3.3 was Xcode 5:
@@ -78,21 +85,35 @@
 #  if defined(WIN32) || defined(_WIN32)
 #    define PYBIND11_EXPORT __declspec(dllexport)
 #  else
 #    define PYBIND11_EXPORT __attribute__ ((visibility("default")))
 #  endif
 #endif
 
+#if !defined(PYBIND11_EXPORT_EXCEPTION)
+#  ifdef __MINGW32__
+// workaround for:
+// error: 'dllexport' implies default visibility, but xxx has already been declared with a different visibility
+#    define PYBIND11_EXPORT_EXCEPTION
+#  else
+#    define PYBIND11_EXPORT_EXCEPTION PYBIND11_EXPORT
+#  endif
+#endif
+
 #if defined(_MSC_VER)
 #  define PYBIND11_NOINLINE __declspec(noinline)
 #else
 #  define PYBIND11_NOINLINE __attribute__ ((noinline))
 #endif
 
-#if defined(PYBIND11_CPP14)
+#if defined(__MINGW32__)
+// For unknown reasons all PYBIND11_DEPRECATED member trigger a warning when declared
+// whether it is used or not
+#  define PYBIND11_DEPRECATED(reason)
+#elif defined(PYBIND11_CPP14)
 #  define PYBIND11_DEPRECATED(reason) [[deprecated(reason)]]
 #else
 #  define PYBIND11_DEPRECATED(reason) __attribute__((deprecated(reason)))
 #endif
 
 #if defined(PYBIND11_CPP17)
 #  define PYBIND11_MAYBE_UNUSED [[maybe_unused]]
@@ -110,21 +131,27 @@
 
 /// Include Python header, disable linking to pythonX_d.lib on Windows in debug mode
 #if defined(_MSC_VER)
 #  if (PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION < 4)
 #    define HAVE_ROUND 1
 #  endif
 #  pragma warning(push)
-#  pragma warning(disable: 4510 4610 4512 4005)
+// C4505: 'PySlice_GetIndicesEx': unreferenced local function has been removed (PyPy only)
+#  pragma warning(disable: 4505)
 #  if defined(_DEBUG) && !defined(Py_DEBUG)
 #    define PYBIND11_DEBUG_MARKER
 #    undef _DEBUG
 #  endif
 #endif
 
+// https://en.cppreference.com/w/c/chrono/localtime
+#if defined(__STDC_LIB_EXT1__) && !defined(__STDC_WANT_LIB_EXT1__)
+#    define __STDC_WANT_LIB_EXT1__
+#endif
+
 #include <Python.h>
 #include <frameobject.h>
 #include <pythread.h>
 
 /* Python #defines overrides on all sorts of core functions, which
    tends to weak havok in C++ codebases that expect these to work
    like regular functions (potentially with several overloads) */
@@ -158,14 +185,32 @@
 #include <stdexcept>
 #include <exception>
 #include <unordered_set>
 #include <unordered_map>
 #include <memory>
 #include <typeindex>
 #include <type_traits>
+#if defined(__has_include)
+#  if __has_include(<version>)
+#    include <version>
+#  endif
+#endif
+
+// #define PYBIND11_STR_LEGACY_PERMISSIVE
+// If DEFINED, pybind11::str can hold PyUnicodeObject or PyBytesObject
+//             (probably surprising and never documented, but this was the
+//             legacy behavior until and including v2.6.x). As a side-effect,
+//             pybind11::isinstance<str>() is true for both pybind11::str and
+//             pybind11::bytes.
+// If UNDEFINED, pybind11::str can only hold PyUnicodeObject, and
+//               pybind11::isinstance<str>() is true only for pybind11::str.
+//               However, for Python 2 only (!), the pybind11::str caster
+//               implicitly decodes bytes to PyUnicodeObject. This is to ease
+//               the transition from the legacy behavior to the non-permissive
+//               behavior.
 
 #if PY_MAJOR_VERSION >= 3 /// Compatibility macros for various Python versions
 #define PYBIND11_INSTANCE_METHOD_NEW(ptr, class_) PyInstanceMethod_New(ptr)
 #define PYBIND11_INSTANCE_METHOD_CHECK PyInstanceMethod_Check
 #define PYBIND11_INSTANCE_METHOD_GET_FUNCTION PyInstanceMethod_GET_FUNCTION
 #define PYBIND11_BYTES_CHECK PyBytes_Check
 #define PYBIND11_BYTES_FROM_STRING PyBytes_FromString
@@ -458,15 +503,15 @@
     /// If true, get_internals().patients has an entry for this object
     bool has_patients : 1;
 
     /// Initializes all of the above type/values/holders data (but not the instance values themselves)
     void allocate_layout();
 
     /// Destroys/deallocates all of the above
-    void deallocate_layout();
+    void deallocate_layout() const;
 
     /// Returns the value_and_holder wrapper for the given type (or the first, if `find_type`
     /// omitted).  Returns a default-constructed (with `.inst = nullptr`) object on failure if
     /// `throw_if_missing` is false.
     value_and_holder get_value_and_holder(const type_info *find_type = nullptr, bool throw_if_missing = true);
 
     /// Bit values for the non-simple status flags
@@ -701,24 +746,31 @@
 #else
 using expand_side_effects = bool[];
 #define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN) (void)pybind11::detail::expand_side_effects{ ((PATTERN), void(), false)..., false }
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
+#if defined(_MSC_VER)
+#  pragma warning(push)
+#  pragma warning(disable: 4275) // warning C4275: An exported class was derived from a class that wasn't exported. Can be ignored when derived from a STL class.
+#endif
 /// C++ bindings of builtin Python exceptions
-class builtin_exception : public std::runtime_error {
+class PYBIND11_EXPORT_EXCEPTION builtin_exception : public std::runtime_error {
 public:
     using std::runtime_error::runtime_error;
     /// Set the error using the Python C API
     virtual void set_error() const = 0;
 };
+#if defined(_MSC_VER)
+#  pragma warning(pop)
+#endif
 
 #define PYBIND11_RUNTIME_EXCEPTION(name, type) \
-    class name : public builtin_exception { public: \
+    class PYBIND11_EXPORT_EXCEPTION name : public builtin_exception { public: \
         using builtin_exception::builtin_exception; \
         name() : name("") { } \
         void set_error() const override { PyErr_SetString(type, what()); } \
     };
 
 PYBIND11_RUNTIME_EXCEPTION(stop_iteration, PyExc_StopIteration)
 PYBIND11_RUNTIME_EXCEPTION(index_error, PyExc_IndexError)
@@ -772,15 +824,16 @@
 
 /// Dummy destructor wrapper that can be used to expose classes with a private destructor
 struct nodelete { template <typename T> void operator()(T*) { } };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 template <typename... Args>
 struct overload_cast_impl {
-    constexpr overload_cast_impl() {}; // NOLINT(modernize-use-equals-default):  MSVC 2015 needs this
+    // NOLINTNEXTLINE(modernize-use-equals-default):  MSVC 2015 needs this
+    constexpr overload_cast_impl() {}
 
     template <typename Return>
     constexpr auto operator()(Return (*pf)(Args...)) const noexcept
                               -> decltype(pf) { return pf; }
 
     template <typename Return, typename Class>
     constexpr auto operator()(Return (Class::*pmf)(Args...), std::false_type = {}) const noexcept
@@ -853,9 +906,27 @@
     std::vector<T> *operator->() { return &v; }
     const std::vector<T> *operator->() const { return &v; }
 };
 
 // Forward-declaration; see detail/class.h
 std::string get_fully_qualified_tp_name(PyTypeObject*);
 
+template <typename T>
+inline static std::shared_ptr<T> try_get_shared_from_this(std::enable_shared_from_this<T> *holder_value_ptr) {
+// Pre C++17, this code path exploits undefined behavior, but is known to work on many platforms.
+// Use at your own risk!
+// See also https://en.cppreference.com/w/cpp/memory/enable_shared_from_this, and in particular
+// the `std::shared_ptr<Good> gp1 = not_so_good.getptr();` and `try`-`catch` parts of the example.
+#if defined(__cpp_lib_enable_shared_from_this) && (!defined(_MSC_VER) || _MSC_VER >= 1912)
+    return holder_value_ptr->weak_from_this().lock();
+#else
+    try {
+        return holder_value_ptr->shared_from_this();
+    }
+    catch (const std::bad_weak_ptr &) {
+        return nullptr;
+    }
+#endif
+}
+
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/descr.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/descr.h`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 #else
 #  define PYBIND11_DESCR_CONSTEXPR const
 #endif
 
 /* Concatenate type signatures at compile time */
 template <size_t N, typename... Ts>
 struct descr {
-    char text[N + 1];
+    char text[N + 1]{'\0'};
 
-    constexpr descr() : text{'\0'} { }
+    constexpr descr() = default;
     constexpr descr(char const (&s)[N+1]) : descr(s, make_index_sequence<N>()) { }
 
     template <size_t... Is>
     constexpr descr(char const (&s)[N+1], index_sequence<Is...>) : text{s[Is]..., '\0'} { }
 
     template <typename... Chars>
     constexpr descr(char c, Chars... cs) : text{c, static_cast<char>(cs)..., '\0'} { }
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/init.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/init.h`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,21 @@
 }
 
 /// Set both the C++ and Python states
 template <typename Class, typename T, typename O,
           enable_if_t<std::is_convertible<O, handle>::value, int> = 0>
 void setstate(value_and_holder &v_h, std::pair<T, O> &&result, bool need_alias) {
     construct<Class>(v_h, std::move(result.first), need_alias);
-    setattr((PyObject *) v_h.inst, "__dict__", result.second);
+    auto d = handle(result.second);
+    if (PyDict_Check(d.ptr()) && PyDict_Size(d.ptr()) == 0) {
+        // Skipping setattr below, to not force use of py::dynamic_attr() for Class unnecessarily.
+        // See PR #2972 for details.
+        return;
+    }
+    setattr((PyObject *) v_h.inst, "__dict__", d);
 }
 
 /// Implementation for py::pickle(GetState, SetState)
 template <typename Get, typename Set,
           typename = function_signature_t<Get>, typename = function_signature_t<Set>>
 struct pickle_factory;
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/internals.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/internals.h`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,16 @@
         internals_pp = static_cast<internals **>(capsule(builtins[id]));
 
         // We loaded builtins through python's builtins, which means that our `error_already_set`
         // and `builtin_exception` may be different local classes than the ones set up in the
         // initial exception translator, below, so add another for our local exception classes.
         //
         // libstdc++ doesn't require this (types there are identified only by name)
+        // libc++ with CPython doesn't require this (types are explicitly exported)
+        // libc++ with PyPy still need it, awaiting further investigation
 #if !defined(__GLIBCXX__)
         (*internals_pp)->registered_exception_translators.push_front(&translate_local_exception);
 #endif
     } else {
         if (!internals_pp) internals_pp = new internals*();
         auto *&internals_ptr = *internals_pp;
         internals_ptr = new internals();
@@ -287,15 +289,15 @@
 
         #if PY_VERSION_HEX < 0x03090000
                 PyEval_InitThreads();
         #endif
         PyThreadState *tstate = PyThreadState_Get();
         #if PY_VERSION_HEX >= 0x03070000
             internals_ptr->tstate = PyThread_tss_alloc();
-            if (!internals_ptr->tstate || PyThread_tss_create(internals_ptr->tstate))
+            if (!internals_ptr->tstate || (PyThread_tss_create(internals_ptr->tstate) != 0))
                 pybind11_fail("get_internals: could not successfully initialize the TSS key!");
             PyThread_tss_set(internals_ptr->tstate, tstate);
         #else
             internals_ptr->tstate = PyThread_create_key();
             if (internals_ptr->tstate == -1)
                 pybind11_fail("get_internals: could not successfully initialize the TLS key!");
             PyThread_set_key_value(internals_ptr->tstate, tstate);
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/detail/typeid.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/eigen.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/eigen.h`

 * *Files 1% similar despite different names*

```diff
@@ -165,29 +165,26 @@
               stride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar));
 
         if (vector) { // Eigen type is a compile-time vector
             if (fixed && size != n)
                 return false; // Vector size mismatch
             return {rows == 1 ? 1 : n, cols == 1 ? 1 : n, stride};
         }
-        else if (fixed) {
+        if (fixed) {
             // The type has a fixed size, but is not a vector: abort
             return false;
         }
-        else if (fixed_cols) {
+        if (fixed_cols) {
             // Since this isn't a vector, cols must be != 1.  We allow this only if it exactly
             // equals the number of elements (rows is Dynamic, and so 1 row is allowed).
             if (cols != n) return false;
             return {1, n, stride};
-        }
-        else {
-            // Otherwise it's either fully dynamic, or column dynamic; both become a column vector
+        } // Otherwise it's either fully dynamic, or column dynamic; both become a column vector
             if (fixed_rows && rows != n) return false;
             return {n, 1, stride};
-        }
     }
 
     static constexpr bool show_writeable = is_eigen_dense_map<Type>::value && is_eigen_mutable_map<Type>::value;
     static constexpr bool show_order = is_eigen_dense_map<Type>::value;
     static constexpr bool show_c_contiguous = show_order && requires_row_major;
     static constexpr bool show_f_contiguous = !show_c_contiguous && show_order && requires_col_major;
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/embed.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/embed.h`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 struct embedded_module {
 #if PY_MAJOR_VERSION >= 3
     using init_t = PyObject *(*)();
 #else
     using init_t = void (*)();
 #endif
     embedded_module(const char *name, init_t init) {
-        if (Py_IsInitialized())
+        if (Py_IsInitialized() != 0)
             pybind11_fail("Can't add new modules after the interpreter has been initialized");
 
         auto result = PyImport_AppendInittab(name, init);
         if (result == -1)
             pybind11_fail("Insufficient memory to add a new module");
     }
 };
@@ -97,15 +97,15 @@
     If initializing the Python interpreter fails, then the program is terminated.  (This
     is controlled by the CPython runtime and is an exception to pybind11's normal behavior
     of throwing exceptions on errors.)
 
     .. _Python documentation: https://docs.python.org/3/c-api/init.html#c.Py_InitializeEx
  \endrst */
 inline void initialize_interpreter(bool init_signal_handlers = true) {
-    if (Py_IsInitialized())
+    if (Py_IsInitialized() != 0)
         pybind11_fail("The interpreter is already running");
 
     Py_InitializeEx(init_signal_handlers ? 1 : 0);
 
     // Make .py files in the working directory available by default
     module_::import("sys").attr("path").cast<list>().append(".");
 }
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/eval.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/eval.h`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
+#include <utility>
+
 #include "pybind11.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 inline void ensure_builtins_in_globals(object &global) {
     #if PY_VERSION_HEX < 0x03080000
@@ -39,25 +41,25 @@
     eval_single_statement,
 
     /// Evaluate a string containing a sequence of statement. Returns \c none
     eval_statements
 };
 
 template <eval_mode mode = eval_expr>
-object eval(str expr, object global = globals(), object local = object()) {
+object eval(const str &expr, object global = globals(), object local = object()) {
     if (!local)
         local = global;
 
     detail::ensure_builtins_in_globals(global);
 
     /* PyRun_String does not accept a PyObject / encoding specifier,
        this seems to be the only alternative */
     std::string buffer = "# -*- coding: utf-8 -*-\n" + (std::string) expr;
 
-    int start;
+    int start = 0;
     switch (mode) {
         case eval_expr:             start = Py_eval_input;   break;
         case eval_single_statement: start = Py_single_input; break;
         case eval_statements:       start = Py_file_input;   break;
         default: pybind11_fail("invalid evaluation mode");
     }
 
@@ -71,16 +73,16 @@
 object eval(const char (&s)[N], object global = globals(), object local = object()) {
     /* Support raw string literals by removing common leading whitespace */
     auto expr = (s[0] == '\n') ? str(module_::import("textwrap").attr("dedent")(s))
                                : str(s);
     return eval<mode>(expr, global, local);
 }
 
-inline void exec(str expr, object global = globals(), object local = object()) {
-    eval<eval_statements>(expr, global, local);
+inline void exec(const str &expr, object global = globals(), object local = object()) {
+    eval<eval_statements>(expr, std::move(global), std::move(local));
 }
 
 template <size_t N>
 void exec(const char (&s)[N], object global = globals(), object local = object()) {
     eval<eval_statements>(s, global, local);
 }
 
@@ -101,15 +103,15 @@
 template <eval_mode mode = eval_statements>
 object eval_file(str fname, object global = globals(), object local = object()) {
     if (!local)
         local = global;
 
     detail::ensure_builtins_in_globals(global);
 
-    int start;
+    int start = 0;
     switch (mode) {
         case eval_expr:             start = Py_eval_input;   break;
         case eval_single_statement: start = Py_single_input; break;
         case eval_statements:       start = Py_file_input;   break;
         default: pybind11_fail("invalid evaluation mode");
     }
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/functional.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/functional.h`

 * *Files 13% similar despite different names*

```diff
@@ -39,43 +39,57 @@
            function via Python, every function call would normally involve
            a full C++ -> Python -> C++ roundtrip, which can be prohibitive.
            Here, we try to at least detect the case where the function is
            stateless (i.e. function pointer or lambda function without
            captured variables), in which case the roundtrip can be avoided.
          */
         if (auto cfunc = func.cpp_function()) {
-            auto c = reinterpret_borrow<capsule>(PyCFunction_GET_SELF(cfunc.ptr()));
-            auto rec = (function_record *) c;
-
-            if (rec && rec->is_stateless &&
-                    same_type(typeid(function_type), *reinterpret_cast<const std::type_info *>(rec->data[1]))) {
-                struct capture { function_type f; };
-                value = ((capture *) &rec->data)->f;
-                return true;
+            auto cfunc_self = PyCFunction_GET_SELF(cfunc.ptr());
+            if (isinstance<capsule>(cfunc_self)) {
+                auto c = reinterpret_borrow<capsule>(cfunc_self);
+                auto rec = (function_record *) c;
+
+                while (rec != nullptr) {
+                    if (rec->is_stateless
+                        && same_type(typeid(function_type),
+                                     *reinterpret_cast<const std::type_info *>(rec->data[1]))) {
+                        struct capture {
+                            function_type f;
+                        };
+                        value = ((capture *) &rec->data)->f;
+                        return true;
+                    }
+                    rec = rec->next;
+                }
             }
+            // PYPY segfaults here when passing builtin function like sum.
+            // Raising an fail exception here works to prevent the segfault, but only on gcc.
+            // See PR #1413 for full details
         }
 
         // ensure GIL is held during functor destruction
         struct func_handle {
             function f;
-            func_handle(function&& f_) : f(std::move(f_)) {}
-            func_handle(const func_handle& f_) {
+            func_handle(function &&f_) noexcept : f(std::move(f_)) {}
+            func_handle(const func_handle &f_) { operator=(f_); }
+            func_handle &operator=(const func_handle &f_) {
                 gil_scoped_acquire acq;
                 f = f_.f;
+                return *this;
             }
             ~func_handle() {
                 gil_scoped_acquire acq;
                 function kill_f(std::move(f));
             }
         };
 
         // to emulate 'move initialization capture' in C++11
         struct func_wrapper {
             func_handle hfunc;
-            func_wrapper(func_handle&& hf): hfunc(std::move(hf)) {}
+            func_wrapper(func_handle &&hf) noexcept : hfunc(std::move(hf)) {}
             Return operator()(Args... args) const {
                 gil_scoped_acquire acq;
                 object retval(hfunc.f(std::forward<Args>(args)...));
                 /* Visual studio 2015 parser issue: need parentheses around this expression */
                 return (retval.template cast<Return>());
             }
         };
@@ -88,16 +102,15 @@
     static handle cast(Func &&f_, return_value_policy policy, handle /* parent */) {
         if (!f_)
             return none().inc_ref();
 
         auto result = f_.template target<function_type>();
         if (result)
             return cpp_function(*result, policy).release();
-        else
-            return cpp_function(std::forward<Func>(f_), policy).release();
+        return cpp_function(std::forward<Func>(f_), policy).release();
     }
 
     PYBIND11_TYPE_CASTER(type, _("Callable[[") + concat(make_caster<Args>::name...) + _("], ")
                                + make_caster<retval_type>::name + _("]"));
 };
 
 PYBIND11_NAMESPACE_END(detail)
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/numpy.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/numpy.h`

 * *Files 2% similar despite different names*

```diff
@@ -160,18 +160,18 @@
             NPY_ULONG_, NPY_UINT_, NPY_USHORT_),
         NPY_INT64_ = platform_lookup<std::int64_t, long, long long, int>(
             NPY_LONG_, NPY_LONGLONG_, NPY_INT_),
         NPY_UINT64_ = platform_lookup<std::uint64_t, unsigned long, unsigned long long, unsigned int>(
             NPY_ULONG_, NPY_ULONGLONG_, NPY_UINT_),
     };
 
-    typedef struct {
+    struct PyArray_Dims {
         Py_intptr_t *ptr;
         int len;
-    } PyArray_Dims;
+    };
 
     static npy_api& get() {
         static npy_api api = lookup();
         return api;
     }
 
     bool PyArray_Check_(PyObject *obj) const {
@@ -315,22 +315,21 @@
 template <size_t N> struct array_info<char[N]> : array_info_scalar<char[N]> { };
 template <size_t N> struct array_info<std::array<char, N>> : array_info_scalar<std::array<char, N>> { };
 template <typename T, size_t N> struct array_info<T[N]> : array_info<std::array<T, N>> { };
 template <typename T> using remove_all_extents_t = typename array_info<T>::type;
 
 template <typename T> using is_pod_struct = all_of<
     std::is_standard_layout<T>,     // since we're accessing directly in memory we need a standard layout type
-#if !defined(__GNUG__) || defined(_LIBCPP_VERSION) || defined(_GLIBCXX_USE_CXX11_ABI)
-    // _GLIBCXX_USE_CXX11_ABI indicates that we're using libstdc++ from GCC 5 or newer, independent
-    // of the actual compiler (Clang can also use libstdc++, but it always defines __GNUC__ == 4).
-    std::is_trivially_copyable<T>,
-#else
-    // GCC 4 doesn't implement is_trivially_copyable, so approximate it
+#if defined(__GLIBCXX__) && (__GLIBCXX__ < 20150422 || __GLIBCXX__ == 20150623 || __GLIBCXX__ == 20150626 || __GLIBCXX__ == 20160803)
+    // libstdc++ < 5 (including versions 4.8.5, 4.9.3 and 4.9.4 which were released after 5)
+    // don't implement is_trivially_copyable, so approximate it
     std::is_trivially_destructible<T>,
     satisfies_any_of<T, std::has_trivial_copy_constructor, std::has_trivial_copy_assign>,
+#else
+    std::is_trivially_copyable<T>,
 #endif
     satisfies_none_of<T, std::is_reference, std::is_array, is_std_array, std::is_arithmetic, is_complex, std::is_enum>
 >;
 
 // Replacement for std::is_pod (deprecated in C++20)
 template <typename T> using is_pod = all_of<
     std::is_standard_layout<T>,
@@ -462,15 +461,17 @@
 class dtype : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(dtype, object, detail::npy_api::get().PyArrayDescr_Check_);
 
     explicit dtype(const buffer_info &info) {
         dtype descr(_dtype_from_pep3118()(PYBIND11_STR_TYPE(info.format)));
         // If info.itemsize == 0, use the value calculated from the format string
-        m_ptr = descr.strip_padding(info.itemsize ? info.itemsize : descr.itemsize()).release().ptr();
+        m_ptr = descr.strip_padding(info.itemsize != 0 ? info.itemsize : descr.itemsize())
+                    .release()
+                    .ptr();
     }
 
     explicit dtype(const std::string &format) {
         m_ptr = from_args(pybind11::str(format)).release().ptr();
     }
 
     dtype(const char *format) : dtype(std::string(format)) { }
@@ -483,15 +484,15 @@
         args["itemsize"] = pybind11::int_(itemsize);
         m_ptr = from_args(args).release().ptr();
     }
 
     /// This is essentially the same as calling numpy.dtype(args) in Python.
     static dtype from_args(object args) {
         PyObject *ptr = nullptr;
-        if (!detail::npy_api::get().PyArray_DescrConverter_(args.ptr(), &ptr) || !ptr)
+        if ((detail::npy_api::get().PyArray_DescrConverter_(args.ptr(), &ptr) == 0) || !ptr)
             throw error_already_set();
         return reinterpret_steal<dtype>(ptr);
     }
 
     /// Return dtype associated with a C++ type.
     template <typename T> static dtype of() {
         return detail::npy_format_descriptor<typename std::remove_cv<T>::type>::dtype();
@@ -503,19 +504,29 @@
     }
 
     /// Returns true for structured data types.
     bool has_fields() const {
         return detail::array_descriptor_proxy(m_ptr)->names != nullptr;
     }
 
-    /// Single-character type code.
+    /// Single-character code for dtype's kind.
+    /// For example, floating point types are 'f' and integral types are 'i'.
     char kind() const {
         return detail::array_descriptor_proxy(m_ptr)->kind;
     }
 
+    /// Single-character for dtype's type.
+    /// For example, ``float`` is 'f', ``double`` 'd', ``int`` 'i', and ``long`` 'd'.
+    char char_() const {
+        // Note: The signature, `dtype::char_` follows the naming of NumPy's
+        // public Python API (i.e., ``dtype.char``), rather than its internal
+        // C API (``PyArray_Descr::type``).
+        return detail::array_descriptor_proxy(m_ptr)->type;
+    }
+
 private:
     static object _dtype_from_pep3118() {
         static PyObject *obj = module_::import("numpy.core._internal")
             .attr("_dtype_from_pep3118").cast<object>().release().ptr();
         return reinterpret_borrow<object>(obj);
     }
 
@@ -529,15 +540,15 @@
         std::vector<field_descr> field_descriptors;
 
         for (auto field : attr("fields").attr("items")()) {
             auto spec = field.cast<tuple>();
             auto name = spec[0].cast<pybind11::str>();
             auto format = spec[1].cast<tuple>()[0].cast<dtype>();
             auto offset = spec[1].cast<tuple>()[1].cast<pybind11::int_>();
-            if (!len(name) && format.kind() == 'V')
+            if ((len(name) == 0u) && format.kind() == 'V')
                 continue;
             field_descriptors.push_back({(PYBIND11_STR_TYPE) name, format.strip_padding(format.itemsize()), offset});
         }
 
         std::sort(field_descriptors.begin(), field_descriptors.end(),
                   [](const field_descr& a, const field_descr& b) {
                       return a.offset.cast<int>() < b.offset.cast<int>();
@@ -859,19 +870,20 @@
 
     explicit array_t(const buffer_info& info, handle base = handle()) : array(info, base) { }
 
     array_t(ShapeContainer shape, StridesContainer strides, const T *ptr = nullptr, handle base = handle())
         : array(std::move(shape), std::move(strides), ptr, base) { }
 
     explicit array_t(ShapeContainer shape, const T *ptr = nullptr, handle base = handle())
-        : array_t(private_ctor{}, std::move(shape),
-                ExtraFlags & f_style
-                ? detail::f_strides(*shape, itemsize())
-                : detail::c_strides(*shape, itemsize()),
-                ptr, base) { }
+        : array_t(private_ctor{},
+                  std::move(shape),
+                  (ExtraFlags & f_style) != 0 ? detail::f_strides(*shape, itemsize())
+                                              : detail::c_strides(*shape, itemsize()),
+                  ptr,
+                  base) {}
 
     explicit array_t(ssize_t count, const T *ptr = nullptr, handle base = handle())
         : array({count}, {}, ptr, base) { }
 
     constexpr ssize_t itemsize() const {
         return sizeof(T);
     }
@@ -1016,23 +1028,28 @@
     static constexpr auto name = _<std::is_same<T, bool>::value>(
         _("bool"), _<std::is_signed<T>::value>("numpy.int", "numpy.uint") + _<sizeof(T)*8>()
     );
 };
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<std::is_floating_point<T>::value>> {
-    static constexpr auto name = _<std::is_same<T, float>::value || std::is_same<T, double>::value>(
+    static constexpr auto name = _<std::is_same<T, float>::value
+                                   || std::is_same<T, const float>::value
+                                   || std::is_same<T, double>::value
+                                   || std::is_same<T, const double>::value>(
         _("numpy.float") + _<sizeof(T)*8>(), _("numpy.longdouble")
     );
 };
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<is_complex<T>::value>> {
     static constexpr auto name = _<std::is_same<typename T::value_type, float>::value
-                                   || std::is_same<typename T::value_type, double>::value>(
+                                   || std::is_same<typename T::value_type, const float>::value
+                                   || std::is_same<typename T::value_type, double>::value
+                                   || std::is_same<typename T::value_type, const double>::value>(
         _("numpy.complex") + _<sizeof(typename T::value_type)*16>(), _("numpy.longcomplex")
     );
 };
 
 template <typename T>
 struct npy_format_descriptor<T, enable_if_t<satisfies_any_of<T, std::is_arithmetic, is_complex>::value>>
     : npy_format_descriptor_name<T> {
@@ -1273,15 +1290,15 @@
 
 class common_iterator {
 public:
     using container_type = std::vector<ssize_t>;
     using value_type = container_type::value_type;
     using size_type = container_type::size_type;
 
-    common_iterator() : p_ptr(0), m_strides() {}
+    common_iterator() : m_strides() {}
 
     common_iterator(void* ptr, const container_type& strides, const container_type& shape)
         : p_ptr(reinterpret_cast<char*>(ptr)), m_strides(strides.size()) {
         m_strides.back() = static_cast<value_type>(strides.back());
         for (size_type i = m_strides.size() - 1; i != 0; --i) {
             size_type j = i - 1;
             auto s = static_cast<value_type>(shape[i]);
@@ -1294,15 +1311,15 @@
     }
 
     void* data() const {
         return p_ptr;
     }
 
 private:
-    char* p_ptr;
+    char *p_ptr{0};
     container_type m_strides;
 };
 
 template <size_t N> class multi_array_iterator {
 public:
     using container_type = std::vector<ssize_t>;
 
@@ -1322,17 +1339,16 @@
 
     multi_array_iterator& operator++() {
         for (size_t j = m_index.size(); j != 0; --j) {
             size_t i = j - 1;
             if (++m_index[i] != m_shape[i]) {
                 increment_common_iterator(i);
                 break;
-            } else {
-                m_index[i] = 0;
             }
+            m_index[i] = 0;
         }
         return *this;
     }
 
     template <size_t K, class T = void> T* data() const {
         return reinterpret_cast<T*>(m_common_iterator[K].data());
     }
@@ -1475,16 +1491,15 @@
 template <typename Func, typename Return, typename... Args>
 struct vectorize_returned_array {
     using Type = array_t<Return>;
 
     static Type create(broadcast_trivial trivial, const std::vector<ssize_t> &shape) {
         if (trivial == broadcast_trivial::f_trivial)
             return array_t<Return, array::f_style>(shape);
-        else
-            return array_t<Return>(shape);
+        return array_t<Return>(shape);
     }
 
     static Return *mutable_data(Type &array) {
         return array.mutable_data();
     }
 
     static Return call(Func &f, Args &... args) {
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/operators.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/options.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/pybind11.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/pybind11.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,62 +6,69 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
-#if defined(__INTEL_COMPILER)
-#  pragma warning push
-#  pragma warning disable 68    // integer conversion resulted in a change of sign
-#  pragma warning disable 186   // pointless comparison of unsigned integer with zero
-#  pragma warning disable 878   // incompatible exception specifications
-#  pragma warning disable 1334  // the "template" keyword used for syntactic disambiguation may only be used within a template
-#  pragma warning disable 1682  // implicit conversion of a 64-bit integral type to a smaller integral type (potential portability problem)
-#  pragma warning disable 1786  // function "strdup" was declared deprecated
-#  pragma warning disable 1875  // offsetof applied to non-POD (Plain Old Data) types is nonstandard
-#  pragma warning disable 2196  // warning #2196: routine is both "inline" and "noinline"
-#elif defined(_MSC_VER)
+#if defined(_MSC_VER) && !defined(__INTEL_COMPILER)
 #  pragma warning(push)
 #  pragma warning(disable: 4100) // warning C4100: Unreferenced formal parameter
 #  pragma warning(disable: 4127) // warning C4127: Conditional expression is constant
-#  pragma warning(disable: 4512) // warning C4512: Assignment operator was implicitly defined as deleted
-#  pragma warning(disable: 4800) // warning C4800: 'int': forcing value to bool 'true' or 'false' (performance warning)
-#  pragma warning(disable: 4996) // warning C4996: The POSIX name for this item is deprecated. Instead, use the ISO C and C++ conformant name
-#  pragma warning(disable: 4702) // warning C4702: unreachable code
-#  pragma warning(disable: 4522) // warning C4522: multiple assignment operators specified
-#  pragma warning(disable: 4505) // warning C4505: 'PySlice_GetIndicesEx': unreferenced local function has been removed (PyPy only)
-#elif defined(__GNUG__) && !defined(__clang__)
+#elif defined(__GNUG__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #  pragma GCC diagnostic push
 #  pragma GCC diagnostic ignored "-Wunused-but-set-parameter"
-#  pragma GCC diagnostic ignored "-Wunused-but-set-variable"
-#  pragma GCC diagnostic ignored "-Wmissing-field-initializers"
-#  pragma GCC diagnostic ignored "-Wstrict-aliasing"
 #  pragma GCC diagnostic ignored "-Wattributes"
-#  if __GNUC__ >= 7
-#    pragma GCC diagnostic ignored "-Wnoexcept-type"
-#  endif
 #endif
 
 #include "attr.h"
+#include "gil.h"
 #include "options.h"
 #include "detail/class.h"
 #include "detail/init.h"
 
 #include <memory>
+#include <new>
 #include <vector>
 #include <string>
 #include <utility>
 
+#include <string.h>
+
+#if defined(__cpp_lib_launder) && !(defined(_MSC_VER) && (_MSC_VER < 1914))
+#  define PYBIND11_STD_LAUNDER std::launder
+#  define PYBIND11_HAS_STD_LAUNDER 1
+#else
+#  define PYBIND11_STD_LAUNDER
+#  define PYBIND11_HAS_STD_LAUNDER 0
+#endif
 #if defined(__GNUG__) && !defined(__clang__)
 #  include <cxxabi.h>
 #endif
 
+/* https://stackoverflow.com/questions/46798456/handling-gccs-noexcept-type-warning
+   This warning is about ABI compatibility, not code health.
+   It is only actually needed in a couple places, but apparently GCC 7 "generates this warning if
+   and only if the first template instantiation ... involves noexcept" [stackoverflow], therefore
+   it could get triggered from seemingly random places, depending on user code.
+   No other GCC version generates this warning.
+ */
+#if defined(__GNUC__) && __GNUC__ == 7
+#    pragma GCC diagnostic push
+#    pragma GCC diagnostic ignored "-Wnoexcept-type"
+#endif
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+#if defined(_MSC_VER)
+#    define PYBIND11_COMPAT_STRDUP _strdup
+#else
+#    define PYBIND11_COMPAT_STRDUP strdup
+#endif
+
 /// Wraps an arbitrary C++ function/method/lambda function/.. into a callable Python object
 class cpp_function : public function {
 public:
     cpp_function() = default;
     cpp_function(std::nullptr_t) { }
 
     /// Construct a cpp_function from a vanilla function pointer
@@ -138,24 +145,37 @@
         auto rec = unique_rec.get();
 
         /* Store the capture object directly in the function record if there is enough space */
         if (sizeof(capture) <= sizeof(rec->data)) {
             /* Without these pragmas, GCC warns that there might not be
                enough space to use the placement new operator. However, the
                'if' statement above ensures that this is the case. */
-#if defined(__GNUG__) && !defined(__clang__) && __GNUC__ >= 6
+#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #  pragma GCC diagnostic push
 #  pragma GCC diagnostic ignored "-Wplacement-new"
 #endif
             new ((capture *) &rec->data) capture { std::forward<Func>(f) };
-#if defined(__GNUG__) && !defined(__clang__) && __GNUC__ >= 6
+#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #  pragma GCC diagnostic pop
 #endif
+#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
+#  pragma GCC diagnostic push
+#  pragma GCC diagnostic ignored "-Wstrict-aliasing"
+#endif
+            // UB without std::launder, but without breaking ABI and/or
+            // a significant refactoring it's "impossible" to solve.
             if (!std::is_trivially_destructible<Func>::value)
-                rec->free_data = [](function_record *r) { ((capture *) &r->data)->~capture(); };
+                rec->free_data = [](function_record *r) {
+                    auto data = PYBIND11_STD_LAUNDER((capture *) &r->data);
+                    (void) data;
+                    data->~capture();
+                };
+#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
+#  pragma GCC diagnostic pop
+#endif
         } else {
             rec->data[0] = new capture { std::forward<Func>(f) };
             rec->free_data = [](function_record *r) { delete ((capture *) r->data[0]); };
         }
 
         /* Type casters for the function arguments and return value */
         using cast_in = argument_loader<Args...>;
@@ -238,15 +258,15 @@
     class strdup_guard {
     public:
         ~strdup_guard() {
             for (auto s : strings)
                 std::free(s);
         }
         char *operator()(const char *s) {
-            auto t = strdup(s);
+            auto t = PYBIND11_COMPAT_STRDUP(s);
             strings.push_back(t);
             return t;
         }
         void release() {
             strings.clear();
         }
     private:
@@ -276,15 +296,16 @@
                 a.name = guarded_strdup(a.name);
             if (a.descr)
                 a.descr = guarded_strdup(a.descr);
             else if (a.value)
                 a.descr = guarded_strdup(repr(a.value).cast<std::string>().c_str());
         }
 
-        rec->is_constructor = !strcmp(rec->name, "__init__") || !strcmp(rec->name, "__setstate__");
+        rec->is_constructor
+            = (strcmp(rec->name, "__init__") == 0) || (strcmp(rec->name, "__setstate__") == 0);
 
 #if !defined(NDEBUG) && !defined(PYBIND11_DISABLE_NEW_STYLE_INIT_WARNING)
         if (rec->is_constructor && !rec->is_new_style_constructor) {
             const auto class_name = detail::get_fully_qualified_tp_name((PyTypeObject *) rec->scope.ptr());
             const auto func_name = std::string(rec->name);
             PyErr_WarnEx(
                 PyExc_FutureWarning,
@@ -390,15 +411,16 @@
         }
 
         if (!chain) {
             /* No existing overload was found, create a new function object */
             rec->def = new PyMethodDef();
             std::memset(rec->def, 0, sizeof(PyMethodDef));
             rec->def->ml_name = rec->name;
-            rec->def->ml_meth = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*) (void)>(*dispatcher));
+            rec->def->ml_meth
+                = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*)()>(dispatcher));
             rec->def->ml_flags = METH_VARARGS | METH_KEYWORDS;
 
             capsule rec_capsule(unique_rec.release(), [](void *ptr) {
                 destruct((detail::function_record *) ptr);
             });
             guarded_strdup.release();
 
@@ -464,15 +486,15 @@
                 if (index > 0) signatures += "\n";
                 if (chain)
                     signatures += std::to_string(++index) + ". ";
                 signatures += rec->name;
                 signatures += it->signature;
                 signatures += "\n";
             }
-            if (it->doc && strlen(it->doc) > 0 && options::show_user_defined_docstrings()) {
+            if (it->doc && it->doc[0] != '\0' && options::show_user_defined_docstrings()) {
                 // If we're appending another docstring, and aren't printing function signatures, we
                 // need to append a newline first:
                 if (!options::show_function_signatures()) {
                     if (first_user_def) first_user_def = false;
                     else signatures += "\n";
                 }
                 if (options::show_function_signatures()) signatures += "\n";
@@ -481,15 +503,16 @@
             }
         }
 
         /* Install docstring */
         auto *func = (PyCFunctionObject *) m_ptr;
         std::free(const_cast<char *>(func->m_ml->ml_doc));
         // Install docstring if it's non-empty (when at least one option is enabled)
-        func->m_ml->ml_doc = signatures.empty() ? nullptr : strdup(signatures.c_str());
+        func->m_ml->ml_doc
+            = signatures.empty() ? nullptr : PYBIND11_COMPAT_STRDUP(signatures.c_str());
 
         if (rec->is_method) {
             m_ptr = PYBIND11_INSTANCE_METHOD_NEW(m_ptr, rec->scope.ptr());
             if (!m_ptr)
                 pybind11_fail("cpp_function::cpp_function(): Could not allocate instance method object");
             Py_DECREF(func);
         }
@@ -550,16 +573,16 @@
         const auto n_args_in = (size_t) PyTuple_GET_SIZE(args_in);
 
         handle parent = n_args_in > 0 ? PyTuple_GET_ITEM(args_in, 0) : nullptr,
                result = PYBIND11_TRY_NEXT_OVERLOAD;
 
         auto self_value_and_holder = value_and_holder();
         if (overloads->is_constructor) {
-            if (!PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
-                PyErr_SetString(PyExc_TypeError, "__init__(self, ...) called with invalid `self` argument");
+            if (!parent || !PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
+                PyErr_SetString(PyExc_TypeError, "__init__(self, ...) called with invalid or missing `self` argument");
                 return nullptr;
             }
 
             const auto tinfo = get_type_info((PyTypeObject *) overloads->scope.ptr());
             const auto pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder = pi->get_value_and_holder(tinfo, true);
 
@@ -630,15 +653,15 @@
                     ++args_copied;
                 }
 
                 // 1. Copy any position arguments given.
                 bool bad_arg = false;
                 for (; args_copied < args_to_copy; ++args_copied) {
                     const argument_record *arg_rec = args_copied < func.args.size() ? &func.args[args_copied] : nullptr;
-                    if (kwargs_in && arg_rec && arg_rec->name && PyDict_GetItemString(kwargs_in, arg_rec->name)) {
+                    if (kwargs_in && arg_rec && arg_rec->name && dict_getitemstring(kwargs_in, arg_rec->name)) {
                         bad_arg = true;
                         break;
                     }
 
                     handle arg(PyTuple_GET_ITEM(args_in, args_copied));
                     if (arg_rec && !arg_rec->none && arg.is_none()) {
                         bad_arg = true;
@@ -678,23 +701,25 @@
                     bool copied_kwargs = false;
 
                     for (; args_copied < num_args; ++args_copied) {
                         const auto &arg_rec = func.args[args_copied];
 
                         handle value;
                         if (kwargs_in && arg_rec.name)
-                            value = PyDict_GetItemString(kwargs.ptr(), arg_rec.name);
+                            value = dict_getitemstring(kwargs.ptr(), arg_rec.name);
 
                         if (value) {
                             // Consume a kwargs value
                             if (!copied_kwargs) {
                                 kwargs = reinterpret_steal<dict>(PyDict_Copy(kwargs.ptr()));
                                 copied_kwargs = true;
                             }
-                            PyDict_DelItemString(kwargs.ptr(), arg_rec.name);
+                            if (PyDict_DelItemString(kwargs.ptr(), arg_rec.name) == -1) {
+                                throw error_already_set();
+                            }
                         } else if (arg_rec.value) {
                             value = arg_rec.value;
                         }
 
                         if (!arg_rec.none && value.is_none()) {
                             break;
                         }
@@ -916,28 +941,28 @@
                     }
                 }
             }
 
             append_note_if_missing_header_is_suspected(msg);
             PyErr_SetString(PyExc_TypeError, msg.c_str());
             return nullptr;
-        } else if (!result) {
+        }
+        if (!result) {
             std::string msg = "Unable to convert function return value to a "
                               "Python type! The signature was\n\t";
             msg += it->signature;
             append_note_if_missing_header_is_suspected(msg);
             PyErr_SetString(PyExc_TypeError, msg.c_str());
             return nullptr;
-        } else {
-            if (overloads->is_constructor && !self_value_and_holder.holder_constructed()) {
-                auto *pi = reinterpret_cast<instance *>(parent.ptr());
-                self_value_and_holder.type->init_instance(pi, nullptr);
-            }
-            return result.ptr();
         }
+        if (overloads->is_constructor && !self_value_and_holder.holder_constructed()) {
+            auto *pi = reinterpret_cast<instance *>(parent.ptr());
+            self_value_and_holder.type->init_instance(pi, nullptr);
+        }
+        return result.ptr();
     }
 };
 
 /// Wrapper for Python extension modules
 class module_ : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(module_, object, PyModule_Check)
@@ -1081,15 +1106,16 @@
     PYBIND11_OBJECT_DEFAULT(generic_type, object, PyType_Check)
 protected:
     void initialize(const type_record &rec) {
         if (rec.scope && hasattr(rec.scope, "__dict__") && rec.scope.attr("__dict__").contains(rec.name))
             pybind11_fail("generic_type: cannot initialize type \"" + std::string(rec.name) +
                           "\": an object with that name is already defined");
 
-        if (rec.module_local ? get_local_type_info(*rec.type) : get_global_type_info(*rec.type))
+        if ((rec.module_local ? get_local_type_info(*rec.type) : get_global_type_info(*rec.type))
+            != nullptr)
             pybind11_fail("generic_type: type \"" + std::string(rec.name) +
                           "\" is already registered!");
 
         m_ptr = make_new_python_type(rec);
 
         /* Register supplemental type information in C++ dict */
         auto *tinfo = new detail::type_info();
@@ -1159,16 +1185,17 @@
         tinfo->get_buffer_data = get_buffer_data;
     }
 
     // rec_func must be set for either fget or fset.
     void def_property_static_impl(const char *name,
                                   handle fget, handle fset,
                                   detail::function_record *rec_func) {
-        const auto is_static = rec_func && !(rec_func->is_method && rec_func->scope);
-        const auto has_doc = rec_func && rec_func->doc && pybind11::options::show_user_defined_docstrings();
+        const auto is_static = (rec_func != nullptr) && !(rec_func->is_method && rec_func->scope);
+        const auto has_doc = (rec_func != nullptr) && (rec_func->doc != nullptr)
+                             && pybind11::options::show_user_defined_docstrings();
         auto property = handle((PyObject *) (is_static ? get_internals().static_property_type
                                                        : &PyProperty_Type));
         attr(name) = property(fget.ptr() ? fget : none(),
                               fset.ptr() ? fset : none(),
                               /*deleter*/none(),
                               pybind11::str(has_doc ? rec_func->doc : ""));
     }
@@ -1407,23 +1434,23 @@
         cpp_function fget([pm](const type &c) -> const D &{ return c.*pm; }, is_method(*this));
         def_property_readonly(name, fget, return_value_policy::reference_internal, extra...);
         return *this;
     }
 
     template <typename D, typename... Extra>
     class_ &def_readwrite_static(const char *name, D *pm, const Extra& ...extra) {
-        cpp_function fget([pm](object) -> const D &{ return *pm; }, scope(*this)),
-                     fset([pm](object, const D &value) { *pm = value; }, scope(*this));
+        cpp_function fget([pm](const object &) -> const D & { return *pm; }, scope(*this)),
+            fset([pm](const object &, const D &value) { *pm = value; }, scope(*this));
         def_property_static(name, fget, fset, return_value_policy::reference, extra...);
         return *this;
     }
 
     template <typename D, typename... Extra>
     class_ &def_readonly_static(const char *name, const D *pm, const Extra& ...extra) {
-        cpp_function fget([pm](object) -> const D &{ return *pm; }, scope(*this));
+        cpp_function fget([pm](const object &) -> const D & { return *pm; }, scope(*this));
         def_property_readonly_static(name, fget, return_value_policy::reference, extra...);
         return *this;
     }
 
     /// Uses return_value_policy::reference_internal by default
     template <typename Getter, typename... Extra>
     class_ &def_property_readonly(const char *name, const Getter &fget, const Extra& ...extra) {
@@ -1480,43 +1507,42 @@
         auto rec_fget = get_function_record(fget), rec_fset = get_function_record(fset);
         auto *rec_active = rec_fget;
         if (rec_fget) {
            char *doc_prev = rec_fget->doc; /* 'extra' field may include a property-specific documentation string */
            detail::process_attributes<Extra...>::init(extra..., rec_fget);
            if (rec_fget->doc && rec_fget->doc != doc_prev) {
               free(doc_prev);
-              rec_fget->doc = strdup(rec_fget->doc);
+              rec_fget->doc = PYBIND11_COMPAT_STRDUP(rec_fget->doc);
            }
         }
         if (rec_fset) {
             char *doc_prev = rec_fset->doc;
             detail::process_attributes<Extra...>::init(extra..., rec_fset);
             if (rec_fset->doc && rec_fset->doc != doc_prev) {
                 free(doc_prev);
-                rec_fset->doc = strdup(rec_fset->doc);
+                rec_fset->doc = PYBIND11_COMPAT_STRDUP(rec_fset->doc);
             }
             if (! rec_active) rec_active = rec_fset;
         }
         def_property_static_impl(name, fget, fset, rec_active);
         return *this;
     }
 
 private:
     /// Initialize holder object, variant 1: object derives from enable_shared_from_this
     template <typename T>
     static void init_holder(detail::instance *inst, detail::value_and_holder &v_h,
             const holder_type * /* unused */, const std::enable_shared_from_this<T> * /* dummy */) {
-        try {
-            auto sh = std::dynamic_pointer_cast<typename holder_type::element_type>(
-                    v_h.value_ptr<type>()->shared_from_this());
-            if (sh) {
-                new (std::addressof(v_h.holder<holder_type>())) holder_type(std::move(sh));
-                v_h.set_holder_constructed();
-            }
-        } catch (const std::bad_weak_ptr &) {}
+
+        auto sh = std::dynamic_pointer_cast<typename holder_type::element_type>(
+                detail::try_get_shared_from_this(v_h.value_ptr<type>()));
+        if (sh) {
+            new (std::addressof(v_h.holder<holder_type>())) holder_type(std::move(sh));
+            v_h.set_holder_constructed();
+        }
 
         if (!v_h.holder_constructed() && inst->owned) {
             new (std::addressof(v_h.holder<holder_type>())) holder_type(v_h.value_ptr<type>());
             v_h.set_holder_constructed();
         }
     }
 
@@ -1624,20 +1650,21 @@
 
     PYBIND11_NOINLINE void init(bool is_arithmetic, bool is_convertible) {
         m_base.attr("__entries") = dict();
         auto property = handle((PyObject *) &PyProperty_Type);
         auto static_property = handle((PyObject *) get_internals().static_property_type);
 
         m_base.attr("__repr__") = cpp_function(
-            [](object arg) -> str {
+            [](const object &arg) -> str {
                 handle type = type::handle_of(arg);
                 object type_name = type.attr("__name__");
                 return pybind11::str("<{}.{}: {}>").format(type_name, enum_name(arg), int_(arg));
-            }, name("__repr__"), is_method(m_base)
-        );
+            },
+            name("__repr__"),
+            is_method(m_base));
 
         m_base.attr("name") = property(cpp_function(&enum_name, name("name"), is_method(m_base)));
 
         m_base.attr("__str__") = cpp_function(
             [](handle arg) -> str {
                 object type_name = type::handle_of(arg).attr("__name__");
                 return pybind11::str("{}.{}").format(type_name, enum_name(arg));
@@ -1667,38 +1694,44 @@
                 dict entries = arg.attr("__entries"), m;
                 for (auto kv : entries)
                     m[kv.first] = kv.second[int_(0)];
                 return m;
             }, name("__members__")), none(), none(), ""
         );
 
-        #define PYBIND11_ENUM_OP_STRICT(op, expr, strict_behavior)                     \
-            m_base.attr(op) = cpp_function(                                            \
-                [](object a, object b) {                                               \
-                    if (!type::handle_of(a).is(type::handle_of(b)))                    \
-                        strict_behavior;                                               \
-                    return expr;                                                       \
-                },                                                                     \
-                name(op), is_method(m_base), arg("other"))
-
-        #define PYBIND11_ENUM_OP_CONV(op, expr)                                        \
-            m_base.attr(op) = cpp_function(                                            \
-                [](object a_, object b_) {                                             \
-                    int_ a(a_), b(b_);                                                 \
-                    return expr;                                                       \
-                },                                                                     \
-                name(op), is_method(m_base), arg("other"))
-
-        #define PYBIND11_ENUM_OP_CONV_LHS(op, expr)                                    \
-            m_base.attr(op) = cpp_function(                                            \
-                [](object a_, object b) {                                              \
-                    int_ a(a_);                                                        \
-                    return expr;                                                       \
-                },                                                                     \
-                name(op), is_method(m_base), arg("other"))
+#define PYBIND11_ENUM_OP_STRICT(op, expr, strict_behavior)                                        \
+    m_base.attr(op) = cpp_function(                                                               \
+        [](const object &a, const object &b) {                                                    \
+            if (!type::handle_of(a).is(type::handle_of(b)))                                       \
+                strict_behavior;                                                                  \
+            return expr;                                                                          \
+        },                                                                                        \
+        name(op),                                                                                 \
+        is_method(m_base),                                                                        \
+        arg("other"))
+
+#define PYBIND11_ENUM_OP_CONV(op, expr)                                                           \
+    m_base.attr(op) = cpp_function(                                                               \
+        [](const object &a_, const object &b_) {                                                  \
+            int_ a(a_), b(b_);                                                                    \
+            return expr;                                                                          \
+        },                                                                                        \
+        name(op),                                                                                 \
+        is_method(m_base),                                                                        \
+        arg("other"))
+
+#define PYBIND11_ENUM_OP_CONV_LHS(op, expr)                                                       \
+    m_base.attr(op) = cpp_function(                                                               \
+        [](const object &a_, const object &b) {                                                   \
+            int_ a(a_);                                                                           \
+            return expr;                                                                          \
+        },                                                                                        \
+        name(op),                                                                                 \
+        is_method(m_base),                                                                        \
+        arg("other"))
 
         if (is_convertible) {
             PYBIND11_ENUM_OP_CONV_LHS("__eq__", !b.is_none() &&  a.equal(b));
             PYBIND11_ENUM_OP_CONV_LHS("__ne__",  b.is_none() || !a.equal(b));
 
             if (is_arithmetic) {
                 PYBIND11_ENUM_OP_CONV("__lt__",   a <  b);
@@ -1707,16 +1740,18 @@
                 PYBIND11_ENUM_OP_CONV("__ge__",   a >= b);
                 PYBIND11_ENUM_OP_CONV("__and__",  a &  b);
                 PYBIND11_ENUM_OP_CONV("__rand__", a &  b);
                 PYBIND11_ENUM_OP_CONV("__or__",   a |  b);
                 PYBIND11_ENUM_OP_CONV("__ror__",  a |  b);
                 PYBIND11_ENUM_OP_CONV("__xor__",  a ^  b);
                 PYBIND11_ENUM_OP_CONV("__rxor__", a ^  b);
-                m_base.attr("__invert__") = cpp_function(
-                    [](object arg) { return ~(int_(arg)); }, name("__invert__"), is_method(m_base));
+                m_base.attr("__invert__")
+                    = cpp_function([](const object &arg) { return ~(int_(arg)); },
+                                   name("__invert__"),
+                                   is_method(m_base));
             }
         } else {
             PYBIND11_ENUM_OP_STRICT("__eq__",  int_(a).equal(int_(b)), return false);
             PYBIND11_ENUM_OP_STRICT("__ne__", !int_(a).equal(int_(b)), return true);
 
             if (is_arithmetic) {
                 #define PYBIND11_THROW throw type_error("Expected an enumeration of matching type!");
@@ -1729,18 +1764,18 @@
         }
 
         #undef PYBIND11_ENUM_OP_CONV_LHS
         #undef PYBIND11_ENUM_OP_CONV
         #undef PYBIND11_ENUM_OP_STRICT
 
         m_base.attr("__getstate__") = cpp_function(
-            [](object arg) { return int_(arg); }, name("__getstate__"), is_method(m_base));
+            [](const object &arg) { return int_(arg); }, name("__getstate__"), is_method(m_base));
 
         m_base.attr("__hash__") = cpp_function(
-            [](object arg) { return int_(arg); }, name("__hash__"), is_method(m_base));
+            [](const object &arg) { return int_(arg); }, name("__hash__"), is_method(m_base));
     }
 
     PYBIND11_NOINLINE void value(char const* name_, object value, const char *doc = nullptr) {
         dict entries = m_base.attr("__entries");
         str name(name_);
         if (entries.contains(name)) {
             std::string type_name = (std::string) str(m_base.attr("__name__"));
@@ -1844,17 +1879,17 @@
     }
 }
 
 PYBIND11_NOINLINE inline void keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret) {
     auto get_arg = [&](size_t n) {
         if (n == 0)
             return ret;
-        else if (n == 1 && call.init_self)
+        if (n == 1 && call.init_self)
             return call.init_self;
-        else if (n <= call.args.size())
+        if (n <= call.args.size())
             return call.args[n - 1];
         return handle();
     };
 
     keep_alive_impl(get_arg(Nurse), get_arg(Patient));
 }
 
@@ -1886,15 +1921,17 @@
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Makes a python iterator from a first and past-the-end C++ InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
+#ifndef DOXYGEN_SHOULD_SKIP_THIS  // Issue in breathe 4.26.1
           typename ValueType = decltype(*std::declval<Iterator>()),
+#endif
           typename... Extra>
 iterator make_iterator(Iterator first, Sentinel last, Extra &&... extra) {
     using state = detail::iterator_state<Iterator, Sentinel, false, Policy>;
 
     if (!detail::get_type_info(typeid(state), false)) {
         class_<state>(handle(), "iterator", pybind11::module_local())
             .def("__iter__", [](state &s) -> state& { return s; })
@@ -1915,15 +1952,17 @@
 }
 
 /// Makes an python iterator over the keys (`.first`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
+#ifndef DOXYGEN_SHOULD_SKIP_THIS  // Issue in breathe 4.26.1
           typename KeyType = decltype((*std::declval<Iterator>()).first),
+#endif
           typename... Extra>
 iterator make_key_iterator(Iterator first, Sentinel last, Extra &&... extra) {
     using state = detail::iterator_state<Iterator, Sentinel, true, Policy>;
 
     if (!detail::get_type_info(typeid(state), false)) {
         class_<state>(handle(), "iterator", pybind11::module_local())
             .def("__iter__", [](state &s) -> state& { return s; })
@@ -2046,15 +2085,15 @@
             detail::get_exception_object<CppException>()(e.what());
         }
     });
     return ex;
 }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
-PYBIND11_NOINLINE inline void print(tuple args, dict kwargs) {
+PYBIND11_NOINLINE inline void print(const tuple &args, const dict &kwargs) {
     auto strings = tuple(args.size());
     for (size_t i = 0; i < args.size(); ++i) {
         strings[i] = str(args[i]);
     }
     auto sep = kwargs.contains("sep") ? kwargs["sep"] : cast(" ");
     auto line = sep.attr("join")(strings);
 
@@ -2084,181 +2123,14 @@
 
 template <return_value_policy policy = return_value_policy::automatic_reference, typename... Args>
 void print(Args &&...args) {
     auto c = detail::collect_arguments<policy>(std::forward<Args>(args)...);
     detail::print(c.args(), c.kwargs());
 }
 
-#if defined(WITH_THREAD) && !defined(PYPY_VERSION)
-
-/* The functions below essentially reproduce the PyGILState_* API using a RAII
- * pattern, but there are a few important differences:
- *
- * 1. When acquiring the GIL from an non-main thread during the finalization
- *    phase, the GILState API blindly terminates the calling thread, which
- *    is often not what is wanted. This API does not do this.
- *
- * 2. The gil_scoped_release function can optionally cut the relationship
- *    of a PyThreadState and its associated thread, which allows moving it to
- *    another thread (this is a fairly rare/advanced use case).
- *
- * 3. The reference count of an acquired thread state can be controlled. This
- *    can be handy to prevent cases where callbacks issued from an external
- *    thread would otherwise constantly construct and destroy thread state data
- *    structures.
- *
- * See the Python bindings of NanoGUI (http://github.com/wjakob/nanogui) for an
- * example which uses features 2 and 3 to migrate the Python thread of
- * execution to another thread (to run the event loop on the original thread,
- * in this case).
- */
-
-class gil_scoped_acquire {
-public:
-    PYBIND11_NOINLINE gil_scoped_acquire() {
-        auto const &internals = detail::get_internals();
-        tstate = (PyThreadState *) PYBIND11_TLS_GET_VALUE(internals.tstate);
-
-        if (!tstate) {
-            /* Check if the GIL was acquired using the PyGILState_* API instead (e.g. if
-               calling from a Python thread). Since we use a different key, this ensures
-               we don't create a new thread state and deadlock in PyEval_AcquireThread
-               below. Note we don't save this state with internals.tstate, since we don't
-               create it we would fail to clear it (its reference count should be > 0). */
-            tstate = PyGILState_GetThisThreadState();
-        }
-
-        if (!tstate) {
-            tstate = PyThreadState_New(internals.istate);
-            #if !defined(NDEBUG)
-                if (!tstate)
-                    pybind11_fail("scoped_acquire: could not create thread state!");
-            #endif
-            tstate->gilstate_counter = 0;
-            PYBIND11_TLS_REPLACE_VALUE(internals.tstate, tstate);
-        } else {
-            release = detail::get_thread_state_unchecked() != tstate;
-        }
-
-        if (release) {
-            PyEval_AcquireThread(tstate);
-        }
-
-        inc_ref();
-    }
-
-    void inc_ref() {
-        ++tstate->gilstate_counter;
-    }
-
-    PYBIND11_NOINLINE void dec_ref() {
-        --tstate->gilstate_counter;
-        #if !defined(NDEBUG)
-            if (detail::get_thread_state_unchecked() != tstate)
-                pybind11_fail("scoped_acquire::dec_ref(): thread state must be current!");
-            if (tstate->gilstate_counter < 0)
-                pybind11_fail("scoped_acquire::dec_ref(): reference count underflow!");
-        #endif
-        if (tstate->gilstate_counter == 0) {
-            #if !defined(NDEBUG)
-                if (!release)
-                    pybind11_fail("scoped_acquire::dec_ref(): internal error!");
-            #endif
-            PyThreadState_Clear(tstate);
-            if (active)
-                PyThreadState_DeleteCurrent();
-            PYBIND11_TLS_DELETE_VALUE(detail::get_internals().tstate);
-            release = false;
-        }
-    }
-
-    /// This method will disable the PyThreadState_DeleteCurrent call and the
-    /// GIL won't be acquired. This method should be used if the interpreter
-    /// could be shutting down when this is called, as thread deletion is not
-    /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
-    /// protect subsequent code.
-    PYBIND11_NOINLINE void disarm() {
-        active = false;
-    }
-
-    PYBIND11_NOINLINE ~gil_scoped_acquire() {
-        dec_ref();
-        if (release)
-           PyEval_SaveThread();
-    }
-private:
-    PyThreadState *tstate = nullptr;
-    bool release = true;
-    bool active = true;
-};
-
-class gil_scoped_release {
-public:
-    explicit gil_scoped_release(bool disassoc = false) : disassoc(disassoc) {
-        // `get_internals()` must be called here unconditionally in order to initialize
-        // `internals.tstate` for subsequent `gil_scoped_acquire` calls. Otherwise, an
-        // initialization race could occur as multiple threads try `gil_scoped_acquire`.
-        const auto &internals = detail::get_internals();
-        tstate = PyEval_SaveThread();
-        if (disassoc) {
-            auto key = internals.tstate;
-            PYBIND11_TLS_DELETE_VALUE(key);
-        }
-    }
-
-    /// This method will disable the PyThreadState_DeleteCurrent call and the
-    /// GIL won't be acquired. This method should be used if the interpreter
-    /// could be shutting down when this is called, as thread deletion is not
-    /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
-    /// protect subsequent code.
-    PYBIND11_NOINLINE void disarm() {
-        active = false;
-    }
-
-    ~gil_scoped_release() {
-        if (!tstate)
-            return;
-        // `PyEval_RestoreThread()` should not be called if runtime is finalizing
-        if (active)
-            PyEval_RestoreThread(tstate);
-        if (disassoc) {
-            auto key = detail::get_internals().tstate;
-            PYBIND11_TLS_REPLACE_VALUE(key, tstate);
-        }
-    }
-private:
-    PyThreadState *tstate;
-    bool disassoc;
-    bool active = true;
-};
-#elif defined(PYPY_VERSION)
-class gil_scoped_acquire {
-    PyGILState_STATE state;
-public:
-    gil_scoped_acquire() { state = PyGILState_Ensure(); }
-    ~gil_scoped_acquire() { PyGILState_Release(state); }
-    void disarm() {}
-};
-
-class gil_scoped_release {
-    PyThreadState *state;
-public:
-    gil_scoped_release() { state = PyEval_SaveThread(); }
-    ~gil_scoped_release() { PyEval_RestoreThread(state); }
-    void disarm() {}
-};
-#else
-class gil_scoped_acquire {
-    void disarm() {}
-};
-class gil_scoped_release {
-    void disarm() {}
-};
-#endif
-
 error_already_set::~error_already_set() {
     if (m_type) {
         gil_scoped_acquire gil;
         error_scope scope;
         m_type.release().dec_ref();
         m_value.release().dec_ref();
         m_trace.release().dec_ref();
@@ -2285,18 +2157,18 @@
         return function();
     }
 
     /* Don't call dispatch code if invoked from overridden function.
        Unfortunately this doesn't work on PyPy. */
 #if !defined(PYPY_VERSION)
     PyFrameObject *frame = PyThreadState_Get()->frame;
-    if (frame && (std::string) str(frame->f_code->co_name) == name &&
-        frame->f_code->co_argcount > 0) {
+    if (frame != nullptr && (std::string) str(frame->f_code->co_name) == name
+        && frame->f_code->co_argcount > 0) {
         PyFrame_FastToLocals(frame);
-        PyObject *self_caller = PyDict_GetItem(
+        PyObject *self_caller = dict_getitem(
             frame->f_locals, PyTuple_GET_ITEM(frame->f_code->co_varnames, 0));
         if (self_caller == self.ptr())
             return function();
     }
 #else
     /* PyPy currently doesn't provide a detailed cpyext emulation of
        frame objects, so we have to emulate this using Python. This
@@ -2333,26 +2205,27 @@
   :return: The Python method by this name from the object or an empty function wrapper.
  \endrst */
 template <class T> function get_override(const T *this_ptr, const char *name) {
     auto tinfo = detail::get_type_info(typeid(T));
     return tinfo ? detail::get_type_override(this_ptr, tinfo, name) : function();
 }
 
-#define PYBIND11_OVERRIDE_IMPL(ret_type, cname, name, ...) \
-    do { \
-        pybind11::gil_scoped_acquire gil; \
-        pybind11::function override = pybind11::get_override(static_cast<const cname *>(this), name); \
-        if (override) { \
-            auto o = override(__VA_ARGS__); \
-            if (pybind11::detail::cast_is_temporary_value_reference<ret_type>::value) { \
-                static pybind11::detail::override_caster_t<ret_type> caster; \
-                return pybind11::detail::cast_ref<ret_type>(std::move(o), caster); \
-            } \
-            else return pybind11::detail::cast_safe<ret_type>(std::move(o)); \
-        } \
+#define PYBIND11_OVERRIDE_IMPL(ret_type, cname, name, ...)                                        \
+    do {                                                                                          \
+        pybind11::gil_scoped_acquire gil;                                                         \
+        pybind11::function override                                                               \
+            = pybind11::get_override(static_cast<const cname *>(this), name);                     \
+        if (override) {                                                                           \
+            auto o = override(__VA_ARGS__);                                                       \
+            if (pybind11::detail::cast_is_temporary_value_reference<ret_type>::value) {           \
+                static pybind11::detail::override_caster_t<ret_type> caster;                      \
+                return pybind11::detail::cast_ref<ret_type>(std::move(o), caster);                \
+            }                                                                                     \
+            return pybind11::detail::cast_safe<ret_type>(std::move(o));                           \
+        }                                                                                         \
     } while (false)
 
 /** \rst
     Macro to populate the virtual method in the trampoline class. This macro tries to look up a method named 'fn'
     from the Python side, deals with the :ref:`gil` and necessary argument conversions to call this method and return
     the appropriate type. See :ref:`overriding_virtuals` for more information. This macro should be used when the method
     name in C is not the same as the method name in Python. For example with `__str__`.
@@ -2440,12 +2313,16 @@
 #define PYBIND11_OVERLOAD(ret_type, cname, fn, ...) \
     PYBIND11_OVERRIDE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__)
 #define PYBIND11_OVERLOAD_PURE(ret_type, cname, fn, ...) \
     PYBIND11_OVERRIDE_PURE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__);
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
 
+#if defined(__GNUC__) && __GNUC__ == 7
+#    pragma GCC diagnostic pop // -Wnoexcept-type
+#endif
+
 #if defined(_MSC_VER) && !defined(__INTEL_COMPILER)
 #  pragma warning(pop)
-#elif defined(__GNUG__) && !defined(__clang__)
+#elif defined(__GNUG__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #  pragma GCC diagnostic pop
 #endif
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/pytypes.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/pytypes.h`

 * *Files 4% similar despite different names*

```diff
@@ -275,16 +275,18 @@
     template <typename T> T cast() &&;
 
 protected:
     // Tags for choosing constructors from raw PyObject *
     struct borrowed_t { };
     struct stolen_t { };
 
+#ifndef DOXYGEN_SHOULD_SKIP_THIS  // Issue in breathe 4.26.1
     template <typename T> friend T reinterpret_borrow(handle);
     template <typename T> friend T reinterpret_steal(handle);
+#endif
 
 public:
     // Only accessible from derived classes and the reinterpret_* functions
     object(handle h, borrowed_t) : handle(h) { inc_ref(); }
     object(handle h, stolen_t) : handle(h) { }
 };
 
@@ -313,19 +315,23 @@
 \endrst */
 template <typename T> T reinterpret_steal(handle h) { return {h, object::stolen_t{}}; }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 inline std::string error_string();
 PYBIND11_NAMESPACE_END(detail)
 
+#if defined(_MSC_VER)
+#  pragma warning(push)
+#  pragma warning(disable: 4275 4251) // warning C4275: An exported class was derived from a class that wasn't exported. Can be ignored when derived from a STL class.
+#endif
 /// Fetch and hold an error which was already set in Python.  An instance of this is typically
 /// thrown to propagate python-side errors back through C++ which can either be caught manually or
 /// else falls back to the function dispatcher (which then raises the captured error back to
 /// python).
-class error_already_set : public std::runtime_error {
+class PYBIND11_EXPORT_EXCEPTION error_already_set : public std::runtime_error {
 public:
     /// Constructs a new exception from the current Python error indicator, if any.  The current
     /// Python error indicator will be cleared.
     error_already_set() : std::runtime_error(detail::error_string()) {
         PyErr_Fetch(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
     }
 
@@ -335,44 +341,50 @@
     inline ~error_already_set() override;
 
     /// Give the currently-held error back to Python, if any.  If there is currently a Python error
     /// already set it is cleared first.  After this call, the current object no longer stores the
     /// error variables (but the `.what()` string is still available).
     void restore() { PyErr_Restore(m_type.release().ptr(), m_value.release().ptr(), m_trace.release().ptr()); }
 
-    /// If it is impossible to raise the currently-held error, such as in destructor, we can write
-    /// it out using Python's unraisable hook (sys.unraisablehook). The error context should be
-    /// some object whose repr() helps identify the location of the error. Python already knows the
-    /// type and value of the error, so there is no need to repeat that. For example, __func__ could
-    /// be helpful. After this call, the current object no longer stores the error variables,
-    /// and neither does Python.
+    /// If it is impossible to raise the currently-held error, such as in a destructor, we can write
+    /// it out using Python's unraisable hook (`sys.unraisablehook`). The error context should be
+    /// some object whose `repr()` helps identify the location of the error. Python already knows the
+    /// type and value of the error, so there is no need to repeat that. After this call, the current
+    /// object no longer stores the error variables, and neither does Python.
     void discard_as_unraisable(object err_context) {
         restore();
         PyErr_WriteUnraisable(err_context.ptr());
     }
+    /// An alternate version of `discard_as_unraisable()`, where a string provides information on the
+    /// location of the error. For example, `__func__` could be helpful.
     void discard_as_unraisable(const char *err_context) {
         discard_as_unraisable(reinterpret_steal<object>(PYBIND11_FROM_STRING(err_context)));
     }
 
     // Does nothing; provided for backwards compatibility.
     PYBIND11_DEPRECATED("Use of error_already_set.clear() is deprecated")
     void clear() {}
 
     /// Check if the currently trapped error type matches the given Python exception class (or a
     /// subclass thereof).  May also be passed a tuple to search for any exception class matches in
     /// the given tuple.
-    bool matches(handle exc) const { return PyErr_GivenExceptionMatches(m_type.ptr(), exc.ptr()); }
+    bool matches(handle exc) const {
+        return (PyErr_GivenExceptionMatches(m_type.ptr(), exc.ptr()) != 0);
+    }
 
     const object& type() const { return m_type; }
     const object& value() const { return m_value; }
     const object& trace() const { return m_trace; }
 
 private:
     object m_type, m_value, m_trace;
 };
+#if defined(_MSC_VER)
+#  pragma warning(pop)
+#endif
 
 /** \defgroup python_builtins _
     Unless stated otherwise, the following C++ functions behave the same
     as their Python counterparts.
  */
 
 /** \ingroup python_builtins
@@ -427,27 +439,25 @@
     if (!result) { throw error_already_set(); }
     return reinterpret_steal<object>(result);
 }
 
 inline object getattr(handle obj, handle name, handle default_) {
     if (PyObject *result = PyObject_GetAttr(obj.ptr(), name.ptr())) {
         return reinterpret_steal<object>(result);
-    } else {
-        PyErr_Clear();
-        return reinterpret_borrow<object>(default_);
     }
+    PyErr_Clear();
+    return reinterpret_borrow<object>(default_);
 }
 
 inline object getattr(handle obj, const char *name, handle default_) {
     if (PyObject *result = PyObject_GetAttrString(obj.ptr(), name)) {
         return reinterpret_steal<object>(result);
-    } else {
-        PyErr_Clear();
-        return reinterpret_borrow<object>(default_);
     }
+    PyErr_Clear();
+    return reinterpret_borrow<object>(default_);
 }
 
 inline void setattr(handle obj, handle name, handle value) {
     if (PyObject_SetAttr(obj.ptr(), name.ptr(), value.ptr()) != 0) { throw error_already_set(); }
 }
 
 inline void setattr(handle obj, const char *name, handle value) {
@@ -472,33 +482,74 @@
 #endif
         if (PyMethod_Check(value.ptr()))
             value = PyMethod_GET_FUNCTION(value.ptr());
     }
     return value;
 }
 
+// Reimplementation of python's dict helper functions to ensure that exceptions
+// aren't swallowed (see #2862)
+
+// copied from cpython _PyDict_GetItemStringWithError
+inline PyObject * dict_getitemstring(PyObject *v, const char *key)
+{
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kv = nullptr, *rv = nullptr;
+    kv = PyUnicode_FromString(key);
+    if (kv == NULL) {
+        throw error_already_set();
+    }
+
+    rv = PyDict_GetItemWithError(v, kv);
+    Py_DECREF(kv);
+    if (rv == NULL && PyErr_Occurred()) {
+        throw error_already_set();
+    }
+    return rv;
+#else
+    return PyDict_GetItemString(v, key);
+#endif
+}
+
+inline PyObject * dict_getitem(PyObject *v, PyObject *key)
+{
+#if PY_MAJOR_VERSION >= 3
+    PyObject *rv = PyDict_GetItemWithError(v, key);
+    if (rv == NULL && PyErr_Occurred()) {
+        throw error_already_set();
+    }
+    return rv;
+#else
+    return PyDict_GetItem(v, key);
+#endif
+}
+
 // Helper aliases/functions to support implicit casting of values given to python accessors/methods.
 // When given a pyobject, this simply returns the pyobject as-is; for other C++ type, the value goes
 // through pybind11::cast(obj) to convert it to an `object`.
 template <typename T, enable_if_t<is_pyobject<T>::value, int> = 0>
 auto object_or_cast(T &&o) -> decltype(std::forward<T>(o)) { return std::forward<T>(o); }
 // The following casting version is implemented in cast.h:
 template <typename T, enable_if_t<!is_pyobject<T>::value, int> = 0>
 object object_or_cast(T &&o);
 // Match a PyObject*, which we want to convert directly to handle via its converting constructor
 inline handle object_or_cast(PyObject *ptr) { return ptr; }
 
+#if defined(_MSC_VER) && _MSC_VER < 1920
+#  pragma warning(push)
+#  pragma warning(disable: 4522) // warning C4522: multiple assignment operators specified
+#endif
 template <typename Policy>
 class accessor : public object_api<accessor<Policy>> {
     using key_type = typename Policy::key_type;
 
 public:
     accessor(handle obj, key_type key) : obj(obj), key(std::move(key)) { }
     accessor(const accessor &) = default;
-    accessor(accessor &&) = default;
+    accessor(accessor &&) noexcept = default;
 
     // accessor overload required to override default assignment operator (templates are not allowed
     // to replace default compiler-generated assignments).
     void operator=(const accessor &a) && { std::move(*this).operator=(handle(a)); }
     void operator=(const accessor &a) & { operator=(handle(a)); }
 
     template <typename T> void operator=(T &&value) && {
@@ -531,14 +582,17 @@
     }
 
 private:
     handle obj;
     key_type key;
     mutable object cache;
 };
+#if defined(_MSC_VER) && _MSC_VER < 1920
+#  pragma warning(pop)
+#endif
 
 PYBIND11_NAMESPACE_BEGIN(accessor_policies)
 struct obj_attr {
     using key_type = object;
     static object get(handle obj, handle key) { return getattr(obj, key); }
     static void set(handle obj, handle key, handle val) { setattr(obj, key, val); }
 };
@@ -715,15 +769,19 @@
     using reference = const value_type;
     using pointer = arrow_proxy<const value_type>;
 
     dict_readonly() = default;
     dict_readonly(handle obj, ssize_t pos) : obj(obj), pos(pos) { increment(); }
 
     reference dereference() const { return {key, value}; }
-    void increment() { if (!PyDict_Next(obj.ptr(), &pos, &key, &value)) { pos = -1; } }
+    void increment() {
+        if (PyDict_Next(obj.ptr(), &pos, &key, &value) == 0) {
+            pos = -1;
+        }
+    }
     bool equal(const dict_readonly &b) const { return pos == b.pos; }
 
 private:
     handle obj;
     PyObject *key = nullptr, *value = nullptr;
     ssize_t pos = -1;
 };
@@ -741,24 +799,28 @@
 using dict_iterator = generic_iterator<iterator_policies::dict_readonly>;
 
 inline bool PyIterable_Check(PyObject *obj) {
     PyObject *iter = PyObject_GetIter(obj);
     if (iter) {
         Py_DECREF(iter);
         return true;
-    } else {
-        PyErr_Clear();
-        return false;
     }
+    PyErr_Clear();
+    return false;
 }
 
 inline bool PyNone_Check(PyObject *o) { return o == Py_None; }
 inline bool PyEllipsis_Check(PyObject *o) { return o == Py_Ellipsis; }
 
+#ifdef PYBIND11_STR_LEGACY_PERMISSIVE
 inline bool PyUnicode_Check_Permissive(PyObject *o) { return PyUnicode_Check(o) || PYBIND11_BYTES_CHECK(o); }
+#define PYBIND11_STR_CHECK_FUN detail::PyUnicode_Check_Permissive
+#else
+#define PYBIND11_STR_CHECK_FUN PyUnicode_Check
+#endif
 
 inline bool PyStaticMethod_Check(PyObject *o) { return o->ob_type == &PyStaticMethod_Type; }
 
 class kwargs_proxy : public handle {
 public:
     explicit kwargs_proxy(handle h) : handle(h) { }
 };
@@ -793,29 +855,33 @@
 #define PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
     public: \
         PYBIND11_DEPRECATED("Use reinterpret_borrow<"#Name">() or reinterpret_steal<"#Name">()") \
         Name(handle h, bool is_borrowed) : Parent(is_borrowed ? Parent(h, borrowed_t{}) : Parent(h, stolen_t{})) { } \
         Name(handle h, borrowed_t) : Parent(h, borrowed_t{}) { } \
         Name(handle h, stolen_t) : Parent(h, stolen_t{}) { } \
         PYBIND11_DEPRECATED("Use py::isinstance<py::python_type>(obj) instead") \
-        bool check() const { return m_ptr != nullptr && (bool) CheckFun(m_ptr); } \
+        bool check() const { return m_ptr != nullptr && (CheckFun(m_ptr) != 0); } \
         static bool check_(handle h) { return h.ptr() != nullptr && CheckFun(h.ptr()); } \
         template <typename Policy_> \
         Name(const ::pybind11::detail::accessor<Policy_> &a) : Name(object(a)) { }
 
 #define PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun) \
     PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
     /* This is deliberately not 'explicit' to allow implicit conversion from object: */ \
     Name(const object &o) \
     : Parent(check_(o) ? o.inc_ref().ptr() : ConvertFun(o.ptr()), stolen_t{}) \
     { if (!m_ptr) throw error_already_set(); } \
     Name(object &&o) \
     : Parent(check_(o) ? o.release().ptr() : ConvertFun(o.ptr()), stolen_t{}) \
     { if (!m_ptr) throw error_already_set(); }
 
+#define PYBIND11_OBJECT_CVT_DEFAULT(Name, Parent, CheckFun, ConvertFun) \
+    PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun) \
+    Name() : Parent() { }
+
 #define PYBIND11_OBJECT_CHECK_FAILED(Name, o_ptr) \
     ::pybind11::type_error("Object of type '" + \
                            ::pybind11::detail::get_fully_qualified_tp_name(Py_TYPE(o_ptr)) + \
                            "' is not an instance of '" #Name "'")
 
 #define PYBIND11_OBJECT(Name, Parent, CheckFun) \
     PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
@@ -930,15 +996,15 @@
     PYBIND11_OBJECT_DEFAULT(iterable, object, detail::PyIterable_Check)
 };
 
 class bytes;
 
 class str : public object {
 public:
-    PYBIND11_OBJECT_CVT(str, object, detail::PyUnicode_Check_Permissive, raw_str)
+    PYBIND11_OBJECT_CVT(str, object, PYBIND11_STR_CHECK_FUN, raw_str)
 
     str(const char *c, size_t n)
         : object(PyUnicode_FromStringAndSize(c, (ssize_t) n), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate string object!");
     }
 
     // 'explicit' is explicitly omitted from the following constructors to allow implicit conversion to py::str from C++ string-like objects
@@ -958,18 +1024,18 @@
     explicit str(handle h) : object(raw_str(h.ptr()), stolen_t{}) { if (!m_ptr) throw error_already_set(); }
 
     operator std::string() const {
         object temp = *this;
         if (PyUnicode_Check(m_ptr)) {
             temp = reinterpret_steal<object>(PyUnicode_AsUTF8String(m_ptr));
             if (!temp)
-                pybind11_fail("Unable to extract string contents! (encoding issue)");
+                throw error_already_set();
         }
-        char *buffer;
-        ssize_t length;
+        char *buffer = nullptr;
+        ssize_t length = 0;
         if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length))
             pybind11_fail("Unable to extract string contents! (invalid type)");
         return std::string(buffer, (size_t) length);
     }
 
     template <typename... Args>
     str format(Args &&...args) const {
@@ -1016,16 +1082,16 @@
 
     // Allow implicit conversion:
     bytes(const std::string &s) : bytes(s.data(), s.size()) { }
 
     explicit bytes(const pybind11::str &s);
 
     operator std::string() const {
-        char *buffer;
-        ssize_t length;
+        char *buffer = nullptr;
+        ssize_t length = 0;
         if (PYBIND11_BYTES_AS_STRING_AND_SIZE(m_ptr, &buffer, &length))
             pybind11_fail("Unable to extract bytes contents!");
         return std::string(buffer, (size_t) length);
     }
 };
 // Note: breathe >= 4.17.0 will fail to build docs if the below two constructors
 // are included in the doxygen group; close here and reopen after as a workaround
@@ -1034,37 +1100,65 @@
 inline bytes::bytes(const pybind11::str &s) {
     object temp = s;
     if (PyUnicode_Check(s.ptr())) {
         temp = reinterpret_steal<object>(PyUnicode_AsUTF8String(s.ptr()));
         if (!temp)
             pybind11_fail("Unable to extract string contents! (encoding issue)");
     }
-    char *buffer;
-    ssize_t length;
+    char *buffer = nullptr;
+    ssize_t length = 0;
     if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length))
         pybind11_fail("Unable to extract string contents! (invalid type)");
     auto obj = reinterpret_steal<object>(PYBIND11_BYTES_FROM_STRING_AND_SIZE(buffer, length));
     if (!obj)
         pybind11_fail("Could not allocate bytes object!");
     m_ptr = obj.release().ptr();
 }
 
 inline str::str(const bytes& b) {
-    char *buffer;
-    ssize_t length;
+    char *buffer = nullptr;
+    ssize_t length = 0;
     if (PYBIND11_BYTES_AS_STRING_AND_SIZE(b.ptr(), &buffer, &length))
         pybind11_fail("Unable to extract bytes contents!");
     auto obj = reinterpret_steal<object>(PyUnicode_FromStringAndSize(buffer, (ssize_t) length));
     if (!obj)
         pybind11_fail("Could not allocate string object!");
     m_ptr = obj.release().ptr();
 }
 
 /// \addtogroup pytypes
 /// @{
+class bytearray : public object {
+public:
+    PYBIND11_OBJECT_CVT(bytearray, object, PyByteArray_Check, PyByteArray_FromObject)
+
+    bytearray(const char *c, size_t n)
+        : object(PyByteArray_FromStringAndSize(c, (ssize_t) n), stolen_t{}) {
+        if (!m_ptr) pybind11_fail("Could not allocate bytearray object!");
+    }
+
+    bytearray()
+        : bytearray("", 0) {}
+
+    explicit bytearray(const std::string &s) : bytearray(s.data(), s.size()) { }
+
+    size_t size() const { return static_cast<size_t>(PyByteArray_Size(m_ptr)); }
+
+    explicit operator std::string() const {
+        char *buffer = PyByteArray_AS_STRING(m_ptr);
+        ssize_t size = PyByteArray_GET_SIZE(m_ptr);
+        return std::string(buffer, static_cast<size_t>(size));
+    }
+};
+// Note: breathe >= 4.17.0 will fail to build docs if the below two constructors
+// are included in the doxygen group; close here and reopen after as a workaround
+/// @} pytypes
+
+/// \addtogroup pytypes
+/// @{
 class none : public object {
 public:
     PYBIND11_OBJECT(none, object, detail::PyNone_Check)
     none() : object(Py_None, borrowed_t{}) { }
 };
 
 class ellipsis : public object {
@@ -1075,22 +1169,22 @@
 
 class bool_ : public object {
 public:
     PYBIND11_OBJECT_CVT(bool_, object, PyBool_Check, raw_bool)
     bool_() : object(Py_False, borrowed_t{}) { }
     // Allow implicit conversion from and to `bool`:
     bool_(bool value) : object(value ? Py_True : Py_False, borrowed_t{}) { }
-    operator bool() const { return m_ptr && PyLong_AsLong(m_ptr) != 0; }
+    operator bool() const { return (m_ptr != nullptr) && PyLong_AsLong(m_ptr) != 0; }
 
 private:
     /// Return the truth value of an object -- always returns a new reference
     static PyObject *raw_bool(PyObject *op) {
         const auto value = PyObject_IsTrue(op);
         if (value == -1) return nullptr;
-        return handle(value ? Py_True : Py_False).inc_ref().ptr();
+        return handle(value != 0 ? Py_True : Py_False).inc_ref().ptr();
     }
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Converts a value to the given unsigned type.  If an error occurs, you get back (Unsigned) -1;
 // otherwise you get back the unsigned long or unsigned long long value cast to (Unsigned).
 // (The distinction is critically important when casting a returned -1 error value to some other
@@ -1101,18 +1195,16 @@
 #if PY_VERSION_HEX < 0x03000000
             || PyInt_Check(o)
 #endif
     ) {
         unsigned long v = PyLong_AsUnsignedLong(o);
         return v == (unsigned long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
     }
-    else {
-        unsigned long long v = PyLong_AsUnsignedLongLong(o);
-        return v == (unsigned long long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
-    }
+    unsigned long long v = PyLong_AsUnsignedLongLong(o);
+    return v == (unsigned long long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
 }
 PYBIND11_NAMESPACE_END(detail)
 
 class int_ : public object {
 public:
     PYBIND11_OBJECT_CVT(int_, object, PYBIND11_LONG_CHECK, PyNumber_Long)
     int_() : object(PyLong_FromLong(0), stolen_t{}) { }
@@ -1157,19 +1249,24 @@
     }
     operator float() const { return (float) PyFloat_AsDouble(m_ptr); }
     operator double() const { return (double) PyFloat_AsDouble(m_ptr); }
 };
 
 class weakref : public object {
 public:
-    PYBIND11_OBJECT_DEFAULT(weakref, object, PyWeakref_Check)
+    PYBIND11_OBJECT_CVT_DEFAULT(weakref, object, PyWeakref_Check, raw_weakref)
     explicit weakref(handle obj, handle callback = {})
         : object(PyWeakref_NewRef(obj.ptr(), callback.ptr()), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate weak reference!");
     }
+
+private:
+    static PyObject *raw_weakref(PyObject *o) {
+        return PyWeakref_NewRef(o, nullptr);
+    }
 };
 
 class slice : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(slice, object, PySlice_Check)
     slice(ssize_t start_, ssize_t stop_, ssize_t step_) {
         int_ start(start_), stop(stop_), step(step_);
@@ -1453,15 +1550,15 @@
         detail::any_container<ssize_t> strides, bool readonly = false);
 
     static memoryview from_buffer(
         const void *ptr, ssize_t itemsize, const char *format,
         detail::any_container<ssize_t> shape,
         detail::any_container<ssize_t> strides) {
         return memoryview::from_buffer(
-            const_cast<void*>(ptr), itemsize, format, shape, strides, true);
+            const_cast<void *>(ptr), itemsize, format, std::move(shape), std::move(strides), true);
     }
 
     template<typename T>
     static memoryview from_buffer(
         T *ptr, detail::any_container<ssize_t> shape,
         detail::any_container<ssize_t> strides, bool readonly = false) {
         return memoryview::from_buffer(
@@ -1510,15 +1607,15 @@
 inline memoryview memoryview::from_buffer(
     void *ptr, ssize_t itemsize, const char* format,
     detail::any_container<ssize_t> shape,
     detail::any_container<ssize_t> strides, bool readonly) {
     size_t ndim = shape->size();
     if (ndim != strides->size())
         pybind11_fail("memoryview: shape length doesn't match strides length");
-    ssize_t size = ndim ? 1 : 0;
+    ssize_t size = ndim != 0u ? 1 : 0;
     for (size_t i = 0; i < ndim; ++i)
         size *= (*shape)[i];
     Py_buffer view;
     view.buf = ptr;
     view.obj = nullptr;
     view.len = size * itemsize;
     view.readonly = static_cast<int>(readonly);
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/stl.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/stl.h`

 * *Files 2% similar despite different names*

```diff
@@ -140,33 +140,36 @@
     PYBIND11_TYPE_CASTER(Type, _("Dict[") + key_conv::name + _(", ") + value_conv::name + _("]"));
 };
 
 template <typename Type, typename Value> struct list_caster {
     using value_conv = make_caster<Value>;
 
     bool load(handle src, bool convert) {
-        if (!isinstance<sequence>(src) || isinstance<str>(src))
+        if (!isinstance<sequence>(src) || isinstance<bytes>(src) || isinstance<str>(src))
             return false;
         auto s = reinterpret_borrow<sequence>(src);
         value.clear();
         reserve_maybe(s, &value);
         for (auto it : s) {
             value_conv conv;
             if (!conv.load(it, convert))
                 return false;
             value.push_back(cast_op<Value &&>(std::move(conv)));
         }
         return true;
     }
 
 private:
-    template <typename T = Type,
-              enable_if_t<std::is_same<decltype(std::declval<T>().reserve(0)), void>::value, int> = 0>
-    void reserve_maybe(sequence s, Type *) { value.reserve(s.size()); }
-    void reserve_maybe(sequence, void *) { }
+    template <
+        typename T                                                                          = Type,
+        enable_if_t<std::is_same<decltype(std::declval<T>().reserve(0)), void>::value, int> = 0>
+    void reserve_maybe(const sequence &s, Type *) {
+        value.reserve(s.size());
+    }
+    void reserve_maybe(const sequence &, void *) {}
 
 public:
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         if (!std::is_lvalue_reference<T>::value)
             policy = return_value_policy_override<Value>::policy(policy);
         list l(src.size());
@@ -271,15 +274,16 @@
         }
         return value_conv::cast(*std::forward<T_>(src), policy, parent);
     }
 
     bool load(handle src, bool convert) {
         if (!src) {
             return false;
-        } else if (src.is_none()) {
+        }
+        if (src.is_none()) {
             return true;  // default-constructed value is already empty
         }
         value_conv inner_caster;
         if (!inner_caster.load(src, convert))
             return false;
 
         value.emplace(cast_op<typename T::value_type &&>(std::move(inner_caster)));
@@ -373,15 +377,19 @@
 template <typename... Ts>
 struct type_caster<std::variant<Ts...>> : variant_caster<std::variant<Ts...>> { };
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
 inline std::ostream &operator<<(std::ostream &os, const handle &obj) {
+#ifdef PYBIND11_HAS_STRING_VIEW
+    os << str(obj).cast<std::string_view>();
+#else
     os << (std::string) str(obj);
+#endif
     return os;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
 
 #if defined(_MSC_VER)
 #pragma warning(pop)
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/include/pybind11/stl_bind.h` & `icupy-0.9.0/src/third_party/pybind11/include/pybind11/stl_bind.h`

 * *Files 2% similar despite different names*

```diff
@@ -124,19 +124,19 @@
     };
 
     cl.def("append",
            [](Vector &v, const T &value) { v.push_back(value); },
            arg("x"),
            "Add an item to the end of the list");
 
-    cl.def(init([](iterable it) {
+    cl.def(init([](const iterable &it) {
         auto v = std::unique_ptr<Vector>(new Vector());
         v->reserve(len_hint(it));
         for (handle h : it)
-           v->push_back(h.cast<T>());
+            v->push_back(h.cast<T>());
         return v.release();
     }));
 
     cl.def("clear",
         [](Vector &v) {
             v.clear();
         },
@@ -147,35 +147,36 @@
        [](Vector &v, const Vector &src) {
            v.insert(v.end(), src.begin(), src.end());
        },
        arg("L"),
        "Extend the list by appending all the items in the given list"
     );
 
-    cl.def("extend",
-       [](Vector &v, iterable it) {
-           const size_t old_size = v.size();
-           v.reserve(old_size + len_hint(it));
-           try {
-               for (handle h : it) {
-                   v.push_back(h.cast<T>());
-               }
-           } catch (const cast_error &) {
-               v.erase(v.begin() + static_cast<typename Vector::difference_type>(old_size), v.end());
-               try {
-                   v.shrink_to_fit();
-               } catch (const std::exception &) {
-                   // Do nothing
-               }
-               throw;
-           }
-       },
-       arg("L"),
-       "Extend the list by appending all the items in the given list"
-    );
+    cl.def(
+        "extend",
+        [](Vector &v, const iterable &it) {
+            const size_t old_size = v.size();
+            v.reserve(old_size + len_hint(it));
+            try {
+                for (handle h : it) {
+                    v.push_back(h.cast<T>());
+                }
+            } catch (const cast_error &) {
+                v.erase(v.begin() + static_cast<typename Vector::difference_type>(old_size),
+                        v.end());
+                try {
+                    v.shrink_to_fit();
+                } catch (const std::exception &) {
+                    // Do nothing
+                }
+                throw;
+            }
+        },
+        arg("L"),
+        "Extend the list by appending all the items in the given list");
 
     cl.def("insert",
         [](Vector &v, DiffType i, const T &x) {
             // Can't use wrap_i; i == v.size() is OK
             if (i < 0)
                 i += v.size();
             if (i < 0 || (SizeType)i > v.size())
@@ -186,104 +187,103 @@
         "Insert an item at a given position."
     );
 
     cl.def("pop",
         [](Vector &v) {
             if (v.empty())
                 throw index_error();
-            T t = v.back();
+            T t = std::move(v.back());
             v.pop_back();
             return t;
         },
         "Remove and return the last item"
     );
 
     cl.def("pop",
         [wrap_i](Vector &v, DiffType i) {
             i = wrap_i(i, v.size());
-            T t = v[(SizeType) i];
-            v.erase(v.begin() + i);
+            T t = std::move(v[(SizeType) i]);
+            v.erase(std::next(v.begin(), i));
             return t;
         },
         arg("i"),
         "Remove and return the item at index ``i``"
     );
 
     cl.def("__setitem__",
         [wrap_i](Vector &v, DiffType i, const T &t) {
             i = wrap_i(i, v.size());
             v[(SizeType)i] = t;
         }
     );
 
     /// Slicing protocol
-    cl.def("__getitem__",
+    cl.def(
+        "__getitem__",
         [](const Vector &v, slice slice) -> Vector * {
-            size_t start, stop, step, slicelength;
+            size_t start = 0, stop = 0, step = 0, slicelength = 0;
 
             if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
                 throw error_already_set();
 
             auto *seq = new Vector();
             seq->reserve((size_t) slicelength);
 
             for (size_t i=0; i<slicelength; ++i) {
                 seq->push_back(v[start]);
                 start += step;
             }
             return seq;
         },
         arg("s"),
-        "Retrieve list elements using a slice object"
-    );
+        "Retrieve list elements using a slice object");
 
-    cl.def("__setitem__",
-        [](Vector &v, slice slice,  const Vector &value) {
-            size_t start, stop, step, slicelength;
+    cl.def(
+        "__setitem__",
+        [](Vector &v, slice slice, const Vector &value) {
+            size_t start = 0, stop = 0, step = 0, slicelength = 0;
             if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
                 throw error_already_set();
 
             if (slicelength != value.size())
                 throw std::runtime_error("Left and right hand size of slice assignment have different sizes!");
 
             for (size_t i=0; i<slicelength; ++i) {
                 v[start] = value[i];
                 start += step;
             }
         },
-        "Assign list elements using a slice object"
-    );
+        "Assign list elements using a slice object");
 
     cl.def("__delitem__",
         [wrap_i](Vector &v, DiffType i) {
             i = wrap_i(i, v.size());
             v.erase(v.begin() + i);
         },
         "Delete the list elements at index ``i``"
     );
 
-    cl.def("__delitem__",
+    cl.def(
+        "__delitem__",
         [](Vector &v, slice slice) {
-            size_t start, stop, step, slicelength;
+            size_t start = 0, stop = 0, step = 0, slicelength = 0;
 
             if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
                 throw error_already_set();
 
             if (step == 1 && false) {
                 v.erase(v.begin() + (DiffType) start, v.begin() + DiffType(start + slicelength));
             } else {
                 for (size_t i = 0; i < slicelength; ++i) {
                     v.erase(v.begin() + DiffType(start));
                     start += step - 1;
                 }
             }
         },
-        "Delete list elements using a slice object"
-    );
-
+        "Delete list elements using a slice object");
 }
 
 // If the type has an operator[] that doesn't return a reference (most notably std::vector<bool>),
 // we have to access by copying; otherwise we return by reference.
 template <typename Vector> using vector_needs_copy = negation<
     std::is_same<decltype(std::declval<Vector>()[typename Vector::size_type()]), typename Vector::value_type &>>;
 
@@ -396,34 +396,33 @@
     // numpy.h declares this for arbitrary types, but it may raise an exception and crash hard at runtime if PYBIND11_NUMPY_DTYPE hasn't been called, so check here
     format_descriptor<T>::format();
 
     cl.def_buffer([](Vector& v) -> buffer_info {
         return buffer_info(v.data(), static_cast<ssize_t>(sizeof(T)), format_descriptor<T>::format(), 1, {v.size()}, {sizeof(T)});
     });
 
-    cl.def(init([](buffer buf) {
+    cl.def(init([](const buffer &buf) {
         auto info = buf.request();
         if (info.ndim != 1 || info.strides[0] % static_cast<ssize_t>(sizeof(T)))
             throw type_error("Only valid 1D buffers can be copied to a vector");
         if (!detail::compare_buffer_info<T>::compare(info) || (ssize_t) sizeof(T) != info.itemsize)
             throw type_error("Format mismatch (Python: " + info.format + " C++: " + format_descriptor<T>::format() + ")");
 
         T *p = static_cast<T*>(info.ptr);
         ssize_t step = info.strides[0] / static_cast<ssize_t>(sizeof(T));
         T *end = p + info.shape[0] * step;
         if (step == 1) {
             return Vector(p, end);
         }
-        else {
-            Vector vec;
-            vec.reserve((size_t) info.shape[0]);
-            for (; p != end; p += step)
-                vec.push_back(*p);
-            return vec;
-        }
+        Vector vec;
+        vec.reserve((size_t) info.shape[0]);
+        for (; p != end; p += step)
+            vec.push_back(*p);
+        return vec;
+
     }));
 
     return;
 }
 
 template <typename Vector, typename Class_, typename... Args>
 void vector_buffer_impl(Class_&, std::false_type) {}
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/FindCatch.cmake` & `icupy-0.9.0/src/third_party/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/FindEigen3.cmake` & `icupy-0.9.0/src/third_party/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/FindPythonLibsNew.cmake` & `icupy-0.9.0/src/third_party/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/check-style.sh` & `icupy-0.9.0/src/third_party/pybind11/tools/check-style.sh`

 * *Files 7% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 # Invoke as: tools/check-style.sh <filenames>
 #
 
 check_style_errors=0
 IFS=$'\n'
 
 
-found="$(grep '\<\(if\|for\|while\|catch\)(\|){' $@ -rn --color=always)"
+found="$(grep '\<\(if\|for\|while\|catch\)(\|){' "$@" -rn --color=always)"
 if [ -n "$found" ]; then
     echo -e '\033[31;01mError: found the following coding style problems:\033[0m'
     check_style_errors=1
-    echo "$found" | sed -e 's/^/    /'
+    echo "${found//^/    /}"
 fi
 
 found="$(awk '
 function prefix(filename, lineno) {
     return "    \033[35m" filename "\033[36m:\033[32m" lineno "\033[36m:\033[0m"
 }
 function mark(pattern, string) { sub(pattern, "\033[01;31m&\033[0m", string); return string }
 last && /^\s*{/ {
     print prefix(FILENAME, FNR-1) mark("\\)\\s*$", last)
     print prefix(FILENAME, FNR)   mark("^\\s*{", $0)
     last=""
 }
 { last = /(if|for|while|catch|switch)\s*\(.*\)\s*$/ ? $0 : "" }
-' $(find include -type f) $@)"
+' "$(find include -type f)" "$@")"
 if [ -n "$found" ]; then
     check_style_errors=1
     echo -e '\033[31;01mError: braces should occur on the same line as the if/while/.. statement. Found issues in the following files:\033[0m'
     echo "$found"
 fi
 
 exit $check_style_errors
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/cmake_uninstall.cmake.in` & `icupy-0.9.0/src/third_party/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/libsize.py` & `icupy-0.9.0/src/third_party/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/make_changelog.py` & `icupy-0.9.0/src/third_party/pybind11/tools/make_changelog.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,29 +23,32 @@
 )
 
 print()
 
 
 api = ghapi.all.GhApi(owner="pybind", repo="pybind11")
 
-issues = api.issues.list_for_repo(labels="needs changelog", state="closed")
+issues_pages = ghapi.page.paged(
+    api.issues.list_for_repo, labels="needs changelog", state="closed"
+)
+issues = (issue for page in issues_pages for issue in page)
 missing = []
 
 for issue in issues:
     changelog = ENTRY.findall(issue.body)
     if changelog:
         (msg,) = changelog
         if not msg.startswith("* "):
             msg = "* " + msg
         if not msg.endswith("."):
             msg += "."
 
         msg += f"\n  `#{issue.number} <{issue.html_url}>`_"
 
-        print(Syntax(msg, "rst", theme="ansi_light"))
+        print(Syntax(msg, "rst", theme="ansi_light", word_wrap=True))
         print()
 
     else:
         missing.append(issue)
 
 if missing:
     print()
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11Common.cmake` & `icupy-0.9.0/src/third_party/pybind11/tools/pybind11Common.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -111,36 +111,40 @@
     PROPERTY INTERFACE_LINK_OPTIONS "$<$<PLATFORM_ID:Darwin>:LINKER:-undefined,dynamic_lookup>")
 endif()
 
 # ------------------------ Windows extras -------------------------
 
 add_library(pybind11::windows_extras IMPORTED INTERFACE ${optional_global})
 
-if(MSVC)
-  # /MP enables multithreaded builds (relevant when there are many files), /bigobj is
-  # needed for bigger binding projects due to the limit to 64k addressable sections
+if(MSVC) # That's also clang-cl
+  # /bigobj is needed for bigger binding projects due to the limit to 64k
+  # addressable sections
   set_property(
     TARGET pybind11::windows_extras
     APPEND
     PROPERTY INTERFACE_COMPILE_OPTIONS /bigobj)
 
-  if(CMAKE_VERSION VERSION_LESS 3.11)
-    set_property(
-      TARGET pybind11::windows_extras
-      APPEND
-      PROPERTY INTERFACE_COMPILE_OPTIONS $<$<NOT:$<CONFIG:Debug>>:/MP>)
-  else()
-    # Only set these options for C++ files.  This is important so that, for
-    # instance, projects that include other types of source files like CUDA
-    # .cu files don't get these options propagated to nvcc since that would
-    # cause the build to fail.
-    set_property(
-      TARGET pybind11::windows_extras
-      APPEND
-      PROPERTY INTERFACE_COMPILE_OPTIONS $<$<NOT:$<CONFIG:Debug>>:$<$<COMPILE_LANGUAGE:CXX>:/MP>>)
+  # /MP enables multithreaded builds (relevant when there are many files) for MSVC
+  if("${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC") # no Clang no Intel
+    if(CMAKE_VERSION VERSION_LESS 3.11)
+      set_property(
+        TARGET pybind11::windows_extras
+        APPEND
+        PROPERTY INTERFACE_COMPILE_OPTIONS $<$<NOT:$<CONFIG:Debug>>:/MP>)
+    else()
+      # Only set these options for C++ files.  This is important so that, for
+      # instance, projects that include other types of source files like CUDA
+      # .cu files don't get these options propagated to nvcc since that would
+      # cause the build to fail.
+      set_property(
+        TARGET pybind11::windows_extras
+        APPEND
+        PROPERTY INTERFACE_COMPILE_OPTIONS
+                 $<$<NOT:$<CONFIG:Debug>>:$<$<COMPILE_LANGUAGE:CXX>:/MP>>)
+    endif()
   endif()
 endif()
 
 # ----------------------- Optimize binary size --------------------------
 
 add_library(pybind11::opt_size IMPORTED INTERFACE ${optional_global})
 
@@ -294,21 +298,26 @@
     set(${linkerflags_out}
         "${linkerflags}"
         PARENT_SCOPE)
   endif()
 endfunction()
 
 function(_pybind11_generate_lto target prefer_thin_lto)
+  if(MINGW)
+    message(STATUS "${target} disabled (problems with undefined symbols for MinGW for now)")
+    return()
+  endif()
+
   if(CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
     set(cxx_append "")
     set(linker_append "")
     if(CMAKE_CXX_COMPILER_ID MATCHES "Clang" AND NOT APPLE)
       # Clang Gold plugin does not support -Os; append -O3 to MinSizeRel builds to override it
       set(linker_append ";$<$<CONFIG:MinSizeRel>:-O3>")
-    elseif(CMAKE_CXX_COMPILER_ID MATCHES "GNU")
+    elseif(CMAKE_CXX_COMPILER_ID MATCHES "GNU" AND NOT MINGW)
       set(cxx_append ";-fno-fat-lto-objects")
     endif()
 
     if(CMAKE_CXX_COMPILER_ID MATCHES "Clang" AND prefer_thin_lto)
       _pybind11_return_if_cxx_and_linker_flags_work(
         HAS_FLTO_THIN "-flto=thin${cxx_append}" "-flto=thin${linker_append}"
         PYBIND11_LTO_CXX_FLAGS PYBIND11_LTO_LINKER_FLAGS)
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11Config.cmake.in` & `icupy-0.9.0/src/third_party/pybind11/tools/pybind11Config.cmake.in`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
 This module defines the following commands to assist with creating Python modules:
 
 .. code-block:: cmake
 
   pybind11_add_module(<target>
     [STATIC|SHARED|MODULE]
-    [THIN_LTO] [OPT_SIZE] [NO_EXTRAS] [WITHOUT_SOBAI]
+    [THIN_LTO] [OPT_SIZE] [NO_EXTRAS] [WITHOUT_SOABI]
     <files>...
     )
 
 Add a module and setup all helpers. You can select the type of the library; the
 default is ``MODULE``. There are several options:
 
 ``OPT_SIZE``
@@ -197,15 +197,16 @@
   find_package(pybind11 CONFIG)
   find_package(pybind11 2.0 EXACT CONFIG REQUIRED)
 
 #]=============================================================================]
 @PACKAGE_INIT@
 
 # Location of pybind11/pybind11.h
-set(pybind11_INCLUDE_DIR "${PACKAGE_PREFIX_DIR}/@CMAKE_INSTALL_INCLUDEDIR@")
+# This will be relative unless explicitly set as absolute
+set(pybind11_INCLUDE_DIR "@pybind11_INCLUDEDIR@")
 
 set(pybind11_LIBRARY "")
 set(pybind11_DEFINITIONS USING_pybind11)
 set(pybind11_VERSION_TYPE "@pybind11_VERSION_TYPE@")
 
 check_required_components(pybind11)
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11NewTools.cmake` & `icupy-0.9.0/src/third_party/pybind11/tools/pybind11NewTools.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
   endif()
 
   if(NOT DEFINED CMAKE_CUDA_VISIBILITY_PRESET)
     set_target_properties(${target_name} PROPERTIES CUDA_VISIBILITY_PRESET "hidden")
   endif()
 
   # If we don't pass a WITH_SOABI or WITHOUT_SOABI, use our own default handling of extensions
-  if(NOT ARG_WITHOUT_SOABI OR NOT "WITH_SOABI" IN_LIST ARG_UNPARSED_ARGUMENTS)
+  if(NOT ARG_WITHOUT_SOABI AND NOT "WITH_SOABI" IN_LIST ARG_UNPARSED_ARGUMENTS)
     pybind11_extension(${target_name})
   endif()
 
   if(ARG_NO_EXTRAS)
     return()
   endif()
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/pybind11Tools.cmake` & `icupy-0.9.0/src/third_party/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/setup_global.py.in` & `icupy-0.9.0/src/third_party/pybind11/tools/setup_global.py.in`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,17 @@
             self.mkpath(dst)
             (out, _) = self.copy_file(header, dst)
             self.outfiles.append(out)
 
 
 main_headers = glob.glob("pybind11/include/pybind11/*.h")
 detail_headers = glob.glob("pybind11/include/pybind11/detail/*.h")
+stl_headers = glob.glob("pybind11/include/pybind11/stl/*.h")
 cmake_files = glob.glob("pybind11/share/cmake/pybind11/*.cmake")
-headers = main_headers + detail_headers
+headers = main_headers + detail_headers + stl_headers
 
 cmdclass = {"install_headers": InstallHeadersNested}
 $extra_cmd
 
 # This will _not_ affect installing from wheels,
 # only building wheels or installing from SDist.
 # Primarily intended on Windows, where this is sometimes
@@ -54,10 +55,11 @@
     version="$version",
     packages=[],
     headers=headers,
     data_files=[
         (base + "share/cmake/pybind11", cmake_files),
         (base + "include/pybind11", main_headers),
         (base + "include/pybind11/detail", detail_headers),
+        (base + "include/pybind11/stl", stl_headers),
     ],
     cmdclass=cmdclass,
 )
```

### Comparing `icupy-0.8.0.post2/src/third_party/pybind11/tools/setup_main.py.in` & `icupy-0.9.0/src/third_party/pybind11/tools/setup_main.py.in`

 * *Files 15% similar despite different names*

```diff
@@ -12,25 +12,30 @@
     name="pybind11",
     version="$version",
     download_url='https://github.com/pybind/pybind11/tarball/v$version',
     packages=[
         "pybind11",
         "pybind11.include.pybind11",
         "pybind11.include.pybind11.detail",
+        "pybind11.include.pybind11.stl",
         "pybind11.share.cmake.pybind11",
     ],
     package_data={
         "pybind11": ["py.typed", "*.pyi"],
         "pybind11.include.pybind11": ["*.h"],
         "pybind11.include.pybind11.detail": ["*.h"],
+        "pybind11.include.pybind11.stl": ["*.h"],
         "pybind11.share.cmake.pybind11": ["*.cmake"],
     },
     extras_require={
         "global": ["pybind11_global==$version"]
         },
     entry_points={
         "console_scripts": [
              "pybind11-config = pybind11.__main__:main",
+        ],
+        "pipx.run": [
+             "pybind11 = pybind11.__main__:main",
         ]
     },
     cmdclass=cmdclass
 )
```

### Comparing `icupy-0.8.0.post2/src/timezone.cpp` & `icupy-0.9.0/src/timezone.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
           py::arg("other"))
       .def(
           "__ne__", [](const TimeZone &self, const TimeZone &other) { return self != other; }, py::is_operator(),
           py::arg("other"));
   // FIXME: Implement "static void icu::TimeZone::adoptDefault(TimeZone *zone)".
   /*
   tz.def_static(
-      "adopt_default", [](TimeZone *zone) { TimeZone::adoptDefault(zone ? zone->clone() : NULL); }, py::arg("zone"));
+      "adopt_default", [](TimeZone *zone) { TimeZone::adoptDefault(zone ? zone->clone() : nullptr); }, py::arg("zone"));
   */
   tz.def("clone", &TimeZone::clone);
   tz.def_static("count_equivalent_ids", &TimeZone::countEquivalentIDs, py::arg("id_"))
       .def_static(
           // const char16_t *id -> const UnicodeString &id
           "count_equivalent_ids", [](const char16_t *id) { return TimeZone::countEquivalentIDs(id); }, py::arg("id_"));
   tz.def_static("create_default", []() -> std::variant<BasicTimeZone *, TimeZone *> {
@@ -94,15 +94,15 @@
           },
           py::arg("id_"));
   tz.def_static(
       "create_time_zone_id_enumeration",
       [](USystemTimeZoneType zone_type, const char *region, const std::optional<int32_t> &raw_offset) {
         UErrorCode error_code = U_ZERO_ERROR;
         auto result = TimeZone::createTimeZoneIDEnumeration(
-            zone_type, region, raw_offset.has_value() ? &raw_offset.value() : NULL, error_code);
+            zone_type, region, raw_offset.has_value() ? &raw_offset.value() : nullptr, error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
       },
       py::arg("zone_type"), py::arg("region"), py::arg("raw_offset"));
 #if (U_ICU_VERSION_MAJOR_NUM >= 55)
@@ -351,32 +351,32 @@
         }
         return result;
       },
       py::arg("tz"), py::arg("start"), py::arg("end"), py::arg("ignore_dst_amount"));
 
   // icu::RuleBasedTimeZone
   rbtz.def(py::init([](const UnicodeString &id, InitialTimeZoneRule *initial_rule) {
-             return std::make_unique<RuleBasedTimeZone>(id, initial_rule ? initial_rule->clone() : NULL);
+             return std::make_unique<RuleBasedTimeZone>(id, initial_rule ? initial_rule->clone() : nullptr);
            }),
            py::arg("id_"), py::arg("initial_rule"))
       .def(py::init([](const char *id, InitialTimeZoneRule *initial_rule) {
-             return std::make_unique<RuleBasedTimeZone>(id, initial_rule ? initial_rule->clone() : NULL);
+             return std::make_unique<RuleBasedTimeZone>(id, initial_rule ? initial_rule->clone() : nullptr);
            }),
            py::arg("id_"), py::arg("initial_rule"))
       .def(py::init<const RuleBasedTimeZone &>(), py::arg("source"))
       .def(py::self != py::self, py::arg("other"))
       .def(py::self == py::self, py::arg("other"));
   rbtz.def("__copy__", &RuleBasedTimeZone::clone)
       .def(
           "__deepcopy__", [](const RuleBasedTimeZone &self, py::dict) { return self.clone(); }, py::arg("memo"));
   rbtz.def(
       "add_transition_rule",
       [](RuleBasedTimeZone &self, TimeZoneRule *rule) {
         UErrorCode error_code = U_ZERO_ERROR;
-        self.addTransitionRule(rule ? rule->clone() : NULL, error_code);
+        self.addTransitionRule(rule ? rule->clone() : nullptr, error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
       },
       py::arg("rule"));
   rbtz.def("clone", &RuleBasedTimeZone::clone);
   rbtz.def("complete", [](RuleBasedTimeZone &self) {
```

### Comparing `icupy-0.8.0.post2/src/tmunit.cpp` & `icupy-0.9.0/src/tmunit.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/translit.cpp` & `icupy-0.9.0/src/translit.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/tzfmt.cpp` & `icupy-0.9.0/src/tzfmt.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/tznames.cpp` & `icupy-0.9.0/src/tznames.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/tzrule.cpp` & `icupy-0.9.0/src/tzrule.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/tztrans.cpp` & `icupy-0.9.0/src/tztrans.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,19 @@
   tzt.def("__copy__", &TimeZoneTransition::clone)
       .def(
           "__deepcopy__", [](const TimeZoneTransition &self, py::dict) { return self.clone(); }, py::arg("memo"));
   // FIXME: Implement "void icu::TimeZoneTransition::adoptFrom(TimeZoneRule *from)".
   // FIXME: Implement "void icu::TimeZoneTransition::adoptTo(TimeZoneRule *to)".
   /*
   tzt.def(
-      "adopt_from", [](TimeZoneTransition &self, TimeZoneRule *from) { self.adoptFrom(from ? from->clone() : NULL); },
+      "adopt_from",
+      [](TimeZoneTransition &self, TimeZoneRule *from) { self.adoptFrom(from ? from->clone() : nullptr); },
       py::arg("from"));
   tzt.def(
-      "adopt_to", [](TimeZoneTransition &self, TimeZoneRule *to) { self.adoptTo(to ? to->clone() : NULL); },
+      "adopt_to", [](TimeZoneTransition &self, TimeZoneRule *to) { self.adoptTo(to ? to->clone() : nullptr); },
       py::arg("to"));
   */
   tzt.def("clone", &TimeZoneTransition::clone);
   tzt.def("get_from", &TimeZoneTransition::getFrom, py::return_value_policy::reference);
   tzt.def("get_time", &TimeZoneTransition::getTime);
   tzt.def("get_to", &TimeZoneTransition::getTo, py::return_value_policy::reference);
   tzt.def("set_from", &TimeZoneTransition::setFrom, py::arg("from"));
```

### Comparing `icupy-0.8.0.post2/src/ubidi.cpp` & `icupy-0.9.0/src/ubidi.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ubidiptr.hpp` & `icupy-0.9.0/src/ubidiptr.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ubrk.cpp` & `icupy-0.9.0/src/ubrk.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucal.cpp` & `icupy-0.9.0/src/ucal.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uchar.cpp` & `icupy-0.9.0/src/uchar.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1018,15 +1018,15 @@
       },
       py::arg("name_choice"), py::arg("name"));
   m.def("u_char_mirror", &u_charMirror, py::arg("c"));
   m.def(
       "u_char_name",
       [](UChar32 code, UCharNameChoice name_choice) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto length = u_charName(code, name_choice, NULL, 0, &error_code);
+        const auto length = u_charName(code, name_choice, nullptr, 0, &error_code);
         std::string result(length, '\0');
         error_code = U_ZERO_ERROR;
         u_charName(code, name_choice, result.data(), (int32_t)result.size(), &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
@@ -1053,15 +1053,15 @@
       py::arg("property_"));
 #endif // (U_ICU_VERSION_MAJOR_NUM >= 63)
   m.def("u_get_combining_class", &u_getCombiningClass, py::arg("c"));
   m.def(
       "u_get_fc_nfkc_closure",
       [](UChar32 c) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto length = u_getFC_NFKC_Closure(c, NULL, 0, &error_code);
+        const auto length = u_getFC_NFKC_Closure(c, nullptr, 0, &error_code);
         std::u16string result(length, u'\0');
         error_code = U_ZERO_ERROR;
         u_getFC_NFKC_Closure(c, result.data(), (int32_t)result.size(), &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
```

### Comparing `icupy-0.8.0.post2/src/ucnv.cpp` & `icupy-0.9.0/src/ucnv.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,16 @@
       py::arg("alias"));
   m.def("ucnv_count_available", &ucnv_countAvailable);
   m.def("ucnv_count_standards", &ucnv_countStandards);
   m.def(
       "ucnv_detect_unicode_signature",
       [](const char *source, int32_t source_length) -> std::optional<const char *> {
         UErrorCode error_code = U_ZERO_ERROR;
-        auto result = ucnv_detectUnicodeSignature(source, source_length, NULL, &error_code);
-        if (result == NULL) {
+        auto result = ucnv_detectUnicodeSignature(source, source_length, nullptr, &error_code);
+        if (result == nullptr) {
           return std::nullopt;
         }
         return result;
       },
       py::arg("source"), py::arg("source_length"));
   m.def(
       "ucnv_fix_file_separator",
@@ -150,15 +150,15 @@
       },
       py::arg("converter"));
   m.def("ucnv_get_default_name", &ucnv_getDefaultName);
   m.def(
       "ucnv_get_display_name",
       [](_UConverterPtr &converter, const char *display_locale) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto length = ucnv_getDisplayName(converter, display_locale, NULL, 0, &error_code);
+        const auto length = ucnv_getDisplayName(converter, display_locale, nullptr, 0, &error_code);
         std::u16string result(length, u'\0');
         error_code = U_ZERO_ERROR;
         ucnv_getDisplayName(converter, display_locale, result.data(), (int32_t)result.size(), &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
```

### Comparing `icupy-0.8.0.post2/src/ucnv_cb.cpp` & `icupy-0.9.0/src/ucnv_cb.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucnv_err.cpp` & `icupy-0.9.0/src/ucnv_err.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucnv_err.hpp` & `icupy-0.9.0/src/ucnv_err.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucol.cpp` & `icupy-0.9.0/src/ucol.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucpmap.cpp` & `icupy-0.9.0/src/ucpmap.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucpmapptr.hpp` & `icupy-0.9.0/src/ucpmapptr.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucsdet.cpp` & `icupy-0.9.0/src/ucsdet.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   m.def(
       "ucsdet_detect",
       [](_UCharsetDetectorPtr &ucsd) -> std::optional<std::unique_ptr<_ConstUCharsetMatchPtr>> {
         UErrorCode error_code = U_ZERO_ERROR;
         auto p = ucsdet_detect(ucsd, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
-        } else if (p == NULL) {
+        } else if (p == nullptr) {
           return std::nullopt;
         }
         return std::make_unique<_ConstUCharsetMatchPtr>(p);
       },
       py::arg("ucsd"));
   m.def(
       "ucsdet_detect_all",
@@ -99,15 +99,15 @@
         return result;
       },
       py::return_value_policy::reference, py::arg("ucsm"));
   m.def(
       "ucsdet_get_uchars",
       [](_ConstUCharsetMatchPtr &ucsm) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto cap = ucsdet_getUChars(ucsm, NULL, 0, &error_code);
+        const auto cap = ucsdet_getUChars(ucsm, nullptr, 0, &error_code);
         std::u16string result(cap, '\0');
         error_code = U_ZERO_ERROR;
         ucsdet_getUChars(ucsm, result.data(), cap, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
```

### Comparing `icupy-0.8.0.post2/src/ucsdetptr.hpp` & `icupy-0.9.0/src/ucsdetptr.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ucurr.cpp` & `icupy-0.9.0/src/ucurr.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/udat.cpp` & `icupy-0.9.0/src/udat.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/udatpg.cpp` & `icupy-0.9.0/src/udatpg.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/udisplaycontext.cpp` & `icupy-0.9.0/src/udisplaycontext.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uenum.cpp` & `icupy-0.9.0/src/uenum.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #include "main.hpp"
 #include "uenumptr.hpp"
-#include <optional>
 #include <pybind11/stl.h>
 #include <unicode/strenum.h>
 #include <unicode/ustring.h>
 
 using namespace icu;
 
 _UEnumerationPtr::_UEnumerationPtr(UEnumeration *p) : p_(p) {}
@@ -28,68 +27,74 @@
         return result;
       },
       py::arg("en"));
   m.def(
       "uenum_next",
       [](_UEnumerationPtr &en) {
         UErrorCode error_code = U_ZERO_ERROR;
-        auto result = uenum_next(en, NULL, &error_code);
+        auto result = uenum_next(en, nullptr, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
       },
       py::return_value_policy::reference, py::arg("en"));
 #if (U_ICU_VERSION_MAJOR_NUM >= 50)
   m.def(
       "uenum_open_char_strings_enumeration",
-      [](const std::vector<std::string> &strings, std::optional<int32_t> count) {
+      [](const std::vector<std::string> &strings, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)strings.size();
+        }
         UErrorCode error_code = U_ZERO_ERROR;
         auto source = std::shared_ptr<char *[]>(new char *[strings.size()], std::default_delete<char *[]>());
         auto s = source.get();
         for (size_t n = 0; n < strings.size(); ++n, ++s) {
           *s = strdup(strings[n].c_str());
         }
-        auto p = uenum_openCharStringsEnumeration(source.get(), count.value_or(strings.size()), &error_code);
+        auto p = uenum_openCharStringsEnumeration(source.get(), count, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return std::make_unique<_UEnumerationPtr>(p, source);
       },
-      py::arg("strings"), py::arg("count") = std::nullopt);
+      py::arg("strings"), py::arg("count") = -1);
 #endif // (U_ICU_VERSION_MAJOR_NUM >= 50)
   m.def(
       "uenum_open_from_string_enumeration",
       [](StringEnumeration *adopted) {
         UErrorCode error_code = U_ZERO_ERROR;
-        auto p = uenum_openFromStringEnumeration(adopted->clone(), &error_code);
+        auto p = uenum_openFromStringEnumeration(adopted ? adopted->clone() : nullptr, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return std::make_unique<_UEnumerationPtr>(p);
       },
       py::arg("adopted"));
 #if (U_ICU_VERSION_MAJOR_NUM >= 50)
   m.def(
       "uenum_open_uchar_strings_enumeration",
-      [](const std::vector<std::u16string> &strings, std::optional<int32_t> count) {
+      [](const std::vector<std::u16string> &strings, int32_t count) {
+        if (count == -1) {
+          count = (int32_t)strings.size();
+        }
         UErrorCode error_code = U_ZERO_ERROR;
         auto source = std::shared_ptr<UChar *[]>(new UChar *[strings.size()], std::default_delete<UChar *[]>());
         auto s = source.get();
         for (size_t n = 0; n < strings.size(); ++n, ++s) {
           *s = new UChar[strings[n].size() + 1];
           u_strcpy(*s, strings[n].c_str());
         }
-        auto p = uenum_openUCharStringsEnumeration(source.get(), count.value_or(strings.size()), &error_code);
+        auto p = uenum_openUCharStringsEnumeration(source.get(), count, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return std::make_unique<_UEnumerationPtr>(p, source);
       },
-      py::arg("strings"), py::arg("count") = std::nullopt);
+      py::arg("strings"), py::arg("count") = -1);
 #endif // (U_ICU_VERSION_MAJOR_NUM >= 50)
   m.def(
       "uenum_reset",
       [](_UEnumerationPtr &en) {
         UErrorCode error_code = U_ZERO_ERROR;
         uenum_reset(en, &error_code);
         if (U_FAILURE(error_code)) {
@@ -97,15 +102,15 @@
         }
       },
       py::arg("en"));
   m.def(
       "uenum_unext",
       [](_UEnumerationPtr &en) {
         UErrorCode error_code = U_ZERO_ERROR;
-        auto result = uenum_unext(en, NULL, &error_code);
+        auto result = uenum_unext(en, nullptr, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
       },
       py::return_value_policy::reference, py::arg("en"));
 }
```

### Comparing `icupy-0.8.0.post2/src/uformattedvalue.cpp` & `icupy-0.9.0/src/uformattedvalue.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uidna.cpp` & `icupy-0.9.0/src/uidna.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uloc.cpp` & `icupy-0.9.0/src/uloc.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uniset.cpp` & `icupy-0.9.0/src/uniset.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
       .def("retain_all", py::overload_cast<const UnicodeString &>(&UnicodeSet::retainAll), py::arg("s"))
       .def(
           // const char16_t *s -> const UnicodeString &s
           "retain_all", [](UnicodeSet &self, const char16_t *s) -> UnicodeSet & { return self.retainAll(s); },
           py::arg("s"));
   us.def("serialize", [](const UnicodeSet &self) {
     UErrorCode error_code = U_ZERO_ERROR;
-    const auto length = self.serialize(NULL, 0, error_code);
+    const auto length = self.serialize(nullptr, 0, error_code);
     std::vector<uint16_t> result(length);
     error_code = U_ZERO_ERROR;
     self.serialize(result.data(), length, error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return result;
```

### Comparing `icupy-0.8.0.post2/src/unistr.cpp` & `icupy-0.9.0/src/unistr.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
           },
           py::arg("src_chars"), py::arg("src_length"));
   us.def(
         // int32_t extract(char *dest, int32_t destCapacity, UConverter *cnv, UErrorCode &errorCode)
         "extract",
         [](const UnicodeString &self, _UConverterPtr &cnv) {
           UErrorCode error_code = U_ZERO_ERROR;
-          const auto length = self.extract(NULL, 0, cnv, error_code);
+          const auto length = self.extract(nullptr, 0, cnv, error_code);
           std::string dest(length, '\0');
           error_code = U_ZERO_ERROR;
           self.extract(dest.data(), (int32_t)dest.size(), cnv, error_code);
           if (U_FAILURE(error_code)) {
             throw ICUError(error_code);
           }
           return py::bytes(dest.data(), length);
@@ -377,42 +377,42 @@
           })
       .def("extract", py::overload_cast<int32_t, int32_t, UnicodeString &>(&UnicodeString::extract, py::const_),
            py::arg("start"), py::arg("length"), py::arg("target"))
       .def(
           // int32_t extract(int32_t start, int32_t startLength, char *target, const char *codepage = 0)
           "extract",
           [](const UnicodeString &self, int32_t start, int32_t start_length, const char *codepage) {
-            const auto length = self.extract(start, start_length, NULL, codepage);
+            const auto length = self.extract(start, start_length, nullptr, codepage);
             if (length <= 0) {
               return py::bytes();
             }
             std::string target(length, '\0');
             self.extract(start, start_length, target.data(), codepage);
             return py::bytes(target.data(), length);
           },
           py::arg("start"), py::arg("start_length"), py::arg("codepage"))
       .def(
           // int32_t extract(int32_t start, int32_t startLength, char *target, int32_t targetCapacity,
           //                 enum EInvariant inv)
           "extract",
           [](const UnicodeString &self, int32_t start, int32_t start_length, UnicodeString::EInvariant inv) {
-            const auto length = self.extract(start, start_length, NULL, 0, inv);
+            const auto length = self.extract(start, start_length, nullptr, 0, inv);
             if (length <= 0) {
               return py::bytes();
             }
             std::string target(length, '\0');
             self.extract(start, start_length, target.data(), (int32_t)target.size(), inv);
             return py::bytes(target.data(), length);
           },
           py::arg("start"), py::arg("start_length"), py::arg("inv"))
       .def(
           // int32_t extract(int32_t start, int32_t startLength, char *target, uint32_t targetLength)
           "extract",
           [](const UnicodeString &self, int32_t start, int32_t start_length) {
-            const auto length = self.extract(start, start_length, (char *)NULL, (uint32_t)0);
+            const auto length = self.extract(start, start_length, (char *)nullptr, (uint32_t)0);
             if (length <= 0) {
               return py::bytes();
             }
             std::string target(length, '\0');
             self.extract(start, start_length, target.data(), (uint32_t)target.size());
             return py::bytes(target.data(), length);
           },
@@ -821,15 +821,15 @@
       .def(
           // const char *locale -> const Locale &locale
           "to_upper", [](UnicodeString &self, const char *locale) -> UnicodeString & { return self.toUpper(locale); },
           py::arg("locale"))
       .def("to_upper", py::overload_cast<>(&UnicodeString::toUpper));
   us.def("to_utf32", [](const UnicodeString &self) {
     UErrorCode error_code = U_ZERO_ERROR;
-    const auto length = self.toUTF32(NULL, 0, error_code);
+    const auto length = self.toUTF32(nullptr, 0, error_code);
     std::vector<UChar32> dest(length);
     error_code = U_ZERO_ERROR;
     self.toUTF32(dest.data(), length, error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
     return std::u32string(dest.begin(), dest.end());
```

### Comparing `icupy-0.8.0.post2/src/unorm2.cpp` & `icupy-0.9.0/src/unorm2.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/unum.cpp` & `icupy-0.9.0/src/unum.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/unumberformatter.cpp` & `icupy-0.9.0/src/unumberformatter.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/unumberrangeformatter.cpp` & `icupy-0.9.0/src/unumberrangeformatter.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uregex.cpp` & `icupy-0.9.0/src/uregex.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uregex.hpp` & `icupy-0.9.0/src/uregex.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/ures.cpp` & `icupy-0.9.0/src/ures.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uscript.cpp` & `icupy-0.9.0/src/uscript.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 #if (U_ICU_VERSION_MAJOR_NUM >= 51)
   m.def("uscript_breaks_between_letters", &uscript_breaksBetweenLetters, py::arg("script"));
 #endif // (U_ICU_VERSION_MAJOR_NUM >= 51)
   m.def(
       "uscript_get_code",
       [](const char *name_or_abbr_or_locale) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto length = uscript_getCode(name_or_abbr_or_locale, NULL, 0, &error_code);
+        const auto length = uscript_getCode(name_or_abbr_or_locale, nullptr, 0, &error_code);
         std::vector<UScriptCode> result(length);
         error_code = U_ZERO_ERROR;
         uscript_getCode(name_or_abbr_or_locale, result.data(), (int32_t)result.size(), &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
@@ -262,15 +262,15 @@
       py::arg("name_or_abbr_or_locale"));
   m.def("uscript_get_name", &uscript_getName, py::arg("script_code"));
 #if (U_ICU_VERSION_MAJOR_NUM >= 51)
   m.def(
       "uscript_get_sample_string",
       [](UScriptCode script) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto length = uscript_getSampleString(script, NULL, 0, &error_code);
+        const auto length = uscript_getSampleString(script, nullptr, 0, &error_code);
         std::u16string result(length, u'\0');
         error_code = U_ZERO_ERROR;
         uscript_getSampleString(script, result.data(), (int32_t)result.size(), &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
@@ -290,15 +290,15 @@
       },
       py::arg("codepoint"));
 #if (U_ICU_VERSION_MAJOR_NUM >= 49)
   m.def(
       "uscript_get_script_extensions",
       [](UChar32 c) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto length = uscript_getScriptExtensions(c, NULL, 0, &error_code);
+        const auto length = uscript_getScriptExtensions(c, nullptr, 0, &error_code);
         std::vector<UScriptCode> result(length);
         error_code = U_ZERO_ERROR;
         uscript_getScriptExtensions(c, result.data(), (int32_t)result.size(), &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
```

### Comparing `icupy-0.8.0.post2/src/usearch.cpp` & `icupy-0.9.0/src/usearch.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uset.cpp` & `icupy-0.9.0/src/uset.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/utext.cpp` & `icupy-0.9.0/src/utext.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 
 _UTextVector::_UTextVector(size_t n) {
   values_ = std::vector<_UTextPtr>(n);
   sources_ = std::vector<UnicodeString>(n);
   UErrorCode error_code;
   for (size_t i = 0; i < n; ++i) {
     error_code = U_ZERO_ERROR;
-    values_[i] = utext_openUnicodeString(NULL, &sources_[i], &error_code);
+    values_[i] = utext_openUnicodeString(nullptr, &sources_[i], &error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
   }
 }
 
 _UTextVector::_UTextVector(const _UnicodeStringList &iterable) {
   const auto size = iterable.size();
   values_ = std::vector<_UTextPtr>(size);
   sources_ = std::vector<UnicodeString>(iterable.begin(), iterable.end());
   UErrorCode error_code;
   for (size_t i = 0; i < size; ++i) {
     error_code = U_ZERO_ERROR;
-    values_[i] = utext_openUnicodeString(NULL, &sources_[i], &error_code);
+    values_[i] = utext_openUnicodeString(nullptr, &sources_[i], &error_code);
     if (U_FAILURE(error_code)) {
       throw ICUError(error_code);
     }
   }
 }
 
 _UTextVector::~_UTextVector() { clear(); }
@@ -108,15 +108,15 @@
         return std::make_unique<_UTextPtr>(p, src.get_source());
       },
       py::arg("dest"), py::arg("src"), py::arg("deep"), py::arg("read_only"));
   m.def(
       "utext_close",
       [](_UTextPtr &ut) -> std::optional<_UTextPtr> {
         auto p = utext_close(ut);
-        if (p == NULL) {
+        if (p == nullptr) {
           return std::nullopt;
         }
         assert(p == (UText *)ut);
         return ut;
       },
       py::arg("ut"));
   m.def(
@@ -133,15 +133,15 @@
       "utext_current32", [](_UTextPtr &ut) { return utext_current32(ut); }, py::arg("ut"));
   m.def(
       "utext_equals", [](_UTextPtr &a, _UTextPtr &b) { return utext_equals(a, b); }, py::arg("a"), py::arg("b"));
   m.def(
       "utext_extract",
       [](_UTextPtr &ut, int64_t native_start, int64_t native_limit) {
         UErrorCode error_code = U_ZERO_ERROR;
-        const auto dest_capacity = utext_extract(ut, native_start, native_limit, NULL, 0, &error_code);
+        const auto dest_capacity = utext_extract(ut, native_start, native_limit, nullptr, 0, &error_code);
         std::u16string result(dest_capacity, u'\0');
         error_code = U_ZERO_ERROR;
         utext_extract(ut, native_start, native_limit, result.data(), dest_capacity, &error_code);
         if (U_FAILURE(error_code)) {
           throw ICUError(error_code);
         }
         return result;
```

### Comparing `icupy-0.8.0.post2/src/utextptr.hpp` & `icupy-0.9.0/src/utextptr.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/utextvec.hpp` & `icupy-0.9.0/src/utextvec.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/utrans.cpp` & `icupy-0.9.0/src/utrans.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/utypes.cpp` & `icupy-0.9.0/src/utypes.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/uversion.cpp` & `icupy-0.9.0/src/uversion.cpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/src/voidptr.cpp` & `icupy-0.9.0/src/voidptr.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -25,12 +25,13 @@
       python_context = std::any_cast<py::object>(context_);
     }
   }
   return python_context;
 }
 
 void init_voidptr(py::module &m) {
-  py::class_<_ConstVoidPtr>(m, "ConstVoidPtr")
-      .def(py::init<std::nullptr_t>(), py::arg("value"))
+  py::class_<_ConstVoidPtr> cvp(m, "ConstVoidPtr");
+  cvp.def(py::init<std::nullptr_t>(), py::arg("value"))
       .def(py::init<const char *>(), py::arg("value").none(false))
       .def(py::init<py::object>(), py::arg("value"));
+  cvp.def("to_object", &_ConstVoidPtr::to_object);
 }
```

### Comparing `icupy-0.8.0.post2/src/voidptr.hpp` & `icupy-0.9.0/src/voidptr.hpp`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/__init__.py` & `icupy-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_coleitr.py` & `icupy-0.9.0/tests/test_coleitr.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_compactdecimalformat.py` & `icupy-0.9.0/tests/test_compactdecimalformat.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_currpinf.py` & `icupy-0.9.0/tests/test_currpinf.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_currunit.py` & `icupy-0.9.0/tests/test_currunit.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_datefmt.py` & `icupy-0.9.0/tests/test_datefmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_dcfmtsym.py` & `icupy-0.9.0/tests/test_dcfmtsym.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_decimfmt.py` & `icupy-0.9.0/tests/test_decimfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_dtfmtsym.py` & `icupy-0.9.0/tests/test_dtfmtsym.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_dtitvfmt.py` & `icupy-0.9.0/tests/test_dtitvfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_dtptngen.py` & `icupy-0.9.0/tests/test_dtptngen.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_fmtable.py` & `icupy-0.9.0/tests/test_fmtable.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_gregocal.py` & `icupy-0.9.0/tests/test_gregocal.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_icupy.py` & `icupy-0.9.0/tests/test_icupy.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_localebuilder.py` & `icupy-0.9.0/tests/test_localebuilder.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_localematcher.py` & `icupy-0.9.0/tests/test_localematcher.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_locid.py` & `icupy-0.9.0/tests/test_locid.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_measfmt.py` & `icupy-0.9.0/tests/test_measfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_measunit.py` & `icupy-0.9.0/tests/test_measunit.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_msgfmt.py` & `icupy-0.9.0/tests/test_msgfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_normalizer2.py` & `icupy-0.9.0/tests/test_normalizer2.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_numberformatter.py` & `icupy-0.9.0/tests/test_numberformatter.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_numberrangeformatter.py` & `icupy-0.9.0/tests/test_numberrangeformatter.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_numfmt.py` & `icupy-0.9.0/tests/test_numfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_plurfmt.py` & `icupy-0.9.0/tests/test_plurfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_plurrule.py` & `icupy-0.9.0/tests/test_plurrule.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_rbbi.py` & `icupy-0.9.0/tests/test_rbbi.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,21 +378,22 @@
     assert rules.length() > 0
 
 
 def test_get_text():
     bi = BreakIterator.create_word_instance(Locale.get_us())
 
     # CharacterIterator &icu::BreakIterator::getText(void)
-    it = bi.get_text()
-    assert it is None
+    # it = bi.get_text()  # Segmentation fault with Clang 12
+    # assert it is None
 
     src = UnicodeString("foo bar baz.")
     bi.set_text(src)
     it = bi.get_text()
     assert isinstance(it, CharacterIterator)
+
     dest = UnicodeString()
     it.get_text(dest)
     assert dest == src
 
 
 def test_get_utext():
     bi = BreakIterator.create_word_instance(Locale.get_us())
```

### Comparing `icupy-0.8.0.post2/tests/test_rbnf.py` & `icupy-0.9.0/tests/test_rbnf.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_regex_matcher.py` & `icupy-0.9.0/tests/test_regex_matcher.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_regex_pattern.py` & `icupy-0.9.0/tests/test_regex_pattern.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_resbund.py` & `icupy-0.9.0/tests/test_resbund.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_schriter.py` & `icupy-0.9.0/tests/test_schriter.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_selfmt.py` & `icupy-0.9.0/tests/test_selfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_smpdtfmt.py` & `icupy-0.9.0/tests/test_smpdtfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_sortkey.py` & `icupy-0.9.0/tests/test_sortkey.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_strenum.py` & `icupy-0.9.0/tests/test_strenum.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_stsearch.py` & `icupy-0.9.0/tests/test_stsearch.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_tblcoll.py` & `icupy-0.9.0/tests/test_tblcoll.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_timezone.py` & `icupy-0.9.0/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_tmunit.py` & `icupy-0.9.0/tests/test_tmunit.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_translit.py` & `icupy-0.9.0/tests/test_translit.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_tzfmt.py` & `icupy-0.9.0/tests/test_tzfmt.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_tznames.py` & `icupy-0.9.0/tests/test_tznames.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_tzrule.py` & `icupy-0.9.0/tests/test_tzrule.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_ubidi.py` & `icupy-0.9.0/tests/test_ubidi.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_uchar.py` & `icupy-0.9.0/tests/test_uchar.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_ucnv.py` & `icupy-0.9.0/tests/test_ucnv.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_ucsdet.py` & `icupy-0.9.0/tests/test_ucsdet.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_uenum.py` & `icupy-0.9.0/tests/test_uenum.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_uniset.py` & `icupy-0.9.0/tests/test_uniset.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_unistr.py` & `icupy-0.9.0/tests/test_unistr.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_uscript.py` & `icupy-0.9.0/tests/test_uscript.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_utext.py` & `icupy-0.9.0/tests/test_utext.py`

 * *Files identical despite different names*

### Comparing `icupy-0.8.0.post2/tests/test_uts46.py` & `icupy-0.9.0/tests/test_uts46.py`

 * *Files identical despite different names*

