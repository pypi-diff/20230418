# Comparing `tmp/flarespy-0.7.0.tar.gz` & `tmp/flarespy-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.7.0.tar", max compression
+gzip compressed data, was "flarespy-0.7.1.tar", max compression
```

## Comparing `flarespy-0.7.0.tar` & `flarespy-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.7.0/LICENSE
--rw-r--r--   0        0        0      428 2023-04-17 15:29:28.993293 flarespy-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.7.0/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.7.0/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.7.0/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    26238 2023-04-17 15:29:29.004037 flarespy-0.7.0/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.7.0/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-17 15:29:28.999991 flarespy-0.7.0/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.7.1/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-18 03:41:22.442092 flarespy-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.7.1/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.7.1/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.7.1/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    26075 2023-04-18 03:36:13.927660 flarespy-0.7.1/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.7.1/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-18 03:41:22.445600 flarespy-0.7.1/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.7.1/PKG-INFO
```

### Comparing `flarespy-0.7.0/LICENSE` & `flarespy-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.0/src/flarespy/Flare_model.py` & `flarespy-0.7.1/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.0/src/flarespy/data/model.dat` & `flarespy-0.7.1/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.0/src/flarespy/flarefinder.py` & `flarespy-0.7.1/src/flarespy/flarefinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,47 +304,45 @@
 
         before = np.nonzero((time > t_start - window) & (time < t_start))[0]
         after = np.nonzero((time > t_stop) & (time < t_stop + window))[0]
 
         return False if (before.size and after.size) else True
 
     def query_stellar_parameters(self):
-        self.stellar_parameters = pd.Series(
-            data=np.full_like(STELLAR_PARAMETER_COLUMNS, np.nan), index=STELLAR_PARAMETER_COLUMNS, dtype=object
+        self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS)
+        self.stellar_parameters.obs_duration = np.round(
+            self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
         )
 
         # Query parallax from Gaia DR3
         coord = SkyCoord(self.ra, self.dec, unit="deg", frame="icrs", equinox="J2000")
-        radius = u.Quantity(5, u.arcmin)
+        radius = u.Quantity(1, u.arcmin)
 
         j = Gaia.cone_search_async(coord, radius)
         r = j.get_results()
 
         qr = QTable([r["ra"].filled(), r["dec"].filled(), r["pmra"].filled(0), r["pmdec"].filled(0)])
         coords_gaia = SkyCoord(
             qr["ra"], qr["dec"], pm_ra_cosdec=qr["pmra"], pm_dec=qr["pmdec"], frame="icrs", obstime=Time("J2016")
         )
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=ErfaWarning)
             coords_gaia_j2000 = coords_gaia.apply_space_motion(new_obstime=Time("J2000"))
         dist = coord.separation(coords_gaia_j2000).arcsec
 
-        if (dist < 8).any():
+        if (dist < 6).any():
             target_index = np.argmin(dist)
             self.stellar_parameters.gaia3_source_id = r["source_id"].data.data[target_index]
-            self.stellar_parameters.parallax = np.round(r["parallax"].data.data[target_index], 4)
+
+            plx = r["parallax"].data.data[target_index]
+            if plx > 0:
+                self.stellar_parameters.parallax = np.round(plx, 4)
             self.stellar_parameters.phot_g_mean_mag = np.round(r["phot_g_mean_mag"].data.data[target_index], 4)
             self.stellar_parameters.phot_bp_mean_mag = np.round(r["phot_bp_mean_mag"].data.data[target_index], 4)
             self.stellar_parameters.phot_rp_mean_mag = np.round(r["phot_rp_mean_mag"].data.data[target_index], 4)
-            self.stellar_parameters.obs_duration = np.round(
-                self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
-            )
-
-            if self.stellar_parameters.parallax < 0:
-                self.stellar_parameters.parallax = np.nan
 
         # Query TESS mag from TIC
         tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
         tic_data.add_index("ID")
         try:
             target_row = tic_data.loc[str(self.ticid)]
             self.stellar_parameters.tess_mag = target_row["Tmag"]
```

### Comparing `flarespy-0.7.0/src/flarespy/utils.py` & `flarespy-0.7.1/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.7.0/PKG-INFO` & `flarespy-0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.7.0
+Version: 0.7.1
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

