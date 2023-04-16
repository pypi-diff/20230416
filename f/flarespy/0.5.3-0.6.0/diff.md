# Comparing `tmp/flarespy-0.5.3.tar.gz` & `tmp/flarespy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.5.3.tar", max compression
+gzip compressed data, was "flarespy-0.6.0.tar", max compression
```

## Comparing `flarespy-0.5.3.tar` & `flarespy-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.5.3/LICENSE
--rw-r--r--   0        0        0      451 2023-04-16 08:24:19.082073 flarespy-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.5.3/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.5.3/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.5.3/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    25295 2023-04-16 09:57:21.426727 flarespy-0.5.3/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.5.3/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-16 07:27:47.598178 flarespy-0.5.3/src/flarespy/version.py
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 flarespy-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.6.0/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-16 16:38:22.310415 flarespy-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.6.0/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.6.0/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.6.0/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    25397 2023-04-16 16:37:37.272788 flarespy-0.6.0/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.6.0/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-16 16:38:11.870628 flarespy-0.6.0/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.6.0/PKG-INFO
```

### Comparing `flarespy-0.5.3/LICENSE` & `flarespy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.3/src/flarespy/Flare_model.py` & `flarespy-0.6.0/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.3/src/flarespy/data/model.dat` & `flarespy-0.6.0/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.3/src/flarespy/flarefinder.py` & `flarespy-0.6.0/src/flarespy/flarefinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,20 +237,20 @@
         coord = SkyCoord(self.ra, self.dec, unit="deg", frame="icrs", equinox="J2000")
         radius = u.Quantity(30, u.arcsec)
         try:
             self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS, dtype=object)
             gaia_dr3_data = Gaia.cone_search_async(coord, radius).get_results()
 
             self.stellar_parameters.gaia3_source_id = gaia_dr3_data["source_id"].data.data[0]
-            self.stellar_parameters.parallax = gaia_dr3_data["parallax"].data.data[0]
-            self.stellar_parameters.phot_g_mean_mag = gaia_dr3_data["phot_g_mean_mag"].data.data[0]
-            self.stellar_parameters.phot_bp_mean_mag = gaia_dr3_data["phot_bp_mean_mag"].data.data[0]
-            self.stellar_parameters.phot_rp_mean_mag = gaia_dr3_data["phot_rp_mean_mag"].data.data[0]
-            self.stellar_parameters.obs_duration = (
-                self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.standardized_flux.value))[0].size
+            self.stellar_parameters.parallax = np.round(gaia_dr3_data["parallax"].data.data[0], 4)
+            self.stellar_parameters.phot_g_mean_mag = np.round(gaia_dr3_data["phot_g_mean_mag"].data.data[0], 4)
+            self.stellar_parameters.phot_bp_mean_mag = np.round(gaia_dr3_data["phot_bp_mean_mag"].data.data[0], 4)
+            self.stellar_parameters.phot_rp_mean_mag = np.round(gaia_dr3_data["phot_rp_mean_mag"].data.data[0], 4)
+            self.stellar_parameters.obs_duration = np.round(
+                self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.standardized_flux.value))[0].size, 4
             )
 
         except IndexError:
             pass
 
         # Query TESS mag from TIC
         tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
@@ -381,17 +381,17 @@
                         i_peak = self.standardized_flux[i_start_ext_array[i] : i_stop_ext_array[i] + 1].argmax()
                         i_peak_array[i] += i_peak
 
                     self.candidates = pd.DataFrame(columns=CANDIDATES_COLUMNS)
                     self.candidates.i_start = i_start_ext_array
                     self.candidates.i_peak = i_peak_array
                     self.candidates.i_stop = i_stop_ext_array
-                    self.candidates.t_start = self.time.value[i_start_ext_array]
-                    self.candidates.t_peak = self.time.value[i_peak_array]
-                    self.candidates.t_stop = self.time.value[i_stop_ext_array]
+                    self.candidates.t_start = np.round(self.time.value[i_start_ext_array], 7)
+                    self.candidates.t_peak = np.round(self.time.value[i_peak_array], 7)
+                    self.candidates.t_stop = np.round(self.time.value[i_stop_ext_array], 7)
 
     def detect_sso(self):
         """Detect if the candidates are caused by SSO encounters."""
 
         if self.candidates is not None:
             sso = np.zeros(len(self.candidates), dtype=bool)
             for row in self.candidates.itertuples():
```

### Comparing `flarespy-0.5.3/src/flarespy/utils.py` & `flarespy-0.6.0/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.3/PKG-INFO` & `flarespy-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.5.3
+Version: 0.6.0
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -12,10 +12,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bottleneck (>=1.3)
 Requires-Dist: lightkurve (>=2.3)
 Requires-Dist: numba (>=0.55.2)
-Requires-Dist: scikit-learn (>=1.1)
 Requires-Dist: wotan (>=1.10)
 Project-URL: Repository, https://github.com/keyuxing/flarespy
```

