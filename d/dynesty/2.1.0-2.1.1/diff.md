# Comparing `tmp/dynesty-2.1.0.tar.gz` & `tmp/dynesty-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynesty-2.1.0.tar", last modified: Thu Feb  2 20:03:32 2023, max compression
+gzip compressed data, was "dynesty-2.1.1.tar", last modified: Sun Apr 16 02:01:46 2023, max compression
```

## Comparing `dynesty-2.1.0.tar` & `dynesty-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,50 @@
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-02-02 20:03:32.618404 dynesty-2.1.0/
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      850 2022-11-30 13:59:46.000000 dynesty-2.1.0/AUTHORS.md
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1166 2022-09-08 14:25:14.000000 dynesty-2.1.0/LICENSE
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       37 2022-09-08 14:25:14.000000 dynesty-2.1.0/MANIFEST.in
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     2954 2023-02-02 20:03:32.622403 dynesty-2.1.0/PKG-INFO
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     2176 2023-02-02 17:51:37.000000 dynesty-2.1.0/README.md
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-02-02 20:03:32.590403 dynesty-2.1.0/py/
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-02-02 20:03:32.618404 dynesty-2.1.0/py/dynesty/
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      361 2022-09-29 14:26:55.000000 dynesty-2.1.0/py/dynesty/__init__.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       22 2023-01-25 15:06:50.000000 dynesty-2.1.0/py/dynesty/_version.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    53481 2022-12-26 22:54:36.000000 dynesty-2.1.0/py/dynesty/bounding.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    93474 2022-12-26 22:54:36.000000 dynesty-2.1.0/py/dynesty/dynamicsampler.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    34242 2023-02-02 17:50:39.000000 dynesty-2.1.0/py/dynesty/dynesty.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    37160 2023-01-11 11:18:05.000000 dynesty-2.1.0/py/dynesty/nestedsamplers.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    90800 2022-11-10 12:41:27.000000 dynesty-2.1.0/py/dynesty/plotting.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     4846 2022-10-16 02:25:38.000000 dynesty-2.1.0/py/dynesty/pool.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      160 2022-09-29 14:26:55.000000 dynesty-2.1.0/py/dynesty/results.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    43788 2023-01-11 11:18:05.000000 dynesty-2.1.0/py/dynesty/sampler.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    40647 2022-10-04 16:28:59.000000 dynesty-2.1.0/py/dynesty/sampling.py
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    80191 2022-12-26 22:54:36.000000 dynesty-2.1.0/py/dynesty/utils.py
-drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-02-02 20:03:32.618404 dynesty-2.1.0/py/dynesty.egg-info/
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     2954 2023-02-02 20:03:32.000000 dynesty-2.1.0/py/dynesty.egg-info/PKG-INFO
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      473 2023-02-02 20:03:32.000000 dynesty-2.1.0/py/dynesty.egg-info/SOURCES.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)        1 2023-02-02 20:03:32.000000 dynesty-2.1.0/py/dynesty.egg-info/dependency_links.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)        8 2023-02-02 20:03:32.000000 dynesty-2.1.0/py/dynesty.egg-info/top_level.txt
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       67 2023-02-02 20:03:32.622403 dynesty-2.1.0/setup.cfg
--rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1841 2022-12-01 21:45:17.000000 dynesty-2.1.0/setup.py
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.530282 dynesty-2.1.1/
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      850 2022-12-02 00:57:09.000000 dynesty-2.1.1/AUTHORS.md
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1166 2022-12-02 00:56:46.000000 dynesty-2.1.1/LICENSE
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)       37 2022-12-02 00:56:46.000000 dynesty-2.1.1/MANIFEST.in
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     2954 2023-04-16 02:01:46.530282 dynesty-2.1.1/PKG-INFO
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     2176 2023-02-28 22:18:22.000000 dynesty-2.1.1/README.md
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.526282 dynesty-2.1.1/py/
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.526282 dynesty-2.1.1/py/dynesty/
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      361 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/__init__.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)       22 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/_version.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    53481 2022-12-26 20:42:45.000000 dynesty-2.1.1/py/dynesty/bounding.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    95151 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/dynamicsampler.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    34682 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/dynesty.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    37294 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/nestedsamplers.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    90800 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/plotting.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     4846 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/pool.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      160 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/results.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    43989 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/sampler.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    40647 2023-03-19 23:04:45.000000 dynesty-2.1.1/py/dynesty/sampling.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    80191 2023-04-15 16:30:55.000000 dynesty-2.1.1/py/dynesty/utils.py
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.526282 dynesty-2.1.1/py/dynesty.egg-info/
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     2954 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/PKG-INFO
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      939 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/SOURCES.txt
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)        1 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/dependency_links.txt
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)        8 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/top_level.txt
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)       67 2023-04-16 02:01:46.530282 dynesty-2.1.1/setup.cfg
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1841 2022-12-02 00:57:09.000000 dynesty-2.1.1/setup.py
+drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.530282 dynesty-2.1.1/tests/
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     5309 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_blob.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1112 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_dyn.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1875 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_egg.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     8684 2022-12-02 00:57:09.000000 dynesty-2.1.1/tests/test_ellipsoid.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    13016 2023-03-16 20:38:54.000000 dynesty-2.1.1/tests/test_gau.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     4205 2023-04-16 00:32:09.000000 dynesty-2.1.1/tests/test_highdim.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)    24687 2023-04-15 23:00:14.000000 dynesty-2.1.1/tests/test_misc.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     5644 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_ncdim.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)      944 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_notebooks.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1520 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_pathology.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     2709 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_periodic.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     9343 2023-04-15 23:00:08.000000 dynesty-2.1.1/tests/test_plateau.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     6161 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_plot.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     6382 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_pool.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1872 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_printing.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1967 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_reflect.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     6629 2023-04-15 23:00:14.000000 dynesty-2.1.1/tests/test_resume.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     3503 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_rosenbrock.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     3633 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_sampling.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     1570 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_saver.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     6187 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_volume.py
+-rw-rw-r--   0 koposov   (1000) koposov   (1000)     2420 2022-12-14 13:10:24.000000 dynesty-2.1.1/tests/test_wedding.py
```

### Comparing `dynesty-2.1.0/AUTHORS.md` & `dynesty-2.1.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/LICENSE` & `dynesty-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/PKG-INFO` & `dynesty-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynesty
-Version: 2.1.0
+Version: 2.1.1
 Summary: A dynamic nested sampling package for computing Bayesian posteriors and evidences.
 Home-page: https://github.com/joshspeagle/dynesty
 Author: Joshua S Speagle, Sergey E Koposov
 Author-email: j.speagle@utoronto.ca
 License: MIT
 Keywords: nested sampling,dynamic,monte carlo,bayesian,inference,modeling
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dynesty-2.1.0/README.md` & `dynesty-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/py/dynesty/bounding.py` & `dynesty-2.1.1/py/dynesty/bounding.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/py/dynesty/dynamicsampler.py` & `dynesty-2.1.1/py/dynesty/dynamicsampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,36 +48,47 @@
     LIVEPOINTSINIT = 2  # after generating livepoints
     INBASE = 3  # during base runs
     BASE_DONE = 4  # base run done
     INBATCH = 5  # after at least one batch
     BATCH_DONE = 6  # after at least one batch
     INBASEADDLIVE = 7  # during addition of livepoints in the
     INBATCHADDLIVE = 8  # during addition of livepoints in the
+    RUN_DONE = 9  # The run has ended
     # end of the base run
 
 
 def compute_weights(results):
     """ Derive evidence and posterior weights.
     return two arrays, evidence weights and posterior weights
     """
     logl = results.logl
     logz = results.logz  # final ln(evidence)
     logvol = results.logvol
     logwt = results.logwt
     samples_n = results.samples_n
 
-    # TODO the logic here needs to be verified
-    logz_remain = logl[-1] + logvol[-1]  # remainder
-    logz_tot = np.logaddexp(logz[-1], logz_remain)  # estimated upper bound
-    lzones = np.ones_like(logz)
-    logzin = logsumexp([lzones * logz_tot, logz], axis=0,
-                       b=[lzones, -lzones])  # ln(remaining evidence)
-    logzweight = logzin - np.log(samples_n)  # ln(evidence weight)
-    logzweight -= logsumexp(logzweight)  # normalize
-    zweight = np.exp(logzweight)  # convert to linear scale
+    if logz.ptp() == 0:
+        # this pathological case can happen if all logl are very small
+        # and all logz are very small and the same
+        # then the calculation below failse
+        warnings.warn('''The calculation of weights is seeing same
+logz values associated with all the samples. It may mean somethings is
+wrong with your likelihood.''')
+        zweight = np.ones(len(logl)) / len(logl)
+    else:
+        # TODO the logic here needs to be verified
+        logz_remain = logl[-1] + logvol[-1]  # remainder
+        logz_tot = np.logaddexp(logz[-1], logz_remain)  # estimated upper bound
+        lzones = np.ones_like(logz)
+        logzin = logsumexp([lzones * logz_tot, logz],
+                           axis=0,
+                           b=[lzones, -lzones])  # ln(remaining evidence)
+        logzweight = logzin - np.log(samples_n)  # ln(evidence weight)
+        logzweight -= logsumexp(logzweight)  # normalize
+        zweight = np.exp(logzweight)  # convert to linear scale
 
     # Derive posterior weights.
     pweight = np.exp(logwt - logz[-1])  # importance weight
     pweight /= np.sum(pweight)  # normalize
     return zweight, pweight
 
 
@@ -162,16 +173,16 @@
     else:
         logl_min, logl_max = logl[bounds[0]], logl[bounds[1]]
 
     if bounds[1] == nsamps - 1:
         logl_max = np.inf
     if return_weights:
         return (logl_min, logl_max), (pweight, zweight, weight)
-    else:
-        return (logl_min, logl_max)
+
+    return (logl_min, logl_max)
 
 
 def _get_update_interval_ratio(update_interval, sample, bound, ndim, nlive,
                                slices, walks):
     """
     Get the update_interval divided by the number of live points
     """
@@ -387,67 +398,81 @@
     """
     logvol_init = 0
     ncalls = 0
     if live_points is None:
         # If no live points are provided, propose them by randomly
         # sampling from the unit cube.
         n_attempts = 1000
-        min_npoints = max(npdim, 10)
+
+        min_npoints = min(nlive, max(npdim + 1, 10))
         # the minimum number points we want with finite logl
-        # we want want at least npdim, because we wanto be able to constraint
+        # we want want at least npdim+1, because we wanto be able to constraint
         # the ellipsoid
-        # and we do not accept below 10 pts, because the volume error
-        # will be large
+        # Note that if nlive <npdim+ 1 this doesn't really make sense
+        # but we should have warned the user earlier, so they are on their own
+        # And the reason we have max(npdim+1, 10) is that we'd like to get at
+        # least 10 points as otherwise the poisson estimate of the volume will
+        # be too large.
+
         live_u = np.zeros((nlive, npdim))
         live_v = np.zeros((nlive, npdim))
         live_logl = np.zeros(nlive)
-        ngoods = 0
+        ngoods = 0  # counter for how many finite logl we have found
         live_blobs = []
-        for iattempt in range(1, n_attempts + 1):
+        iattempt = 0
+        while True:
+            iattempt += 1
+
+            # simulate nlive points by uniform sampling
             cur_live_u = rstate.random(size=(nlive, npdim))
             if use_pool_ptform:
                 cur_live_v = M(prior_transform, np.asarray(cur_live_u))
             else:
                 cur_live_v = map(prior_transform, np.asarray(cur_live_u))
             cur_live_v = np.array(list(cur_live_v))
             cur_live_logl = loglikelihood.map(np.asarray(cur_live_v))
             if blob:
                 cur_live_blobs = np.array([_.blob for _ in cur_live_logl])
             cur_live_logl = np.array([_.val for _ in cur_live_logl])
             ncalls += nlive
+
             # Convert all `-np.inf` log-likelihoods to finite large
             # numbers. Necessary to keep estimators in our sampler from
             # breaking.
             finite = np.isfinite(cur_live_logl)
             not_finite = ~finite
             neg_infinite = np.isneginf(cur_live_logl)
             if np.any(not_finite & (~neg_infinite)):
                 raise ValueError("The log-likelihood of live "
                                  "point is invalid.")
             cur_live_logl[not_finite] = _LOWL_VAL
 
+            # how many finite logl values we have
             cur_ngood = finite.sum()
             if cur_ngood > 0:
+                # append them to our list
                 nextra = min(nlive - ngoods, cur_ngood)
+                assert nextra >= 0
                 cur_ind = np.nonzero(finite)[0][:nextra]
                 live_logl[ngoods:ngoods + nextra] = cur_live_logl[cur_ind]
                 live_u[ngoods:ngoods + nextra] = cur_live_u[cur_ind]
                 live_v[ngoods:ngoods + nextra] = cur_live_v[cur_ind]
                 if blob:
                     live_blobs.extend(cur_live_blobs[cur_ind])
                 ngoods += nextra
-            # Check to make sure there are enough finite
-            # log-likelihood value within the initial set of live
-            # points.
-            if ngoods > min_npoints:
+
+            # Check if we have more than the minimum required number
+            # after that we will stop
+            if ngoods >= min_npoints:
                 # we need to fill the rest with points with
                 # not finite logl
                 nextra = nlive - ngoods
                 if nextra > 0:
                     cur_ind = np.nonzero(not_finite)[0][:nextra]
+                    assert len(cur_ind) == nextra
                     live_logl[ngoods:ngoods + nextra] = cur_live_logl[cur_ind]
                     live_u[ngoods:ngoods + nextra] = cur_live_u[cur_ind]
                     live_v[ngoods:ngoods + nextra] = cur_live_v[cur_ind]
                     if blob:
                         live_blobs.extend(cur_live_blobs[cur_ind])
                 logvol_init = -np.log(iattempt)
                 # The logic is the following:
@@ -456,21 +481,30 @@
                 # then the volume associated with pts above LOWL_VAL
                 # can be estimated as k/(Nn)
                 # the rest of the points have 1/Nn volume per pt
                 # Since we quit with k points above LOWL_VAL and
                 # (n-k)  LOWL points
                 # The volume is k/(Nn) + (n-k)/(Nn) = 1/N
                 break
-        else:
-            # If we found nothing after many attempts, raise the alarm.
-            raise RuntimeError(f"After {n_attempts} attempts, we cound not "
-                               f"find at least {min_npoints} points"
-                               "that have a valid log-likelihood! Please "
-                               "check your prior transform and/or "
-                               "log-likelihood.")
+            if iattempt == n_attempts:
+                if ngoods == 0:
+                    # If we found nothing after many attempts, raise the alarm.
+                    raise RuntimeError(
+                        f"After {n_attempts} attempts, we cound not "
+                        "find a single point "
+                        "that have a valid log-likelihood! Please "
+                        "check your prior transform and/or "
+                        "log-likelihood.")
+                else:
+                    # If we found nothing after many attempts, raise the alarm.
+                    warnings.warn(f"After {n_attempts} attempts, we cound not "
+                                  f"find at least {min_npoints} points "
+                                  "that have a valid log-likelihood! "
+                                  "The initial sampling is very inefficient!")
+
     else:
         # If live points were provided, convert the log-likelihoods and
         # then run a quick safety check.
         live_u, live_v, live_logl = live_points[:3]
         if blob:
             live_blobs = live_points[3]
         live_logl = np.asarray(live_logl)
@@ -482,15 +516,15 @@
                     raise ValueError("The log-likelihood ({0}) of live "
                                      "point {1} located at u={2} v={3} "
                                      " is invalid.".format(
                                          logl, i, live_u[i], live_v[i]))
         if np.all(live_logl == _LOWL_VAL):
             raise ValueError("Not a single provided live point has a "
                              "valid log-likelihood!")
-    if (np.ptp(live_logl) == 0):
+    if np.ptp(live_logl) == 0:
         warnings.warn(
             'All the initial likelihood values are the same. '
             'You likely have a plateau in the likelihood. '
             'Nested sampling may not be the best sampler in this case.',
             RuntimeWarning)
     if not blob:
         live_blobs = None
@@ -581,14 +615,15 @@
         main_sampler.queue_size,
         main_sampler.pool,
         main_sampler.use_pool,
         ncdim=main_sampler.ncdim,
         kwargs=main_sampler.kwargs,
         blob=main_sampler.blob)
     batch_sampler.save_bounds = save_bounds
+    batch_sampler.logl_first_update = main_sampler.sampler.logl_first_update
 
     # Initialize ln(likelihood) bounds.
     if logl_bounds is None:
         # the reason we set logl_max to not the highest logl
         # is because the last few points are always added in the end
         # without sampling through add_live_points()
         # so here I pick up the first point where the volume is
@@ -637,14 +672,17 @@
                                     vstar=live_v[i],
                                     loglstar=live_logl[i],
                                     nc=1,
                                     worst_it=live_it[i] + main_sampler.it,
                                     boundidx=0,
                                     bounditer=0,
                                     eff=main_sampler.eff))
+        batch_sampler.update_bound_if_needed(logl_min)
+        # Trigger an update of the internal bounding distribution based
+        # on the "new" set of live points.
     else:
         # If the lower bound doesn't encompass all base samples,
         # we need to create a uniform sample from the prior subject
         # to the likelihood boundary constraint
 
         subset0 = np.nonzero(saved_logl > logl_min)[0]
 
@@ -723,23 +761,19 @@
         # and scale factor.
         batch_sampler.nlive = cur_nlive
         batch_sampler.live_u = live_u
         batch_sampler.live_v = live_v
         batch_sampler.live_logl = live_logl
         batch_sampler.scale = live_scale
         batch_sampler.live_blobs = live_blobs
+
+        batch_sampler.update_bound_if_needed(logl_min)
         # Trigger an update of the internal bounding distribution based
         # on the "new" set of live points.
 
-        bound = batch_sampler.update()
-        if save_bounds:
-            batch_sampler.bound.append(copy.deepcopy(bound))
-        batch_sampler.nbound += 1
-        batch_sampler.since_update = 0
-        batch_sampler.logl_first_update = logl_min
         live_u = np.empty((nlive_new, main_sampler.npdim))
         live_v = np.empty((nlive_new, saved_v.shape[1]))
         live_logl = np.empty(nlive_new)
         live_bound = np.zeros(nlive_new, dtype=int)
         live_it = np.zeros(nlive_new, dtype=int)
 
         live_nc = np.empty(nlive_new, dtype=int)
@@ -785,23 +819,15 @@
     batch_sampler.live_u = live_u
     batch_sampler.live_v = live_v
     batch_sampler.live_logl = live_logl
     batch_sampler.live_bound = live_bound
     batch_sampler.live_blobs = live_blobs
     batch_sampler.live_it = live_it
 
-    # Trigger an update of the internal bounding distribution
-    if not psel:
-        bound = batch_sampler.update()
-        if save_bounds:
-            batch_sampler.bound.append(copy.deepcopy(bound))
-        batch_sampler.nbound += 1
-        batch_sampler.since_update = 0
-        batch_sampler.logl_first_update = logl_min
-    else:
+    if psel:
         batch_sampler.logvol_init = logvol0
 
     # Figure out where the new run would would join the previous run
     if logl_min == -np.inf:
         vol_idx = 0
     else:
         vol_idx = np.argmin(np.abs(saved_logl - logl_min)) + 1
@@ -1536,15 +1562,15 @@
             it0 = batch_sampler.it0
             logl_min, logl_max = self.new_logl_min, self.new_logl_max
             maxcall_left = maxcall
             maxiter_left = maxiter
             # I have decided that maxcall/maxiter_left will not be preserved
             # if interrupted and resumed
 
-        for i in range(len(batch_sampler.first_points)):
+        for _ in range(len(batch_sampler.first_points)):
             yield batch_sampler.first_points.pop(0)
             # these yields are just for printing
             # we are not actually storing those in new_run
             # because we're not sampling yet, we've just
             # set up nlive_new points above our logl_min boundary
             # The reason why I'm popping the items is to ensure if we
             # are interrupted and then resume we don't start again
@@ -1997,14 +2023,19 @@
         ncall = self.ncall
 
         niter = self.it - 1
         logl_bounds = (-np.inf, np.inf)
         maxcall_init = min(maxcall_init, maxcall)  # set max calls
         maxiter_init = min(maxiter_init, maxiter)  # set max iterations
 
+        if resume and self.internal_state == DynamicSamplerStatesEnum.RUN_DONE:
+            warnings.warn(
+                """You tried to resume the run that has ended successfully.
+This is not supported. No sampling was performed""", RuntimeWarning)
+            return
         # Baseline run.
         pbar, print_func = get_print_func(print_func, print_progress)
         timer = DelayTimer(checkpoint_every)
         try:
             if not self.base:
                 for results in self.sample_initial(
                         nlive=nlive_init,
@@ -2085,14 +2116,15 @@
                                    stop_val=stop_val,
                                    logl_min=logl_bounds[0],
                                    logl_max=logl_bounds[1])
                     break
                 else:
                     # We didn't run a single batch but now we're done!
                     break
+            self.internal_state = DynamicSamplerStatesEnum.RUN_DONE
             if checkpoint_file is not None:
                 # In the very end I save the checkpoint no matter
                 # the timing
                 self.save(checkpoint_file)
         finally:
             if pbar is not None:
                 pbar.close()
@@ -2266,14 +2298,16 @@
                                    ncall,
                                    nbatch=n + 1,
                                    stop_val=stop_val,
                                    logl_min=logl_min,
                                    logl_max=logl_max)
                     if (checkpoint_file is not None and self.internal_state !=
                             DynamicSamplerStatesEnum.INBATCHADDLIVE
+                            and self.internal_state !=
+                            DynamicSamplerStatesEnum.BATCH_DONE
                             and timer.is_time()):
                         # we do not save the state if we are finishing the
                         # batch run and we are just adding live-points in
                         # the end
                         self.save(checkpoint_file)
             finally:
                 if pbar is not None:
```

### Comparing `dynesty-2.1.0/py/dynesty/dynesty.py` & `dynesty-2.1.1/py/dynesty/dynesty.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,17 @@
 
     def reflist_tostring(x):
         """ internal function to convert reference lists to
         a printable string
         """
         if isinstance(x, str):
             return x
-        elif isinstance(x, tuple):
+        if isinstance(x, tuple):
             return x[0] + ': ' + x[1]
-        elif isinstance(x, list):
+        if isinstance(x, list):
             return '\n'.join([_[0] + ': ' + _[1] for _ in x])
         else:
             return str(x)
 
     default_citations = reflist_tostring(default_refs)
     nested_citations = reflist_tostring(nested_refs)
     # if using a custom sampler, dynesty does not know the citations
@@ -212,14 +212,24 @@
                                  "explicitly.") from e
     else:
         raise ValueError("`queue_size > 1` but no `pool` provided.")
 
     return M, queue_size
 
 
+def _check_first_update(first_update):
+    """
+    Verify that the first_update dictionary is valid
+    Specifically that it doesn't have unrecognized keywords
+    """
+    for k in first_update.keys():
+        if k not in ['min_ncall', 'min_eff']:
+            raise ValueError('Unrecognized keywords in first_update')
+
+
 def _assemble_sampler_docstring(dynamic):
     """
     Assemble the docstring for the NestedSampler and DynamicNestedSampler
     We do that to avoid duplicating the parameter descriptions
     """
     common = """
         Parameters
@@ -579,14 +589,16 @@
         kwargs['nonbounded'] = nonbounded
         kwargs['periodic'] = periodic
         kwargs['reflective'] = reflective
 
         # Keyword arguments controlling the first update.
         if first_update is None:
             first_update = {}
+        else:
+            _check_first_update(first_update)
 
         # Random state.
         if rstate is None:
             rstate = get_random_generator()
 
         # Log-likelihood.
         if logl_args is None:
@@ -759,15 +771,15 @@
 
         walks, slices = _get_walks_slices(walks, slices, sample, ndim)
 
         if ncdim != npdim and sample in ['slice', 'hslice', 'rslice']:
             raise ValueError('ncdim unsupported for slice sampling')
 
         update_interval_ratio = _get_update_interval_ratio(
-            update_interval, sample, bound, ndim, 1, slices, walks)
+            update_interval, sample, bound, ndim, nlive, slices, walks)
 
         kwargs = {}
 
         # Custom sampling function.
         if sample not in _SAMPLING and not callable(sample):
             raise ValueError(f"Unknown sampling method: {sample}")
 
@@ -783,14 +795,16 @@
         kwargs['nonbounded'] = nonbounded
         kwargs['periodic'] = periodic
         kwargs['reflective'] = reflective
         kwargs['blob'] = blob
         # Keyword arguments controlling the first update.
         if first_update is None:
             first_update = {}
+        else:
+            _check_first_update(first_update)
 
         # Random state.
         if rstate is None:
             rstate = get_random_generator()
 
         # Log-likelihood.
         if logl_args is None:
```

### Comparing `dynesty-2.1.0/py/dynesty/nestedsamplers.py` & `dynesty-2.1.1/py/dynesty/nestedsamplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,15 +491,19 @@
                          pool,
                          use_pool,
                          ncdim=ncdim,
                          blob=blob,
                          logvol_init=logvol_init,
                          kwargs=kwargs or {})
 
-        self.ell = Ellipsoid(np.zeros(self.ncdim), np.identity(self.ncdim))
+        self.ell = Ellipsoid(
+            np.zeros(self.ncdim) + .5,
+            np.identity(self.ncdim) * self.ncdim / 4)
+        # this is ellipsoid in the center of the cube that contains
+        # the whole cube
         self.bounding = 'single'
 
     def update(self, subset=slice(None)):
         """Update the bounding ellipsoid using the current set of
         live points."""
 
         # Check if we should use the provided pool for updating.
@@ -652,16 +656,19 @@
                          pool,
                          use_pool,
                          ncdim=ncdim,
                          blob=blob,
                          logvol_init=logvol_init,
                          kwargs=kwargs or {})
 
-        self.mell = MultiEllipsoid(ctrs=[np.zeros(self.ncdim)],
-                                   covs=[np.identity(self.ncdim)])
+        self.mell = MultiEllipsoid(
+            ctrs=[np.zeros(self.ncdim) + .5],
+            covs=[np.identity(self.ncdim) * self.ncdim / 4])
+        # this is ellipsoid in the center of the cube that contains
+        # the whole cube
         self.bounding = 'multi'
 
     def update(self, subset=slice(None)):
         """Update the bounding ellipsoids using the current set of
         live points."""
 
         # Check if we should use the pool for updating.
@@ -723,20 +730,15 @@
         # Copy a random live point.
         u = self.live_u[i, :]
         u_fit = u[:self.ncdim]
 
         # Automatically trigger an update if we're not in any ellipsoid.
         if not self.mell.contains(u_fit):
             # Update the bounding ellipsoids.
-            bound = self.update()
-            if self.save_bounds:
-                self.bound.append(bound)
-            self.nbound += 1
-            self.since_update = 0
-
+            self.update_bound_if_needed(-np.inf, force=True)
             # Check for ellipsoid overlap (again).
             if not self.mell.contains(u_fit):
                 raise RuntimeError('Update of the ellipsoid failed')
 
         if self.sampling in ['rwalk', 'rslice', 'slice']:
             # Pick a random ellipsoid (not necessarily the one that contains u)
             # This a crucial step as we must choose a random ellipsoid,
```

### Comparing `dynesty-2.1.0/py/dynesty/plotting.py` & `dynesty-2.1.1/py/dynesty/plotting.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/py/dynesty/pool.py` & `dynesty-2.1.1/py/dynesty/pool.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/py/dynesty/sampler.py` & `dynesty-2.1.1/py/dynesty/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,20 +95,14 @@
             self.live_blobs = live_points[3]
         else:
             self.live_blobs = None
         self.nlive = len(self.live_u)
         self.live_bound = np.zeros(self.nlive, dtype=int)
         self.live_it = np.zeros(self.nlive, dtype=int)
 
-        # bounding updates
-        self.update_interval = update_interval
-        self.ubound_ncall = first_update.get('min_ncall', 2 * self.nlive)
-        self.ubound_eff = first_update.get('min_eff', 10.)
-        self.logl_first_update = None
-
         # random state
         self.rstate = rstate
 
         # set to none just for qa
         self.scale = None
         self.method = None
         self.kwargs = {}
@@ -131,25 +125,33 @@
         self.queue = []  # proposed live point queue
         self.nqueue = 0  # current size of the queue
         self.unused = 0  # total number of proposals unused
         self.used = 0  # total number of proposals used
 
         # sampling
         self.it = 1  # current iteration
-        self.since_update = 0  # number of calls since the last update
         self.ncall = self.nlive  # number of function calls
         self.dlv = math.log((self.nlive + 1.) / self.nlive)  # shrinkage/iter
-        self.bound = [UnitCube(self.ncdim)]  # bounding distributions
-        self.nbound = 1  # total number of unique bounding distributions
         self.added_live = False  # whether leftover live points were used
         self.eff = 0.  # overall sampling efficiency
         self.cite = ''  # Default empty
         self.save_samples = True
         self.save_bounds = True
 
+        # bounding updates
+        self.bound_update_interval = update_interval
+        self.first_bound_update_ncall = first_update.get(
+            'min_ncall', 2 * self.nlive)
+        self.first_bound_update_eff = first_update.get('min_eff', 10.)
+        self.logl_first_update = None
+        self.unit_cube_sampling = True
+        self.bound = [UnitCube(self.ncdim)]  # bounding distributions
+        self.nbound = 1  # total number of unique bounding distributions
+        self.ncall_at_last_update = 0
+
         self.logvol_init = logvol_init
 
         self.plateau_mode = False
         self.plateau_counter = None
         self.plateau_logdvol = None
         # results
         self.saved_run = RunRecord()
@@ -162,15 +164,15 @@
 
     def evolve_point(self, *args):
         raise RuntimeError('Should be overriden')
 
     def update_proposal(self, *args, **kwargs):
         raise RuntimeError('Should be overriden')
 
-    def update(self):
+    def update(self, subset=None):
         raise RuntimeError('Should be overriden')
 
     def __setstate__(self, state):
         self.__dict__ = state
         self.pool = None
         self.M = map
 
@@ -206,18 +208,18 @@
         self.queue = []
         self.nqueue = 0
         self.unused = 0
         self.used = 0
 
         # sampling
         self.it = 1
-        self.since_update = 0
         self.ncall = self.nlive
         self.bound = [UnitCube(self.ncdim)]
         self.nbound = 1
+        self.unit_cube_sampling = True
         self.added_live = False
 
         self.plateau_mode = False
         self.plateau_counter = None
         self.plateau_logdvol = None
 
         # results
@@ -285,32 +287,55 @@
         Return list of papers that should be cited given the specified
         configuration of the sampler.
 
         """
 
         return self.cite
 
-    def _beyond_unit_bound(self, loglstar):
-        """Check whether we should update our bound beyond the initial
-        unit cube."""
-
-        if self.logl_first_update is None:
-            # If we haven't already updated our bounds, check if we satisfy
-            # the provided criteria for establishing the first bounding update.
-            check = (self.ncall > self.ubound_ncall
-                     and self.eff < self.ubound_eff)
-            if check:
-                # Save the log-likelihood where our first update took place.
+    def update_bound_if_needed(self, loglstar, ncall=None, force=False):
+        """
+        Here we update the bound depending on the situation
+        The arguments are the loglstar and number of calls
+        if force is true we update the bound no matter what
+        """
+
+        if ncall is None:
+            ncall = self.ncall
+        call_check_first = (ncall >= self.first_bound_update_ncall)
+        call_check = (ncall >=
+                      self.bound_update_interval + self.ncall_at_last_update)
+        efficiency_check = (self.eff < self.first_bound_update_eff)
+        # there are three cases when we update the bound
+        # * if we are still using uniform cube sampling and both efficiency is
+        # lower than the threshold and the number of calls is larger than the
+        # threshold
+        # * if we are sampling from uniform cube and loglstar is larger than
+        # the previously saved logl_first_update
+        # * if we are not uniformly cube sampling and the ncall is larger
+        # than the ncall of the previous update by the update_interval
+        # * we are forced
+        if ((self.unit_cube_sampling and efficiency_check and call_check_first)
+                or (not self.unit_cube_sampling and call_check) or
+            (self.unit_cube_sampling and self.logl_first_update is not None
+             and loglstar > self.logl_first_update)) or force:
+            if loglstar == _LOWL_VAL:
+                # in the case we just started and we have some
+                # LOWL_VAL points we don't want to use them for the
+                # boundary
+                subset = self.live_logl > loglstar
+            else:
+                subset = slice(None)
+            bound = self.update(subset=subset)
+            if self.save_bounds:
+                self.bound.append(bound)
+            self.nbound += 1
+            self.ncall_at_last_update = ncall
+            if self.unit_cube_sampling:
+                self.unit_cube_sampling = False
                 self.logl_first_update = loglstar
-            return check
-        else:
-            # If we've already update our bounds, check if we've exceeded the
-            # saved log-likelihood threshold. (This is useful when sampling
-            # within `dynamicsampler`).
-            return loglstar >= self.logl_first_update
 
     def _fill_queue(self, loglstar):
         """Sequentially add new live point proposals to the queue."""
 
         # All the samplers should have have a starting point
         # satisfying a strict logl>loglstar criterion
         # The slice sampler will just fail if it's not the case
@@ -322,15 +347,15 @@
                 raise RuntimeError(
                     'No live points are above loglstar. '
                     'Do you have a likelihood plateau ? '
                     'It is also possible that you are trying to sample '
                     'excessively around the very peak of the posterior')
         else:
             args = ()
-        if self._beyond_unit_bound(loglstar):
+        if not self.unit_cube_sampling:
             # Add/zip arguments to submit to the queue.
             point_queue = []
             axes_queue = []
             # Propose points using the provided sampling/bounding options.
             evolve_point = self.evolve_point
             while self.nqueue < self.queue_size:
                 point, axes = self.propose_point(*args)
@@ -385,74 +410,72 @@
 
         return u, v, logl, nc, blob
 
     def _new_point(self, loglstar):
         """Propose points until a new point that satisfies the log-likelihood
         constraint `loglstar` is found."""
 
-        ncall, nupdate = 0, 0
+        ncall = self.ncall
+        ncall_accum = 0
         while True:
             # Get the next point from the queue
             u, v, logl, nc, blob = self._get_point_value(loglstar)
             ncall += nc
+            ncall_accum += nc
 
-            # Bounding checks.
-            ucheck = ncall >= self.update_interval * (1 + nupdate)
-            bcheck = self._beyond_unit_bound(loglstar)
-
-            if blob is not None and bcheck:
+            if blob is not None and not self.unit_cube_sampling:
                 # If our queue is empty, update any tuning parameters
                 # associated
                 # with our proposal (sampling) method.
                 # If it's not empty we are just accumulating the
                 # the history of evaluations
                 self.update_proposal(blob, update=self.nqueue <= 0)
 
+            # the reason I'm not using self.ncall is that it's updated at
+            # higher level
+            # also on purpose this is placed in nqueue==0
+            # because we only want update if we are planning to generate
+            # new points
+            if self.nqueue == 0:
+                self.update_bound_if_needed(loglstar, ncall=ncall)
+
             # If we satisfy the log-likelihood constraint, we're done!
             if logl > loglstar:
                 break
 
-            # If there has been more than `update_interval` function calls
-            # made *and* we satisfy the criteria for moving beyond sampling
-            # from the unit cube, update the bound.
-            if ucheck and bcheck:
-                if loglstar == _LOWL_VAL:
-                    # in the case we just started and we have some
-                    # LOWL_VAL points we don't want to use them for the
-                    # boundary
-                    subset = self.live_logl > loglstar
-                else:
-                    subset = slice(None)
-                bound = self.update(subset=subset)
-                if self.save_bounds:
-                    self.bound.append(bound)
-                self.nbound += 1
-                nupdate += 1
-                self.since_update = -ncall  # ncall will be added back later
-
-        return u, v, logl, ncall
+        return u, v, logl, ncall_accum
 
     def add_live_points(self):
         """Add the remaining set of live points to the current set of dead
         points. Instantiates a generator that will be called by
         the user. Returns the same outputs as :meth:`sample`."""
 
         # Check if the remaining live points have already been added
         # to the output set of samples.
         if self.added_live:
             raise ValueError("The remaining live points have already "
                              "been added to the list of samples!")
         else:
             self.added_live = True
+        if len(self.saved_run['logz']) > 0:
+            logz = self.saved_run['logz'][-1]
+            logzvar = self.saved_run['logzvar'][-1]
+            h = self.saved_run['h'][-1]
+            loglstar = self.saved_run['logl'][-1]
+            logvol = self.saved_run['logvol'][-1]
+        else:
+            # this is special case if we didn't do any running
+            # just sampled uniformly and bailed out
+            h = 0.  # information, initially *0.*
+            logz = -1.e300  # ln(evidence), initially *0.*
+            logzvar = 0.  # var[ln(evidence)], initially *0.*
+            logvol = self.logvol_init
+            # initially contains the whole prior (volume=1.)
+            loglstar = -1.e300  # initial ln(likelihood)
 
-        logz = self.saved_run['logz'][-1]
-        logzvar = self.saved_run['logzvar'][-1]
-        h = self.saved_run['h'][-1]
-        loglstar = self.saved_run['logl'][-1]
-        logvol = self.saved_run['logvol'][-1]
         # After N samples have been taken out, the remaining volume is
         # `e^(-N / nlive)`. The remaining points are distributed uniformly
         # within the remaining volume so that the expected volume enclosed
         # by the `i`-th worst likelihood is
         # `e^(-N / nlive) * (nlive + 1 - i) / (nlive + 1)`.
         # The tricky bit here is what to do if we have a plateau that we
         # haven't fully exhausted
@@ -478,15 +501,15 @@
         dlvs = -np.diff(logvols, prepend=0)
         logvols += logvol
         # Sorting remaining live points.
         lsort_idx = np.argsort(self.live_logl)
         loglmax = max(self.live_logl)
 
         # Grabbing relevant values from the last dead point.
-        if self._beyond_unit_bound(loglstar):
+        if not self.unit_cube_sampling:
             bounditer = self.nbound - 1
         else:
             bounditer = 0
 
         # Add contributions from the remaining live points in order
         # from the lowest to the highest log-likelihoods.
         for i in range(self.nlive):
@@ -699,22 +722,14 @@
             logz = -1.e300  # ln(evidence), initially *0.*
             logzvar = 0.  # var[ln(evidence)], initially *0.*
             logvol = self.logvol_init
             # initially contains the whole prior (volume=1.)
             loglstar = -1.e300  # initial ln(likelihood)
             delta_logz = 1.e300  # ln(ratio) of total/current evidence
 
-            # Check if we should initialize a different bounding distribution
-            # instead of using the unit cube.
-            if self._beyond_unit_bound(loglstar):
-                bound = self.update()
-                if self.save_bounds:
-                    self.bound.append(bound)
-                    self.nbound += 1
-                self.since_update = 0
         else:
             # Remove live points (if added) from previous run.
             if self.added_live and not resume:
                 self._remove_live_points()
 
             # Get final state from previous run.
             h, logz, logzvar, logvol = [
@@ -783,26 +798,14 @@
                                     logzvar=logzvar,
                                     h=h,
                                     logvol=logvol,
                                     logl=loglstar)
                     self.saved_run.append(add_info)
                 break
 
-            # After `update_interval` interations have passed *and* we meet
-            # the criteria for moving beyond sampling from the unit cube,
-            # update the bound using the current set of live points.
-            ucheck = self.since_update >= self.update_interval
-            bcheck = self._beyond_unit_bound(loglstar)
-            if ucheck and bcheck:
-                bound = self.update()
-                if self.save_bounds:
-                    self.bound.append(bound)
-                self.nbound += 1
-                self.since_update = 0
-
             worst = np.argmin(self.live_logl)  # index
             # Locate the "live" point with the lowest `logl`.
             worst_it = self.live_it[worst]  # when point was proposed
             boundidx = self.live_bound[worst]  # associated bound index
 
             if not self.plateau_mode:
                 nplateau = (self.live_logl == self.live_logl[worst]).sum()
@@ -834,26 +837,25 @@
 
             # Sample a new live point from within the likelihood constraint
             # `logl > loglstar` using the bounding distribution and sampling
             # method from our sampler.
             u, v, logl, nc = self._new_point(loglstar_new)
             ncall += nc
             self.ncall += nc
-            self.since_update += nc
             if self.blob:
                 new_blob = logl.blob
             else:
                 new_blob = None
             (logwt, logz, logzvar,
              h) = progress_integration(loglstar, loglstar_new, logz, logzvar,
                                        logvol, cur_dlv, h)
             loglstar = loglstar_new
 
             # Compute bound index at the current iteration.
-            if self._beyond_unit_bound(loglstar):
+            if not self.unit_cube_sampling:
                 bounditer = self.nbound - 1
             else:
                 bounditer = 0
 
             # Save the worst live point. It is now a "dead" point.
             if self.save_samples:
                 self.saved_run.append(
```

### Comparing `dynesty-2.1.0/py/dynesty/sampling.py` & `dynesty-2.1.1/py/dynesty/sampling.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/py/dynesty/utils.py` & `dynesty-2.1.1/py/dynesty/utils.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.0/py/dynesty.egg-info/PKG-INFO` & `dynesty-2.1.1/py/dynesty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynesty
-Version: 2.1.0
+Version: 2.1.1
 Summary: A dynamic nested sampling package for computing Bayesian posteriors and evidences.
 Home-page: https://github.com/joshspeagle/dynesty
 Author: Joshua S Speagle, Sergey E Koposov
 Author-email: j.speagle@utoronto.ca
 License: MIT
 Keywords: nested sampling,dynamic,monte carlo,bayesian,inference,modeling
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dynesty-2.1.0/setup.py` & `dynesty-2.1.1/setup.py`

 * *Files identical despite different names*

