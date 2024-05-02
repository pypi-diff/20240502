# Comparing `tmp/labcodes-1.0.0.tar.gz` & `tmp/labcodes-1.0.1.tar.gz`

## Comparing `labcodes-1.0.0.tar` & `labcodes-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0   131011 2020-02-02 00:00:00.000000 labcodes-1.0.0/examples/Q_of_LC_CCoupled.ipynb
--rw-r--r--   0        0        0   122313 2020-02-02 00:00:00.000000 labcodes-1.0.0/examples/Q_of_LC_MCoupled.ipynb
--rw-r--r--   0        0        0   189862 2020-02-02 00:00:00.000000 labcodes-1.0.0/examples/all you need is pandas.ipynb
--rw-r--r--   0        0        0   195390 2020-02-02 00:00:00.000000 labcodes-1.0.0/examples/fitter_basic.ipynb
--rw-r--r--   0        0        0   143137 2020-02-02 00:00:00.000000 labcodes-1.0.0/examples/plot2d.ipynb
--rw-r--r--   0        0        0   193473 2020-02-02 00:00:00.000000 labcodes-1.0.0/examples/state_discrimination.ipynb
--rw-r--r--   0        0        0   290921 2020-02-02 00:00:00.000000 labcodes-1.0.0/examples/tomo.ipynb
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/__about__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/__init__.py
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/crosstalk.py
--rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/enr_cross.py
--rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fit_resonator.py
--rw-r--r--   0        0        0    24134 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fitter.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/misc.py
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/models.py
--rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/state_disc.py
--rw-r--r--   0        0        0    33230 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/tomo.py
--rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/app/mat_editor.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/calc/__init__.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/calc/base.py
--rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/calc/qubits.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/calc/resonator_qc.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fileio/__init__.py
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fileio/base.py
--rw-r--r--   0        0        0    23160 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fileio/labber.py
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fileio/labrad.py
--rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fileio/ltspice.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/fileio/misc.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/benchmark.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/iq_scatter.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/labrad_timefunc2freq.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/pulse_calc.py
--rw-r--r--   0        0        0    35424 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/routine.py
--rw-r--r--   0        0        0    57486 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/state_list.py
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/tele.py
--rw-r--r--   0        0        0    10784 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/tele_gate.py
--rw-r--r--   0        0        0    15959 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/tele_state.py
--rw-r--r--   0        0        0    30003 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/frog/tele_swep.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/plotter/__init__.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/plotter/matrix.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/plotter/misc.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 labcodes-1.0.0/labcodes/plotter/plot2d.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 labcodes-1.0.0/tests/rt_qst_qpt.py
--rw-r--r--   0        0        0    83813 2020-02-02 00:00:00.000000 labcodes-1.0.0/tests/data/00003 - power shift.csv
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 labcodes-1.0.0/tests/data/00003 - power shift.ini
--rw-r--r--   0        0        0    71586 2020-02-02 00:00:00.000000 labcodes-1.0.0/tests/data/fit_resonator.feather
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 labcodes-1.0.0/.gitignore
--rw-r--r--   0        0        0    35813 2020-02-02 00:00:00.000000 labcodes-1.0.0/LICENSE
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 labcodes-1.0.0/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 labcodes-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 labcodes-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0   131011 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/Q_of_LC_CCoupled.ipynb
+-rw-r--r--   0        0        0   122313 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/Q_of_LC_MCoupled.ipynb
+-rw-r--r--   0        0        0   189862 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/all you need is pandas.ipynb
+-rw-r--r--   0        0        0   195390 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/fitter_basic.ipynb
+-rw-r--r--   0        0        0   143137 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/plot2d.ipynb
+-rw-r--r--   0        0        0   193473 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/state_discrimination.ipynb
+-rw-r--r--   0        0        0   290921 2020-02-02 00:00:00.000000 labcodes-1.0.1/examples/tomo.ipynb
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/__about__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/__init__.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/crosstalk.py
+-rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/enr_cross.py
+-rw-r--r--   0        0        0    13557 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fit_resonator.py
+-rw-r--r--   0        0        0    24134 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fitter.py
+-rw-r--r--   0        0        0    16865 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/misc.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/models.py
+-rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/state_disc.py
+-rw-r--r--   0        0        0    33230 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/tomo.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/app/mat_editor.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/__init__.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/base.py
+-rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/qubits.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/calc/resonator_qc.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/__init__.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/base.py
+-rw-r--r--   0        0        0    23160 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/labber.py
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/labrad.py
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/ltspice.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/fileio/misc.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/benchmark.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/iq_scatter.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/labrad_timefunc2freq.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/pulse_calc.py
+-rw-r--r--   0        0        0    35424 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/routine.py
+-rw-r--r--   0        0        0    57486 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/state_list.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele.py
+-rw-r--r--   0        0        0    10784 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele_gate.py
+-rw-r--r--   0        0        0    15959 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele_state.py
+-rw-r--r--   0        0        0    30003 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/frog/tele_swep.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/__init__.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/matrix.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/misc.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 labcodes-1.0.1/labcodes/plotter/plot2d.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/rt_qst_qpt.py
+-rw-r--r--   0        0        0    83813 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/data/00003 - power shift.csv
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/data/00003 - power shift.ini
+-rw-r--r--   0        0        0    71586 2020-02-02 00:00:00.000000 labcodes-1.0.1/tests/data/fit_resonator.feather
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 labcodes-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35813 2020-02-02 00:00:00.000000 labcodes-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 labcodes-1.0.1/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 labcodes-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 labcodes-1.0.1/PKG-INFO
```

### Comparing `labcodes-1.0.0/examples/Q_of_LC_CCoupled.ipynb` & `labcodes-1.0.1/examples/Q_of_LC_CCoupled.ipynb`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/examples/Q_of_LC_MCoupled.ipynb` & `labcodes-1.0.1/examples/Q_of_LC_MCoupled.ipynb`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/examples/all you need is pandas.ipynb` & `labcodes-1.0.1/examples/all you need is pandas.ipynb`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/examples/fitter_basic.ipynb` & `labcodes-1.0.1/examples/fitter_basic.ipynb`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/examples/plot2d.ipynb` & `labcodes-1.0.1/examples/plot2d.ipynb`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/examples/state_discrimination.ipynb` & `labcodes-1.0.1/examples/state_discrimination.ipynb`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/examples/tomo.ipynb` & `labcodes-1.0.1/examples/tomo.ipynb`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/crosstalk.py` & `labcodes-1.0.1/labcodes/crosstalk.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/enr_cross.py` & `labcodes-1.0.1/labcodes/enr_cross.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/fit_resonator.py` & `labcodes-1.0.1/labcodes/fit_resonator.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from labcodes import misc, plotter
 
 logger = logging.getLogger(__file__)
 
 
 def s21m1(x, Qi=1e6, Qc=1e3, f0=4, phi=0, alpha=-50, phiv=10, phi0=0, amp=1):
     """Normalized s21^-1 for linear resonator.
-    
+
     Original paper see https://doi.org/10.1063/1.3693409
     Improved by Xiayu Linpeng.
     """
     Qc = Qc * np.exp(1j * phi)
     s21m1 = 1 + (Qi / Qc / (1 + 2j * Qi * (x - f0) / f0))
     bg_amp = amp / (1 + alpha * (x - f0) / f0)
     bg_phase = np.exp(1j * (phiv * (x - f0) + phi0))
@@ -25,47 +25,51 @@
 
 
 model = lmfit.Model(s21m1)
 
 
 def n_photon(f0_Hz, Qi, Qc, p_dBm):
     """Returns photon number in the resonator.
-    
+
     See https://doi.org/10.1063/1.4919761
     """
     p_watt = 10 ** (p_dBm / 10) / 1000
     wr = 2 * np.pi * f0_Hz
-    n = 2 / (const.hbar * wr**2) * Qc * (Qi / (Qi + Qc))**2 * p_watt
+    n = 2 / (const.hbar * wr**2) * Qc * (Qi / (Qi + Qc)) ** 2 * p_watt
     return n
 
 
 class FitResonator:
     """Fit the s21 data of linear resonator side loaded to feedline.
-    
+
     Adapted from:
     1. https://lmfit.github.io/lmfit-py/examples/example_complex_resonator_model.html
     2. programs by Xiayu Linpeng.
     """
-    def __init__(self, freq: np.ndarray, s21_dB: np.ndarray, s21_rad: np.ndarray, **fit_kws):
+
+    def __init__(
+        self, freq: np.ndarray, s21_dB: np.ndarray, s21_rad: np.ndarray, **fit_kws
+    ):
         """fit(Qi=1e6) to overwrite initial guess."""
         # Normalize data with y0=0.
-        s21_dB = misc.remove_background(s21_dB, freq, fit_mask=100, offset=0)
-        s21_rad = misc.remove_background(s21_rad, freq, fit_mask=100, offset=0)
+        s21_rad = np.unwrap(s21_rad)
+        s21_dB = remove_background(s21_dB, freq, fit_mask=100, offset=0)
+        s21_rad = remove_background(s21_rad, freq, fit_mask=100, offset=0)
         s21_cplx = 10 ** (s21_dB / 20) * np.exp(1j * s21_rad)
         s21m1_cplx = 1 / s21_cplx
         self.df = pd.DataFrame(
             dict(
                 freq=freq,
                 s21_dB=s21_dB,
                 s21_rad=s21_rad,
                 s21_cplx=s21_cplx,
                 s21m1_cplx=s21m1_cplx,
             )
         )
-        self.params = None
+        self.init_params = None
         self.guess_and_update_params()
         self.result: lmfit.minimizer.MinimizerResult = None
         try:
             self.fit(**fit_kws)
         except:
             logger.exception("Error in fitting.")
 
@@ -73,92 +77,77 @@
         """fit(Qi=1e6) to overwrite initial guess."""
         freq = self.df.freq.values
         s21m1_cplx = self.df.s21m1_cplx.values
 
         self.result = model.fit(
             s21m1_cplx,
             x=freq,
-            params=self.params,
-            weights=np.abs(s21m1_cplx) ** 2,
+            params=self.init_params,
+            # weights=np.abs(s21m1_cplx),  # not necessary.
             method="Powell",
             **fit_kws,
         )
         return self.result
 
     def guess_and_update_params(self):
         freq = self.df.freq.values
         s21_dB = self.df.s21_dB.values
         s21_cplx = self.df.s21_cplx.values
         s21m1_cplx = self.df.s21m1_cplx.values
 
         idip = np.argmin(s21_dB)
         fr = freq[idip]
 
-        # Guess Qc using Lorentz fit of S21
-        half_maximum = s21_dB[idip] + 3
-        fwhm = 0.2 * np.abs(  # Emprical value.
-            freq[np.argmin(np.abs(s21_dB[:idip] - half_maximum))]
-            - freq[np.argmin(np.abs(s21_dB[idip:] - half_maximum))]
-        )
-        Qc = np.abs(fr / fwhm)
-
-        # Guess Qi using Lorentz fit of S21^-1
-        half_maximum = (np.abs(s21m1_cplx[idip]) + 1) / 2
-        fwhm = 0.1 * np.abs(  # Emprical value.
-            freq[np.argmin(np.abs(s21m1_cplx[:idip]) - half_maximum)]
-            - freq[np.argmin(np.abs(s21m1_cplx[idip:]) - half_maximum)]
-        )
-        Qi = np.abs(fr / fwhm)
-        if np.mean(np.real(s21m1_cplx)) < 1:
-            Qi = -Qi
+        Qc = guess_Qc(s21_cplx, freq, fr, idip, s21_dB)
+        Qi = guess_Qi(s21m1_cplx, freq, fr, idip)
 
-        alpha = fr * (abs(s21_cplx[-1]) - abs(s21_cplx[0])) / (freq[-1] - freq[0])
-        phiv = np.angle(s21_cplx[-1] / s21_cplx[0]) / (freq[-1] - freq[0])
+        freq_span = freq[-1] - freq[0]
+        alpha = fr * (abs(s21_cplx[-1]) - abs(s21_cplx[0])) / freq_span
+        phiv = np.angle(s21m1_cplx[-1] / s21m1_cplx[0]) / freq_span
 
         params = lmfit.Parameters()
         params.set(Qi=Qi, Qc=Qc, f0=fr, phi=0, alpha=alpha, phiv=phiv, phi0=0, amp=1)
-        self.params = params
+        params.set(phiv=dict(min=-np.pi / freq_span, max=np.pi / freq_span))
+        self.init_params = params
         return params
 
     def __getitem__(self, key: str):
         if self.result is not None:
             if key == "chi":
                 return np.sqrt(self.result.chisqr)
             elif key.endswith("_err"):
                 return self.result.params[key[:-4]].stderr
             else:
                 return self.result.params[key].value
         else:
-            return self.params[key].value
-        
+            return self.init_params[key].value
+
     def n_photon(self, p_dBm, f0_Hz=None, Qi=None, Qc=None):
         """Returns photon number in the resonator.
-        
+
         See https://doi.org/10.1063/1.4919761
         """
         if f0_Hz is None:
             f0_Hz = self["f0"]
         if Qi is None:
             Qi = self["Qi"]
         if Qc is None:
             Qc = self["Qc"]
         return n_photon(f0_Hz, Qi, Qc, p_dBm)
 
     def plot_cplx(
         self,
         ax: plt.Axes = None,
         freq: np.ndarray = None,
+        plot_fit: bool = True,
         plot_init: bool = False,
-        plot_annotate: bool = True,
-        plot_orig: bool = True,
     ):
         if ax is None:
             _, ax = plt.subplots(figsize=(3, 3), layout="compressed")
-            ax.set_xlabel("Re[$S_{21}^{-1}$]")
-            ax.set_ylabel("Im[$S_{21}^{-1}$]")
+            setup_ax_cplx(ax)
         if freq is None:
             freq = self.df.freq.values
 
         f0 = self["f0"]
         Qi = self["Qi"]
         Qc = self["Qc"]
         dfi = f0 / Qi / 2
@@ -169,53 +158,45 @@
             mask1 = dx <= dfi
             mask3 = dx >= dfi * 10
             mask2 = np.logical_not(mask1 | mask3)
             ax.plot(y.real[mask1], y.imag[mask1], sty, color="C0", **kw)
             ax.plot(y.real[mask2], y.imag[mask2], sty, color="C1", **kw)
             ax.plot(y.real[mask3], y.imag[mask3], sty, color="C2", **kw)
 
-        ax.set_aspect("equal")
-
         plot(ax, self.df.freq.values, self.df.s21m1_cplx.values, ".", alpha=0.5)
-        if self.result is not None:
-            plot(ax, freq, self.result.eval(x=freq), "-")
-        if plot_init:
-            init_param = {k: p.init_value for k, p in self.result.params.items()}
-            plot(ax, freq, model.eval(x=freq, **init_param), "--")
 
-        if plot_annotate:
+        if (self.result is not None) and plot_fit:
+            plot(ax, freq, self.result.eval(x=freq), "-")
             ax.annotate(
                 f"$f_0$={misc.estr(f0)}\n$Q_i$={misc.estr(Qi)}\n$Q_c$={misc.estr(Qc)}",
                 (0.5, 0.5),
                 xycoords="axes fraction",
                 ha="center",
                 va="center",
             )
-        if plot_orig:
-            ax.axhline(y=0, color="gray", alpha=0.5, zorder=1)
-            ax.axvline(x=1, color="gray", alpha=0.5, zorder=1)
+
+        if plot_init:
+            init_param = {k: p.init_value for k, p in self.result.params.items()}
+            plot(ax, freq, model.eval(x=freq, **init_param), "--")
+
         return ax
 
     def plot_s21(
         self,
         axs: tuple[plt.Axes, plt.Axes] = None,
         freq: np.ndarray = None,
+        plot_fit: bool = True,
         plot_init: bool = False,
     ):
         if axs is None:
             _, (ax, ax2) = plt.subplots(figsize=(6, 2), ncols=2)
-            ax.set_xlabel("freq")
-            ax.set_ylabel("s21_dB")
-            ax2.set_xlabel("freq")
-            ax2.set_ylabel("s21_rad")
+            setup_ax_abs(ax)
+            setup_ax_rad(ax2)
         else:
             ax, ax2 = axs
-        ax2.set_ylim(-3.2, 3.2)
-        ax2.yaxis.set_major_locator(plt.MultipleLocator(np.pi / 2))
-        ax2.yaxis.set_major_formatter(plotter.misc.multiple_formatter(2, np.pi))
 
         if freq is None:
             freq = self.df.freq.values
 
         f0 = self["f0"]
         Qi = self["Qi"]
         Qc = self["Qc"]
@@ -236,45 +217,224 @@
             ax.plot(x[mask2b], y[mask2b], sty, color="C1")
             ax.plot(x[mask3a], y[mask3a], sty, color="C2")
             ax.plot(x[mask3b], y[mask3b], sty, color="C2")
 
         plot(ax, self.df.freq.values, self.df.s21_dB.values, ".")
         plot(ax2, self.df.freq.values, self.df.s21_rad.values, ".")
 
-        if self.result is not None:
+        if (self.result is not None) and plot_fit:
             s21_cplx = 1 / self.result.eval(x=freq)
             ax.plot(freq, 20 * np.log10(np.abs(s21_cplx)), "k-")
             ax2.plot(freq, np.angle(s21_cplx), "k-")
 
         if plot_init:
             init_param = {k: p.init_value for k, p in self.result.params.items()}
             s21_cplx = 1 / model.eval(x=freq, **init_param)
             ax.plot(freq, 20 * np.log10(np.abs(s21_cplx)), "--", color="gray")
             ax2.plot(freq, np.angle(s21_cplx), "--", color="gray")
 
         return ax, ax2
 
-    def plot(self, title: str = None, axs: tuple[plt.Axes, plt.Axes, plt.Axes] = None):
+    def plot(
+        self,
+        axs: tuple[plt.Axes, plt.Axes, plt.Axes] = None,
+        freq: np.ndarray = None,
+        plot_fit: bool = True,
+        plot_init: bool = False,
+    ):
         if axs is None:
             _, (ax, ax2, ax3) = plt.subplots(
                 figsize=(8, 3), ncols=3, layout="constrained"
             )
-            ax.set_xlabel("freq")
-            ax.set_title("s21_dB")
-            ax2.set_xlabel("freq")
-            ax2.set_title("s21_rad")
-            ax3.set_xlabel("Re[$S_{21}^{-1}$]")
-            ax3.set_ylabel("Im[$S_{21}^{-1}$]")
-        self.plot_cplx(ax=ax3)
-        self.plot_s21(axs=(ax, ax2))
-        ax3.set_title(title)
-        return axs
+            setup_ax_abs(ax)
+            setup_ax_rad(ax2)
+            setup_ax_cplx(ax3)
+        else:
+            ax, ax2, ax3 = axs
 
+        self.plot_cplx(ax=ax3, freq=freq, plot_fit=plot_fit, plot_init=plot_init)
+        self.plot_s21(axs=(ax, ax2), freq=freq, plot_fit=plot_fit, plot_init=plot_init)
+        return ax, ax2, ax3
+
+
+def setup_ax_abs(ax: plt.Axes):
+    ax.set_xlabel("freq")
+    ax.set_title("s21_dB")
+
+
+def setup_ax_rad(ax: plt.Axes):
+    ax.set_xlabel("freq")
+    ax.set_title("s21_rad")
+    ax.set_ylim(-3.2, 3.2)
+    ax.yaxis.set_major_locator(plt.MultipleLocator(np.pi / 2))
+    ax.yaxis.set_major_formatter(plotter.misc.multiple_formatter(2, np.pi))
+
+
+def setup_ax_cplx(ax: plt.Axes):
+    ax.set_xlabel("Re[$S_{21}^{-1}$]")
+    ax.set_ylabel("Im[$S_{21}^{-1}$]")
+    ax.set_aspect("equal")
+    ax.axhline(y=0, color="gray", alpha=0.5, zorder=1)
+    ax.axvline(x=1, color="gray", alpha=0.5, zorder=1)
+
+
+def remove_background(
+    y: np.ndarray,
+    x: np.ndarray = None,
+    fit_mask: int | slice | np.ndarray = None,
+    offset: float = None,
+    plot: bool = False,
+):
+    """Remove linear background from data.
+
+    Args:
+        fit_mask: mask of data to use for background estimation.
+            if int, use the first and last fit_mask points.
+        offset: offset after background removal.
+            if None, use y[0].
+
+    Examples:
+    >>> np.round(remove_background([0,3,1], fit_mask=1), decimals=2)
+    array([0. , 2.5, 0. ])
+    """
+    if x is None:
+        x = np.arange(len(y))
+    y = np.asarray(y)
+    x = np.asarray(x)
+
+    if fit_mask is None:
+        x_to_fit, y_to_fit = x, y
+    elif isinstance(fit_mask, int):
+        x_to_fit = np.r_[x[:fit_mask], x[-fit_mask:]]
+        y_to_fit = np.r_[y[:fit_mask], y[-fit_mask:]]
+    else:
+        x_to_fit, y_to_fit = x[fit_mask], y[fit_mask]
+
+    if offset is None:
+        offset = y[0]
+
+    bg_params = np.polyfit(x_to_fit, y_to_fit, 1)  # Linear fit.
+    y_fit = np.polyval(bg_params, x)
+    new_y = y - y_fit + offset
+    if plot:
+        _, ax = plt.subplots()
+        ax.plot(x, y, ".-", label="raw")
+        ax.plot(x, y_fit, label="bg")
+        ax.plot(x, new_y, label="new")
+        ax.legend()
+        plt.show()
+    return new_y
+
+
+def lorentz(x, center, width, amp, offset):
+    return amp * width / ((x - center) ** 2 + width**2) + offset
+
+
+def lorentz_m1(x, center, width, amp, offset):
+    return 1 - amp * width / ((x - center) ** 2 + width**2) + offset
+
+
+model_lorentz = lmfit.Model(lorentz)
+model_lorentz_m1 = lmfit.Model(lorentz_m1)
+
+
+def guess_Qi(
+    s21m1_cplx: np.ndarray,
+    freq: np.ndarray,
+    fr: float,
+    idip: int = None,
+):
+    s21m1_abs = np.abs(s21m1_cplx)
+    if idip is None:
+        idip = np.argmax(s21m1_abs)
+    if idip == 0:
+        logger.warn("fr <= freq.")
+        idip = 1
+    if idip == np.size(freq):
+        logger.warn("fr >= freq.")
+        idip = -2
+
+    half_maximum = (s21m1_abs[idip] + 1) / 2
+    fwhm = 0.1 * np.abs(  # Emprical value.
+        freq[np.argmin(np.abs(s21m1_abs[:idip] - half_maximum))]
+        - freq[np.argmin(np.abs(s21m1_abs[idip:] - half_maximum))]
+    )
+    Qi = np.abs(fr / fwhm)
+
+    try:
+        res = model_lorentz.fit(
+            s21m1_abs,
+            x=freq,
+            center=fr,
+            width=fwhm / 5,
+            amp=0.1 * (s21m1_abs[idip] - 1),
+            offset=1,
+        )
+        Qi = np.abs(res.params["center"].value / res.params["width"].value)
+    except:
+        logger.warn("Fail to fit Lorentz in guessing Qi.")
+
+    if np.mean(np.real(s21m1_cplx)) < 1:
+        Qi = -Qi
+
+    return Qi
+
+
+def guess_Qc(
+    s21_cplx: np.ndarray,
+    freq: np.ndarray,
+    fr: float,
+    idip: int = None,
+    s21_dB: np.ndarray = None,
+):
+    s21_abs = np.abs(s21_cplx)
+    if idip is None:
+        idip = np.argmin(s21_abs)
+    if idip == 0:
+        logger.warn("fr <= freq.")
+        idip = 1
+    if idip == np.size(freq):
+        logger.warn("fr >= freq.")
+        idip = -2
+
+    if s21_dB is None:
+        s21_dB = 20 * np.log10(s21_abs)
+
+    half_maximum = s21_dB[idip] + 3
+    fwhm = 0.2 * np.abs(  # Emprical value.
+        freq[np.argmin(np.abs(s21_dB[:idip] - half_maximum))]
+        - freq[np.argmin(np.abs(s21_dB[idip:] - half_maximum))]
+    )
+    Qc = np.abs(fr / fwhm)
+
+    try:
+        res = model_lorentz_m1.fit(
+            s21_cplx,
+            x=freq,
+            center=fr,
+            width=fwhm / 2,
+            amp=1 - s21_abs[idip],
+            offset=0,
+        )
+        Qc = np.abs(res.params["center"].value / res.params["width"].value / 2)
+    except:
+        logger.warn("Fail to fit Lorentz in guessing Qc.")
 
-if __name__ == "__main__":
-    from labcodes import TEST_DATA_PATH
+    return Qc
 
-    df = pd.read_feather(TEST_DATA_PATH / "fit_resonator.feather")
-    rfit = FitResonator(df.freq_GHz, df.s21_mag_dB, df.s21_phase_rad)
+
+if __name__ == "__main__":
+    freq = misc.segments(
+        misc.center_span(4, 0.01e-3, n=101),
+        misc.center_span(4, 10e-3, n=101),
+    )
+    freq = np.sort(freq)
+    s21m1_cplx = s21m1(freq)
+    s21_cplx = 1 / s21m1_cplx
+    s21_dB = 20 * np.log10(np.abs(s21_cplx))
+    s21_rad = np.angle(s21_cplx)
+    rfit = FitResonator(freq, s21_dB, s21_rad)
+    # rfit.result = None
     rfit.plot()
+    # rfit.result.plot_residuals()
     rfit.result
     plt.show()
```

### Comparing `labcodes-1.0.0/labcodes/fitter.py` & `labcodes-1.0.1/labcodes/fitter.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/misc.py` & `labcodes-1.0.1/labcodes/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,60 +72,14 @@
         ax.plot(freq, e_phase, label='e_phase')
         ax.plot(freq, new_rad, label='new_rad')
         ax.legend()
         plt.show()
     return new_rad
 
 
-def remove_background(
-    y: np.ndarray,
-    x: np.ndarray = None,
-    fit_mask: int | slice | np.ndarray = None,
-    offset: float = None,
-    plot: bool = False,
-):
-    """Remove linear background from data.
-    
-    Args:
-        fit_mask: mask of data to use for background estimation.
-            if int, use the first and last fit_mask points.
-        offset: offset after background removal.
-            if None, use y[0].
-
-    Examples:
-    >>> np.round(remove_background([0,3,1], fit_mask=1), decimals=2)
-    array([0. , 2.5, 0. ])
-    """
-    if x is None: x = np.arange(len(y))
-    y = np.asarray(y)
-    x = np.asarray(x)
-    
-    if fit_mask is None:
-        x_to_fit, y_to_fit = x, y
-    elif isinstance(fit_mask, int):
-        x_to_fit = np.r_[x[:fit_mask], x[-fit_mask:]]
-        y_to_fit = np.r_[y[:fit_mask], y[-fit_mask:]]
-    else:
-        x_to_fit, y_to_fit = x[fit_mask], y[fit_mask]
-
-    if offset is None: offset = y[0]
-
-    bg_params = np.polyfit(x_to_fit, y_to_fit, 1)  # Linear fit.
-    y_fit = np.polyval(bg_params, x)
-    new_y = y - y_fit + offset
-    if plot:
-        _, ax = plt.subplots()
-        ax.plot(x, y, '.-', label='raw')
-        ax.plot(x, y_fit, label='bg')
-        ax.plot(x, new_y, label='new')
-        ax.legend()
-        plt.show()
-    return new_y
-
-
 def remove_background_2d(df, x_name, y_name, z_name):
     """Remove the background of Z which varies along X and constant along Y.
 
     Assumes rectangle grid sampling.
 
     Example:
         remove_background_2d(lf.df, 'ro_freq_GHz', 'z_pulse_offset', ['iq_amp', 'abs(s21)_dB', 'iq_phase_rad'])
```

### Comparing `labcodes-1.0.0/labcodes/models.py` & `labcodes-1.0.1/labcodes/models.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/state_disc.py` & `labcodes-1.0.1/labcodes/state_disc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/tomo.py` & `labcodes-1.0.1/labcodes/tomo.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/app/mat_editor.py` & `labcodes-1.0.1/labcodes/app/mat_editor.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/calc/__init__.py` & `labcodes-1.0.1/labcodes/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/calc/base.py` & `labcodes-1.0.1/labcodes/calc/base.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/calc/qubits.py` & `labcodes-1.0.1/labcodes/calc/qubits.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/calc/resonator_qc.py` & `labcodes-1.0.1/labcodes/calc/resonator_qc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/fileio/__init__.py` & `labcodes-1.0.1/labcodes/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/fileio/base.py` & `labcodes-1.0.1/labcodes/fileio/base.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/fileio/labber.py` & `labcodes-1.0.1/labcodes/fileio/labber.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/fileio/labrad.py` & `labcodes-1.0.1/labcodes/fileio/labrad.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/fileio/ltspice.py` & `labcodes-1.0.1/labcodes/fileio/ltspice.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/benchmark.py` & `labcodes-1.0.1/labcodes/frog/benchmark.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/iq_scatter.py` & `labcodes-1.0.1/labcodes/frog/iq_scatter.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/labrad_timefunc2freq.py` & `labcodes-1.0.1/labcodes/frog/labrad_timefunc2freq.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/pulse_calc.py` & `labcodes-1.0.1/labcodes/frog/pulse_calc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/routine.py` & `labcodes-1.0.1/labcodes/frog/routine.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/state_list.py` & `labcodes-1.0.1/labcodes/frog/state_list.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/tele.py` & `labcodes-1.0.1/labcodes/frog/tele.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/tele_gate.py` & `labcodes-1.0.1/labcodes/frog/tele_gate.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/tele_state.py` & `labcodes-1.0.1/labcodes/frog/tele_state.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/frog/tele_swep.py` & `labcodes-1.0.1/labcodes/frog/tele_swep.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/plotter/__init__.py` & `labcodes-1.0.1/labcodes/plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/plotter/matrix.py` & `labcodes-1.0.1/labcodes/plotter/matrix.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/plotter/misc.py` & `labcodes-1.0.1/labcodes/plotter/misc.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/labcodes/plotter/plot2d.py` & `labcodes-1.0.1/labcodes/plotter/plot2d.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/tests/rt_qst_qpt.py` & `labcodes-1.0.1/tests/rt_qst_qpt.py`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/tests/data/00003 - power shift.csv` & `labcodes-1.0.1/tests/data/00003 - power shift.csv`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/tests/data/00003 - power shift.ini` & `labcodes-1.0.1/tests/data/00003 - power shift.ini`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/tests/data/fit_resonator.feather` & `labcodes-1.0.1/tests/data/fit_resonator.feather`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/.gitignore` & `labcodes-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/LICENSE` & `labcodes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/pyproject.toml` & `labcodes-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labcodes-1.0.0/PKG-INFO` & `labcodes-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labcodes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple routines for superconducting quantum circuits.
 Project-URL: Homepage, https://github.com/Qiujv/LabCodes
 Author-email: Qiujv <qiujv@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -41,20 +41,16 @@
 
 `misc`: Useful functions that not fitting anywhere else.
 
 `frog`: Codes for FROG experiments only.
 
 # Installation
 
-To use LabCodes,
-download this repository,
-go to the directory (make sure `ls` shows `setup.py`)
-and run:
 ```powershell
-pip install --editable .
+pip install labcodes
 ```
 
 # Documentation
 
 All functions, classes comes with necessary documentations in their docstrings. 
 Check them out with command like `help(balabala)`.
 To browser the contents within, try `dir(balabala)` or `help(module_name)`.
```

