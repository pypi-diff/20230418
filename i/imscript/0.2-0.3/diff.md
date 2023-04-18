# Comparing `tmp/imscript-0.2.tar.gz` & `tmp/imscript-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imscript-0.2.tar", last modified: Fri Apr 14 07:26:57 2023, max compression
+gzip compressed data, was "imscript-0.3.tar", last modified: Tue Apr 18 09:51:40 2023, max compression
```

## Comparing `imscript-0.2.tar` & `imscript-0.3.tar`

### file list

```diff
@@ -1,11 +1,140 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-14 07:26:57.825003 imscript-0.2/
--rw-rw-r--   0 coco      (1000) coco      (1000)       10 2023-04-14 07:25:46.000000 imscript-0.2/MANIFEST.in
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-14 07:26:57.825003 imscript-0.2/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.2/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-14 07:26:57.821003 imscript-0.2/imscript.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      155 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/top_level.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-04-14 07:26:57.825003 imscript-0.2/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      780 2023-04-14 07:25:46.000000 imscript-0.2/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-18 09:51:40.837712 imscript-0.3/
+-rw-rw-r--   0 coco      (1000) coco      (1000)       59 2023-04-18 09:51:25.000000 imscript-0.3/MANIFEST.in
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6218 2023-03-20 09:48:02.000000 imscript-0.3/Makefile
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-18 09:51:40.837712 imscript-0.3/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.3/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-18 09:51:40.821712 imscript-0.3/imscript.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-18 09:51:40.000000 imscript-0.3/imscript.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2019 2023-04-18 09:51:40.000000 imscript-0.3/imscript.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-18 09:51:40.000000 imscript-0.3/imscript.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-18 09:51:40.000000 imscript-0.3/imscript.egg-info/top_level.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-04-18 09:51:40.837712 imscript-0.3/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      780 2023-04-18 09:50:23.000000 imscript-0.3/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-18 09:51:40.837712 imscript-0.3/src/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      911 2017-10-23 14:34:44.000000 imscript-0.3/src/abstract_dsf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      689 2017-10-23 14:34:44.000000 imscript-0.3/src/abstract_dsf.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5374 2017-10-23 14:34:44.000000 imscript-0.3/src/abstract_heap.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8946 2022-11-07 09:50:33.000000 imscript-0.3/src/amle.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2129 2018-02-16 16:28:06.000000 imscript-0.3/src/autotrim.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4987 2019-05-07 13:07:56.000000 imscript-0.3/src/backflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      825 2022-02-25 16:40:51.000000 imscript-0.3/src/bandslice.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5426 2022-11-07 09:50:33.000000 imscript-0.3/src/bdint.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2510 2017-10-23 14:34:44.000000 imscript-0.3/src/bicubic.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1471 2017-10-23 14:34:44.000000 imscript-0.3/src/bicubic_gray.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3011 2017-10-23 14:34:44.000000 imscript-0.3/src/bilinear_interpolation.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    13982 2020-01-10 14:32:47.000000 imscript-0.3/src/blur.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     9431 2018-02-16 16:26:37.000000 imscript-0.3/src/bmms.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5726 2021-04-23 16:53:33.000000 imscript-0.3/src/carve.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    18033 2018-12-02 15:33:58.000000 imscript-0.3/src/ccproc.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      783 2017-10-23 14:34:44.000000 imscript-0.3/src/ccproc.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2529 2017-10-23 14:34:44.000000 imscript-0.3/src/censust.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7642 2019-12-18 13:54:29.000000 imscript-0.3/src/cleant_cgpois.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2238 2017-11-12 08:49:58.000000 imscript-0.3/src/colorcoordsf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4044 2017-11-24 18:26:29.000000 imscript-0.3/src/colormatch.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14726 2022-11-07 09:50:33.000000 imscript-0.3/src/contihist.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1535 2018-04-25 10:33:08.000000 imscript-0.3/src/crop.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      141 2020-04-06 13:26:01.000000 imscript-0.3/src/d5.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    13607 2018-02-16 16:03:22.000000 imscript-0.3/src/dataconv.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2113 2017-10-23 14:34:44.000000 imscript-0.3/src/dct.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1956 2017-10-23 14:34:44.000000 imscript-0.3/src/dht.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5142 2022-11-02 07:40:05.000000 imscript-0.3/src/dither.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5017 2020-01-10 14:33:49.000000 imscript-0.3/src/downsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3508 2019-07-16 11:46:25.000000 imscript-0.3/src/drawsegment.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2448 2017-10-23 14:34:44.000000 imscript-0.3/src/drawtriangle.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2591 2018-11-17 18:44:45.000000 imscript-0.3/src/eucdist.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8492 2017-10-23 14:34:44.000000 imscript-0.3/src/exterior_algebra.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1794 2017-10-23 14:34:44.000000 imscript-0.3/src/extrapolators.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1628 2022-11-07 15:14:20.000000 imscript-0.3/src/fail.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1418 2018-02-16 16:27:35.000000 imscript-0.3/src/fancy_crop.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3506 2018-02-16 16:27:51.000000 imscript-0.3/src/fancy_downsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    20717 2022-07-13 12:27:58.000000 imscript-0.3/src/fancy_image.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4280 2018-10-19 07:13:31.000000 imscript-0.3/src/fancy_image.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7059 2023-04-07 10:19:22.000000 imscript-0.3/src/fft.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1379 2017-10-23 14:34:44.000000 imscript-0.3/src/fftshift.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    84778 2021-06-03 13:20:54.000000 imscript-0.3/src/flambda.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3235 2018-07-10 14:32:43.000000 imscript-0.3/src/flowarrows.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3618 2018-02-16 16:16:06.000000 imscript-0.3/src/flowinv.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    24129 2023-03-20 09:45:46.000000 imscript-0.3/src/fontu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    32612 2021-06-28 07:40:10.000000 imscript-0.3/src/geomedian.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1604 2021-07-23 15:12:25.000000 imscript-0.3/src/getbands.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4854 2019-04-15 16:46:40.000000 imscript-0.3/src/getpixel.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5688 2022-11-02 07:40:05.000000 imscript-0.3/src/ghisto.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8043 2018-01-03 11:41:10.000000 imscript-0.3/src/gntiply.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1702 2017-10-23 14:34:44.000000 imscript-0.3/src/gram_schmidt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3144 2017-10-23 14:34:44.000000 imscript-0.3/src/grid.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3798 2018-03-22 08:54:00.000000 imscript-0.3/src/heatd.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1127 2018-02-16 18:36:16.000000 imscript-0.3/src/help_stuff.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2848 2017-10-23 14:34:44.000000 imscript-0.3/src/homographies.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6286 2022-02-23 15:28:45.000000 imscript-0.3/src/homwarp.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1039 2018-02-07 17:22:02.000000 imscript-0.3/src/idump.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)   183486 2022-11-24 17:47:57.000000 imscript-0.3/src/iio.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8888 2022-05-24 10:44:02.000000 imscript-0.3/src/iio.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3023 2023-01-23 08:50:42.000000 imscript-0.3/src/iion.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      626 2020-02-07 12:37:20.000000 imscript-0.3/src/iion_int.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      753 2022-11-07 09:50:33.000000 imscript-0.3/src/iion_pure.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      824 2017-10-23 14:34:44.000000 imscript-0.3/src/iion_u16.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      253 2021-03-16 15:08:51.000000 imscript-0.3/src/im.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5683 2020-01-10 14:32:38.000000 imscript-0.3/src/imflip.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      338 2020-01-30 09:53:05.000000 imscript-0.3/src/imhalve.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    23117 2020-01-10 14:32:44.000000 imscript-0.3/src/imprintf.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2968 2021-06-15 10:19:21.000000 imscript-0.3/src/linalg.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3661 2022-11-02 07:40:05.000000 imscript-0.3/src/lrcat.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6290 2018-02-16 16:14:16.000000 imscript-0.3/src/marching_interpolation.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2962 2017-10-23 14:34:44.000000 imscript-0.3/src/marching_squares.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7313 2019-01-08 11:10:02.000000 imscript-0.3/src/mdither.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7482 2019-01-08 11:10:15.000000 imscript-0.3/src/mdither2.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7327 2018-11-23 08:20:02.000000 imscript-0.3/src/mdither3.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      193 2017-11-30 11:51:08.000000 imscript-0.3/src/means.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6215 2017-11-01 15:45:05.000000 imscript-0.3/src/mediator.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1756 2017-10-23 14:34:44.000000 imscript-0.3/src/minicg.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    11894 2018-07-10 14:32:17.000000 imscript-0.3/src/modes_detector.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17399 2022-11-07 14:49:50.000000 imscript-0.3/src/moistiv_epipolar.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    15593 2023-02-16 15:39:37.000000 imscript-0.3/src/morsi.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7493 2022-11-02 08:49:14.000000 imscript-0.3/src/nnint.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1938 2017-12-30 15:31:26.000000 imscript-0.3/src/nonmaxsup.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      765 2017-10-23 14:34:44.000000 imscript-0.3/src/ntiply.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      162 2017-12-12 13:31:10.000000 imscript-0.3/src/numbersio.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    12436 2017-10-23 14:34:44.000000 imscript-0.3/src/ok_list.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17774 2023-01-24 10:59:47.000000 imscript-0.3/src/palette.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4036 2020-12-06 18:05:01.000000 imscript-0.3/src/parsenumbers.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1252 2017-11-13 14:55:57.000000 imscript-0.3/src/pickopt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      450 2020-02-13 08:44:15.000000 imscript-0.3/src/pixdump.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)   104566 2023-04-07 10:24:56.000000 imscript-0.3/src/plambda.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4668 2021-06-23 14:55:11.000000 imscript-0.3/src/points.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8894 2020-03-09 14:57:59.000000 imscript-0.3/src/ppsmooth.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    29708 2021-12-09 13:36:31.000000 imscript-0.3/src/pview.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    96888 2021-06-14 15:31:43.000000 imscript-0.3/src/pλ.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5168 2022-04-21 08:24:03.000000 imscript-0.3/src/qauto.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2227 2022-11-02 08:48:01.000000 imscript-0.3/src/qeasy.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3944 2023-02-21 16:29:17.000000 imscript-0.3/src/random.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17472 2017-10-23 14:34:44.000000 imscript-0.3/src/ransac.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    24327 2019-05-07 10:03:01.000000 imscript-0.3/src/ransac_cases.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1265 2018-05-31 18:07:33.000000 imscript-0.3/src/redim.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4984 2017-10-23 14:34:44.000000 imscript-0.3/src/registration.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    21672 2023-03-20 12:53:49.000000 imscript-0.3/src/rpc2.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6501 2019-02-23 19:54:59.000000 imscript-0.3/src/rpcfit33.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8640 2021-05-27 20:42:20.000000 imscript-0.3/src/rpctk.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    12960 2019-02-08 09:45:19.000000 imscript-0.3/src/rpctk_old.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      460 2017-10-23 14:34:44.000000 imscript-0.3/src/seconds.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    40509 2022-11-07 15:00:57.000000 imscript-0.3/src/siftie.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    15912 2017-10-23 14:34:44.000000 imscript-0.3/src/siftu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    13108 2022-11-07 09:50:33.000000 imscript-0.3/src/simpois.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1349 2018-08-24 10:55:52.000000 imscript-0.3/src/smapa.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)    10832 2018-02-16 16:10:48.000000 imscript-0.3/src/spline.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6230 2020-12-04 11:17:12.000000 imscript-0.3/src/srmatch.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5886 2017-10-23 14:34:44.000000 imscript-0.3/src/strt.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1376 2017-10-23 14:34:44.000000 imscript-0.3/src/synflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    29109 2018-02-16 16:35:04.000000 imscript-0.3/src/synflow_core.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     3652 2022-11-02 07:40:05.000000 imscript-0.3/src/tbcat.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    23780 2022-11-07 15:01:37.000000 imscript-0.3/src/tiff_octaves_rw.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    73306 2022-11-07 14:55:30.000000 imscript-0.3/src/tiffu.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4488 2018-07-11 18:56:13.000000 imscript-0.3/src/upsa.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17626 2021-07-19 17:20:01.000000 imscript-0.3/src/veco.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    14287 2020-01-10 14:33:16.000000 imscript-0.3/src/vecoh.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7890 2020-01-10 14:33:18.000000 imscript-0.3/src/vecov.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      482 2018-01-11 09:37:54.000000 imscript-0.3/src/vector.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)     8319 2022-12-15 15:23:14.000000 imscript-0.3/src/viewflow.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)    37651 2017-10-23 14:34:44.000000 imscript-0.3/src/vvector.h
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5234 2018-03-10 17:30:58.000000 imscript-0.3/src/warp.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      780 2017-10-23 14:34:44.000000 imscript-0.3/src/xfopen.c
+-rw-rw-r--   0 coco      (1000) coco      (1000)      847 2022-07-13 12:24:19.000000 imscript-0.3/src/xmalloc.c
```

### Comparing `imscript-0.2/setup.py` & `imscript-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 		os.system("make bin/plambda bin/qauto")
 		install.run(self)
 
 
 import setuptools
 setuptools.setup(
 	name = "imscript",
-	version = "0.2",
+	version = "0.3",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@fastmail.com",
 	description = "Image Processing with Unix Pipes",
 	url = "https://github.com/mnhrdt/imscript",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

