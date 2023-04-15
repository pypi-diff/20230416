# Comparing `tmp/spleaf-2.1.2.tar.gz` & `tmp/spleaf-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleaf-2.1.2.tar", last modified: Mon Feb 27 16:02:40 2023, max compression
+gzip compressed data, was "spleaf-2.1.3.tar", last modified: Sat Apr 15 23:03:49 2023, max compression
```

## Comparing `spleaf-2.1.2.tar` & `spleaf-2.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 16:02:40.700117 spleaf-2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-02-27 16:01:07.000000 spleaf-2.1.2/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-02-27 16:01:07.000000 spleaf-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      802 2023-02-27 16:02:40.700117 spleaf-2.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-02-27 16:01:07.000000 spleaf-2.1.2/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 16:02:40.700117 spleaf-2.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-02-27 16:01:07.000000 spleaf-2.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 16:02:40.696116 spleaf-2.1.2/spleaf/
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-02-27 16:01:07.000000 spleaf-2.1.2/spleaf/__info__.py
--rw-rw-rw-   0 root         (0) root         (0)    29194 2023-02-27 16:01:07.000000 spleaf-2.1.2/spleaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16971 2023-02-27 16:01:07.000000 spleaf-2.1.2/spleaf/cov.py
--rw-rw-rw-   0 root         (0) root         (0)    30205 2023-02-27 16:01:07.000000 spleaf-2.1.2/spleaf/libspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)     4571 2023-02-27 16:01:07.000000 spleaf-2.1.2/spleaf/libspleaf.h
--rw-rw-rw-   0 root         (0) root         (0)    61577 2023-02-27 16:01:07.000000 spleaf-2.1.2/spleaf/pywrapspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)    65826 2023-02-27 16:01:07.000000 spleaf-2.1.2/spleaf/term.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 16:02:40.696116 spleaf-2.1.2/spleaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      802 2023-02-27 16:02:40.000000 spleaf-2.1.2/spleaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      352 2023-02-27 16:02:40.000000 spleaf-2.1.2/spleaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 16:02:40.000000 spleaf-2.1.2/spleaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-27 16:02:40.000000 spleaf-2.1.2/spleaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-02-27 16:02:40.000000 spleaf-2.1.2/spleaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 16:02:40.700117 spleaf-2.1.2/test/
--rw-rw-rw-   0 root         (0) root         (0)    27167 2023-02-27 16:01:07.000000 spleaf-2.1.2/test/test_cov.py
--rw-rw-rw-   0 root         (0) root         (0)    11276 2023-02-27 16:01:07.000000 spleaf-2.1.2/test/test_spleaf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.022904 spleaf-2.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-04-15 23:02:33.000000 spleaf-2.1.3/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-15 23:02:33.000000 spleaf-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      802 2023-04-15 23:03:49.022904 spleaf-2.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-15 23:02:33.000000 spleaf-2.1.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 23:03:49.022904 spleaf-2.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-04-15 23:02:33.000000 spleaf-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.021904 spleaf-2.1.3/spleaf/
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/__info__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29194 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16971 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    49962 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/fenrir.py
+-rw-rw-rw-   0 root         (0) root         (0)    30205 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/libspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)     4571 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/libspleaf.h
+-rw-rw-rw-   0 root         (0) root         (0)    61577 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/pywrapspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)    82399 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.022904 spleaf-2.1.3/spleaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      802 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.022904 spleaf-2.1.3/test/
+-rw-rw-rw-   0 root         (0) root         (0)    27167 2023-04-15 23:02:33.000000 spleaf-2.1.3/test/test_cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    11276 2023-04-15 23:02:33.000000 spleaf-2.1.3/test/test_spleaf.py
```

### Comparing `spleaf-2.1.2/COPYING` & `spleaf-2.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.2/PKG-INFO` & `spleaf-2.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleaf
-Version: 2.1.2
+Version: 2.1.3
 Summary: Symmetric S+LEAF matrix.
 Home-page: https://gitlab.unige.ch/jean-baptiste.delisle/spleaf
 Author: Jean-Baptiste Delisle
 Author-email: jean-baptiste.delisle@unige.ch
 License: GPLv3
 Requires-Python: >=3.6
 License-File: COPYING
```

### Comparing `spleaf-2.1.2/README.rst` & `spleaf-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.2/setup.py` & `spleaf-2.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2019-2022 Jean-Baptiste Delisle
+# Copyright 2019-2023 Jean-Baptiste Delisle
 #
 # This file is part of spleaf.
 #
 # spleaf is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `spleaf-2.1.2/spleaf/__info__.py` & `spleaf-2.1.3/spleaf/__info__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2019-2022 Jean-Baptiste Delisle
+# Copyright 2019-2023 Jean-Baptiste Delisle
 #
 # This file is part of spleaf.
 #
 # spleaf is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -19,8 +19,8 @@
 
 __title__ = 'spleaf'
 __description__ = 'Symmetric S+LEAF matrix.'
 __author__ = 'Jean-Baptiste Delisle'
 __author_email__ = 'jean-baptiste.delisle@unige.ch'
 __license__ = 'GPLv3'
 __url__ = 'https://gitlab.unige.ch/jean-baptiste.delisle/spleaf'
-__version__ = "2.1.2"
+__version__ = "2.1.3"
```

### Comparing `spleaf-2.1.2/spleaf/__init__.py` & `spleaf-2.1.3/spleaf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2019-2022 Jean-Baptiste Delisle
+# Copyright 2019-2023 Jean-Baptiste Delisle
 #
 # This file is part of spleaf.
 #
 # spleaf is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `spleaf-2.1.2/spleaf/cov.py` & `spleaf-2.1.3/spleaf/cov.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020-2022 Jean-Baptiste Delisle
+# Copyright 2019-2023 Jean-Baptiste Delisle
 #
 # This file is part of spleaf.
 #
 # spleaf is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `spleaf-2.1.2/spleaf/libspleaf.c` & `spleaf-2.1.3/spleaf/libspleaf.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019-2022 Jean-Baptiste Delisle
+// Copyright 2019-2023 Jean-Baptiste Delisle
 //
 // This file is part of spleaf.
 //
 // spleaf is free software: you can redistribute it and/or modify
 // it under the terms of the GNU General Public License as published by
 // the Free Software Foundation, either version 3 of the License, or
 // (at your option) any later version.
```

### Comparing `spleaf-2.1.2/spleaf/libspleaf.h` & `spleaf-2.1.3/spleaf/libspleaf.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019-2022 Jean-Baptiste Delisle
+// Copyright 2019-2023 Jean-Baptiste Delisle
 //
 // This file is part of spleaf.
 //
 // spleaf is free software: you can redistribute it and/or modify
 // it under the terms of the GNU General Public License as published by
 // the Free Software Foundation, either version 3 of the License, or
 // (at your option) any later version.
```

### Comparing `spleaf-2.1.2/spleaf/pywrapspleaf.c` & `spleaf-2.1.3/spleaf/pywrapspleaf.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019-2022 Jean-Baptiste Delisle
+// Copyright 2019-2023 Jean-Baptiste Delisle
 //
 // This file is part of spleaf.
 //
 // spleaf is free software: you can redistribute it and/or modify
 // it under the terms of the GNU General Public License as published by
 // the Free Software Foundation, either version 3 of the License, or
 // (at your option) any later version.
```

### Comparing `spleaf-2.1.2/spleaf/term.py` & `spleaf-2.1.3/spleaf/term.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020-2022 Jean-Baptiste Delisle
+# Copyright 2019-2023 Jean-Baptiste Delisle
 #
 # This file is part of spleaf.
 #
 # spleaf is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,17 +16,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with spleaf.  If not, see <http://www.gnu.org/licenses/>.
 
 __all__ = [
   'Error', 'Jitter', 'InstrumentJitter', 'CalibrationError',
   'CalibrationJitter', 'ExponentialKernel', 'QuasiperiodicKernel',
-  'Matern32Kernel', 'Matern52Kernel', 'SumKernel', 'ProductKernel',
+  'Matern12Kernel', 'Matern32Kernel', 'Matern52Kernel', 'SumKernel',
+  'SimpleSumKernel', 'ProductKernel', 'SimpleProductKernel', 'TransformKernel',
   'USHOKernel', 'OSHOKernel', 'SHOKernel', 'MEPKernel', 'ESKernel',
-  'ESPKernel', 'MultiSeriesKernel'
+  'ESPKernel', 'MultiSeriesKernel', 'MultiFourierKernel'
 ]
 
 import numpy as np
 from scipy.special import ive
 import warnings
 
 
@@ -134,15 +135,22 @@
     r"""
     Compute the S+LEAF representation of the derivative of the GP
     for a new calendar t2.
     """
 
     pass
 
-  def eval(self, dt):
+  def set_conditional_coef(self, *args, **kwargs):
+    r"""
+    Set the coefficients used for the conditional computations.
+    """
+
+    pass
+
+  def eval(self, dt, series_id=None):
     r"""
     Evaluate the kernel at lag dt.
     """
 
     raise NotImplementedError(
       'The eval method should be implemented in Kernel childs.')
 
@@ -408,15 +416,15 @@
     V2[:, self._offset] = 1.0
     phi2[:, self._offset] = np.exp(-self._la * dt2)
     phi2left[:, self._offset] = np.exp(-self._la * dt2left)
     phi2right[:, self._offset] = np.exp(-self._la * dt2right)
     if dV2 is not None:
       dV2[:, self._offset] = self._la
 
-  def eval(self, dt):
+  def eval(self, dt, series_id=None):
     return (self._a * np.exp(-self._la * np.abs(dt)))
 
 
 class QuasiperiodicKernel(Kernel):
   r"""
   Quasiperiodic kernel.
 
@@ -567,20 +575,56 @@
       None]
     phi2right[:,
       self._offset:self._offset + 2] = np.exp(-self._la * dt2right)[:, None]
     if dV2 is not None:
       dV2[:, self._offset] = self._la * cnut2 - self._nu * snut2
       dV2[:, self._offset + 1] = self._la * snut2 + self._nu * cnut2
 
-  def eval(self, dt):
+  def eval(self, dt, series_id=None):
     adt = np.abs(dt)
     return (np.exp(-self._la * adt) *
       (self._a * np.cos(self._nu * adt) + self._b * np.sin(self._nu * adt)))
 
 
+class Matern12Kernel(ExponentialKernel):
+  r"""
+  Matérn 1/2 kernel.
+
+  .. math:: k(\Delta t) = \sigma^2 \mathrm{e}^{-\frac{\Delta t}{\rho}}
+
+  Parameters
+  ----------
+  sig : float
+    Amplitude (std).
+  rho : float
+    Scale.
+  """
+
+  def __init__(self, sig, rho):
+    super().__init__(sig * sig, 1 / rho)
+    self._sig = sig
+    self._rho = rho
+    self._param = ['sig', 'rho']
+
+  def _set_param(self, sig=None, rho=None):
+    if sig is not None:
+      self._sig = sig
+      self._a = sig * sig
+    if rho is not None:
+      self._rho = rho
+      self._la = 1 / rho
+
+  def _grad_param(self, grad_dU=None, grad_dV=None):
+    sgrad = super()._grad_param(grad_dU, grad_dV)
+    grad = {}
+    grad['sig'] = 2 * self._sig * sgrad['a']
+    grad['rho'] = -self._la * self._la * sgrad['la']
+    return (grad)
+
+
 class Matern32Kernel(Kernel):
   r"""
   Matérn 3/2 kernel.
 
   .. math:: k(\Delta t) = \sigma^2 \mathrm{e}^{-\sqrt{3}\frac{\Delta t}{\rho}}
     \left(1 + \sqrt{3}\frac{\Delta t}{\rho}\right)
 
@@ -697,15 +741,15 @@
       None]
     phi2right[:,
       self._offset:self._offset + 2] = np.exp(-self._la * dt2right)[:, None]
     if dV2 is not None:
       dV2[:, self._offset] = self._la
       dV2[:, self._offset + 1] = -self._la * x2
 
-  def eval(self, dt):
+  def eval(self, dt, series_id=None):
     dx = self._la * np.abs(dt)
     return (self._a * np.exp(-dx) * (1 + dx))
 
 
 class Matern52Kernel(Kernel):
   r"""
   Matérn 5/2 kernel.
@@ -849,15 +893,15 @@
     phi2right[:,
       self._offset:self._offset + 3] = np.exp(-self._la * dt2right)[:, None]
     if dV2 is not None:
       dV2[:, self._offset] = self._la
       dV2[:, self._offset + 1] = -self._la * x2 / 3 * onemx2
       dV2[:, self._offset + 2] = -2 / 3 * self._la * (1 + x2)
 
-  def eval(self, dt):
+  def eval(self, dt, series_id=None):
     dx = self._la * np.abs(dt)
     return (self._a * np.exp(-dx) * (1 + dx + dx * dx / 3))
 
 
 class SumKernel(Kernel):
   r"""
   Generic class for the sum of several kernel terms.
@@ -926,16 +970,61 @@
     phi2left,
     phi2right,
     dV2=None):
     for kernel in self._kernels:
       kernel._deriv_t2(t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right,
         phi2left, phi2right, dV2)
 
-  def eval(self, dt):
-    return (sum(kernel.eval(dt) for kernel in self._kernels))
+  def eval(self, dt, series_id=(0, 0)):
+    return (sum(kernel.eval(dt, series_id) for kernel in self._kernels))
+
+
+class SimpleSumKernel(SumKernel):
+  r"""
+  """
+
+  def __init__(self, **kwargs):
+    self._kerneldic = kwargs
+    super().__init__(*kwargs.values())
+    self._param = [
+      f'{kern}_{key}' for kern in kwargs for key in kwargs[kern]._param
+    ]
+
+  def _kernel_param(self, **kwargs):
+    paramKern = {kern: {} for kern in self._kerneldic}
+    for par in kwargs:
+      kern, key = par.split('_', 1)
+      paramKern[kern][key] = kwargs[par]
+    return (paramKern.values())
+
+  def _kernel_param_back(self, *args):
+    grad = {}
+    for kern, gk in zip(self._kerneldic, args):
+      for key in gk:
+        grad[f'{kern}_{key}'] = gk[key]
+    return (grad)
+
+  def _get_param(self, par):
+    kern, key = par.split('_', 1)
+    return (self._kerneldic[kern]._get_param(key))
+
+  def set_conditional_coef(self, **kwargs):
+    r"""
+    Set the coefficients used for the conditional computations.
+    """
+    paramKern = {kern: {} for kern in self._kerneldic}
+    for par in kwargs:
+      if par == 'series_id':
+        for kern in self._kerneldic:
+          paramKern[kern][par] = kwargs[par]
+      else:
+        kern, key = par.split('_', 1)
+        paramKern[kern][key] = kwargs[par]
+    for kern in self._kerneldic:
+      self._kerneldic[kern].set_conditional_coef(**paramKern[kern])
 
 
 class _FakeCov:
 
   def __init__(self, t, dt, r):
     self.t = t
     self.dt = dt
@@ -1199,16 +1288,121 @@
         self._offset + k1 * self._kernel2._r:self._offset + (k1 + 1) *
         self._kernel2._r] = kernel1_phi2right[:, k1, None] * kernel2_phi2right
       if dV2 is not None:
         dV2[:, self._offset + k1 * self._kernel2._r:self._offset +
           (k1 + 1) * self._kernel2._r] = kernel1_dV2[:, k1,
           None] * kernel2_V2 + kernel1_V2[:, k1, None] * kernel2_dV2
 
-  def eval(self, dt):
-    return (self._kernel1.eval(dt) * self._kernel2.eval(dt))
+  def eval(self, dt, series_id=(0, 0)):
+    return (self._kernel1.eval(dt, series_id) *
+      self._kernel2.eval(dt, series_id))
+
+
+class SimpleProductKernel(ProductKernel):
+  r"""
+  """
+
+  def __init__(self, **kwargs):
+    assert len(kwargs) == 2
+    self._kerneldic = kwargs
+    super().__init__(*kwargs.values())
+    self._param = [
+      f'{kern}_{key}' for kern in kwargs for key in kwargs[kern]._param
+    ]
+
+  def _kernel_param(self, **kwargs):
+    paramKern = {kern: {} for kern in self._kerneldic}
+    for par in kwargs:
+      kern, key = par.split('_', 1)
+      paramKern[kern][key] = kwargs[par]
+    return (paramKern.values())
+
+  def _kernel_param_back(self, *args):
+    grad = {}
+    for kern, gk in zip(self._kerneldic, args):
+      for key in gk:
+        grad[f'{kern}_{key}'] = gk[key]
+    return (grad)
+
+  def _get_param(self, par):
+    kern, key = par.split('_', 1)
+    return (self._kerneldic[kern]._get_param(key))
+
+  def set_conditional_coef(self, **kwargs):
+    r"""
+    Set the coefficients used for the conditional computations.
+    """
+    paramKern = {kern: {} for kern in self._kerneldic}
+    for par in kwargs:
+      if par == 'series_id':
+        for kern in self._kerneldic:
+          paramKern[kern][par] = kwargs[par]
+      else:
+        kern, key = par.split('_', 1)
+        paramKern[kern][key] = kwargs[par]
+    for kern in self._kerneldic:
+      self._kerneldic[kern].set_conditional_coef(**paramKern[kern])
+
+class TransformKernel(Kernel):
+
+  def __init__(
+      self,
+      inner_kernel,
+      translate_param,
+      translate_param_back=None,
+      **kwargs):
+
+    super().__init__()
+    self._value = kwargs
+    self._translate_param = translate_param
+    self._translate_param_back = translate_param_back
+    self._kernel = inner_kernel
+    self._kernel._set_param(**self._translate_param(**self._value))
+    self._r = self._kernel._r
+    self._param = list(self._value.keys())
+
+  def _link(self, cov, offset):
+    super()._link(cov, offset)
+    self._kernel._link(cov, offset)
+
+  def _compute(self):
+    self._kernel._compute()
+
+  def _get_param(self, par):
+    return (self._value[par])
+
+  def _set_param(self, *args, **kwargs):
+    for karg, arg in enumerate(args):
+      par = self._param[karg]
+      if par in kwargs:
+        raise Exception(
+          f'TransformKernel._set_param: parameter {par} multiply defined.')
+      kwargs[par] = arg
+    self._value.update(kwargs)
+    self._kernel._set_param(**self._translate_param(**self._value))
+
+  def _grad_param(self, grad_dU=None, grad_dV=None):
+    grad_kernel = self._kernel._grad_param(grad_dU, grad_dV)
+    return (self._translate_param_back(grad_kernel))
+
+  def set_conditional_coef(self, *args, **kwargs):
+    r"""
+    Set the coefficients used for the conditional computations.
+    """
+
+    self._kernel.set_conditional_coef(*args, **kwargs)
+
+  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
+    phi2left, phi2right):
+
+    self._kernel._compute_t2(t2, dt2, U2, V2, phi2, ref2left, dt2left,
+      dt2right, phi2left, phi2right)
+
+  def eval(self, dt, series_id=(0, 0)):
+    return (self._kernel.eval(dt, series_id))
 
 
 class USHOKernel(QuasiperiodicKernel):
   r"""
   Under-damped SHO Kernel.
 
   This kernel follows the differential equation of
@@ -1427,15 +1621,15 @@
     if self._Q > 0.5:
       self._usho._deriv_t2(t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right,
         phi2left, phi2right, dV2)
     else:
       self._osho._deriv_t2(t2, dt2, dU2, V2, phi2, ref2left, dt2left, dt2right,
         phi2left, phi2right, dV2)
 
-  def eval(self, dt):
+  def eval(self, dt, series_id=None):
     if self._Q > 0.5:
       return (self._usho.eval(dt))
     else:
       return (self._osho.eval(dt))
 
 
 class MEPKernel(SumKernel):
@@ -1971,15 +2165,15 @@
         kernel_dV2)
       # cov(GP, dGP), cov(dGP, GP), cov(dGP, dGP)
       U2[:, self._offset:self._offset + self._r] += beta * kernel_dU2
       V2[:, self._offset:self._offset + self._r] += beta * kernel_dV2
 
   def _deriv(self, calc_d2=False):
     if self._with_derivative:
-      raise NotImplementedError
+      raise NotImplementedError()
     else:
       self._kernel._deriv(calc_d2)
       for k in range(self._nseries):
         ik = self._series_index[k]
         self._cov._dU[ik, self._offset:self._offset +
           self._r] = self._alpha[k] * self._kernel._cov._dU
         if calc_d2:
@@ -1996,15 +2190,15 @@
     dt2left,
     dt2right,
     phi2left,
     phi2right,
     dV2=None):
 
     if self._with_derivative:
-      raise NotImplementedError
+      raise NotImplementedError()
     else:
       if self._cond_series_id is None:
         alpha = self._cond_alpha
       else:
         alpha = self._alpha[self._cond_series_id]
       kernel_dU2 = np.empty((t2.size, self._r))
       kernel_V2 = np.empty((t2.size, self._r))
@@ -2023,9 +2217,287 @@
       if dV2 is not None:
         dV2[:, self._offset:self._offset + self._r] = alpha * kernel_dV2
 
       phi2[:, self._offset:self._offset + self._r] = kernel_phi2
       phi2left[:, self._offset:self._offset + self._r] = kernel_phi2left
       phi2right[:, self._offset:self._offset + self._r] = kernel_phi2right
 
-  def eval(self, dt):
+  def eval(self, dt, series_id=None):
+    if series_id is not None:
+      raise NotImplementedError()
     return (self._kernel.eval(dt))
+
+
+class MultiFourierKernel(Kernel):
+  r"""
+  Multivariate Fourier series kernel.
+
+  For :math:`m` times series (:math:`y_1,\dots y_m`), the covariance between
+  two time series :math:`y_i, y_j` follows:
+
+  .. math:: k_{i,j}(\Delta t) = \sum_{k=0}^{n_\mathrm{harm}} a_{k; i,j} \cos(k \nu \Delta t) + b_{k; i,j} \sin(k \nu \Delta t),
+
+  where :math:`a_k` and :math:`b_k` are the :math:`m\times m` matrices given by:
+
+  .. math:: a_k = \alpha_k \alpha_k^\mathrm{T} + \beta_k \beta_k^\mathrm{T},
+
+  .. math:: b_k = \alpha_k \beta_k^\mathrm{T} - \beta_k \alpha_k^\mathrm{T},
+
+  and :math:`\alpha_k`, :math:`\beta_k` are :math:`m\times r` matrices.
+
+  Parameters
+  ----------
+  nu : float
+    Fundamental angular frequency.
+  alpha, beta: (nharm + 1, m, r) ndarrays
+    Fourier coefficients. beta[0] should be filled with zeros.
+  series_index : list of ndarrays
+    Indices corresponding to each original time series in the merged time series.
+  vectorize :
+    Whether alpha, beta should be directly passed as parameters or split by index.
+  """
+
+  def __init__(self, P, alpha, beta, series_index=None, vectorize=False):
+    super().__init__()
+    self._series_index = series_index if series_index else [slice(None)]
+    self._nseries = len(self._series_index)
+    self._P = P
+    self._alpha = alpha
+    self._beta = beta
+    self._nfreq = self._alpha.shape[0]
+    self._nharm = self._nfreq - 1
+    self._coef_rank = self._alpha.shape[2]
+    assert self._alpha.shape[1] == self._nseries
+    if self._nharm > 0:
+      assert self._beta.shape[0] == self._nfreq
+      assert self._beta.shape[1] == self._nseries
+      assert self._beta.shape[2] == self._coef_rank
+      assert np.all(self._beta[0] == 0)
+    self._r = (2 * self._nfreq - 1) * self._coef_rank
+    self._cond_alpha = None
+    self._cond_beta = None
+    self._cond_series_id = 0
+    self._vectorize = vectorize
+    if self._vectorize:
+      param_alpha = ['alpha']
+      param_beta = ['beta']
+    else:
+      param_alpha = [
+        f'alpha_{h}_{i}_{s}' for h in range(self._nfreq)
+        for i in range(self._nseries) for s in range(self._coef_rank)
+      ]
+      param_beta = [
+        f'beta_{h}_{i}_{s}' for h in range(self._nfreq)
+        for i in range(self._nseries) for s in range(self._coef_rank)
+      ]
+    if self._nharm == 0:
+      self._param = param_alpha
+    else:
+      self._param = ['P'] + param_alpha + param_beta
+
+  def _compute(self):
+    if self._nharm == 0:
+      for k, ik in enumerate(self._series_index):
+        self._cov.A[ik] += np.sum(self._alpha[0, k] * self._alpha[0, k])
+        self._cov.U[ik,
+          self._offset:self._offset + self._coef_rank] = self._alpha[0, k]
+    else:
+      self._nu = 2 * np.pi / self._P
+      self._nut = self._nu * self._cov.t
+      self._cjnut = np.empty((self._cov.n, self._nharm))
+      self._sjnut = np.empty((self._cov.n, self._nharm))
+      self._cjnut[:, 0] = np.cos(self._nut)
+      self._sjnut[:, 0] = np.sin(self._nut)
+      for j in range(1, self._nharm):
+        self._cjnut[:, j] = self._cjnut[:, j - 1] * self._cjnut[:,
+          0] - self._sjnut[:, j - 1] * self._sjnut[:, 0]
+        self._sjnut[:, j] = self._sjnut[:, j - 1] * self._cjnut[:,
+          0] + self._cjnut[:, j - 1] * self._sjnut[:, 0]
+
+      for k, ik in enumerate(self._series_index):
+        self._cov.A[ik] += np.sum(self._alpha[:, k] * self._alpha[:, k] +
+          self._beta[:, k] * self._beta[:, k])
+        self._cov.U[ik,
+          self._offset:self._offset + self._coef_rank] = self._alpha[0, k]
+        self._cov.U[ik, self._offset + self._coef_rank:self._offset +
+          self._nfreq * self._coef_rank] = (
+          self._alpha[1:, k] * self._cjnut[ik, :, np.newaxis] -
+          self._beta[1:, k] * self._sjnut[ik, :, np.newaxis]).reshape(
+          -1, self._nharm * self._coef_rank)
+        self._cov.U[ik,
+          self._offset + self._nfreq * self._coef_rank:self._offset +
+          self._r] = (self._alpha[1:, k] * self._sjnut[ik, :, np.newaxis] +
+          self._beta[1:, k] * self._cjnut[ik, :, np.newaxis]).reshape(
+          -1, self._nharm * self._coef_rank)
+    self._cov.V[:, self._offset:self._offset + self._r] = self._cov.U[:,
+      self._offset:self._offset + self._r]
+    self._cov.phi[:, self._offset:self._offset + self._r] = 1.0
+
+  def _get_param(self, par):
+    if par.startswith('alpha_'):
+      return (self._alpha[tuple(int(s) for s in par.split('_')[1:])])
+    elif par.startswith('beta_'):
+      return (self._beta[tuple(int(s) for s in par.split('_')[1:])])
+    else:
+      return (super()._get_param(par))
+
+  def _set_param(self, *args, **kwargs):
+    for karg, arg in enumerate(args):
+      par = self._param[karg]
+      if par in kwargs:
+        raise Exception(
+          f'MultiFourierKernel._set_param: parameter {par} multiply defined.')
+      kwargs[par] = arg
+
+    self._P = kwargs.get('P', self._P)
+    if self._vectorize:
+      self._alpha = kwargs.get('alpha', self._alpha)
+      self._beta = kwargs.get('beta', self._beta)
+    else:
+      for par in kwargs:
+        if par.startswith('alpha_'):
+          self._alpha[tuple(int(s) for s in par.split('_')[1:])] = kwargs[par]
+        elif par.startswith('beta_'):
+          self._beta[tuple(int(s) for s in par.split('_')[1:])] = kwargs[par]
+    if self._nharm > 0:
+      assert np.all(self._beta[0] == 0)
+
+  def _grad_param(self, grad_dU=None, grad_dV=None):
+    if grad_dU is not None or grad_dV is not None:
+      raise NotImplementedError()
+
+    grad = {}
+
+    grad_U = self._cov._grad_U[:, self._offset:self._offset +
+      self._r] + self._cov._grad_V[:, self._offset:self._offset + self._r]
+
+    if self._nharm > 0:
+      grad_nu = self._cov.t @ np.sum(
+        (grad_U[:, self._nfreq * self._coef_rank:] *
+        self._cov.U[:, self._offset + self._coef_rank:self._offset +
+        self._nfreq * self._coef_rank] -
+        grad_U[:, self._coef_rank:self._nfreq * self._coef_rank] *
+        self._cov.U[:, self._offset +
+        self._nfreq * self._coef_rank:self._offset + self._r]).reshape(
+        (-1, self._nharm, self._coef_rank)),
+        axis=2) @ np.arange(1, self._nfreq)
+      grad['P'] = -self._nu / self._P * grad_nu
+
+    grad_alpha = np.empty((self._nfreq, self._nseries, self._coef_rank))
+    grad_beta = np.empty((self._nfreq, self._nseries, self._coef_rank))
+    grad_beta[0] = 0
+    for k, ik in enumerate(self._series_index):
+      grad_A_k = np.sum(self._cov._grad_A[ik])
+      grad_alpha[:, k] = 2 * self._alpha[:, k] * grad_A_k
+      grad_alpha[0, k] += np.sum(grad_U[ik, :self._coef_rank], axis=0)
+      if self._nharm > 0:
+        grad_beta[1:, k] = 2 * self._beta[1:, k] * grad_A_k
+        grad_alpha[1:, k] += np.sum(self._cjnut[ik, :, np.newaxis] *
+          grad_U[ik, self._coef_rank:self._nfreq * self._coef_rank].reshape(
+          -1, self._nharm, self._coef_rank),
+          axis=0)
+        grad_beta[1:, k] -= np.sum(self._sjnut[ik, :, np.newaxis] *
+          grad_U[ik, self._coef_rank:self._nfreq * self._coef_rank].reshape(
+          -1, self._nharm, self._coef_rank),
+          axis=0)
+        grad_alpha[1:, k] += np.sum(self._sjnut[ik, :, np.newaxis] *
+          grad_U[ik, self._nfreq * self._coef_rank:].reshape(
+          -1, self._nharm, self._coef_rank),
+          axis=0)
+        grad_beta[1:, k] += np.sum(self._cjnut[ik, :, np.newaxis] *
+          grad_U[ik, self._nfreq * self._coef_rank:].reshape(
+          -1, self._nharm, self._coef_rank),
+          axis=0)
+    if self._vectorize:
+      grad['alpha'] = grad_alpha
+      if self._nharm > 0:
+        grad['beta'] = grad_beta
+    else:
+      for ndk in np.ndindex(grad_alpha.shape):
+        grad['alpha_' + '_'.join([f'{k}' for k in ndk])] = grad_alpha[ndk]
+        if self._nharm > 0:
+          grad['beta_' + '_'.join([f'{k}' for k in ndk])] = grad_beta[ndk]
+
+    return (grad)
+
+  def set_conditional_coef(self, alpha=None, beta=None, series_id=0):
+    r"""
+    Set the coefficients used for the conditional computations.
+
+    Parameters
+    ----------
+    alpha, beta : (nharm + 1, r) ndarray
+      Fourier coefficients for the conditional computation.
+      This is only used if series_id is None.
+    series_id : int
+      Use the coefficents corresponding to a given time series.
+    """
+
+    self._cond_series_id = series_id
+    if series_id is None:
+      self._cond_alpha = alpha
+      self._cond_beta = beta
+    else:
+      self._cond_alpha = None
+      self._cond_beta = None
+
+  def _compute_t2(self, t2, dt2, U2, V2, phi2, ref2left, dt2left, dt2right,
+    phi2left, phi2right):
+    if self._cond_series_id is None:
+      alpha = self._cond_alpha
+      beta = self._cond_beta
+    else:
+      alpha = self._alpha[:, self._cond_series_id]
+      if self._nharm > 0:
+        beta = self._beta[:, self._cond_series_id]
+
+    U2[:, self._offset:self._offset + self._coef_rank] = alpha[0]
+    if self._nharm > 0:
+      nut2 = self._nu * t2
+      cjnut2 = np.empty((t2.size, self._nharm))
+      sjnut2 = np.empty((t2.size, self._nharm))
+      cjnut2[:, 0] = np.cos(nut2)
+      sjnut2[:, 0] = np.sin(nut2)
+      for j in range(1, self._nharm):
+        cjnut2[:, j] = cjnut2[:, j - 1] * cjnut2[:, 0] - sjnut2[:,
+          j - 1] * sjnut2[:, 0]
+        sjnut2[:, j] = sjnut2[:, j - 1] * cjnut2[:, 0] + cjnut2[:,
+          j - 1] * sjnut2[:, 0]
+      U2[:, self._offset + self._coef_rank:self._offset +
+        self._nfreq * self._coef_rank] = (
+        alpha[1:] * cjnut2[:, :, np.newaxis] -
+        beta[1:] * sjnut2[:, :, np.newaxis]).reshape(
+        -1, self._nharm * self._coef_rank)
+      U2[:, self._offset + self._nfreq * self._coef_rank:self._offset +
+        self._r] = (alpha[1:] * sjnut2[:, :, np.newaxis] +
+        beta[1:] * cjnut2[:, :, np.newaxis]).reshape(
+        -1, self._nharm * self._coef_rank)
+    V2[:, self._offset:self._offset + self._r] = U2[:,
+      self._offset:self._offset + self._r]
+    phi2[:, self._offset:self._offset + self._r] = 1.0
+    phi2left[:, self._offset:self._offset + self._r] = 1.0
+    phi2right[:, self._offset:self._offset + self._r] = 1.0
+
+  def eval(self, dt, series_id=(0, 0)):
+    k = np.sum(self._alpha[0, series_id[0]] * self._alpha[0, series_id[1]])
+    if self._nharm > 0:
+      a = np.sum(
+        self._alpha[1:, series_id[0]] * self._alpha[1:, series_id[1]] +
+        self._beta[1:, series_id[0]] * self._beta[1:, series_id[1]],
+        axis=1)
+      b = np.sum(
+        self._alpha[1:, series_id[0]] * self._beta[1:, series_id[1]] -
+        self._beta[1:, series_id[0]] * self._alpha[1:, series_id[1]],
+        axis=1)
+
+      cjnudt = np.empty((dt.size, self._nharm))
+      sjnudt = np.empty((dt.size, self._nharm))
+      nudt = self._nu * dt
+      cjnudt[:, 0] = np.cos(nudt)
+      sjnudt[:, 0] = np.sin(nudt)
+      for j in range(1, self._nharm):
+        cjnudt[:, j] = cjnudt[:, j - 1] * cjnudt[:, 0] - sjnudt[:,
+          j - 1] * sjnudt[:, 0]
+        sjnudt[:, j] = sjnudt[:, j - 1] * cjnudt[:, 0] + cjnudt[:,
+          j - 1] * sjnudt[:, 0]
+      k += cjnudt @ a + sjnudt @ b
+    return (k)
```

### Comparing `spleaf-2.1.2/spleaf.egg-info/PKG-INFO` & `spleaf-2.1.3/spleaf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleaf
-Version: 2.1.2
+Version: 2.1.3
 Summary: Symmetric S+LEAF matrix.
 Home-page: https://gitlab.unige.ch/jean-baptiste.delisle/spleaf
 Author: Jean-Baptiste Delisle
 Author-email: jean-baptiste.delisle@unige.ch
 License: GPLv3
 Requires-Python: >=3.6
 License-File: COPYING
```

### Comparing `spleaf-2.1.2/test/test_cov.py` & `spleaf-2.1.3/test/test_cov.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.2/test/test_spleaf.py` & `spleaf-2.1.3/test/test_spleaf.py`

 * *Files identical despite different names*

