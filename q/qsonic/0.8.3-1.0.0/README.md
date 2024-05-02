# Comparing `tmp/qsonic-0.8.3.tar.gz` & `tmp/qsonic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.8.3.tar", last modified: Fri Jan 19 21:09:12 2024, max compression
+gzip compressed data, was "qsonic-1.0.0.tar", last modified: Thu May  2 14:37:28 2024, max compression
```

## Comparing `qsonic-0.8.3.tar` & `qsonic-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:09:12.450251 qsonic-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-19 21:08:58.000000 qsonic-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-01-19 21:09:12.450251 qsonic-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-01-19 21:08:58.000000 qsonic-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:09:12.446251 qsonic-0.8.3/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:09:12.446251 qsonic-0.8.3/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    19805 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    56482 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:09:12.450251 qsonic-0.8.3/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    30764 2024-01-19 21:08:58.000000 qsonic-0.8.3/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:09:12.450251 qsonic-0.8.3/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-01-19 21:09:12.000000 qsonic-0.8.3/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-19 21:09:12.000000 qsonic-0.8.3/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 21:09:12.000000 qsonic-0.8.3/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-19 21:09:12.000000 qsonic-0.8.3/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-19 21:09:12.000000 qsonic-0.8.3/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-19 21:09:12.000000 qsonic-0.8.3/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-19 21:08:58.000000 qsonic-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-19 21:08:58.000000 qsonic-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-19 21:09:12.454251 qsonic-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 21:08:58.000000 qsonic-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:09:12.450251 qsonic-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-01-19 21:08:58.000000 qsonic-0.8.3/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:37:28.443253 qsonic-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 14:37:19.000000 qsonic-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-02 14:37:28.443253 qsonic-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-02 14:37:19.000000 qsonic-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:37:28.435253 qsonic-1.0.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:37:28.439253 qsonic-1.0.0/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56545 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:37:28.443253 qsonic-1.0.0/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/scripts/qsonic_coadd_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34753 2024-05-02 14:37:19.000000 qsonic-1.0.0/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:37:28.443253 qsonic-1.0.0/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-02 14:37:28.000000 qsonic-1.0.0/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-02 14:37:28.000000 qsonic-1.0.0/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:37:28.000000 qsonic-1.0.0/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 14:37:28.000000 qsonic-1.0.0/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 14:37:28.000000 qsonic-1.0.0/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 14:37:28.000000 qsonic-1.0.0/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 14:37:19.000000 qsonic-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 14:37:19.000000 qsonic-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 14:37:28.443253 qsonic-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:37:19.000000 qsonic-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:37:28.443253 qsonic-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-02 14:37:19.000000 qsonic-1.0.0/tests/test_spectrum.py
```

### Comparing `qsonic-0.8.3/LICENSE` & `qsonic-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/PKG-INFO` & `qsonic-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.8.3
+Version: 1.0.0
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: numpy~=1.24.0
-Requires-Dist: numba~=0.57.0
-Requires-Dist: scipy~=1.10.0
-Requires-Dist: astropy~=5.2.0
+Requires-Dist: numpy~=1.26.0
+Requires-Dist: numba~=0.58.1
+Requires-Dist: scipy~=1.12.0
+Requires-Dist: astropy~=6.0.0
 Requires-Dist: healpy~=1.16.0
-Requires-Dist: fitsio~=1.1.0
+Requires-Dist: fitsio~=1.1.9
 Requires-Dist: iminuit~=2.18.0
 Requires-Dist: mpi4py
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Provides-Extra: doc
@@ -53,15 +53,15 @@
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms can be performed after continuum fitting or disabled entirely.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
-- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
+- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled by passing ``--var-fit-eta``. A covariance matrix is calculated based on delete-one Jackknife over subsamples between var_pipe and var_obs data points, and used in var_lss, eta fitting if ``--var-use-cov`` passed (soft recommendation to always enable this).
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
 + Delta files are the same. ``CONT`` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
```

### Comparing `qsonic-0.8.3/README.rst` & `qsonic-1.0.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms can be performed after continuum fitting or disabled entirely.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
-- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
+- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled by passing ``--var-fit-eta``. A covariance matrix is calculated based on delete-one Jackknife over subsamples between var_pipe and var_obs data points, and used in var_lss, eta fitting if ``--var-use-cov`` passed (soft recommendation to always enable this).
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
 + Delta files are the same. ``CONT`` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
```

### Comparing `qsonic-0.8.3/py/qsonic/calibration.py` & `qsonic-1.0.0/py/qsonic/calibration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Calibration module for noise and flux. """
 import argparse
 
 import fitsio
 import numpy as np
 
 from qsonic.mathtools import (
-    FastCubic1DInterp, FastLinear1DInterp, _zero_function)
+    FastCubic1DInterp, FastLinear1DInterp, _one_function)
 from qsonic.mpi_utils import mpi_fnc_bcast
 
 
 def add_calibration_parser(parser=None):
     """ Adds calibration related arguments to parser. These arguments are
     grouped under 'Noise and flux calibation options'.
 
@@ -28,15 +28,15 @@
     calib_group = parser.add_argument_group(
         'Noise and flux calibation options')
 
     calib_group.add_argument(
         "--noise-calibration", help="Noise calibration file.")
     calib_group.add_argument(
         "--varlss-as-additive-noise", action="store_true",
-        help="var_lss as additive noise term.")
+        help="var_lss as additive noise term after continuum fitting.")
     calib_group.add_argument(
         "--flux-calibration", help="Flux calibration file.")
 
     return parser
 
 
 class NoiseCalibrator():
@@ -54,14 +54,17 @@
     ----------
     fname: str
         Filename to read by ``fitsio``.
     comm: None or MPI.COMM_WORLD, default: None
     mpi_rank: int, default: 0
     add_varlss: bool, default: False
         Use var_lss as an additive correction to noise in observed frame.
+        Requires continuum.
+    no_eta: bool, default: False
+        Turns off eta scaling by using eta=1.
 
     Attributes
     ----------
     eta_interp: FastCubic1DInterp
         Eta interpolator.
     """
 
@@ -83,38 +86,56 @@
 
         eta = np.array(data['eta'], dtype='d')
         eta[eta == 0] = 1
         eta_interp = FastCubic1DInterp(waves_0, dwave, eta)
 
         return eta_interp, varlss_interp
 
-    def __init__(self, fname, comm=None, mpi_rank=0, add_varlss=False):
+    def __init__(
+            self, fname, comm=None, mpi_rank=0,
+            add_varlss=False, no_eta=False
+    ):
         self.eta_interp, self.varlss_interp = mpi_fnc_bcast(
             self._read, comm, mpi_rank,
             f"Error loading NoiseCalibrator from file {fname}.",
             fname)
 
         if not add_varlss:
-            self.varlss_interp = _zero_function
+            self.varlss_interp = None
+
+        if no_eta:
+            self.eta_interp = _one_function
 
     def apply(self, spectra_list):
         """ Apply the noise calibration by **only** scaling
         :attr:`forestivar <qsonic.spectrum.Spectrum.forestivar>`. Smooth
         component must be set after this.
 
         Arguments
         ----------
         spectra_list: list(Spectrum)
             Spectrum objects to noise calibrate.
         """
-        for spec in spectra_list:
-            for arm, wave_arm in spec.forestwave.items():
-                eta = self.eta_interp(wave_arm)
-                varlss = self.varlss_interp(wave_arm)
-                spec.forestivar[arm] /= (eta + spec.forestivar[arm] * varlss)
+        if self.varlss_interp:
+            if not all(spec.cont_params['cont'] for spec in spectra_list):
+                raise Exception(
+                    "NoiseCalibrator needs continuum for additive correction.")
+
+            for spec in spectra_list:
+                for arm, wave_arm in spec.forestwave.items():
+                    eta = self.eta_interp(wave_arm)
+                    vlss = self.varlss_interp(wave_arm)
+                    vlss *= spec.cont_params['cont'][arm]**2
+                    spec.forestivar[arm] /= (eta + spec.forestivar[arm] * vlss)
+                    spec.forestivar[arm][spec.forestivar[arm] < 0] = 0
+        else:
+            for spec in spectra_list:
+                for arm, wave_arm in spec.forestwave.items():
+                    eta = self.eta_interp(wave_arm)
+                    spec.forestivar[arm] /= eta
 
 
 class FluxCalibrator():
     """ Flux calibration object.
 
     .. math::
```

### Comparing `qsonic-0.8.3/py/qsonic/catalog.py` & `qsonic-1.0.0/py/qsonic/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     set(['SURVEY']),
     set(['COADD_LASTNIGHT', 'LAST_NIGHT', 'LASTNIGHT'])
 ]
 """list(set): Required columns for real data analysis."""
 _required_tile_columns = [set(['TILEID']), set(['PETAL_LOC'])]
 """list(set): Required columns for tile data analysis."""
 _optional_columns = [
-    'HPXPIXEL', 'VMIN_CIV_450', 'VMAX_CIV_450', 'VMIN_CIV_2000',
+    'HPXPIXEL', 'PROGRAM', 'VMIN_CIV_450', 'VMAX_CIV_450', 'VMIN_CIV_2000',
     'VMAX_CIV_2000'
 ]
 """list(str): Optional columns."""
 _all_columns = [
     col for reqset in (
         _required_columns + _required_data_columns + _required_tile_columns
     ) for col in reqset
```

### Comparing `qsonic-0.8.3/py/qsonic/io.py` & `qsonic-1.0.0/py/qsonic/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,15 +604,16 @@
         catalog_hpx = catalog_hpx[idx_cat]
 
     fspec = f"{input_dir}/{pixnum//100}/{pixnum}/truth-{nside}-{pixnum}.fits"
     if read_true_continuum:
         data['cont'] = _read_true_continuum(catalog_hpx['TARGETID'], fspec)
 
     if skip_resomat:
-        return qsonic.spectrum.generate_spectra_list_from_data(catalog_hpx, data)
+        return qsonic.spectrum.generate_spectra_list_from_data(
+            catalog_hpx, data)
 
     with fitsio.FITS(fspec) as fitsfile:
         for arm in arms_to_keep:
             data['reso'][arm] = np.array(fitsfile[f'{arm}_RESOLUTION'].read())
 
     return qsonic.spectrum.generate_spectra_list_from_data(catalog_hpx, data)
```

### Comparing `qsonic-0.8.3/py/qsonic/masks.py` & `qsonic-1.0.0/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/py/qsonic/mathtools.py` & `qsonic-1.0.0/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/py/qsonic/mpi_utils.py` & `qsonic-1.0.0/py/qsonic/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/py/qsonic/picca_continuum.py` & `qsonic-1.0.0/py/qsonic/picca_continuum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1094,15 +1094,18 @@
             Wavelength array.
         delta: :external+numpy:py:class:`ndarray <numpy.ndarray>`
             Delta array.
         ivar: :external+numpy:py:class:`ndarray <numpy.ndarray>`
             Inverse variance array.
         """
         # add 1 to match searchsorted/bincount output/input
-        wave_indx = ((wave - self.waveobs[0]) / self.dwobs + 1.5).astype(int)
+        wave_indx = np.clip(
+            ((wave - self.waveobs[0]) / self.dwobs + 1.5).astype(int),
+            0, self.nwbins + 1
+        )
         ivar_indx = np.searchsorted(self.ivar_edges, ivar)
         all_indx = ivar_indx + wave_indx * (self.nvarbins + 2)
         var = np.zeros_like(ivar)
         w = ivar > 0
         var[w] = 1. / ivar[w]
 
         npix = np.bincount(all_indx, minlength=self.minlength)
```

### Comparing `qsonic-0.8.3/py/qsonic/scripts/qsonic_calib.py` & `qsonic-1.0.0/py/qsonic/scripts/qsonic_calib.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     deltas_list = mpi_read_all_deltas(args, comm, mpi_rank, mpi_size)
     # Flatten this list of lists and remove quasars
     deltas_list = [x for alist in deltas_list for x in alist if _is_kept(x)]
 
     for delta in deltas_list:
         varfitter.add(delta.wave, delta.delta, delta.ivar)
 
-    logging.info("Fitting variance for VarLSS and eta")
+    logging.info("Fitting var_lss and eta")
     fit_results = np.ones((varfitter.nwbins, 2))
     fit_results[:, 0] = 0.1
     fit_results, std_results = varfitter.fit(fit_results)
 
     # Save variance stats to file
     logging.info("Saving variance stats to files")
     suffix = f"snr{args.min_snr:.1f}-{args.max_snr:.1f}"
```

### Comparing `qsonic-0.8.3/py/qsonic/scripts/qsonic_fit.py` & `qsonic-1.0.0/py/qsonic/scripts/qsonic_fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,18 +139,18 @@
     logging.info(f"All {nspec_all} spectra are read in {etime:.1f} mins.")
 
     return spectra_list
 
 
 def mpi_noise_flux_calibrate(spectra_list, args, comm, mpi_rank):
     if args.noise_calibration:
-        logging.info("Applying noise calibration.")
+        logging.info("Applying noise calibration (eta only).")
         ncal = qsonic.calibration.NoiseCalibrator(
             args.noise_calibration, comm, mpi_rank,
-            args.varlss_as_additive_noise)
+            add_varlss=False)
         ncal.apply(spectra_list)
 
     if args.flux_calibration:
         logging.info("Applying flux calibration.")
         fcal = qsonic.calibration.FluxCalibrator(
             args.flux_calibration, comm, mpi_rank)
         fcal.apply(spectra_list)
@@ -267,24 +267,38 @@
         # Iterate
         logging.info("Fitting continuum.")
         qcfit.iterate(spectra_list)
     else:
         logging.info("True continuum.")
         qcfit.true_continuum(spectra_list, args)
 
+    valid_spectra = list(qsonic.spectrum.valid_spectra(spectra_list))
+
+    # Final noise calibration for additive var_lss.
+    if args.noise_calibration and args.varlss_as_additive_noise:
+        logging.info("Applying noise calibration (varlss only).")
+        ncal = qsonic.calibration.NoiseCalibrator(
+            args.noise_calibration, comm, mpi_rank,
+            add_varlss=True, no_eta=True)
+        ncal.apply(valid_spectra)
+
+        for spec in valid_spectra:
+            spec.set_smooth_forestivar(spec._smoothing_scale)
+            spec.set_forest_weight(qcfit.varlss_interp, qcfit.eta_interp)
+
     if args.coadd_arms == "after":
         logging.info("Coadding arms.")
-        for spec in qsonic.spectrum.valid_spectra(spectra_list):
+        for spec in valid_spectra:
             spec.coadd_arms_forest(qcfit.varlss_interp, qcfit.eta_interp)
             spec.calc_continuum_chi2()
 
     qcfit.save_contchi2_catalog(spectra_list)
 
     # Keep only valid spectra
-    spectra_list = list(qsonic.spectrum.valid_spectra(spectra_list))
+    spectra_list = valid_spectra
 
     # Final cleaning. Especially important if not coadding arms.
     for spec in spectra_list:
         spec.drop_short_arms(args.forest_w1, args.forest_w2, args.skip)
 
     etime = (time.time() - start_time) / 60  # min
     logging.info(f"Continuum fitting and tweaking took {etime:.1f} mins.")
```

### Comparing `qsonic-0.8.3/py/qsonic/spectrum.py` & `qsonic-1.0.0/py/qsonic/spectrum.py`

 * *Files 10% similar despite different names*

```diff
@@ -718,14 +718,15 @@
 
             hdr_dict['MEANSNR'] = self.mean_snr[arm]
 
             cont_est = self.cont_params['cont'][arm]
             delta = self.forestflux[arm] / cont_est - 1
             ivar = self.forestivar[arm] * cont_est**2
             weight = self.forestweight[arm] * cont_est**2
+            delta[ivar == 0] = 0
 
             cols = [wave_arm, delta, ivar, weight, cont_est]
             if self.forestreso:
                 hdr_dict['MEANRESO'] = self.mean_resolution(arm)
                 cols.append(self.forestreso[arm].T.astype('f8'))
 
             fts_file.write(
@@ -834,14 +835,16 @@
         Deltas.
     ivar: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Inverse variance.
     weight: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Weights, which includes var_lss.
     cont: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Continuum.
+    reso: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        Resolution matrix. ``None`` if not present.
     header: FITS header
         Header.
     targetid: int
         TARGETID, MOCKID or THING_ID from header.
     mean_snr: float
         MEANSNR from header.
     """
@@ -885,11 +888,127 @@
         key = Delta._check_hdu(colnames, "wave")
         if key == "LOGLAM":
             self.wave = 10**data['LOGLAM']
         else:
             self.wave = data[key].astype("f8")
 
         key = Delta._check_hdu(colnames, "delta")
+        self._is_blinded = key == "DELTA_BLIND"
         self.delta = data[key].astype("f8")
         self.ivar = data['IVAR'].astype("f8")
         self.weight = data['WEIGHT'].astype("f8")
         self.cont = data['CONT'].astype("f8")
+
+        self.delta[self.ivar == 0] = 0
+
+        if 'RESOMAT' in colnames:
+            self.reso = data['RESOMAT'].T.astype("f8")
+        else:
+            self.reso = None
+
+    def write(self, fts_file):
+        """Writes to FITS file. This function is aimed at saving coadded
+        deltas.
+
+        Writes 'LAMBDA', 'DELTA', 'IVAR', 'WEIGHT', 'CONT' columns and
+        'RESOMAT' column if resolution matrix is present to extension name
+        ``targetid``. FITS file must be initialized before. Note that ``arm``
+        is lost in the extension name.
+
+        Arguments
+        ---------
+        fts_file: FITS file
+            The file handler, not filename.
+        """
+        hdr_dict = self.header
+
+        cols = [self.wave, self.delta, self.ivar, self.weight, self.cont]
+        names = ['LAMBDA', 'DELTA', 'IVAR', 'WEIGHT', 'CONT']
+
+        if self._is_blinded:
+            names[1] = 'DELTA_BLIND'
+
+        if self.reso is not None:
+            cols.append(self.reso.T)
+            names.append('RESOMAT')
+
+        fts_file.write(
+            cols, names=names, header=hdr_dict,
+            extname=f"{self.targetid}")
+
+    def _coadd_reso(self, other, nwaves, idxes):
+        max_ndia = max(self.reso.shape[0], other.reso.shape[0])
+        coadd_reso = np.zeros((max_ndia, nwaves))
+        coadd_norm = np.zeros(nwaves)
+
+        for j, obj in enumerate([self, other]):
+            weight = obj.weight.copy()
+            weight[weight == 0] = 1e-8
+
+            ddia = max_ndia - obj.reso.shape[0]
+            # Assumption ddia cannot be odd
+            ddia = ddia // 2
+            if ddia > 0:
+                obj.reso = np.pad(obj.reso, ((ddia, ddia), (0, 0)))
+
+            coadd_reso[:, idxes[j]] += weight * obj.reso
+            coadd_norm[idxes[j]] += weight
+
+        coadd_reso /= coadd_norm
+        self.reso = coadd_reso
+
+    def coadd(self, other, dwave=0.8):
+        min_wave = min(self.wave[0], other.wave[0])
+        max_wave = max(self.wave[-1], other.wave[-1])
+
+        nwaves = int((max_wave - min_wave) / dwave + 0.1) + 1
+        coadd_wave = np.linspace(min_wave, max_wave, nwaves)
+        coadd_delta = np.zeros(nwaves)
+        coadd_ivar = np.zeros(nwaves)
+        coadd_lss = np.zeros(nwaves)
+        coadd_cont = np.zeros(nwaves)
+        coadd_norm = np.zeros(nwaves)
+
+        idxes = [None, None]
+        for j, obj in enumerate([self, other]):
+            i0 = ((obj.wave[0] - min_wave) / dwave + 0.1).astype(int)
+            idx = np.s_[i0:i0 + obj.wave.size]
+            idxes[j] = idx
+
+            var = np.zeros_like(obj.weight)
+            w = (obj.weight > 0) & (obj.ivar > 0)
+            var[w] = 1 / obj.ivar[w]
+
+            coadd_delta[idx] += obj.weight * obj.delta
+            coadd_cont[idx] += obj.weight * obj.cont
+            coadd_ivar[idx] += obj.weight**2 * var
+            coadd_lss[idx] += 1 - obj.weight * var
+            coadd_norm[idx] += obj.weight
+
+        w = coadd_norm > 0
+        coadd_delta[w] /= coadd_norm[w]
+        coadd_cont[w] /= coadd_norm[w]
+        coadd_lss[w] /= coadd_norm[w]
+        coadd_ivar[w] = coadd_norm[w]**2 / coadd_ivar[w]
+
+        if self.reso is not None:
+            self._coadd_reso(other, nwaves, idxes)
+
+        self.wave = coadd_wave
+        self.delta = coadd_delta
+        self.ivar = coadd_ivar
+        self.weight = self.ivar / (1 + self.ivar * coadd_lss)
+        self.cont = coadd_cont
+
+        self.mean_snr = np.dot(
+            np.sqrt(coadd_ivar), coadd_delta + 1) / np.sum(coadd_ivar > 0)
+        self.header['MEANSNR'] = self.mean_snr
+
+    @property
+    def ra(self):
+        """float: Right ascension in degrees."""
+        return np.degrees(self.header['RA'])
+
+    @property
+    def dec(self):
+        """float: Declination in degrees"""
+        return np.degrees(self.header['DEC'])
```

### Comparing `qsonic-0.8.3/py/qsonic.egg-info/PKG-INFO` & `qsonic-1.0.0/py/qsonic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.8.3
+Version: 1.0.0
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: numpy~=1.24.0
-Requires-Dist: numba~=0.57.0
-Requires-Dist: scipy~=1.10.0
-Requires-Dist: astropy~=5.2.0
+Requires-Dist: numpy~=1.26.0
+Requires-Dist: numba~=0.58.1
+Requires-Dist: scipy~=1.12.0
+Requires-Dist: astropy~=6.0.0
 Requires-Dist: healpy~=1.16.0
-Requires-Dist: fitsio~=1.1.0
+Requires-Dist: fitsio~=1.1.9
 Requires-Dist: iminuit~=2.18.0
 Requires-Dist: mpi4py
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Provides-Extra: doc
@@ -53,15 +53,15 @@
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms can be performed after continuum fitting or disabled entirely.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
-- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
+- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled by passing ``--var-fit-eta``. A covariance matrix is calculated based on delete-one Jackknife over subsamples between var_pipe and var_obs data points, and used in var_lss, eta fitting if ``--var-use-cov`` passed (soft recommendation to always enable this).
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
 + Delta files are the same. ``CONT`` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
```

### Comparing `qsonic-0.8.3/py/qsonic.egg-info/SOURCES.txt` & `qsonic-1.0.0/py/qsonic.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 py/qsonic.egg-info/PKG-INFO
 py/qsonic.egg-info/SOURCES.txt
 py/qsonic.egg-info/dependency_links.txt
 py/qsonic.egg-info/entry_points.txt
 py/qsonic.egg-info/requires.txt
 py/qsonic.egg-info/top_level.txt
 py/qsonic/scripts/qsonic_calib.py
+py/qsonic/scripts/qsonic_coadd_deltas.py
 py/qsonic/scripts/qsonic_fit.py
 tests/test_calibration.py
 tests/test_catalog.py
 tests/test_io.py
 tests/test_masks.py
 tests/test_mathtools.py
 tests/test_mpi_utils.py
```

### Comparing `qsonic-0.8.3/setup.cfg` & `qsonic-1.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.3
+current_version = 1.0.0
 commit = True
 tag = False
 message = [skip ci] Bump version: {current_version} → {new_version}
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
@@ -21,24 +21,25 @@
 	Documentation=http://qsonic.readthedocs.io/
 	Source=https://github.com/p-slash/qsonic
 
 [options]
 package_dir = 
 	=py
 packages = find_namespace:
-python_requires = >=3.7, <3.11
+python_requires = >=3.7
 install_requires = file: requirements.txt
 
 [options.packages.find]
 where = py
 
 [options.entry_points]
 console_scripts = 
 	qsonic-fit = qsonic.scripts.qsonic_fit:main
 	qsonic-calib = qsonic.scripts.qsonic_calib:main
+	qsonic-coadd = qsonic.scripts.qsonic_coadd_deltas:main
 
 [options.extras_require]
 dev = 
 	pytest
 	flake8
 	bump2version
 doc =
```

### Comparing `qsonic-0.8.3/tests/test_calibration.py` & `qsonic-1.0.0/tests/test_calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,21 @@
     spec = spectra_list[0]
     spec.set_forest_region(3600., 6000., 1050., 1300.)
     f0 = spec.flux['B'][0]
 
     ncal.apply(spectra_list)
     npt.assert_allclose(spec.forestivar['B'], 0.5)
     npt.assert_allclose(spec.forestivar['R'], 0.5)
+
+    with pytest.raises(Exception):
+        ncal_plus.apply(spectra_list)
+
+    spec.cont_params['cont'] = {
+        arm: np.ones_like(flux) for arm, flux in spec.forestflux.items()
+    }
     ncal_plus.apply(spectra_list)
     npt.assert_allclose(spec.forestivar['B'], 0.2)
     npt.assert_allclose(spec.forestivar['R'], 0.2)
 
     fcal.apply(spectra_list)
     npt.assert_allclose(spec.forestflux['B'], f0 / 5)
     npt.assert_allclose(spec.forestflux['R'], f0 / 5)
```

### Comparing `qsonic-0.8.3/tests/test_catalog.py` & `qsonic-1.0.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/tests/test_io.py` & `qsonic-1.0.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/tests/test_masks.py` & `qsonic-1.0.0/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/tests/test_mathtools.py` & `qsonic-1.0.0/tests/test_mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/tests/test_mpi_utils.py` & `qsonic-1.0.0/tests/test_mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/tests/test_picca_continuum.py` & `qsonic-1.0.0/tests/test_picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/tests/test_qsonic_calib.py` & `qsonic-1.0.0/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.8.3/tests/test_qsonic_fit.py` & `qsonic-1.0.0/tests/test_qsonic_fit.py`

 * *Files identical despite different names*

