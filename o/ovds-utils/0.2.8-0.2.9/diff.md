# Comparing `tmp/ovds_utils-0.2.8.tar.gz` & `tmp/ovds_utils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovds_utils-0.2.8.tar", last modified: Wed Oct 12 07:23:16 2022, max compression
+gzip compressed data, was "dist/ovds_utils-0.2.9.tar", last modified: Wed Oct 12 09:19:32 2022, max compression
```

## Comparing `ovds_utils-0.2.8.tar` & `ovds_utils-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 07:23:16.367741 ovds_utils-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-10-12 07:23:16.367741 ovds_utils-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-12 07:23:16.367741 ovds_utils-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 07:23:16.363741 ovds_utils-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 07:23:16.363741 ovds_utils-0.2.8/src/ovds_utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 07:23:16.367741 ovds_utils-0.2.8/src/ovds_utils/ovds/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/ovds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/ovds/copy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/ovds/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     6418 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/ovds/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5716 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/ovds/writing.py
--rw-r--r--   0 runner    (1001) docker     (121)    18958 2022-10-12 07:23:08.000000 ovds_utils-0.2.8/src/ovds_utils/vds.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 07:23:16.363741 ovds_utils-0.2.8/src/ovds_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-10-12 07:23:16.000000 ovds_utils-0.2.8/src/ovds_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-10-12 07:23:16.000000 ovds_utils-0.2.8/src/ovds_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 07:23:16.000000 ovds_utils-0.2.8/src/ovds_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-12 07:23:16.000000 ovds_utils-0.2.8/src/ovds_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-12 07:23:16.000000 ovds_utils-0.2.8/src/ovds_utils.egg-info/top_level.txt
+drwxrwxr-x   0 micmur    (1000) micmur    (1000)        0 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     3467 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/PKG-INFO
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     2255 2022-03-04 11:28:21.000000 ovds_utils-0.2.9/README.md
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)      147 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/setup.cfg
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     1205 2022-10-12 09:18:35.000000 ovds_utils-0.2.9/setup.py
+drwxrwxr-x   0 micmur    (1000) micmur    (1000)        0 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/
+drwxrwxr-x   0 micmur    (1000) micmur    (1000)        0 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils/
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)        0 2022-02-24 12:17:59.000000 ovds_utils-0.2.9/src/ovds_utils/__init__.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)       93 2022-02-24 15:16:17.000000 ovds_utils-0.2.9/src/ovds_utils/exceptions.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)      477 2022-02-24 19:35:28.000000 ovds_utils-0.2.9/src/ovds_utils/logging.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     1971 2022-10-12 07:12:31.000000 ovds_utils-0.2.9/src/ovds_utils/metadata.py
+drwxrwxr-x   0 micmur    (1000) micmur    (1000)        0 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils/ovds/
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)      330 2022-10-12 08:47:58.000000 ovds_utils-0.2.9/src/ovds_utils/ovds/__init__.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)      862 2022-10-12 07:12:31.000000 ovds_utils-0.2.9/src/ovds_utils/ovds/copy.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     3041 2022-10-12 08:42:33.000000 ovds_utils-0.2.9/src/ovds_utils/ovds/enums.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     6418 2022-10-12 07:12:31.000000 ovds_utils-0.2.9/src/ovds_utils/ovds/utils.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     6324 2022-10-12 08:47:11.000000 ovds_utils-0.2.9/src/ovds_utils/ovds/writing.py
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)    19107 2022-10-12 09:18:47.000000 ovds_utils-0.2.9/src/ovds_utils/vds.py
+drwxrwxr-x   0 micmur    (1000) micmur    (1000)        0 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils.egg-info/
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)     3467 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)      497 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)        1 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)       55 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils.egg-info/requires.txt
+-rw-rw-r--   0 micmur    (1000) micmur    (1000)       11 2022-10-12 09:19:32.000000 ovds_utils-0.2.9/src/ovds_utils.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ovds_utils-0.2.8/PKG-INFO` & `ovds_utils-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovds_utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utilities package for Open VDS.
 Home-page: https://github.com/micmurawski/ovds-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Description: # Introduction
```

### Comparing `ovds_utils-0.2.8/README.md` & `ovds_utils-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ovds_utils-0.2.8/setup.py` & `ovds_utils-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def get_dependencies():
     with open("requirements.txt", encoding="utf-8") as fh:
         return fh.read().splitlines()
 
 
 setup(
     name='ovds_utils',
-    version='0.2.8',
+    version='0.2.9',
     author="Michal Murawski",
     author_email="mmurawski777@gmail.com",
     description="Utilities package for Open VDS.",
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     url="https://github.com/micmurawski/ovds-utils/",
     package_dir={"": "src"},
```

### Comparing `ovds_utils-0.2.8/src/ovds_utils/metadata.py` & `ovds_utils-0.2.9/src/ovds_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `ovds_utils-0.2.8/src/ovds_utils/ovds/copy.py` & `ovds_utils-0.2.9/src/ovds_utils/ovds/copy.py`

 * *Files identical despite different names*

### Comparing `ovds_utils-0.2.8/src/ovds_utils/ovds/enums.py` & `ovds_utils-0.2.9/src/ovds_utils/ovds/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-from enum import Enum
+from enum import Enum, auto
 
 import openvds
 
 
+class InitValue(Enum):
+    NaN = auto()
+    zero = auto()
+
+
 class Formats(Enum):
     _1Bit = openvds.VolumeDataChannelDescriptor.Format.Format_1Bit
     U8 = openvds.VolumeDataChannelDescriptor.Format.Format_U8
     U16 = openvds.VolumeDataChannelDescriptor.Format.Format_U16
     R32 = openvds.VolumeDataChannelDescriptor.Format.Format_R32
     U32 = openvds.VolumeDataChannelDescriptor.Format.Format_U32
     U64 = openvds.VolumeDataChannelDescriptor.Format.Format_U64
```

### Comparing `ovds_utils-0.2.8/src/ovds_utils/ovds/utils.py` & `ovds_utils-0.2.9/src/ovds_utils/ovds/utils.py`

 * *Files identical despite different names*

### Comparing `ovds_utils-0.2.8/src/ovds_utils/ovds/writing.py` & `ovds_utils-0.2.9/src/ovds_utils/ovds/writing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, AnyStr, Dict, List
 
 import numpy as np
 import openvds
 
+from .enums import InitValue
 from .utils import copy_ovds_metadata
 
 FORMAT2FLOAT = {
     openvds.VolumeDataChannelDescriptor.Format.Format_R64: np.float64,
     openvds.VolumeDataChannelDescriptor.Format.Format_R32: np.float32
 }
 
@@ -33,19 +34,38 @@
     accessor: openvds.core.VolumeDataPageAccessor,
     format: openvds.VolumeDataChannelDescriptor.Format
 ):
     dtype = FORMAT2FLOAT[format]
     for c in range(accessor.getChunkCount()):
         page = accessor.createPage(c)
         buf = np.array(page.getWritableBuffer(), copy=False, dtype=dtype)
-        buf[:, :, :] = np.full(buf.shape, np.nan)
+        buf[:, :, :] = np.full(buf.shape, np.nan, dtype=dtype)
         page.release()
     accessor.commit()
 
 
+def write_zero_pages(
+    accessor: openvds.core.VolumeDataPageAccessor,
+    format: openvds.VolumeDataChannelDescriptor.Format
+):
+    dtype = FORMAT2FLOAT[format]
+    for c in range(accessor.getChunkCount()):
+        page = accessor.createPage(c)
+        buf = np.array(page.getWritableBuffer(), copy=False, dtype=dtype)
+        buf[:, :, :] = np.zeros(buf.shape, dtype=dtype)
+        page.release()
+    accessor.commit()
+
+
+INITVALUE = {
+    InitValue.NaN: write_nan_pages,
+    InitValue.zero: write_zero_pages
+}
+
+
 def create_vds_attributes(
     databrick_size: openvds.core.VolumeDataLayoutDescriptor.BrickSize,
     metadata_dict: Dict[AnyStr, Any],
     lod_levels: openvds.VolumeDataLayoutDescriptor.LODLevels,
     options: openvds.VolumeDataLayoutDescriptor.Options,
     negative_margin: int,
     positive_margin: int,
@@ -104,14 +124,15 @@
     access_mode: openvds.IVolumeDataAccessManager.AccessMode,
     lod: openvds.VolumeDataLayoutDescriptor.LODLevels,
     options: int,
     brick_size_2d_multiplier: int,
     full_resolution_dimension: int,
     default_max_pages: int = 8,
     channels_data=None,
+    init_value: InitValue = InitValue.zero,
     close=True
 ):
     (
         layout_descriptor,
         axis_descriptors,
         channel_descriptors,
         metadata_container
@@ -171,12 +192,12 @@
             accessor = access_manager.createVolumeDataPageAccessor(
                 dimensionsND=channel.dimensions_nd.value,
                 accessMode=access_mode,
                 lod=lod,
                 channel=i,
                 maxPages=default_max_pages,
             )
-            write_nan_pages(accessor, channel.format.value)
+            INITVALUE[init_value](accessor, channel.format.value)
 
     if close:
         openvds.close(vds)
     return vds
```

### Comparing `ovds_utils-0.2.8/src/ovds_utils/vds.py` & `ovds_utils-0.2.9/src/ovds_utils/vds.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import numpy as np
 import openvds
 
 from ovds_utils.exceptions import VDSException
 from ovds_utils.logging import get_logger
 from ovds_utils.metadata import MetadataContainer
-from ovds_utils.ovds import LOD, AccessModes, BrickSizes, Components, Dimensions, Formats, Options, create_vds
+from ovds_utils.ovds import (LOD, AccessModes, BrickSizes, Components, Dimensions, Formats, InitValue, Options,
+                             create_vds)
 from ovds_utils.ovds.utils import get_vds_info
 from ovds_utils.ovds.writing import FORMAT2FLOAT
 
 logger = get_logger(__name__)
 
 
 class VDSChunk:
@@ -213,28 +214,29 @@
 
     def commit(self):
         self.accessor.commit()
 
 
 class VDS:
     def __init__(
-            self,
-            path: AnyStr,
-            connection_string: AnyStr = "",
-            databrick_size: BrickSizes = BrickSizes._128,
-            metadata_dict: MetadataContainer = {},
-            channels_data: List[np.array] = None,
-            channels: List[Channel] = None,
-            axes: List[Axis] = None,
-            lod=LOD._None,
-            negative_margin: int = 0,
-            positive_margin: int = 0,
-            options: Options = Options._None,
-            full_resolution_dimension: int = 0,
-            brick_size_2d_multiplier: int = 4,
+        self,
+        path: AnyStr,
+        connection_string: AnyStr = "",
+        databrick_size: BrickSizes = BrickSizes._128,
+        metadata_dict: MetadataContainer = {},
+        channels_data: List[np.array] = None,
+        channels: List[Channel] = None,
+        axes: List[Axis] = None,
+        lod: LOD = LOD._None,
+        negative_margin: int = 0,
+        positive_margin: int = 0,
+        options: Options = Options._None,
+        full_resolution_dimension: int = 0,
+        brick_size_2d_multiplier: int = 4,
+        init_value: InitValue = InitValue.zero
     ) -> None:
         super().__init__()
         self.path = path
         self.connection_string = connection_string
         self._channels = {}
         self._axes = {}
 
@@ -254,15 +256,16 @@
                     channels_data=channels_data,
                     access_mode=AccessModes.Create,
                     lod=lod,
                     positive_margin=positive_margin,
                     negagitve_margin=negative_margin,
                     options=options,
                     full_resolution_dimension=full_resolution_dimension,
-                    brick_size_2d_multiplier=brick_size_2d_multiplier
+                    brick_size_2d_multiplier=brick_size_2d_multiplier,
+                    init_value=init_value
                 )
                 self = self.__init__(
                     path=path,
                     connection_string=connection_string,
                     databrick_size=databrick_size,
                     metadata_dict=metadata_dict,
                 )
@@ -384,14 +387,15 @@
         axes: List[Axis],
         positive_margin: int,
         negagitve_margin: int,
         full_resolution_dimension: int,
         brick_size_2d_multiplier: int,
         lod: LOD,
         options: Options,
+        init_value: InitValue,
         metadata_dict: MetadataContainer = None,
         channels_data: List[np.array] = None,
     ):
         return create_vds(
             path=path,
             connection_string=connection_string,
             metadata_dict=metadata_dict,
@@ -402,14 +406,15 @@
             lod=lod.value,
             channels_data=channels_data,
             negative_margin=negagitve_margin,
             positive_margin=positive_margin,
             options=options.value,
             brick_size_2d_multiplier=brick_size_2d_multiplier,
             full_resolution_dimension=full_resolution_dimension,
+            init_value=init_value,
             close=True
         )
 
     @property
     def accessor(self):
         if self._accessor is None:
             raise VDSException("Accessor was not initialized use create_accessor method.")
```

### Comparing `ovds_utils-0.2.8/src/ovds_utils.egg-info/PKG-INFO` & `ovds_utils-0.2.9/src/ovds_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovds-utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utilities package for Open VDS.
 Home-page: https://github.com/micmurawski/ovds-utils/
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 License: MIT
 Description: # Introduction
```

