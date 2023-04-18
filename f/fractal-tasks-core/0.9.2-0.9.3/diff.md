# Comparing `tmp/fractal_tasks_core-0.9.2.tar.gz` & `tmp/fractal_tasks_core-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_tasks_core-0.9.2.tar", max compression
+gzip compressed data, was "fractal_tasks_core-0.9.3.tar", max compression
```

## Comparing `fractal_tasks_core-0.9.2.tar` & `fractal_tasks_core-0.9.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1584 2022-12-14 07:50:09.683341 fractal_tasks_core-0.9.2/LICENSE
--rw-r--r--   0        0        0     3697 2023-02-28 11:55:29.287745 fractal_tasks_core-0.9.2/README.md
--rw-r--r--   0        0        0       32 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/.gitignore
--rw-r--r--   0        0        0     3844 2023-04-11 14:35:05.288431 fractal_tasks_core-0.9.2/fractal_tasks_core/__FRACTAL_MANIFEST__.json
--rw-r--r--   0        0        0      165 2023-04-11 14:37:10.762595 fractal_tasks_core-0.9.2/fractal_tasks_core/__init__.py
--rw-r--r--   0        0        0     3005 2023-03-09 07:50:09.409308 fractal_tasks_core-0.9.2/fractal_tasks_core/_utils.py
--rw-r--r--   0        0        0    26138 2023-04-05 07:06:38.774355 fractal_tasks_core-0.9.2/fractal_tasks_core/cellpose_segmentation.py
--rw-r--r--   0        0        0     2543 2023-02-27 16:31:49.719523 fractal_tasks_core-0.9.2/fractal_tasks_core/compress_tif.py
--rw-r--r--   0        0        0     7687 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/copy_ome_zarr.py
--rw-r--r--   0        0        0    17556 2023-03-17 13:05:36.650239 fractal_tasks_core-0.9.2/fractal_tasks_core/create_ome_zarr.py
--rw-r--r--   0        0        0    19924 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/create_ome_zarr_multiplex.py
--rw-r--r--   0        0        0     9186 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/illumination_correction.py
--rw-r--r--   0        0        0    13467 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_ROI_overlaps.py
--rw-r--r--   0        0        0     8931 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_channels.py
--rw-r--r--   0        0        0     1403 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_glob.py
--rw-r--r--   0        0        0     9331 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_masked_loading.py
--rw-r--r--   0        0        0    12604 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_metadata_parsing.py
--rw-r--r--   0        0        0     3244 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_parse_filename_metadata.py
--rw-r--r--   0        0        0     3367 2023-01-17 14:38:05.370269 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_pyramid_creation.py
--rw-r--r--   0        0        0     3459 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_read_fractal_metadata.py
--rw-r--r--   0        0        0    12430 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_regions_of_interest.py
--rw-r--r--   0        0        0     7138 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_upscale_array.py
--rw-r--r--   0        0        0     3997 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.2/fractal_tasks_core/lib_zattrs_utils.py
--rw-r--r--   0        0        0     4658 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.2/fractal_tasks_core/maximum_intensity_projection.py
--rw-r--r--   0        0        0    24482 2023-04-05 07:07:32.849750 fractal_tasks_core-0.9.2/fractal_tasks_core/napari_workflows_wrapper.py
--rw-r--r--   0        0        0        0 2022-12-14 07:50:09.687341 fractal_tasks_core-0.9.2/fractal_tasks_core/tools/__init__.py
--rw-r--r--   0        0        0     3590 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.2/fractal_tasks_core/tools/lib_metadata_checks.py
--rw-r--r--   0        0        0     7262 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.2/fractal_tasks_core/yokogawa_to_ome_zarr.py
--rw-r--r--   0        0        0     2372 2023-04-11 14:37:10.762595 fractal_tasks_core-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     5056 1970-01-01 00:00:00.000000 fractal_tasks_core-0.9.2/setup.py
--rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 fractal_tasks_core-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1584 2022-12-14 07:50:09.683341 fractal_tasks_core-0.9.3/LICENSE
+-rw-r--r--   0        0        0     3697 2023-02-28 11:55:29.287745 fractal_tasks_core-0.9.3/README.md
+-rw-r--r--   0        0        0       32 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.3/fractal_tasks_core/.gitignore
+-rw-r--r--   0        0        0     3844 2023-04-11 14:35:05.288431 fractal_tasks_core-0.9.3/fractal_tasks_core/__FRACTAL_MANIFEST__.json
+-rw-r--r--   0        0        0      165 2023-04-18 13:46:50.733563 fractal_tasks_core-0.9.3/fractal_tasks_core/__init__.py
+-rw-r--r--   0        0        0     3005 2023-03-09 07:50:09.409308 fractal_tasks_core-0.9.3/fractal_tasks_core/_utils.py
+-rw-r--r--   0        0        0    26138 2023-04-18 12:48:15.162857 fractal_tasks_core-0.9.3/fractal_tasks_core/cellpose_segmentation.py
+-rw-r--r--   0        0        0     2543 2023-02-27 16:31:49.719523 fractal_tasks_core-0.9.3/fractal_tasks_core/compress_tif.py
+-rw-r--r--   0        0        0     7687 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.3/fractal_tasks_core/copy_ome_zarr.py
+-rw-r--r--   0        0        0    17556 2023-03-17 13:05:36.650239 fractal_tasks_core-0.9.3/fractal_tasks_core/create_ome_zarr.py
+-rw-r--r--   0        0        0    20156 2023-04-18 13:44:35.575251 fractal_tasks_core-0.9.3/fractal_tasks_core/create_ome_zarr_multiplex.py
+-rw-r--r--   0        0        0     9186 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.3/fractal_tasks_core/illumination_correction.py
+-rw-r--r--   0        0        0    13467 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_ROI_overlaps.py
+-rw-r--r--   0        0        0     8931 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_channels.py
+-rw-r--r--   0        0        0     1403 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_glob.py
+-rw-r--r--   0        0        0     9331 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_masked_loading.py
+-rw-r--r--   0        0        0    12604 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_metadata_parsing.py
+-rw-r--r--   0        0        0     3244 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_parse_filename_metadata.py
+-rw-r--r--   0        0        0     3367 2023-01-17 14:38:05.370269 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_pyramid_creation.py
+-rw-r--r--   0        0        0     3459 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_read_fractal_metadata.py
+-rw-r--r--   0        0        0    12616 2023-04-18 13:44:35.575251 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_regions_of_interest.py
+-rw-r--r--   0        0        0     7138 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_upscale_array.py
+-rw-r--r--   0        0        0     3997 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.3/fractal_tasks_core/lib_zattrs_utils.py
+-rw-r--r--   0        0        0     4658 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.3/fractal_tasks_core/maximum_intensity_projection.py
+-rw-r--r--   0        0        0    24663 2023-04-18 13:44:35.575251 fractal_tasks_core-0.9.3/fractal_tasks_core/napari_workflows_wrapper.py
+-rw-r--r--   0        0        0        0 2022-12-14 07:50:09.687341 fractal_tasks_core-0.9.3/fractal_tasks_core/tools/__init__.py
+-rw-r--r--   0        0        0     3590 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.3/fractal_tasks_core/tools/lib_metadata_checks.py
+-rw-r--r--   0        0        0     7262 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.3/fractal_tasks_core/yokogawa_to_ome_zarr.py
+-rw-r--r--   0        0        0     2372 2023-04-18 13:46:50.733563 fractal_tasks_core-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     5056 1970-01-01 00:00:00.000000 fractal_tasks_core-0.9.3/setup.py
+-rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 fractal_tasks_core-0.9.3/PKG-INFO
```

### Comparing `fractal_tasks_core-0.9.2/LICENSE` & `fractal_tasks_core-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/README.md` & `fractal_tasks_core-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/__FRACTAL_MANIFEST__.json` & `fractal_tasks_core-0.9.3/fractal_tasks_core/__FRACTAL_MANIFEST__.json`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/_utils.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/cellpose_segmentation.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/cellpose_segmentation.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/compress_tif.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/compress_tif.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/copy_ome_zarr.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/copy_ome_zarr.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/create_ome_zarr.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/create_ome_zarr.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/create_ome_zarr_multiplex.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/create_ome_zarr_multiplex.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,17 @@
         dict_acquisitions[acquisition] = {}
         dict_acquisitions[acquisition]["plate"] = plate
         dict_acquisitions[acquisition]["original_plate"] = original_plate
         dict_acquisitions[acquisition]["plate_prefix"] = plate_prefix
         dict_acquisitions[acquisition]["image_folder"] = in_path
         dict_acquisitions[acquisition]["original_paths"] = [in_path]
         dict_acquisitions[acquisition]["actual_channels"] = actual_channels
+        dict_acquisitions[acquisition][
+            "actual_wavelength_ids"
+        ] = actual_wavelength_ids
 
     acquisitions = sorted(list(dict_acquisitions.keys()))
     current_plates = [item["plate"] for item in dict_acquisitions.values()]
     if len(set(current_plates)) > 1:
         raise ValueError(f"{current_plates=}")
     plate = current_plates[0]
 
@@ -305,14 +308,17 @@
                     filename_metadata = parse_filename(os.path.basename(fpath))
                     A = filename_metadata["A"]
                     C = filename_metadata["C"]
                     well_wavelength_ids.append(f"A{A}_C{C}")
                 except IndexError:
                     logger.info(f"Skipping {fpath}")
             well_wavelength_ids = sorted(list(set(well_wavelength_ids)))
+            actual_wavelength_ids = dict_acquisitions[acquisition][
+                "actual_wavelength_ids"
+            ]
             if well_wavelength_ids != actual_wavelength_ids:
                 raise Exception(
                     f"ERROR: well {well} in plate {plate} (prefix: "
                     f"{plate_prefix}) has missing channels.\n"
                     f"Expected: {actual_wavelength_ids}\n"
                     f"Found: {well_wavelength_ids}.\n"
                 )
```

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/illumination_correction.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/illumination_correction.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_ROI_overlaps.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_ROI_overlaps.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_channels.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_channels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_glob.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_glob.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_masked_loading.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_masked_loading.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_metadata_parsing.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_metadata_parsing.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_parse_filename_metadata.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_parse_filename_metadata.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_pyramid_creation.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_pyramid_creation.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_read_fractal_metadata.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_read_fractal_metadata.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_regions_of_interest.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_regions_of_interest.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,17 @@
     Description
 
     FIXME add docstring
 
     :param dummy: this is just a placeholder
     :type dummy: int
     """
+    # Handle empty ROI table
+    if len(ROI) == 0:
+        return []
 
     # Set pyramid-level pixel sizes
     pxl_size_z, pxl_size_y, pxl_size_x = full_res_pxl_sizes_zyx
     prefactor = coarsening_xy**level
     pxl_size_x *= prefactor
     pxl_size_y *= prefactor
 
@@ -335,16 +338,19 @@
         "y_micrometer",
         "z_micrometer",
         "len_x_micrometer",
         "len_y_micrometer",
         "len_z_micrometer",
     ]
 
-    df = pd.DataFrame(np.array(elem_list), columns=df_columns)
-    df["label"] = labels
+    if len(elem_list) == 0:
+        df = pd.DataFrame(columns=[x for x in df_columns] + ["label"])
+    else:
+        df = pd.DataFrame(np.array(elem_list), columns=df_columns)
+        df["label"] = labels
 
     return df
 
 
 def is_ROI_table_valid(*, table_path: str, use_masks: bool) -> Optional[bool]:
     """
     Verify some validity assumptions on a ROI table
```

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_upscale_array.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_upscale_array.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/lib_zattrs_utils.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/lib_zattrs_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/maximum_intensity_projection.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/maximum_intensity_projection.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/napari_workflows_wrapper.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/napari_workflows_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,24 +554,28 @@
 
     # Output handling: "dataframe" type (for each output, concatenate ROI
     # dataframes, clean up, and store in a AnnData table on-disk)
     for (name, params) in dataframe_outputs:
         table_name = params["table_name"]
         # Concatenate all FOV dataframes
         list_dfs = output_dataframe_lists[name]
-        df_well = pd.concat(list_dfs, axis=0, ignore_index=True)
-        # Extract labels and drop them from df_well
-        labels = pd.DataFrame(df_well["label"].astype(str))
-        df_well.drop(labels=["label"], axis=1, inplace=True)
-        # Convert all to float (warning: some would be int, in principle)
-        measurement_dtype = np.float32
-        df_well = df_well.astype(measurement_dtype)
-        # Convert to anndata
-        measurement_table = ad.AnnData(df_well, dtype=measurement_dtype)
-        measurement_table.obs = labels
+        if len(list_dfs) == 0:
+            measurement_table = ad.AnnData()
+        else:
+            df_well = pd.concat(list_dfs, axis=0, ignore_index=True)
+            # Extract labels and drop them from df_well
+            labels = pd.DataFrame(df_well["label"].astype(str))
+            df_well.drop(labels=["label"], axis=1, inplace=True)
+            # Convert all to float (warning: some would be int, in principle)
+            measurement_dtype = np.float32
+            df_well = df_well.astype(measurement_dtype)
+            df_well.index = df_well.index.map(str)
+            # Convert to anndata
+            measurement_table = ad.AnnData(df_well, dtype=measurement_dtype)
+            measurement_table.obs = labels
         # Write to zarr group
         group_tables = zarr.group(f"{in_path}/{component}/tables/")
         write_elem(group_tables, table_name, measurement_table)
         # Update OME-NGFF metadata
         current_tables = group_tables.attrs.asdict().get("tables") or []
         if table_name in current_tables:
             # FIXME: move this check to an earlier stage of the task
```

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/tools/lib_metadata_checks.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/tools/lib_metadata_checks.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/fractal_tasks_core/yokogawa_to_ome_zarr.py` & `fractal_tasks_core-0.9.3/fractal_tasks_core/yokogawa_to_ome_zarr.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.2/pyproject.toml` & `fractal_tasks_core-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-tasks-core"
-version = "0.9.2"
+version = "0.9.3"
 description = ""
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Joel Lüthi  <joel.luethi@fmi.ch>",
 ]
@@ -75,15 +75,15 @@
 branch = true
 parallel = true
 relative_files = true
 source = ["fractal_tasks_core"]
 omit = ["tests/*", "examples/*"]
 
 [tool.bumpver]
-current_version = "0.9.2"
+current_version = "0.9.3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_tasks_core-0.9.2/setup.py` & `fractal_tasks_core-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'zarr>=2.13.6,<2.14.0']
 
 extras_require = \
 {'tools': ['matplotlib']}
 
 setup_kwargs = {
     'name': 'fractal-tasks-core',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': '',
     'long_description': '# Fractal Core Tasks\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-tasks-core?color=gree)](https://pypi.org/project/fractal-tasks-core/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-tasks-core/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-tasks-core/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![Documentation Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/documentation.yaml/badge.svg)](https://fractal-analytics-platform.github.io/fractal-tasks-core)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high-content imaging data at scale and prepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nFractal provides distributed workflows that convert TBs of image data into OME-Zarr files. The platform then processes the 3D image data by applying tasks like illumination correction, maximum intensity projection, 3D segmentation using [cellpose](https://cellpose.readthedocs.io/en/latest/) and measurements using [napari workflows](https://github.com/haesleinhuepf/napari-workflows). The pyramidal OME-Zarr files enable interactive visualization in the napari viewer.\n\nThis is the **core-tasks repository**, containing the python tasks that parse Yokogawa CV7000 images into OME-Zarr and process OME-Zarr files. Find more information about Fractal in general and the other repositories at the [Fractal home page](https://fractal-analytics-platform.github.io).\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-tasks-core\n\n\n## Available tasks\n\nCurrently, the following tasks are available:\n- Create Zarr Structure: Task to generate the zarr structure based on Yokogawa metadata files\n- Yokogawa to Zarr: Parses the Yokogawa CV7000 image data and saves it to the Zarr file\n- Illumination Correction: Applies an illumination correction based on a flatfield image & subtracts a background from the image.\n- Image Labeling (& Image Labeling Whole Well): Applies a cellpose network to the image of a single ROI or the whole well. cellpose parameters can be tuned for optimal performance.\n- Maximum Intensity Projection: Creates a maximum intensity projection of the whole plate.\n- Measurement: Make some standard measurements (intensity & morphology) using napari workflows, saving results to AnnData tables.\n\nSome additional tasks are currently being worked on and some older tasks are still present in the fractal_tasks_core folder.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-tasks-core',
```

### Comparing `fractal_tasks_core-0.9.2/PKG-INFO` & `fractal_tasks_core-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tasks-core
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Home-page: https://github.com/fractal-analytics-platform/fractal-tasks-core
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

