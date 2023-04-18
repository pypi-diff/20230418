# Comparing `tmp/zen3geo-0.5.0.tar.gz` & `tmp/zen3geo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen3geo-0.5.0.tar", max compression
+gzip compressed data, was "zen3geo-0.6.0.tar", max compression
```

## Comparing `zen3geo-0.5.0.tar` & `zen3geo-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     7652 2022-09-26 04:23:08.973391 zen3geo-0.5.0/LICENSE.md
--rw-r--r--   0        0        0      826 2022-09-26 04:23:08.973391 zen3geo-0.5.0/README.md
--rw-r--r--   0        0        0     2263 2022-09-26 04:24:06.781759 zen3geo-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      207 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/__init__.py
--rw-r--r--   0        0        0      950 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/__init__.py
--rw-r--r--   0        0        0    15153 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/datashader.py
--rw-r--r--   0        0        0     7162 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/geopandas.py
--rw-r--r--   0        0        0     3350 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/pyogrio.py
--rw-r--r--   0        0        0     3395 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/pystac.py
--rw-r--r--   0        0        0     5232 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/pystac_client.py
--rw-r--r--   0        0        0     2723 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/rioxarray.py
--rw-r--r--   0        0        0     7123 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/stackstac.py
--rw-r--r--   0        0        0     4177 2022-09-26 04:23:08.977392 zen3geo-0.5.0/zen3geo/datapipes/xbatcher.py
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 zen3geo-0.5.0/setup.py
--rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 zen3geo-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-04-18 01:40:28.438814 zen3geo-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0      826 2023-04-18 01:40:28.438814 zen3geo-0.6.0/README.md
+-rw-r--r--   0        0        0     2912 2023-04-18 01:40:51.284191 zen3geo-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/__init__.py
+-rw-r--r--   0        0        0     1050 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/__init__.py
+-rw-r--r--   0        0        0    15153 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/datashader.py
+-rw-r--r--   0        0        0     7162 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/geopandas.py
+-rw-r--r--   0        0        0     3350 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/pyogrio.py
+-rw-r--r--   0        0        0     3395 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/pystac.py
+-rw-r--r--   0        0        0     5232 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/pystac_client.py
+-rw-r--r--   0        0        0     2723 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/rioxarray.py
+-rw-r--r--   0        0        0     7123 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/stackstac.py
+-rw-r--r--   0        0        0     3899 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/xbatcher.py
+-rw-r--r--   0        0        0     5302 2023-04-18 01:40:28.442814 zen3geo-0.6.0/zen3geo/datapipes/xpystac.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 zen3geo-0.6.0/setup.py
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 zen3geo-0.6.0/PKG-INFO
```

### Comparing `zen3geo-0.5.0/LICENSE.md` & `zen3geo-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/README.md` & `zen3geo-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/pyproject.toml` & `zen3geo-0.6.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen3geo"
-version = "0.5.0"
+version = "0.6.0"
 description = "The 🌏 data science library you've been waiting for~"
 authors = ["Wei Ji <23487320+weiji14@users.noreply.github.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -12,39 +12,52 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Software Development :: Libraries",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 exclude = ["zen3geo/tests"]
 
+[tool.poetry.urls]
+"Homepage" = "https://github.com/weiji14/zen3geo/discussions"
+"Changelog" = "https://zen3geo.readthedocs.io/en/latest/changelog.html"
+"Documentation" = "https://zen3geo.readthedocs.io"
+"Download" = "https://anaconda.org/conda-forge/zen3geo"
+"Source Code" = "https://github.com/weiji14/zen3geo"
+"Sponsor" = "https://github.com/sponsors/weiji14"
+
 [tool.poetry.dependencies]
 # Required
-python = ">=3.8, <3.12"
+python = ">=3.8, <4.0"
 rioxarray = ">=0.10.0"
 torchdata = ">=0.4.0"
 # Optional
 datashader = {version = ">=0.14.0", optional = true}
 pyogrio = {version = ">=0.4.0", extras = ["geopandas"], optional = true}
 pystac = {version=">=1.4.0", optional=true}
 pystac-client = {version = ">=0.4.0", optional = true}
 spatialpandas = {version = ">=0.4.0", optional = true}
 stackstac = {version = ">=0.4.0", optional = true}
-xbatcher = {version = ">=0.1.0", optional = true}
+xbatcher = {version = ">=0.2.0", optional = true}
+xpystac = {version = ">=0.0.1", optional = true}
+zarr = {version = ">=2.13.0", optional = true}
 # Docs
 adlfs = {version = "*", optional = true}
 contextily = {version = "*", optional = true}
 graphviz = {version = "*", optional = true}
 jupyter-book = {version="*", optional=true}
 matplotlib = {version = "*", optional = true}
 planetary-computer = {version="*", optional=true}
+xarray-datatree = {version="*", optional=true}
 
 [tool.poetry.group.dev.dependencies]
+aiohttp = "*"
 black = "*"
 pytest = "*"
 
 [tool.poetry.extras]
 docs = [
     "adlfs",
     "contextily",
@@ -54,30 +67,37 @@
     "matplotlib",
     "planetary-computer",
     "pyogrio",
     "pystac",
     "pystac_client",
     "stackstac",
     "spatialpandas",
-    "xbatcher"
+    "xarray-datatree",
+    "xbatcher",
+    "xpystac",
+    "zarr"
+]
+raster = [
+    "xbatcher",
+    "zarr"
 ]
-raster = ["xbatcher"]
 spatial = [
     "datashader",
     "spatialpandas"
 ]
 stac = [
     "pystac",
     "pystac_client",
-    "stackstac"
+    "stackstac",
+    "xpystac"
 ]
 vector = ["pyogrio"]
 
 [tool.poetry-dynamic-versioning]
 bump = true
 enable = true
 metadata = false
 style = "pep440"
 
 [build-system]
-requires = ["poetry-core>=1.1.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.4.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/__init__.py` & `zen3geo-0.6.0/zen3geo/datapipes/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,7 +16,10 @@
 )
 from zen3geo.datapipes.rioxarray import RioXarrayReaderIterDataPipe as RioXarrayReader
 from zen3geo.datapipes.stackstac import (
     StackSTACMosaickerIterDataPipe as StackSTACMosaicker,
     StackSTACStackerIterDataPipe as StackSTACStacker,
 )
 from zen3geo.datapipes.xbatcher import XbatcherSlicerIterDataPipe as XbatcherSlicer
+from zen3geo.datapipes.xpystac import (
+    XpySTACAssetReaderIterDataPipe as XpySTACAssetReader,
+)
```

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/datashader.py` & `zen3geo-0.6.0/zen3geo/datapipes/datashader.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/geopandas.py` & `zen3geo-0.6.0/zen3geo/datapipes/geopandas.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/pyogrio.py` & `zen3geo-0.6.0/zen3geo/datapipes/pyogrio.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/pystac.py` & `zen3geo-0.6.0/zen3geo/datapipes/pystac.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/pystac_client.py` & `zen3geo-0.6.0/zen3geo/datapipes/pystac_client.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/rioxarray.py` & `zen3geo-0.6.0/zen3geo/datapipes/rioxarray.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/stackstac.py` & `zen3geo-0.6.0/zen3geo/datapipes/stackstac.py`

 * *Files identical despite different names*

### Comparing `zen3geo-0.5.0/zen3geo/datapipes/xbatcher.py` & `zen3geo-0.6.0/zen3geo/datapipes/xbatcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     input_dims : dict
         A dictionary specifying the size of the inputs in each dimension to
         slice along, e.g. ``{'lon': 64, 'lat': 64}``. These are the dimensions
         the machine learning library will see. All other dimensions will be
         stacked into one dimension called ``batch``.
 
     kwargs : Optional
-        Extra keyword arguments to pass to :py:func:`xbatcher.BatchGenerator`.
+        Extra keyword arguments to pass to :py:class:`xbatcher.BatchGenerator`.
 
     Yields
     ------
     chip : xarray.DataArray
         An :py:class:`xarray.DataArray` or :py:class:`xarray.Dataset` object
         containing the sliced raster data, with the size/shape defined by the
         ``input_dims`` parameter.
@@ -57,37 +57,42 @@
     >>> xbatcher = pytest.importorskip("xbatcher")
     ...
     >>> from torchdata.datapipes.iter import IterableWrapper
     >>> from zen3geo.datapipes import XbatcherSlicer
     ...
     >>> # Sliced window view of xarray.DataArray using DataPipe
     >>> dataarray: xr.DataArray = xr.DataArray(
-    ...     data=np.ones(shape=(3, 128, 128)),
+    ...     data=np.ones(shape=(3, 64, 64)),
     ...     name="foo",
     ...     dims=["band", "y", "x"]
     ... )
     >>> dp = IterableWrapper(iterable=[dataarray])
-    >>> dp_xbatcher = dp.slice_with_xbatcher(input_dims={"y": 64, "x": 64})
+    >>> dp_xbatcher = dp.slice_with_xbatcher(input_dims={"y": 2, "x": 2})
     ...
     >>> # Loop or iterate over the DataPipe stream
     >>> it = iter(dp_xbatcher)
     >>> dataarray_chip = next(it)
     >>> dataarray_chip
-    <xarray.Dataset>
-    Dimensions:  (band: 3, y: 64, x: 64)
+    <xarray.DataArray 'foo' (band: 3, y: 2, x: 2)>
+    array([[[1., 1.],
+            [1., 1.]],
+    <BLANKLINE>
+           [[1., 1.],
+            [1., 1.]],
+    <BLANKLINE>
+           [[1., 1.],
+            [1., 1.]]])
     Dimensions without coordinates: band, y, x
-    Data variables:
-        foo      (band, y, x) float64 1.0 1.0 1.0 1.0 1.0 ... 1.0 1.0 1.0 1.0 1.0
     """
 
     def __init__(
         self,
         source_datapipe: IterDataPipe[Union[xr.DataArray, xr.Dataset]],
         input_dims: Dict[Hashable, int],
-        **kwargs: Optional[Dict[str, Any]]
+        **kwargs: Optional[Dict[str, Any]],
     ) -> None:
         if xbatcher is None:
             raise ModuleNotFoundError(
                 "Package `xbatcher` is required to be installed to use this datapipe. "
                 "Please use `pip install xbatcher` "
                 "to install the package"
             )
@@ -95,21 +100,17 @@
             Union[xr.DataArray, xr.Dataset]
         ] = source_datapipe
         self.input_dims: Dict[Hashable, int] = input_dims
         self.kwargs = kwargs
 
     def __iter__(self) -> Iterator[Union[xr.DataArray, xr.Dataset]]:
         for dataarray in self.source_datapipe:
-            if hasattr(dataarray, "name") and dataarray.name is None:
-                # Workaround for ValueError: unable to convert unnamed
-                # DataArray to a Dataset without providing an explicit name
-                dataarray = dataarray.to_dataset(
-                    name=xr.backends.api.DATAARRAY_VARIABLE
-                )[xr.backends.api.DATAARRAY_VARIABLE]
-                # dataarray.name = "z"  # doesn't work for some reason
             for chip in dataarray.batch.generator(
                 input_dims=self.input_dims, **self.kwargs
             ):
                 yield chip
 
-    # def __len__(self) -> int:
-    #     return len(self.source_datapipe)
+    def __len__(self) -> int:
+        return sum(
+            len(dataarray.batch.generator(input_dims=self.input_dims, **self.kwargs))
+            for dataarray in self.source_datapipe
+        )
```

### Comparing `zen3geo-0.5.0/setup.py` & `zen3geo-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,38 +13,44 @@
 extras_require = \
 {'docs': ['datashader>=0.14.0',
           'pyogrio[geopandas]>=0.4.0',
           'pystac>=1.4.0',
           'pystac-client>=0.4.0',
           'spatialpandas>=0.4.0',
           'stackstac>=0.4.0',
-          'xbatcher>=0.1.0',
+          'xbatcher>=0.2.0',
+          'xpystac>=0.0.1',
+          'zarr>=2.13.0',
           'adlfs',
           'contextily',
           'graphviz',
           'jupyter-book',
           'matplotlib',
-          'planetary-computer'],
- 'raster': ['xbatcher>=0.1.0'],
+          'planetary-computer',
+          'xarray-datatree'],
+ 'raster': ['xbatcher>=0.2.0', 'zarr>=2.13.0'],
  'spatial': ['datashader>=0.14.0', 'spatialpandas>=0.4.0'],
- 'stac': ['pystac>=1.4.0', 'pystac-client>=0.4.0', 'stackstac>=0.4.0'],
+ 'stac': ['pystac>=1.4.0',
+          'pystac-client>=0.4.0',
+          'stackstac>=0.4.0',
+          'xpystac>=0.0.1'],
  'vector': ['pyogrio[geopandas]>=0.4.0']}
 
 setup_kwargs = {
     'name': 'zen3geo',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': "The 🌏 data science library you've been waiting for~",
     'long_description': "# zen3geo\n\nThe 🌏 data science library you've been waiting for~\n\n> 君の前前前世から僕は 君を探しはじめたよ\n>\n> Since your past life, I have been searching for you\n\n## 公案\n\n```\nGeography is difficult, but easy it can also be\nDeep Learning, you hope, has an answer to all\nToo this, too that, where to though, where to?\nLook out, sense within, and now you must know\n```\n\n## Installation\n\nTo install the development version from GitHub, do:\n\n    pip install git+https://github.com/weiji14/zen3geo.git\n\nOr the stable version from [PyPI](https://pypi.org/project/zen3geo):\n\n    pip install zen3geo\n\nIf instead, [conda-forge](https://anaconda.org/conda-forge/zen3geo) you desire:\n\n    mamba install --channel conda-forge zen3geo\n\nOther instructions, see https://zen3geo.readthedocs.io/en/latest/#installation\n",
     'author': 'Wei Ji',
     'author_email': '23487320+weiji14@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

