# Comparing `tmp/scaffoldmaker-0.8.1.tar.gz` & `tmp/scaffoldmaker-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaffoldmaker-0.8.1.tar", last modified: Sat Mar 25 00:51:12 2023, max compression
+gzip compressed data, was "scaffoldmaker-0.9.0.tar", last modified: Mon Apr 17 23:31:40 2023, max compression
```

## Comparing `scaffoldmaker-0.8.1.tar` & `scaffoldmaker-0.9.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:51:12.609351 scaffoldmaker-0.8.1/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2022-03-31 21:19:35.000000 scaffoldmaker-0.8.1/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1723 2023-03-25 00:51:12.609046 scaffoldmaker-0.8.1/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      561 2022-03-31 21:19:35.000000 scaffoldmaker-0.8.1/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-03-25 00:51:12.609451 scaffoldmaker-0.8.1/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1531 2023-03-25 00:44:24.000000 scaffoldmaker-0.8.1/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:51:12.523710 scaffoldmaker-0.8.1/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:51:12.526586 scaffoldmaker-0.8.1/src/scaffoldmaker/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:51:12.537217 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 00:23:23.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    35794 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/annotationgroup.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2858 2022-08-08 11:58:38.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/bladder_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1050 2021-04-29 00:23:23.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/body_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2402 2021-10-20 02:05:49.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/brainstem_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1682 2021-11-23 01:12:53.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/colon_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1670 2022-03-31 21:19:35.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/esophagus_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5258 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/heart_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5237 2022-07-26 04:35:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/lung_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      702 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/muscle_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14883 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/nerve_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      830 2021-11-23 01:12:53.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/smallintestine_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      621 2021-04-29 00:23:23.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/stellate_terms.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6814 2022-03-31 21:19:35.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/stomach_terms.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:51:12.588307 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 00:23:23.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13990 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_1d_bifurcationtree1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    12899 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_1d_path1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4796 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_plate1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    15753 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_platehole1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    17764 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_sphere1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5036 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_tube1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    10211 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcation1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6136 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcationtree1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    49408 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_bladder1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    96545 2022-08-08 11:58:38.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_bladderurethra1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6908 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_box1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    18192 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_boxhole1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    38868 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_brainstem.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    53565 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_cecum1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    48641 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_colon1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   127183 2021-11-23 01:12:53.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_colonsegment1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    25534 2022-03-10 22:23:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_esophagus1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    26703 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heart1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4445 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heart2.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    31128 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialroot1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    19106 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialvalve1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   266527 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    86624 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria2.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    88510 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    59191 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles2.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    64701 2021-11-23 01:12:53.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles3.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    99065 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   102362 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase2.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    12420 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_lens1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   166018 2022-03-10 22:23:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_lung1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   120891 2022-07-26 04:35:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_lung2.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    12369 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_musclefusiform1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    48303 2022-08-08 11:58:38.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_ostium1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    90401 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_smallintestine1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    10973 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_solidcylinder1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    27370 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     8880 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere2.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    22159 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshell1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    62504 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshellseptum1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    41934 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_stellate1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   173982 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_stomach1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   415957 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_stomachhuman1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     8560 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_tube1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    15432 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_tubeseptum1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    65800 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_wholebody1.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    10051 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/scaffold_base.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    20785 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/scaffoldpackage.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7132 2022-07-26 04:35:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/scaffolds.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:51:12.608014 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 00:23:23.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    46030 2022-08-08 11:58:38.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/annulusmesh.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    16890 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/bifurcation.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    41057 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/cylindermesh.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    21780 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/derivativemoothing.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    15918 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/eft_utils.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    30899 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/eftfactory_bicubichermitelinear.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   106521 2022-07-26 04:35:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/eftfactory_tricubichermite.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     8633 2022-03-31 21:19:43.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/exportvtk.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    21596 2022-07-26 04:35:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/geometry.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    44059 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/interpolation.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1187 2021-04-29 00:23:23.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/matrix.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13991 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/meshrefinement.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2434 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/mirror.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5829 2021-11-04 03:08:25.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/octree.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002   163470 2023-02-09 03:26:46.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/shieldmesh.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    60466 2022-03-10 22:23:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/spheremesh.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    28890 2022-06-28 22:43:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/tracksurface.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    49575 2022-08-08 11:58:38.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/tubemesh.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2784 2021-11-23 01:12:53.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/vector.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    25252 2023-03-24 22:47:29.000000 scaffoldmaker-0.8.1/src/scaffoldmaker/utils/zinc_utils.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-03-25 00:51:12.528949 scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1723 2023-03-25 00:51:12.000000 scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4405 2023-03-25 00:51:12.000000 scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-03-25 00:51:12.000000 scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-04-29 00:23:48.000000 scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       72 2023-03-25 00:51:12.000000 scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       14 2023-03-25 00:51:12.000000 scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:31:40.889804 scaffoldmaker-0.9.0/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2022-03-31 21:19:35.000000 scaffoldmaker-0.9.0/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     2030 2023-04-17 23:31:40.889489 scaffoldmaker-0.9.0/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      545 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/README.rst
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-17 23:31:40.889912 scaffoldmaker-0.9.0/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1495 2023-04-17 23:31:16.000000 scaffoldmaker-0.9.0/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:31:40.845687 scaffoldmaker-0.9.0/src/
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:31:40.847707 scaffoldmaker-0.9.0/src/scaffoldmaker/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-11-04 03:08:25.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/__init__.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:31:40.858704 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 00:23:23.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    35770 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/annotationgroup.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     2858 2022-08-08 11:58:38.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/bladder_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1050 2021-04-29 00:23:23.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/body_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     2402 2021-10-20 02:05:49.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/brainstem_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1682 2021-11-23 01:12:53.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/colon_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1670 2022-03-31 21:19:35.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/esophagus_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5258 2022-06-28 22:43:48.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/heart_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5237 2022-07-26 04:35:25.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/lung_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      702 2022-06-28 22:43:48.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/muscle_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    14883 2023-02-09 03:26:46.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/nerve_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      830 2021-11-23 01:12:53.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/smallintestine_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      621 2021-04-29 00:23:23.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/stellate_terms.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6814 2022-03-31 21:19:35.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/stomach_terms.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:31:40.876601 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 00:23:23.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    13972 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_1d_bifurcationtree1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    12884 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_1d_path1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     4784 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_plate1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    15741 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_platehole1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    17752 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_sphere1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5024 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_tube1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    10199 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcation1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6127 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcationtree1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    49396 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_bladder1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    96533 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_bladderurethra1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6896 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_box1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    18180 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_boxhole1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    38850 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_brainstem.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    53559 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_cecum1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    48635 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_colon1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   127171 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_colonsegment1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    25522 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_esophagus1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    26688 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heart1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     4442 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heart2.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    31113 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialroot1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    19088 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialvalve1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   266506 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    86609 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria2.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    88498 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    59179 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles2.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    64686 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles3.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    99050 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   102347 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase2.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    12414 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_lens1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   166006 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_lung1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   120873 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_lung2.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    12363 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_musclefusiform1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    48294 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_ostium1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    90398 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_smallintestine1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    10967 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_solidcylinder1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    27358 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     8877 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere2.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    22147 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshell1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    62492 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshellseptum1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    41922 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_stellate1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   173964 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_stomach1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   415932 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_stomachhuman1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     8548 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_tube1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    15420 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_tubeseptum1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    65782 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_wholebody1.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    10045 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/scaffold_base.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    20770 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/scaffoldpackage.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     7132 2022-07-26 04:35:25.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/scaffolds.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:31:40.888864 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2021-04-29 00:23:23.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    46021 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/annulusmesh.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    16881 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/bifurcation.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    41048 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/cylindermesh.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    21765 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/derivativemoothing.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    15909 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/eft_utils.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    30893 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/eftfactory_bicubichermitelinear.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   106506 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/eftfactory_tricubichermite.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     8621 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/exportvtk.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    21593 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/geometry.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    44059 2021-11-04 03:08:25.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/interpolation.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1187 2021-04-29 00:23:23.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/matrix.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    13976 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/meshrefinement.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     2434 2021-11-04 03:08:25.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/mirror.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5829 2021-11-04 03:08:25.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/octree.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002   163461 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/shieldmesh.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    60460 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/spheremesh.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    28890 2022-06-28 22:43:48.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/tracksurface.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    49563 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/tubemesh.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     2784 2021-11-23 01:12:53.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/vector.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    25228 2023-04-17 23:31:06.000000 scaffoldmaker-0.9.0/src/scaffoldmaker/utils/zinc_utils.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-17 23:31:40.849988 scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     2030 2023-04-17 23:31:40.000000 scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     4405 2023-04-17 23:31:40.000000 scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-17 23:31:40.000000 scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2021-04-29 00:23:48.000000 scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/not-zip-safe
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       50 2023-04-17 23:31:40.000000 scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       14 2023-04-17 23:31:40.000000 scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/top_level.txt
```

### Comparing `scaffoldmaker-0.8.1/LICENSE` & `scaffoldmaker-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/PKG-INFO` & `scaffoldmaker-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 Metadata-Version: 2.1
 Name: scaffoldmaker
-Version: 0.8.1
-Summary: Python client for generating anatomical scaffolds using OpenCMISS-Zinc
+Version: 0.9.0
+Summary: Python client for generating anatomical scaffolds using Zinc
 Home-page: https://github.com/ABI-Software/scaffoldmaker
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
+Description: Scaffold Maker
+        ==============
+        
+        Anatomical scaffold generator using Zinc.
+        Install with::
+        
+          pip install scaffoldmaker
+        
+        For developing scaffolds::
+        
+          git clone git+https://github.com/ABI-Software/scaffoldmaker
+          cd scaffoldmaker
+          pip install -e .
+        
+        Requires the following Python libraries to be installed.
+        
+        * cmlibs.zinc
+        * cmlibs.utils
+        
+        We recommend installing scaffoldmaker into a virtual python environment.
+        See `python virtual environment documentation <https://docs.python.org/3/library/venv.html>`__ for information on virtual environments.
+        
+        
+        License
+        =======
+        
+        ::
+        
+        
+           Copyright 2022 University of Auckland
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Scaffold Maker
-==============
-
-Anatomical scaffold generator using OpenCMISS-Zinc.
-Install with::
-
-  pip install scaffoldmaker
-
-For developing scaffolds::
-
-  git clone git+https://github.com/ABI-Software/scaffoldmaker
-  cd scaffoldmaker
-  pip install -e .
-
-Requires the following Python libraries to be installed.
-
-* opencmiss.zinc
-* opencmiss.utils
-
-We recommend installing scaffoldmaker into a virtual python environment.
-See `python virtual environment documentation <https://docs.python.org/3/library/venv.html>`__ for information on virtual environments.
-
-
-License
-=======
-
-::
-
-
-   Copyright 2022 University of Auckland
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
-
```

### Comparing `scaffoldmaker-0.8.1/README.rst` & `scaffoldmaker-0.9.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Scaffold Maker
 ==============
 
-Anatomical scaffold generator using OpenCMISS-Zinc.
+Anatomical scaffold generator using Zinc.
 Install with::
 
   pip install scaffoldmaker
 
 For developing scaffolds::
 
   git clone git+https://github.com/ABI-Software/scaffoldmaker
   cd scaffoldmaker
   pip install -e .
 
 Requires the following Python libraries to be installed.
 
-* opencmiss.zinc
-* opencmiss.utils
+* cmlibs.zinc
+* cmlibs.utils
 
 We recommend installing scaffoldmaker into a virtual python environment.
 See `python virtual environment documentation <https://docs.python.org/3/library/venv.html>`__ for information on virtual environments.
```

### Comparing `scaffoldmaker-0.8.1/setup.py` & `scaffoldmaker-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 readme.append('')
 readme.append('')
 
 # For requirements not hosted on PyPi place listings
 # into the 'requirements.txt' file.
 requires = [
     # minimal requirements listing
-    "opencmiss.maths",
-    "opencmiss.utils >= 0.3",
-    "opencmiss.zinc >= 3.10.2",
+    "cmlibs.maths",
+    "cmlibs.utils",
+    "cmlibs.zinc",
     "scipy",
     "numpy",
 ]
 source_license = readfile("LICENSE")
 
 setup(
     name="scaffoldmaker",
-    version="0.8.1",
-    description="Python client for generating anatomical scaffolds using OpenCMISS-Zinc",
+    version="0.9.0",
+    description="Python client for generating anatomical scaffolds using Zinc",
     long_description="\n".join(readme) + source_license,
     long_description_content_type="text/x-rst",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Medical Science Apps."
     ],
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/annotationgroup.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/annotationgroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Describes subdomains of a scaffold with attached names and terms.
 """
 import sys
 
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.utils.zinc.field import find_or_create_field_coordinates, find_or_create_field_group, \
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.utils.zinc.field import find_or_create_field_coordinates, find_or_create_field_group, \
     find_or_create_field_stored_mesh_location, find_or_create_field_stored_string
-from opencmiss.zinc.element import Element, Mesh
-from opencmiss.zinc.field import Field, FieldFiniteElement, FieldGroup, FieldStoredMeshLocation, FieldStoredString, \
+from cmlibs.zinc.element import Element, Mesh
+from cmlibs.zinc.field import Field, FieldFiniteElement, FieldGroup, FieldStoredMeshLocation, FieldStoredString, \
     FieldFindMeshLocation
-from opencmiss.zinc.fieldcache import Fieldcache
-from opencmiss.zinc.fieldmodule import Fieldmodule
-from opencmiss.zinc.node import Node
-from opencmiss.zinc.result import RESULT_OK
+from cmlibs.zinc.fieldcache import Fieldcache
+from cmlibs.zinc.fieldmodule import Fieldmodule
+from cmlibs.zinc.node import Node
+from cmlibs.zinc.result import RESULT_OK
 from scaffoldmaker.utils.zinc_utils import get_highest_dimension_mesh, get_next_unused_node_identifier, \
     group_get_highest_dimension, identifier_ranges_from_string, identifier_ranges_to_string, \
     mesh_group_add_identifier_ranges, mesh_group_to_identifier_ranges, \
     nodeset_group_add_identifier_ranges, nodeset_group_to_identifier_ranges
 
 
 class AnnotationGroup(object):
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/bladder_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/bladder_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/body_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/body_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/brainstem_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/brainstem_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/colon_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/colon_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/esophagus_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/esophagus_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/heart_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/heart_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/lung_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/lung_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/muscle_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/muscle_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/nerve_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/nerve_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/smallintestine_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/smallintestine_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/stellate_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/stellate_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/annotation/stomach_terms.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/annotation/stomach_terms.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_1d_bifurcationtree1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_1d_bifurcationtree1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Generates a 1-D tree of bifurcating curves with radius.
 """
 
 from __future__ import division
 from math import cos, radians, sin
 
-from opencmiss.maths.vectorops import add, cross, magnitude, mult, normalize, sub
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldFiniteElement
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.maths.vectorops import add, cross, magnitude, mult, normalize, sub
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldFiniteElement
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 
 
 class MeshType_1d_bifurcationtree1(Scaffold_base):
     '''
     Generates a 1-D tree of bifurcating curves with radius.
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_1d_path1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_1d_path1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Generates a 1-D path mesh.
 """
 
 from __future__ import division
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.interpolation import smoothCubicHermiteCrossDerivativesLine
 
 
 class MeshType_1d_path1(Scaffold_base):
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_plate1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_plate1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Generates a 2-D unit plate mesh with variable numbers of elements in 2 directions.
 """
 
 from __future__ import division
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 
 
 class MeshType_2d_plate1(Scaffold_base):
     '''
     classdocs
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_platehole1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_platehole1.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 directions go around the hole.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis, Elementfieldtemplate
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis, Elementfieldtemplate
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.interpolation import interpolateCubicHermite, interpolateCubicHermiteDerivative
 
 
 class MeshType_2d_platehole1(Scaffold_base):
     '''
     classdocs
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_sphere1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_sphere1.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Generates a 2-D unit sphere mesh with variable numbers of elements around and up.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis, Elementfieldtemplate
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis, Elementfieldtemplate
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 
 
 class MeshType_2d_sphere1(Scaffold_base):
     '''
     classdocs
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_tube1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_tube1.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Generates a 2-D unit tube mesh with variable numbers of elements around, along.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 
 
 class MeshType_2d_tube1(Scaffold_base):
     '''
     classdocs
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcation1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcation1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Generates a 2-D tube bifurcation mesh.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.maths.vectorops import cross, mult, normalize, sub
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.maths.vectorops import cross, mult, normalize, sub
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.bifurcation import get_tube_bifurcation_connection_elements_counts, \
     make_tube_bifurcation_points, make_tube_bifurcation_elements_2d
 from scaffoldmaker.utils.geometry import createCirclePoints
 
 
 class MeshType_2d_tubebifurcation1(Scaffold_base):
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcationtree1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_2d_tubebifurcationtree1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Generates a 2-D tube bifurcation mesh.
 """
 
 from __future__ import division
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.meshtype_1d_bifurcationtree1 import MeshType_1d_bifurcationtree1
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils.bifurcation import get_curve_circle_points
 from scaffoldmaker.utils.interpolation import getCubicHermiteArcLength
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_bladder1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_bladder1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 
 from __future__ import division
 
 import copy
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.bladder_terms import get_bladder_term
 from scaffoldmaker.meshtypes.meshtype_3d_ostium1 import MeshType_3d_ostium1, generateOstiumMesh
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_bladderurethra1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_bladderurethra1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 with variable numbers of elements around, along and through
 wall.
 """
 
 import copy
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldGroup, findOrCreateFieldNodeGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldGroup, findOrCreateFieldNodeGroup, \
     findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, \
     getAnnotationGroupForTerm
 from scaffoldmaker.annotation.bladder_terms import get_bladder_term
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1, extractPathParametersFromRegion
 from scaffoldmaker.meshtypes.meshtype_3d_ostium1 import MeshType_3d_ostium1, generateOstiumMesh
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_box1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_box1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Generates a 3-D unit box mesh with variable numbers of elements in 3 directions.
 """
 
 from __future__ import division
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 
 
 class MeshType_3d_box1(Scaffold_base):
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_boxhole1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_boxhole1.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 directions go around the hole.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis, Elementfieldtemplate
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis, Elementfieldtemplate
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.interpolation import interpolateCubicHermite, interpolateCubicHermiteDerivative
 
 
 class MeshType_3d_boxhole1(Scaffold_base):
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_brainstem.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_brainstem.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 Brainstem mesh using a tapered cylinder
 """
 
 from __future__ import division
 
 import copy
 
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.node import Node
-from opencmiss.zinc.field import FieldFindMeshLocation
-from opencmiss.utils.zinc.field import Field, findOrCreateFieldCoordinates, findOrCreateFieldGroup, findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, \
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.node import Node
+from cmlibs.zinc.field import FieldFindMeshLocation
+from cmlibs.utils.zinc.field import Field, findOrCreateFieldCoordinates, findOrCreateFieldGroup, findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, \
     findOrCreateFieldStoredString
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.utils.zinc.finiteelement import getMaximumNodeIdentifier
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.utils.zinc.finiteelement import getMaximumNodeIdentifier
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm
 from scaffoldmaker.annotation.brainstem_terms import get_brainstem_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils.cylindermesh import CylinderMesh, CylinderShape, CylinderEnds, CylinderCentralPath
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_cecum1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_cecum1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 numbers of elements around, along and through wall, with
 variable radius and thickness along.
 """
 
 import copy
 import math
 
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.annotation.colon_terms import get_colon_term
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1, extractPathParametersFromRegion
 from scaffoldmaker.meshtypes.meshtype_3d_colonsegment1 import ColonSegmentTubeMeshInnerPoints, \
     getFullProfileFromHalfHaustrum, getTeniaColi, createNodesAndElementsTeniaColi
 from scaffoldmaker.meshtypes.meshtype_3d_ostium1 import MeshType_3d_ostium1, generateOstiumMesh
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_colon1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_colon1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Generates a 3-D colon mesh along the central line, with variable
 numbers of elements around, along and through wall, with
 variable radius and thickness along.
 """
 
 import copy
 
-from opencmiss.zinc.node import Node
-from opencmiss.zinc.element import Element
+from cmlibs.zinc.node import Node
+from cmlibs.zinc.element import Element
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.colon_terms import get_colon_term
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1, extractPathParametersFromRegion
 from scaffoldmaker.meshtypes.meshtype_3d_colonsegment1 import MeshType_3d_colonsegment1, ColonSegmentTubeMeshInnerPoints, \
     getTeniaColi, createFlatCoordinatesTeniaColi, createColonCoordinatesTeniaColi, createNodesAndElementsTeniaColi
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_colonsegment1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_colonsegment1.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 through wall and number of tenia coli, with variable radius
 and thickness along.
 """
 
 import copy
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, mergeAnnotationGroups, \
     findOrCreateAnnotationGroupForTerm, findAnnotationGroupByName, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.colon_terms import get_colon_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import matrix
 from scaffoldmaker.utils import tubemesh
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_esophagus1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_esophagus1.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Generates a 3-D esophagus mesh along the central line,
 with variable numbers of elements around, along and through
 wall, with variable radius and thickness along.
 """
 
 import copy
 import math
-from opencmiss.utils.zinc.field import findOrCreateFieldGroup, findOrCreateFieldStoredString, \
+from cmlibs.utils.zinc.field import findOrCreateFieldGroup, findOrCreateFieldStoredString, \
     findOrCreateFieldStoredMeshLocation, findOrCreateFieldNodeGroup
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, getAnnotationGroupForTerm, \
     findOrCreateAnnotationGroupForTerm
 from scaffoldmaker.annotation.esophagus_terms import get_esophagus_term
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1, extractPathParametersFromRegion
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils import geometry
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heart1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heart1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Generates a 3-D heart model including ventricles, base and atria.
 """
 
 from __future__ import division
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm, mergeAnnotationGroups
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.meshtype_3d_heartatria1 import MeshType_3d_heartatria1
 from scaffoldmaker.meshtypes.meshtype_3d_heartventriclesbase1 import MeshType_3d_heartventriclesbase1
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_bicubichermitelinear import eftfactory_bicubichermitelinear
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heart2.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heart2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Generates a 3-D heart model including ventricles, base and atria.
 """
 
 from __future__ import division
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
 from scaffoldmaker.annotation.annotationgroup import mergeAnnotationGroups
 from scaffoldmaker.meshtypes.meshtype_3d_heartatria2 import MeshType_3d_heartatria2
 from scaffoldmaker.meshtypes.meshtype_3d_heartventriclesbase2 import MeshType_3d_heartventriclesbase2
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialroot1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialroot1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 for attaching to a 6-element-around bicubic-linear orifice.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_bicubichermitelinear import eftfactory_bicubichermitelinear
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialvalve1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartarterialvalve1.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Bicubic with linear through wall.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.maths.vectorops import eulerToRotationMatrix3
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.maths.vectorops import eulerToRotationMatrix3
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.geometry import createCirclePoints
 from scaffoldmaker.utils.interpolation import interpolateLagrangeHermiteDerivative, smoothCubicHermiteDerivativesLine
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria1.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 """
 
 from __future__ import division
 
 import copy
 import math
 
-from opencmiss.maths.vectorops import add, cross, dot, magnitude, mult, normalize, sub
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.maths.vectorops import add, cross, dot, magnitude, mult, normalize, sub
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field, FieldGroup
-from opencmiss.zinc.node import Node
-from opencmiss.zinc.result import RESULT_OK
+from cmlibs.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field, FieldGroup
+from cmlibs.zinc.node import Node
+from cmlibs.zinc.result import RESULT_OK
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findAnnotationGroupByName, \
     findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.meshtype_3d_ostium1 import MeshType_3d_ostium1, generateOstiumMesh
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils import interpolation as interp
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria2.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartatria2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 3-D Heart Ventricles with Base 2.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 Variant using collapsed/wedge elements at septum junction.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles2.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles2.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Generates 3-D Left and Right ventricles mesh starting from modified sphere shell mesh.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftNodeValueLabel, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles3.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventricles3.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 Variant using collapsed/wedge elements at septum junction.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.geometry import createEllipsoidPoints, getApproximateEllipsePerimeter, getEllipseArcLength, getEllipseRadiansToX
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase1.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 """
 
 from __future__ import division
 
 import copy
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field, FieldGroup
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field, FieldGroup
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.meshtype_3d_heartatria1 import MeshType_3d_heartatria1, getAtriumBasePoints
 from scaffoldmaker.meshtypes.meshtype_3d_heartventricles1 import MeshType_3d_heartventricles1
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase2.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_heartventriclesbase2.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 pulmonary trunk and their valve regions.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.finiteelement import getMaximumElementIdentifier, getMaximumNodeIdentifier
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.heart_terms import get_heart_term
 from scaffoldmaker.meshtypes.meshtype_3d_heartventricles2 import MeshType_3d_heartventricles2
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_lens1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_lens1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 around, up the central axis, and radially.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.field import Field
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.field import Field
 from scaffoldmaker.meshtypes.meshtype_3d_solidsphere1 import MeshType_3d_solidsphere1
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 
 
 class MeshType_3d_lens1(Scaffold_base):
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_lung1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_lung1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 Generates 3D lung surface mesh.
 '''
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.lung_terms import get_lung_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_lung2.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_lung2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,29 @@
     smoothCubicHermiteDerivativesLine, interpolateSampleLinear
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.lung_terms import get_lung_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, remapEftNodeValueLabelsVersion, setEftScaleFactorIds
 from scaffoldmaker.utils.cylindermesh import createEllipsePerimeter
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
-from opencmiss.utils.zinc.general import ChangeManager
+from cmlibs.utils.zinc.general import ChangeManager
 from scaffoldmaker.utils.geometry import createEllipsoidPoints, getEllipseRadiansToX, getEllipseArcLength, \
     getApproximateEllipsePerimeter, sampleEllipsePoints, updateEllipseAngleByArcLength, getEllipsoidPlaneA, \
     getEllipsoidPolarCoordinatesFromPosition, getEllipsoidPolarCoordinatesTangents
 from scaffoldmaker.utils.interpolation import computeCubicHermiteDerivativeScaling, interpolateCubicHermite, \
     interpolateCubicHermiteDerivative
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 from scaffoldmaker.utils.vector import magnitude, setMagnitude, crossproduct3, normalise
-from opencmiss.maths.vectorops import add, cross, dot, mult, normalize, sub
+from cmlibs.maths.vectorops import add, cross, dot, mult, normalize, sub
 from scaffoldmaker.utils.zinc_utils import disconnectFieldMeshGroupBoundaryNodes
-from opencmiss.utils.zinc.field import Field, findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.utils.zinc.field import Field, findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString, createFieldEulerAnglesRotationMatrix
-from opencmiss.utils.zinc.finiteelement import get_element_node_identifiers
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.finiteelement import get_element_node_identifiers
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.node import Node
 
 class MeshType_3d_lung2(Scaffold_base):
     '''
     Generic 3D lung scaffold.
     '''
 
     """
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_musclefusiform1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_musclefusiform1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
  with variable numbers of elements in major, minor, shell and axial directions.
 """
 
 from __future__ import division
 
 import copy
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils.cylindermesh import CylinderMesh, CylinderShape, CylinderEnds, CylinderCentralPath
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 from scaffoldmaker.utils.zinc_utils import exnodeStringFromNodeValues
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_ostium1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_ostium1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 from __future__ import division
 
 import copy
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.annulusmesh import createAnnulusMesh3d
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.geometry import createCirclePoints, getCircleProjectionAxes
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_smallintestine1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_smallintestine1.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Generates a 3-D small intestine mesh along the central line,
 with variable numbers of elements around, along and through
 wall, with variable radius and thickness along.
 """
 
 import copy
 
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.annotation.smallintestine_terms import get_smallintestine_term
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1, extractPathParametersFromRegion
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import tubemesh
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_solidcylinder1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_solidcylinder1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
  with variable numbers of elements in major, minor, shell and axial directions.
 """
 
 from __future__ import division
 
 import copy
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
 from scaffoldmaker.utils.cylindermesh import CylinderMesh, CylinderShape, CylinderEnds, CylinderCentralPath
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 from scaffoldmaker.utils.zinc_utils import exnodeStringFromNodeValues
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere1.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 around, up the central axis, and radially.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere2.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_solidsphere2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generates a solid sphere (spheroid/ellipsoid in general) using a ShieldMesh of all cube elements,
  with variable numbers of elements across axes and shell directions.
 """
 
 from __future__ import division
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 from scaffoldmaker.utils.spheremesh import SphereMesh, SphereShape
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshell1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshell1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 around, up and through the thickness.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eftfactory_bicubichermitelinear import eftfactory_bicubichermitelinear
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 
 
 class MeshType_3d_sphereshell1(Scaffold_base):
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshellseptum1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_sphereshellseptum1.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 Only one element throught the wall is currently implemented.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element, Elementbasis, Elementfieldtemplate
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element, Elementbasis, Elementfieldtemplate
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.interpolation import interpolateCubicHermite, interpolateCubicHermiteDerivative
 
 
 class MeshType_3d_sphereshellseptum1(Scaffold_base):
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_stellate1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_stellate1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Generates a 3-D planar stellate mesh with cross arms radiating from a central node, and variable numbers of elements along each arm.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, findOrCreateFieldNodeGroup, findOrCreateFieldStoredMeshLocation, \
     findOrCreateFieldStoredString
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm, getAnnotationGroupForTerm
 from scaffoldmaker.annotation.stellate_terms import get_stellate_term
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eft_utils import remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds, remapEftLocalNodes
 from scaffoldmaker.utils.eftfactory_bicubichermitelinear import eftfactory_bicubichermitelinear
 from scaffoldmaker.utils.interpolation import smoothCubicHermiteDerivativesLine
 from scaffoldmaker.utils.matrix import rotateAboutZAxis
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_stomach1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_stomach1.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 """
 
 from __future__ import division
 
 import copy
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.utils.zinc.finiteelement import get_element_node_identifiers, getMaximumNodeIdentifier
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.finiteelement import get_element_node_identifiers, getMaximumNodeIdentifier
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, mergeAnnotationGroups, \
     getAnnotationGroupForTerm, findOrCreateAnnotationGroupForTerm
 from scaffoldmaker.annotation.stomach_terms import get_stomach_term
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1, extractPathParametersFromRegion
 from scaffoldmaker.meshtypes.meshtype_3d_ostium1 import MeshType_3d_ostium1, generateOstiumMesh
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.scaffoldpackage import ScaffoldPackage
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_stomachhuman1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_stomachhuman1.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 A source mesh based scaffold generator for human stomach geometry
 Provenance information at http://models.cellml.org/workspace/516
 """
 
 from __future__ import division
 
 import numpy as np
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldFibres
-from opencmiss.zinc.context import Context
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldFibres
+from cmlibs.zinc.context import Context
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scipy.interpolate import splprep, splev
 
 
 class Stomach:
     '''
@@ -9502,15 +9502,15 @@
                 _,v = hfl.evaluateReal(fieldCache,fieldNames[fn])                
                 fv[fn] = v  
             nodes[nd] = fv
         return nodes    
     
     def generateMesh(self,region,circumferentialElements,axialElements,wallElements,normalizeCircumferentialSegmentLengths,refineAtLength={},refineAtTheta={}):
         '''
-        region - opencmiss zinc region where mesh needs to be created
+        region - zinc region where mesh needs to be created
         circumferentialElements - number of elements along the circumference
         axialElements - number of elements along the axis
         wallElements - number of elements along the wall
         normalizeCircumferentialSegmentLengths - If True, the circumferential segment lengths along a lattitute will be nearly equal
         refineAtLength - dict of axial length that need to be refined at an xi 
                         {1:0.25}, a new row of elements will be create by splitting the first row of elements at xi=0.25
         refineAtTheta - list of circumferential elements that need to be refined
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_tube1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_tube1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 through wall, plus variable wall thickness for unit diameter.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 
 
 class MeshType_3d_tube1(Scaffold_base):
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_tubeseptum1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_tubeseptum1.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 The number of elements along the tube and across the septum can be varied.
 """
 
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 
 
 class MeshType_3d_tubeseptum1(Scaffold_base):
     '''
     classdocs
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/meshtype_3d_wholebody1.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/meshtype_3d_wholebody1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
  with variable numbers of elements in major, minor, shell and for each section of abdomen, thorax, neck and head.
 """
 
 from __future__ import division
 
 import copy
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, \
     findOrCreateFieldStoredString, findOrCreateFieldStoredMeshLocation, findOrCreateFieldNodeGroup
-from opencmiss.utils.zinc.finiteelement import getMaximumNodeIdentifier, get_element_node_identifiers
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.finiteelement import getMaximumNodeIdentifier, get_element_node_identifiers
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation import heart_terms, bladder_terms, lung_terms, stomach_terms, brainstem_terms
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findOrCreateAnnotationGroupForTerm
 from scaffoldmaker.annotation.annotationgroup import getAnnotationGroupForTerm
 from scaffoldmaker.annotation.body_terms import get_body_term
 from scaffoldmaker.annotation.nerve_terms import get_nerve_term
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import MeshType_1d_path1
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/meshtypes/scaffold_base.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/meshtypes/scaffold_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Scaffold abstract base class.
 Describes methods each scaffold must or may override.
 """
 import copy
 
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.field import Field
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.field import Field
 from scaffoldmaker.utils.derivativemoothing import DerivativeSmoothing
 from scaffoldmaker.utils.interpolation import DerivativeScalingMode
 from scaffoldmaker.utils.meshrefinement import MeshRefinement
 from scaffoldmaker.utils.zinc_utils import extract_node_field_parameters, print_node_field_parameters
 
 
 class Scaffold_base:
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/scaffoldpackage.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/scaffoldpackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Class packaging a scaffold type, options and modifications.
 Supports serialisation to/from JSON. Can be used as a scaffold option.
 """
 
 import copy
 import math
 
-from opencmiss.maths.vectorops import euler_to_rotation_matrix
-from opencmiss.utils.zinc.field import createFieldEulerAnglesRotationMatrix
-from opencmiss.utils.zinc.finiteelement import get_maximum_node_identifier
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.field import Field, FieldGroup
+from cmlibs.maths.vectorops import euler_to_rotation_matrix
+from cmlibs.utils.zinc.field import createFieldEulerAnglesRotationMatrix
+from cmlibs.utils.zinc.finiteelement import get_maximum_node_identifier
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.field import Field, FieldGroup
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup, findAnnotationGroupByName, \
     getAnnotationMarkerLocationField  # , getAnnotationMarkerNameField
 from scaffoldmaker.meshtypes.scaffold_base import Scaffold_base
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.zinc_utils import get_highest_dimension_mesh
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/scaffolds.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/scaffolds.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/annulusmesh.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/annulusmesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Utility functions for generating annulus mesh between start and end loops of points.
 """
 from __future__ import division
 
 import copy
 from collections.abc import Sequence
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.node import Node
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftNodeValueLabel, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_bicubichermitelinear import eftfactory_bicubichermitelinear
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/bifurcation.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/bifurcation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Utilities for building bifurcating network meshes.
 """
 
 from __future__ import division
 
-from opencmiss.maths.vectorops import add, cross, dot, magnitude, mult, normalize, sub
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.node import Node
+from cmlibs.maths.vectorops import add, cross, dot, magnitude, mult, normalize, sub
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.node import Node
 from scaffoldmaker.utils.eft_utils import remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds
 from scaffoldmaker.utils.geometry import createCirclePoints
 from scaffoldmaker.utils.interpolation import DerivativeScalingMode, interpolateCubicHermite, interpolateCubicHermiteDerivative, \
     interpolateCubicHermiteSecondDerivative, smoothCubicHermiteDerivativesLine, interpolateLagrangeHermiteDerivative
 
 
 def get_curve_circle_points(x1, xd1, x2, xd2, r1, rd1, r2, rd2, xi, dmag, side, elementsCountAround):
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/cylindermesh.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/cylindermesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
  orientation can be controlled using a central path subscaffold. It can be used to generate
 a solid truncated cone. It also can be used for transition from a 2D base to another base (e.g., ellipse to a circle).
 """
 
 import math
 from enum import Enum
 
-from opencmiss.utils.zinc.finiteelement import getMaximumNodeIdentifier, getMaximumElementIdentifier
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.finiteelement import getMaximumNodeIdentifier, getMaximumElementIdentifier
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.meshtypes.meshtype_1d_path1 import extractPathParametersFromRegion
 from scaffoldmaker.utils import vector, geometry
 from scaffoldmaker.utils.interpolation import sampleCubicHermiteCurves, interpolateSampleCubicHermite, \
     smoothCubicHermiteDerivativesLine
 from scaffoldmaker.utils.mirror import Mirror
 from scaffoldmaker.utils.shieldmesh import ShieldMesh2D, ShieldShape2D, ShieldRimDerivativeMode
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/derivativemoothing.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/derivativemoothing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 '''
 Class for globally smoothing field derivatives.
 '''
 from __future__ import division
 
 import math
 
-from opencmiss.maths.vectorops import magnitude
-from opencmiss.utils.zinc.field import findOrCreateFieldGroup
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
+from cmlibs.maths.vectorops import magnitude
+from cmlibs.utils.zinc.field import findOrCreateFieldGroup
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
 from scaffoldmaker.utils.interpolation import DerivativeScalingMode, getCubicHermiteArcLength, interpolateHermiteLagrangeDerivative, interpolateLagrangeHermiteDerivative
 from scaffoldmaker.utils.vector import setMagnitude
 
 
 class EdgeCurve:
     '''
     A description of a 1D Hermite curve mapped from an element edge
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/eft_utils.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/eft_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Utility functions for element field templates shared by mesh generators.
 '''
-from opencmiss.utils.zinc.finiteelement import getElementNodeIdentifiers
-from opencmiss.zinc.element import Elementfieldtemplate
-from opencmiss.zinc.result import RESULT_OK
+from cmlibs.utils.zinc.finiteelement import getElementNodeIdentifiers
+from cmlibs.zinc.element import Elementfieldtemplate
+from cmlibs.zinc.result import RESULT_OK
 
 
 def getEftTermScaling(eft, functionIndex, termIndex):
     '''
     Convenience function to get the scale factor indexes scaling a term as a list.
     :eft:  Element field template to query.
     :functionIndex:  Function index from 1 to number of basis functions.
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/eftfactory_bicubichermitelinear.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/eftfactory_bicubichermitelinear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Definitions of standard element field templates using bicubic Hermite x linear Lagrange basis.
 '''
-from opencmiss.zinc.element import Elementbasis
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.element import Elementbasis
+from cmlibs.zinc.node import Node
 from scaffoldmaker.utils.eft_utils import remapEftLocalNodes, remapEftNodeValueLabel, setEftScaleFactorIds
 
 
 class eftfactory_bicubichermitelinear:
     '''
     Factory class for creating element field templates for a 3-D mesh using bicubic Hermite x linear Lagrange basis.
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/eftfactory_tricubichermite.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/eftfactory_tricubichermite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''
 Definitions of standard element field templates shared by mesh generators.
 '''
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.utils.zinc.finiteelement import getElementNodeIdentifiers
-from opencmiss.zinc.element import Element, Elementbasis, Elementfieldtemplate
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.finiteelement import getElementNodeIdentifiers
+from cmlibs.zinc.element import Element, Elementbasis, Elementfieldtemplate
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import mapEftFunction1Node1Term, remapEftLocalNodes, remapEftNodeValueLabel, scaleEftNodeValueLabels, setEftScaleFactorIds
 
 
 class eftfactory_tricubichermite:
     '''
     Factory class for creating element field templates for a 3-D mesh using tricubic Hermite basis.
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/exportvtk.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/exportvtk.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 '''
 
 import io
 import os
 import sys
 from sys import version_info
 
-from opencmiss.utils.zinc.finiteelement import getElementNodeIdentifiersBasisOrder
-from opencmiss.utils.zinc.general import ChangeManager
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.result import RESULT_OK
+from cmlibs.utils.zinc.finiteelement import getElementNodeIdentifiersBasisOrder
+from cmlibs.utils.zinc.general import ChangeManager
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.result import RESULT_OK
 
 
 class ExportVtk:
     '''
     Class for exporting a Scaffold from Zinc to legacy vtk text format.
     Limited to writing only 3-D hexahedral elements. Assumes all nodes have field defined.
     '''
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/geometry.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 
 from __future__ import division
 
 import copy
 import math
 
-from opencmiss.maths.vectorops import magnitude, mult
+from cmlibs.maths.vectorops import magnitude, mult
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.tracksurface import calculate_surface_delta_xi
 
 
 def getApproximateEllipsePerimeter(a, b):
     '''
     Get perimeter of ellipse using Ramanujan II approximation.
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/interpolation.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/matrix.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/meshrefinement.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/meshrefinement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 '''
 Class for refining a mesh from one region to another.
 '''
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, findOrCreateFieldNodeGroup, \
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldGroup, findOrCreateFieldNodeGroup, \
     findOrCreateFieldStoredMeshLocation, findOrCreateFieldStoredString
-from opencmiss.zinc.element import Element, Elementbasis
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
-from opencmiss.zinc.result import RESULT_OK as ZINC_OK
+from cmlibs.zinc.element import Element, Elementbasis
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
+from cmlibs.zinc.result import RESULT_OK as ZINC_OK
 from scaffoldmaker.annotation.annotationgroup import AnnotationGroup
 from scaffoldmaker.utils.octree import Octree
 
 
 class MeshRefinement:
     '''
     Class for refining a mesh from one region to another.
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/mirror.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/mirror.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/octree.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/octree.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/shieldmesh.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/shieldmesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 merge to form a triangle.
 """
 
 from __future__ import division
 import copy
 from enum import Enum
 
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eft_utils import remapEftNodeValueLabel, setEftScaleFactorIds
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.interpolation import DerivativeScalingMode, sampleCubicHermiteCurves, \
     smoothCubicHermiteDerivativesLine
 from scaffoldmaker.utils.mirror import Mirror
 from scaffoldmaker.utils.tracksurface import TrackSurface, calculate_surface_axes
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/spheremesh.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/spheremesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Utility functions for generating a solid sphere/spheroid (ellipsoid in general).
 """
 
 from enum import Enum
 
 import math
 
-from opencmiss.utils.zinc.finiteelement import getMaximumNodeIdentifier, getMaximumElementIdentifier
-from opencmiss.zinc.field import Field
+from cmlibs.utils.zinc.finiteelement import getMaximumNodeIdentifier, getMaximumElementIdentifier
+from cmlibs.zinc.field import Field
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.interpolation import sampleCubicHermiteCurves, smoothCubicHermiteDerivativesLine
 from scaffoldmaker.utils.cylindermesh import Ellipse2D, EllipseShape
 from scaffoldmaker.utils.shieldmesh import ShieldMesh3D
 
 
 class SphereShape(Enum):
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/tracksurface.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/tracksurface.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/tubemesh.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/tubemesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Utility function for generating tubular mesh from a central line
 using a segment profile.
 '''
 from __future__ import division
 
 import math
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldTextureCoordinates
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.field import Field
-from opencmiss.zinc.node import Node
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates, findOrCreateFieldTextureCoordinates
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.field import Field
+from cmlibs.zinc.node import Node
 from scaffoldmaker.annotation.annotationgroup import mergeAnnotationGroups
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import matrix
 from scaffoldmaker.utils import vector
 from scaffoldmaker.utils.eftfactory_bicubichermitelinear import eftfactory_bicubichermitelinear
 from scaffoldmaker.utils.eftfactory_tricubichermite import eftfactory_tricubichermite
 from scaffoldmaker.utils.eft_utils import remapEftNodeValueLabelsVersion
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/vector.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/vector.py`

 * *Files identical despite different names*

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker/utils/zinc_utils.py` & `scaffoldmaker-0.9.0/src/scaffoldmaker/utils/zinc_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 '''
 Utility functions for easing use of Zinc API.
 '''
 
-from opencmiss.utils.zinc.field import findOrCreateFieldCoordinates
-from opencmiss.utils.zinc.general import ChangeManager, HierarchicalChangeManager
-from opencmiss.zinc.context import Context
-from opencmiss.zinc.element import Mesh, MeshGroup
-from opencmiss.zinc.field import Field, FieldGroup
-from opencmiss.zinc.fieldmodule import Fieldmodule
-from opencmiss.zinc.node import Node, Nodeset
-from opencmiss.zinc.result import RESULT_OK
+from cmlibs.utils.zinc.field import findOrCreateFieldCoordinates
+from cmlibs.utils.zinc.general import ChangeManager, HierarchicalChangeManager
+from cmlibs.zinc.context import Context
+from cmlibs.zinc.element import Mesh, MeshGroup
+from cmlibs.zinc.field import Field, FieldGroup
+from cmlibs.zinc.fieldmodule import Fieldmodule
+from cmlibs.zinc.node import Node, Nodeset
+from cmlibs.zinc.result import RESULT_OK
 from scaffoldmaker.utils import interpolation as interp
 from scaffoldmaker.utils import vector
 
 
 def interpolateNodesCubicHermite(cache, coordinates, xi, normal_scale, \
         node1, derivative1, scale1, cross_derivative1, cross_scale1, \
         node2, derivative2, scale2, cross_derivative2, cross_scale2):
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/PKG-INFO` & `scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 Metadata-Version: 2.1
 Name: scaffoldmaker
-Version: 0.8.1
-Summary: Python client for generating anatomical scaffolds using OpenCMISS-Zinc
+Version: 0.9.0
+Summary: Python client for generating anatomical scaffolds using Zinc
 Home-page: https://github.com/ABI-Software/scaffoldmaker
 Author: Auckland Bioengineering Institute
 Author-email: r.christie@auckland.ac.nz
 License: Apache Software License
+Description: Scaffold Maker
+        ==============
+        
+        Anatomical scaffold generator using Zinc.
+        Install with::
+        
+          pip install scaffoldmaker
+        
+        For developing scaffolds::
+        
+          git clone git+https://github.com/ABI-Software/scaffoldmaker
+          cd scaffoldmaker
+          pip install -e .
+        
+        Requires the following Python libraries to be installed.
+        
+        * cmlibs.zinc
+        * cmlibs.utils
+        
+        We recommend installing scaffoldmaker into a virtual python environment.
+        See `python virtual environment documentation <https://docs.python.org/3/library/venv.html>`__ for information on virtual environments.
+        
+        
+        License
+        =======
+        
+        ::
+        
+        
+           Copyright 2022 University of Auckland
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Scaffold Maker
-==============
-
-Anatomical scaffold generator using OpenCMISS-Zinc.
-Install with::
-
-  pip install scaffoldmaker
-
-For developing scaffolds::
-
-  git clone git+https://github.com/ABI-Software/scaffoldmaker
-  cd scaffoldmaker
-  pip install -e .
-
-Requires the following Python libraries to be installed.
-
-* opencmiss.zinc
-* opencmiss.utils
-
-We recommend installing scaffoldmaker into a virtual python environment.
-See `python virtual environment documentation <https://docs.python.org/3/library/venv.html>`__ for information on virtual environments.
-
-
-License
-=======
-
-::
-
-
-   Copyright 2022 University of Auckland
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
-
```

### Comparing `scaffoldmaker-0.8.1/src/scaffoldmaker.egg-info/SOURCES.txt` & `scaffoldmaker-0.9.0/src/scaffoldmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

