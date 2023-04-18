# Comparing `tmp/potentials-0.3.5.tar.gz` & `tmp/potentials-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\potentials\dist\tmpj_bmccrk\potentials-0.3.5.tar", last modified: Mon Oct  3 14:41:21 2022, max compression
+gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\potentials\dist\.tmp-6b0tjit8\potentials-0.3.6.tar", last modified: Tue Apr 18 20:20:19 2023, max compression
```

## Comparing `potentials-0.3.5.tar` & `potentials-0.3.6.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/
--rw-rw-rw-   0        0        0     2776 2020-07-21 17:56:46.000000 potentials-0.3.5/LICENSE.TXT
--rw-rw-rw-   0        0        0      160 2022-06-01 17:13:54.000000 potentials-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4243 2022-10-03 14:41:21.000000 potentials-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3463 2021-09-14 15:58:47.000000 potentials-0.3.5/README.rst
--rw-rw-rw-   0        0        0     2908 2022-10-03 14:37:52.000000 potentials-0.3.5/UPDATES.rst
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:20.000000 potentials-0.3.5/potentials/
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/Database/
--rw-rw-rw-   0        0        0    14382 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/__init__.py
--rw-rw-rw-   0        0        0    15046 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_action.py
--rw-rw-rw-   0        0        0    18665 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_citation.py
--rw-rw-rw-   0        0        0    11655 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_faq.py
--rw-rw-rw-   0        0        0    14789 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_kim_potential.py
--rw-rw-rw-   0        0        0    42725 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_lammps_potential.py
--rw-rw-rw-   0        0        0    18434 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_potential.py
--rw-rw-rw-   0        0        0    24254 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_record.py
--rw-rw-rw-   0        0        0    10620 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_related_models.py
--rw-rw-rw-   0        0        0    12559 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_request.py
--rw-rw-rw-   0        0        0    11597 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/_widgets.py
--rw-rw-rw-   0        0        0     1228 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Database/load_database.py
--rw-rw-rw-   0        0        0     9996 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/Settings.py
--rw-rw-rw-   0        0        0        5 2022-10-03 14:37:55.000000 potentials-0.3.5/potentials/VERSION
--rw-rw-rw-   0        0        0      727 2022-03-31 22:10:53.000000 potentials-0.3.5/potentials/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/buildrecord/
--rw-rw-rw-   0        0        0      107 2022-03-31 22:10:53.000000 potentials-0.3.5/potentials/buildrecord/__init__.py
--rw-rw-rw-   0        0        0     1359 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/build_lammps_potential.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/
--rw-rw-rw-   0        0        0     6135 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/EamBuilder.py
--rw-rw-rw-   0        0        0     5551 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/EimBuilder.py
--rw-rw-rw-   0        0        0     5916 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/KimBuilder.py
--rw-rw-rw-   0        0        0     6212 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py
--rw-rw-rw-   0        0        0    13157 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/PairBuilder.py
--rw-rw-rw-   0        0        0     6210 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py
--rw-rw-rw-   0        0        0    19230 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py
--rw-rw-rw-   0        0        0      315 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/paramfile/
--rw-rw-rw-   0        0        0    51311 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/paramfile/EAM.py
--rw-rw-rw-   0        0        0    55972 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/paramfile/EAMAlloy.py
--rw-rw-rw-   0        0        0    57842 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/paramfile/EAMFS.py
--rw-rw-rw-   0        0        0      192 2022-03-31 22:10:53.000000 potentials-0.3.5/potentials/paramfile/__init__.py
--rw-rw-rw-   0        0        0     6747 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/paramfile/converters.py
--rw-rw-rw-   0        0        0     2188 2022-09-19 13:36:46.000000 potentials-0.3.5/potentials/paramfile/load_eam.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/record/
--rw-rw-rw-   0        0        0    18817 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/Action.py
--rw-rw-rw-   0        0        0     7400 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/Artifact.py
--rw-rw-rw-   0        0        0    24747 2022-07-22 20:58:10.000000 potentials-0.3.5/potentials/record/BasePotentialLAMMPS.py
--rw-rw-rw-   0        0        0    16320 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/Citation.py
--rw-rw-rw-   0        0        0     7859 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/FAQ.py
--rw-rw-rw-   0        0        0    12748 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/Implementation.py
--rw-rw-rw-   0        0        0     5258 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/Link.py
--rw-rw-rw-   0        0        0     5363 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/Parameter.py
--rw-rw-rw-   0        0        0    23649 2022-07-22 18:07:18.000000 potentials-0.3.5/potentials/record/Potential.py
--rw-rw-rw-   0        0        0    27640 2022-07-25 16:44:57.000000 potentials-0.3.5/potentials/record/PotentialLAMMPS.py
--rw-rw-rw-   0        0        0    37140 2022-07-25 16:44:59.000000 potentials-0.3.5/potentials/record/PotentialLAMMPSKIM.py
--rw-rw-rw-   0        0        0    14879 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/record/Request.py
--rw-rw-rw-   0        0        0      655 2022-03-31 22:10:53.000000 potentials-0.3.5/potentials/record/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/tools/
--rw-rw-rw-   0        0        0      446 2022-03-31 22:10:53.000000 potentials-0.3.5/potentials/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/tools/__pycache__/
--rw-rw-rw-   0        0        0      543 2022-03-31 22:26:25.000000 potentials-0.3.5/potentials/tools/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1173 2019-07-31 19:39:47.000000 potentials-0.3.5/potentials/tools/__pycache__/aslist.cpython-37.pyc
--rw-rw-rw-   0        0        0     7975 2022-05-25 17:25:42.000000 potentials-0.3.5/potentials/tools/__pycache__/atomic_info.cpython-37.pyc
--rw-rw-rw-   0        0        0   152808 2021-08-03 17:29:36.000000 potentials-0.3.5/potentials/tools/__pycache__/atomicdata.cpython-37.pyc
--rw-rw-rw-   0        0        0     1399 2022-05-25 17:25:42.000000 potentials-0.3.5/potentials/tools/__pycache__/numderivative.cpython-37.pyc
--rw-rw-rw-   0        0        0     1546 2022-05-25 17:25:42.000000 potentials-0.3.5/potentials/tools/__pycache__/parse_authors.cpython-37.pyc
--rw-rw-rw-   0        0        0      601 2020-07-23 20:51:50.000000 potentials-0.3.5/potentials/tools/__pycache__/screen_input.cpython-37.pyc
--rw-rw-rw-   0        0        0     1610 2019-12-28 16:49:05.000000 potentials-0.3.5/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc
--rw-rw-rw-   0        0        0    11550 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/tools/atomic_info.py
--rw-rw-rw-   0        0        0   132864 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/tools/atomicdata.csv
--rw-rw-rw-   0        0        0     1448 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/tools/numderivative.py
--rw-rw-rw-   0        0        0     2200 2022-05-23 16:10:08.000000 potentials-0.3.5/potentials/tools/parse_authors.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/xsd/
--rw-rw-rw-   0        0        0     9468 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/Action.xsd
--rw-rw-rw-   0        0        0     3699 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/Citation.xsd
--rw-rw-rw-   0        0        0      448 2022-03-31 22:10:53.000000 potentials-0.3.5/potentials/xsd/FAQ.xsd
--rw-rw-rw-   0        0        0    16696 2022-07-22 17:55:47.000000 potentials-0.3.5/potentials/xsd/Potential.xsd
--rw-rw-rw-   0        0        0     5944 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/Request.xsd
--rw-rw-rw-   0        0        0        0 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/xsd/__pycache__/
--rw-rw-rw-   0        0        0      164 2022-07-25 16:45:13.000000 potentials-0.3.5/potentials/xsd/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1318 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/artifact.xsd
--rw-rw-rw-   0        0        0     3982 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/implementation.xsd
--rw-rw-rw-   0        0        0     1316 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/link.xsd
--rw-rw-rw-   0        0        0      667 2021-08-03 11:09:29.000000 potentials-0.3.5/potentials/xsd/parameter.xsd
--rw-rw-rw-   0        0        0     5499 2022-07-25 16:28:26.000000 potentials-0.3.5/potentials/xsd/potential_LAMMPS.xsd
--rw-rw-rw-   0        0        0     1718 2022-07-25 16:28:08.000000 potentials-0.3.5/potentials/xsd/potential_LAMMPS_KIM.xsd
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/xsl/
--rw-rw-rw-   0        0        0      891 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/Action.xsl
--rw-rw-rw-   0        0        0     3657 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/Citation.xsl
--rw-rw-rw-   0        0        0      583 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/FAQ.xsl
--rw-rw-rw-   0        0        0    10387 2022-10-03 14:26:23.000000 potentials-0.3.5/potentials/xsl/Potential.xsl
--rw-rw-rw-   0        0        0     1759 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/Request.xsl
--rw-rw-rw-   0        0        0        0 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:21.000000 potentials-0.3.5/potentials/xsl/__pycache__/
--rw-rw-rw-   0        0        0      164 2021-08-09 15:09:12.000000 potentials-0.3.5/potentials/xsl/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      584 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/artifact.xsl
--rw-rw-rw-   0        0        0     5446 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/implementation.xsl
--rw-rw-rw-   0        0        0      580 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/link.xsl
--rw-rw-rw-   0        0        0      582 2021-08-03 11:09:30.000000 potentials-0.3.5/potentials/xsl/parameter.xsl
--rw-rw-rw-   0        0        0     2203 2022-07-22 20:07:25.000000 potentials-0.3.5/potentials/xsl/potential_LAMMPS.xsl
--rw-rw-rw-   0        0        0     2218 2022-07-25 16:04:25.000000 potentials-0.3.5/potentials/xsl/potential_LAMMPS_KIM.xsl
-drwxrwxrwx   0        0        0        0 2022-10-03 14:41:20.000000 potentials-0.3.5/potentials.egg-info/
--rw-rw-rw-   0        0        0     4243 2022-10-03 14:41:20.000000 potentials-0.3.5/potentials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3337 2022-10-03 14:41:20.000000 potentials-0.3.5/potentials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-03 14:41:20.000000 potentials-0.3.5/potentials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-02-04 15:07:00.000000 potentials-0.3.5/potentials.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      121 2022-10-03 14:41:20.000000 potentials-0.3.5/potentials.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-03 14:41:20.000000 potentials-0.3.5/potentials.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-03-31 22:10:53.000000 potentials-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-03 14:41:21.000000 potentials-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1746 2022-10-03 14:38:24.000000 potentials-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/
+-rw-rw-rw-   0        0        0     2776 2020-07-21 17:56:46.000000 potentials-0.3.6/LICENSE.TXT
+-rw-rw-rw-   0        0        0      160 2022-06-01 17:13:54.000000 potentials-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4243 2023-04-18 20:20:19.000000 potentials-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3463 2021-09-14 15:58:47.000000 potentials-0.3.6/README.rst
+-rw-rw-rw-   0        0        0     3083 2023-04-04 19:01:01.000000 potentials-0.3.6/UPDATES.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/Database/
+-rw-rw-rw-   0        0        0    14382 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/__init__.py
+-rw-rw-rw-   0        0        0    15046 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_action.py
+-rw-rw-rw-   0        0        0    18665 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_citation.py
+-rw-rw-rw-   0        0        0    11655 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_faq.py
+-rw-rw-rw-   0        0        0    14818 2023-04-04 15:40:25.000000 potentials-0.3.6/potentials/Database/_kim_potential.py
+-rw-rw-rw-   0        0        0    42725 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_lammps_potential.py
+-rw-rw-rw-   0        0        0    17183 2023-04-04 17:08:21.000000 potentials-0.3.6/potentials/Database/_potential.py
+-rw-rw-rw-   0        0        0    24254 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_record.py
+-rw-rw-rw-   0        0        0    10620 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_related_models.py
+-rw-rw-rw-   0        0        0    12559 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/_request.py
+-rw-rw-rw-   0        0        0    11603 2023-03-24 17:02:24.000000 potentials-0.3.6/potentials/Database/_widgets.py
+-rw-rw-rw-   0        0        0     1228 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Database/load_database.py
+-rw-rw-rw-   0        0        0     9996 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/Settings.py
+-rw-rw-rw-   0        0        0        5 2023-04-04 17:52:48.000000 potentials-0.3.6/potentials/VERSION
+-rw-rw-rw-   0        0        0      727 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/buildrecord/
+-rw-rw-rw-   0        0        0      107 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/buildrecord/__init__.py
+-rw-rw-rw-   0        0        0     1359 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/build_lammps_potential.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/
+-rw-rw-rw-   0        0        0     6135 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EamBuilder.py
+-rw-rw-rw-   0        0        0     5551 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EimBuilder.py
+-rw-rw-rw-   0        0        0     5916 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/KimBuilder.py
+-rw-rw-rw-   0        0        0     6212 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py
+-rw-rw-rw-   0        0        0    13157 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PairBuilder.py
+-rw-rw-rw-   0        0        0     6210 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py
+-rw-rw-rw-   0        0        0    19230 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py
+-rw-rw-rw-   0        0        0      315 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/paramfile/
+-rw-rw-rw-   0        0        0    51311 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/EAM.py
+-rw-rw-rw-   0        0        0    55972 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/EAMAlloy.py
+-rw-rw-rw-   0        0        0    57842 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/EAMFS.py
+-rw-rw-rw-   0        0        0      192 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/paramfile/__init__.py
+-rw-rw-rw-   0        0        0     6747 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/paramfile/converters.py
+-rw-rw-rw-   0        0        0     2188 2022-09-19 13:36:46.000000 potentials-0.3.6/potentials/paramfile/load_eam.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/record/
+-rw-rw-rw-   0        0        0    13706 2023-04-07 14:29:04.000000 potentials-0.3.6/potentials/record/Action.py
+-rw-rw-rw-   0        0        0     7400 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Artifact.py
+-rw-rw-rw-   0        0        0    21924 2023-04-04 16:04:52.000000 potentials-0.3.6/potentials/record/BasePotentialLAMMPS.py
+-rw-rw-rw-   0        0        0    11669 2023-04-03 20:05:11.000000 potentials-0.3.6/potentials/record/Citation.py
+-rw-rw-rw-   0        0        0     5378 2023-04-03 20:06:44.000000 potentials-0.3.6/potentials/record/FAQ.py
+-rw-rw-rw-   0        0        0    12748 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Implementation.py
+-rw-rw-rw-   0        0        0     5258 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Link.py
+-rw-rw-rw-   0        0        0     5363 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/record/Parameter.py
+-rw-rw-rw-   0        0        0    17400 2023-04-04 17:06:29.000000 potentials-0.3.6/potentials/record/Potential.py
+-rw-rw-rw-   0        0        0    25778 2023-04-04 15:19:25.000000 potentials-0.3.6/potentials/record/PotentialLAMMPS.py
+-rw-rw-rw-   0        0        0    36541 2023-04-04 16:09:47.000000 potentials-0.3.6/potentials/record/PotentialLAMMPSKIM.py
+-rw-rw-rw-   0        0        0    11939 2023-04-03 20:24:30.000000 potentials-0.3.6/potentials/record/Request.py
+-rw-rw-rw-   0        0        0      655 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/record/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/tools/
+-rw-rw-rw-   0        0        0      446 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/tools/__pycache__/
+-rw-rw-rw-   0        0        0      543 2022-03-31 22:26:25.000000 potentials-0.3.6/potentials/tools/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1173 2019-07-31 19:39:47.000000 potentials-0.3.6/potentials/tools/__pycache__/aslist.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7975 2022-05-25 17:25:42.000000 potentials-0.3.6/potentials/tools/__pycache__/atomic_info.cpython-37.pyc
+-rw-rw-rw-   0        0        0   152808 2021-08-03 17:29:36.000000 potentials-0.3.6/potentials/tools/__pycache__/atomicdata.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1399 2022-05-25 17:25:42.000000 potentials-0.3.6/potentials/tools/__pycache__/numderivative.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1546 2022-05-25 17:25:42.000000 potentials-0.3.6/potentials/tools/__pycache__/parse_authors.cpython-37.pyc
+-rw-rw-rw-   0        0        0      601 2020-07-23 20:51:50.000000 potentials-0.3.6/potentials/tools/__pycache__/screen_input.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1610 2019-12-28 16:49:05.000000 potentials-0.3.6/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc
+-rw-rw-rw-   0        0        0    11550 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/atomic_info.py
+-rw-rw-rw-   0        0        0   132864 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/atomicdata.csv
+-rw-rw-rw-   0        0        0     1448 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/numderivative.py
+-rw-rw-rw-   0        0        0     2200 2022-05-23 16:10:08.000000 potentials-0.3.6/potentials/tools/parse_authors.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsd/
+-rw-rw-rw-   0        0        0     9468 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/Action.xsd
+-rw-rw-rw-   0        0        0     3699 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/Citation.xsd
+-rw-rw-rw-   0        0        0      448 2022-03-31 22:10:53.000000 potentials-0.3.6/potentials/xsd/FAQ.xsd
+-rw-rw-rw-   0        0        0    16696 2022-07-22 17:55:47.000000 potentials-0.3.6/potentials/xsd/Potential.xsd
+-rw-rw-rw-   0        0        0     5944 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/Request.xsd
+-rw-rw-rw-   0        0        0        0 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsd/__pycache__/
+-rw-rw-rw-   0        0        0      164 2022-07-25 16:45:13.000000 potentials-0.3.6/potentials/xsd/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1318 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/artifact.xsd
+-rw-rw-rw-   0        0        0     3982 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/implementation.xsd
+-rw-rw-rw-   0        0        0     1316 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/link.xsd
+-rw-rw-rw-   0        0        0      667 2021-08-03 11:09:29.000000 potentials-0.3.6/potentials/xsd/parameter.xsd
+-rw-rw-rw-   0        0        0     5499 2022-07-25 16:28:26.000000 potentials-0.3.6/potentials/xsd/potential_LAMMPS.xsd
+-rw-rw-rw-   0        0        0     1718 2022-07-25 16:28:08.000000 potentials-0.3.6/potentials/xsd/potential_LAMMPS_KIM.xsd
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsl/
+-rw-rw-rw-   0        0        0      891 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/Action.xsl
+-rw-rw-rw-   0        0        0     3657 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/Citation.xsl
+-rw-rw-rw-   0        0        0      583 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/FAQ.xsl
+-rw-rw-rw-   0        0        0    10387 2022-10-03 14:26:23.000000 potentials-0.3.6/potentials/xsl/Potential.xsl
+-rw-rw-rw-   0        0        0     1759 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/Request.xsl
+-rw-rw-rw-   0        0        0        0 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials/xsl/__pycache__/
+-rw-rw-rw-   0        0        0      164 2021-08-09 15:09:12.000000 potentials-0.3.6/potentials/xsl/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      584 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/artifact.xsl
+-rw-rw-rw-   0        0        0     5446 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/implementation.xsl
+-rw-rw-rw-   0        0        0      580 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/link.xsl
+-rw-rw-rw-   0        0        0      582 2021-08-03 11:09:30.000000 potentials-0.3.6/potentials/xsl/parameter.xsl
+-rw-rw-rw-   0        0        0     2203 2022-07-22 20:07:25.000000 potentials-0.3.6/potentials/xsl/potential_LAMMPS.xsl
+-rw-rw-rw-   0        0        0     2218 2022-07-25 16:04:25.000000 potentials-0.3.6/potentials/xsl/potential_LAMMPS_KIM.xsl
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/
+-rw-rw-rw-   0        0        0     4243 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3360 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-02-04 15:07:00.000000 potentials-0.3.6/potentials.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      121 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 20:20:19.000000 potentials-0.3.6/potentials.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-03-31 22:10:53.000000 potentials-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 20:20:19.000000 potentials-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-04-04 18:08:19.000000 potentials-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:20:19.000000 potentials-0.3.6/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-03 14:26:23.000000 potentials-0.3.6/tests/test_settings.py
```

### Comparing `potentials-0.3.5/LICENSE.TXT` & `potentials-0.3.6/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/PKG-INFO` & `potentials-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potentials
-Version: 0.3.5
+Version: 0.3.6
 Summary: API database tools for accessing the NIST Interatomic Potentials Repository: explore and download interatomic potentials and computed properties.
 Home-page: https://github.com/usnistgov/potentials
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics,interatomic potential,force field
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `potentials-0.3.5/README.rst` & `potentials-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/UPDATES.rst` & `potentials-0.3.6/UPDATES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Updates
 =======
 
+0.3.6
+-----
+
+- Code adjustments related to yabadaba 0.2.0 updates to Query handling.
+  The parameters supported by query operations can now be viewed with
+  querydoc.
+
 0.3.5
 -----
 
 - URL fields added to Potential and BasePotentialLAMMPS records which are
   used as PIDs on potentials.nist.gov, i.e. permanent hyperlinks for the
   records.
 - XSL and XSD representations updated to coincide with record structure and
```

### Comparing `potentials-0.3.5/potentials/Database/__init__.py` & `potentials-0.3.6/potentials/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_action.py` & `potentials-0.3.6/potentials/Database/_action.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_citation.py` & `potentials-0.3.6/potentials/Database/_citation.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_faq.py` & `potentials-0.3.6/potentials/Database/_faq.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_kim_potential.py` & `potentials-0.3.6/potentials/Database/_kim_potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # https://numpy.org/
 import numpy as np
 
 # https://pandas.pydata.org/
 import pandas as pd
 
 # https://github.com/usnistgov/yabadaba
-from yabadaba import query
+from yabadaba import load_query
 
 # Local imports
 from ..tools import aslist
 from .. import settings, load_record
 
 @property
 def kim_models(self) -> list:
@@ -194,16 +194,16 @@
 
     records2 = np.array(records2)
     df2 = pd.DataFrame(df2)
 
     # Filter by key and id if needed
     if len(records2) > 0:
         matches = (
-            query.str_match.pandas(df2, 'key', key)
-            &query.str_match.pandas(df2, 'id', id)
+            load_query('str_match', name='key').pandas(df2, key)
+            &load_query('str_match', name='id').pandas(df2, id)
         )
         df2 = df2[matches]
         records2 = records2[matches]
         df2.reset_index(drop=True)
 
     if verbose:
         print(f'Built {len(records2)} lammps potentials for KIM models')
@@ -281,15 +281,15 @@
 
     # Build bash commands to list kim api collections
     commands = f'source {kim_api_directory}/kim-api-activate\n'
     commands += 'kim-api-collections-management list'
     
     # Run commands as a subprocess
     process = subprocess.Popen('/bin/bash', stdin=subprocess.PIPE, stdout=subprocess.PIPE, text=True)
-    out, err = process.communicate(commands)
+    out = process.communicate(commands)[0]
 
     # Parse output to extract installed KIM models
     self.__kim_models = []
     capture = False
     for line in out.split('\n'):
         line = line.strip()
```

### Comparing `potentials-0.3.5/potentials/Database/_lammps_potential.py` & `potentials-0.3.6/potentials/Database/_lammps_potential.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_potential.py` & `potentials-0.3.6/potentials/Database/_potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
                    name: Union[str, list, None] = None,
                    key: Union[str, list, None] = None,
                    id: Union[str, list, None] = None,
                    notes: Union[str, list, None] = None,
                    fictional: Union[bool, list, None] = None,
                    element: Union[str, list, None] = None,
                    othername: Union[str, list, None] = None,
-                   modelname: Union[str, list, None] = None,
                    year: Union[int, list, None] = None,
                    author: Union[str, list, None] = None,
                    abstract: Union[str, list, None] = None,
                    local: Optional[bool] = None,
                    remote: Optional[bool] = None,
                    refresh_cache: bool = False,
                    return_df: bool = False,
@@ -45,19 +44,15 @@
     notes : str or list
         Term(s) to search for in the potential's notes field.
     fictional : bool
         Limits based on if the potential is labeled as fictional or not.
     element : str or list
         Element(s) in the model to parse by.
     othername : str or list
-        Alternate system names (often compounds or molecules) to parse by.
-    modelname : str or list
-        Identifying model names to parse by.  These are used to differentiate
-        between potentials that would otherwise have the same id based on year,
-        primary author and elements. 
+        Alternate system names (often compounds or molecules) to parse by. 
     year : int or list
         Publication year(s) to parse by.
     author : str or list
         Author name(s) to parse by.  This works best for last names only.
     abstract : str or list
         Term(s) to search for in the potential's citation's abstract field.
     local : bool, optional
@@ -87,26 +82,25 @@
     pandas.DataFrame
         A table of the records' metadata.  Returned if return_df = True.
     """
     return self.get_records(
         style='Potential', name=name, local=local, remote=remote,
         refresh_cache=refresh_cache, return_df=return_df, verbose=verbose,
         key=key, id=id, notes=notes, fictional=fictional, element=element,
-        othername=othername, modelname=modelname, year=year, author=author,
+        othername=othername, year=year, author=author,
         abstract=abstract)
 
 def get_potential(self, 
                   name: Union[str, list, None] = None,
                   key: Union[str, list, None] = None,
                   id: Union[str, list, None] = None,
                   notes: Union[str, list, None] = None,
                   fictional: Union[bool, list, None] = None,
                   element: Union[str, list, None] = None,
                   othername: Union[str, list, None] = None,
-                  modelname: Union[str, list, None] = None,
                   year: Union[int, list, None] = None,
                   author: Union[str, list, None] = None,
                   abstract: Union[str, list, None] = None,
                   local: Optional[bool] = None,
                   remote: Optional[bool] = None, 
                   prompt: bool = True,
                   refresh_cache: bool = False,
@@ -127,18 +121,14 @@
         Term(s) to search for in the potential's notes field.
     fictional : bool
         Limits based on if the potential is labeled as fictional or not.
     element : str or list
         Element(s) in the model to parse by.
     othername : str or list
         Alternate system names (often compounds or molecules) to parse by.
-    modelname : str or list
-        Identifying model names to parse by.  These are used to differentiate
-        between potentials that would otherwise have the same id based on year,
-        primary author and elements. 
     year : int or list
         Publication year(s) to parse by.
     author : str or list
         Author name(s) to parse by.  This works best for last names only.
     abstract : str or list
         Term(s) to search for in the potential's citation's abstract field.
     local : bool, optional
@@ -162,27 +152,26 @@
         If True, info messages will be printed during operations.  Default
         value is False.
     """
     return self.get_record(
         style='Potential', name=name, local=local, remote=remote, 
         prompt=prompt, refresh_cache=refresh_cache, verbose=verbose,
         key=key, id=id, notes=notes, fictional=fictional, element=element,
-        othername=othername, modelname=modelname, year=year, author=author,
+        othername=othername, year=year, author=author,
         abstract=abstract)
 
 def retrieve_potential(self, 
                        name: Union[str, list, None] = None,
                        dest: Optional[Path] = None,
                        key: Union[str, list, None] = None,
                        id: Union[str, list, None] = None,
                        notes: Union[str, list, None] = None,
                        fictional: Union[bool, list, None] = None,
                        element: Union[str, list, None] = None,
                        othername: Union[str, list, None] = None,
-                       modelname: Union[str, list, None] = None,
                        year: Union[int, list, None] = None,
                        author: Union[str, list, None] = None,
                        abstract: Union[str, list, None] = None,
                        local: Optional[bool] = None,
                        remote: Optional[bool] = None, 
                        prompt: bool = True,
                        format: str = 'json',
@@ -208,18 +197,14 @@
         Term(s) to search for in the potential's notes field.
     fictional : bool
         Limits based on if the potential is labeled as fictional or not.
     element : str or list
         Element(s) in the model to parse by.
     othername : str or list
         Alternate system names (often compounds or molecules) to parse by.
-    modelname : str or list
-        Identifying model names to parse by.  These are used to differentiate
-        between potentials that would otherwise have the same id based on year,
-        primary author and elements. 
     year : int or list
         Publication year(s) to parse by.
     author : str or list
         Author name(s) to parse by.  This works best for last names only.
     abstract : str or list
         Term(s) to search for in the potential's citation's abstract field.
     local : bool, optional
@@ -259,26 +244,25 @@
         If multiple or no matching records are discovered.
     """
     self.retrieve_record(
         style='Potential', name=name, dest=dest, local=local, remote=remote,
         prompt=prompt, format=format, indent=indent,
         refresh_cache=refresh_cache, verbose=verbose,
         key=key, id=id, notes=notes, fictional=fictional, element=element,
-        othername=othername, modelname=modelname, year=year, author=author,
+        othername=othername, year=year, author=author,
         abstract=abstract)
 
 def download_potentials(self, 
                         name: Union[str, list, None] = None,
                         key: Union[str, list, None] = None,
                         id: Union[str, list, None] = None,
                         notes: Union[str, list, None] = None,
                         fictional: Union[bool, list, None] = None,
                         element: Union[str, list, None] = None,
                         othername: Union[str, list, None] = None,
-                        modelname: Union[str, list, None] = None,
                         year: Union[int, list, None] = None,
                         author: Union[str, list, None] = None,
                         abstract: Union[str, list, None] = None,
                         overwrite: bool = False,
                         return_records: bool = False,
                         verbose: bool = False) -> Optional[np.ndarray]:
     """
@@ -297,18 +281,14 @@
         Term(s) to search for in the potential's notes field.
     fictional : bool
         Limits based on if the potential is labeled as fictional or not.
     element : str or list
         Element(s) in the model to parse by.
     othername : str or list
         Alternate system names (often compounds or molecules) to parse by.
-    modelname : str or list
-        Identifying model names to parse by.  These are used to differentiate
-        between potentials that would otherwise have the same id based on year,
-        primary author and elements. 
     year : int or list
         Publication year(s) to parse by.
     author : str or list
         Author name(s) to parse by.  This works best for last names only.
     abstract : str or list
         Term(s) to search for in the potential's citation's abstract field.
     overwrite : bool, optional
@@ -323,15 +303,15 @@
         value is False.
 
     """
     return self.download_records(
         style='Potential', name=name, overwrite=overwrite,
         return_records=return_records, verbose=verbose,
         key=key, id=id, notes=notes, fictional=fictional, element=element,
-        othername=othername, modelname=modelname, year=year, author=author,
+        othername=othername, year=year, author=author,
         abstract=abstract)
 
 def save_potential(self,
                    potential: Record,
                    overwrite: bool = False,
                    verbose: bool = False):
     """
```

### Comparing `potentials-0.3.5/potentials/Database/_record.py` & `potentials-0.3.6/potentials/Database/_record.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_related_models.py` & `potentials-0.3.6/potentials/Database/_related_models.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_request.py` & `potentials-0.3.6/potentials/Database/_request.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Database/_widgets.py` & `potentials-0.3.6/potentials/Database/_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import numpy as np
 import numpy.typing as npt
 
 # https://pandas.pydata.org/
 import pandas as pd
 
 # Local imports
-from ..record import Potential, PotentialLAMMPS
+from .. import load_record
 
 def widget_search_potentials(self,
                              potentials: Optional[npt.ArrayLike] = None,
                              potentials_df: Optional[pd.DataFrame] = None):
     """
     Builds ipywidgets for selecting an interatomic potential from the database
     and displaying its full html representation (citation plus implementations)
@@ -106,15 +106,15 @@
         # Set author value
         if author_text.value != '':
             author = author_text.value
         else:
             author = None
 
         # Parse potentials using author, year, elements
-        matches = potentials_df[Potential().pandasfilter(potentials_df, author=author, year=year, element=elements)]
+        matches = potentials_df[load_record('Potential').pandasfilter(potentials_df, author=author, year=year, element=elements)]
         
         # Update potential dropdown accordingly
         potential_dropdown.options = matches.id.tolist()
 
     # Tie elements, year and text widgets to above function
     element1_dropdown.observe(update_potential_dropdown_options, 'value')
     element2_dropdown.observe(update_potential_dropdown_options, 'value')
@@ -232,15 +232,15 @@
 
         # Set pair_style value
         pair_style = pair_style_dropdown.value
         if pair_style == '':
             pair_style = None
 
         # Parse for pair_style and elements
-        matches = lammps_potentials_df[PotentialLAMMPS().pandasfilter(lammps_potentials_df, pair_style=pair_style, elements=elements)]
+        matches = lammps_potentials_df[load_record('potential_LAMMPS').pandasfilter(lammps_potentials_df, pair_style=pair_style, elements=elements)]
         
         # Update potential dropdown accordingly
         potential_dropdown.options = matches.id.tolist()
 
     # Tie elements, year and text widgets to above function
     element1_dropdown.observe(update_potential_dropdown_options, 'value')
     element2_dropdown.observe(update_potential_dropdown_options, 'value')
```

### Comparing `potentials-0.3.5/potentials/Database/load_database.py` & `potentials-0.3.6/potentials/Database/load_database.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/Settings.py` & `potentials-0.3.6/potentials/Settings.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/__init__.py` & `potentials-0.3.6/potentials/__init__.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/build_lammps_potential.py` & `potentials-0.3.6/potentials/buildrecord/build_lammps_potential.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/EamBuilder.py` & `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EamBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/EimBuilder.py` & `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/EimBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/KimBuilder.py` & `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/KimBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py` & `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/LibParamBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/PairBuilder.py` & `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PairBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py` & `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/ParamFileBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py` & `potentials-0.3.6/potentials/buildrecord/potential_LAMMPS/PotentialLAMMPSBuilder.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/paramfile/EAM.py` & `potentials-0.3.6/potentials/paramfile/EAM.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/paramfile/EAMAlloy.py` & `potentials-0.3.6/potentials/paramfile/EAMAlloy.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/paramfile/EAMFS.py` & `potentials-0.3.6/potentials/paramfile/EAMFS.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/paramfile/converters.py` & `potentials-0.3.6/potentials/paramfile/converters.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/paramfile/load_eam.py` & `potentials-0.3.6/potentials/paramfile/load_eam.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/record/Action.py` & `potentials-0.3.6/potentials/record/Action.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 from typing import Optional, Tuple, Union
 
 # https://github.com/usnistgov/DataModelDict
 from DataModelDict import DataModelDict as DM
 
 # https://github.com/usnistgov/yabadaba
 from yabadaba.record import Record
-from yabadaba import load_query 
-
-# https://pandas.pydata.org/
-import pandas as pd
+from yabadaba import load_query
 
 # Local imports
 from . import Potential
 
 __all__ = ['Action']
 
 class PotInfo():
@@ -32,54 +29,54 @@
         ----------
         potential : Potential, str or DataModelDict
             A Potential record object or DataModelDict contents for a Potential
             record.  This prodives the information to link the Potential to the
             Action.
         """
         if isinstance(potential, Potential.Potential):
-            
+
             # Extract relevant properties from the Potential object
             self.__id = potential.id
             self.__key = potential.key
             self.__dois = []
             for citation in potential.citations:
                 try:
                     self.__dois.append(citation.doi)
                 except:
                     pass
             self.__fictional = potential.fictional
             self.__elements = potential.elements
             self.__othername = potential.othername
-            
+
         else:
 
             # Extract relevant properties from potential record contents
             model = DM(potential).find('potential')
             self.__id = model['id']
             self.__key = model['key']
             self.__dois = model.aslist('doi')
 
             felements = model.aslist('fictional-element')
             oelements = model.aslist('other-element')
             elements = model.aslist('element')
-            
+
             if len(felements) > 0:
                 assert len(elements) == 0
                 self.__fictional = True
                 self.__elements = felements
             else:
                 assert len(elements) > 0
                 self.__fictional = False
                 self.__elements = elements
             if len(oelements) > 0:
                 assert len(oelements) == 1
                 self.__othername = oelements[0]
             else:
                 self.__othername = None
-    
+
     @property
     def id(self) -> str:
         """str: The Potential's id"""
         return self.__id
 
     @property
     def key(self) -> str:
@@ -91,47 +88,47 @@
         """list: The Potential's DOIs"""
         return self.__dois
 
     @property
     def elements(self) -> list:
         """list: The elements modeled by the Potential"""
         return self.__elements
-    
+
     @property
     def othername(self) -> Optional[str]:
         """str or None: The Potential's othername"""
         return self.__othername
-    
+
     @property
     def fictional(self) -> bool:
         """bool: Flag indicating if the Potential is classified as fictional."""
         return self.__fictional
 
     def build_model(self) -> DM:
         """
         Generates and returns model content based on the values set to object.
         """
         # Build core elements
         model = DM()
         model['potential'] = DM()
         model['potential']['key'] = self.key
         model['potential']['id'] = self.id
-        
+
         # Append DOIs
         for doi in self.dois:
             model['potential'].append('doi', doi)
 
         # Add elements or fictional elements
         if self.fictional:
             for element in self.elements:
                 model['potential'].append('fictional-element', element)
         else:
             for element in self.elements:
                 model['potential'].append('element', element)
-        
+
         # Add othername if set
         if self.othername is not None:
             model['potential']['other-element'] = self.othername
 
         #self._set_model(model)
         return model
 
@@ -187,15 +184,15 @@
         """str: The record style"""
         return 'Action'
 
     @property
     def modelroot(self) -> str:
         """str: The root element of the content"""
         return 'action'
-    
+
     @property
     def xsl_filename(self) -> Tuple[str, str]:
         """tuple: The module path and file name of the record's xsl html transformer"""
         return ('potentials.xsl', 'Action.xsl')
 
     @property
     def xsd_filename(self) -> Tuple[str, str]:
@@ -297,27 +294,28 @@
             The Action type to assign to the record.
         potentials : list, optional
             Potential or model contents for Potential records to associate
             with the action.
         comment : str, optional
             Any additional comments to assign to the record.
         """
+
         if date is not None:
             self.date = date
         if type is not None:
             self.type = type
         if comment is not None:
             self.comment = comment
         if potentials is not None:
             self.__potentials = []
             for potential in potentials:
                 self.potentials.append(PotInfo(potential))
 
         if name is not None:
-            self.name = name
+            super().set_values(name=name)
         elif date is not None or comment is not None:
             self.build_name()
 
     def build_name(self):
         """Builds a name for the record based on date + comment"""
         if self.comment is None:
             self.name = f"{self.date}"
@@ -329,15 +327,15 @@
         Generates and returns model content based on the values set to object.
         """
         # Add Action's date and type
         model = DM()
         model['action'] = DM()
         model['action']['date'] = str(self.date)
         model['action']['type'] = self.type 
-        
+
         # Add any related potentials
         for potential in self.potentials:
             model['action'].append('potential', potential.build_model()['potential'])
 
         # Add comments
         if self.comment is not None:
             model['action']['comment'] = self.comment
@@ -352,166 +350,49 @@
         for multiple records of the same style.
         """
         data = {}
         data['name'] = self.name
         data['date'] = self.date
         data['type'] = self.type
         data['comment'] = self.comment
-        
+
         data['potentials'] = []
         for pot in self.potentials:
             data['potentials'].append(pot.metadata())
-        
+
         return data
 
     @property
     def queries(self) -> dict:
         """dict: Query objects and their associated parameter names."""
         return {
             'date': load_query(
                 style = 'date_match',
-                name = 'date', 
-                path = f'{self.modelroot}.date'),
+                name = 'date',
+                path = f'{self.modelroot}.date',
+                description='search for web update actions on specific dates'),
             'type': load_query(
                 style = 'str_match',
                 name = 'type',
-                path = f'{self.modelroot}.type'),
+                path = f'{self.modelroot}.type',
+                description="search by the action type: 'new posting', 'updated posting', 'retraction', 'site change'"),
             'potential_id': load_query(
                 style = 'str_match',
                 name = 'id', parent = 'potentials',
-                path = f'{self.modelroot}.potential.id'),
+                path = f'{self.modelroot}.potential.id',
+                description="search based on the ids of the involved potentials"),
             'potential_key': load_query(
                 style = 'str_match',
                 name = 'key', parent = 'potentials',
-                path = f'{self.modelroot}.potential.key'),
+                path = f'{self.modelroot}.potential.key',
+                description="search based on the UUID keys of the involved potentials"),
             'element': load_query(
                 style = 'list_contains',
                 name = 'element', parent = 'potentials',
-                path = f'{self.modelroot}.potential.element'),
+                path = f'{self.modelroot}.potential.element',
+                description='search based on the elements of the involved potentials'),
             'comment': load_query(
                 style = 'str_contains',
                 name = 'comment',
-                path = f'{self.modelroot}.comment'),
+                path = f'{self.modelroot}.comment',
+                description='search for comments containing specific strings'),
         }
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     date: Union[str, list, None] = None,
-                     type: Union[str, list, None] = None,
-                     potential_id: Union[str, list, None] = None,
-                     potential_key: Union[str, list, None] = None,
-                     element: Union[str, list, None] = None,
-                     comment: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list, optional
-            The record name(s) to parse by.
-        date : str or list, optional
-            The date associated with the record.
-        type : str or list, optional
-            The type of action: 'new posting', 'updated posting', 'retraction',
-            or 'site change'.
-        potential_id : str or list, optional
-            Limits results to entries related to the given potential id.
-        potential_key : str or list, optional
-            Limits results to entries related to the given potential key.
-        element : str or list, optional
-            Limits results to entries related to potentials with the given
-            element(s).
-        comment : str or list, optional
-            Term(s) to search for in the action's comment field.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, date=date, type=type,
-                                       potential_id=potential_id,
-                                       potential_key=potential_key, element=element,
-                                       comment=comment)
-        return matches
-
-    def mongoquery(self, 
-                   name: Union[str, list, None] = None,
-                   date: Union[str, list, None] = None,
-                   type: Union[str, list, None] = None,
-                   potential_id: Union[str, list, None] = None,
-                   potential_key: Union[str, list, None] = None,
-                   element: Union[str, list, None] = None,
-                   comment: Union[str, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        name : str or list, optional
-            The record name(s) to parse by.
-        date : str or list, optional
-            The date associated with the record.
-        type : str or list, optional
-            The type of action: 'new posting', 'updated posting', 'retraction',
-            or 'site change'.
-        potential_id : str or list, optional
-            Limits results to entries related to the given potential id.
-        potential_key : str or list, optional
-            Limits results to entries related to the given potential key.
-        element : str or list, optional
-            Limits results to entries related to potentials with the given
-            element(s).
-        comment : str or list, optional
-            Term(s) to search for in the action's comment field.
-        
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """        
-        mquery = super().mongoquery(name=name, date=date, type=type,
-                                       potential_id=potential_id,
-                                       potential_key=potential_key, element=element,
-                                       comment=comment)
-        return mquery
-
-    def cdcsquery(self,
-                  date: Union[str, list, None] = None,
-                  type: Union[str, list, None] = None,
-                  potential_id: Union[str, list, None] = None,
-                  potential_key: Union[str, list, None] = None,
-                  element: Union[str, list, None] = None,
-                  comment: Union[str, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        date : str or list, optional
-            The date associated with the record.
-        type : str or list, optional
-            The type of action: 'new posting', 'updated posting', 'retraction',
-            or 'site change'.
-        potential_id : str or list, optional
-            Limits results to entries related to the given potential id.
-        potential_key : str or list, optional
-            Limits results to entries related to the given potential key.
-        element : str or list, optional
-            Limits results to entries related to potentials with the given
-            element(s).
-        comment : str or list, optional
-            Term(s) to search for in the action's comment field.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(date=date, type=type,
-                                   potential_id=potential_id,
-                                   potential_key=potential_key, element=element,
-                                   comment=comment)
-        return mquery
```

### Comparing `potentials-0.3.5/potentials/record/Artifact.py` & `potentials-0.3.6/potentials/record/Artifact.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/record/BasePotentialLAMMPS.py` & `potentials-0.3.6/potentials/record/BasePotentialLAMMPS.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,25 @@
 import numpy.typing as npt
 
 # https://github.com/usnistgov/DataModelDict
 from DataModelDict import DataModelDict as DM
 
 # https://github.com/usnistgov/yabadaba
 from yabadaba.record import Record
-from yabadaba import query 
-
-# https://pandas.pydata.org/
-import pandas as pd
 
 # atomman imports
 from ..tools import aslist, atomic_mass
 
 class BasePotentialLAMMPS(Record):
     """
     Base parent class for PotentialLAMMPS objects
     """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
-                 name: Optional[str] = None,
-                 **kwargs):
+                 name: Optional[str] = None):
         """
         Initializes an instance and loads content from a data model.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
@@ -40,25 +35,38 @@
             The record name to use.  If not given, this will be set to the
             potential's id.
         **kwargs : any, optional
             Any other keyword parameters supported by the child class.
         """
         # Check if base class is initialized directly
         if self.__module__ == __name__:
-            raise TypeError("Don't use base class")
-        
+            raise TypeError("don't use base class")
+
         # Set default values
         self.pot_dir = ''
         self.__artifacts = []
+        self._id = None
+        self._key = None
+        self._url = None
+        self._potid = None
+        self._potkey = None
+        self._poturl = None
+        self._units = None
+        self._atom_style = None
+        self._elements = []
+        self._symbols = []
+        self._masses = []
+        self._charges = []
+        self._pair_style = None
+        self._allsymbols = False
+        self._status = None
+
 
         # Pass parameters to load
-        if model is not None:
-            self.load_model(model, name=name, **kwargs)
-        elif name is not None:
-            self.name = name
+        super().__init__(model, name=name)
         
     @property
     def id(self) -> str:
         """str : Human-readable identifier for the LAMMPS implementation."""
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self._id
@@ -197,16 +205,15 @@
                 else:
                     num_skipped += 1
 
         return num_downloaded, num_skipped
 
     def load_model(self,
                    model: Union[str, io.IOBase, DM],
-                   name: Optional[str] = None,
-                   **kwargs):
+                   name: Optional[str] = None):
         """
         Loads data model info associated with a LAMMPS potential.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict
             A JSON/XML data model for the content.
@@ -218,36 +225,36 @@
 
         # Extract values from model
         pot = self.model[self.modelroot]
 
         self._id = pot['id']
         try:
             self.name
-        except:
+        except AttributeError:
             self.name = self.id
 
         self._key = pot['key']
         self._url = pot.get('key', None)
         try:
             self._potid = pot['potential']['id']
-        except:
+        except (KeyError, TypeError):
             self._potid = None
         try:
             self._potkey = pot['potential']['key']
-        except:
+        except (KeyError, TypeError):
             self._potkey = None
         try:
             self._poturl = pot['potential']['url']
-        except:
+        except (KeyError, TypeError):
             self._poturl = None
         self._units = pot.get('units', 'metal')
         self._atom_style = pot.get('atom_style', 'atomic')
         try:
             self._pair_style = pot['pair_style']['type']
-        except:
+        except (KeyError, TypeError):
             self._pair_style = None
 
         allsymbols = pot.get('allsymbols', False)
         if isinstance(allsymbols, bool):
             self._allsymbols = allsymbols
         elif allsymbols.lower() == 'true':
             self._allsymbols = True
@@ -422,81 +429,14 @@
         d['pair_style'] = self.pair_style
         d['status'] = self.status
         d['symbols'] = self.symbols
         d['elements'] = self.elements()
 
         return d
 
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     key: Union[str, list, None] = None,
-                     id: Union[str, list, None] = None,
-                     potid: Union[str, list, None] = None,
-                     potkey: Union[str, list, None] = None,
-                     units: Union[str, list, None] = None,
-                     atom_style: Union[str, list, None] = None,
-                     pair_style: Union[str, list, None] = None,
-                     status: Union[str, list, None] = None,
-                     symbols: Union[str, list, None] = None,
-                     elements: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list, optional
-            The record name(s) to parse by.
-        key : str or list, optional
-            The UUID4 key(s) associated with the LAMMPS implementations to
-            parse by.
-        id : str or list, optional
-            The unique id(s) associated with the LAMMPS implementations to
-            parse by.
-        potid : str or list, optional
-            The unique id(s) associated with the general potential model to
-            parse by.
-        potkey : str or list, optional
-            The UUID4 key(s) associated with the general potential model to
-            parse by.
-        units : str or list, optional
-            The LAMMPS unit style(s) to parse by.
-        atom_style : str or list, optional
-            The LAMMPS atom_style values(s) to parse by.
-        pair_style : str or list, optional
-            The LAMMPS pair_style values(s) to parse by.
-        status : str or list, optional
-            The implementation status value(s) to parse by.
-        symbols : str or list, optional
-            Symbol model(s) to parse by.
-        elements : str or list, optional
-            Elemental tag(s) to parse by.
-
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        matches = (
-            query.str_match.pandas(dataframe, 'name', name)
-            &query.str_match.pandas(dataframe, 'key', key)
-            &query.str_match.pandas(dataframe, 'id', id)
-            &query.str_match.pandas(dataframe, 'potkey', potkey)
-            &query.str_match.pandas(dataframe, 'potid', potid)
-            &query.str_match.pandas(dataframe, 'units', units)
-            &query.str_match.pandas(dataframe, 'atom_style', atom_style)
-            &query.str_match.pandas(dataframe, 'pair_style', pair_style)
-            &query.str_match.pandas(dataframe, 'status', status)
-            &query.in_list.pandas(dataframe, 'symbols', symbols)
-            &query.in_list.pandas(dataframe, 'elements', elements)
-        )
-        return matches
-
     def build_model(self) -> DM:
         if self.model is None:
             raise AttributeError('No model information loaded')
         return self.model
 
     def pair_info(self,
                   symbols: Union[str, list, None] = None,
@@ -639,8 +579,8 @@
 
         Returns
         -------
         str
             The LAMMPS input command lines that specifies the potential and a restart
             file to read.
         """
-        raise NotImplementedError('Needs to be defined by the child class')
+        raise NotImplementedError('Needs to be defined by the child class')
```

### Comparing `potentials-0.3.5/potentials/record/Citation.py` & `potentials-0.3.6/potentials/record/Citation.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 import bibtexparser
 from bibtexparser.bparser import BibTexParser
 from bibtexparser.customization import convert_to_unicode
 from bibtexparser.bibdatabase import BibDatabase
 
 # https://github.com/usnistgov/yabadaba
 from yabadaba.record import Record
-from yabadaba import load_query 
+from yabadaba import load_query
 
-# https://pandas.pydata.org/
-import pandas as pd
 class Citation(Record):
     """
     Class for representing Citation metadata records.
     """
 
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
@@ -76,15 +74,15 @@
         return self.__bib
 
     @property
     def doifname(self) -> str:
         """str: file path compatible form of doi"""
         try:
             name = self.bib['doi']
-        except:
+        except KeyError:
             name = self.bib['note']
         return name.lower().replace('/', '_')
 
     def load_model(self,
                    model: Union[str, io.IOBase, DM],
                    name: Optional[str] = None):
         """
@@ -154,19 +152,19 @@
         DataModelDict: The data model content.
         """
         citmodel = DM()
         
         def asint(val):
             try:
                 return int(val)
-            except:
+            except (TypeError, ValueError):
                 return val
 
         if self.bib['ENTRYTYPE'] == 'article':
-            citmodel['document-type'] = 'journal' 
+            citmodel['document-type'] = 'journal'
             citmodel['title'] = self.bib['title']
             citmodel['author'] = self.parse_authors(self.bib['author'])
             if 'journal' in self.bib:
                 citmodel['publication-name'] = self.bib['journal']
             citmodel['publication-date'] = DM()
             citmodel['publication-date']['year'] = asint(self.bib['year'])
             if 'volume' in self.bib:
@@ -212,168 +210,48 @@
     @property
     def queries(self) -> dict:
         """dict: Query objects and their associated parameter names."""
         return {
             'year': load_query(
                 style='int_match',
                 name='year', 
-                path=f'{self.modelroot}.publication-date.year'),
+                path=f'{self.modelroot}.publication-date.year',
+                description="search based on publication year"),
             'volume': load_query(
                 style='str_match',
                 name='volume',
-                path=f'{self.modelroot}.volume'),
+                path=f'{self.modelroot}.volume',
+                description="search based on volume number"),
             'title': load_query(
                 style='str_contains',
                 name='title',
-                path=f'{self.modelroot}.title'),
+                path=f'{self.modelroot}.title',
+                description="search article titles for contained strings"),
             'journal': load_query(
                 style='str_match',
                 name='journal',
-                path=f'{self.modelroot}..publication-name'),
+                path=f'{self.modelroot}..publication-name',
+                description="search based on publication journal name"),
             'doi': load_query(
                 style='str_match',
                 name='doi',
-                path=f'{self.modelroot}.DOI'),
+                path=f'{self.modelroot}.DOI',
+                description="search based on publication DOI"),
             'author': load_query(
                 style='str_contains',
                 name='author',
-                path=f'{self.modelroot}.author.surname'),
+                path=f'{self.modelroot}.author.surname',
+                description="search based on publication author"),
             'abstract': load_query(
                 style='str_contains',
                 name='abstract',
-                path=f'{self.modelroot}.abstract'),
+                path=f'{self.modelroot}.abstract',
+                description="search article abstract for contained strings"),
         }
 
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     year: Union[int, list, None] = None,
-                     volume: Union[int, list, None] = None,
-                     title: Union[str, list, None] = None,
-                     journal: Union[str, list, None] = None,
-                     doi: Union[str, list, None] = None,
-                     author: Union[str, list, None] = None,
-                     abstract: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list
-            The record name(s) to parse by.
-        year : int or list
-            The publication/creation year for the citation.
-        volume : int or list
-            The journal volume for the citation.
-        title : str or list
-            The article title for the citation.
-        journal : str or list
-            The journal name.
-        doi : str or list
-            The citation's DOI.
-        author : str or list
-            Author names to search for - only guaranteed to work with last names.
-        abstract : str or list
-            Key words to search for in the citation abstract.
-
-        Returns
-        -------
-        pandas.Series, numpy.NDArray
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, year=year,
-                                       volume=volume, title=title,
-                                       journal=journal, doi=doi, author=author,
-                                       abstract=abstract)
-
-        return matches
-
-    def mongoquery(self,
-                   name: Union[str, list, None] = None,
-                   year: Union[int, list, None] = None,
-                   volume: Union[int, list, None] = None,
-                   title: Union[str, list, None] = None,
-                   journal: Union[str, list, None] = None,
-                   doi: Union[str, list, None] = None,
-                   author: Union[str, list, None] = None,
-                   abstract: Union[str, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        name : str or list
-            The record name(s) to parse by.
-        year : int or list
-            The publication/creation year for the citation.
-        volume : int or list
-            The journal volume for the citation.
-        title : str or list
-            The article title for the citation.
-        journal : str or list
-            The journal name.
-        doi : str or list
-            The citation's DOI.
-        author : str or list
-            Author names to search for - only guaranteed to work with last names.
-        abstract : str or list
-            Key words to search for in the citation abstract.
-        
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """        
-        
-        mquery = super().mongoquery(name=name, year=year,
-                                    volume=volume, title=title,
-                                    journal=journal, doi=doi, author=author,
-                                    abstract=abstract)
-        return mquery
-
-    def cdcsquery(self,
-                  year: Union[int, list, None] = None,
-                  volume: Union[int, list, None] = None,
-                  title: Union[str, list, None] = None,
-                  journal: Union[str, list, None] = None,
-                  doi: Union[str, list, None] = None,
-                  author: Union[str, list, None] = None,
-                  abstract: Union[str, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        year : int or list
-            The publication/creation year for the citation.
-        volume : int or list
-            The journal volume for the citation.
-        title : str or list
-            The article title for the citation.
-        journal : str or list
-            The journal name.
-        doi : str or list
-            The citation's DOI.
-        author : str or list
-            Author names to search for - only guaranteed to work with last names.
-        abstract : str or list
-            Key words to search for in the citation abstract.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(year=year, volume=volume, title=title,
-                                   journal=journal, doi=doi, author=author,
-                                   abstract=abstract)
-        return mquery
-
     @property
     def year_authors(self) -> str:
         """
         str: Partial id for potentials that uses YEAR--LAST-F-M with up to 4 authors.
         """
         partialid = str(self.bib['year']) + '-'
         authors = self.parse_authors(self.bib['author'])
```

### Comparing `potentials-0.3.5/potentials/record/FAQ.py` & `potentials-0.3.6/potentials/record/FAQ.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 from typing import Optional, Tuple, Union
 
 # https://github.com/usnistgov/DataModelDict
 from DataModelDict import DataModelDict as DM
 
 # https://github.com/usnistgov/yabadaba
 from yabadaba.record import Record
-from yabadaba import load_query 
-
-# https://pandas.pydata.org/
-import pandas as pd
+from yabadaba import load_query
 
 __all__ = ['FAQ']
 
 class FAQ(Record):
     """
     Class for representing FAQ records that document the FAQs for the NIST
     Interatomic Potentials Repository.
@@ -155,86 +152,15 @@
     @property
     def queries(self) -> dict:
         """dict: Query objects and their associated parameter names."""
         return {
             'question': load_query(
                 style='str_contains',
                 name='question',
-                path=f'{self.modelroot}.question'),
+                path=f'{self.modelroot}.question',
+                description="search FAQ question for matching strings"),
             'answer': load_query(
                 style='str_contains',
                 name='answer',
-                path=f'{self.modelroot}.answer'),
+                path=f'{self.modelroot}.answer',
+                description="search FAQ answer for matching strings"),
         }
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     question: Union[str, list, None] = None,
-                     answer: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list
-            The record name(s) to parse by.
-        question : str or list
-            Term(s) to search for in the question field.
-        answer : str or list
-            Term(s) to search for in the answer field.
-        
-        Returns
-        -------
-        pandas.Series, numpy.NDArray
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, question=question,
-                                       answer=answer)
-        return matches
-
-    def mongoquery(self,
-                   name: Union[str, list, None] = None,
-                   question: Union[str, list, None] = None,
-                   answer: Union[str, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        name : str or list
-            The record name(s) to parse by.
-        question : str or list
-            Term(s) to search for in the question field.
-        answer : str or list
-            Term(s) to search for in the answer field.
-        
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """     
-        mquery = super().mongoquery(name=name, question=question, answer=answer)
-        return mquery
-
-    def cdcsquery(self,
-                  question: Union[str, list, None] = None,
-                  answer: Union[str, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        question : str or list
-            Term(s) to search for in the question field.
-        answer : str or list
-            Term(s) to search for in the answer field.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(question=question, answer=answer)
-        return mquery
```

### Comparing `potentials-0.3.5/potentials/record/Implementation.py` & `potentials-0.3.6/potentials/record/Implementation.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/record/Link.py` & `potentials-0.3.6/potentials/record/Link.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/record/Parameter.py` & `potentials-0.3.6/potentials/record/Parameter.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/record/PotentialLAMMPS.py` & `potentials-0.3.6/potentials/record/PotentialLAMMPS.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import numpy as np
 import numpy.typing as npt
 
 # https://github.com/usnistgov/DataModelDict
 from DataModelDict import DataModelDict as DM
 
 # https://github.com/usnistgov/yabadaba
-from yabadaba import query
+from yabadaba import load_query
 
 # local imports
-from ..tools import atomic_mass, aslist
+from ..tools import aslist
 from .BasePotentialLAMMPS import BasePotentialLAMMPS
 from .Artifact import Artifact
 
 class PotentialLAMMPS(BasePotentialLAMMPS):
     """
     Class for building LAMMPS input lines from a potential-LAMMPS data model.
     """
@@ -40,16 +40,16 @@
             The record name to use.  If not given, this will be set to the
             potential's id.
         pot_dir : str, optional
             The path to a directory containing any artifacts associated with
             the potential.  Default value is None, which assumes any required
             files will be in the working directory when LAMMPS is executed.
         """
-        super().__init__(model=model, name=name, pot_dir=pot_dir)
-        if model is None and pot_dir is not None:
+        super().__init__(model=model, name=name)
+        if pot_dir is not None:
             self.pot_dir = pot_dir
 
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'potential_LAMMPS'
 
@@ -115,15 +115,18 @@
         return out
  
     @property
     def artifacts(self) -> list:
         """list : The list of file artifacts for the potential including download URLs."""
         return self.__artifacts
 
-    def load_model(self, model, name=None, pot_dir=None):
+    def load_model(self,
+                   model: Union[str, io.IOBase, DM],
+                   name: Optional[str] = None,
+                   pot_dir: Optional[str] = None):
         """
         Loads potential-LAMMPS data model info.
         
         Parameters
         ----------
         model : str, file-like object or DataModelDict
             A JSON/XML data model for the content.
@@ -179,149 +182,119 @@
             
             # Add values to the lists
             self._elements.append(element)
             self._symbols.append(symbol)
             self._masses.append(mass)
             self._charges.append(charge)
     
+    @property
+    def queries(self) -> dict:
+        """dict: Query objects and their associated parameter names."""
+        return {
+            'key': load_query(
+                style='str_match',
+                name='key',
+                path=f'{self.modelroot}.key',
+                description="search based on the implementation's UUID key"),
+            'id': load_query(
+                style='str_match',
+                name='id',
+                path=f'{self.modelroot}.id',
+                description="search based on the implementation's id"),
+            'potkey': load_query(
+                style='str_match',
+                name='potkey',
+                path=f'{self.modelroot}.potential.key',
+                description="search based on the potential's UUID key"),
+            'potid': load_query(
+                style='str_match',
+                name='potid',
+                path=f'{self.modelroot}.potential.id',
+                description="search based on the potential's id"),
+            'units': load_query(
+                style='str_match',
+                name='units',
+                path=f'{self.modelroot}.units',
+                description="search based on LAMMPS units setting"),
+            'atom_style': load_query(
+                style='str_match',
+                name='atom_style',
+                path=f'{self.modelroot}.atom_style',
+                description="search based on LAMMPS atom_style setting"),
+            'pair_style': load_query(
+                style='str_match',
+                name='pair_style',
+                path=f'{self.modelroot}.pair_style.type',
+                description="search based on LAMMPS pair_style setting"),
+            'status': load_query(
+                style='str_match',
+                name='status',
+                path=f'{self.modelroot}.status',
+                description="search based on implementation status: active, superseded or retracted"),
+            'symbols': load_query(
+                style='list_contains',
+                name='symbols',
+                path=f'{self.modelroot}.atom.symbol',
+                description="search based on atomic model symbols"),
+            'elements': load_query(
+                style='list_contains',
+                name='elements',
+                path=f'{self.modelroot}.atom.element',
+                description="search based on atomic model elements"),
+        }
+
     def mongoquery(self,
                    name: Union[str, list, None] = None,
-                   key: Union[str, list, None] = None,
-                   id: Union[str, list, None] = None,
-                   potid: Union[str, list, None] = None,
-                   potkey: Union[str, list, None] = None,
-                   units: Union[str, list, None] = None,
-                   atom_style: Union[str, list, None] = None,
-                   pair_style: Union[str, list, None] = None,
-                   status: Union[str, list, None] = None,
-                   symbols: Union[str, list, None] = None,
-                   elements: Union[str, list, None] = None) -> dict:
+                   **kwargs) -> dict:
         """
         Builds a Mongo-style query based on kwargs values for the record style.
         
         Parameters
         ----------
-        name : str or list, optional
+        name : str or list
             The record name(s) to parse by.
-        key : str or list, optional
-            The UUID4 key(s) associated with the LAMMPS implementations to
-            parse by.
-        id : str or list, optional
-            The unique id(s) associated with the LAMMPS implementations to
-            parse by.
-        potid : str or list, optional
-            The unique id(s) associated with the general potential model to
-            parse by.
-        potkey : str or list, optional
-            The UUID4 key(s) associated with the general potential model to
-            parse by.
-        units : str or list, optional
-            The LAMMPS unit style(s) to parse by.
-        atom_style : str or list, optional
-            The LAMMPS atom_style values(s) to parse by.
-        pair_style : str or list, optional
-            The LAMMPS pair_style values(s) to parse by.
-        status : str or list, optional
-            The implementation status value(s) to parse by.
-        symbols : str or list, optional
-            Symbol model(s) to parse by.
-        elements : str or list, optional
-            Elemental tag(s) to parse by.
+        **kwargs : any
+            Any of the record style-specific search parameters.
         
         Returns
         -------
         dict
             The Mongo-style query
         """
-        if status is not None:
-            status = aslist(status)
-            if 'active' in status:
-                status.append(None)
-
-        mquery = {}
-        query.str_match.mongo(mquery, f'name', name)
-
-        root = f'content.{self.modelroot}'
-        query.str_match.mongo(mquery, f'{root}.key', key)
-        query.str_match.mongo(mquery, f'{root}.id', id)
-        query.str_match.mongo(mquery, f'{root}.potential.id', potid)
-        query.str_match.mongo(mquery, f'{root}.potential.key', potkey)
-        query.str_match.mongo(mquery, f'{root}.units', units)
-        query.str_match.mongo(mquery, f'{root}.atom_style', atom_style)
-        query.str_match.mongo(mquery, f'{root}.pair_style.type', pair_style)
-        query.str_match.mongo(mquery, f'{root}.status', status)
-        query.in_list.mongo(mquery, f'{root}.atom.element', elements)
-        query.in_list.mongo(mquery, f'{root}.atom.symbol', symbols)
+        # Modify status
+        if 'status' in kwargs and kwargs['status'] is not None:
+            kwargs['status'] = aslist(kwargs['status'])
+            if 'active' in kwargs['status']:
+                kwargs['status'].append(None)
+
+        mquery = super().mongoquery(name=name, **kwargs)
 
         return mquery
 
-    def cdcsquery(self,
-                  key: Union[str, list, None] = None,
-                  id: Union[str, list, None] = None,
-                  potid: Union[str, list, None] = None,
-                  potkey: Union[str, list, None] = None,
-                  units: Union[str, list, None] = None,
-                  atom_style: Union[str, list, None] = None,
-                  pair_style: Union[str, list, None] = None,
-                  status: Union[str, list, None] = None,
-                  symbols: Union[str, list, None] = None,
-                  elements: Union[str, list, None] = None) -> dict:
+    def cdcsquery(self, **kwargs) -> dict:
         """
         Builds a CDCS-style query based on kwargs values for the record style.
         
         Parameters
         ----------
-        key : str or list, optional
-            The UUID4 key(s) associated with the LAMMPS implementations to
-            parse by.
-        id : str or list, optional
-            The unique id(s) associated with the LAMMPS implementations to
-            parse by.
-        potid : str or list, optional
-            The unique id(s) associated with the general potential model to
-            parse by.
-        potkey : str or list, optional
-            The UUID4 key(s) associated with the general potential model to
-            parse by.
-        units : str or list, optional
-            The LAMMPS unit style(s) to parse by.
-        atom_style : str or list, optional
-            The LAMMPS atom_style values(s) to parse by.
-        pair_style : str or list, optional
-            The LAMMPS pair_style values(s) to parse by.
-        status : str or list, optional
-            The implementation status value(s) to parse by.
-        symbols : str or list, optional
-            Symbol model(s) to parse by.
-        elements : str or list, optional
-            Elemental tag(s) to parse by.
+        **kwargs : any
+            Any of the record style-specific search parameters.
         
         Returns
         -------
         dict
             The CDCS-style query
         """
-        if status is not None:
-            status = aslist(status)
-            if 'active' in status:
-                status.append(None)
-
-        mquery = {}
-        root = self.modelroot
-
-        query.str_match.mongo(mquery, f'{root}.key', key)
-        query.str_match.mongo(mquery, f'{root}.id', id)
-        query.str_match.mongo(mquery, f'{root}.potential.id', potid)
-        query.str_match.mongo(mquery, f'{root}.potential.key', potkey)
-        query.str_match.mongo(mquery, f'{root}.units', units)
-        query.str_match.mongo(mquery, f'{root}.atom_style', atom_style)
-        query.str_match.mongo(mquery, f'{root}.pair_style.type', pair_style)
-        query.str_match.mongo(mquery, f'{root}.status', status)
-        query.in_list.mongo(mquery, f'{root}.atom.element', elements)
-        query.in_list.mongo(mquery, f'{root}.atom.symbol', symbols)
+        # Modify status
+        if 'status' in kwargs and kwargs['status'] is not None:
+            kwargs['status'] = aslist(kwargs['status'])
+            if 'active' in kwargs['status']:
+                kwargs['status'].append(None)
+
+        mquery = super().cdcsquery(**kwargs)
 
         return mquery
     
     @property
     def symbolsets(self) -> list:
         """list : The sets of symbols that correspond to all related potentials"""
         return [self._symbols]
```

### Comparing `potentials-0.3.5/potentials/record/PotentialLAMMPSKIM.py` & `potentials-0.3.6/potentials/record/PotentialLAMMPSKIM.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from DataModelDict import DataModelDict as DM
 
 # https://numpy.org/
 import numpy as np
 import numpy.typing as npt
 
 # https://github.com/usnistgov/yabadaba
-from yabadaba import query 
+from yabadaba import load_query
 
 # local imports
 from ..tools import aslist
 from .BasePotentialLAMMPS import BasePotentialLAMMPS
 class PotentialLAMMPSKIM(BasePotentialLAMMPS):
     """
     Class for building LAMMPS input lines from a potential-LAMMPS-KIM data model.
@@ -54,19 +54,35 @@
             This controls which symbols are available.
         symbolset : str or list, optional
             Specifies which potential (by symbols value) to use.  Only important
             if the kim model is associated with multiple potential entries.
             If potkey or potid is not given, then the first potential entry
             found with all listed symbols will be selected.
         """
-        super().__init__(model=model, name=name, id=id, potkey=potkey, potid=potid,
-                         symbolset=symbolset)
-        if model is None and id is not None:
-            self.id = id
-    
+
+        # Call super with only name
+        super().__init__(model=None, name=name)
+
+        # Call load_model if needed
+        if model is not None:
+            self.load_model(model=model, name=name, id=id, potkey=potkey,
+                            potid=potid, symbolset=symbolset)
+        
+        elif id is not None:
+            raise ValueError('model must be given with id')
+        elif potkey is not None:
+            raise ValueError('model must be given with potkey')
+        elif potid is not None:
+            raise ValueError('model must be given with potid')
+        elif symbolset is not None:
+            raise ValueError('model must be given with symbolset')
+
+        # Explicitly set pair_style
+        self._pair_style = 'kim'
+
     @property
     def style(self) -> str:
         """str: The record style"""
         return 'potential_LAMMPS_KIM'
 
     @property
     def shortcode(self) -> str:
@@ -159,14 +175,17 @@
             If potkey or potid is not given, then the first potential entry
             found with all listed symbols will be selected.
         """
         # Call parent load to read model and some parameters
         super().load_model(model, name=name)
         kimpot = self.model[self.modelroot]
         
+        # Explicitly set pair_style
+        self._pair_style = 'kim'
+        
         # Handle shortcode, id and name identifiers
         self.__shortcode = kimpot['id']
         if id is not None:
             self._id = id
         else:
             # Get last known id
             self._id = kimpot.aslist('full-kim-id')[-1]
@@ -174,17 +193,14 @@
         # Set key as shortcode plus version
         self._key = self.id.split('__')[-1]
         
         # Set name as shortcode
         if self.name is None:
             self.name = self.shortcode
         
-        # Explicitly set pair_style
-        self._pair_style = 'kim'
-        
         # Initialize fields for atomic info
         self._potkeys = []
         self._potids = []
         self._symbolsets = []
         self._elementsets = []
         self._masssets = []
         self._chargesets = []
@@ -244,186 +260,174 @@
         self._elements = self._fullelements
         self._masses = self._fullmasses
         self._charges = self._fullcharges
 
         # Select the potential model
         self.select_potential(potkey=potkey, potid=potid, symbolset=symbolset)
 
+    @property
+    def queries(self) -> dict:
+        """dict: Query objects and their associated parameter names."""
+        return {
+            'key': load_query(
+                style='str_match',
+                name='key',
+                path=f'{self.modelroot}.key',
+                description="search based on the implementation's UUID key"),
+            'id': load_query(
+                style='str_match',
+                name='id',
+                path=f'{self.modelroot}.id',
+                description="search based on the implementation's id (KIM ID)"),
+            'potkey': load_query(
+                style='str_match',
+                name='potkey',
+                path=f'{self.modelroot}.potential.key',
+                description="search based on the potential's UUID key"),
+            'potid': load_query(
+                style='str_match',
+                name='potid',
+                path=f'{self.modelroot}.potential.id',
+                description="search based on the potential's id"),
+            'units': load_query(
+                style='str_match',
+                name='units',
+                path=None,
+                description="search based on LAMMPS units setting"),
+            'atom_style': load_query(
+                style='str_match',
+                name='atom_style',
+                path=None,
+                description="search based on LAMMPS atom_style setting"),
+            'pair_style': load_query(
+                style='str_match',
+                name='pair_style',
+                path=None,
+                description="search based on LAMMPS pair_style setting"),
+            'status': load_query(
+                style='str_match',
+                name='status',
+                path=f'{self.modelroot}.status',
+                description="search based on implementation status: active, superseded or retracted"),
+            'symbols': load_query(
+                style='list_contains',
+                name='symbols',
+                path=f'{self.modelroot}.potential.atom.symbol',
+                description="search based on atomic model symbols"),
+            'elements': load_query(
+                style='list_contains',
+                name='elements',
+                path=f'{self.modelroot}.potential.atom.element',
+                description="search based on atomic model elements"),
+        }
+
     def mongoquery(self,
                    name: Union[str, list, None] = None,
-                   key: Union[str, list, None] = None,
-                   id: Union[str, list, None] = None,
-                   potid: Union[str, list, None] = None,
-                   potkey: Union[str, list, None] = None,
-                   units: Union[str, list, None] = None,
-                   atom_style: Union[str, list, None] = None,
-                   pair_style: Union[str, list, None] = None,
-                   status: Union[str, list, None] = None,
-                   symbols: Union[str, list, None] = None,
-                   elements: Union[str, list, None] = None) -> dict:
+                   **kwargs) -> dict:
         """
         Builds a Mongo-style query based on kwargs values for the record style.
         
         Parameters
         ----------
-        name : str or list, optional
+        name : str or list
             The record name(s) to parse by.
-        key : str or list, optional
-            The UUID4 key(s) associated with the LAMMPS implementations to
-            parse by.
-        id : str or list, optional
-            The unique id(s) associated with the LAMMPS implementations to
-            parse by.
-        potid : str or list, optional
-            The unique id(s) associated with the general potential model to
-            parse by.
-        potkey : str or list, optional
-            The UUID4 key(s) associated with the general potential model to
-            parse by.
-        units : str or list, optional
-            The LAMMPS unit style(s) to parse by.
-        atom_style : str or list, optional
-            The LAMMPS atom_style values(s) to parse by.
-        pair_style : str or list, optional
-            The LAMMPS pair_style values(s) to parse by.
-        status : str or list, optional
-            The implementation status value(s) to parse by.
-        symbols : str or list, optional
-            Symbol model(s) to parse by.
-        elements : str or list, optional
-            Elemental tag(s) to parse by.
+        **kwargs : any
+            Any of the record style-specific search parameters.
         
         Returns
         -------
         dict
             The Mongo-style query
         """
 
         # Return bad query if pair_style kim not included
-        if pair_style is not None and 'kim' not in aslist(pair_style):
+        if ('pair_style' in kwargs and
+            kwargs['pair_style'] is not None and 
+            'kim' not in aslist(kwargs['pair_style'])):
             return {"not.kim.pair_style":"get nothing"}
-        
-        # Transform key, id values into shortcodes for query
+
+        # Modify status
+        if 'status' in kwargs and kwargs['status'] is not None:
+            kwargs['status'] = aslist(kwargs['status'])
+            if 'active' in kwargs['status']:
+                kwargs['status'].append(None)
+
+        # Transform id values into shortcodes for query
         shortcodes = set()
-        if key is not None:
-            for k in aslist(key):
-                shortcode = '_'.join(k.split('_')[:-1])
-                shortcodes.add(shortcode)
-        if id is not None:
-            for i in aslist(id):
+        if 'id' in kwargs and kwargs['id'] is not None:
+            for i in aslist(kwargs['id']):
                 k = i.split('__')[-1]
                 shortcode = '_'.join(k.split('_')[:-1])
                 shortcodes.add(shortcode)
         if len(shortcodes) == 0:
             shortcodes = None
         else:
             shortcodes = list(shortcodes)
+        kwargs['id'] = shortcodes
 
-        mquery = {}
-        query.str_match.mongo(mquery, f'name', name)
+        # Remove terms ignored by queries
+        if 'pair_style' in kwargs:
+            del kwargs['pair_style']
+        if 'units' in kwargs:
+            del kwargs['units']
+        if 'atom_style' in kwargs:
+            del kwargs['atom_style']
 
-        root = f'content.{self.modelroot}'
-        #query.str_match.mongo(mquery, f'{root}.key', key)
-        query.str_match.mongo(mquery, f'{root}.id', shortcodes)
-        query.str_match.mongo(mquery, f'{root}.potential.id', potid)
-        query.str_match.mongo(mquery, f'{root}.potential.key', potkey)
-        query.in_list.mongo(mquery, f'{root}.potential.atom.symbol', symbols)
-        query.in_list.mongo(mquery, f'{root}.potential.atom.element', elements)
-        
-        if status is not None:
-            status = aslist(status)
-            if 'active' in status:
-                status.append(None)
-
-        query.str_match.mongo(mquery, f'{root}.status', status)
+        mquery = super().mongoquery(name=name, **kwargs)
         
         return mquery
 
-    def cdcsquery(self,
-                  key: Union[str, list, None] = None,
-                  id: Union[str, list, None] = None,
-                  potid: Union[str, list, None] = None,
-                  potkey: Union[str, list, None] = None,
-                  units: Union[str, list, None] = None,
-                  atom_style: Union[str, list, None] = None,
-                  pair_style: Union[str, list, None] = None,
-                  status: Union[str, list, None] = None,
-                  symbols: Union[str, list, None] = None,
-                  elements: Union[str, list, None] = None) -> dict:
+    def cdcsquery(self, **kwargs) -> dict:
         """
         Builds a CDCS-style query based on kwargs values for the record style.
         
         Parameters
         ----------
-        key : str or list, optional
-            The UUID4 key(s) associated with the LAMMPS implementations to
-            parse by.
-        id : str or list, optional
-            The unique id(s) associated with the LAMMPS implementations to
-            parse by.
-        potid : str or list, optional
-            The unique id(s) associated with the general potential model to
-            parse by.
-        potkey : str or list, optional
-            The UUID4 key(s) associated with the general potential model to
-            parse by.
-        units : str or list, optional
-            The LAMMPS unit style(s) to parse by.
-        atom_style : str or list, optional
-            The LAMMPS atom_style values(s) to parse by.
-        pair_style : str or list, optional
-            The LAMMPS pair_style values(s) to parse by.
-        status : str or list, optional
-            The implementation status value(s) to parse by.
-        symbols : str or list, optional
-            Symbol model(s) to parse by.
-        elements : str or list, optional
-            Elemental tag(s) to parse by.
+        **kwargs : any
+            Any of the record style-specific search parameters.
         
         Returns
         -------
         dict
             The CDCS-style query
         """
-        #  Return bad query if pair_style kim not included
-        if pair_style is not None and 'kim' not in aslist(pair_style):
+        # Return bad query if pair_style kim not included
+        if ('pair_style' in kwargs and
+            kwargs['pair_style'] is not None and 
+            'kim' not in aslist(kwargs['pair_style'])):
             return {"not.kim.pair_style":"get nothing"}
 
-        # Transform key, id values into shortcodes for query
+        # Modify status
+        if 'status' in kwargs and kwargs['status'] is not None:
+            kwargs['status'] = aslist(kwargs['status'])
+            if 'active' in kwargs['status']:
+                kwargs['status'].append(None)
+
+        # Transform id values into shortcodes for query
         shortcodes = set()
-        if key is not None:
-            for k in aslist(key):
-                shortcode = '_'.join(k.split('_')[:-1])
-                shortcodes.add(shortcode)
-        if id is not None:
-            for i in aslist(id):
+        if 'id' in kwargs and kwargs['id'] is not None:
+            for i in aslist(kwargs['id']):
                 k = i.split('__')[-1]
                 shortcode = '_'.join(k.split('_')[:-1])
                 shortcodes.add(shortcode)
         if len(shortcodes) == 0:
             shortcodes = None
         else:
             shortcodes = list(shortcodes)
+        kwargs['id'] = shortcodes
 
-        mquery = {}
-        root = self.modelroot
-
-        #query.str_match.mongo(mquery, f'{root}.key', key)
-        query.str_match.mongo(mquery, f'{root}.id', shortcodes)
-        query.str_match.mongo(mquery, f'{root}.potential.id', potid)
-        query.str_match.mongo(mquery, f'{root}.potential.key', potkey)
-        query.in_list.mongo(mquery, f'{root}.potential.atom.symbol', symbols)
-        query.in_list.mongo(mquery, f'{root}.potential.atom.element', elements)
-
-        if status is not None:
-            status = aslist(status)
-            if 'active' in status:
-                status.append(None)
+        # Remove terms ignored by queries
+        if 'pair_style' in kwargs:
+            del kwargs['pair_style']
+        if 'units' in kwargs:
+            del kwargs['units']
+        if 'atom_style' in kwargs:
+            del kwargs['atom_style']
 
-        query.str_match.mongo(mquery, f'{root}.status', status)
+        mquery = super().cdcsquery(**kwargs)
 
         return mquery
 
     @property
     def symbolsets(self) -> list:
         """list : The sets of symbols that correspond to all related potentials"""
         if self.model is None:
@@ -480,15 +484,15 @@
             self._masses = self._masssets[0]
             self._charges = self._chargesets[0]
 
             if symbolset is not None:
                 # Check that symbols are in symbolset
                 for symbol in aslist(symbolset):
                     if symbol not in self.symbols:
-                        raise ValueError(f'symbolset does not match potential')
+                        raise ValueError('symbolset does not match potential')
             if potkey is not None:
                 if potkey != self.potkey:
                     raise ValueError('potkey does not match potential')
             if potid is not None:
                 if potid != self.potid:
                     raise ValueError('potid does not match potential')
 
@@ -518,15 +522,15 @@
                     if potkey != self.potkey:
                         raise ValueError('potkey does not match potential given by potid')
                 
                 # Check that symbols are in symbolset
                 if symbolset is not None:
                     for symbol in aslist(symbolset):
                         if symbol not in self.symbols:
-                            raise ValueError(f'symbolset does not match potential given by potid')
+                            raise ValueError('symbolset does not match potential given by potid')
                 
             elif potkey is not None:
                 # Find match and set values
                 i = self.potkeys.index(potkey)
                 self._potid = self._potids[i]
                 self._potkey = self._potkeys[i]
                 self._symbols = self._symbolsets[i]
```

### Comparing `potentials-0.3.5/potentials/record/Request.py` & `potentials-0.3.6/potentials/record/Potential.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,31 @@
 # coding: utf-8
 # Standard Python libraries
 import io
 from typing import Optional, Tuple, Union
+import uuid
 import datetime
 
 # https://github.com/usnistgov/DataModelDict
-from DataModelDict import DataModelDict as DM 
+from DataModelDict import DataModelDict as DM
 
 # https://github.com/usnistgov/yabadaba
 from yabadaba.record import Record
-from yabadaba import load_query 
+from yabadaba import load_query
 
-# https://pandas.pydata.org/
-import pandas as pd
-
-# local imports
+# Local imports
+from .Citation import Citation
+from .Implementation import Implementation
 from ..tools import aslist
 
-class System():
+class Potential(Record):
     """
-    Component class for representing an elemental system being requested.
+    Class for representing Potential metadata records.
     """
-    def __init__(self,
-                 model: Union[str, io.IOBase, DM, None] = None,
-                 formula: Optional[str] = None,
-                 elements: Union[str, list, None] = None):
-        """
-        Class initializer.
-
-        Parameters
-        ----------
-        model : str, file-like object or DataModelDict, optional
-            The contents of the record associated with the system info.
-        formula : str, optional
-            A specific chemical formula being requested.
-        elements : str or list, optional
-            A set of elements for the elemental system being requested.
-        """
-        if model is not None:
-            try:
-                assert formula is None
-                assert elements is None
-            except AssertionError as e:
-                raise ValueError('model cannot be given with any other arguments') from e
-            self.load_model(model)
-        else:
-            self.formula = formula
-            self.elements = elements
-
-    @property
-    def formula(self) -> Optional[str]:
-        """str : A specific chemical formula being requested."""
-        return self.__formula
-
-    @formula.setter
-    def formula(self, value: Optional[str]):
-        if value is None:
-            self.__formula = None
-        else:
-            self.__formula = str(value)
-
-    @property
-    def elements(self) -> Optional[list]:
-        """list : A combination of elements being requested."""
-        return self.__elements
-
-    @elements.setter
-    def elements(self, value: Union[str, list, None]):
-        if value is None:
-            self.__elements = []
-        else:
-            self.__elements = aslist(value)
-
-    def load_model(self, model: Union[str, io.IOBase, DM]):
-        """
-        Loads record contents from a given model.
 
-        Parameters
-        ----------
-        model : str, file-like object or DataModelDict
-            A JSON/XML data model for the content.
-        """
-        model = DM(model).find('system')
-        self.formula = model.get('chemical-formula', None)
-        self.elements = model.get('element', None)
-
-    def build_model(self) -> DM:
-        """
-        Generates and returns model content based on the values set to object.
-        """
-        model = DM()
-        model['system'] = DM()
-        if self.formula is not None:
-            model['system']['chemical-formula'] = self.formula
-        if self.elements is not None:
-            for element in self.elements:
-                model['system'].append('element', element)
-        return model
-
-    def metadata(self) -> dict:
-        """
-        Generates a dict of simple metadata values associated with the record.
-        Useful for quickly comparing records and for building pandas.DataFrames
-        for multiple records of the same style.
-        """
-        return {
-            'formula':self.formula,
-            'elements':self.elements}
-
-class Request(Record):
-    """
-    Class for representing Request records that are associated with user
-    requests to the NIST Interatomic Potentials Repository for new potentials.
-    """
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
                  **kwargs):
         """
         Initializes a Record object for a given style.
         
@@ -124,299 +33,471 @@
         ----------
         model : str, file-like object or DataModelDict, optional
             A JSON/XML data model for the content.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
-        date : datetime.date, optional
-            The date the request was made.
-        comment : str, optional
-            Any additional comments for the request, often what type of study
-            the requested potential is wanted for.
-        systems : list, optional
-            The System component objects or associated content to describe
-            the elemental system being requested.
+        
         """
         # Set default values
-        self.__systems = []
-        self.date = datetime.date.today()
-        self.comment = None
+        self.url = None
+        self.elements = None
+        self.key = None
+        self.othername = None
+        self.fictional = False
+        self.modelname = None
+        self.notes = None
+        self.recorddate = datetime.date.today()
+        self.__citations = []
+        self.__implementations = []
 
         super().__init__(model=model, name=name, **kwargs)
 
     @property
     def style(self) -> str:
         """str: The record style"""
-        return 'Request'
+        return 'Potential'
 
     @property
-    def modelroot(self) -> str:
-        """str: The root element of the content"""
-        return 'request'
-    
-    @property
     def xsl_filename(self) -> Tuple[str, str]:
         """tuple: The module path and file name of the record's xsl html transformer"""
-        return ('potentials.xsl', 'Request.xsl')
+        return ('potentials.xsl', 'Potential.xsl')
 
     @property
     def xsd_filename(self) -> Tuple[str, str]:
         """tuple: The module path and file name of the record's xsd schema"""
-        return ('potentials.xsd', 'Request.xsd')
+        return ('potentials.xsd', 'Potential.xsd')
 
     @property
-    def date(self) -> datetime.date:
-        """datetime.date : The date that the request was submitted."""
-        return self.__date
-
-    @date.setter
-    def date(self, value: Union[str, datetime.date]):
-        if isinstance(value, datetime.date):
-            self.__date = value
-        else:
-            self.__date = datetime.datetime.strptime(value, '%Y-%m-%d').date()
+    def modelroot(self) -> str:
+        """str: The root element of the content"""
+        return 'interatomic-potential'
 
-    @property
-    def comment(self) -> Optional[str]:
-        """str: Any additional comments associated with the request."""
-        return self.__comment
+    def load_model(self,
+                   model: Union[str, io.IOBase, DM],
+                   name: Optional[str] = None):
+        """
+        Loads record contents from a given model.
 
-    @comment.setter
-    def comment(self, value: Optional[str]):
-        if value is None:
-            self.__comment = None
+        Parameters
+        ----------
+        model : str, file-like object or DataModelDict
+            A JSON/XML data model for the content.
+        name : str, optional
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        """
+        super().load_model(model, name=name)
+        potential = self.model[self.modelroot]
+        
+        # Extract information
+        self.key = potential['key']
+        self.url = potential.get('URL', None)
+        self.recorddate = potential['record-version']
+        
+        description = potential['description']
+
+        self.__citations = []
+        for citation in description.iteraslist('citation'):
+            self.add_citation(model=DM([('citation', citation)]))
+        if 'notes' in description:
+            self.notes = description['notes']['text']
         else:
-            self.__comment = str(value)
+            self.notes = None
 
-    @property
-    def systems(self) -> list:
-        """list: The System component objects associated with the request."""
-        return self.__systems
+        self.__implementations = []
+        for implementation in potential.iteraslist('implementation'):
+            self.add_implementation(model=DM([('implementation', implementation)]))
+
+        felements = potential.aslist('fictional-element')
+        oelements = potential.aslist('other-element')
+        elements = potential.aslist('element')
+        
+        if len(felements) > 0:
+            assert len(elements) == 0
+            self.fictional = True
+            self.elements = felements
+        else:
+            assert len(elements) > 0
+            self.fictional = False
+            self.elements = elements
+        if len(oelements) > 0:
+            assert len(oelements) == 1
+            self.othername = oelements[0]
+        else:
+            self.othername = None
+        
+        # Identify modelname and check id
+        self.modelname = None
+        pot_id = potential['id']
+        if self.id != pot_id:
+            try:
+                assert self.id == pot_id[:len(self.id)]
+            except AssertionError:
+                print(f"Different ids: {self.id} != {pot_id} {self.key}")
+            else:
+                self.modelname = pot_id[len(self.id):].strip('-')
+                if self.id != pot_id:
+                    print(f"Different ids: {self.id} != {pot_id} {self.key}")
+
+        # Set name based on id if no name given
+        try:
+            self.name
+        except:
+            self.name = f'potential.{self.id}'
 
     def set_values(self,
                    name: Optional[str] = None,
-                   date: Union[datetime.date, str, None] = None,
-                   comment: Optional[str] = None,
-                   systems: Optional[list] = None):
+                   **kwargs):
         """
         Set multiple object attributes at the same time.
-        
+
         Parameters
         ----------
         name : str, optional
-            The unique name to assign to the record.  If model is a file
-            path, then the default record name is the file name without
-            extension.
-        date : datetime.date, optional
-            The date the request was made.
+            The name to assign to the record.  Often inferred from other
+            attributes if not given.
+        date : str or datetime.date, optional
+            The date to assign to the record.
+        type : str, optional
+            The Action type to assign to the record.
+        potentials : list, optional
+            Potential or model contents for Potential records to associate
+            with the action.
         comment : str, optional
-            Any additional comments for the request, often what type of study
-            the requested potential is wanted for.
-        systems : list, optional
-            The System component objects or associated content to describe
-            the elemental system being requested.
-        """
-        
-        if date is not None:
-            self.date = date
-        if comment is not None:
-            self.comment = comment
-        if systems is not None:
-            self.__systems = []
-            if systems is not None:
-                for system in aslist(systems):
-                    if isinstance(system, System):
-                        self.systems.append(system)
-                    else:
-                        self.add_system(**system)
+            Any additional comments to assign to the record.
+        """
+        if 'url' in kwargs:
+            self.url = kwargs['url']
+        if 'elements' in kwargs:
+            self.elements = kwargs['elements']
+        if 'key' in kwargs:
+            self.key = kwargs['key']
+        if 'othername' in kwargs:
+            self.othername = kwargs['othername']
+        if 'fictional' in kwargs:
+            self.fictional = kwargs['fictional']
+        if 'modelname' in kwargs:
+            self.modelname = kwargs['modelname']
+        if 'notes' in kwargs:
+            self.notes = kwargs['notes']
+        if 'recorddate' in kwargs:
+            self.recorddate = kwargs['recorddate']
+        
+        if 'citations' in kwargs:
+            self.__citations = []
+            for citation in aslist(kwargs['citations']):
+                if isinstance(citation, dict):
+                    self.add_citation(**citation)
+                elif isinstance(citation, Citation):
+                    self.citations.append(citation)
+        
+        if 'implementations' in kwargs:
+            self.__implementations = []
+            for implementation in aslist(kwargs['implementations']):
+                if isinstance(implementation, dict):
+                    self.add_implementation(**implementation)
+                elif isinstance(implementation, Implementation):
+                    self.implementations.append(implementation)
 
+        # Set name
         if name is not None:
             self.name = name
         else:
-            elements = []
-            for system in self.systems:
-                elements.extend(system.elements)
-            self.name = f'{self.date} {" ".join(elements)}'
+            try:
+                self.name = f'potential.{self.id}'
+            except:
+                self.name = 'potential.unknown'
 
-    def load_model(self,
-                   model: Union[str, io.IOBase, DM],
-                   name: Optional[str] = None):
-        """
-        Loads record contents from a given model.
+    @property
+    def key(self) -> str:
+        """str : The potential's uuid4 key"""
+        return self.__key
+    
+    @key.setter
+    def key(self, v: Optional[str]):
+        if v is None:
+            self.__key = str(uuid.uuid4())
+        else:
+            self.__key = str(v)
 
-        Parameters
-        ----------
-        model : str, file-like object or DataModelDict
-            A JSON/XML data model for the content.
-        name : str, optional
-            The name to assign to the record.  Often inferred from other
-            attributes if not given.
-        """
-        super().load_model(model, name=name)
-        req = DM(model).find('request')
-        self.date = req['date']
-        self.comment = req.get('comment', None)
-        self.__systems = []
-        for system in req.aslist('system'):
-            self.add_system(model=DM([('system',system)]))
+    @property
+    def id(self) -> str:
+        """str : The potential's unique id generated from citation info"""
+        # Check for a citation
+        if len(self.citations) > 0:
+            potential_id = self.citations[0].year_authors
+        else:
+            return None
+        
+        potential_id += '-'
+        
+        if self.fictional:
+            potential_id += '-fictional'
+        
+        if self.othername is not None:
+            potential_id += '-' + str(self.othername)
+        else:
+            for element in self.elements:
+                potential_id += '-' + element
+        
+        if self.modelname is not None:
+            potential_id += '-' + str(self.modelname)
+        
+        return potential_id
 
-        if name is not None:
-            self.name = name
+    @property
+    def url(self):
+        """str : URL for an online copy of the record."""
+        return self.__url
+
+    @url.setter
+    def url(self, v: Union[str, None]):
+        if v is None:
+            self.__url = None
         else:
-            elements = []
-            for system in self.systems:
-                elements.extend(system.elements)
-            self.name = f'{self.date} {" ".join(elements)}'
+            self.__url = str(v)
 
-    def build_model(self) -> DM:
-        """
-        Generates and returns model content based on the values set to object.
-        """
-        model = DM()
-        model['request'] = DM()
-        model['request']['date'] = str(self.date)
-        for system in self.systems:
-            model['request'].append('system', system.build_model()['system'])
-        if self.comment is not None:
-            model['request']['comment'] = self.comment
+    @property
+    def impid_prefix(self) -> str:
+        """str : The recommended prefix to use for implementation ids"""
+        if len(self.citations) > 0:
+            potential_id = self.citations[0].year_first_author
+        else:
+            return None
+        
+        potential_id += '-'
+        
+        if self.fictional:
+            potential_id += '-fictional'
+        
+        if self.othername is not None:
+            potential_id += '-' + str(self.othername)
+        else:
+            for element in self.elements:
+                potential_id += '-' + element
+        
+        if self.modelname is not None:
+            potential_id += '-' + str(self.modelname)
+        
+        return potential_id
 
-        self._set_model(model)
-        return model
+    @property
+    def recorddate(self) -> datetime.date:
+        """datetime.date : The date associated with the record"""
+        return self.__recorddate
+    
+    @recorddate.setter
+    def recorddate(self, v: Union[datetime.date, str, None]):
+        if v is None:
+            self.__recorddate = datetime.date.today()
+        elif isinstance(v, datetime.date):
+            self.__recorddate = v
+        elif isinstance(v, str):
+            self.__recorddate = datetime.datetime.strptime(v, '%Y-%m-%d').date()
+        else:
+            raise TypeError('Invalid date type')
+
+    @property
+    def citations(self) -> list:
+        """list: Any associated Citation objects"""
+        return self.__citations
+
+    @property
+    def implementations(self) -> list:
+        """list: Any associated Implementation objects"""
+        return self.__implementations
+
+    @property
+    def elements(self) -> list:
+        """list: elements associated with the potential"""
+        return self.__elements
+
+    @elements.setter
+    def elements(self, v: Union[str, list, None]):
+        if v is None:
+            self.__elements = None
+        else:
+            self.__elements = aslist(v)
+    
+    @property
+    def othername(self) -> Optional[str]:
+        """str or None: Alternate name for what the potential models"""
+        return self.__othername
+    
+    @othername.setter
+    def othername(self, v: Optional[str]):
+        if v is None:
+            self.__othername = None
+        else:
+            self.__othername = str(v)
+    
+    @property
+    def fictional(self) -> bool:
+        """bool: Indicates if the potential is classified as fictional"""
+        return self.__fictional
+    
+    @fictional.setter
+    def fictional(self, v: bool):
+        assert isinstance(v, bool)
+        self.__fictional = v
+    
+    @property
+    def modelname(self) -> Optional[str]:
+        """str: Extra tag for differentiating potentials when needed"""
+        return self.__modelname
+    
+    @modelname.setter
+    def modelname(self, v: Optional[str]):
+        if v is None:
+            self.__modelname = None
+        else:
+            self.__modelname = str(v)
+
+    @property
+    def notes(self) -> Optional[str]:
+        """str or None: Any extra notes associated with the potential"""
+        return self.__notes
+
+    @notes.setter
+    def notes(self, v: Optional[str]):
+        if v is None:
+            self.__notes = None
+        else:
+            self.__notes = str(v)
 
     def metadata(self) -> dict:
         """
         Generates a dict of simple metadata values associated with the record.
         Useful for quickly comparing records and for building pandas.DataFrames
         for multiple records of the same style.
         """
         data = {}
-        data['name'] = self.name
-        data['date'] = self.date
-        data['comment'] = self.comment
-        
-        data['systems'] = []
-        for system in self.systems:
-            data['systems'].append(system.metadata())
         
+        # Copy class attributes to dict
+        data['name'] = self.name
+        data['key'] = self.key
+        data['id'] = self.id
+        data['url'] = self.url
+        data['recorddate'] = self.recorddate
+        data['notes'] = self.notes
+        data['fictional'] = self.fictional
+        data['elements'] = self.elements
+        data['othername'] = self.othername
+        data['modelname'] = self.modelname
+        
+        data['citations'] = []
+        for citation in self.citations:
+            data['citations'].append(citation.metadata())
+
+        data['implementations'] = []
+        for implementation in self.implementations:
+            data['implementations'].append(implementation.metadata())
+
         return data
 
-    def add_system(self,
-                   model: Union[str, io.IOBase, DM, None] = None,
-                   formula: Optional[str] = None,
-                   elements: Union[str, list, None] = None):
+    def build_model(self) -> DM:
+        """
+        Generates and returns model content based on the values set to object.
         """
-        Initializes a System component class and appends it to the systems list.
+        # Initialize model
+        model = DM()
+        model['interatomic-potential'] = potential = DM()
+        
+        # Build identifiers
+        potential['key'] = self.key
+        potential['id'] = self.id
+        if self.url is not None:
+            potential['URL'] = self.url
+        potential['record-version'] = str(self.recorddate)
+        
+        # Build description
+        potential['description'] = description = DM()
+        for citation in self.citations:
+            description.append('citation', citation.build_model()['citation'])
+        if self.notes is not None:
+            description['notes'] = DM([('text', self.notes)])
+        
+        # Build implementations
+        for implementation in self.implementations:
+            potential.append('implementation', implementation.build_model()['implementation'])
 
-        Parameters
-        ----------
-        model : str, file-like object or DataModelDict, optional
-            The contents of the record associated with the system info.
-        formula : str, optional
-            A specific chemical formula being requested.
-        elements : str or list, optional
-            A set of elements for the elemental system being requested.
+        # Build element information
+        if self.fictional:
+            for element in self.elements:
+                potential.append('fictional-element', element)
+        else:
+            for element in self.elements:
+                potential.append('element', element)
+        if self.othername is not None:
+            potential['other-element'] = self.othername
+
+        self._set_model(model)
+        return model
+        
+    def add_citation(self, **kwargs):
+        """
+        Initializes a new Citation object and appends it to the citations list.
         """
-        self.systems.append(System(model=model, formula=formula, elements=elements))
+        self.citations.append(Citation(**kwargs))
+
+    def add_implementation(self, **kwargs):
+        """
+        Initializes a new Implementation object and appends it to the implementations list.
+        """
+        implementation = Implementation(**kwargs)
+        for imp in self.implementations:
+            if imp.id == implementation.id:
+                raise ValueError(f'Implementation with id {imp.id} already exists')
+        self.implementations.append(implementation)
 
     @property
     def queries(self) -> dict:
         """dict: Query objects and their associated parameter names."""
         return {
-            'date': load_query(
-                style='date_match',
-                name='date', 
-                path=f'{self.modelroot}.date'),
+            'key': load_query(
+                style='str_match',
+                name='key', 
+                path=f'{self.modelroot}.key',
+                description="search based on potential UUID key"),
+            'id': load_query(
+                style='str_match',
+                name='id',
+                path=f'{self.modelroot}.id',
+                description="search based on potential id"),
+            'notes': load_query(
+                style='str_contains',
+                name='notes',
+                path=f'{self.modelroot}.notes',
+                description='search potential notes for contained strings'),
+            'fictional': load_query(
+                style='str_match',
+                name='fictional',
+                path=f'{self.modelroot}.fictional-element',
+                description='search for fictional potentials'),
             'element': load_query(
                 style='list_contains',
-                name='elements', parent='systems',
-                path=f'{self.modelroot}.system.element'),
-            'comment': load_query(
+                name='elements',
+                path=f'{self.modelroot}.element',
+                description='search based on potential elements'),
+            'othername': load_query(
+                style='str_match',
+                name='othername',
+                path=f'{self.modelroot}.other-element',
+                description='search based on the othername field'),
+            'year': load_query(
+                style='int_match',
+                name='year', parent='citations',
+                path=f'{self.modelroot}.description.citation.publication-date.year',
+                description='search based on publication year'),
+            'author': load_query(
+                style='str_contains',
+                name='author', parent='citations',
+                path=f'{self.modelroot}.description.citation.author.surname',
+                description='search based on publication authors'),
+            'abstract': load_query(
                 style='str_contains',
-                name='comment',
-                path=f'{self.modelroot}.comment'),
+                name='abstract', parent='citations',
+                path=f'{self.modelroot}.description.citation.abstract',
+                description='search publication abstract for contained strings'),
         }
-
-    def pandasfilter(self,
-                     dataframe: pd.DataFrame,
-                     name: Union[str, list, None] = None,
-                     date: Union[str, list, None] = None,
-                     element: Union[str, list, None] = None,
-                     comment: Union[str, list, None] = None) -> pd.Series:
-        """
-        Filters a pandas.DataFrame based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        dataframe : pandas.DataFrame
-            A table of metadata for multiple records of the record style.
-        name : str or list
-            The record name(s) to parse by.
-        date : str or list
-            The date associated with the record.
-        element : str or list
-            Element(s) to search for in the request.
-        comment : str or list
-            Term(s) to search for in the action's comment field.
-        
-        Returns
-        -------
-        pandas.Series
-            Boolean map of matching values
-        """
-        matches = super().pandasfilter(dataframe, name=name, date=date,
-                                       element=element, comment=comment)
-
-        return matches
-
-    def mongoquery(self,
-                   name: Union[str, list, None] = None,
-                   date: Union[str, list, None] = None,
-                   element: Union[str, list, None] = None,
-                   comment: Union[str, list, None] = None) -> dict:
-        """
-        Builds a Mongo-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        name : str or list
-            The record name(s) to parse by.
-        date : str or list
-            The date associated with the record.
-        element : str or list
-            Element(s) to search for in the request.
-        comment : str or list
-            Term(s) to search for in the action's comment field.
-        
-        Returns
-        -------
-        dict
-            The Mongo-style query
-        """     
-        mquery = super().mongoquery(name=name, date=date,
-                                    element=element, comment=comment)
-        return mquery
-
-    def cdcsquery(self,
-                  date: Union[str, list, None] = None,
-                  element: Union[str, list, None] = None,
-                  comment: Union[str, list, None] = None) -> dict:
-        """
-        Builds a CDCS-style query based on kwargs values for the record style.
-        
-        Parameters
-        ----------
-        date : str or list
-            The date associated with the record.
-        element : str or list
-            Element(s) to search for in the request.
-        comment : str or list
-            Term(s) to search for in the action's comment field.
-        
-        Returns
-        -------
-        dict
-            The CDCS-style query
-        """
-        mquery = super().cdcsquery(date=date,
-                                   element=element, comment=comment)
-        return mquery
```

### Comparing `potentials-0.3.5/potentials/record/__init__.py` & `potentials-0.3.6/potentials/record/__init__.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/__init__.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/aslist.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/aslist.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/atomic_info.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/atomic_info.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/atomicdata.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/atomicdata.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/numderivative.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/numderivative.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/parse_authors.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/parse_authors.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/screen_input.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/screen_input.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc` & `potentials-0.3.6/potentials/tools/__pycache__/uber_open_rmode.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/atomic_info.py` & `potentials-0.3.6/potentials/tools/atomic_info.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/atomicdata.csv` & `potentials-0.3.6/potentials/tools/atomicdata.csv`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/numderivative.py` & `potentials-0.3.6/potentials/tools/numderivative.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/tools/parse_authors.py` & `potentials-0.3.6/potentials/tools/parse_authors.py`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/Action.xsd` & `potentials-0.3.6/potentials/xsd/Action.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/Citation.xsd` & `potentials-0.3.6/potentials/xsd/Citation.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/Potential.xsd` & `potentials-0.3.6/potentials/xsd/Potential.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/Request.xsd` & `potentials-0.3.6/potentials/xsd/Request.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/artifact.xsd` & `potentials-0.3.6/potentials/xsd/artifact.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/implementation.xsd` & `potentials-0.3.6/potentials/xsd/implementation.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/link.xsd` & `potentials-0.3.6/potentials/xsd/link.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/parameter.xsd` & `potentials-0.3.6/potentials/xsd/parameter.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/potential_LAMMPS.xsd` & `potentials-0.3.6/potentials/xsd/potential_LAMMPS.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsd/potential_LAMMPS_KIM.xsd` & `potentials-0.3.6/potentials/xsd/potential_LAMMPS_KIM.xsd`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/Action.xsl` & `potentials-0.3.6/potentials/xsl/Action.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/Citation.xsl` & `potentials-0.3.6/potentials/xsl/Citation.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/FAQ.xsl` & `potentials-0.3.6/potentials/xsl/FAQ.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/Potential.xsl` & `potentials-0.3.6/potentials/xsl/Potential.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/Request.xsl` & `potentials-0.3.6/potentials/xsl/Request.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/artifact.xsl` & `potentials-0.3.6/potentials/xsl/artifact.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/implementation.xsl` & `potentials-0.3.6/potentials/xsl/implementation.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/link.xsl` & `potentials-0.3.6/potentials/xsl/link.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/parameter.xsl` & `potentials-0.3.6/potentials/xsl/parameter.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/potential_LAMMPS.xsl` & `potentials-0.3.6/potentials/xsl/potential_LAMMPS.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials/xsl/potential_LAMMPS_KIM.xsl` & `potentials-0.3.6/potentials/xsl/potential_LAMMPS_KIM.xsl`

 * *Files identical despite different names*

### Comparing `potentials-0.3.5/potentials.egg-info/PKG-INFO` & `potentials-0.3.6/potentials.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potentials
-Version: 0.3.5
+Version: 0.3.6
 Summary: API database tools for accessing the NIST Interatomic Potentials Repository: explore and download interatomic potentials and computed properties.
 Home-page: https://github.com/usnistgov/potentials
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: atom,atomic,atomistic,molecular dynamics,interatomic potential,force field
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `potentials-0.3.5/potentials.egg-info/SOURCES.txt` & `potentials-0.3.6/potentials.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -90,8 +90,9 @@
 potentials/xsl/__init__.py
 potentials/xsl/artifact.xsl
 potentials/xsl/implementation.xsl
 potentials/xsl/link.xsl
 potentials/xsl/parameter.xsl
 potentials/xsl/potential_LAMMPS.xsl
 potentials/xsl/potential_LAMMPS_KIM.xsl
-potentials/xsl/__pycache__/__init__.cpython-37.pyc
+potentials/xsl/__pycache__/__init__.cpython-37.pyc
+tests/test_settings.py
```

### Comparing `potentials-0.3.5/setup.py` & `potentials-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,14 @@
         'unidecode',
         'numpy',
         'matplotlib',
         'pandas',
         'requests',
         'habanero',
         'bibtexparser',
-        'cdcs>=0.1.5',
         'ipywidgets',
-        'yabadaba'
+        'cdcs',
+        'yabadaba>=0.2.0'
     ],
     include_package_data = True,
     zip_safe = False
 )
```

