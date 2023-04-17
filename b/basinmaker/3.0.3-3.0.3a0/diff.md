# Comparing `tmp/basinmaker-3.0.3.tar.gz` & `tmp/basinmaker-3.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basinmaker-3.0.3.tar", last modified: Mon Apr 10 22:43:29 2023, max compression
+gzip compressed data, was "basinmaker-3.0.3a0.tar", last modified: Mon Apr 17 22:51:00 2023, max compression
```

## Comparing `basinmaker-3.0.3.tar` & `basinmaker-3.0.3a0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:29.030584 basinmaker-3.0.3/
--rw-rw-rw-   0        0        0     8852 2022-07-20 16:58:36.000000 basinmaker-3.0.3/LICENSE
--rw-rw-rw-   0        0        0       22 2022-07-20 16:58:36.000000 basinmaker-3.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5505 2023-04-10 22:43:29.030584 basinmaker-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5014 2022-07-20 16:58:36.000000 basinmaker-3.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.622676 basinmaker-3.0.3/basinmaker/
--rw-rw-rw-   0        0        0        0 2022-07-20 16:58:36.000000 basinmaker-3.0.3/basinmaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.679523 basinmaker-3.0.3/basinmaker/addattributes/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/__init__.py
--rw-rw-rw-   0        0        0    13278 2023-03-04 13:49:59.000000 basinmaker-3.0.3/basinmaker/addattributes/addattributestocatchments.py
--rw-rw-rw-   0        0        0     2915 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/addgaugeattributesqgis.py
--rw-rw-rw-   0        0        0     6980 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/addlakeattributesqgis.py
--rw-rw-rw-   0        0        0    12534 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addattributes/calbkfwidthdepthqgis.py
--rw-rw-rw-   0        0        0    17015 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addattributes/calculatebasicattributesqgis.py
--rw-rw-rw-   0        0        0     3919 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/calfloodmanningnqgis.py
--rw-rw-rw-   0        0        0    20857 2023-03-17 02:53:13.000000 basinmaker-3.0.3/basinmaker/addattributes/createattributestemplatearcgis.py
--rw-rw-rw-   0        0        0     1403 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/createattributestemplateqgis.py
--rw-rw-rw-   0        0        0     5634 2023-03-04 13:50:28.000000 basinmaker-3.0.3/basinmaker/addattributes/exportoutputsqgis.py
--rw-rw-rw-   0        0        0     2844 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/joinpandastoattributesqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.714429 basinmaker-3.0.3/basinmaker/addlakeandobs/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/__init__.py
--rw-rw-rw-   0        0        0    10672 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addlakeandobsintowatershed.py
--rw-rw-rw-   0        0        0     7245 2023-03-27 15:33:34.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addlakesarcgis.py
--rw-rw-rw-   0        0        0    14219 2022-12-12 16:45:02.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addlakesqgis.py
--rw-rw-rw-   0        0        0     3984 2023-02-09 00:34:07.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addobsarcgis.py
--rw-rw-rw-   0        0        0     6701 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addobsqgis.py
--rw-rw-rw-   0        0        0     5535 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/definecatrivarcgis.py
--rw-rw-rw-   0        0        0     6490 2022-12-12 17:39:29.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/definecatrivqgis.py
--rw-rw-rw-   0        0        0     1859 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/definelaketypeqgis.py
--rw-rw-rw-   0        0        0     4943 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/filterlakesqgis.py
--rw-rw-rw-   0        0        0    31231 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/modifyfdr.py
--rw-rw-rw-   0        0        0     3281 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/modifystr.py
--rw-rw-rw-   0        0        0    16301 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/pourpointsqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.733380 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/__init__.py
--rw-rw-rw-   0        0        0     1826 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1141 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1377 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py
--rw-rw-rw-   0        0        0      626 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1194 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py
--rw-rw-rw-   0        0        0    68581 2023-04-10 22:39:55.000000 basinmaker-3.0.3/basinmaker/basinmaker.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.757320 basinmaker-3.0.3/basinmaker/delineationnolake/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/__init__.py
--rw-rw-rw-   0        0        0     8657 2023-01-03 01:23:58.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watdelineationwithoutlake.py
--rw-rw-rw-   0        0        0     3000 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemarcgis.py
--rw-rw-rw-   0        0        0     2079 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemqgis.py
--rw-rw-rw-   0        0        0     3018 2022-11-27 20:34:05.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingfacqgis.py
--rw-rw-rw-   0        0        0     3282 2023-04-02 02:37:44.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrarcgis.py
--rw-rw-rw-   0        0        0     2915 2023-01-03 01:24:50.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrqgis.py
--rw-rw-rw-   0        0        0     2339 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingsubregionddata.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.784244 basinmaker-3.0.3/basinmaker/extent/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/extent/__init__.py
--rw-rw-rw-   0        0        0     7764 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/extent/projectextent.py
--rw-rw-rw-   0        0        0     3492 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/extent/usingdemarcgis.py
--rw-rw-rw-   0        0        0     4841 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/extent/usingdemqgis.py
--rw-rw-rw-   0        0        0     4900 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/extent/usinghybasinplyarcgis.py
--rw-rw-rw-   0        0        0     7193 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/extent/usinghybasinplyqgis.py
--rw-rw-rw-   0        0        0     6027 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/extent/usinginputplyqgis.py
--rw-rw-rw-   0        0        0     6861 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/extent/usingoutletpointqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.808179 basinmaker-3.0.3/basinmaker/func/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.837102 basinmaker-3.0.3/basinmaker/func/__pycache__/
--rw-rw-rw-   0        0        0      164 2022-08-17 20:03:20.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    18510 2023-02-27 03:41:01.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/arcgis.cpython-39.pyc
--rw-rw-rw-   0        0        0     6084 2022-08-17 20:05:59.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/fgdal.cpython-39.pyc
--rw-rw-rw-   0        0        0    15904 2022-08-18 02:30:26.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/grassgis.cpython-39.pyc
--rw-rw-rw-   0        0        0    47805 2023-04-01 13:38:31.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/pdtable.cpython-39.pyc
--rw-rw-rw-   0        0        0    10361 2022-11-27 20:15:59.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/purepy.cpython-39.pyc
--rw-rw-rw-   0        0        0    26797 2022-08-18 02:30:27.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/qgis.cpython-39.pyc
--rw-rw-rw-   0        0        0    12224 2022-08-18 02:30:32.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/rarray.cpython-39.pyc
--rw-rw-rw-   0        0        0    35090 2023-02-27 03:39:45.000000 basinmaker-3.0.3/basinmaker/func/arcgis.py
--rw-rw-rw-   0        0        0     9448 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/fgdal.py
--rw-rw-rw-   0        0        0    27465 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/grassgis.py
--rw-rw-rw-   0        0        0   139946 2023-04-01 13:38:19.000000 basinmaker-3.0.3/basinmaker/func/pdtable.py
--rw-rw-rw-   0        0        0    17567 2023-04-10 21:29:09.000000 basinmaker-3.0.3/basinmaker/func/purepy.py
--rw-rw-rw-   0        0        0    42623 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/qgis.py
--rw-rw-rw-   0        0        0    25878 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/rarray.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.844084 basinmaker-3.0.3/basinmaker/hymodin/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/hymodin/__init__.py
--rw-rw-rw-   0        0        0    92339 2022-11-17 01:32:01.000000 basinmaker-3.0.3/basinmaker/hymodin/raveninput.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.926861 basinmaker-3.0.3/basinmaker/postprocessing/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/__init__.py
--rw-rw-rw-   0        0        0    10250 2023-04-01 13:38:13.000000 basinmaker-3.0.3/basinmaker/postprocessing/assigninterestsites.py
--rw-rw-rw-   0        0        0     6500 2023-03-04 13:51:54.000000 basinmaker-3.0.3/basinmaker/postprocessing/combine.py
--rw-rw-rw-   0        0        0     6538 2023-03-04 13:52:08.000000 basinmaker-3.0.3/basinmaker/postprocessing/combinearcgis.py
--rw-rw-rw-   0        0        0     5693 2023-03-04 13:52:19.000000 basinmaker-3.0.3/basinmaker/postprocessing/combinepurepy.py
--rw-rw-rw-   0        0        0     7412 2023-04-01 14:30:36.000000 basinmaker-3.0.3/basinmaker/postprocessing/downloadpd.py
--rw-rw-rw-   0        0        0     2836 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/downloadpdptspurepy.py
--rw-rw-rw-   0        0        0    21586 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/gridweight.py
--rw-rw-rw-   0        0        0     3482 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/gridweightarcgis.py
--rw-rw-rw-   0        0        0    59494 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/hru.py
--rw-rw-rw-   0        0        0    40585 2022-09-07 02:20:09.000000 basinmaker-3.0.3/basinmaker/postprocessing/hruarcgis.py
--rw-rw-rw-   0        0        0    38578 2022-11-27 18:54:39.000000 basinmaker-3.0.3/basinmaker/postprocessing/hrupurepy.py
--rw-rw-rw-   0        0        0    10971 2023-03-04 13:53:00.000000 basinmaker-3.0.3/basinmaker/postprocessing/increaseda.py
--rw-rw-rw-   0        0        0     9072 2023-03-04 14:14:28.000000 basinmaker-3.0.3/basinmaker/postprocessing/increasedaarcgis.py
--rw-rw-rw-   0        0        0     8693 2023-03-04 13:53:46.000000 basinmaker-3.0.3/basinmaker/postprocessing/increasedapurepy.py
--rw-rw-rw-   0        0        0     3303 2022-09-11 18:50:03.000000 basinmaker-3.0.3/basinmaker/postprocessing/inversetopology.py
--rw-rw-rw-   0        0        0     8035 2023-04-01 13:38:19.000000 basinmaker-3.0.3/basinmaker/postprocessing/plotleaflet.py
--rw-rw-rw-   0        0        0    15290 2023-02-05 00:48:12.000000 basinmaker-3.0.3/basinmaker/postprocessing/postprocessingfunctions.py
--rw-rw-rw-   0        0        0    10902 2023-03-04 14:03:13.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectlake.py
--rw-rw-rw-   0        0        0     8912 2023-03-04 14:08:34.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectlakearcgis.py
--rw-rw-rw-   0        0        0     8114 2023-03-04 14:09:00.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectlakepurepy.py
--rw-rw-rw-   0        0        0    11957 2023-03-04 14:09:12.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectprod.py
--rw-rw-rw-   0        0        0    11211 2023-03-04 14:09:22.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectprodarcgis.py
--rw-rw-rw-   0        0        0     7266 2023-04-01 13:38:19.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectprodpurepy.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.958776 basinmaker-3.0.3/basinmaker/preprocessing/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1180 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preinputpolygonqgis.py
--rw-rw-rw-   0        0        0     3446 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preprocessinglakeply.py
--rw-rw-rw-   0        0        0     1363 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preprocessingobs.py
--rw-rw-rw-   0        0        0     2665 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preprocessrasterqgis.py
--rw-rw-rw-   0        0        0     4187 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py
--rw-rw-rw-   0        0        0     3610 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.973736 basinmaker-3.0.3/basinmaker/subreg/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/subreg/__init__.py
--rw-rw-rw-   0        0        0     3612 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/subreg/defsubreg.py
--rw-rw-rw-   0        0        0    38989 2022-11-23 01:59:53.000000 basinmaker-3.0.3/basinmaker/subreg/generatesubregionqgis.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.980718 basinmaker-3.0.3/basinmaker/utilities/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/utilities/__init__.py
--rw-rw-rw-   0        0        0     7554 2022-11-27 20:24:39.000000 basinmaker-3.0.3/basinmaker/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.649610 basinmaker-3.0.3/basinmaker.egg-info/
--rw-rw-rw-   0        0        0     5505 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5345 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-20 16:58:37.000000 basinmaker-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 22:43:29.033578 basinmaker-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-01-22 00:27:34.000000 basinmaker-3.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:43:29.027593 basinmaker-3.0.3/tests/
--rw-rw-rw-   0        0        0     5251 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py
--rw-rw-rw-   0        0        0     6085 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_Generateinputdata.py
--rw-rw-rw-   0        0        0     6187 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_Generatmaskregion.py
--rw-rw-rw-   0        0        0     5729 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py
--rw-rw-rw-   0        0        0     2298 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py
--rw-rw-rw-   0        0        0     3378 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py
--rw-rw-rw-   0        0        0     3474 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py
--rw-rw-rw-   0        0        0     1966 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py
--rw-rw-rw-   0        0        0     4695 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_SelectLakes.py
--rw-rw-rw-   0        0        0     7034 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py
--rw-rw-rw-   0        0        0     5916 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py
--rw-rw-rw-   0        0        0     6998 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_WatershedDiscretizationToolset.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.040775 basinmaker-3.0.3a0/
+-rw-rw-rw-   0        0        0     8852 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/LICENSE
+-rw-rw-rw-   0        0        0       22 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5507 2023-04-17 22:51:00.041781 basinmaker-3.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5014 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.756533 basinmaker-3.0.3a0/basinmaker/
+-rw-rw-rw-   0        0        0        0 2022-07-20 16:58:36.000000 basinmaker-3.0.3a0/basinmaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.802410 basinmaker-3.0.3a0/basinmaker/addattributes/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/__init__.py
+-rw-rw-rw-   0        0        0    13278 2023-03-04 13:49:59.000000 basinmaker-3.0.3a0/basinmaker/addattributes/addattributestocatchments.py
+-rw-rw-rw-   0        0        0     2915 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/addgaugeattributesqgis.py
+-rw-rw-rw-   0        0        0     6980 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/addlakeattributesqgis.py
+-rw-rw-rw-   0        0        0    12534 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addattributes/calbkfwidthdepthqgis.py
+-rw-rw-rw-   0        0        0    17015 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addattributes/calculatebasicattributesqgis.py
+-rw-rw-rw-   0        0        0     3919 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/calfloodmanningnqgis.py
+-rw-rw-rw-   0        0        0    21271 2023-04-17 21:45:20.000000 basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplatearcgis.py
+-rw-rw-rw-   0        0        0     1403 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplateqgis.py
+-rw-rw-rw-   0        0        0     5634 2023-03-04 13:50:28.000000 basinmaker-3.0.3a0/basinmaker/addattributes/exportoutputsqgis.py
+-rw-rw-rw-   0        0        0     2844 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addattributes/joinpandastoattributesqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.832331 basinmaker-3.0.3a0/basinmaker/addlakeandobs/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/__init__.py
+-rw-rw-rw-   0        0        0    10672 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakeandobsintowatershed.py
+-rw-rw-rw-   0        0        0     7245 2023-03-27 15:33:34.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesarcgis.py
+-rw-rw-rw-   0        0        0    14219 2022-12-12 16:45:02.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesqgis.py
+-rw-rw-rw-   0        0        0     3984 2023-02-09 00:34:07.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsarcgis.py
+-rw-rw-rw-   0        0        0     6701 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsqgis.py
+-rw-rw-rw-   0        0        0     5535 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivarcgis.py
+-rw-rw-rw-   0        0        0     6490 2022-12-12 17:39:29.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivqgis.py
+-rw-rw-rw-   0        0        0     1859 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/definelaketypeqgis.py
+-rw-rw-rw-   0        0        0     4943 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/filterlakesqgis.py
+-rw-rw-rw-   0        0        0    31231 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifyfdr.py
+-rw-rw-rw-   0        0        0     3281 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifystr.py
+-rw-rw-rw-   0        0        0    16301 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/addlakeandobs/pourpointsqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.845295 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/__init__.py
+-rw-rw-rw-   0        0        0     1826 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1141 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1377 2022-08-17 20:01:16.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0      626 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1194 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0    68582 2023-04-17 22:26:13.000000 basinmaker-3.0.3a0/basinmaker/basinmaker.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.864244 basinmaker-3.0.3a0/basinmaker/delineationnolake/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/__init__.py
+-rw-rw-rw-   0        0        0     8657 2023-01-03 01:23:58.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watdelineationwithoutlake.py
+-rw-rw-rw-   0        0        0     3000 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemarcgis.py
+-rw-rw-rw-   0        0        0     2079 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemqgis.py
+-rw-rw-rw-   0        0        0     3018 2022-11-27 20:34:05.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfacqgis.py
+-rw-rw-rw-   0        0        0     3282 2023-04-02 02:37:44.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrarcgis.py
+-rw-rw-rw-   0        0        0     2915 2023-01-03 01:24:50.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrqgis.py
+-rw-rw-rw-   0        0        0     2339 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingsubregionddata.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.880202 basinmaker-3.0.3a0/basinmaker/extent/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/extent/__init__.py
+-rw-rw-rw-   0        0        0     7764 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/extent/projectextent.py
+-rw-rw-rw-   0        0        0     3492 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/extent/usingdemarcgis.py
+-rw-rw-rw-   0        0        0     4841 2022-12-18 02:16:17.000000 basinmaker-3.0.3a0/basinmaker/extent/usingdemqgis.py
+-rw-rw-rw-   0        0        0     4900 2022-08-17 20:01:17.000000 basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyarcgis.py
+-rw-rw-rw-   0        0        0     7193 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyqgis.py
+-rw-rw-rw-   0        0        0     6027 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/extent/usinginputplyqgis.py
+-rw-rw-rw-   0        0        0     6861 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/extent/usingoutletpointqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.901145 basinmaker-3.0.3a0/basinmaker/func/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.925083 basinmaker-3.0.3a0/basinmaker/func/__pycache__/
+-rw-rw-rw-   0        0        0      164 2022-08-17 20:03:20.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    18510 2023-02-27 03:41:01.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/arcgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6084 2022-08-17 20:05:59.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/fgdal.cpython-39.pyc
+-rw-rw-rw-   0        0        0    15904 2022-08-18 02:30:26.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/grassgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    47805 2023-04-01 13:38:31.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/pdtable.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10323 2023-04-16 18:06:34.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/purepy.cpython-39.pyc
+-rw-rw-rw-   0        0        0    26797 2022-08-18 02:30:27.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/qgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12224 2022-08-18 02:30:32.000000 basinmaker-3.0.3a0/basinmaker/func/__pycache__/rarray.cpython-39.pyc
+-rw-rw-rw-   0        0        0    35090 2023-02-27 03:39:45.000000 basinmaker-3.0.3a0/basinmaker/func/arcgis.py
+-rw-rw-rw-   0        0        0     9448 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/fgdal.py
+-rw-rw-rw-   0        0        0    27465 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/grassgis.py
+-rw-rw-rw-   0        0        0   139946 2023-04-01 13:38:19.000000 basinmaker-3.0.3a0/basinmaker/func/pdtable.py
+-rw-rw-rw-   0        0        0    17567 2023-04-10 21:29:09.000000 basinmaker-3.0.3a0/basinmaker/func/purepy.py
+-rw-rw-rw-   0        0        0    42623 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/qgis.py
+-rw-rw-rw-   0        0        0    25878 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/func/rarray.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.930074 basinmaker-3.0.3a0/basinmaker/hymodin/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/hymodin/__init__.py
+-rw-rw-rw-   0        0        0    92339 2022-11-17 01:32:01.000000 basinmaker-3.0.3a0/basinmaker/hymodin/raveninput.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.983925 basinmaker-3.0.3a0/basinmaker/postprocessing/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0    10250 2023-04-01 13:38:13.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/assigninterestsites.py
+-rw-rw-rw-   0        0        0     6500 2023-03-04 13:51:54.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/combine.py
+-rw-rw-rw-   0        0        0     6538 2023-03-04 13:52:08.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/combinearcgis.py
+-rw-rw-rw-   0        0        0     5693 2023-03-04 13:52:19.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/combinepurepy.py
+-rw-rw-rw-   0        0        0     7412 2023-04-01 14:30:36.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpd.py
+-rw-rw-rw-   0        0        0     2836 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpdptspurepy.py
+-rw-rw-rw-   0        0        0    21586 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/gridweight.py
+-rw-rw-rw-   0        0        0     3482 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/gridweightarcgis.py
+-rw-rw-rw-   0        0        0    59494 2022-08-17 20:01:18.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/hru.py
+-rw-rw-rw-   0        0        0    40585 2022-09-07 02:20:09.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/hruarcgis.py
+-rw-rw-rw-   0        0        0    38578 2022-11-27 18:54:39.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/hrupurepy.py
+-rw-rw-rw-   0        0        0    10971 2023-03-04 13:53:00.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/increaseda.py
+-rw-rw-rw-   0        0        0     9072 2023-03-04 14:14:28.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/increasedaarcgis.py
+-rw-rw-rw-   0        0        0     8693 2023-03-04 13:53:46.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/increasedapurepy.py
+-rw-rw-rw-   0        0        0     3303 2022-09-11 18:50:03.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/inversetopology.py
+-rw-rw-rw-   0        0        0     8035 2023-04-01 13:38:19.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/plotleaflet.py
+-rw-rw-rw-   0        0        0    15290 2023-02-05 00:48:12.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/postprocessingfunctions.py
+-rw-rw-rw-   0        0        0    10902 2023-03-04 14:03:13.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectlake.py
+-rw-rw-rw-   0        0        0     8912 2023-03-04 14:08:34.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectlakearcgis.py
+-rw-rw-rw-   0        0        0     8114 2023-03-04 14:09:00.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectlakepurepy.py
+-rw-rw-rw-   0        0        0    11957 2023-03-04 14:09:12.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectprod.py
+-rw-rw-rw-   0        0        0    11211 2023-03-04 14:09:22.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodarcgis.py
+-rw-rw-rw-   0        0        0     7266 2023-04-01 13:38:19.000000 basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodpurepy.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.997888 basinmaker-3.0.3a0/basinmaker/preprocessing/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     1180 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preinputpolygonqgis.py
+-rw-rw-rw-   0        0        0     3446 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessinglakeply.py
+-rw-rw-rw-   0        0        0     1363 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessingobs.py
+-rw-rw-rw-   0        0        0     2665 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessrasterqgis.py
+-rw-rw-rw-   0        0        0     4187 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py
+-rw-rw-rw-   0        0        0     3610 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.002875 basinmaker-3.0.3a0/basinmaker/subreg/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/subreg/__init__.py
+-rw-rw-rw-   0        0        0     3612 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/subreg/defsubreg.py
+-rw-rw-rw-   0        0        0    38989 2022-11-23 01:59:53.000000 basinmaker-3.0.3a0/basinmaker/subreg/generatesubregionqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.007861 basinmaker-3.0.3a0/basinmaker/utilities/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3a0/basinmaker/utilities/__init__.py
+-rw-rw-rw-   0        0        0     7554 2022-11-27 20:24:39.000000 basinmaker-3.0.3a0/basinmaker/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:50:59.773491 basinmaker-3.0.3a0/basinmaker.egg-info/
+-rw-rw-rw-   0        0        0     5507 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5345 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 22:50:59.000000 basinmaker-3.0.3a0/basinmaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:51:00.044761 basinmaker-3.0.3a0/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-04-17 22:49:07.000000 basinmaker-3.0.3a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:51:00.038778 basinmaker-3.0.3a0/tests/
+-rw-rw-rw-   0        0        0     5251 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py
+-rw-rw-rw-   0        0        0     6085 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_Generateinputdata.py
+-rw-rw-rw-   0        0        0     6187 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_Generatmaskregion.py
+-rw-rw-rw-   0        0        0     5729 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py
+-rw-rw-rw-   0        0        0     2298 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py
+-rw-rw-rw-   0        0        0     3378 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py
+-rw-rw-rw-   0        0        0     3474 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py
+-rw-rw-rw-   0        0        0     1966 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py
+-rw-rw-rw-   0        0        0     4695 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_SelectLakes.py
+-rw-rw-rw-   0        0        0     7034 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py
+-rw-rw-rw-   0        0        0     5916 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py
+-rw-rw-rw-   0        0        0     6998 2022-07-20 16:58:37.000000 basinmaker-3.0.3a0/tests/test_RoutingTool_WatershedDiscretizationToolset.py
```

### Comparing `basinmaker-3.0.3/LICENSE` & `basinmaker-3.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/PKG-INFO` & `basinmaker-3.0.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basinmaker
-Version: 3.0.3
+Version: 3.0.3a0
 Summary: An automated GIS toolbox for watershed delineation with lakes
 Home-page: https://github.com/dustming/basinmaker
 Author: basinmaker development team
 Author-email: m43han@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basinmaker-3.0.3/README.md` & `basinmaker-3.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/addattributestocatchments.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/addattributestocatchments.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/addgaugeattributesqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/addgaugeattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/addlakeattributesqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/addlakeattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/calbkfwidthdepthqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/calbkfwidthdepthqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/calculatebasicattributesqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/calculatebasicattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/calfloodmanningnqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/calfloodmanningnqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/createattributestemplatearcgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplatearcgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,17 +332,25 @@
     riv_line = riv_line.merge(attri_table,on='SubId',how='left')
     riv_line = riv_line.fillna(-1.2345)
     riv_line['Obs_NM'] = riv_line['Obs_NM'].astype('str')
     riv_line['SRC_obs'] = riv_line['SRC_obs'].astype('str')
     riv_line = riv_line.drop_duplicates(subset=['SubId'], keep='first')
     riv_line.spatial.to_featureclass(location=os.path.join(output_folder,river_without_merging_lakes+"_v1-0"),overwrite=True,sanitize_columns=False)
 
+    
     arcpy.FeatureClassToFeatureClass_conversion("sl_connected_lake_v", output_folder,"sl_connected_lake_v1-0.shp")
     arcpy.FeatureClassToFeatureClass_conversion("sl_nonconnect_lake_v",output_folder,"sl_non_connected_lake_v1-0.shp")
 
+    arcpy.DeleteField_management(os.path.join(output_folder,"sl_connected_lake_v1-0.shp"),
+        ["area_ratio", "Id","ORIG_FID", "BUFF_DIST","newarea0","newarea1","Shape_Leng","Shape_Area"]
+    )
+    arcpy.DeleteField_management(os.path.join(output_folder,"sl_non_connected_lake_v1-0.shp"),
+        ["area_ratio", "Id","ORIG_FID", "BUFF_DIST","newarea0","newarea1","Shape_Leng","Shape_Area"]
+    )
+
     obs_v = pd.DataFrame.spatial.from_featureclass("obs_v")
     obs_v['obsid'] = obs_v['grid_code']
     obs_v2 = pd.DataFrame.spatial.from_featureclass("obs_clip")
     obs_v2['obsid'] = obs_v2['Obs_ID']
     obs_v_missing = obs_v2[~obs_v2['obsid'].isin(final_pourpoints['obsid'].values)].copy(deep=True)
 
     final_pourpoints_2 = final_pourpoints[['obsid','SubId']]
```

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/createattributestemplateqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/createattributestemplateqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/exportoutputsqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/exportoutputsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addattributes/joinpandastoattributesqgis.py` & `basinmaker-3.0.3a0/basinmaker/addattributes/joinpandastoattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/addlakeandobsintowatershed.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakeandobsintowatershed.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/addlakesarcgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/addlakesqgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addlakesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/addobsarcgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/addobsqgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/addobsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/definecatrivarcgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/definecatrivqgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/definecatrivqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/definelaketypeqgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/definelaketypeqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/filterlakesqgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/filterlakesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/modifyfdr.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifyfdr.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/modifystr.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/modifystr.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/addlakeandobs/pourpointsqgis.py` & `basinmaker-3.0.3a0/basinmaker/addlakeandobs/pourpointsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py` & `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py` & `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py` & `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py` & `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py` & `basinmaker-3.0.3a0/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/basinmaker.py` & `basinmaker-3.0.3a0/basinmaker/basinmaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1073,16 +1073,16 @@
         path_sub_reg_lake_bd_r="#",
         search_radius=100,
         mode="#",
         max_memroy=1024 * 4,
         gis_platform="qgis",
     ):
         """ Update the subbasin delineation result by adding lake inflow and
-        outflow points and observation gauges as a new subbasin outlets. The output
-        is not the final delineation result. because:
+        outflow points and observation gauges as a new subbasin outlets. 
+        The output is not the final delineation result. because:
 
         | 1) Hydrologcial related attributes for each subbasin are not calcuated yet.
         | 2) Some lakes may cover several subbasins. The output needs to be finalized
              by combing those subbasins with the same lake as one subbasin only.
 
 
         Parameters
```

### Comparing `basinmaker-3.0.3/basinmaker/delineationnolake/watdelineationwithoutlake.py` & `basinmaker-3.0.3a0/basinmaker/delineationnolake/watdelineationwithoutlake.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemarcgis.py` & `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemqgis.py` & `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingdemqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/delineationnolake/watusingfacqgis.py` & `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfacqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrarcgis.py` & `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrqgis.py` & `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingfdrqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/delineationnolake/watusingsubregionddata.py` & `basinmaker-3.0.3a0/basinmaker/delineationnolake/watusingsubregionddata.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/extent/projectextent.py` & `basinmaker-3.0.3a0/basinmaker/extent/projectextent.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/extent/usingdemarcgis.py` & `basinmaker-3.0.3a0/basinmaker/extent/usingdemarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/extent/usingdemqgis.py` & `basinmaker-3.0.3a0/basinmaker/extent/usingdemqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/extent/usinghybasinplyarcgis.py` & `basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/extent/usinghybasinplyqgis.py` & `basinmaker-3.0.3a0/basinmaker/extent/usinghybasinplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/extent/usinginputplyqgis.py` & `basinmaker-3.0.3a0/basinmaker/extent/usinginputplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/extent/usingoutletpointqgis.py` & `basinmaker-3.0.3a0/basinmaker/extent/usingoutletpointqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/__pycache__/arcgis.cpython-39.pyc` & `basinmaker-3.0.3a0/basinmaker/func/__pycache__/arcgis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/__pycache__/fgdal.cpython-39.pyc` & `basinmaker-3.0.3a0/basinmaker/func/__pycache__/fgdal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/__pycache__/grassgis.cpython-39.pyc` & `basinmaker-3.0.3a0/basinmaker/func/__pycache__/grassgis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/__pycache__/pdtable.cpython-39.pyc` & `basinmaker-3.0.3a0/basinmaker/func/__pycache__/pdtable.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/__pycache__/purepy.cpython-39.pyc` & `basinmaker-3.0.3a0/basinmaker/func/__pycache__/purepy.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Nov 27 18:54:35 2022 UTC, .py size: 17590 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6bb2 8363 b644 0000  a.......k..c.D..
+00000000: 610d 0d0a 0000 0000 a57f 3464 9f44 0000  a.........4d.D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6401 6c06 5a06 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c0a 5a0a 6400 6403 6c0b 6d0c 5a0c  d.l.Z.d.d.l.m.Z.
@@ -204,31 +204,31 @@
 00000cb0: 6f5f 6372 73da 0765 7870 6c6f 6465 da04  o_crs..explode..
 00000cc0: 636c 6970 da15 636c 6561 6e5f 6765 6f6d  clip..clean_geom
 00000cd0: 6574 7279 5f70 7572 6570 79da 0763 6f6c  etry_purepy..col
 00000ce0: 756d 6e73 da05 7072 696e 74da 0373 7973  umns..print..sys
 00000cf0: da04 6578 6974 721f 0000 00da 0f64 726f  ..exitr......dro
 00000d00: 705f 6475 706c 6963 6174 6573 7213 0000  p_duplicatesr...
 00000d10: 00da 056d 6572 6765 290d da0a 6c61 7965  ...merge)...laye
-00000d20: 725f 7061 7468 5a09 436c 6173 735f 436f  r_pathZ.Class_Co
+00000d20: 725f 7061 7468 da09 436c 6173 735f 436f  r_path..Class_Co
 00000d30: 6cda 0a74 656d 7066 6f6c 6465 72da 0a6d  l..tempfolder..m
-00000d40: 6173 6b5f 6c61 7965 725a 0c43 6c61 7373  ask_layerZ.Class
-00000d50: 5f4e 4d5f 436f 6c5a 0a69 6e66 6f5f 7461  _NM_ColZ.info_ta
+00000d40: 6173 6b5f 6c61 7965 72da 0c43 6c61 7373  ask_layer..Class
+00000d50: 5f4e 4d5f 436f 6cda 0a69 6e66 6f5f 7461  _NM_Col..info_ta
 00000d60: 626c 655a 076e 6577 5f63 7273 da04 6461  bleZ.new_crs..da
 00000d70: 7461 5a09 7072 6f6a 6563 7465 64da 0763  taZ.projected..c
 00000d80: 6c69 7070 6564 da07 636c 6561 6e65 645a  lipped..cleanedZ
 00000d90: 0f69 6e66 6f5f 7461 626c 655f 636f 7079  .info_table_copy
 00000da0: 5a10 696e 666f 5f74 6162 6c65 5f63 6f70  Z.info_table_cop
 00000db0: 7932 720a 0000 0072 0a00 0000 720e 0000  y2r....r....r...
 00000dc0: 00da 2c52 6570 726f 6a5f 436c 6970 5f44  ..,Reproj_Clip_D
 00000dd0: 6973 736f 6c76 655f 5369 6d70 6c69 6679  issolve_Simplify
 00000de0: 5f50 6f6c 7967 6f6e 5f70 7572 6570 7935  _Polygon_purepy5
 00000df0: 0000 0073 3000 0000 0027 0601 0a02 0a01  ...s0....'......
 00000e00: 0c01 0a03 0a01 0a01 0a01 0a01 0801 0a01  ................
 00000e10: 0a01 0801 0a01 0a01 0802 0c01 1201 0c01  ................
-00000e20: 0c01 1a02 1201 0c06 7241 0000 00da 0553  ........rA.....S
+00000e20: 0c01 1a02 1201 0c06 7244 0000 00da 0553  ........rD.....S
 00000e30: 7562 4964 6307 0000 0000 0000 0000 0000  ubIdc...........
 00000e40: 0014 0000 0008 0000 0043 0000 0073 2604  .........C...s&.
 00000e50: 0000 6700 6401 a201 7d07 6402 7c00 6a00  ..g.d...}.d.|.j.
 00000e60: 7600 7218 6403 7d08 6e04 6404 7d08 7401  v.r.d.}.n.d.}.t.
 00000e70: a002 7c08 a101 7d09 7403 7404 6a05 a006  ..|...}.t.t.j...
 00000e80: 7c02 6405 a102 6406 8302 8f1c 7d0a 7c0a  |.d...d.....}.|.
 00000e90: a007 7c09 6a08 a101 0100 5700 6400 0400  ..|.j.....W.d...
@@ -295,72 +295,72 @@
 00001260: 7404 6a05 a006 7c02 6420 a102 a101 0100  t.j...|.d ......
 00001270: 7c00 5300 6400 5300 2922 4e29 10da 0753  |.S.d.S.)"N)...S
 00001280: 7562 4964 5f31 da02 4964 da07 6e73 7562  ubId_1..Id..nsub
 00001290: 6964 32da 066e 7375 6269 64da 0a6e 646f  id2..nsubid..ndo
 000012a0: 776e 7375 6269 64da 094f 6c64 5f53 7562  wnsubid..Old_Sub
 000012b0: 4964 da0a 4f6c 645f 446f 7753 7562 da0a  Id..Old_DowSub..
 000012c0: 4a6f 696e 5f43 6f75 6e74 da0a 5441 5247  Join_Count..TARG
-000012d0: 4554 5f46 4944 7244 0000 00da 0a53 7562  ET_FIDrD.....Sub
+000012d0: 4554 5f46 4944 7247 0000 00da 0a53 7562  ET_FIDrG.....Sub
 000012e0: 4944 5f4f 6c64 72da 0a48 5255 5f49 445f  ID_Oldr..HRU_ID_
 000012f0: 4e5f 31da 0a48 5255 5f49 445f 4e5f 32da  N_1..HRU_ID_N_2.
 00001300: 0766 6163 7465 7273 da0c 4f6c 645f 446f  .facters..Old_Do
-00001310: 7753 7562 4964 5a07 5375 6249 6474 32da  wSubIdZ.SubIdt2.
+00001310: 7753 7562 4964 5a07 5375 6249 6474 325a  wSubIdZ.SubIdt2Z
 00001320: 0844 415f 4368 6e5f 4c7a 4168 7474 7073  .DA_Chn_LzAhttps
 00001330: 3a2f 2f67 6974 6875 622e 636f 6d2f 6475  ://github.com/du
 00001340: 7374 6d69 6e67 2f52 6f75 7469 6e67 546f  stming/RoutingTo
 00001350: 6f6c 2f77 696b 692f 4669 6c65 732f 5245  ol/wiki/Files/RE
 00001360: 4144 4d45 5f4f 4948 2e70 6466 7a40 6874  ADME_OIH.pdfz@ht
 00001370: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00001380: 2f64 7573 746d 696e 672f 526f 7574 696e  /dustming/Routin
 00001390: 6754 6f6f 6c2f 7769 6b69 2f46 696c 6573  gTool/wiki/Files
 000013a0: 2f52 4541 444d 455f 4e41 2e70 6466 7a0a  /README_NA.pdfz.
 000013b0: 5245 4144 4d45 2e70 6466 da02 7762 7226  README.pdf..wbr&
-000013c0: 0000 0072 4200 0000 7248 0000 00da 0867  ...rB...rH.....g
+000013c0: 0000 0072 4500 0000 724b 0000 00da 0867  ...rE...rK.....g
 000013d0: 656f 6d65 7472 79a9 0172 3500 0000 5472  eometry..r5...Tr
 000013e0: 1a00 0000 da04 6c65 6674 2902 722d 0000  ......left).r-..
 000013f0: 0072 2c00 0000 da05 6669 7273 7446 a903  .r,.....firstF..
 00001400: da02 6279 da07 6167 6766 756e 63da 0861  ..by..aggfunc..a
-00001410: 735f 696e 6465 78da 0a63 656e 7472 6f69  s_index..centroi
-00001420: 645f 78da 0a63 656e 7472 6f69 645f 79da  d_x..centroid_y.
-00001430: 084c 616b 655f 4361 74e9 0200 0000 da08  .Lake_Cat.......
+00001410: 735f 696e 6465 785a 0a63 656e 7472 6f69  s_indexZ.centroi
+00001420: 645f 785a 0a63 656e 7472 6f69 645f 79da  d_xZ.centroid_y.
+00001430: 084c 616b 655f 4361 74e9 0200 0000 5a08  .Lake_Cat.....Z.
 00001440: 446f 7753 7562 4964 7201 0000 0067 8d97  DowSubIdr....g..
-00001450: 6e12 83c0 f3bf da08 5269 7653 6c6f 7065  n.......RivSlope
-00001460: da09 5269 764c 656e 6774 68da 0846 6c6f  ..RivLength..Flo
-00001470: 6f64 505f 6eda 0443 685f 6eda 074d 6178  odP_n..Ch_n..Max
-00001480: 5f44 454d da07 4d69 6e5f 4445 4d7a 0b6f  _DEM..Min_DEMz.o
-00001490: 7574 6c69 6e65 2e73 6870 290f da05 5348  utline.shp)...SH
-000014a0: 4150 4572 4300 0000 7244 0000 0072 4500  APErC...rD...rE.
-000014b0: 0000 7246 0000 0072 4700 0000 7249 0000  ..rF...rG...rI..
-000014c0: 0072 4a00 0000 724b 0000 0072 4400 0000  .rJ...rK...rD...
-000014d0: 724c 0000 0072 4d00 0000 724e 0000 0072  rL...rM...rN...r
-000014e0: 4f00 0000 7250 0000 0029 1b72 3500 0000  O...rP...).r5...
+00001450: 6e12 83c0 f3bf 5a08 5269 7653 6c6f 7065  n.....Z.RivSlope
+00001460: 5a09 5269 764c 656e 6774 685a 0846 6c6f  Z.RivLengthZ.Flo
+00001470: 6f64 505f 6e5a 0443 685f 6e5a 074d 6178  odP_nZ.Ch_nZ.Max
+00001480: 5f44 454d 5a07 4d69 6e5f 4445 4d7a 0b6f  _DEMZ.Min_DEMz.o
+00001490: 7574 6c69 6e65 2e73 6870 290f 5a05 5348  utline.shp).Z.SH
+000014a0: 4150 4572 4600 0000 7247 0000 0072 4800  APErF...rG...rH.
+000014b0: 0000 7249 0000 0072 4a00 0000 724c 0000  ..rI...rJ...rL..
+000014c0: 0072 4d00 0000 724e 0000 0072 4700 0000  .rM...rN...rG...
+000014d0: 724f 0000 0072 5000 0000 7251 0000 0072  rO...rP...rQ...r
+000014e0: 5200 0000 7253 0000 0029 1b72 3500 0000  R...rS...).r5...
 000014f0: da08 7265 7175 6573 7473 da03 6765 74da  ..requests..get.
 00001500: 046f 7065 6eda 026f 73da 0470 6174 68da  .open..os..path.
 00001510: 046a 6f69 6eda 0577 7269 7465 da07 636f  .join..write..co
 00001520: 6e74 656e 7472 2f00 0000 7230 0000 00da  ntentr/...r0....
 00001530: 0464 726f 7072 1f00 0000 7213 0000 0072  .dropr....r....r
 00001540: 3a00 0000 da08 6469 7373 6f6c 7665 da15  :.....dissolve..
 00001550: 6164 645f 6365 6e74 726f 6964 5f69 6e5f  add_centroid_in_
 00001560: 7767 7338 34da 0676 616c 7565 7372 2200  wgs84..valuesr".
-00001570: 0000 7242 0000 0072 2100 0000 7220 0000  ..rB...r!...r ..
+00001570: 0000 7245 0000 0072 2100 0000 7220 0000  ..rE...r!...r ..
 00001580: 00da 0774 6f5f 6669 6c65 da03 6c6f 63da  ...to_file..loc.
 00001590: 1963 7265 6174 655f 7761 7465 7273 6865  .create_watershe
 000015a0: 645f 626f 756e 6461 7279 da15 6372 6561  d_boundary..crea
 000015b0: 7465 5f67 656f 5f6a 6173 6f6e 5f66 696c  te_geo_jason_fil
 000015c0: 65da 0569 6e64 6578 2914 da0e 6d61 706f  e..index)...mapo
-000015d0: 6c64 6e65 775f 696e 666f 723c 0000 00da  ldnew_infor<....
+000015d0: 6c64 6e65 775f 696e 666f 723d 0000 00da  ldnew_infor=....
 000015e0: 0c4f 7574 7075 7446 6f6c 6465 72da 0863  .OutputFolder..c
 000015f0: 6174 5f6e 616d 65da 0872 6976 5f6e 616d  at_name..riv_nam
 00001600: 65da 0e50 6174 685f 6669 6e61 6c5f 7269  e..Path_final_ri
-00001610: 765a 0c64 6973 5f63 6f6c 5f6e 616d 655a  vZ.dis_col_nameZ
+00001610: 76da 0c64 6973 5f63 6f6c 5f6e 616d 655a  v..dis_col_nameZ
 00001620: 124e 4545 445f 544f 5f52 454d 4f56 455f  .NEED_TO_REMOVE_
 00001630: 4944 53da 0375 726c da08 7265 7370 6f6e  IDS..url..respon
 00001640: 7365 da01 665a 0672 6976 5f70 645a 0663  se..fZ.riv_pdZ.c
 00001650: 6174 5f70 645a 0963 6174 5f63 5f78 5f79  at_pdZ.cat_c_x_y
-00001660: da19 7269 765f 7064 5f6e 6e63 6c73 5f72  ..riv_pd_nncls_r
+00001660: 5a19 7269 765f 7064 5f6e 6e63 6c73 5f72  Z.riv_pd_nncls_r
 00001670: 6f75 7469 6e67 5f69 6e66 6f5a 0e72 656d  outing_infoZ.rem
 00001680: 6f76 655f 6368 616e 6e65 6cda 0573 7562  ove_channel..sub
 00001690: 6964 5a0a 6361 745f 636f 6c6e 6d73 5a0f  idZ.cat_colnmsZ.
 000016a0: 6472 6f70 5f63 6174 5f63 6f6c 6e6d 73da  drop_cat_colnms.
 000016b0: 076f 7574 6c69 6e65 720a 0000 0072 0a00  .outliner....r..
 000016c0: 0000 720e 0000 00da 2373 6176 655f 6d6f  ..r.....#save_mo
 000016d0: 6469 6669 6564 5f61 7474 7269 6275 7465  dified_attribute
@@ -370,26 +370,26 @@
 00001710: 010c 0112 0110 0310 010c 0214 010a 0110  ................
 00001720: 010a 0220 0104 010e 0110 010e 010a 0112  ... ............
 00001730: 0106 010e 010c 010e 0114 0216 0116 0116  ................
 00001740: 0116 0116 0116 0206 010e 010c 0114 0208  ................
 00001750: 0114 0116 0410 020c 020c 010a 0120 0104  ............. ..
 00001760: 010e 0110 010e 0216 0116 0116 0116 0116  ................
 00001770: 0116 0306 0112 010c 0114 0108 0114 0172  ...............r
-00001780: 8300 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00001780: 7b00 0000 6301 0000 0000 0000 0000 0000  {...c...........
 00001790: 0002 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
 000017a0: 0000 7c00 6a00 6401 6402 8d01 6403 6701  ..|.j.d.d...d.g.
 000017b0: 1900 7d01 6404 7c01 6405 3c00 7c01 6a01  ..}.d.|.d.<.|.j.
 000017c0: 6405 6406 6407 6408 8d03 7d01 7c01 5300  d.d.d.d...}.|.S.
-000017d0: 2909 4e54 721a 0000 0072 5300 0000 721e  ).NTr....rS...r.
-000017e0: 0000 00da 0249 4472 5600 0000 4672 5700  .....IDrV...FrW.
-000017f0: 0000 2902 721f 0000 0072 7000 0000 2902  ..).r....rp...).
-00001800: 7278 0000 0072 5200 0000 720a 0000 0072  rx...rR...r....r
-00001810: 0a00 0000 720e 0000 0072 7500 0000 e000  ....r....ru.....
+000017d0: 2909 4e54 721a 0000 0072 5500 0000 721e  ).NTr....rU...r.
+000017e0: 0000 005a 0249 4472 5800 0000 4672 5900  ...Z.IDrX...FrY.
+000017f0: 0000 2902 721f 0000 0072 6800 0000 2902  ..).r....rh...).
+00001800: 7270 0000 0072 5400 0000 720a 0000 0072  rp...rT...r....r
+00001810: 0a00 0000 720e 0000 0072 6d00 0000 e000  ....r....rm.....
 00001820: 0000 7308 0000 0000 0112 0108 0110 0172  ..s............r
-00001830: 7500 0000 6302 0000 0000 0000 0000 0000  u...c...........
+00001830: 6d00 0000 6302 0000 0000 0000 0000 0000  m...c...........
 00001840: 0005 0000 0005 0000 0043 0000 0073 8400  .........C...s..
 00001850: 0000 7400 a001 7c00 6401 1900 a002 7c01  ..t...|.d.....|.
 00001860: a101 a101 7d02 7c00 6402 1900 6403 6b03  ....}.|.d...d.k.
 00001870: 7d03 7400 a003 7c02 7c03 a102 7d04 6404  }.t...|.|...}.d.
 00001880: 7c00 6a04 7c04 6401 6602 3c00 6404 7c00  |.j.|.d.f.<.d.|.
 00001890: 6a04 7c04 6405 6602 3c00 6404 7c00 6a04  j.|.d.f.<.d.|.j.
 000018a0: 7c04 6406 6602 3c00 6404 7c00 6a04 7c04  |.d.f.<.d.|.j.|.
@@ -408,42 +408,42 @@
 00001970: 5265 7475 726e 733a 0a20 2020 202d 2d2d  Returns:.    ---
 00001980: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
 00001990: 652c 2074 6865 2061 7474 7269 6275 7465  e, the attribute
 000019a0: 2074 6162 6c65 206f 6620 5061 7468 5f73   table of Path_s
 000019b0: 6870 6669 6c65 2077 696c 6c20 6265 2075  hpfile will be u
 000019c0: 7064 6174 6564 0a20 2020 20da 0848 794c  pdated.    ..HyL
 000019d0: 616b 6549 6472 5d00 0000 725e 0000 0072  akeIdr]...r^...r
-000019e0: 0100 0000 da07 4c61 6b65 566f 6cda 084c  ......LakeVol..L
-000019f0: 616b 6541 7265 61da 094c 616b 6544 6570  akeArea..LakeDep
-00001a00: 7468 da08 4c61 6b65 7479 7065 2905 da02  th..Laketype)...
+000019e0: 0100 0000 5a07 4c61 6b65 566f 6c5a 084c  ....Z.LakeVolZ.L
+000019f0: 616b 6541 7265 615a 094c 616b 6544 6570  akeAreaZ.LakeDep
+00001a00: 7468 5a08 4c61 6b65 7479 7065 2905 da02  thZ.Laketype)...
 00001a10: 6e70 da0b 6c6f 6769 6361 6c5f 6e6f 7472  np..logical_notr
 00001a20: 2100 0000 da0b 6c6f 6769 6361 6c5f 616e  !.....logical_an
-00001a30: 6472 7400 0000 2905 5a0c 6669 6e61 6c63  drt...).Z.finalc
-00001a40: 6174 5f70 6c79 da0d 436f 6e6e 5f4c 616b  at_ply..Conn_Lak
+00001a30: 6472 6c00 0000 2905 5a0c 6669 6e61 6c63  drl...).Z.finalc
+00001a40: 6174 5f70 6c79 5a0d 436f 6e6e 5f4c 616b  at_plyZ.Conn_Lak
 00001a50: 655f 4964 73da 056d 6173 6b31 da05 6d61  e_Ids..mask1..ma
 00001a60: 736b 32da 046d 6173 6b72 0a00 0000 720a  sk2..maskr....r.
 00001a70: 0000 0072 0e00 0000 da37 5265 6d6f 7665  ...r.....7Remove
 00001a80: 5f55 6e73 656c 6563 7465 645f 4c61 6b65  _Unselected_Lake
 00001a90: 5f41 7474 7269 6275 7465 5f49 6e5f 4669  _Attribute_In_Fi
 00001aa0: 6e61 6c63 6174 696e 666f 5f70 7572 6570  nalcatinfo_purep
 00001ab0: 79e6 0000 0073 1400 0000 000d 1401 0c01  y....s..........
-00001ac0: 0c02 0e01 0e01 0e01 0e01 0e01 0e02 7291  ..............r.
+00001ac0: 0c02 0e01 0e01 0e01 0e01 0e01 0e02 7283  ..............r.
 00001ad0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
 00001ae0: 0300 0000 0700 0000 4300 0000 732a 0000  ........C...s*..
 00001af0: 007c 006a 0074 01a0 0274 01a0 037c 006a  .|.j.t...t...|.j
 00001b00: 007c 01a1 02a1 0119 007d 027c 006a 047c  .|.......}.|.j.|
-00001b10: 0264 018d 017d 007c 0053 0029 024e 7254  .d...}.|.S.).NrT
-00001b20: 0000 0029 0572 3500 0000 728a 0000 0072  ...).r5...r....r
-00001b30: 8b00 0000 7221 0000 0072 6f00 0000 2903  ....r!...ro...).
+00001b10: 0264 018d 017d 007c 0053 0029 024e 7256  .d...}.|.S.).NrV
+00001b20: 0000 0029 0572 3500 0000 727d 0000 0072  ...).r5...r}...r
+00001b30: 7e00 0000 7221 0000 0072 6700 0000 2903  ~...r!...rg...).
 00001b40: da05 7461 626c 65da 056e 616d 6573 5a13  ..table..namesZ.
 00001b50: 7265 6d6f 7665 5f63 6f6c 756d 6e5f 6e61  remove_column_na
 00001b60: 6d65 7372 0a00 0000 720a 0000 0072 0e00  mesr....r....r..
 00001b70: 0000 da1b 636c 6561 6e5f 6174 7472 6962  ....clean_attrib
 00001b80: 7574 655f 6e61 6d65 5f70 7572 6570 7900  ute_name_purepy.
-00001b90: 0100 0073 0600 0000 0001 1a01 0c01 7294  ...s..........r.
+00001b90: 0100 0073 0600 0000 0001 1a01 0c01 7286  ...s..........r.
 00001ba0: 0000 00e9 ffff ffff 6302 0000 0000 0000  ........c.......
 00001bb0: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
 00001bc0: 0073 ca00 0000 7c01 6401 6b04 721a 7c00  .s....|.d.k.r.|.
 00001bd0: 6402 1900 a000 6403 a101 7c00 6402 3c00  d.....d...|.d.<.
 00001be0: 7c00 6402 1900 a001 a100 0f00 7d02 7c00  |.d.........}.|.
 00001bf0: 6a02 0f00 7d03 7c00 6a03 6401 6b04 7d04  j...}.|.j.d.k.}.
 00001c00: 7404 a005 7c02 7c03 a102 7d05 7404 a005  t...|.|...}.t...
@@ -451,198 +451,196 @@
 00001c20: 7d00 7c00 6a06 7c00 6a07 6404 6b03 1900  }.|.j.|.j.d.k...
 00001c30: 7d00 7408 7c00 6a06 7c00 6a07 6405 6b02  }.t.|.j.|.j.d.k.
 00001c40: 1900 8301 6401 6b04 72b0 7409 6406 8301  ....d.k.r.t.d...
 00001c50: 0100 7409 6407 8301 0100 7409 7c00 6a06  ..t.d.....t.|.j.
 00001c60: 7c00 6a07 6405 6b02 1900 8301 0100 7409  |.j.d.k.......t.
 00001c70: 6406 8301 0100 7c00 6a06 7c00 6a07 6405  d.....|.j.|.j.d.
 00001c80: 6b03 1900 7d00 7c00 6a0a 0100 7c00 5300  k...}.|.j...|.S.
-00001c90: 2908 4e72 0100 0000 7253 0000 0067 9564  ).Nr....rS...g.d
+00001c90: 2908 4e72 0100 0000 7255 0000 0067 9564  ).Nr....rU...g.d
 00001ca0: 79e1 7ffd a53d da05 506f 696e 74da 1247  y....=..Point..G
 00001cb0: 656f 6d65 7472 7943 6f6c 6c65 6374 696f  eometryCollectio
 00001cc0: 6e7a 1b23 2323 2323 2323 2323 2323 2323  nz.#############
 00001cd0: 2323 2323 2323 2323 2323 2323 2323 7a1c  ##############z.
 00001ce0: 6368 6563 6b20 7468 6520 666f 6c6c 6f77  check the follow
 00001cf0: 696e 6720 6665 6174 7572 6573 290b da06  ing features)...
 00001d00: 6275 6666 6572 da04 6973 6e61 da08 6973  buffer..isna..is
-00001d10: 5f65 6d70 7479 da04 6172 6561 728a 0000  _empty..arear...
-00001d20: 0072 8c00 0000 7274 0000 00da 0967 656f  .r....rt.....geo
+00001d10: 5f65 6d70 7479 da04 6172 6561 727d 0000  _empty..arear}..
+00001d20: 0072 7f00 0000 726c 0000 00da 0967 656f  .r....rl.....geo
 00001d30: 6d5f 7479 7065 7220 0000 0072 3600 0000  m_typer ...r6...
-00001d40: da06 7369 6e64 6578 2907 723e 0000 005a  ..sindex).r>...Z
+00001d40: da06 7369 6e64 6578 2907 7241 0000 00da  ..sindex).rA....
 00001d50: 0d73 6574 5f70 7265 6369 7369 6f6e 5a05  .set_precisionZ.
 00001d60: 6e61 726f 775a 0565 6d72 6f77 5a07 6172  narowZ.emrowZ.ar
 00001d70: 6561 726f 775a 0472 6f77 315a 0972 6f77  earowZ.row1Z.row
 00001d80: 7365 6c65 6374 720a 0000 0072 0a00 0000  selectr....r....
 00001d90: 720e 0000 0072 3400 0000 0501 0000 7322  r....r4.......s"
 00001da0: 0000 0000 0308 0112 060e 0208 020a 030c  ................
 00001db0: 010c 030a 0210 0118 0108 0108 0114 0108  ................
 00001dc0: 0210 0106 0272 3400 0000 6303 0000 0000  .....r4...c.....
 00001dd0: 0000 0000 0000 0006 0000 0003 0000 0043  ...............C
 00001de0: 0000 0073 3800 0000 7c00 6a00 7d03 7c00  ...s8...|.j.}.|.
 00001df0: a001 a100 7d04 7c00 a002 7c01 a101 7d04  ....}.|...|...}.
 00001e00: 7c04 6a03 7c04 7c02 3c00 7c04 6a01 6401  |.j.|.|.<.|.j.d.
 00001e10: 6402 8d01 a002 7c03 a101 7d05 7c05 5300  d.....|...}.|.S.
 00001e20: 2903 4e54 721a 0000 0029 0472 2e00 0000  ).NTr....).r....
-00001e30: 721f 0000 0072 3100 0000 729b 0000 0029  r....r1...r....)
-00001e40: 0672 3e00 0000 5a07 7072 6a5f 6372 735a  .r>...Z.prj_crsZ
+00001e30: 721f 0000 0072 3100 0000 728d 0000 0029  r....r1...r....)
+00001e40: 0672 4100 0000 da07 7072 6a5f 6372 735a  .rA.....prj_crsZ
 00001e50: 0861 7265 615f 636f 6cda 0773 7263 5f73  .area_col..src_s
 00001e60: 7263 da04 746f 7374 da03 6f75 7472 0a00  rc..tost..outr..
 00001e70: 0000 720a 0000 0072 0e00 0000 da0e 6164  ..r....r......ad
 00001e80: 645f 6172 6561 5f69 6e5f 6d32 2801 0000  d_area_in_m2(...
 00001e90: 730c 0000 0000 0106 0108 020a 010a 0212  s...............
-00001ea0: 0272 a100 0000 6303 0000 0000 0000 0000  .r....c.........
+00001ea0: 0272 9500 0000 6303 0000 0000 0000 0000  .r....c.........
 00001eb0: 0000 0006 0000 0003 0000 0043 0000 0073  ...........C...s
 00001ec0: 4a00 0000 7c00 6a00 7d03 7c00 a001 a100  J...|.j.}.|.....
 00001ed0: 7d04 7c04 a002 6401 a101 7d04 7c04 6a03  }.|...d...}.|.j.
 00001ee0: 6a04 6a05 7c04 7c02 3c00 7c04 6a03 6a04  j.j.|.|.<.|.j.j.
 00001ef0: 6a06 7c04 7c01 3c00 7c04 6a01 6402 6403  j.|.|.<.|.j.d.d.
 00001f00: 8d01 a002 7c03 a101 7d05 7c05 5300 2904  ....|...}.|.S.).
 00001f10: 4efa 0945 5053 473a 3433 3236 5472 1a00  N..EPSG:4326Tr..
 00001f20: 0000 2907 722e 0000 0072 1f00 0000 7231  ..).r....r....r1
-00001f30: 0000 0072 5300 0000 da08 6365 6e74 726f  ...rS.....centro
-00001f40: 6964 da01 7972 0b00 0000 2906 723e 0000  id..yr....).r>..
-00001f50: 005a 0463 6f6c 785a 0463 6f6c 7972 9e00  .Z.colxZ.colyr..
-00001f60: 0000 729f 0000 0072 a000 0000 720a 0000  ..r....r....r...
-00001f70: 0072 0a00 0000 720e 0000 0072 7100 0000  .r....r....rq...
+00001f30: 0000 0072 5500 0000 da08 6365 6e74 726f  ...rU.....centro
+00001f40: 6964 da01 7972 0b00 0000 2906 7241 0000  id..yr....).rA..
+00001f50: 005a 0463 6f6c 785a 0463 6f6c 7972 9200  .Z.colxZ.colyr..
+00001f60: 0000 7293 0000 0072 9400 0000 720a 0000  ..r....r....r...
+00001f70: 0072 0a00 0000 720e 0000 0072 6900 0000  .r....r....ri...
 00001f80: 3301 0000 730e 0000 0000 0106 0108 020a  3...s...........
-00001f90: 020e 010e 0212 0272 7100 0000 6301 0000  .......rq...c...
+00001f90: 020e 010e 0212 0272 6900 0000 6301 0000  .......ri...c...
 00001fa0: 0000 0000 0000 0000 001c 0000 0008 0000  ................
 00001fb0: 0043 0000 0073 7e03 0000 6401 7c00 7601  .C...s~...d.|.v.
 00001fc0: 720c 6400 5300 7400 6a01 a002 7c00 a101  r.d.S.t.j...|...
 00001fd0: 7d01 7400 6a01 a003 7c00 a101 a004 6402  }.t.j...|.....d.
 00001fe0: a101 7d02 7405 7c02 8301 7d03 7c02 7c03  ..}.t.|...}.|.|.
 00001ff0: 6403 1800 1900 6404 6405 8502 1900 7d04  d.....d.d.....}.
-00002000: 6700 6406 a201 7d05 6401 7d06 6407 7d07  g.d...}.d.}.d.}.
-00002010: 6408 7d08 6409 7d09 6700 7d0a 6700 7d0b  d.}.d.}.g.}.g.}.
-00002020: 640a 7c04 7600 72e8 7c06 6402 1700 7c04  d.|.v.r.|.d...|.
-00002030: 1700 640b 1700 7c07 6402 1700 7c04 1700  ..d...|.d...|...
-00002040: 640b 1700 7c08 6402 1700 7c04 1700 640b  d...|.d...|...d.
-00002050: 1700 7c09 6402 1700 7c04 1700 640b 1700  ..|.d...|...d...
-00002060: 6704 7d0a 7c06 6402 1700 7c04 1700 640c  g.}.|.d...|...d.
-00002070: 1700 7c07 6402 1700 7c04 1700 640c 1700  ..|.d...|...d...
-00002080: 7c08 6402 1700 7c04 1700 640c 1700 7c09  |.d...|...d...|.
-00002090: 6402 1700 7c04 1700 640c 1700 6704 7d0b  d...|...d...g.}.
-000020a0: 6e38 7c06 640b 1700 7c07 640b 1700 7c08  n8|.d...|.d...|.
-000020b0: 640b 1700 7c09 640b 1700 6704 7d0a 7c06  d...|.d...g.}.|.
-000020c0: 640c 1700 7c07 640c 1700 7c08 640c 1700  d...|.d...|.d...
-000020d0: 7c09 640c 1700 6704 7d0b 6700 7d0c 6700  |.d...g.}.g.}.g.
+00002000: 6406 6407 6702 7d05 6401 7d06 6408 7d07  d.d.g.}.d.}.d.}.
+00002010: 6409 7d08 640a 7d09 6700 7d0a 6700 7d0b  d.}.d.}.g.}.g.}.
+00002020: 640b 7c04 7600 72e8 7c06 6402 1700 7c04  d.|.v.r.|.d...|.
+00002030: 1700 640c 1700 7c07 6402 1700 7c04 1700  ..d...|.d...|...
+00002040: 640c 1700 7c08 6402 1700 7c04 1700 640c  d...|.d...|...d.
+00002050: 1700 7c09 6402 1700 7c04 1700 640c 1700  ..|.d...|...d...
+00002060: 6704 7d0a 7c06 6402 1700 7c04 1700 640d  g.}.|.d...|...d.
+00002070: 1700 7c07 6402 1700 7c04 1700 640d 1700  ..|.d...|...d...
+00002080: 7c08 6402 1700 7c04 1700 640d 1700 7c09  |.d...|...d...|.
+00002090: 6402 1700 7c04 1700 640d 1700 6704 7d0b  d...|...d...g.}.
+000020a0: 6e38 7c06 640c 1700 7c07 640c 1700 7c08  n8|.d...|.d...|.
+000020b0: 640c 1700 7c09 640c 1700 6704 7d0a 7c06  d...|.d...g.}.|.
+000020c0: 640d 1700 7c07 640d 1700 7c08 640d 1700  d...|.d...|.d...
+000020d0: 7c09 640d 1700 6704 7d0b 6700 7d0c 6700  |.d...g.}.g.}.g.
 000020e0: 7d0d 7406 6404 7405 7c0a 8301 8302 4400  }.t.d.t.|.....D.
 000020f0: 9001 5d2e 7d0e 7400 6a01 a007 7c01 7c0a  ..].}.t.j...|.|.
 00002100: 7c0e 1900 a102 7d0f 7400 6a01 a007 7c01  |.....}.t.j...|.
 00002110: 7c0b 7c0e 1900 a102 7d10 7400 6a01 a008  |.|.....}.t.j...
 00002120: 7c0f a101 9001 7372 9001 7136 7c0c a009  |.....sr..q6|...
-00002130: 7c10 a101 0100 6407 7c0a 7c0e 1900 7600  |.....d.|.|...v.
-00002140: 9001 7398 640d 7c0a 7c0e 1900 7600 9001  ..s.d.|.|...v...
+00002130: 7c10 a101 0100 6408 7c0a 7c0e 1900 7600  |.....d.|.|...v.
+00002140: 9001 7398 640e 7c0a 7c0e 1900 7600 9001  ..s.d.|.|...v...
 00002150: 72a2 7c0d a009 7c10 a101 0100 740a a00b  r.|...|.....t...
-00002160: 7c0f a101 7d11 7c11 a00c 640e a101 7d12  |...}.|...d...}.
-00002170: 6401 7c0a 7c0e 1900 7600 9001 73d2 6407  d.|.|...v...s.d.
-00002180: 7c0a 7c0e 1900 7600 9002 7214 7c12 640f  |.|...v...r.|.d.
+00002160: 7c0f a101 7d11 7c11 a00c 640f a101 7d12  |...}.|...d...}.
+00002170: 6401 7c0a 7c0e 1900 7600 9001 73d2 6408  d.|.|...v...s.d.
+00002180: 7c0a 7c0e 1900 7600 9002 7214 7c12 6410  |.|...v...r.|.d.
 00002190: 1900 a00d 740e a101 a00d 740f a101 7c12  ....t.....t...|.
-000021a0: 6410 3c00 7c12 6a10 4400 5d22 7d13 6411  d.<.|.j.D.]"}.d.
-000021b0: 7c12 6a11 7c13 6410 6602 1900 1700 7c12  |.j.|.d.f.....|.
-000021c0: 6a11 7c13 6410 6602 3c00 9001 71f0 7c12  j.|.d.f.<...q.|.
+000021a0: 6411 3c00 7c12 6a10 4400 5d22 7d13 6412  d.<.|.j.D.]"}.d.
+000021b0: 7c12 6a11 7c13 6411 6602 1900 1700 7c12  |.j.|.d.f.....|.
+000021c0: 6a11 7c13 6411 6602 3c00 9001 71f0 7c12  j.|.d.f.<...q.|.
 000021d0: 7d14 7c05 4400 5d46 7d15 7c14 a012 7c15  }.|.D.]F}.|...|.
-000021e0: a101 7c14 6412 3c00 7c14 6a13 7c10 6413  ..|.d.<.|.j.|.d.
-000021f0: 6414 8d02 0100 7400 a014 7c10 a101 6a15  d.....t...|...j.
-00002200: 6415 1b00 6415 1b00 7d16 7c16 6416 6b01  d...d...}.|.d.k.
+000021e0: a101 7c14 6413 3c00 7c14 6a13 7c10 6414  ..|.d.<.|.j.|.d.
+000021f0: 6415 8d02 0100 7400 a014 7c10 a101 6a15  d.....t...|...j.
+00002200: 6416 1b00 6416 1b00 7d16 7c16 6417 6b01  d...d...}.|.d.k.
 00002210: 9002 721c 0100 9001 7136 9002 711c 9001  ..r.....q6..q...
 00002220: 7136 7405 7c0d 8301 6403 6b04 9003 727a  q6t.|...d.k...rz
 00002230: 7400 a014 7400 6a01 a007 7c01 7c0b 6404  t...t.j...|.|.d.
-00002240: 1900 a102 a101 6a15 6415 1b00 6415 1b00  ......j.d...d...
-00002250: 6417 6b00 9003 727a 7406 6404 7405 7c0d  d.k...rzt.d.t.|.
+00002240: 1900 a102 a101 6a15 6416 1b00 6416 1b00  ......j.d...d...
+00002250: 6418 6b00 9003 727a 7406 6404 7405 7c0d  d.k...rzt.d.t.|.
 00002260: 8301 8302 4400 5d80 7d0e 7416 7417 7c0d  ....D.].}.t.t.|.
-00002270: 7c0e 1900 8301 8301 7d17 6407 7c0d 7c0e  |.......}.d.|.|.
-00002280: 1900 7600 9003 7206 6700 7d18 7c17 6418  ..v...r.g.}.|.d.
-00002290: 1900 4400 5d22 7d19 7c19 6419 1900 641a  ..D.]"}.|.d...d.
+00002270: 7c0e 1900 8301 8301 7d17 6408 7c0d 7c0e  |.......}.d.|.|.
+00002280: 1900 7600 9003 7206 6700 7d18 7c17 6419  ..v...r.g.}.|.d.
+00002290: 1900 4400 5d22 7d19 7c19 641a 1900 641b  ..D.]"}.|.d...d.
 000022a0: 1900 6404 6b02 9002 72da 7c18 a009 7c19  ..d.k...r.|...|.
-000022b0: a101 0100 9002 71da 7c18 7c17 6418 3c00  ......q.|.|.d.<.
+000022b0: a101 0100 9002 71da 7c18 7c17 6419 3c00  ......q.|.|.d.<.
 000022c0: 7c0e 6404 6b02 9003 7216 7c17 7d1a 6e14  |.d.k...r.|.}.n.
-000022d0: 7c1a 6418 0500 1900 7c17 6418 1900 3700  |.d.....|.d...7.
+000022d0: 7c1a 6419 0500 1900 7c17 6419 1900 3700  |.d.....|.d...7.
 000022e0: 0300 3c00 9002 71ac 7417 7400 6a01 a007  ..<...q.t.t.j...
-000022f0: 7c01 641b a102 641c 641d 641e 8d03 8f22  |.d...d.d.d...."
-00002300: 7d1b 7418 6a19 7c1a 7c1b 641f 6405 6420  }.t.j.|.|.d.d.d 
+000022f0: 7c01 641c a102 641d 641e 641f 8d03 8f22  |.d...d.d.d...."
+00002300: 7d1b 7418 6a19 7c1a 7c1b 6420 6405 6421  }.t.j.|.|.d d.d!
 00002310: 8d04 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
 00002320: 6e12 3100 9003 7370 3000 0100 0100 0100  n.1...sp0.......
-00002330: 5900 0100 6400 5300 2921 4eda 0d66 696e  Y...d.S.)!N..fin
+00002330: 5900 0100 6400 5300 2922 4e5a 0d66 696e  Y...d.S.)"NZ.fin
 00002340: 616c 6361 745f 696e 666f da01 5f72 1e00  alcat_info.._r..
-00002350: 0000 7201 0000 00e9 0400 0000 2906 672d  ..r.........).g-
-00002360: 431c ebe2 361a 3f67 fca9 f1d2 4d62 403f  C...6.?g....Mb@?
-00002370: 67fc a9f1 d24d 6250 3f67 7b14 ae47 e17a  g....MbP?g{..G.z
-00002380: 743f 677b 14ae 47e1 7a84 3f67 9a99 9999  t?g{..G.z.?g....
-00002390: 9999 a93f da11 6669 6e61 6c63 6174 5f69  ...?..finalcat_i
-000023a0: 6e66 6f5f 7269 76da 1173 6c5f 636f 6e6e  nfo_riv..sl_conn
-000023b0: 6563 7465 645f 6c61 6b65 da15 736c 5f6e  ected_lake..sl_n
-000023c0: 6f6e 5f63 6f6e 6e65 6374 6564 5f6c 616b  on_connected_lak
-000023d0: 65da 0176 7a04 2e73 6870 7a08 2e67 656f  e..vz..shpz..geo
-000023e0: 6a73 6f6e da0e 636f 6e6e 6563 7465 645f  json..connected_
-000023f0: 6c61 6b65 72a2 0000 0072 4200 0000 da07  laker....rB.....
-00002400: 7276 684e 616d 65da 0373 7562 7253 0000  rvhName..subrS..
-00002410: 00da 0747 656f 4a53 4f4e 2901 da06 6472  ...GeoJSON)...dr
-00002420: 6976 6572 6900 0400 00e9 6400 0000 69f4  iveri.....d...i.
-00002430: 0100 00da 0866 6561 7475 7265 7372 0800  .....featuresr..
-00002440: 0000 725d 0000 007a 2272 6f75 7469 6e67  ..r]...z"routing
-00002450: 5f70 726f 6475 6374 5f6c 616b 655f 7269  _product_lake_ri
-00002460: 7665 722e 6765 6f6a 736f 6eda 0177 7a05  ver.geojson..wz.
-00002470: 7574 662d 3829 01da 0865 6e63 6f64 696e  utf-8)...encodin
-00002480: 6746 2902 da0c 656e 7375 7265 5f61 7363  gF)...ensure_asc
-00002490: 6969 da06 696e 6465 6e74 291a 726a 0000  ii..indent).rj..
-000024a0: 0072 6b00 0000 da07 6469 726e 616d 65da  .rk.....dirname.
-000024b0: 0862 6173 656e 616d 65da 0573 706c 6974  .basename..split
-000024c0: 7220 0000 00da 0572 616e 6765 726c 0000  r .....rangerl..
-000024d0: 00da 0665 7869 7374 7372 2200 0000 722f  ...existsr"...r/
-000024e0: 0000 0072 3000 0000 7231 0000 00da 0661  ...r0...r1.....a
-000024f0: 7374 7970 65da 0369 6e74 da03 7374 7272  stype..int..strr
-00002500: 7700 0000 7274 0000 00da 0873 696d 706c  w...rt.....simpl
-00002510: 6966 7972 7300 0000 da04 7374 6174 da07  ifyrs.....stat..
-00002520: 7374 5f73 697a 6572 0200 0000 7269 0000  st_sizer....ri..
-00002530: 00da 046a 736f 6eda 0464 756d 7029 1cda  ...json..dump)..
-00002540: 1249 6e70 7574 5f50 6f6c 7967 6f6e 5f70  .Input_Polygon_p
-00002550: 6174 68da 0b70 726f 6475 6374 5f64 6972  ath..product_dir
-00002560: da08 4e61 6d65 735f 696e da07 6e5f 6368  ..Names_in..n_ch
-00002570: 6172 63da 0776 6572 7369 6f6e da0a 544f  arc..version..TO
-00002580: 4c45 5241 4e43 4573 da0d 6865 6164 5f6e  LERANCEs..head_n
-00002590: 616d 655f 6361 74da 0d68 6561 645f 6e61  ame_cat..head_na
-000025a0: 6d65 5f72 6976 da0f 6865 6164 5f6e 616d  me_riv..head_nam
-000025b0: 655f 736c 616b 65da 0f68 6561 645f 6e61  e_slake..head_na
-000025c0: 6d65 5f6e 6c61 6b65 da0f 496e 7075 745f  me_nlake..Input_
-000025d0: 6669 6c65 5f6e 616d 65da 104f 7574 7075  file_name..Outpu
-000025e0: 745f 6669 6c65 5f6e 616d 65da 1363 7265  t_file_name..cre
-000025f0: 6174 6564 5f6a 6173 6f6e 5f66 696c 6573  ated_jason_files
-00002600: da1c 6372 6561 7465 645f 6a61 736f 6e5f  ..created_jason_
-00002610: 6669 6c65 735f 6c61 6b65 5f72 6976 7224  files_lake_rivr$
-00002620: 0000 00da 0a69 6e70 7574 5f70 6174 68da  .....input_path.
-00002630: 116f 7574 7075 745f 6a61 736f 6e5f 7061  .output_jason_pa
-00002640: 7468 5a08 696e 7075 745f 7064 da0c 696e  thZ.input_pd..in
-00002650: 7075 745f 7767 735f 3834 da03 6964 78da  put_wgs_84..idx.
-00002660: 0c69 6e70 7574 5f74 6f6a 736f 6eda 0954  .input_tojson..T
-00002670: 4f4c 4552 414e 4345 da0e 6a73 6f6e 5f66  OLERANCE..json_f
-00002680: 696c 655f 7369 7a65 da07 696e 6a73 6f6e  ile_size..injson
-00002690: 32da 0c6e 6577 5f66 6561 7475 7265 73da  2..new_features.
-000026a0: 0765 6c65 6d65 6e74 da15 6f75 7470 7574  .element..output
-000026b0: 5f6a 6173 6f6e 5f6c 616b 655f 7269 7672  _jason_lake_rivr
-000026c0: 7f00 0000 720a 0000 0072 0a00 0000 720e  ....r....r....r.
-000026d0: 0000 0072 7600 0000 4101 0000 7390 0000  ...rv...A...s...
-000026e0: 0000 0208 0204 020c 0112 0108 0114 0108  ................
-000026f0: 0304 0104 0104 0104 0204 0104 0108 020e  ................
-00002700: 010e 010e 010e fc04 070e 010e 010e 010e  ................
-00002710: fc06 0806 0106 0106 0106 fc04 0706 0106  ................
-00002720: 0106 0106 fc04 0604 0104 0214 0112 0112  ................
-00002730: 010e 0104 010a 021c 010a 030a 020a 041c  ................
-00002740: 0118 010a 0120 0304 0208 010e 010e 0214  ..... ..........
-00002750: 010a 010e 0236 0112 0110 010e 0104 010c  .....6..........
-00002760: 0112 010e 0108 020a 0106 0218 021a 0132  ...............2
-00002770: 0272 7600 0000 2902 7226 0000 0072 2600  .rv...).r&...r&.
-00002780: 0000 2901 7242 0000 0029 0172 9500 0000  ..).rB...).r....
-00002790: 291b 722f 0000 00da 056e 756d 7079 728a  ).r/.....numpyr.
-000027a0: 0000 0072 6a00 0000 da06 7061 6e64 6173  ...rj.....pandas
-000027b0: 7213 0000 0072 c200 0000 7202 0000 0072  r....r....r....r
-000027c0: 0300 0000 7267 0000 0072 3700 0000 da05  ....rg...r7.....
-000027d0: 6f73 6765 6f72 0400 0000 7205 0000 005a  osgeor....r....Z
-000027e0: 0b72 6173 7465 7273 7461 7473 7206 0000  .rasterstatsr...
-000027f0: 0072 1900 0000 7225 0000 0072 4100 0000  .r....r%...rA...
-00002800: 7283 0000 0072 7500 0000 7291 0000 0072  r....ru...r....r
-00002810: 9400 0000 7234 0000 0072 a100 0000 7271  ....r4...r....rq
-00002820: 0000 0072 7600 0000 720a 0000 0072 0a00  ...rv...r....r..
-00002830: 0000 720a 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
-00002840: 6f64 756c 653e 0100 0000 732a 0000 0008  odule>....s*....
-00002850: 0108 0108 0108 0110 0108 0108 0108 0310  ................
-00002860: 010c 0208 0c08 1c00 ff0a 4b0a 6008 0608  ..........K.`...
-00002870: 1a08 050a 2308 0b08 0e                   ....#....
+00002350: 0000 7201 0000 00e9 0400 0000 672d 431c  ..r.........g-C.
+00002360: ebe2 361a 3f67 7b14 ae47 e17a 743f 5a11  ..6.?g{..G.zt?Z.
+00002370: 6669 6e61 6c63 6174 5f69 6e66 6f5f 7269  finalcat_info_ri
+00002380: 76da 1173 6c5f 636f 6e6e 6563 7465 645f  v..sl_connected_
+00002390: 6c61 6b65 da15 736c 5f6e 6f6e 5f63 6f6e  lake..sl_non_con
+000023a0: 6e65 6374 6564 5f6c 616b 65da 0176 7a04  nected_lake..vz.
+000023b0: 2e73 6870 7a08 2e67 656f 6a73 6f6e 5a0e  .shpz..geojsonZ.
+000023c0: 636f 6e6e 6563 7465 645f 6c61 6b65 7296  connected_laker.
+000023d0: 0000 0072 4500 0000 5a07 7276 684e 616d  ...rE...Z.rvhNam
+000023e0: 65da 0373 7562 7255 0000 00da 0747 656f  e..subrU.....Geo
+000023f0: 4a53 4f4e 2901 da06 6472 6976 6572 6900  JSON)...driveri.
+00002400: 0400 00e9 6400 0000 69f4 0100 00da 0866  ....d...i......f
+00002410: 6561 7475 7265 7372 0800 0000 725d 0000  eaturesr....r]..
+00002420: 007a 2272 6f75 7469 6e67 5f70 726f 6475  .z"routing_produ
+00002430: 6374 5f6c 616b 655f 7269 7665 722e 6765  ct_lake_river.ge
+00002440: 6f6a 736f 6eda 0177 7a05 7574 662d 3829  ojson..wz.utf-8)
+00002450: 01da 0865 6e63 6f64 696e 6746 2902 da0c  ...encodingF)...
+00002460: 656e 7375 7265 5f61 7363 6969 da06 696e  ensure_ascii..in
+00002470: 6465 6e74 291a 7262 0000 0072 6300 0000  dent).rb...rc...
+00002480: da07 6469 726e 616d 65da 0862 6173 656e  ..dirname..basen
+00002490: 616d 65da 0573 706c 6974 7220 0000 00da  ame..splitr ....
+000024a0: 0572 616e 6765 7264 0000 00da 0665 7869  .rangerd.....exi
+000024b0: 7374 7372 2200 0000 722f 0000 0072 3000  stsr"...r/...r0.
+000024c0: 0000 7231 0000 00da 0661 7374 7970 65da  ..r1.....astype.
+000024d0: 0369 6e74 da03 7374 7272 6f00 0000 726c  .int..strro...rl
+000024e0: 0000 00da 0873 696d 706c 6966 7972 6b00  .....simplifyrk.
+000024f0: 0000 da04 7374 6174 da07 7374 5f73 697a  ....stat..st_siz
+00002500: 6572 0200 0000 7261 0000 00da 046a 736f  er....ra.....jso
+00002510: 6eda 0464 756d 7029 1c5a 1249 6e70 7574  n..dump).Z.Input
+00002520: 5f50 6f6c 7967 6f6e 5f70 6174 685a 0b70  _Polygon_pathZ.p
+00002530: 726f 6475 6374 5f64 6972 5a08 4e61 6d65  roduct_dirZ.Name
+00002540: 735f 696e 5a07 6e5f 6368 6172 63da 0776  s_inZ.n_charc..v
+00002550: 6572 7369 6f6e da0a 544f 4c45 5241 4e43  ersion..TOLERANC
+00002560: 4573 5a0d 6865 6164 5f6e 616d 655f 6361  EsZ.head_name_ca
+00002570: 745a 0d68 6561 645f 6e61 6d65 5f72 6976  tZ.head_name_riv
+00002580: 5a0f 6865 6164 5f6e 616d 655f 736c 616b  Z.head_name_slak
+00002590: 655a 0f68 6561 645f 6e61 6d65 5f6e 6c61  eZ.head_name_nla
+000025a0: 6b65 5a0f 496e 7075 745f 6669 6c65 5f6e  keZ.Input_file_n
+000025b0: 616d 655a 104f 7574 7075 745f 6669 6c65  ameZ.Output_file
+000025c0: 5f6e 616d 655a 1363 7265 6174 6564 5f6a  _nameZ.created_j
+000025d0: 6173 6f6e 5f66 696c 6573 5a1c 6372 6561  ason_filesZ.crea
+000025e0: 7465 645f 6a61 736f 6e5f 6669 6c65 735f  ted_jason_files_
+000025f0: 6c61 6b65 5f72 6976 7224 0000 005a 0a69  lake_rivr$...Z.i
+00002600: 6e70 7574 5f70 6174 68da 116f 7574 7075  nput_path..outpu
+00002610: 745f 6a61 736f 6e5f 7061 7468 5a08 696e  t_jason_pathZ.in
+00002620: 7075 745f 7064 5a0c 696e 7075 745f 7767  put_pdZ.input_wg
+00002630: 735f 3834 da03 6964 785a 0c69 6e70 7574  s_84..idxZ.input
+00002640: 5f74 6f6a 736f 6eda 0954 4f4c 4552 414e  _tojson..TOLERAN
+00002650: 4345 da0e 6a73 6f6e 5f66 696c 655f 7369  CE..json_file_si
+00002660: 7a65 5a07 696e 6a73 6f6e 325a 0c6e 6577  zeZ.injson2Z.new
+00002670: 5f66 6561 7475 7265 73da 0765 6c65 6d65  _features..eleme
+00002680: 6e74 5a15 6f75 7470 7574 5f6a 6173 6f6e  ntZ.output_jason
+00002690: 5f6c 616b 655f 7269 7672 7800 0000 720a  _lake_rivrx...r.
+000026a0: 0000 0072 0a00 0000 720e 0000 0072 6e00  ...r....r....rn.
+000026b0: 0000 4101 0000 7390 0000 0000 0208 0204  ..A...s.........
+000026c0: 020c 0112 0108 0114 0108 0304 0104 0104  ................
+000026d0: 0104 0204 0104 0108 020e 010e 010e 010e  ................
+000026e0: fc04 070e 010e 010e 010e fc06 0806 0106  ................
+000026f0: 0106 0106 fc04 0706 0106 0106 0106 fc04  ................
+00002700: 0604 0104 0214 0112 0112 010e 0104 010a  ................
+00002710: 021c 010a 030a 020a 041c 0118 010a 0120  ............... 
+00002720: 0304 0208 010e 010e 0214 010a 010e 0236  ...............6
+00002730: 0112 0110 010e 0104 010c 0112 010e 0108  ................
+00002740: 020a 0106 0218 021a 0132 0272 6e00 0000  .........2.rn...
+00002750: 2902 7226 0000 0072 2600 0000 2901 7245  ).r&...r&...).rE
+00002760: 0000 0029 0172 8700 0000 291b 722f 0000  ...).r....).r/..
+00002770: 00da 056e 756d 7079 727d 0000 0072 6200  ...numpyr}...rb.
+00002780: 0000 da06 7061 6e64 6173 7213 0000 0072  ....pandasr....r
+00002790: b200 0000 7202 0000 0072 0300 0000 725f  ....r....r....r_
+000027a0: 0000 0072 3700 0000 da05 6f73 6765 6f72  ...r7.....osgeor
+000027b0: 0400 0000 7205 0000 005a 0b72 6173 7465  ....r....Z.raste
+000027c0: 7273 7461 7473 7206 0000 0072 1900 0000  rstatsr....r....
+000027d0: 7225 0000 0072 4400 0000 727b 0000 0072  r%...rD...r{...r
+000027e0: 6d00 0000 7283 0000 0072 8600 0000 7234  m...r....r....r4
+000027f0: 0000 0072 9500 0000 7269 0000 0072 6e00  ...r....ri...rn.
+00002800: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+00002810: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00002820: 0100 0000 732a 0000 0008 0108 0108 0108  ....s*..........
+00002830: 0110 0108 0108 0108 0310 010c 0208 0c08  ................
+00002840: 1c00 ff0a 4b0a 6008 0608 1a08 050a 2308  ....K.`.......#.
+00002850: 0b08 0e                                  ...
```

### Comparing `basinmaker-3.0.3/basinmaker/func/__pycache__/qgis.cpython-39.pyc` & `basinmaker-3.0.3a0/basinmaker/func/__pycache__/qgis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/__pycache__/rarray.cpython-39.pyc` & `basinmaker-3.0.3a0/basinmaker/func/__pycache__/rarray.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/arcgis.py` & `basinmaker-3.0.3a0/basinmaker/func/arcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/fgdal.py` & `basinmaker-3.0.3a0/basinmaker/func/fgdal.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/grassgis.py` & `basinmaker-3.0.3a0/basinmaker/func/grassgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/pdtable.py` & `basinmaker-3.0.3a0/basinmaker/func/pdtable.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/purepy.py` & `basinmaker-3.0.3a0/basinmaker/func/purepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/qgis.py` & `basinmaker-3.0.3a0/basinmaker/func/qgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/func/rarray.py` & `basinmaker-3.0.3a0/basinmaker/func/rarray.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/hymodin/raveninput.py` & `basinmaker-3.0.3a0/basinmaker/hymodin/raveninput.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/assigninterestsites.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/assigninterestsites.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/combine.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/combine.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/combinearcgis.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/combinearcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/combinepurepy.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/combinepurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/downloadpd.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpd.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/downloadpdptspurepy.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/downloadpdptspurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/gridweight.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/gridweight.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/gridweightarcgis.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/gridweightarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/hru.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/hru.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/hruarcgis.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/hruarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/hrupurepy.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/hrupurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/increaseda.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/increaseda.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/increasedaarcgis.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/increasedaarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/increasedapurepy.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/increasedapurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/inversetopology.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/inversetopology.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/plotleaflet.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/plotleaflet.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/postprocessingfunctions.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/postprocessingfunctions.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/selectlake.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/selectlake.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/selectlakearcgis.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/selectlakearcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/selectlakepurepy.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/selectlakepurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/selectprod.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/selectprod.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/selectprodarcgis.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/postprocessing/selectprodpurepy.py` & `basinmaker-3.0.3a0/basinmaker/postprocessing/selectprodpurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/preprocessing/preinputpolygonqgis.py` & `basinmaker-3.0.3a0/basinmaker/preprocessing/preinputpolygonqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/preprocessing/preprocessinglakeply.py` & `basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessinglakeply.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/preprocessing/preprocessingobs.py` & `basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessingobs.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/preprocessing/preprocessrasterqgis.py` & `basinmaker-3.0.3a0/basinmaker/preprocessing/preprocessrasterqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py` & `basinmaker-3.0.3a0/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py` & `basinmaker-3.0.3a0/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/subreg/defsubreg.py` & `basinmaker-3.0.3a0/basinmaker/subreg/defsubreg.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/subreg/generatesubregionqgis.py` & `basinmaker-3.0.3a0/basinmaker/subreg/generatesubregionqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker/utilities/utilities.py` & `basinmaker-3.0.3a0/basinmaker/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/basinmaker.egg-info/PKG-INFO` & `basinmaker-3.0.3a0/basinmaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basinmaker
-Version: 3.0.3
+Version: 3.0.3a0
 Summary: An automated GIS toolbox for watershed delineation with lakes
 Home-page: https://github.com/dustming/basinmaker
 Author: basinmaker development team
 Author-email: m43han@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basinmaker-3.0.3/basinmaker.egg-info/SOURCES.txt` & `basinmaker-3.0.3a0/basinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/setup.py` & `basinmaker-3.0.3a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="basinmaker",
-    version="3.0.3",
+    version="3.0.3a",
     author="basinmaker development team",
     author_email="m43han@uwaterloo.ca",
     description="An automated GIS toolbox for watershed delineation with lakes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dustming/basinmaker",
     packages = setuptools.find_packages(
```

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_Generateinputdata.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_Generateinputdata.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_Generatmaskregion.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_Generatmaskregion.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_SelectLakes.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_SelectLakes.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.3/tests/test_RoutingTool_WatershedDiscretizationToolset.py` & `basinmaker-3.0.3a0/tests/test_RoutingTool_WatershedDiscretizationToolset.py`

 * *Files identical despite different names*

