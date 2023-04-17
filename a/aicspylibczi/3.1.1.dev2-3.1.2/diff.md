# Comparing `tmp/aicspylibczi-3.1.1.dev2.tar.gz` & `tmp/aicspylibczi-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicspylibczi-3.1.1.dev2.tar", last modified: Thu Apr 13 00:39:10 2023, max compression
+gzip compressed data, was "aicspylibczi-3.1.2.tar", last modified: Mon Apr 17 22:17:33 2023, max compression
```

## Comparing `aicspylibczi-3.1.1.dev2.tar` & `aicspylibczi-3.1.2.tar`

### file list

```diff
@@ -1,655 +1,665 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.890509 aicspylibczi-3.1.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-13 00:39:10.890509 aicspylibczi-3.1.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.810510 aicspylibczi-3.1.1.dev2/_aicspylibczi/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/CSimpleStreamImplFromFd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/CSimpleStreamImplFromFd.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/DimIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/DimIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/Image.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/ImageFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/ImageFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/ImagesContainer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/IndexMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/IndexMap.h
--rw-r--r--   0 runner    (1001) docker     (123)    22052 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/Reader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/Reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/SourceRange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/StreamImplLockingRead.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/StreamImplLockingRead.h
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/SubblockMetaVec.h
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/SubblockSortable.h
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/TargetRange.h
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/Threadpool.h
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/TypedImage.h
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/constants.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/helper_algorithms.h
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/inc_libCZI.h
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_BytesIO.h
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_DimIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_ImagesContainer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_SubblockMetaVec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_libCZI_DimensionIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pylibczi_ostream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/_aicspylibczi/pylibczi_ostream.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.810510 aicspylibczi-3.1.1.dev2/aicspylibczi/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/aicspylibczi/CziFile.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/aicspylibczi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/aicspylibczi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/aicspylibczi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.810510 aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-13 00:39:10.000000 aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-04-13 00:39:10.000000 aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:39:10.000000 aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:39:10.000000 aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-13 00:39:10.000000 aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 00:39:10.000000 aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.814509 aicspylibczi-3.1.1.dev2/libCZI/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 00:38:57.000000 aicspylibczi-3.1.1.dev2/libCZI/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.818509 aicspylibczi-3.1.1.dev2/libCZI/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.818509 aicspylibczi-3.1.1.dev2/libCZI/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.818509 aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/cla.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/reuse.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.mega-linter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.818509 aicspylibczi-3.1.1.dev2/libCZI/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/CPPLINT.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.818509 aicspylibczi-3.1.1.dev2/libCZI/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/LICENSES/RSA-MD.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.818509 aicspylibczi-3.1.1.dev2/libCZI/Src/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.822509 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   344178 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenFreeType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenFreeType.h
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenGdiplus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenGdiplus.h
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenNull.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenNull.h
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/CZIcmd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/CZIcmd_Config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/DisplaySettingsHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/IBitmapGen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/SaveBitmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/SaveBitmap.h
--rw-r--r--   0 runner    (1001) docker     (123)    70123 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/cmdlineoptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/cmdlineoptions.h
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/consoleio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/consoleio.h
--rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/execute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/execute.h
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/executeCreateCzi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/executeCreateCzi.h
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/inc_CZIcmd_Config.h
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/inc_libCZI.h
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/inc_rapidjson.h
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/platform_defines.h
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/stdafx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/stdafx.h
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/targetver.h
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)   124401 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.822509 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.830509 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/
--rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGlue.c
--rw-r--r--   0 runner    (1001) docker     (123)    29672 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGlue.h
--rw-r--r--   0 runner    (1001) docker     (123)    79862 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGlueJxr.c
--rw-r--r--   0 runner    (1001) docker     (123)    69235 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGluePFC.c
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRMeta.c
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRMeta.h
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTest.h
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestBmp.c
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestHdr.c
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestPnm.c
--rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestTif.c
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.c
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestYUV.c
--rw-r--r--   0 runner    (1001) docker     (123)    45760 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTranscode.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.830509 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/_x86/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/_x86/_x86.h
--rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/adapthuff.c
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/ansi.h
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/decode.c
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/decode.h
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/encode.c
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/encode.h
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/image.c
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/jxr_defines.h
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/perfTimer.h
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/perfTimerANSI.c
--rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/postprocess.c
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/priv_guiddef.h
--rw-r--r--   0 runner    (1001) docker     (123)    42889 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/segdec.c
--rw-r--r--   0 runner    (1001) docker     (123)    43079 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/segenc.c
--rw-r--r--   0 runner    (1001) docker     (123)    37192 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strFwdTransform.c
--rw-r--r--   0 runner    (1001) docker     (123)    66836 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strInvTransform.c
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strPredQuant.c
--rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strPredQuantDec.c
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strPredQuantEnc.c
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strTransform.c
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strTransform.h
--rw-r--r--   0 runner    (1001) docker     (123)    38332 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strcodec.c
--rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strcodec.h
--rw-r--r--   0 runner    (1001) docker     (123)   147549 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strdec.c
--rw-r--r--   0 runner    (1001) docker     (123)    50202 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strdec_x86.c
--rw-r--r--   0 runner    (1001) docker     (123)    95696 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strenc.c
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strenc_x86.c
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/windowsmediaphoto.h
--rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmsal.h
--rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstring.h
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_adt.h
--rw-r--r--   0 runner    (1001) docker     (123)    56756 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_strict.h
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_undef.h
--rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/JxrDecode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/JxrDecode.h
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/stdafx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/stdafx.h
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/targetver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.842509 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/
--rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/BitmapOperations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/BitmapOperations.h
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/BitmapOperations.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CZIReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CZIReader.h
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CreateBitmap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachment.h
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachmentsDirectory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachmentsDirectory.h
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDimensionInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDimensionInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDisplaySettings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDisplaySettings.h
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadata.h
--rw-r--r--   0 runner    (1001) docker     (123)    36205 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataBuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)    69987 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    40371 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.h
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataSegment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataSegment.h
--rw-r--r--   0 runner    (1001) docker     (123)    32099 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziParse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziParse.h
--rw-r--r--   0 runner    (1001) docker     (123)    36436 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziReaderWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziReaderWriter.h
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziStructs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziStructs.h
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlock.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlockDirectory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlockDirectory.h
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziUtils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)    58313 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziWriter.h
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/DimCoordinate.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.842509 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/
--rw-r--r--   0 runner    (1001) docker     (123)    24987 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/CZICmd_usage.markdown
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.846509 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/CZI_1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/CZI_2.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   629984 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png
--rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   508732 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   435548 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/Tinting-LUT.png
--rw-r--r--   0 runner    (1001) docker     (123)    95014 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/VisualStudio_cmake1.png
--rw-r--r--   0 runner    (1001) docker     (123)   947057 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   149904 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   242149 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   270106 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    59883 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/compositors_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/compositors_2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.846509 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/drawings/
--rw-r--r--   0 runner    (1001) docker     (123)   100864 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project.pub
--rw-r--r--   0 runner    (1001) docker     (123)   108032 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project_2.pub
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/gradationcurve_1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/gradationcurve_2.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept1.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept2.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept3.PNG
--rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept4.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Todos.markdown
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/accessors.markdown
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/building_libCZI.markdown
--rw-r--r--   0 runner    (1001) docker     (123)    92375 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/drawings.docx
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/image_document_concept.markdown
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/mainpage.markdown
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/multichannelcomposition.markdown
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/using_libCZI.markdown
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/write_czi.markdown
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/FileHeaderSegmentData.h
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/ImportExport.h
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/IndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/IndexSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/MD5Sum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/MD5Sum.h
--rw-r--r--   0 runner    (1001) docker     (123)    55139 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/MultiChannelCompositor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/MultiChannelCompositor.h
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelAccessorBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelAccessorBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.h
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelTileAccessor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelTileAccessor.h
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelTileCompositor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelTileCompositor.h
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Site.h
--rw-r--r--   0 runner    (1001) docker     (123)    19700 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/StreamImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/StreamImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/XmlNodeWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/bitmapData.h
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder.h
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_wic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_wic.h
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_zstd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_zstd.h
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/inc_libCZI_Config.h
--rw-r--r--   0 runner    (1001) docker     (123)    34770 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI.h
--rw-r--r--   0 runner    (1001) docker     (123)    29910 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Compositor.h
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_DimCoordinate.h
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Lib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    68869 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Metadata.h
--rw-r--r--   0 runner    (1001) docker     (123)    62344 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Metadata2.h
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Pixels.h
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_ReadWrite.h
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Site.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Site.h
--rw-r--r--   0 runner    (1001) docker     (123)    23328 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Utilities.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Utilities.h
--rw-r--r--   0 runner    (1001) docker     (123)    32167 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Write.h
--rw-r--r--   0 runner    (1001) docker     (123)    40279 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_compress.h
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/priv_guiddef.h
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/pugiconfig.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   385316 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/pugixml.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    58161 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/pugixml.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/splines.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/splines.h
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/stdAllocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/stdAllocator.h
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/stdafx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/stdafx.h
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/targetver.h
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/utilities.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/utilities.h
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/utilities_simd.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/zstdCompress.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.862509 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt.in
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.h
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemOutputStream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemOutputStream.h
--rw-r--r--   0 runner    (1001) docker     (123)   364946 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.h
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/SegmentWalker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/SegmentWalker.h
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/inc_libCZI.h
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/pch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/pch.h
--rw-r--r--   0 runner    (1001) docker     (123)  8401252 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImage.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImage.h
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImage1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImageHiLo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_CziSubBlockDirectory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_DimCoordinate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_DisplaySettings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_IndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_JxrDecode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_LUT.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_StreamImplementations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_Utilities.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_ZstdCompress.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_ZstdDecode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_bitmapOperations.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28041 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_metadatabuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25444 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_metadatareading.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_multichannelcomposite.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    44591 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_readerwriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_splines.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    79307 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   728991 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/THIRD_PARTY_LICENSES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/cla_corporate.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/cla_individual.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.862509 aicspylibczi-3.1.1.dev2/libCZI/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/cmake/ExternalEIGEN3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/cmake/TestLargeFile.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/cmake/check_can_use_neon_intrinsics.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/cmake/check_unaligned_access.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-13 00:38:58.000000 aicspylibczi-3.1.1.dev2/libCZI/opencppcoverage.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.862509 aicspylibczi-3.1.1.dev2/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.cmake-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.codespell-ignore-lines
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 00:38:57.000000 aicspylibczi-3.1.1.dev2/pybind11/.git
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.862509 aicspylibczi-3.1.1.dev2/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.862509 aicspylibczi-3.1.1.dev2/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.862509 aicspylibczi-3.1.1.dev2/pybind11/.github/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.866509 aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.866509 aicspylibczi-3.1.1.dev2/pybind11/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.790510 aicspylibczi-3.1.1.dev2/pybind11/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.866509 aicspylibczi-3.1.1.dev2/pybind11/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.866509 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.870509 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.870509 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)   114174 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/classes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.870509 aicspylibczi-3.1.1.dev2/pybind11/docs/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/cmake/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/compiling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61034 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.794510 aicspylibczi-3.1.1.dev2/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.870509 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.874509 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.874509 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.874509 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.874509 aicspylibczi-3.1.1.dev2/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/constructor_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/extra_python_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/extra_setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/local_bindings.h
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_async.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_call_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)    24874 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_class.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_const_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_copy_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.886509 aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_eval_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_iostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_modules.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_union.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:39:10.890509 aicspylibczi-3.1.1.dev2/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-13 00:38:59.000000 aicspylibczi-3.1.1.dev2/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-13 00:39:10.890509 aicspylibczi-3.1.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-13 00:38:55.000000 aicspylibczi-3.1.1.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.443935 aicspylibczi-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-17 22:17:33.443935 aicspylibczi-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.279928 aicspylibczi-3.1.2/_aicspylibczi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/CSimpleStreamImplFromFd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/CSimpleStreamImplFromFd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/DimIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/DimIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/Image.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/ImageFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/ImageFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/ImagesContainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/IndexMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/IndexMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22052 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/Reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/Reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/SourceRange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/StreamImplLockingRead.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/StreamImplLockingRead.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/SubblockMetaVec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/SubblockSortable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/TargetRange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/Threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/TypedImage.h
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/constants.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/helper_algorithms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/inc_libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_caster_BytesIO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_caster_DimIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_caster_ImagesContainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_caster_SubblockMetaVec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_caster_libCZI_DimensionIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pb_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pylibczi_ostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/_aicspylibczi/pylibczi_ostream.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.279928 aicspylibczi-3.1.2/aicspylibczi/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/aicspylibczi/CziFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/aicspylibczi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-17 22:17:13.000000 aicspylibczi-3.1.2/aicspylibczi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/aicspylibczi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.279928 aicspylibczi-3.1.2/aicspylibczi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-17 22:17:33.000000 aicspylibczi-3.1.2/aicspylibczi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22230 2023-04-17 22:17:33.000000 aicspylibczi-3.1.2/aicspylibczi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:17:33.000000 aicspylibczi-3.1.2/aicspylibczi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:17:33.000000 aicspylibczi-3.1.2/aicspylibczi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-17 22:17:33.000000 aicspylibczi-3.1.2/aicspylibczi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 22:17:33.000000 aicspylibczi-3.1.2/aicspylibczi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.283928 aicspylibczi-3.1.2/c_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   657410 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/test_DimIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/test_Image.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/test_Iterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24272 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/test_Reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/test_boundingboxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/c_tests/test_main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.287928 aicspylibczi-3.1.2/libCZI/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 22:17:16.000000 aicspylibczi-3.1.2/libCZI/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.287928 aicspylibczi-3.1.2/libCZI/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.287928 aicspylibczi-3.1.2/libCZI/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.287928 aicspylibczi-3.1.2/libCZI/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/workflows/cla.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/workflows/mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.github/workflows/reuse.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.mega-linter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.287928 aicspylibczi-3.1.2/libCZI/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/CPPLINT.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.291928 aicspylibczi-3.1.2/libCZI/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/LICENSES/RSA-MD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.291928 aicspylibczi-3.1.2/libCZI/Src/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.299928 aicspylibczi-3.1.2/libCZI/Src/CZICmd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   344178 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenFreeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenFreeType.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenGdiplus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenGdiplus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenNull.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenNull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/CZIcmd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/CZIcmd_Config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/DisplaySettingsHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/IBitmapGen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/SaveBitmap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/SaveBitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70123 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/cmdlineoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/cmdlineoptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/consoleio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/consoleio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/execute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/execute.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/executeCreateCzi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/executeCreateCzi.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/inc_CZIcmd_Config.h
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/inc_libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/inc_rapidjson.h
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/platform_defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/targetver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/CZICmd/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124401 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.299928 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.311929 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/
+-rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGlue.c
+-rw-r--r--   0 runner    (1001) docker     (123)    29672 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGlue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79862 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGlueJxr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69235 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGluePFC.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRMeta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRMeta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestBmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestHdr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestPnm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestTif.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestYUV.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45760 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTranscode.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.311929 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/_x86/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/_x86/_x86.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/adapthuff.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/ansi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/decode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/encode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/encode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/image.c
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/jxr_defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/perfTimer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/perfTimerANSI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/postprocess.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/priv_guiddef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42889 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/segdec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43079 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/segenc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    37192 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strFwdTransform.c
+-rw-r--r--   0 runner    (1001) docker     (123)    66836 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strInvTransform.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strPredQuant.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strPredQuantDec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strPredQuantEnc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strTransform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strTransform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38332 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strcodec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strcodec.h
+-rw-r--r--   0 runner    (1001) docker     (123)   147549 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strdec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    50202 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strdec_x86.c
+-rw-r--r--   0 runner    (1001) docker     (123)    95696 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strenc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strenc_x86.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/windowsmediaphoto.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmsal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_adt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56756 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_strict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_undef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/JxrDecode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/JxrDecode.h
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/JxrDecode/targetver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.343930 aicspylibczi-3.1.2/libCZI/Src/libCZI/
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/BitmapOperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/BitmapOperations.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/BitmapOperations.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CZIReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CZIReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CreateBitmap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachmentsDirectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachmentsDirectory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDimensionInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDimensionInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDisplaySettings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDisplaySettings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36205 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataBuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69987 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    40371 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataSegment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataSegment.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32099 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziParse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziParse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36436 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziReaderWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziReaderWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziStructs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziStructs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlockDirectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlockDirectory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziUtils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58313 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/CziWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/DimCoordinate.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.343930 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    24987 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/CZICmd_usage.markdown
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.355931 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/CZI_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/CZI_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   629984 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   508732 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   435548 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/Tinting-LUT.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95014 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/VisualStudio_cmake1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   947057 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   149904 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   242149 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   270106 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    59883 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/compositors_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/compositors_2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.355931 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/drawings/
+-rw-r--r--   0 runner    (1001) docker     (123)   100864 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project.pub
+-rw-r--r--   0 runner    (1001) docker     (123)   108032 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project_2.pub
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/gradationcurve_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/gradationcurve_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept3.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept4.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Todos.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/accessors.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/building_libCZI.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)    92375 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/drawings.docx
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/image_document_concept.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/mainpage.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/multichannelcomposition.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/using_libCZI.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/write_czi.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/FileHeaderSegmentData.h
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/ImportExport.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/IndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/IndexSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/MD5Sum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/MD5Sum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55139 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/MultiChannelCompositor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/MultiChannelCompositor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelAccessorBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelAccessorBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelTileAccessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelTileAccessor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelTileCompositor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelTileCompositor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/Site.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19700 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/StreamImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/StreamImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/XmlNodeWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/bitmapData.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_wic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_wic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_zstd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_zstd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/inc_libCZI_Config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34770 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29910 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Compositor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_DimCoordinate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    68869 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62344 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Metadata2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Pixels.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_ReadWrite.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Site.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Site.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23328 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Utilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Utilities.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32167 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Write.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40279 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_compress.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/priv_guiddef.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/pugiconfig.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   385316 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/pugixml.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    58161 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/pugixml.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/splines.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/splines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/stdAllocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/stdAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/targetver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/utilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/utilities.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/utilities_simd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI/zstdCompress.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.379932 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemOutputStream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemOutputStream.h
+-rw-r--r--   0 runner    (1001) docker     (123)   364946 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/SegmentWalker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/SegmentWalker.h
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/inc_libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/pch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/pch.h
+-rw-r--r--   0 runner    (1001) docker     (123)  8401252 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImage1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImageHiLo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_CziSubBlockDirectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_DimCoordinate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_DisplaySettings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_IndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_JxrDecode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_LUT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_StreamImplementations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_Utilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_ZstdCompress.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_ZstdDecode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_bitmapOperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28041 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_metadatabuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25444 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_metadatareading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_multichannelcomposite.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44591 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_readerwriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_splines.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    79307 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   728991 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/cla_corporate.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/cla_individual.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.379932 aicspylibczi-3.1.2/libCZI/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/cmake/ExternalEIGEN3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/cmake/TestLargeFile.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/cmake/check_can_use_neon_intrinsics.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/cmake/check_unaligned_access.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-17 22:17:18.000000 aicspylibczi-3.1.2/libCZI/opencppcoverage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.383932 aicspylibczi-3.1.2/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.cmake-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 22:17:17.000000 aicspylibczi-3.1.2/pybind11/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.387932 aicspylibczi-3.1.2/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.387932 aicspylibczi-3.1.2/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.387932 aicspylibczi-3.1.2/pybind11/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.387932 aicspylibczi-3.1.2/pybind11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.395933 aicspylibczi-3.1.2/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.263927 aicspylibczi-3.1.2/pybind11/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.395933 aicspylibczi-3.1.2/pybind11/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.395933 aicspylibczi-3.1.2/pybind11/docs/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.395933 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.399933 aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   114174 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.399933 aicspylibczi-3.1.2/pybind11/docs/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/compiling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61034 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.267927 aicspylibczi-3.1.2/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.403933 aicspylibczi-3.1.2/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.407933 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.407933 aicspylibczi-3.1.2/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.407933 aicspylibczi-3.1.2/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.411933 aicspylibczi-3.1.2/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.435934 aicspylibczi-3.1.2/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.435934 aicspylibczi-3.1.2/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.435934 aicspylibczi-3.1.2/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/local_bindings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24874 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_class.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.435934 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.435934 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.435934 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.435934 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.439934 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.439934 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.439934 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_const_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.439934 aicspylibczi-3.1.2/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:17:33.443935 aicspylibczi-3.1.2/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-17 22:17:19.000000 aicspylibczi-3.1.2/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-17 22:17:33.443935 aicspylibczi-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-17 22:17:14.000000 aicspylibczi-3.1.2/setup.py
```

### Comparing `aicspylibczi-3.1.1.dev2/CMakeLists.txt` & `aicspylibczi-3.1.2/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,24 +25,23 @@
     set(PYBIND11_CPP_STANDARD -std=c++14)
     SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread -std=c++14 -fPIC -O0 -g -D_FILE_OFFSET_BITS=64 -fvisibility=hidden")
     SET(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -D__ANSI__ -fPIC -D_FILE_OFFSET_BITS=64")
     add_compile_definitions(LINUXENV)
 
 ENDIF(WIN32)
 
-SET(pybind11_DIR pybind11)
+SET(pybind11_DIR ${CMAKE_CURRENT_LIST_DIR}/pybind11)
 
 add_compile_definitions(_LIBCZISTATICLIB)
 add_compile_definitions(LIBCZI_BUILD_UNITTESTS=OFF)
 add_compile_definitions(LIBCZI_BUILD_DYNLIB=OFF)
 add_compile_definitions(LIBCZI_BUILD_CZICMD=OFF)
 add_subdirectory(libCZI)
 add_subdirectory(pybind11)
 
-find_package(pybind11)
 message(STATUS "Found pybind11 v${pybind11_VERSION}: ${pybind11_INCLUDE_DIRS}")
 
 set(PYLIBCZI_C_SRC_HEADERS _aicspylibczi/Reader.h _aicspylibczi/helper_algorithms.h _aicspylibczi/exceptions.h _aicspylibczi/inc_libCZI.h
         _aicspylibczi/IndexMap.h _aicspylibczi/Image.h _aicspylibczi/TypedImage.h _aicspylibczi/ImageFactory.h
         _aicspylibczi/SourceRange.h _aicspylibczi/TargetRange.h _aicspylibczi/pylibczi_ostream.h
         _aicspylibczi/SubblockMetaVec.h _aicspylibczi/DimIndex.h _aicspylibczi/constants.h
         _aicspylibczi/StreamImplLockingRead.h _aicspylibczi/Threadpool.h)
```

### Comparing `aicspylibczi-3.1.1.dev2/CONTRIBUTING.md` & `aicspylibczi-3.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/LICENSE` & `aicspylibczi-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/PKG-INFO` & `aicspylibczi-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicspylibczi
-Version: 3.1.1.dev2
+Version: 3.1.2
 Summary: A python module and a python extension for Zeiss (CZI/ZISRAW) microscopy files.
 Home-page: https://github.com/AllenCellModeling/aicspylibczi
 Author: Jamie Sherman, Paul Watkins
 Author-email: jamies@alleninstitute.org, pwatkins@gmail.com
 Keywords: aicspylibczi,allen cell,imaging,computational biology
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aicspylibczi-3.1.1.dev2/README.md` & `aicspylibczi-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/CSimpleStreamImplFromFd.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/CSimpleStreamImplFromFd.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/CSimpleStreamImplFromFd.h` & `aicspylibczi-3.1.2/_aicspylibczi/CSimpleStreamImplFromFd.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/DimIndex.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/DimIndex.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/DimIndex.h` & `aicspylibczi-3.1.2/_aicspylibczi/DimIndex.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/Image.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/Image.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/Image.h` & `aicspylibczi-3.1.2/_aicspylibczi/Image.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/ImageFactory.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/ImageFactory.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/ImageFactory.h` & `aicspylibczi-3.1.2/_aicspylibczi/ImageFactory.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/ImagesContainer.h` & `aicspylibczi-3.1.2/_aicspylibczi/ImagesContainer.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/IndexMap.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/IndexMap.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/IndexMap.h` & `aicspylibczi-3.1.2/_aicspylibczi/IndexMap.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/Reader.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/Reader.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/Reader.h` & `aicspylibczi-3.1.2/_aicspylibczi/Reader.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/SourceRange.h` & `aicspylibczi-3.1.2/_aicspylibczi/SourceRange.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/StreamImplLockingRead.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/StreamImplLockingRead.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/StreamImplLockingRead.h` & `aicspylibczi-3.1.2/_aicspylibczi/StreamImplLockingRead.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/SubblockMetaVec.h` & `aicspylibczi-3.1.2/_aicspylibczi/SubblockMetaVec.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/SubblockSortable.h` & `aicspylibczi-3.1.2/_aicspylibczi/SubblockSortable.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/TargetRange.h` & `aicspylibczi-3.1.2/_aicspylibczi/TargetRange.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/Threadpool.h` & `aicspylibczi-3.1.2/_aicspylibczi/Threadpool.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/TypedImage.h` & `aicspylibczi-3.1.2/_aicspylibczi/TypedImage.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/constants.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/constants.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/exceptions.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/exceptions.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/exceptions.h` & `aicspylibczi-3.1.2/_aicspylibczi/exceptions.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/helper_algorithms.h` & `aicspylibczi-3.1.2/_aicspylibczi/helper_algorithms.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/inc_libCZI.h` & `aicspylibczi-3.1.2/_aicspylibczi/inc_libCZI.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_bindings.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/pb_bindings.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_BytesIO.h` & `aicspylibczi-3.1.2/_aicspylibczi/pb_caster_BytesIO.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_DimIndex.h` & `aicspylibczi-3.1.2/_aicspylibczi/pb_caster_DimIndex.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_ImagesContainer.h` & `aicspylibczi-3.1.2/_aicspylibczi/pb_caster_ImagesContainer.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_SubblockMetaVec.h` & `aicspylibczi-3.1.2/_aicspylibczi/pb_caster_SubblockMetaVec.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_caster_libCZI_DimensionIndex.h` & `aicspylibczi-3.1.2/_aicspylibczi/pb_caster_libCZI_DimensionIndex.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_helpers.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/pb_helpers.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pb_helpers.h` & `aicspylibczi-3.1.2/_aicspylibczi/pb_helpers.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/_aicspylibczi/pylibczi_ostream.cpp` & `aicspylibczi-3.1.2/_aicspylibczi/pylibczi_ostream.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/aicspylibczi/CziFile.py` & `aicspylibczi-3.1.2/aicspylibczi/CziFile.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/PKG-INFO` & `aicspylibczi-3.1.2/aicspylibczi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicspylibczi
-Version: 3.1.1.dev2
+Version: 3.1.2
 Summary: A python module and a python extension for Zeiss (CZI/ZISRAW) microscopy files.
 Home-page: https://github.com/AllenCellModeling/aicspylibczi
 Author: Jamie Sherman, Paul Watkins
 Author-email: jamies@alleninstitute.org, pwatkins@gmail.com
 Keywords: aicspylibczi,allen cell,imaging,computational biology
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/SOURCES.txt` & `aicspylibczi-3.1.2/aicspylibczi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CMakeLists.txt
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+main.cpp
 setup.cfg
 setup.py
 _aicspylibczi/CSimpleStreamImplFromFd.cpp
 _aicspylibczi/CSimpleStreamImplFromFd.h
 _aicspylibczi/DimIndex.cpp
 _aicspylibczi/DimIndex.h
 _aicspylibczi/Image.cpp
@@ -48,14 +49,22 @@
 aicspylibczi/types.py
 aicspylibczi.egg-info/PKG-INFO
 aicspylibczi.egg-info/SOURCES.txt
 aicspylibczi.egg-info/dependency_links.txt
 aicspylibczi.egg-info/not-zip-safe
 aicspylibczi.egg-info/requires.txt
 aicspylibczi.egg-info/top_level.txt
+c_tests/CMakeLists.txt
+c_tests/catch.hpp
+c_tests/test_DimIndex.cpp
+c_tests/test_Image.cpp
+c_tests/test_Iterator.cpp
+c_tests/test_Reader.cpp
+c_tests/test_boundingboxes.cpp
+c_tests/test_main.cpp
 libCZI/.editorconfig
 libCZI/.git
 libCZI/.gitignore
 libCZI/.mega-linter.yml
 libCZI/CMakeLists.txt
 libCZI/CODE_OF_CONDUCT.md
 libCZI/CONTRIBUTING.md
```

### Comparing `aicspylibczi-3.1.1.dev2/aicspylibczi.egg-info/requires.txt` & `aicspylibczi-3.1.2/aicspylibczi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.editorconfig` & `aicspylibczi-3.1.2/libCZI/.editorconfig`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/ISSUE_TEMPLATE/bug_report.md` & `aicspylibczi-3.1.2/libCZI/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/ISSUE_TEMPLATE/feature_request.md` & `aicspylibczi-3.1.2/libCZI/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/PULL_REQUEST_TEMPLATE.md` & `aicspylibczi-3.1.2/libCZI/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/cla.yml` & `aicspylibczi-3.1.2/libCZI/.github/workflows/cla.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/cmake.yml` & `aicspylibczi-3.1.2/libCZI/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/codeql.yml` & `aicspylibczi-3.1.2/libCZI/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/mega-linter.yml` & `aicspylibczi-3.1.2/libCZI/.github/workflows/mega-linter.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.github/workflows/pages.yml` & `aicspylibczi-3.1.2/libCZI/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.gitignore` & `aicspylibczi-3.1.2/libCZI/.gitignore`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.mega-linter.yml` & `aicspylibczi-3.1.2/libCZI/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/.reuse/dep5` & `aicspylibczi-3.1.2/libCZI/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/CMakeLists.txt` & `aicspylibczi-3.1.2/libCZI/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/CODE_OF_CONDUCT.md` & `aicspylibczi-3.1.2/libCZI/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/CONTRIBUTING.md` & `aicspylibczi-3.1.2/libCZI/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/COPYING` & `aicspylibczi-3.1.2/libCZI/COPYING`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/COPYING.LESSER` & `aicspylibczi-3.1.2/libCZI/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/CPPLINT.cfg` & `aicspylibczi-3.1.2/libCZI/CPPLINT.cfg`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/LICENSES/BSD-3-Clause.txt` & `aicspylibczi-3.1.2/libCZI/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/LICENSES/CC0-1.0.txt` & `aicspylibczi-3.1.2/libCZI/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/LICENSES/LGPL-3.0-or-later.txt` & `aicspylibczi-3.1.2/libCZI/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/LICENSES/MIT.txt` & `aicspylibczi-3.1.2/libCZI/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/LICENSES/RSA-MD.txt` & `aicspylibczi-3.1.2/libCZI/LICENSES/RSA-MD.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/README.md` & `aicspylibczi-3.1.2/libCZI/README.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/SECURITY.md` & `aicspylibczi-3.1.2/libCZI/SECURITY.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGen.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGen.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenFreeType.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenFreeType.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenFreeType.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenFreeType.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenGdiplus.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenGdiplus.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenGdiplus.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenGdiplus.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenNull.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenNull.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/BitmapGenNull.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/BitmapGenNull.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/CMakeLists.txt` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/CZIcmd.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/CZIcmd.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/DisplaySettingsHelper.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/DisplaySettingsHelper.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/IBitmapGen.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/IBitmapGen.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/SaveBitmap.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/SaveBitmap.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/SaveBitmap.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/SaveBitmap.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/cmdlineoptions.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/cmdlineoptions.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/cmdlineoptions.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/cmdlineoptions.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/consoleio.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/consoleio.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/consoleio.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/consoleio.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/execute.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/execute.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/executeCreateCzi.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/executeCreateCzi.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/stdafx.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/stdafx.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/utils.cpp` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/utils.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/CZICmd/utils.h` & `aicspylibczi-3.1.2/libCZI/Src/CZICmd/utils.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/Doxyfile` & `aicspylibczi-3.1.2/libCZI/Src/Doxyfile`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/CMakeLists.txt` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGlue.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGlue.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGlue.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGlue.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGlueJxr.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGlueJxr.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRGluePFC.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRGluePFC.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRMeta.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRMeta.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRMeta.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRMeta.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTest.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTest.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTest.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTest.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestBmp.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestBmp.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestHdr.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestHdr.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestPnm.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestPnm.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestTif.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestTif.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTestYUV.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTestYUV.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/JXRTranscode.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/JXRTranscode.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/_x86/_x86.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/_x86/_x86.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/adapthuff.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/adapthuff.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/ansi.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/ansi.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/common.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/common.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/decode.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/decode.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/decode.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/decode.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/encode.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/encode.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/encode.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/encode.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/image.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/image.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/perfTimer.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/perfTimer.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/perfTimerANSI.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/perfTimerANSI.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/postprocess.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/postprocess.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/priv_guiddef.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/priv_guiddef.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/segdec.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/segdec.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/segenc.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/segenc.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strFwdTransform.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strFwdTransform.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strInvTransform.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strInvTransform.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strPredQuant.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strPredQuant.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strPredQuantDec.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strPredQuantDec.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strPredQuantEnc.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strPredQuantEnc.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strTransform.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strTransform.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strTransform.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strTransform.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strcodec.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strcodec.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strcodec.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strcodec.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strdec.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strdec.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strdec_x86.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strdec_x86.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strenc.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strenc.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/strenc_x86.c` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/strenc_x86.c`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/windowsmediaphoto.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/windowsmediaphoto.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmsal.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmsal.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstring.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstring.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_adt.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_adt.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_strict.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_strict.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_undef.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/Jxr/wmspecstrings_undef.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/JxrDecode.cpp` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/JxrDecode.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/JxrDecode/JxrDecode.h` & `aicspylibczi-3.1.2/libCZI/Src/JxrDecode/JxrDecode.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/BitmapOperations.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/BitmapOperations.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/BitmapOperations.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/BitmapOperations.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/BitmapOperations.hpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/BitmapOperations.hpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CMakeLists.txt` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CZIReader.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CZIReader.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CZIReader.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CZIReader.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CreateBitmap.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CreateBitmap.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachment.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachment.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachment.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachment.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachmentsDirectory.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachmentsDirectory.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziAttachmentsDirectory.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziAttachmentsDirectory.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDimensionInfo.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDimensionInfo.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDimensionInfo.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDimensionInfo.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDisplaySettings.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDisplaySettings.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziDisplaySettings.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziDisplaySettings.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadata.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadata.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadata.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadata.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataBuilder.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataBuilder.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataBuilder.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataBuilder.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataDocumentInfo2.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataSegment.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataSegment.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziMetadataSegment.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziMetadataSegment.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziParse.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziParse.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziParse.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziParse.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziReaderWriter.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziReaderWriter.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziReaderWriter.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziReaderWriter.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziStructs.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziStructs.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziStructs.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziStructs.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlock.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlock.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlock.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlock.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlockDirectory.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlockDirectory.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziSubBlockDirectory.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziSubBlockDirectory.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziUtils.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziUtils.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziUtils.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziUtils.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziWriter.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziWriter.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/CziWriter.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/CziWriter.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/DimCoordinate.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/DimCoordinate.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/CZICmd_usage.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/CZICmd_usage.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/CZI_1.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/CZI_1.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/CZI_2.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/CZI_2.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/Tinting-LUT.png` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/Tinting-LUT.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/VisualStudio_cmake1.png` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/VisualStudio_cmake1.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/compositors_1.png` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/compositors_1.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/compositors_2.png` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/compositors_2.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project.pub` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project.pub`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project_2.pub` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/drawings/VS-project_2.pub`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/gradationcurve_1.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/gradationcurve_1.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/gradationcurve_2.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/gradationcurve_2.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept1.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept1.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept2.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept2.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept3.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept3.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Images/image_document_concept4.PNG` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Images/image_document_concept4.PNG`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/Todos.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/Todos.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/accessors.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/accessors.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/building_libCZI.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/building_libCZI.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/drawings.docx` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/drawings.docx`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/image_document_concept.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/image_document_concept.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/mainpage.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/mainpage.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/multichannelcomposition.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/multichannelcomposition.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/using_libCZI.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/using_libCZI.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/Doc/write_czi.markdown` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/Doc/write_czi.markdown`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/FileHeaderSegmentData.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/FileHeaderSegmentData.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/ImportExport.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/ImportExport.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/IndexSet.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/IndexSet.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/IndexSet.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/IndexSet.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/MD5Sum.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/MD5Sum.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/MD5Sum.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/MD5Sum.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/MultiChannelCompositor.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/MultiChannelCompositor.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelAccessorBase.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelAccessorBase.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelAccessorBase.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelAccessorBase.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelTileAccessor.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelTileAccessor.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelTileAccessor.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/SingleChannelTileCompositor.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/SingleChannelTileCompositor.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/StreamImpl.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/StreamImpl.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/StreamImpl.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/StreamImpl.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/XmlNodeWrapper.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/XmlNodeWrapper.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/bitmapData.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/bitmapData.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_wic.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_wic.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_wic.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_wic.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_zstd.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_zstd.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/decoder_zstd.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/decoder_zstd.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Compositor.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Compositor.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Config.h.in` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Config.h.in`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_DimCoordinate.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_DimCoordinate.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Helpers.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Helpers.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Lib.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Lib.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Metadata.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Metadata.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Metadata2.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Metadata2.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Pixels.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Pixels.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_ReadWrite.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_ReadWrite.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Site.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Site.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Site.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Site.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Utilities.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Utilities.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Utilities.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Utilities.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_Write.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_Write.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_compress.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_compress.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/libCZI_exceptions.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/libCZI_exceptions.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/priv_guiddef.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/priv_guiddef.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/pugiconfig.hpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/pugiconfig.hpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/pugixml.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/pugixml.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/pugixml.hpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/pugixml.hpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/splines.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/splines.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/splines.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/splines.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/stdAllocator.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/stdAllocator.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/stdAllocator.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/stdAllocator.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/stdafx.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/stdafx.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/utilities.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/utilities.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/utilities.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/utilities.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/utilities_simd.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/utilities_simd.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI/zstdCompress.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI/zstdCompress.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt.in` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/CMakeLists.txt.in`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemOutputStream.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemOutputStream.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MemOutputStream.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MemOutputStream.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/SegmentWalker.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/SegmentWalker.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/SegmentWalker.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/SegmentWalker.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImage.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImage.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImage.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImage.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImage1.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImage1.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/testImageHiLo.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/testImageHiLo.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_CziSubBlockDirectory.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_CziSubBlockDirectory.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_DimCoordinate.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_DimCoordinate.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_DisplaySettings.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_DisplaySettings.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_IndexSet.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_IndexSet.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_JxrDecode.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_JxrDecode.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_LUT.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_LUT.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_StreamImplementations.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_StreamImplementations.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_Utilities.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_Utilities.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_ZstdCompress.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_ZstdCompress.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_ZstdDecode.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_ZstdDecode.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_bitmapOperations.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_bitmapOperations.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_metadatabuilder.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_metadatabuilder.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_metadatareading.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_metadatareading.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_multichannelcomposite.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_multichannelcomposite.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_reader.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_reader.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_readerwriter.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_readerwriter.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_splines.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_splines.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/test_writer.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/test_writer.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/utils.cpp` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/utils.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/Src/libCZI_UnitTests/utils.h` & `aicspylibczi-3.1.2/libCZI/Src/libCZI_UnitTests/utils.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/THIRD_PARTY_LICENSES.txt` & `aicspylibczi-3.1.2/libCZI/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/cla_corporate.txt` & `aicspylibczi-3.1.2/libCZI/cla_corporate.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/cla_individual.txt` & `aicspylibczi-3.1.2/libCZI/cla_individual.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/cmake/ExternalEIGEN3.cmake` & `aicspylibczi-3.1.2/libCZI/cmake/ExternalEIGEN3.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/cmake/TestLargeFile.cmake` & `aicspylibczi-3.1.2/libCZI/cmake/TestLargeFile.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/cmake/check_can_use_neon_intrinsics.cmake` & `aicspylibczi-3.1.2/libCZI/cmake/check_can_use_neon_intrinsics.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/libCZI/cmake/check_unaligned_access.cmake` & `aicspylibczi-3.1.2/libCZI/cmake/check_unaligned_access.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.appveyor.yml` & `aicspylibczi-3.1.2/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.clang-format` & `aicspylibczi-3.1.2/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.clang-tidy` & `aicspylibczi-3.1.2/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.cmake-format.yaml` & `aicspylibczi-3.1.2/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.codespell-ignore-lines` & `aicspylibczi-3.1.2/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/CONTRIBUTING.md` & `aicspylibczi-3.1.2/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `aicspylibczi-3.1.2/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/matchers/pylint.json` & `aicspylibczi-3.1.2/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/pull_request_template.md` & `aicspylibczi-3.1.2/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/ci.yml` & `aicspylibczi-3.1.2/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/configure.yml` & `aicspylibczi-3.1.2/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/format.yml` & `aicspylibczi-3.1.2/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/labeler.yml` & `aicspylibczi-3.1.2/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/pip.yml` & `aicspylibczi-3.1.2/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.github/workflows/upstream.yml` & `aicspylibczi-3.1.2/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/.pre-commit-config.yaml` & `aicspylibczi-3.1.2/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/LICENSE` & `aicspylibczi-3.1.2/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/README.rst` & `aicspylibczi-3.1.2/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/Doxyfile` & `aicspylibczi-3.1.2/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/Makefile` & `aicspylibczi-3.1.2/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/chrono.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/custom.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/eigen.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/functional.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/index.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/overview.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/stl.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/cast/strings.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/classes.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/embedding.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/exceptions.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/functions.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/misc.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/numpy.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/object.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/pycpp/utilities.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/advanced/smart_ptrs.rst` & `aicspylibczi-3.1.2/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/basics.rst` & `aicspylibczi-3.1.2/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/benchmark.py` & `aicspylibczi-3.1.2/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/benchmark.rst` & `aicspylibczi-3.1.2/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/changelog.rst` & `aicspylibczi-3.1.2/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/classes.rst` & `aicspylibczi-3.1.2/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/compiling.rst` & `aicspylibczi-3.1.2/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/conf.py` & `aicspylibczi-3.1.2/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/faq.rst` & `aicspylibczi-3.1.2/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/index.rst` & `aicspylibczi-3.1.2/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/installing.rst` & `aicspylibczi-3.1.2/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/limitations.rst` & `aicspylibczi-3.1.2/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11-logo.png` & `aicspylibczi-3.1.2/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python1.png` & `aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python1.svg` & `aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python2.png` & `aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/pybind11_vs_boost_python2.svg` & `aicspylibczi-3.1.2/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/reference.rst` & `aicspylibczi-3.1.2/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/release.rst` & `aicspylibczi-3.1.2/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/docs/upgrade.rst` & `aicspylibczi-3.1.2/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/attr.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/buffer_info.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/cast.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/chrono.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/complex.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/class.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/common.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/descr.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/init.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/internals.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/type_caster_base.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/detail/typeid.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eigen/matrix.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eigen/tensor.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/embed.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/eval.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/functional.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/gil.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/iostream.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/numpy.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/operators.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/options.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/pybind11.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/pytypes.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/stl/filesystem.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/stl.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/include/pybind11/stl_bind.h` & `aicspylibczi-3.1.2/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/noxfile.py` & `aicspylibczi-3.1.2/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/pybind11/__main__.py` & `aicspylibczi-3.1.2/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/pybind11/commands.py` & `aicspylibczi-3.1.2/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/pybind11/setup_helpers.py` & `aicspylibczi-3.1.2/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/pyproject.toml` & `aicspylibczi-3.1.2/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/setup.cfg` & `aicspylibczi-3.1.2/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/setup.py` & `aicspylibczi-3.1.2/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/conftest.py` & `aicspylibczi-3.1.2/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/constructor_stats.h` & `aicspylibczi-3.1.2/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/cross_module_gil_utils.cpp` & `aicspylibczi-3.1.2/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `aicspylibczi-3.1.2/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/env.py` & `aicspylibczi-3.1.2/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/extra_python_package/test_files.py` & `aicspylibczi-3.1.2/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/extra_setuptools/test_setuphelper.py` & `aicspylibczi-3.1.2/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/local_bindings.h` & `aicspylibczi-3.1.2/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/object.h` & `aicspylibczi-3.1.2/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/pybind11_cross_module_tests.cpp` & `aicspylibczi-3.1.2/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/pybind11_tests.cpp` & `aicspylibczi-3.1.2/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/pybind11_tests.h` & `aicspylibczi-3.1.2/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/pytest.ini` & `aicspylibczi-3.1.2/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/requirements.txt` & `aicspylibczi-3.1.2/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_async.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_async.py` & `aicspylibczi-3.1.2/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_buffers.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_buffers.py` & `aicspylibczi-3.1.2/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_builtin_casters.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_builtin_casters.py` & `aicspylibczi-3.1.2/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_call_policies.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_call_policies.py` & `aicspylibczi-3.1.2/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_callbacks.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_callbacks.py` & `aicspylibczi-3.1.2/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_chrono.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_chrono.py` & `aicspylibczi-3.1.2/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_class.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_class.py` & `aicspylibczi-3.1.2/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/embed.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_const_name.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_const_name.py` & `aicspylibczi-3.1.2/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_constants_and_functions.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_constants_and_functions.py` & `aicspylibczi-3.1.2/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_copy_move.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_copy_move.py` & `aicspylibczi-3.1.2/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_casters.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_casters.py` & `aicspylibczi-3.1.2/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_setup.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_custom_type_setup.py` & `aicspylibczi-3.1.2/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_docstring_options.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_docstring_options.py` & `aicspylibczi-3.1.2/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_matrix.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_matrix.py` & `aicspylibczi-3.1.2/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_tensor.inl` & `aicspylibczi-3.1.2/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_eigen_tensor.py` & `aicspylibczi-3.1.2/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/CMakeLists.txt` & `aicspylibczi-3.1.2/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/catch.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/external_module.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_embed/test_interpreter.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_enum.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_enum.py` & `aicspylibczi-3.1.2/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_eval.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_eval.py` & `aicspylibczi-3.1.2/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_exceptions.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_exceptions.py` & `aicspylibczi-3.1.2/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_factory_constructors.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_factory_constructors.py` & `aicspylibczi-3.1.2/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_gil_scoped.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_gil_scoped.py` & `aicspylibczi-3.1.2/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_iostream.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_iostream.py` & `aicspylibczi-3.1.2/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_kwargs_and_defaults.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_kwargs_and_defaults.py` & `aicspylibczi-3.1.2/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_local_bindings.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_local_bindings.py` & `aicspylibczi-3.1.2/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_methods_and_attributes.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_methods_and_attributes.py` & `aicspylibczi-3.1.2/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_modules.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_modules.py` & `aicspylibczi-3.1.2/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_multiple_inheritance.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_multiple_inheritance.py` & `aicspylibczi-3.1.2/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_array.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_array.py` & `aicspylibczi-3.1.2/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_dtypes.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_dtypes.py` & `aicspylibczi-3.1.2/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_vectorize.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_numpy_vectorize.py` & `aicspylibczi-3.1.2/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_opaque_types.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_opaque_types.py` & `aicspylibczi-3.1.2/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_operator_overloading.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_operator_overloading.py` & `aicspylibczi-3.1.2/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_pickling.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_pickling.py` & `aicspylibczi-3.1.2/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_pytypes.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_pytypes.py` & `aicspylibczi-3.1.2/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_sequences_and_iterators.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_sequences_and_iterators.py` & `aicspylibczi-3.1.2/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_smart_ptr.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_smart_ptr.py` & `aicspylibczi-3.1.2/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl.py` & `aicspylibczi-3.1.2/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl_binders.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_stl_binders.py` & `aicspylibczi-3.1.2/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_tagbased_polymorphic.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_tagbased_polymorphic.py` & `aicspylibczi-3.1.2/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_thread.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_thread.py` & `aicspylibczi-3.1.2/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_union.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_virtual_functions.cpp` & `aicspylibczi-3.1.2/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/test_virtual_functions.py` & `aicspylibczi-3.1.2/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/valgrind-numpy-scipy.supp` & `aicspylibczi-3.1.2/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tests/valgrind-python.supp` & `aicspylibczi-3.1.2/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/FindCatch.cmake` & `aicspylibczi-3.1.2/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/FindEigen3.cmake` & `aicspylibczi-3.1.2/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/FindPythonLibsNew.cmake` & `aicspylibczi-3.1.2/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/JoinPaths.cmake` & `aicspylibczi-3.1.2/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/check-style.sh` & `aicspylibczi-3.1.2/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/cmake_uninstall.cmake.in` & `aicspylibczi-3.1.2/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/codespell_ignore_lines_from_errors.py` & `aicspylibczi-3.1.2/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/libsize.py` & `aicspylibczi-3.1.2/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/make_changelog.py` & `aicspylibczi-3.1.2/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11Common.cmake` & `aicspylibczi-3.1.2/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11Config.cmake.in` & `aicspylibczi-3.1.2/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11NewTools.cmake` & `aicspylibczi-3.1.2/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/pybind11Tools.cmake` & `aicspylibczi-3.1.2/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/setup_global.py.in` & `aicspylibczi-3.1.2/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/pybind11/tools/setup_main.py.in` & `aicspylibczi-3.1.2/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.1.dev2/setup.cfg` & `aicspylibczi-3.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.1.1.dev2
+current_version = 3.1.2
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `aicspylibczi-3.1.1.dev2/setup.py` & `aicspylibczi-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call(['cmake', '--build', '.', '--target', '_aicspylibczi'] + build_args, cwd=self.build_temp, env=env)
 
 setup(
     name='aicspylibczi',
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.md
-    version='3.1.1.dev2',
+    version='3.1.2',
     author='Jamie Sherman, Paul Watkins',
     author_email='jamies@alleninstitute.org, pwatkins@gmail.com',
     description='A python module and a python extension for Zeiss (CZI/ZISRAW) microscopy files.',
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="aicspylibczi, allen cell, imaging, computational biology",
```

