# Comparing `tmp/xarrayaita-0.2.5-py3-none-any.whl.zip` & `tmp/xarrayaita-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 28554 bytes, number of entries: 13
--rw-r--r--  2.0 unx      263 b- defN 22-Sep-28 09:31 xarrayaita/__init__.py
+Zip file size: 28568 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      263 b- defN 23-Apr-18 08:38 xarrayaita/__init__.py
 -rw-r--r--  2.0 unx     1347 b- defN 22-Sep-27 07:28 xarrayaita/aita.py
 -rw-r--r--  2.0 unx     4898 b- defN 22-Sep-27 07:28 xarrayaita/aita_export.py
 -rw-r--r--  2.0 unx     6679 b- defN 22-Sep-27 07:28 xarrayaita/aita_geom.py
 -rw-r--r--  2.0 unx    16005 b- defN 22-Sep-27 07:28 xarrayaita/aita_interactive_nb.py
 -rw-r--r--  2.0 unx      975 b- defN 22-Nov-17 13:24 xarrayaita/aita_plot.py
 -rw-r--r--  2.0 unx    12164 b- defN 22-Sep-27 07:28 xarrayaita/aita_processing.py
--rw-r--r--  2.0 unx     6861 b- defN 23-Jan-04 13:58 xarrayaita/loadData_aita.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jan-04 14:02 xarrayaita-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1072 b- defN 23-Jan-04 14:02 xarrayaita-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-04 14:02 xarrayaita-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jan-04 14:02 xarrayaita-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1058 b- defN 23-Jan-04 14:02 xarrayaita-0.2.5.dist-info/RECORD
-13 files, 86574 bytes uncompressed, 26796 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx     6899 b- defN 23-Apr-18 08:37 xarrayaita/loadData_aita.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-18 08:46 xarrayaita-0.2.6.dist-info/RECORD
+13 files, 86612 bytes uncompressed, 26810 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: xarrayaita/aita_processing.py
 Comment: 
 
 Filename: xarrayaita/loadData_aita.py
 Comment: 
 
-Filename: xarrayaita-0.2.5.dist-info/LICENSE
+Filename: xarrayaita-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: xarrayaita-0.2.5.dist-info/METADATA
+Filename: xarrayaita-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: xarrayaita-0.2.5.dist-info/WHEEL
+Filename: xarrayaita-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: xarrayaita-0.2.5.dist-info/top_level.txt
+Filename: xarrayaita-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xarrayaita-0.2.5.dist-info/RECORD
+Filename: xarrayaita-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xarrayaita/__init__.py

```diff
@@ -5,8 +5,8 @@
 from .loadData_aita import aita5col
 from .loadData_aita import aita3col
 from .loadData_aita import craft_input
 
 
 __all__ = ['aita', 'aita5col', 'aita3col', 'craft_input']
 
-__version__='0.2.2'
+__version__='0.2.6'
```

## xarrayaita/loadData_aita.py

```diff
@@ -5,28 +5,28 @@
 from skimage import morphology
 import vtk
 from vtk.util.numpy_support import vtk_to_numpy
 import scipy
 import pickle as pk
 
 
-def aita5col(adr_data, micro_adress=0):
+def aita5col(adr_data, micro_adress=0,**kwargs):
     '''
     Function to load the data from G50 analyser that have 5 columns
 
     :param adr_data: path to the data
     :type adr_data: str
     :param micro_adress: path to microstructure file (black and white image where grains boundaries are white) `.bmp`
     :type micro_adress: str
     '''
     data = pd.read_csv(adr_data, usecols=[1, 2, 3, 4, 6], skiprows=16, comment='[', header=0, names=[
-                       'x', 'y', 'azi', 'col', 'qua'], delimiter=' ')
+                       'x', 'y', 'azi', 'col', 'qua'], delimiter=' ',**kwargs)
 
     # read head of file
-    file = open(adr_data, 'r')
+    file = open(adr_data, 'rb')
     a = []
     [a.append(file.readline()) for i in list(range(16))]
     file.close()
     # resolution mu m
     res = float(a[5][10:12])
     # transforme the resolution in mm
     resolution = res/1000.
@@ -70,41 +70,41 @@
     ds.attrs["step_size"] = resolution
     ds.attrs["path_dat"] = adr_data
     return ds
 
 # ---------------------------------------
 
 
-def aita3col(adr_data, image=None, micro_adress=0,filter_no_ice=False):
+def aita3col(adr_data, image=None, micro_adress=0,filter_no_ice=False,**kwargs):
     '''
     Function to load the data from G50 analyser that have 3 columns
 
     :param adr_data: path to the data
     :type adr_data: str
     :param image: path to one image from G50 analyser
     :type image: str
     :param micro_adress: path to microstructure file (black and white image where grains boundaries are white) `.bmp`
     :type micro_adress: str
     '''
 
     # read head of file
-    file = open(adr_data, 'r')
+    file = open(adr_data, 'rb')
     a = []
     [a.append(file.readline()) for i in list(range(20))]
     file.close()
     # find type of file
     id_f=a.index('[data]\n')
 
     # resolution mu m
     res = float(a[5][10:12])
     # transforme the resolution in mm
     resolution = res/1000.
 
     data = pd.read_csv(adr_data, usecols=[0, 1, 2], skiprows=id_f, comment='[', names=[
-                        'azi', 'col', 'qua'], delimiter=' ')
+                        'azi', 'col', 'qua'], delimiter=' ',**kwargs)
 
     if filter_no_ice:
         id=((data.azi**2+data.col**2)==0)
         data.qua[id]=0
 
     if id_f==17:
         nx=int(a[12].split('=')[-1])
```

## Comparing `xarrayaita-0.2.5.dist-info/LICENSE` & `xarrayaita-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xarrayaita-0.2.5.dist-info/METADATA` & `xarrayaita-0.2.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarrayaita
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tools to work on output from AITA
 Home-page: https://gricad-gitlab.univ-grenoble-alpes.fr/mecaiceige/tools/lib_python/xarray_aita
 Author: Thomas Chauve
 Author-email: thomas.chauve@univ-grenoble-alpes.fr
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

## Comparing `xarrayaita-0.2.5.dist-info/RECORD` & `xarrayaita-0.2.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-xarrayaita/__init__.py,sha256=byqo-tEVx-OYxBEz_V9lu5oiF3FMrzryPOvv93vHnNY,263
+xarrayaita/__init__.py,sha256=yn2X2skf4ihNjaMVMh3Bdj606_xKP5Yzt7eRY5XNfNY,263
 xarrayaita/aita.py,sha256=brGzqVA5fufWG-tsLyIOdGunj1DdrTDhakZG-B73Cg8,1347
 xarrayaita/aita_export.py,sha256=H0eEgeIgNY-tZHJ_syo2xqX_6k-Jn0T3pYEaYSRbK9k,4898
 xarrayaita/aita_geom.py,sha256=olZffQqAaNH8Vhrb-aR_3EdCUXjkCEL3v7nkYPuLXD4,6679
 xarrayaita/aita_interactive_nb.py,sha256=roYRhc_PfrMSsoHeSd1xhZ30W99RYsURjTorZ2PXYds,16005
 xarrayaita/aita_plot.py,sha256=sitVEzjxFNgchlM93RckdWPNQT-nikDENv07nyKrEcA,975
 xarrayaita/aita_processing.py,sha256=LyrSR0tsTZ7Mj6n5hutEeXjFNpmeh5XDcyljZr7wC-w,12164
-xarrayaita/loadData_aita.py,sha256=FtL8lnVVETEmwEx5aV3N1vyDvbfG4LnM-JKtfSGnYV0,6861
-xarrayaita-0.2.5.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-xarrayaita-0.2.5.dist-info/METADATA,sha256=7FqA4WnEnAexN5txsnHRNwinLuN0tllvpaWh8XsFPWw,1072
-xarrayaita-0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xarrayaita-0.2.5.dist-info/top_level.txt,sha256=Ohg9Yo4Ya3hbXoW4drW0ZIPQBb94aXXWy8SgHsfeFI4,11
-xarrayaita-0.2.5.dist-info/RECORD,,
+xarrayaita/loadData_aita.py,sha256=nspH4OIKTiU6dAvnh-rdpi60Cvw1ZyxYeIusxBOCVxw,6899
+xarrayaita-0.2.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+xarrayaita-0.2.6.dist-info/METADATA,sha256=I5f6o-89g5jpjvS_HYcesPoR43icYOUfWPbOvuOkxTA,1072
+xarrayaita-0.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xarrayaita-0.2.6.dist-info/top_level.txt,sha256=Ohg9Yo4Ya3hbXoW4drW0ZIPQBb94aXXWy8SgHsfeFI4,11
+xarrayaita-0.2.6.dist-info/RECORD,,
```

