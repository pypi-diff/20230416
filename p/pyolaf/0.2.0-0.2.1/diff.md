# Comparing `tmp/pyolaf-0.2.0.tar.gz` & `tmp/pyolaf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyolaf-0.2.0.tar", last modified: Tue Apr 11 23:49:14 2023, max compression
+gzip compressed data, was "pyolaf-0.2.1.tar", last modified: Sat Apr 15 22:48:10 2023, max compression
```

## Comparing `pyolaf-0.2.0.tar` & `pyolaf-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 23:49:14.869633 pyolaf-0.2.0/
--rw-rw-r--   0 lili      (1000) lili      (1000)    11300 2023-04-10 19:39:37.000000 pyolaf-0.2.0/LICENSE
--rw-rw-r--   0 lili      (1000) lili      (1000)     2007 2023-04-11 23:49:14.869633 pyolaf-0.2.0/PKG-INFO
--rw-rw-r--   0 lili      (1000) lili      (1000)     1372 2023-04-11 19:33:26.000000 pyolaf-0.2.0/README.md
-drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 23:49:14.869633 pyolaf-0.2.0/pyolaf/
--rw-rw-r--   0 lili      (1000) lili      (1000)      236 2023-04-11 23:49:03.000000 pyolaf-0.2.0/pyolaf/__init__.py
--rw-rw-r--   0 lili      (1000) lili      (1000)     2943 2023-04-11 21:41:27.000000 pyolaf-0.2.0/pyolaf/aliasing.py
--rw-rw-r--   0 lili      (1000) lili      (1000)     1899 2023-04-11 19:29:52.000000 pyolaf-0.2.0/pyolaf/fftpack.py
--rw-rw-r--   0 lili      (1000) lili      (1000)    35001 2023-04-11 23:35:03.000000 pyolaf-0.2.0/pyolaf/geometry.py
--rw-rw-r--   0 lili      (1000) lili      (1000)    34050 2023-04-11 23:45:54.000000 pyolaf-0.2.0/pyolaf/lf.py
--rw-rw-r--   0 lili      (1000) lili      (1000)    12433 2023-04-11 23:18:28.000000 pyolaf-0.2.0/pyolaf/project.py
--rw-rw-r--   0 lili      (1000) lili      (1000)     2458 2023-04-11 23:07:15.000000 pyolaf-0.2.0/pyolaf/transform.py
-drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-11 23:49:14.869633 pyolaf-0.2.0/pyolaf.egg-info/
--rw-rw-r--   0 lili      (1000) lili      (1000)     2007 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/PKG-INFO
--rw-rw-r--   0 lili      (1000) lili      (1000)      301 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/SOURCES.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)        1 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/dependency_links.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)       69 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/requires.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)        7 2023-04-11 23:49:14.000000 pyolaf-0.2.0/pyolaf.egg-info/top_level.txt
--rw-rw-r--   0 lili      (1000) lili      (1000)       38 2023-04-11 23:49:14.869633 pyolaf-0.2.0/setup.cfg
--rw-rw-r--   0 lili      (1000) lili      (1000)     1061 2023-04-11 23:48:50.000000 pyolaf-0.2.0/setup.py
+drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-15 22:48:10.014057 pyolaf-0.2.1/
+-rw-rw-r--   0 lili      (1000) lili      (1000)    11300 2023-04-10 19:39:37.000000 pyolaf-0.2.1/LICENSE
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1967 2023-04-15 22:48:10.014057 pyolaf-0.2.1/PKG-INFO
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1332 2023-04-15 22:47:55.000000 pyolaf-0.2.1/README.md
+drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-15 22:48:10.014057 pyolaf-0.2.1/pyolaf/
+-rw-rw-r--   0 lili      (1000) lili      (1000)      236 2023-04-15 22:47:04.000000 pyolaf-0.2.1/pyolaf/__init__.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)     2943 2023-04-11 21:41:27.000000 pyolaf-0.2.1/pyolaf/aliasing.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1899 2023-04-11 19:29:52.000000 pyolaf-0.2.1/pyolaf/fftpack.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)    29813 2023-04-14 23:58:14.000000 pyolaf-0.2.1/pyolaf/geometry.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)    34037 2023-04-15 22:24:42.000000 pyolaf-0.2.1/pyolaf/lf.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)    12433 2023-04-11 23:18:28.000000 pyolaf-0.2.1/pyolaf/project.py
+-rw-rw-r--   0 lili      (1000) lili      (1000)     2458 2023-04-11 23:07:15.000000 pyolaf-0.2.1/pyolaf/transform.py
+drwxrwxr-x   0 lili      (1000) lili      (1000)        0 2023-04-15 22:48:10.014057 pyolaf-0.2.1/pyolaf.egg-info/
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1967 2023-04-15 22:48:09.000000 pyolaf-0.2.1/pyolaf.egg-info/PKG-INFO
+-rw-rw-r--   0 lili      (1000) lili      (1000)      301 2023-04-15 22:48:09.000000 pyolaf-0.2.1/pyolaf.egg-info/SOURCES.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)        1 2023-04-15 22:48:09.000000 pyolaf-0.2.1/pyolaf.egg-info/dependency_links.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)       76 2023-04-15 22:48:09.000000 pyolaf-0.2.1/pyolaf.egg-info/requires.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)        7 2023-04-15 22:48:09.000000 pyolaf-0.2.1/pyolaf.egg-info/top_level.txt
+-rw-rw-r--   0 lili      (1000) lili      (1000)       38 2023-04-15 22:48:10.014057 pyolaf-0.2.1/setup.cfg
+-rw-rw-r--   0 lili      (1000) lili      (1000)     1079 2023-04-15 22:46:28.000000 pyolaf-0.2.1/setup.py
```

### Comparing `pyolaf-0.2.0/LICENSE` & `pyolaf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyolaf-0.2.0/PKG-INFO` & `pyolaf-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyolaf
-Version: 0.2.0
+Version: 0.2.1
 Summary: 3D reconstruction framework for light field microscopy
 Home-page: https://github.com/lambdaloop/pyolaf
 Author: Lili Karashchuk
 Author-email: krchtchk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,15 @@
 
 # pyolaf - A Python-based 3D reconstruction framework for light field microscopy
 
 pyolaf is a Python port of the [oLaF](https://gitlab.lrz.de/IP/olaf/) 3D reconstruction framework for light field microscopy (LFM). 
 
 ## Overview
   
-The light field microscope (LFM) allows for 3D imaging of fluorescent specimens using an array of micro-lenses (MLA) that capture both spatial and directional light field information in a single shot. oLaF is a Matlab framework for 3D reconstruction of LFM data that makes use of advanced algorithms for artifact-free deconvolution and Fourier integral microscopy. 
+The light field microscope (LFM) allows for 3D imaging of fluorescent specimens using an array of micro-lenses (MLA) that capture both spatial and directional light field information in a single shot. oLaF is a Matlab framework for 3D reconstruction of LFM data with a deconvolution algorithm that reduces aliasing artifacts.
 
 pyolaf brings these same features to the Python ecosystem, using GPU acceleration and some further code optimizations to **speed up deconvolution by 20x**. 
 
 ## Limitations
 
 pyolaf only supports regular grids and single-focus conventional light-field microscopes.
 In particular Fourier LFM, hexagonal grids, and multi-focus lenslets are currently not supported.
```

### Comparing `pyolaf-0.2.0/README.md` & `pyolaf-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyolaf - A Python-based 3D reconstruction framework for light field microscopy
 
 pyolaf is a Python port of the [oLaF](https://gitlab.lrz.de/IP/olaf/) 3D reconstruction framework for light field microscopy (LFM). 
 
 ## Overview
   
-The light field microscope (LFM) allows for 3D imaging of fluorescent specimens using an array of micro-lenses (MLA) that capture both spatial and directional light field information in a single shot. oLaF is a Matlab framework for 3D reconstruction of LFM data that makes use of advanced algorithms for artifact-free deconvolution and Fourier integral microscopy. 
+The light field microscope (LFM) allows for 3D imaging of fluorescent specimens using an array of micro-lenses (MLA) that capture both spatial and directional light field information in a single shot. oLaF is a Matlab framework for 3D reconstruction of LFM data with a deconvolution algorithm that reduces aliasing artifacts.
 
 pyolaf brings these same features to the Python ecosystem, using GPU acceleration and some further code optimizations to **speed up deconvolution by 20x**. 
 
 ## Limitations
 
 pyolaf only supports regular grids and single-focus conventional light-field microscopes.
 In particular Fourier LFM, hexagonal grids, and multi-focus lenslets are currently not supported.
```

### Comparing `pyolaf-0.2.0/pyolaf/aliasing.py` & `pyolaf-0.2.1/pyolaf/aliasing.py`

 * *Files identical despite different names*

### Comparing `pyolaf-0.2.0/pyolaf/fftpack.py` & `pyolaf-0.2.1/pyolaf/fftpack.py`

 * *Files identical despite different names*

### Comparing `pyolaf-0.2.0/pyolaf/geometry.py` & `pyolaf-0.2.1/pyolaf/geometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -682,138 +682,7 @@
     # Compute lenslets centers on the sensor and corresponding repetition patches centers in texture space (in voxels)
     NewLensletGridModel['FirstPosShiftRow'] = LensletGridModel['FirstPosShiftRow']
     TextureGridModel['FirstPosShiftRow'] = NewLensletGridModel['FirstPosShiftRow']
     LensletCenters = LFM_computeLensCenters(NewLensletGridModel, TextureGridModel, Resolution['sensorRes'], Camera['focus'], Camera['gridType'])
 
     return LensletCenters, Resolution, LensletGridModel, NewLensletGridModel
 
-
-
-
-def LFM_computeTube2MLA(lensPitch, mla2sensor, deltaOT, objRad, ftl):
-
-    # tube2mla satisfies 3 conditions:
-    # 1. matching effective f number with the
-    # 2. effective tubeLensRadius
-    # 3. the above when focused on the MLA
-
-    # solve quadratic equation
-    a = ftl*lensPitch/(2*mla2sensor)
-    # b = delta_ot*objRad - ftl*objRad - mla2sensor*ftl;
-    b = deltaOT*objRad - ftl*objRad
-    c = -ftl*deltaOT*objRad
-
-    delta_equation = (b**2 - 4*a*c)**(1/2)
-
-    tube2mla = [(-b+delta_equation)/(2*a), (-b-delta_equation)/(2*a)]
-    tube2mla = [i for i in tube2mla if i > 0]
-
-    return tube2mla
-
-def LFM_setCameraParams(configFile, newSpacingPx):
-
-    # set LFM parameters:
-    #### objective params
-    # M-> objective magnification
-    # NA-> objective aperture
-    # ftl-> focal length of tube lens (only for microscopes)
-
-    #### sensor
-    # lensPitch-> lenslet pitch
-    # pixelPitch-> sensor pixel pitch
-
-    #### MLA params
-    # gridType-> microlens grid type: "reg" -> regular grid array; "hex" -> hexagonal grid array
-    # focus-> microlens focus: "single" -> all ulens in the array have the same focal length; 'multi' -> 3 mixed focal lenghts in a hex grid
-    # fml-> focal length of the lenslets
-    # uLensMask-> 1 when there is no space between ulenses (rect shape); 0 when there is space between ulenses (circ aperture)
-
-    #### light characteristics
-    # n-> refraction index (1 for air)
-    # wavelenght-> wavelenght of the the emission light
-
-    ##### distances
-    # plenoptic-> plenoptic type: "1" for the original LFM configuration (tube2mla = ftl); "2" for defocused LFM (tube2mla != ftl) design
-    # tube2mla-> distance between tube lens and MLA (= ftl in original LFM design)
-    # mla2sensor-> distance between MLA and sensor
-
-    with open(configFile, "r") as f:
-        Camera = yaml.safe_load(f)
-
-    # if isinstance(Camera["fm"], list):
-    #     Camera["fm"] = [float(val) for val in Camera["fm"]]
-    #     Camera["fm"] = float(sum(Camera["fm"]))
-
-    # compute extra LFM configuration specific parameters
-    # for regular grid we only need to compute 1/4 of the psf pattens, due to symmetry
-    if Camera["gridType"] == "reg":
-        Camera["range"] = "quarter"
-    elif Camera["gridType"] == "hex":
-        Camera["range"] = "full"
-
-    Camera["fobj"] = Camera["ftl"]/Camera["M"]  ## focal length of objective lens
-    Camera["Delta_ot"] = Camera["ftl"] + Camera["fobj"] ## obj2tube distance
-
-    # ulens spacing = ulens pitch
-    spacingPx = Camera["lensPitch"]/Camera["pixelPitch"]
-    if newSpacingPx == "default":
-        newSpacingPx = spacingPx
-
-    Camera["spacingPx"] = spacingPx
-    Camera["newSpacingPx"] = newSpacingPx  # artificial spacing, usually lower than spacingPx for speed up
-    Camera["newPixelPitch"] = Camera["lensPitch"]/newSpacingPx
-
-    Camera["k"] = 2 * np.pi * Camera["n"] / Camera["WaveLength"] ## wave number
-
-    objRad = Camera["fobj"] * Camera["NA"] # objective radius
-
-    if Camera["plenoptic"] == 2:
-
-        obj2tube = Camera["fobj"] + Camera["ftl"]  ## objective to tl distance
-
-        # check if tube2mla is provided by user, otherwise compute it s.t. the F number matching condition is satisfied
-        if Camera["tube2mla"] == 0:
-            if Camera["mla2sensor"] == 0:
-                raise ValueError("At least one of the 'tube2mla' or 'mla2sensor' distances need to be provided in the - plenoptic == 2 - case")
-            else:
-                tube2mla = LFM_computeTube2MLA(Camera["lensPitch"], Camera["mla2sensor"], obj2tube, objRad, Camera["ftl"])
-                Camera["tube2mla"] = tube2mla
-
-        dot = Camera["ftl"] * Camera["tube2mla"] / (Camera["tube2mla"] - Camera["ftl"])  ## depth focused on the mla by the tube lens (object side of tl)
-        dio = obj2tube - dot  ## image side of the objective
-        dof = Camera["fobj"] * dio / (dio - Camera["fobj"])  ## object side of the objective -> dof is focused on the MLA
-        if np.isnan(dof):
-            dof = Camera["fobj"]
-
-        # M_mla = tube2mla/dof
-        M_mla = Camera["M"]  ## in 4f systems magnification does not change with depth ?
-        tubeRad = (dio - obj2tube) * objRad / dio
-
-        # if tube2mla is known and mla2sensor has to be retrived s.t. F number matching condition is satisfied
-        if Camera["mla2sensor"] == 0:
-            mla2sensor = tube2mla * Camera["lensPitch"] / 2 / tubeRad
-            Camera["mla2sensor"] = mla2sensor
-
-    elif Camera["plenoptic"] == 1:
-
-        if Camera["tube2mla"] == 0:
-            Camera["tube2mla"] = Camera["ftl"]
-
-        if Camera["mla2sensor"] == 0:
-            Camera["mla2sensor"] = Camera["fm"]
-
-        tubeRad = objRad
-        dof = Camera["fobj"]  ## object side of the objective -> dof is focused on the mla
-        M_mla = Camera["M"]  # magnification up to the mla position
-
-    # Write extra computed parameters to Camera dictionary
-    uRad =  tubeRad * Camera["mla2sensor"] / Camera["tube2mla"]
-    offsetFobj = dof - Camera["fobj"]
-
-    Camera["objRad"] = objRad
-    Camera["uRad"] = uRad
-    Camera["tubeRad"] = tubeRad
-    Camera["dof"] = dof
-    Camera["offsetFobj"] = offsetFobj
-    Camera["M_mla"] = M_mla
-
-    return Camera
```

### Comparing `pyolaf-0.2.0/pyolaf/lf.py` & `pyolaf-0.2.1/pyolaf/lf.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
             print('PSF: {}/{} already computed for depth {}'.format(i + 1, len(Resolution["depths"]), Resolution["depths"][idx]))
 
         psfWaveStack[:, :, i]  = psfWAVE
 
     print('...')
     return psfWaveStack
 
-import numba
 from scipy import integrate, special
 import scipy.special
 
 
 def LFM_calcPSF(p1, p2, p3, Camera, Resolution):
     """
     Computes the PSF at the Camera.Native image plane for a source point (p1, p2, p3) using wave optics theory
```

### Comparing `pyolaf-0.2.0/pyolaf/project.py` & `pyolaf-0.2.1/pyolaf/project.py`

 * *Files identical despite different names*

### Comparing `pyolaf-0.2.0/pyolaf/transform.py` & `pyolaf-0.2.1/pyolaf/transform.py`

 * *Files identical despite different names*

### Comparing `pyolaf-0.2.0/pyolaf.egg-info/PKG-INFO` & `pyolaf-0.2.1/pyolaf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyolaf
-Version: 0.2.0
+Version: 0.2.1
 Summary: 3D reconstruction framework for light field microscopy
 Home-page: https://github.com/lambdaloop/pyolaf
 Author: Lili Karashchuk
 Author-email: krchtchk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,15 @@
 
 # pyolaf - A Python-based 3D reconstruction framework for light field microscopy
 
 pyolaf is a Python port of the [oLaF](https://gitlab.lrz.de/IP/olaf/) 3D reconstruction framework for light field microscopy (LFM). 
 
 ## Overview
   
-The light field microscope (LFM) allows for 3D imaging of fluorescent specimens using an array of micro-lenses (MLA) that capture both spatial and directional light field information in a single shot. oLaF is a Matlab framework for 3D reconstruction of LFM data that makes use of advanced algorithms for artifact-free deconvolution and Fourier integral microscopy. 
+The light field microscope (LFM) allows for 3D imaging of fluorescent specimens using an array of micro-lenses (MLA) that capture both spatial and directional light field information in a single shot. oLaF is a Matlab framework for 3D reconstruction of LFM data with a deconvolution algorithm that reduces aliasing artifacts.
 
 pyolaf brings these same features to the Python ecosystem, using GPU acceleration and some further code optimizations to **speed up deconvolution by 20x**. 
 
 ## Limitations
 
 pyolaf only supports regular grids and single-focus conventional light-field microscopes.
 In particular Fourier LFM, hexagonal grids, and multi-focus lenslets are currently not supported.
```

### Comparing `pyolaf-0.2.0/setup.py` & `pyolaf-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyolaf",
-    version="0.2.0",
+    version="0.2.1",
     author="Lili Karashchuk",
     author_email="krchtchk@gmail.com",
     description="3D reconstruction framework for light field microscopy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lambdaloop/pyolaf",
     packages=setuptools.find_packages(),
@@ -26,14 +26,15 @@
     install_requires=[
         'pyyaml',
         'numpy',
         'scipy',
         'tqdm',
         'tifffile',
         'scikit-image',
-        'matplotlib'
+        'matplotlib',
+        'pyyaml'
     ],
     extras_require={
         'gpu':  ["cupy"]
     }
 
 )
```

