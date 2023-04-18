# Comparing `tmp/lndb_storage-0.2rc4.tar.gz` & `tmp/lndb_storage-0.2rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.2rc4.tar", last modified: Fri Apr 14 10:46:22 2023, max compression
+gzip compressed data, was "lndb_storage-0.2rc5.tar", last modified: Tue Apr 18 11:37:12 2023, max compression
```

## Comparing `lndb_storage-0.2rc4.tar` & `lndb_storage-0.2rc5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.2rc4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc4/.gitignore
--rw-r--r--   0        0        0     1758 2023-03-29 20:45:21.388537 lndb_storage-0.2rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc4/LICENSE
--rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc4/README.md
--rw-r--r--   0        0        0     2039 2023-04-14 10:46:01.815237 lndb_storage-0.2rc4/docs/changelog.md
--rw-r--r--   0        0        0     3283 2023-04-09 22:15:42.448966 lndb_storage-0.2rc4/docs/guide/add-replace-stage.ipynb
--rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc4/docs/guide/index.md
--rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc4/docs/guide/iris.csv
--rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc4/docs/guide/iris.data
--rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.2rc4/docs/guide/serialize-cache.ipynb
--rw-r--r--   0        0        0     7035 2023-04-09 22:14:23.875871 lndb_storage-0.2rc4/docs/guide/stream.ipynb
--rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.2rc4/docs/guide/upload.ipynb
--rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.2rc4/docs/index.md
--rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc4/docs/reference.md
--rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc4/lamin-project.yaml
--rw-r--r--   0        0        0      580 2023-04-14 10:45:33.547174 lndb_storage-0.2rc4/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3317 2023-04-14 10:44:40.713660 lndb_storage-0.2rc4/lndb_storage/_file.py
--rw-r--r--   0        0        0      497 2023-04-09 20:42:44.950134 lndb_storage-0.2rc4/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc4/lndb_storage/_images.py
--rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc4/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc4/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc4/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      950 2023-03-29 20:45:21.391028 lndb_storage-0.2rc4/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc4/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc4/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc4/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     3507 2023-04-09 20:42:44.950762 lndb_storage-0.2rc4/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      913 2023-04-09 22:16:03.478614 lndb_storage-0.2rc4/noxfile.py
--rw-r--r--   0        0        0     1044 2023-04-09 20:42:44.951084 lndb_storage-0.2rc4/pyproject.toml
--rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc4/tests/test_notebooks.py
--rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 lndb_storage-0.2rc4/PKG-INFO
+-rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.2rc5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc5/.gitignore
+-rw-r--r--   0        0        0     1758 2023-03-29 20:45:21.388537 lndb_storage-0.2rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc5/LICENSE
+-rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc5/README.md
+-rw-r--r--   0        0        0     2314 2023-04-18 11:36:46.449362 lndb_storage-0.2rc5/docs/changelog.md
+-rw-r--r--   0        0        0     4351 2023-04-16 20:58:33.197754 lndb_storage-0.2rc5/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc5/docs/guide/index.md
+-rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc5/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc5/docs/guide/iris.data
+-rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.2rc5/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     7032 2023-04-16 21:09:57.518313 lndb_storage-0.2rc5/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.2rc5/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.2rc5/docs/index.md
+-rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc5/docs/reference.md
+-rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc5/lamin-project.yaml
+-rw-r--r--   0        0        0      580 2023-04-18 11:36:25.922864 lndb_storage-0.2rc5/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.2rc5/lndb_storage/_file.py
+-rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.2rc5/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc5/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc5/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc5/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc5/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.2rc5/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc5/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc5/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc5/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     3507 2023-04-09 20:42:44.950762 lndb_storage-0.2rc5/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      913 2023-04-09 22:16:03.478614 lndb_storage-0.2rc5/noxfile.py
+-rw-r--r--   0        0        0     1064 2023-04-16 20:58:33.198898 lndb_storage-0.2rc5/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc5/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 lndb_storage-0.2rc5/PKG-INFO
```

### Comparing `lndb_storage-0.2rc4/.github/workflows/build.yml` & `lndb_storage-0.2rc5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/.github/workflows/latest-changes.yml` & `lndb_storage-0.2rc5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/.gitignore` & `lndb_storage-0.2rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/.pre-commit-config.yaml` & `lndb_storage-0.2rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/LICENSE` & `lndb_storage-0.2rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/docs/changelog.md` & `lndb_storage-0.2rc5/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✅ Check add with key | [20](https://github.com/laminlabs/lndb-storage/pull/20) | [Koncopd](https://github.com/Koncopd) | 2023-04-16 | 0.2rc5
+♻️ Refactoring | [19](https://github.com/laminlabs/lndb-storage/pull/19) | [Koncopd](https://github.com/Koncopd) | 2023-04-16 |
 ♻️ Remove call to nbproject in progress bar | [18](https://github.com/laminlabs/lndb-storage/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-04-14 | 0.2rc4
 ✅ Introduce separate upload guide | [14](https://github.com/laminlabs/lndb-storage/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 | 0.2rc3
 💚 Attempt fix CI | [12](https://github.com/laminlabs/lndb-storage/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 |
 🚚 Move `UPath` back to `lndb` | [11](https://github.com/laminlabs/lndb-storage/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 |
 ✅ Add test for replace and stage | [10](https://github.com/laminlabs/lndb-storage/pull/10) | [Koncopd](https://github.com/Koncopd) | 2023-04-04 |
 ➕ Add upath to deps | [9](https://github.com/laminlabs/lndb-storage/pull/9) | [Koncopd](https://github.com/Koncopd) | 2023-03-26 | 0.2rc2
 ➖ Remove lndb as explicit dependency | [7](https://github.com/laminlabs/lndb-storage/pull/7) | [Koncopd](https://github.com/Koncopd) | 2023-03-26 | 0.2rc1
```

### Comparing `lndb_storage-0.2rc4/docs/guide/add-replace-stage.ipynb` & `lndb_storage-0.2rc5/docs/guide/add-replace-stage.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9632936507936508%*

 * *Differences: {"'cells'": "{1: {'source': ['import lamindb as ln\\n', 'from lndb.dev.upath import UPath']}, 13: "*

 * *            "{'source': ['assert cache_data_path.stat().st_mtime >= "*

 * *            "cache_csv_path.stat().st_mtime']}, insert: [(15, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('id', 'bff43702'), ('metadata', OrderedDict()), ('source', ['## Add "*

 * *            "with `key`'])])), (16, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('id', '48d77993'), ('metadata', Ordered […]*

```diff
@@ -11,15 +11,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dca2c05d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb as ln"
+                "import lamindb as ln\n",
+                "from lndb.dev.upath import UPath"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1c5186af",
             "metadata": {},
@@ -131,26 +132,84 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c75115b2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert cache_data_path.stat().st_mtime > cache_csv_path.stat().st_mtime"
+                "assert cache_data_path.stat().st_mtime >= cache_csv_path.stat().st_mtime"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7273324a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.delete(file, delete_data_from_storage=True)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "bff43702",
+            "metadata": {},
+            "source": [
+                "## Add with `key`"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "48d77993",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "file = ln.File(\"iris.csv\", key=\"iris.csv\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4249829f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.add(file)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "7d7f97fe",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "key_path = UPath(\"s3://lamindb-ci/iris.csv\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "fb8790e5",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "assert key_path.exists()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ced86160",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.delete(file, delete_data_from_storage=True)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `lndb_storage-0.2rc4/docs/guide/iris.csv` & `lndb_storage-0.2rc5/docs/guide/iris.csv`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/docs/guide/iris.data` & `lndb_storage-0.2rc5/docs/guide/iris.data`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/docs/guide/serialize-cache.ipynb` & `lndb_storage-0.2rc5/docs/guide/serialize-cache.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/docs/guide/stream.ipynb` & `lndb_storage-0.2rc5/docs/guide/stream.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996212121212121%*

 * *Differences: {"'cells'": "{19: {'source': ['file = ln.select(ln.File, run_id=ln.context.run.id, "*

 * *            'suffix=".h5ad").one()\']}}'}*

```diff
@@ -163,15 +163,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "file = ln.select(ln.File, source_id=ln.context.run.id, suffix=\".h5ad\").one()"
+                "file = ln.select(ln.File, run_id=ln.context.run.id, suffix=\".h5ad\").one()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Next, we prepare the query strings to query the columns of `.obs` for each `AnnData` object. For details see the [pandas docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.query.html).\n",
```

### Comparing `lndb_storage-0.2rc4/docs/guide/upload.ipynb` & `lndb_storage-0.2rc5/docs/guide/upload.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/lndb_storage/__init__.py` & `lndb_storage-0.2rc5/lndb_storage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :toctree: .
 
    store_object
    store_png
    delete_storage
 """
 
-__version__ = "0.2rc4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.2rc5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 from lndb.dev.upath import UPath
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 
 from ._file import delete_storage, load_to_memory, store_object
 from ._h5ad import h5ad_to_anndata
 from ._images import store_png
```

### Comparing `lndb_storage-0.2rc4/lndb_storage/_file.py` & `lndb_storage-0.2rc5/lndb_storage/_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 from pathlib import Path
 from typing import Union
 
 import fsspec
 import pandas as pd
 import readfcs
+from lndb import settings
 from lndb.dev.upath import UPath
 
 from ._h5ad import read_adata_h5ad
 from ._zarr import read_adata_zarr
 
 READER_FUNCS = {
     ".csv": pd.read_csv,
@@ -40,16 +41,14 @@
 
 
 def store_object(localpath: Union[str, Path], storagekey: str) -> float:
     """Store arbitrary file to configured storage location.
 
     Returns size in bytes.
     """
-    from lndb import settings
-
     storagepath = settings.instance.storage.key_to_filepath(storagekey)
     localpath = Path(localpath)
 
     if localpath.is_file():
         size = localpath.stat().st_size
     else:
         size = sum(f.stat().st_size for f in localpath.rglob("*") if f.is_file())
@@ -57,31 +56,30 @@
     if isinstance(storagepath, UPath):
         if localpath.suffix != ".zarr":
             cb = ProgressCallback()
         else:
             # todo: make proper progress bar for zarr
             cb = fsspec.callbacks.NoOpCallback()
         storagepath.upload_from(localpath, recursive=True, callback=cb)
-    else:
+    else:  # storage path is local
+        storagepath.parent.mkdir(parents=True, exist_ok=True)
         if localpath.is_file():
             try:
                 shutil.copyfile(localpath, storagepath)
             except shutil.SameFileError:
                 pass
         else:
             if storagepath.exists():
                 shutil.rmtree(storagepath)
             shutil.copytree(localpath, storagepath)
     return float(size)  # because this is how we store in the db
 
 
 def delete_storage(storagekey: str):
     """Delete arbitrary file."""
-    from lndb import settings
-
     storagepath = settings.instance.storage.key_to_filepath(storagekey)
     if storagepath.is_file():
         storagepath.unlink()
     elif storagepath.is_dir():
         if isinstance(storagepath, UPath):
             storagepath.rmdir()
         else:
@@ -91,16 +89,14 @@
 
 
 def load_to_memory(filepath: Union[str, Path, UPath], stream: bool = False):
     """Load a file into memory.
 
     Returns the filepath if no in-memory form is found.
     """
-    from lndb import settings
-
     if isinstance(filepath, str):
         filepath = Path(filepath)
 
     if filepath.suffix == ".zarr":
         stream = True
     elif filepath.suffix != ".h5ad":
         stream = False
```

### Comparing `lndb_storage-0.2rc4/lndb_storage/_subset.py` & `lndb_storage-0.2rc5/lndb_storage/_subset.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/lndb_storage/_zarr.py` & `lndb_storage-0.2rc5/lndb_storage/_zarr.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/lndb_storage/object/_anndata.py` & `lndb_storage-0.2rc5/lndb_storage/object/_anndata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 from pathlib import Path
 
 from anndata import AnnData
 from lamin_logger import logger
+from lndb import settings
 from typeguard import typechecked
 
 
 @typechecked
 def anndata_to_h5ad(adata: AnnData, filekey: str) -> Path:
     """AnnData → h5ad."""
-    from lndb import settings
-
     path = settings.instance.storage.key_to_filepath(filekey)
     if settings.instance.storage.is_cloud:
         cache_file = settings.instance.storage.cloud_to_local_no_update(path)  # type: ignore  # noqa
         cache_file.parent.mkdir(exist_ok=True)
         logger.debug(f"Writing cache file: {cache_file}.")
         adata.write(cache_file)
         logger.debug("Uploading cache file.")
```

### Comparing `lndb_storage-0.2rc4/lndb_storage/object/_anndata_sizes.py` & `lndb_storage-0.2rc5/lndb_storage/object/_anndata_sizes.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/lndb_storage/object/_core.py` & `lndb_storage-0.2rc5/lndb_storage/object/_core.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/lndb_storage/object/_lazy_field.py` & `lndb_storage-0.2rc5/lndb_storage/object/_lazy_field.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/lndb_storage/object/_subset_anndata.py` & `lndb_storage-0.2rc5/lndb_storage/object/_subset_anndata.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/noxfile.py` & `lndb_storage-0.2rc5/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc4/pyproject.toml` & `lndb_storage-0.2rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [project]
 name = "lndb_storage"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     "lnschema_core",
+    "lndb>=0.41.0",
     "lamin_logger>=0.3.0",
     "nbproject",
     "readfcs",
     "python-dateutil",
     "anndata",
     "zarr",
     "boto3==1.24.59", # for aiobotocore inside s3fs, to fix deps resolution
```

### Comparing `lndb_storage-0.2rc4/PKG-INFO` & `lndb_storage-0.2rc5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: lndb_storage
-Version: 0.2rc4
+Version: 0.2rc5
 Summary: Storage → object.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core
+Requires-Dist: lndb>=0.41.0
 Requires-Dist: lamin_logger>=0.3.0
 Requires-Dist: nbproject
 Requires-Dist: readfcs
 Requires-Dist: python-dateutil
 Requires-Dist: anndata
 Requires-Dist: zarr
 Requires-Dist: boto3==1.24.59
```

