# Comparing `tmp/esbmtk-0.8.0.0.tar.gz` & `tmp/esbmtk-0.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esbmtk-0.8.0.0.tar", last modified: Sat Jul 23 17:04:39 2022, max compression
+gzip compressed data, was "esbmtk-0.9.0.1.tar", last modified: Fri Jul 28 08:49:16 2023, max compression
```

## Comparing `esbmtk-0.8.0.0.tar` & `esbmtk-0.9.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 uliw      (1000) users      (100)        0 2022-07-23 17:04:39.531510 esbmtk-0.8.0.0/
--rw-r--r--   0 uliw      (1000) users      (100)     3356 2020-10-29 15:39:35.000000 esbmtk-0.8.0.0/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 uliw      (1000) users      (100)        0 2022-07-23 17:04:39.523510 esbmtk-0.8.0.0/Documentation/
--rw-r--r--   0 uliw      (1000) users      (100)    91167 2020-11-18 20:09:54.000000 esbmtk-0.8.0.0/Documentation/C_Cycle_Ocean.csv
--rw-r--r--   0 uliw      (1000) users      (100)      122 2020-11-05 18:05:55.000000 esbmtk-0.8.0.0/Documentation/test-data.csv
--rw-r--r--   0 uliw      (1000) users      (100)       20 2022-05-11 19:51:45.000000 esbmtk-0.8.0.0/MANIFEST.in
--rw-r--r--   0 uliw      (1000) users      (100)    18639 2022-07-23 17:04:39.531510 esbmtk-0.8.0.0/PKG-INFO
--rw-r--r--   0 uliw      (1000) users      (100)    17938 2022-07-23 17:03:43.000000 esbmtk-0.8.0.0/README.md
-drwxr-xr-x   0 uliw      (1000) users      (100)        0 2022-07-23 17:04:39.527510 esbmtk-0.8.0.0/esbmtk/
--rw-r--r--   0 uliw      (1000) users      (100)     4952 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/Constructor.py
--rw-r--r--   0 uliw      (1000) users      (100)     8327 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/Equation_Terms.py
--rw-r--r--   0 uliw      (1000) users      (100)    80589 2021-03-26 19:18:49.000000 esbmtk-0.8.0.0/esbmtk/Hypsometric_Curve_05m.csv
--rw-r--r--   0 uliw      (1000) users      (100)     2414 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/ODEINT_Solver.py
--rw-r--r--   0 uliw      (1000) users      (100)      890 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/__init__.py
--rw-r--r--   0 uliw      (1000) users      (100)    29600 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/carbonate_chemistry.py
--rw-r--r--   0 uliw      (1000) users      (100)    13078 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/carbonate_chemistry_2.py
--rw-r--r--   0 uliw      (1000) users      (100)    54081 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/connections.py
--rw-r--r--   0 uliw      (1000) users      (100)    79127 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/esbmtk.py
--rw-r--r--   0 uliw      (1000) users      (100)     9920 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/esbmtk_base.py
--rw-r--r--   0 uliw      (1000) users      (100)    78108 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/extended_classes.py
--rw-r--r--   0 uliw      (1000) users      (100)    24989 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/odeuli2.py
--rw-r--r--   0 uliw      (1000) users      (100)    63841 2022-05-11 19:51:45.000000 esbmtk-0.8.0.0/esbmtk/processes-old.py
--rw-r--r--   0 uliw      (1000) users      (100)    56530 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/processes.py
--rw-r--r--   0 uliw      (1000) users      (100)     9590 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/sealevel.py
--rw-r--r--   0 uliw      (1000) users      (100)    16790 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/solver.py
--rw-r--r--   0 uliw      (1000) users      (100)     7550 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/species_definitions.py
--rw-r--r--   0 uliw      (1000) users      (100)    46994 2022-07-23 17:01:22.000000 esbmtk-0.8.0.0/esbmtk/utility_functions.py
-drwxr-xr-x   0 uliw      (1000) users      (100)        0 2022-07-23 17:04:39.527510 esbmtk-0.8.0.0/esbmtk.egg-info/
--rw-r--r--   0 uliw      (1000) users      (100)    18639 2022-07-23 17:04:39.000000 esbmtk-0.8.0.0/esbmtk.egg-info/PKG-INFO
--rw-r--r--   0 uliw      (1000) users      (100)      880 2022-07-23 17:04:39.000000 esbmtk-0.8.0.0/esbmtk.egg-info/SOURCES.txt
--rw-r--r--   0 uliw      (1000) users      (100)        1 2022-07-23 17:04:39.000000 esbmtk-0.8.0.0/esbmtk.egg-info/dependency_links.txt
--rw-r--r--   0 uliw      (1000) users      (100)        7 2022-07-23 17:04:39.000000 esbmtk-0.8.0.0/esbmtk.egg-info/top_level.txt
-drwxr-xr-x   0 uliw      (1000) users      (100)        0 2022-07-23 17:04:39.523510 esbmtk-0.8.0.0/examples/
-drwxr-xr-x   0 uliw      (1000) users      (100)        0 2022-07-23 17:04:39.527510 esbmtk-0.8.0.0/examples/one-box-ocean/
--rw-r--r--   0 uliw      (1000) users      (100)   465865 2021-03-17 14:44:46.000000 esbmtk-0.8.0.0/examples/one-box-ocean/C_Cycle_Ocean.csv
--rw-r--r--   0 uliw      (1000) users      (100)     6418 2020-11-11 18:28:06.000000 esbmtk-0.8.0.0/examples/one-box-ocean/emissions-full.csv
--rw-r--r--   0 uliw      (1000) users      (100)     6418 2020-11-23 21:15:15.000000 esbmtk-0.8.0.0/examples/one-box-ocean/emissions.csv
--rw-r--r--   0 uliw      (1000) users      (100)      273 2020-11-18 19:16:20.000000 esbmtk-0.8.0.0/examples/one-box-ocean/measured_c_isotopes.csv
--rw-r--r--   0 uliw      (1000) users      (100)      106 2022-05-11 19:51:45.000000 esbmtk-0.8.0.0/pyproject.toml
--rw-r--r--   0 uliw      (1000) users      (100)      852 2022-07-23 17:04:39.531510 esbmtk-0.8.0.0/setup.cfg
--rw-r--r--   0 uliw      (1000) users      (100)       69 2022-05-11 19:55:11.000000 esbmtk-0.8.0.0/setup.py
-drwxr-xr-x   0 uliw      (1000) users      (100)        0 2022-07-23 17:04:39.527510 esbmtk-0.8.0.0/tests/
--rw-r--r--   0 uliw      (1000) users      (100)      273 2020-11-18 19:16:20.000000 esbmtk-0.8.0.0/tests/measured_c_isotopes.csv
+drwxr-xr-x   0 uliw      (1000) users      (100)        0 2023-07-28 08:49:16.208758 esbmtk-0.9.0.1/
+-rw-r--r--   0 uliw      (1000) users      (100)     3356 2022-10-01 14:48:03.000000 esbmtk-0.9.0.1/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 uliw      (1000) users      (100)        0 2023-07-28 08:49:16.204758 esbmtk-0.9.0.1/Documentation/
+-rw-r--r--   0 uliw      (1000) users      (100)    91167 2022-10-01 15:14:20.000000 esbmtk-0.9.0.1/Documentation/C_Cycle_Ocean.csv
+-rw-r--r--   0 uliw      (1000) users      (100)      122 2022-10-01 15:14:39.000000 esbmtk-0.9.0.1/Documentation/test-data.csv
+-rw-r--r--   0 uliw      (1000) users      (100)       20 2022-10-01 14:49:02.000000 esbmtk-0.9.0.1/MANIFEST.in
+-rw-r--r--   0 uliw      (1000) users      (100)     5987 2023-07-28 08:49:16.208758 esbmtk-0.9.0.1/PKG-INFO
+-rw-r--r--   0 uliw      (1000) users      (100)     5286 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/README.md
+drwxr-xr-x   0 uliw      (1000) users      (100)        0 2023-07-28 08:49:16.204758 esbmtk-0.9.0.1/esbmtk/
+-rw-r--r--   0 uliw      (1000) users      (100)    80589 2022-10-01 15:15:18.000000 esbmtk-0.9.0.1/esbmtk/Hypsometric_Curve_05m.csv
+-rw-r--r--   0 uliw      (1000) users      (100)      842 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/__init__.py
+-rw-r--r--   0 uliw      (1000) users      (100)    21030 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/carbonate_chemistry.py
+-rw-r--r--   0 uliw      (1000) users      (100)     9471 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/carbonate_chemistry_2.py
+-rw-r--r--   0 uliw      (1000) users      (100)    54612 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/connections.py
+-rw-r--r--   0 uliw      (1000) users      (100)    22337 2023-07-28 08:40:59.000000 esbmtk-0.9.0.1/esbmtk/depreceated_code.py
+-rw-r--r--   0 uliw      (1000) users      (100)    79306 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/esbmtk.py
+-rw-r--r--   0 uliw      (1000) users      (100)     9913 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/esbmtk_base.py
+-rw-r--r--   0 uliw      (1000) users      (100)    80514 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/extended_classes.py
+-rw-r--r--   0 uliw      (1000) users      (100)    32751 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/ode_backend.py
+-rw-r--r--   0 uliw      (1000) users      (100)     6751 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/ode_backend_2.py
+-rw-r--r--   0 uliw      (1000) users      (100)     3224 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/post_processing.py
+-rw-r--r--   0 uliw      (1000) users      (100)    44228 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/processes.py
+-rw-r--r--   0 uliw      (1000) users      (100)     9605 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/sealevel.py
+-rw-r--r--   0 uliw      (1000) users      (100)     6143 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/solver.py
+-rw-r--r--   0 uliw      (1000) users      (100)     7609 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/species_definitions.py
+-rw-r--r--   0 uliw      (1000) users      (100)    46969 2023-07-28 08:24:26.000000 esbmtk-0.9.0.1/esbmtk/utility_functions.py
+drwxr-xr-x   0 uliw      (1000) users      (100)        0 2023-07-28 08:49:16.208758 esbmtk-0.9.0.1/esbmtk.egg-info/
+-rw-r--r--   0 uliw      (1000) users      (100)     5987 2023-07-28 08:49:16.000000 esbmtk-0.9.0.1/esbmtk.egg-info/PKG-INFO
+-rw-r--r--   0 uliw      (1000) users      (100)      887 2023-07-28 08:49:16.000000 esbmtk-0.9.0.1/esbmtk.egg-info/SOURCES.txt
+-rw-r--r--   0 uliw      (1000) users      (100)        1 2023-07-28 08:49:16.000000 esbmtk-0.9.0.1/esbmtk.egg-info/dependency_links.txt
+-rw-r--r--   0 uliw      (1000) users      (100)        7 2023-07-28 08:49:16.000000 esbmtk-0.9.0.1/esbmtk.egg-info/top_level.txt
+drwxr-xr-x   0 uliw      (1000) users      (100)        0 2023-07-28 08:49:16.204758 esbmtk-0.9.0.1/examples/
+drwxr-xr-x   0 uliw      (1000) users      (100)        0 2023-07-28 08:49:16.208758 esbmtk-0.9.0.1/examples/one-box-ocean/
+-rw-r--r--   0 uliw      (1000) users      (100)   465865 2022-10-01 20:08:42.000000 esbmtk-0.9.0.1/examples/one-box-ocean/C_Cycle_Ocean.csv
+-rw-r--r--   0 uliw      (1000) users      (100)     6418 2022-10-01 20:08:42.000000 esbmtk-0.9.0.1/examples/one-box-ocean/emissions-full.csv
+-rw-r--r--   0 uliw      (1000) users      (100)     6418 2022-10-01 20:08:42.000000 esbmtk-0.9.0.1/examples/one-box-ocean/emissions.csv
+-rw-r--r--   0 uliw      (1000) users      (100)      273 2022-10-01 20:08:42.000000 esbmtk-0.9.0.1/examples/one-box-ocean/measured_c_isotopes.csv
+-rw-r--r--   0 uliw      (1000) users      (100)      106 2022-10-01 14:49:02.000000 esbmtk-0.9.0.1/pyproject.toml
+-rw-r--r--   0 uliw      (1000) users      (100)      852 2023-07-28 08:49:16.208758 esbmtk-0.9.0.1/setup.cfg
+-rw-r--r--   0 uliw      (1000) users      (100)       69 2022-10-01 14:49:02.000000 esbmtk-0.9.0.1/setup.py
+drwxr-xr-x   0 uliw      (1000) users      (100)        0 2023-07-28 08:49:16.208758 esbmtk-0.9.0.1/tests/
+-rw-r--r--   0 uliw      (1000) users      (100)      273 2022-10-01 15:15:35.000000 esbmtk-0.9.0.1/tests/measured_c_isotopes.csv
+-rw-r--r--   0 uliw      (1000) users      (100)    37887 2022-10-01 15:16:24.000000 esbmtk-0.9.0.1/tests/test_esbmtk.py
```

### Comparing `esbmtk-0.8.0.0/CODE_OF_CONDUCT.md` & `esbmtk-0.9.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `esbmtk-0.8.0.0/Documentation/C_Cycle_Ocean.csv` & `esbmtk-0.9.0.1/Documentation/C_Cycle_Ocean.csv`

 * *Files identical despite different names*

### Comparing `esbmtk-0.8.0.0/esbmtk/Hypsometric_Curve_05m.csv` & `esbmtk-0.9.0.1/esbmtk/Hypsometric_Curve_05m.csv`

 * *Files identical despite different names*

### Comparing `esbmtk-0.8.0.0/esbmtk/__init__.py` & `esbmtk-0.9.0.1/esbmtk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 from __future__ import annotations
-
+import numpy as np
 from pint import UnitRegistry
-
 ureg = UnitRegistry(on_redefinition="ignore")
 ureg.enable_contexts("chemistry")
 Q_ = ureg.Quantity
-
 ureg.define("Sverdrup = 1e6 * meter **3 / second = Sv = Sverdrups")
 ureg.define("Mol = 1 * mol / liter = M")
 ureg.define("fraction = [] = frac")
 ureg.define("percent = 1e-2 frac = pct")
 ureg.define("permil = 1e-3 fraction")
 ureg.define("ppm = 1e-6 fraction")
-
-import numpy as np
-
-np.seterr(invalid="ignore")
-
-import typing as tp
-
 from .esbmtk_base import *
 from .esbmtk import *
 from .extended_classes import *
 from .connections import *
 from .processes import *
 from .carbonate_chemistry import *
 from .utility_functions import *
 from .sealevel import *
 from .solver import *
-from .Equation_Terms import *
-from .ODEINT_Solver import *
-from .Constructor import *
-from .odeuli2 import *
+from .ode_backend import *
+from .ode_backend_2 import *
 from .carbonate_chemistry_2 import *
+from .post_processing import *
+
+np.seterr(invalid="ignore")
```

### Comparing `esbmtk-0.8.0.0/esbmtk/carbonate_chemistry.py` & `esbmtk-0.9.0.1/esbmtk/carbonate_chemistry.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,18 +12,16 @@
      General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see
      <https://www.gnu.org/licenses/>.
 
 """
-
+from __future__ import annotations
 import typing as tp
-from numba import njit
-from numba.typed import List
 import numpy as np
 from .esbmtk_base import esbmtkBase
 
 if tp.TYPE_CHECKING:
     from .esbmtk import Reservoir, Model
     from .extended_classes import ReservoirGroup
 
@@ -41,19 +39,20 @@
 
     pH = -np.log10(m)
     return pH
 
 
 class SeawaterConstants(esbmtkBase):
     """Provide basic seawater properties as a function of T, P and Salinity.
+    This module does not reca
 
     Example:
 
     Seawater(name="SW",
-             model=,
+             register=M # model handle
              temperature = optional in C, defaults to 25,
              salinity  = optional in psu, defaults to 35,
              pressure = optional, defaults to 0 bars = 1atm,
              pH = optional, defaults to 8.1,
             )
 
     Results are always in mol/kg
@@ -72,20 +71,18 @@
 
     After initialization this class provides access to each value the following way
 
     instance_name.variable_name
 
     """
 
-    
-    
     def __init__(self, **kwargs: dict[str, str]):
 
         from esbmtk import Model, Reservoir, ReservoirGroup
-        
+
         self.defaults: dict[list[any, tuple]] = {
             "name": ["None", (str)],
             "salinity": [35.0, (int, float)],
             "temperature": [25.0, (int, float)],
             "pH": [8.1, (int, float)],
             "pressure": [0, (int, float)],
             "register": ["None", (Model, Reservoir, ReservoirGroup)],
@@ -102,14 +99,15 @@
         self.hplus = 10**-self.pH
         self.constants: list = ["K0", "K1", "K2", "KW", "KB", "Ksp", "Ksp0", "KS", "KF"]
         self.species: list = [
             "dic",
             "ta",
             "ca",
             "co2",
+            "co2aq",
             "hco3",
             "co3",
             "boron",
             "boh4",
             "boh3",
             "oh",
             "ca2",
@@ -141,30 +139,32 @@
         self.__init_c_fractionation_factors__()
 
         # get total alkalinity
         self.ca = self.hco3 + 2 * self.co3
         self.ta = self.ca + self.boh4 + self.oh - self.hplus
 
     def show(self) -> None:
-        """Printout pK values."""
+        """Printout constants"""
 
         from math import log10
 
         for n in self.species:
             v = getattr(self, n)
             print(f"{n} = {v * 1E6:.2f} nmol/kg")
 
-        print(f"pH = {-log10(self.hplus):.2f}\n")
+        print()
+        print(f"pCO2 = {get_pco2(self):.2e}")
+        print(f"pH = {-log10(self.hplus):.2f}")
         print(f"salinity = {self.salinity:.2f}")
         print(f"temperature = {self.temperature:.2f}\n")
 
         for n in self.constants:
-            K = getattr(self, n)
-            pk = getattr(self, f"p{n.lower()}")
-            print(f"{n} = {K:.2e}, p{n} = {pk:.2f}")
+            K = getattr(self, n)  # get K value
+            pk = f"p{n.lower()}"  # get K name
+            print(f"{n} = {K:.2e}, {pk} = {-log10(K):.2f}")
 
     def __get_density__(self):
         """Calculate seawater density as function of temperature,
         pressure and salinity in kg/m^3. Shamelessy copied
         from R. Zeebes equic.m mathlab file.
 
         TC = temp in C
@@ -337,21 +337,29 @@
         self.K0: float = exp(lnK0)
         self.K1: float = exp(lnk1)
         self.K2: float = exp(lnk2)
 
         self.K1 = self.__pressure_correction__("K1", self.K1)
         self.K2 = self.__pressure_correction__("K2", self.K2)
 
+        self.K1K1: float = self.K1 * self.K1
+        self.K1K2: float = self.K1 * self.K2
+
+        # self.K_l : list = [self.K0, self.K1, self.K2, self.K1K1, self.K1K2]
+
         self.co2 = self.dic / (
             1 + self.K1 / self.hplus + self.K1 * self.K2 / self.hplus**2
         )
         self.hco3 = self.dic / (1 + self.hplus / self.K1 + self.K2 / self.hplus)
         self.co3 = self.dic / (
             1 + self.hplus / self.K2 + self.hplus**2 / (self.K1 * self.K2)
         )
+        self.co2aq = self.dic / (
+            1 + (self.K1 / self.hplus) + (self.K1 * self.K2 / (self.hplus**2))
+        )
 
     def __init_boron__(self) -> None:
         """Calculate the boron equilibrium values as function of
         temperature T and salinity S
 
         """
 
@@ -563,15 +571,15 @@
 
         # CO2g versus HCO3, e = epsilon, a = alpha
         self.e_gb: float = -9483 / T + 23.89
         self.a_gb: float = 1 + self.e_gb / 1000
 
         # CO2aq versus CO2g
         self.e_dg: float = -373 / T + 0.19
-        self. a_dg: float = 1 + self.e_dg / 1000
+        self.a_dg: float = 1 + self.e_dg / 1000
 
         # CO2aq versus HCO3
         self.e_db: float = -9866 / T + 24.12
         self.a_db: float = 1 + self.e_db / 1000
 
         # CO32- versus HCO3
         self.e_cb: float = -867 / T + 2.52
@@ -590,14 +598,26 @@
     dic: tp.Union[Reservoir, esbmtk.extended_classes.VirtualReservoir],
     hplus: tp.Union[Reservoir, esbmtk.extended_classes.VirtualReservoir],
     SW: SeawaterConstants,
 
 """
 
 
+def get_pco2(SW) -> float:
+    """Calculate the concentration of pCO2"""
+
+    dic_c: float = SW.dic
+    hplus_c: float = SW.hplus
+    k1: float = SW.K1
+    k2: float = SW.K2
+    co2: np.ndarray = dic_c / (1 + (k1 / hplus_c) + (k1 * k2 / (hplus_c**2)))
+    pco2: np.ndarray = co2 / SW.K0 * 1e6
+    return pco2
+
+
 def calc_pCO2(
     dic,  # see above why no type hints
     hplus,
     SW,
 ) -> np.ndarray:
 
     """
@@ -667,272 +687,7 @@
     k2: float = SW.K2
 
     co2: np.ndarray = dic_c / (1 + (k1 / hplus_c) + (k1 * k2 / (hplus_c**2)))
 
     pco2: np.ndarray = co2 / SW.K0 * 1e6
 
     return pco2
-
-
-@njit(parallel=False, fastmath=True, error_model="numpy")
-def calc_carbonates_1(i: int, input_data: List, vr_data: List, params: List) -> None:
-    """Calculates and returns the carbonate concentrations and saturation state
-     at the ith time-step of the model.
-
-    The function assumes that vr_data will be in the following order:
-        [H+, CA, HCO3, CO3, CO2(aq), omega]
-
-    LIMITATIONS:
-    - This in used in conjunction with ExternalCode objects!
-    - Assumes all concentrations are in mol/kg
-    - Assumes your Model is in mol/kg ! Otherwise, DIC and TA updating will not
-    be correct.
-
-    Calculations are based off equations from:
-    Boudreau et al., 2010, https://doi.org/10.1029/2009GB003654
-    Follows, 2006, doi:10.1016/j.ocemod.2005.05.004
-
-    See add_carbonate_system_1 in utility_functions.py on how to call this function
-
-    Author: M. Niazi & T. Tsan, 2021
-    """
-
-    k1 = params[0]  # K1
-    k2 = params[1]  # K2
-    KW = params[2]  # KW
-    KB = params[3]  # KB
-    boron = params[4]  # boron
-    ca2 = params[5]  # Ca2+
-    ksp = params[6]  # Ksp
-
-    dic: float = input_data[0][i - 1]
-    ta: float = input_data[1][i - 1]
-    hplus: float = vr_data[0][i - 1]
-
-    # calculates carbonate alkalinity (ca) based on H+ concentration from the
-    # previous time-step
-    oh: float = KW / hplus
-    boh4: float = boron * KB / (hplus + KB)
-    fg: float = hplus - oh - boh4
-    ca: float = ta + fg
-
-    # hplus
-    gamm: float = dic / ca
-    dummy: float = (1 - gamm) * (1 - gamm) * k1 * k1 - 4 * k1 * k2 * (1 - (2 * gamm))
-
-    hplus: float = 0.5 * ((gamm - 1) * k1 + (dummy**0.5))
-    # hco3 and co3
-    """ Since CA = [hco3] + 2[co3], can the below expression can be simplified
-    """
-    # co3: float = dic / (1 + (hplus / k2) + ((hplus ** 2) / (k1 * k2)))
-    hco3: float = dic / (1 + (hplus / k1) + (k2 / hplus))
-    co3: float = (ca - hco3) / 2
-    # co2 (aq)
-    """DIC = hco3 + co3 + co2 + H2CO3 The last term is however rather
-    small, so it may be ok to simply write co2aq = dic - hco3 + co3.
-    Let's test this once we have a case where pco2 is calculated from co2aq
-    """
-    #  co2aq: float = dic / (1 + (k1 / hplus) + (k1 * k2 / (hplus ** 2)))
-    co2aq: float = dic - hco3 - co3
-    # omega: float = ca2 * co3 / ksp
-
-    vr_data[0][i] = hplus
-    vr_data[1][i] = ca
-    vr_data[2][i] = hco3
-    vr_data[3][i] = co3
-    vr_data[4][i] = co2aq
-    # vr_data[5][i] = oh
-    # vr_data[5][i] = boh4
-    # vr_data[5][i] = omega
-
-
-@njit(fastmath=True, error_model="numpy")
-def calc_carbonates_2(i: int, input_data: List, vr_data: List, params: List) -> None:
-    """Calculates and returns the carbonate concentrations and carbonate compensation
-    depth (zcc) at the ith time-step of the model.
-
-    The function assumes that vr_data will be in the following order:
-        [H+, CA, HCO3, CO3, CO2(aq), zsat, zcc, zsnow, Fburial,
-        B, BNS, BDS_under, BDS_resp, BDS, BCC, BPDC, BD,omega]
-
-    LIMITATIONS:
-    - This in used in conjunction with ExternalCode objects!
-    - Assumes all concentrations are in mol/kg
-    - Assumes your Model is in mol/kg ! Otherwise, DIC and TA updating will not
-    be correct.
-
-    Calculations are based off equations from:
-    Boudreau et al., 2010, https://doi.org/10.1029/2009GB003654
-    Follows, 2006, doi:10.1016/j.ocemod.2005.05.004
-
-    See add_carbonate_system_2 in utility_functions.py on how to call this function.
-    The input data is a follows
-
-        reservoir DIC.m,  # 0
-        reservoir DIC.l,  # 1
-        reservoir DIC.c,  # 2
-        reservoir TA.m,  # 3 TA mass
-        reservoir.TA.c,  # 4 TA concentration
-        Export_flux.fa,  # 5
-        area_table,  # 6
-        area_dz_table,  # 7
-        Csat_table,  # 8
-        reservoir.DIC.v,  # 9 reservoir volume
-
-    Author: M. Niazi & T. Tsan, 2021
-    """
-
-    # Parameters
-    k1 = params[0]
-    k2 = params[1]
-    KW = params[2]
-    KB = params[3]
-    boron = params[4]
-    ksp0 = params[5]
-    kc = params[6]
-    AD = params[8]
-    zsat0 = int(abs(params[9]))
-    ca2 = params[10]
-    dt = params[11]
-    I_caco3 = params[12]
-    alpha = params[13]
-    zsat_min = int(abs(params[14]))
-    zmax = int(abs(params[15]))
-    z0 = int(abs(params[16]))
-
-    # Data
-    dic: float = input_data[2][i - 1]  # DIC concentration [mol/kg]
-    ta: float = input_data[4][i - 1]  # TA concentration [mol/kg]
-    Bm: float = input_data[5][0]  # Carbonate Export Flux [mol/yr]
-    B12: float = input_data[5][1]  # Carbonate Export Flux light isotope
-    v: float = input_data[9][i - 1]  # volume
-    # lookup tables
-    depth_area_table: np.ndarray = input_data[6]  # depth look-up table
-    area_dz_table: np.ndarray = input_data[7]  # area_dz table
-    Csat_table: np.ndarray = input_data[8]  # Csat table
-
-    # vr_data
-    hplus: float = vr_data[0][i - 1]  # H+ concentration [mol/kg]
-    zsnow = vr_data[7][i - 1]  # previous zsnow
-    
-    # calc carbonate alkalinity based t-1
-    oh: float = KW / hplus
-    boh4: float = boron * KB / (hplus + KB)
-    fg: float = hplus - oh - boh4
-    ca: float = ta + fg
-
-    # calculate carbon speciation
-    # The following equations are after Follows et al. 2006
-    gamm: float = dic / ca
-    dummy: float = (1 - gamm) * (1 - gamm) * k1 * k1 - 4 * k1 * k2 * (1 - (2 * gamm))
-
-    hplus: float = 0.5 * ((gamm - 1) * k1 + (dummy**0.5))
-    # co3: float = dic / (1 + (hplus / k2) + ((hplus ** 2) / (k1 * k2)))
-    hco3: float = dic / (1 + (hplus / k1) + (k2 / hplus))
-    co3: float = (ca - hco3) / 2
-    # DIC = hco3 + co3 + co2 + H2CO3 The last term is however rather
-    # small, so it may be ok to simply write co2aq = dic - hco3 + co3.
-    co2aq: float = dic - co3 - hco3
-    # co2aq: float = dic / (1 + (k1 / hplus) + (k1 * k2 / (hplus ** 2)))
-    # omega: float = (ca2 * co3) / ksp
-
-    # ---------- compute critical depth intervals eq after  Boudreau (2010)
-    # all depths will be positive to facilitate the use of lookup_tables
-
-    # prevent co3 from becoming zero
-    if co3 <= 0:
-        co3 = 1e-16
-
-    zsat = int(max((zsat0 * np.log(ca2 * co3 / ksp0)), zsat_min))  # eq2
-    if zsat < zsat_min:
-        zsat = int(zsat_min)
-
-    zcc = int(zsat0 * np.log(Bm * ca2 / (ksp0 * AD * kc) + ca2 * co3 / ksp0))  # eq3
-
-    # ---- Get fractional areas
-    B_AD = Bm / AD
-
-    if zcc > zmax:
-        zcc = int(zmax)
-    if zcc < zsat_min:
-        zcc = zsat_min
-
-    A_z0_zsat = depth_area_table[z0] - depth_area_table[zsat]
-    A_zsat_zcc = depth_area_table[zsat] - depth_area_table[zcc]
-    A_zcc_zmax = depth_area_table[zcc] - depth_area_table[zmax]
-
-    # ------------------------Calculate Burial Fluxes------------------------------------
-    # BCC = (A(zcc, zmax) / AD) * B, eq 7
-    BCC = A_zcc_zmax * B_AD
-
-    # BNS = alpha_RD * ((A(z0, zsat) * B) / AD) eq 8
-    BNS = alpha * A_z0_zsat * B_AD
-
-    # BDS_under = kc int(zcc,zsat) area' Csat(z,t) - [CO3](t) dz, eq 9a
-    diff_co3 = Csat_table[zsat:zcc] - co3
-    area_p = area_dz_table[zsat:zcc]
-
-    BDS_under = kc * area_p.dot(diff_co3)
-    BDS_resp = alpha * (A_zsat_zcc * B_AD - BDS_under)
-    BDS = BDS_under + BDS_resp
-
-    # BPDC =  kc int(zsnow,zcc) area' Csat(z,t) - [CO3](t) dz, eq 10
-    if zcc < zsnow:  # zcc cannot
-        if zsnow > zmax:  # zsnow cannot exceed ocean depth
-            zsnow = zmax
-
-        diff = Csat_table[zcc : int(zsnow)] - co3
-        area_p = area_dz_table[zcc : int(zsnow)]
-      
-        BPDC = kc * area_p.dot(diff)
-        zold = BPDC / (area_dz_table[int(zsnow)] * I_caco3) * dt
-        # eq 4 dzsnow/dt = Bpdc(t) / (a'(zsnow(t)) * ICaCO3
-        zsnow = zsnow - BPDC / (area_dz_table[int(zsnow)] * I_caco3) * dt
-
-    else:  # zcc > zsnow
-        # there is no carbonate below zsnow, so BPDC = 0
-        zsnow = zcc
-        BPDC = 0
-
-    # BD & F_burial
-    BD: float = BDS + BCC + BNS + BPDC
-    Fburial = Bm - BD
-    Fburial12 = Fburial * input_data[1][i - 1] / input_data[0][i - 1]
-    diss = (Bm - Fburial) * dt  # dissolution flux
-    diss12 = (B12 - Fburial12) * dt  # dissolution flux light isotope
-
-    # # print("{Fburial}.format(")
-    # print(Bm)
-    # print(Fburial)
-    # print(diss)
-    # print()
-    # # print('df ={:.2e}\n'.format(diss/dt))
-
-    """ Now that the fluxes are known we need to update the reservoirs.
-    The concentration in the in the DIC (and TA) of this box are
-    DIC.m[i] + Export Flux - Burial Flux, where the isotope ratio
-    the Export flux is determined by the overlying box, and the isotope ratio
-    of the burial flux is determined by the isotope ratio of this box
-    """
-
-    # Update DIC in the deep box
-    input_data[0][i] = input_data[0][i] + diss  # DIC
-    input_data[1][i] = input_data[1][i] + diss12  # 12C
-    input_data[2][i] = input_data[0][i] / v  # DIC concentration
-
-    # Update TA in deep box
-    input_data[3][i] = input_data[3][i] + 2 * diss  # TA
-    input_data[4][i] = input_data[3][i] / v  # TA concentration
-
-    # copy results into datafields
-    vr_data[0][i] = hplus  # 0
-    vr_data[1][i] = ca  # 1
-    vr_data[2][i] = hco3  # 2
-    vr_data[3][i] = co3  # 3
-    vr_data[4][i] = co2aq  # 4
-    vr_data[5][i] = zsat  # 5
-    vr_data[6][i] = zcc  # 6
-    vr_data[7][i] = zsnow  # 7
-    vr_data[8][i] = Fburial  # 8
-    vr_data[9][i] = Fburial12  # 9
-    vr_data[10][i] = diss / dt  # 9
-    vr_data[11][i] = Bm  # 9
```

### Comparing `esbmtk-0.8.0.0/esbmtk/carbonate_chemistry_2.py` & `esbmtk-0.9.0.1/esbmtk/carbonate_chemistry_2.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,21 +12,22 @@
      General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see
      <https://www.gnu.org/licenses/>.
 
 """
-
+from __future__ import annotations
 import typing as tp
 import numpy as np
-from esbmtk import ReservoirGroup, Flux
+from math import log, sqrt
+from esbmtk import ReservoirGroup
 
-if tp.TYPE_CHECKING:
-    from .esbmtk import ReservoirGroup, Flux
+# if tp.TYPE_CHECKING:
+#     from .esbmtk import ReservoirGroup, Flux
 
 
 def get_hplus(
     rg: ReservoirGroup,
     dic: float,
     ta: float,
     hplus: float,
@@ -45,26 +46,24 @@
     boh4: float = boron * KB / (hplus + KB)
     fg: float = hplus - oh - boh4
     ca: float = ta + fg
 
     # hplus
     gamm: float = dic / ca
     dummy: float = (1 - gamm) * (1 - gamm) * k1 * k1 - 4 * k1 * k2 * (1 - (2 * gamm))
-    hplus: float = 0.5 * ((gamm - 1) * k1 + (dummy**0.5))
+    hplus: float = 0.5 * ((gamm - 1) * k1 + sqrt(dummy))
 
     return hplus - hplus_0
 
 
 def carbonate_system_1_ode(
-    rg: ReservoirGroup,
+    swc: any,
     dic: float,
     ta: float,
     hplus: float,
-    i: float,
-    max_i: float,
 ) -> float:
 
     """Calculates and returns the H+ and carbonate alkalinity concentrations
      for the given reservoirgroup
 
     LIMITATIONS:
     - Assumes all concentrations are in mol/kg
@@ -73,326 +72,196 @@
 
     Calculations are based off equations from:
     Boudreau et al., 2010, https://doi.org/10.1029/2009GB003654
     Follows, 2006, doi:10.1016/j.ocemod.2005.05.004
 
     """
 
-    k1 = rg.swc.K1  # K1
-    k2 = rg.swc.K2  # K2
-    KW = rg.swc.KW  # KW
-    KB = rg.swc.KB  # KB
-    boron = rg.swc.boron  # boron
+    k1 = swc.K1  # K1
+    k1k1 = swc.K1K1  #  K1 * K1
+    k1k2 = swc.K1K2  # K1 * K2
+    KW = swc.KW  # KW
+    KB = swc.KB  # KB
+    boron = swc.boron  # boron
     hplus_0 = hplus
 
     # calculates carbonate alkalinity (ca) based on H+ concentration from the
     # previous time-step
     oh: float = KW / hplus
     boh4: float = boron * KB / (hplus + KB)
     fg: float = hplus - oh - boh4
     ca: float = ta + fg
 
     # hplus
     gamm: float = dic / ca
-    dummy: float = (1 - gamm) * (1 - gamm) * k1 * k1 - 4 * k1 * k2 * (1 - (2 * gamm))
-    hplus: float = 0.5 * ((gamm - 1) * k1 + (dummy**0.5))
-
-    hco3: float = dic / (1 + (hplus / k1) + (k2 / hplus))
-    co3: float = (ca - hco3) / 2
-    # co2 (aq)
-    """DIC = hco3 + co3 + co2 + H2CO3 The last term is however rather
-    small, so it may be ok to simply write co2aq = dic - hco3 + co3.
-    Let's test this once we have a case where pco2 is calculated from co2aq
-    """
-    #  co2aq: float = dic / (1 + (k1 / hplus) + (k1 * k2 / (hplus ** 2)))
-    co2aq: float = dic - hco3 - co3
-
-    # diff = hplus - rg.cs.H.extend
-    # save in state for co2aq, hco3, co3
-    if i >= max_i:
-        rg.cs.H = np.append(rg.cs.H, hplus)
-        rg.cs.CA = np.append(rg.cs.CA, ca)
-        rg.cs.HCO3 = np.append(rg.cs.HCO3, hco3)
-        rg.cs.CO3 = np.append(rg.cs.CO3, co3)
-        rg.cs.CO2aq = np.append(rg.cs.CO2aq, co2aq)
-    else:
-        rg.cs.H[i] = hplus  # 1
-        rg.cs.CA[i] = ca  # 1
-        rg.cs.HCO3[i] = hco3  # 2
-        rg.cs.CO3[i] = co3  # 3
-        rg.cs.CO2aq[i] = co2aq  # 4
-
+    dummy: float = (1 - gamm) * (1 - gamm) * k1k1 - k1k2 * (4 - 8 * gamm)
+    hplus: float = 0.5 * ((gamm - 1) * k1 + sqrt(dummy))
+    co2aq: float = dic / (1 + (k1 / hplus) + (k1k2 / (hplus * hplus)))
     diff = hplus - hplus_0
 
     return diff, co2aq
 
 
+# @njit(parallel=False, fastmath=True, error_model="numpy")
 def carbonate_system_2_ode(
-    t,  # time step
-    rg: ReservoirGroup,  # Reservoir handle
-    Bm: float,  # CaCO3 export flux as DIC
-    dic_db: float,  # DIC in the deep box
-    ta_db: float,  # TA in the deep box
-    dic_sb: float,  # [DIC] in the surface box
-    dic_sb_l: float,  # [DIC_l] in the surface box
-    hplus: float,  # hplus in the deep box at t-1
-    zsnow: float,  # snowline in meters below sealevel at t-1
-    i: float,  # current index
-    max_i: float,  # max length of vr vectors
-    last_t: float,  # time of the last calls to cs2
+    rg: ReservoirGroup,  # 2 Reservoir handle
+    Bm: float,  # 3 CaCO3 export flux as DIC
+    dic_db: float,  # 4 DIC in the deep box
+    ta_db: float,  # 5 TA in the deep box
+    dic_sb: float,  # 6 [DIC] in the surface box
+    dic_sb_l: float,  # 7 [DIC_l] in the surface box
+    hplus_0: float,  # 8 hplus in the deep box at t-1
+    zsnow: float,  # 9 snowline in meters below sealevel at t-1
 ) -> tuple:
     """Calculates and returns the fraction of the carbonate rain that is
     dissolved an returned back into the ocean. This functions returns:
 
     DIC_burial, DIC_burial_l, Hplus, zsnow
 
-    Additionally, it calculates  the following critical depth intervals:
-
-    zsat: top of lysocline
-    zcc: carbonate compensation depth
-
     LIMITATIONS:
     - Assumes all concentrations are in mol/kg
     - Assumes your Model is in mol/kg ! Otherwise, DIC and TA updating will not
     be correct.
 
     Calculations are based off equations from:
     Boudreau et al., 2010, https://doi.org/10.1029/2009GB003654
     Follows, 2006, doi:10.1016/j.ocemod.2005.05.004
-
-    Author: M. Niazi & T. Tsan, 2021
     """
 
-    hplus_0 = hplus  # hplus from last timestep
-
     # Parameters
     k1 = rg.swc.K1  # K1
+    k1k1 = rg.swc.K1K1
     k2 = rg.swc.K2  # K2
+    k1k2 = rg.swc.K1K2  # K2
     KW = rg.swc.KW  # KW
     KB = rg.swc.KB  # KB
     boron = rg.swc.boron  # boron
-
     p = rg.cs.function_params
-
     ksp0 = p[5]
     ca2 = rg.swc.ca2  # Ca2+
     kc = p[6]
     AD = p[8]
     zsat0 = int(abs(p[9]))
     I_caco3 = p[12]
     alpha = p[13]
     zsat_min = int(abs(p[14]))
     zmax = int(abs(p[15]))
     z0 = int(abs(p[16]))
-    # zsnow = int(abs(p[19]))  # previous zsnow
     depth_area_table = rg.cs.depth_area_table
     area_dz_table = rg.cs.area_dz_table
     Csat_table = rg.cs.Csat_table
 
     # calc carbonate alkalinity based t-1
-    oh: float = KW / hplus
-    boh4: float = boron * KB / (hplus + KB)
-    fg: float = hplus - oh - boh4
+    oh: float = KW / hplus_0
+    boh4: float = boron * KB / (hplus_0 + KB)
+    fg: float = hplus_0 - oh - boh4
     ca: float = ta_db + fg
 
     # calculate carbon speciation
     # The following equations are after Follows et al. 2006
     gamm: float = dic_db / ca
-    dummy: float = (1 - gamm) * (1 - gamm) * k1 * k1 - 4 * k1 * k2 * (1 - (2 * gamm))
-
-    hplus: float = 0.5 * ((gamm - 1) * k1 + (dummy**0.5))
-    # co3: float = dic / (1 + (hplus / k2) + ((hplus ** 2) / (k1 * k2)))
-    hco3: float = dic_db / (1 + (hplus / k1) + (k2 / hplus))
-    co3: float = (ca - hco3) / 2
-    # DIC = hco3 + co3 + co2 + H2CO3 The last term is however rather
-    # small, so it may be ok to simply write co2aq = dic - hco3 + co3.
-    co2aq: float = dic_db - co3 - hco3
-    # co2aq: float = dic / (1 + (k1 / hplus) + (k1 * k2 / (hplus ** 2)))
-    # omega: float = (ca2 * co3) / ksp
-
+    dummy: float = (1 - gamm) * (1 - gamm) * k1k1 - k1k2 * (4 - 8 * gamm)
+    hplus: float = 0.5 * ((gamm - 1) * k1 + sqrt(dummy))
+    co3 = max(dic_db / (1 + hplus / k2 + hplus * hplus / k1k2), 3.7e-05)
     # ---------- compute critical depth intervals eq after  Boudreau (2010)
     # all depths will be positive to facilitate the use of lookup_tables
-
-    # prevent co3 from becoming zero
-    if co3 <= 0:
-        co3 = 1e-16
-
-    zsat = int(max((zsat0 * np.log(ca2 * co3 / ksp0)), zsat_min))  # eq2
-
-    # print(
-    #     f"i = {i}, zsat0 = {zsat0:.1f}, ca= {ca:.2e}, co3 = {co3:.2e}, ksp0 = {ksp0:.2e}, zsat_min = {zsat_min:.1f}"
-    # )
-    # print(f"zsat = {zsat:.1f}\n")
-    if zsat < zsat_min:
-        zsat = int(zsat_min)
-
-    zcc = int(zsat0 * np.log(Bm * ca2 / (ksp0 * AD * kc) + ca2 * co3 / ksp0))  # eq3
-
-    # ---- Get fractional areas
+    zsat = int(zsat0 * log(ca2 * co3 / ksp0))
+    zsat = np.clip(zsat, zsat_min, zmax)
+    zcc = int(zsat0 * log(Bm * ca2 / (ksp0 * AD * kc) + ca2 * co3 / ksp0))  # eq3
+    zcc = np.clip(zcc, zsat_min, zmax)
+    # get fractional areas
     B_AD = Bm / AD
-
-    if zcc > zmax:
-        zcc = int(zmax)
-    if zcc < zsat_min:
-        zcc = zsat_min
-
     A_z0_zsat = depth_area_table[z0] - depth_area_table[zsat]
     A_zsat_zcc = depth_area_table[zsat] - depth_area_table[zcc]
     A_zcc_zmax = depth_area_table[zcc] - depth_area_table[zmax]
-
     # ------------------------Calculate Burial Fluxes----------------------------- #
-    # BCC = (A(zcc, zmax) / AD) * B, eq 7
     BCC = A_zcc_zmax * B_AD
-
-    # BNS = alpha_RD * ((A(z0, zsat) * B) / AD) eq 8
     BNS = alpha * A_z0_zsat * B_AD
-
-    # BDS_under = kc int(zcc,zsat) area' Csat(z,t) - [CO3](t) dz, eq 9a
     diff_co3 = Csat_table[zsat:zcc] - co3
     area_p = area_dz_table[zsat:zcc]
-
     BDS_under = kc * area_p.dot(diff_co3)
     BDS_resp = alpha * (A_zsat_zcc * B_AD - BDS_under)
     BDS = BDS_under + BDS_resp
-
-    # BPDC =  kc int(zsnow,zcc) area' Csat(z,t) - [CO3](t) dz, eq 10
-    # if zcc < zsnow:  # zsnow is deeper than zcc, so we need to dissolve
-    #     if zsnow > zmax:  # zsnow cannot exceed ocean depth
-    #         zsnow = zmax
-    # sedimentary CaCO3
-    # if zsnow > zmax:  # zsnow cannot exceed ocean depth
-    #     zsnow = zmax
-    # moved to equations.py
-
-    # get saturation difference per depth interval
     diff: np.ndarray = Csat_table[zcc : int(zsnow)] - co3
-
-    # get table of depth intervals
-    # print(f"zcc = {zcc}, zsnow = {zsnow}")
     area_p: np.ndarray = area_dz_table[zcc : int(zsnow)]
-
     # integrate saturation difference over area
     BPDC = kc * area_p.dot(diff)
-
-    if BPDC < 0:
-        BPDC = 0
-    #     d_zsnow = 0
-    # print(f"BPDC = {BPDC:.2e}")
-    # eq 4 dzsnow/dt = Bpdc(t) / (a'(zsnow(t)) * ICaCO3
-    # print(f"area_dz_table[int(zsnow)] = {area_dz_table[int(zsnow)]:.2e}")
-    # print(f"I_caco3 = {I_caco3}, dt = {(t - last_t):.2e}")
-
+    BPDC = max(BPDC, 0)  # prevent negative values
     d_zsnow = -BPDC / (area_dz_table[int(zsnow)] * I_caco3)
-
-    # elif zcc >= zsnow:  # e.g. 5000 > 4750
-    #     # there is no carbonate below 4750, so BPDC = 0
-    #     d_zsnow = 0
-    #     BPDC = 0
-
     # get isotope ratio in reservoir
-    # BD & F_burial
     BD: float = BDS + BCC + BNS + BPDC
-    Fburial = Bm - BD
-
-    if i > max_i:
-        rg.cs.H = np.append(rg.cs.H, hplus)
-        rg.cs.CA = np.append(rg.cs.CA, ca)
-        rg.cs.HCO3 = np.append(rg.cs.HCO3, hco3)
-        rg.cs.CO3 = np.append(rg.cs.CO3, co3)
-        rg.cs.CO2aq = np.append(rg.cs.CO2aq, co2aq)
-        rg.cs.zsat = np.append(rg.cs.zsat, zsat)
-        rg.cs.zcc = np.append(rg.cs.zcc, zcc)
-        # rg.cs.zsnow = np.append(rg.cs.zsnow, zsnow)
-        rg.cs.Fburial = np.append(rg.cs.Fburial, Fburial)
-    else:
-        rg.cs.H[i] = hplus  #
-        rg.cs.CA[i] = ca  # 1
-        rg.cs.HCO3[i] = hco3  # 2
-        rg.cs.CO3[i] = co3  # 3
-        rg.cs.CO2aq[i] = co2aq  # 4
-        rg.cs.zsat[i] = zsat  # 5
-        rg.cs.zcc[i] = zcc  # 6
-        # rg.cs.zsnow[i] = zsnow  # 7 claculated explicitly by the ode system
-        rg.cs.Fburial[i] = Fburial
-
     """Bm is the flux of CaCO3 into the box. However, the model should
     use the bypass option and leave all flux calculations to the
     cs_code.  As such, we simply add the fraction of the input flux
     that dissolves, and ignore the fraction that is buried.  
 
     The isotope ratio of the dissolutio flux is determined by the delta
     value of the sediments we are dissolving, and the delta of the carbonate rain.
     The currrent code, assumes that both are the same.
     """
-    # SB_r = # isotope ratio of surface box
-    # DB_r = # isotope ratio of deep box
     BD_l = BD * dic_sb_l / dic_sb
-    # Fburial_l = Fburial * DB_r
-
     dH = hplus - hplus_0
+
     return -BD, -BD_l, dH, d_zsnow
 
 
-def gas_exchange_ode(scale, gas_c, p_H2O, solubility, c_aq) -> float:
+def gas_exchange_ode(scale, gas_c, p_H2O, solubility, g_c_aq) -> float:
     """Calculate the gas exchange flux across the air sea interface
 
     Parameters:
-     scale: surface area in m^2
-     gas_c: species concentration in atmosphere
-     p_H2O: water vapor partial pressure
-     solubility: species solubility  mol/(m^3 atm)
-     c_aq: concentration of the dissolved gas in water
+    scale: surface area in m^2
+    gas_c: species concentration in atmosphere
+    p_H2O: water vapor partial pressure
+    solubility: species solubility  mol/(m^3 atm)
+    gc_aq: concentration of the dissolved gas in water
     """
-
-    f = scale * (  # area in m^2
-        gas_c  # Atmosphere
-        * (1 - p_H2O)  # p_H2O
-        * solubility  # SA_co2 = mol/(m^3 atm)
-        - c_aq * 1000  # [CO2]aq mol
-    )
+    beta = solubility * (1 - p_H2O)
+    f = scale * (gas_c * beta - g_c_aq * 1e3)
 
     return -f
 
 
 def gas_exchange_ode_with_isotopes(
-    scale,  # surface area in m^2
+    scale,  # surface area in m^2 * piston velocity
     gas_c,  # species concentration in atmosphere
     gas_c_l,  # same but for the light isotope
     liquid_c,  # c of the reference species (e.g., DIC)
-    liquid_c_l,  # same but for the light isotope
+    liquid_c_l,  # same but for the light isotopeof DIC
     p_H2O,  # water vapor pressure
     solubility,  # solubility constant
-    c_aq,  # Gas concentration in liquid phase
+    gas_c_aq,  # Gas concentration in liquid phase
     a_db,  # fractionation factor between dissolved CO2aq and HCO3-
     a_dg,  # fractionation between CO2aq and CO2g
     a_u,  # kinetic fractionation during gas exchange
-) -> tuple:
+) -> tuple(float, float):
     """Calculate the gas exchange flux across the air sea interface
-    for co2 incliding isotope effects.
+    for co2 including isotope effects.
 
     Note that the sink delta is co2aq as returned by the carbonate VR
     this equation is for mmol but esbmtk uses mol, so we need to
     multiply by 1E3
-    """
 
-    # equilibrium concentration of CO2 in water based on pCO2
-    eco2_at = gas_c * (1 - p_H2O) * solubility  # p Atmosphere  # p_H2O
-    # equilibrium concentration of CO2 in water based on CO2aq
-    eco2_aq = c_aq * 1000
-
-    # total flux
-    f = scale * (eco2_at - eco2_aq)
-
-    # get heavy isotope concentration in the respective reservoirs
-    c13g = gas_c - gas_c_l  #
-    c13aq = liquid_c - liquid_c_l
-    # get 13C CO2 equlibrium concentration  CO2 in water based on pCO2
-    eco2_at_13 = gas_c * c13g * (1 - p_H2O) * solubility * a_dg  # p_H2O
-
-    # get 13C equilibrium  CO2 in water based on DIC m & l
-    eco2_aq_13 = a_db * eco2_aq * c13aq
-
-    # 13C flux
-    f13 = scale * a_u * (eco2_at_13 - eco2_aq_13)
-    f12 = f - f13
+    The Total flux across interface dpends on the difference in either
+    concentration or pressure the atmospheric pressure is known, as gas_c, and
+    we can calculate the equilibrium pressure that corresponds to the dissolved
+    gas in the water as [CO2]aq/beta.
+
+    Conversely, we can convert the the pCO2 into the amount of dissolved CO2 =
+    pCO2 * beta
+
+    The h/c ratio in HCO3 estimated via h/c in DIC. Zeebe writes C12/C13 ratio
+    but that does not work. the C13/C ratio results however in -8 permil
+    offset, which is closer to observations
+    """
+    # Solibility with correction for pH2O
+    beta = solubility * (1 - p_H2O)
+    # f as afunction of solubility difference
+    f = scale * (beta * gas_c - gas_c_aq * 1e3)
+    # isotope ratio of DIC
+    Rt = (liquid_c - liquid_c_l) / liquid_c
+    # get heavy isotope concentrations in atmosphere
+    gas_c_h = gas_c - gas_c_l  # gas heavy isotope concentration
+    # get exchange of the heavy isotope
+    f_h = scale * a_u * (a_dg * gas_c_h * beta - Rt * a_db * gas_c_aq * 1e3)
+    f_l = f - f_h  # the corresponding flux of the light isotope
 
-    return -f, -f12
+    return -f, -f_l
```

### Comparing `esbmtk-0.8.0.0/esbmtk/connections.py` & `esbmtk-0.9.0.1/esbmtk/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from __future__ import annotations
 
 # from numbers import Number
 import typing as tp
 import numpy as np
 import copy as cp
 import logging
+import uuid
 from .esbmtk import esbmtkBase
 from .utility_functions import map_units
 from .utility_functions import check_for_quantity
 
 np.set_printoptions(precision=4)
 
 if tp.TYPE_CHECKING:
@@ -293,15 +294,15 @@
             "source": ["None", (str, Source, Reservoir, GasReservoir)],
             "sink": ["None", (str, Sink, Reservoir, GasReservoir)],
             "delta": ["None", (int, float, str)],
             "rate": ["None", (str, int, float, Q_)],
             "pl": ["None", (list, str)],
             "alpha": ["None", (int, float, str)],
             "species": ["None", (Species, str)],
-            "ctype": ["None", (str)],
+            "ctype": ["regular", (str)],
             "ref_reservoirs": ["None", (Reservoir, GasReservoir, str, list)],
             "reservoir_ref": ["None", (GasReservoir, str)],
             "ref_flux": ["None", (Flux, str, list)],
             "ratio": ["None", (int, float, str)],
             "scale": [1, (int, float, Q_, str)],
             "ref_value": ["None", (str, int, float, Q_)],
             "k_value": ["None", (int, float, str, Q_)],
@@ -321,22 +322,27 @@
             "pco2_0": ["280 ppm", (str, Q_)],
             "piston_velocity": ["None", (str, int, float)],
             "function_ref": ["None", (str, callable)],
             "save_flux_data": ["None", (bool, str)],
         }
 
         # provide a list of absolutely required keywords
-        self.lrk: list = ["source", "sink", "register", "id"]
+        self.lrk: list = ["source", "sink"]
 
-        self.lop: list = list()
-        self.lof: list = list()
+        self.lop: list = []
+        self.lof: list = []
 
         # validate and initialize instance variables
         self.__initialize_keyword_variables__(kwargs)
 
+        if self.register == "None":
+            self.register = self.source.register
+        if self.id == "None":
+            self.id = str(uuid.uuid4())[:8]
+
         # legacy names
         self.influx: int = 1
         self.outflux: int = -1
         self.mo = self.source.sp.mo
         self.model = self.mo
         self.sp = self.source.species
         self.p = 0  # the default process handle
@@ -345,19 +351,15 @@
         self.parent = self.register
 
         if isinstance(self.pco2_0, str):
             self.pco2_0 = Q_(self.pco2_0).to("ppm").magnitude * 1e-6
         elif isinstance(self.pco2_0, Q_):
             self.pco2_0 = self.pco2_0.magnitude.to("ppm").magnitude * 1e-6
 
-        if "pl" in kwargs:
-            self.lop: list[Process] = self.pl
-        else:
-            self.lop: list[Process] = []
-
+        self.lop: list[Process] = self.pl if "pl" in kwargs else []
         if self.signal != "None":
             self.lop.append(self.signal)
 
         # if we have a signal, save flux data
         if self.signal != "None":
             self.save_flux_data = True
         # else if save_flux_data is unsepcified, use model default
@@ -463,35 +465,35 @@
             elif isinstance(self.source.parent, Source):
                 so = self.source.parent.name
             elif isinstance(self.source.parent, SourceGroup):
                 so = self.source.parent.name
             else:
                 so = self.source.name
 
-            if isinstance(self.sink.parent, ReservoirGroup):
-                si = self.sink.parent.name
-            else:
-                si = self.sink.name
-                
+            si = (
+                self.sink.parent.name
+                if isinstance(self.sink.parent, ReservoirGroup)
+                else self.sink.name
+            )
+
             self.name = f"C_{so}_to_{si}_{self.source.sp.name}"
+        elif self.sink.species.name == self.source.species.name:
+            self.name = f"{self.source.species.name}"
         else:
-            # same species?
-            if self.sink.species.name == self.source.species.name:
-                self.name = f"{self.source.species.name}"
-            else:
-                self.name = f"{self.source.species.name}_to_{self.sink.species.name}"
+            self.name = f"{self.source.species.name}_to_{self.sink.species.name}"
 
         # id set?
         if self.id != "None":
             if (self.source.species.name in self.id) or (
                 self.sink.species.name in self.id
             ):
                 self.name = f"{self.id}"
             else:
                 self.name = f"{self.name}_{self.id}"
+                # self.name = f"{self.name}@{self.id}"
 
         # always overide name with id for manual connections
         # if not isinstance(self.parent, ConnectionGroup):
         #     if self.id != "None":
         #         self.name = f"{self.source.name}_{self.id}_{self.sp.name}"
 
     def update(self, **kwargs):
@@ -513,43 +515,27 @@
         backward fluxes the species depends on the r2
 
         """
 
         from esbmtk import Source
 
         # print(f"r1 = {r1.n}, r2 = {r2.n}")
-        if isinstance(self.r1, Source):
-            self.r = r1
-        else:  # in this case we do have an upstream reservoir
-            self.r = r2
-
+        self.r = r1 if isinstance(self.r1, Source) else r2
         # test if species was explicitly given
-        if "species" in self.kwargs:  # this is a quick fix only
-            self.sp = self.kwargs["species"]
-        else:
-            self.sp = self.r.sp  # get the parent species
+        self.sp = self.kwargs["species"] if "species" in self.kwargs else self.r.sp
 
     def __create_flux__(self) -> None:
         """Create flux object, and register with reservoir and global
         namespace"""
 
         from esbmtk import Flux, Source, Sink
 
         # test if default arguments present
-        if self.delta == "None":
-            d = 0
-        else:
-            d = self.delta
-
-        if self.rate == "None":
-            r = f"0 {self.sp.mo.f_unit}"
-            # self._rate = r
-        else:
-            r = self.rate
-
+        d = 0 if self.delta == "None" else self.delta
+        r = f"0 {self.sp.mo.f_unit}" if self.rate == "None" else self.rate
         # derive flux unit from species obbject
         # funit = self.sp.mu + "/" + str(self.sp.mo.bu)  # xxx
 
         self.fh = Flux(
             species=self.sp,  # Species handle
             delta=d,  # delta value of flux
             rate=r,  # flux value
@@ -623,58 +609,57 @@
         p_copy = cp.copy(self.lop)
         for p in p_copy:  # loop over process list if provided during init
             if isinstance(p, Signal):
                 self.lop.remove(p)
                 if p.ty == "addition":
                     # create AddSignal Process object
                     n = AddSignal(
-                        name=p.n + "_addition_process",
+                        name=f"{p.n}_addition_process",
                         reservoir=self.r,
                         flux=self.fh,
                         lt=p.data,
                         register=self.fh,
                         model=self.mo,
                     )
+
                     self.lop.insert(0, n)  # signals must come first
                     logging.debug(f"Inserting {n.n} in {self.name} for {self.r.n}")
                 elif p.ty == "multiplication":
                     # create AddSignal Process object
                     n = MultiplySignal(
-                        name=p.n + "_multiplication_process",
+                        name=f"{p.n}_multiplication_process",
                         reservoir=self.r,
                         flux=self.fh,
                         lt=p.data,
                         register=self.fh,
                         model=self.mo,
                     )
+
                     self.lop.insert(len(self.lop), n)  # multiplaction should come last
                     logging.debug(f"Inserting {n.n} in {self.name} for {self.r.n}")
                 else:
                     raise ValueError(f"Signal type {p.ty} is not defined")
 
         # ensure that processes are in the correct order
         self.__move_process_to_top_of_queue__(self.lop, MultiplySignal)
         self.__move_process_to_top_of_queue__(self.lop, AddSignal)
         self.__move_process_to_top_of_queue__(self.lop, ScaleFlux)
         self.__move_process_to_top_of_queue__(self.lop, VarDeltaOut)
         self.__move_process_to_end_of_queue__(self.lop, SaveFluxData)
 
-        # nwo we can register everythig on lop
-        i = 0
-        for p in self.lop:
+        for i, p in enumerate(self.lop):
             if isinstance(p, (MultiplySignal)) and i > 0:
                 p.__execute__ = p.__multiply_with_flux_fa__
                 p.__get_process_args__ = p.__get_process_args_fa__
             if isinstance(p, (AddSignal)) and i > 0:
-                print(f"Found Add signal")
+                print("Found Add signal")
                 p.__execute__ = p.__add_with_fa__
                 p.__get_process_args__ = p.__get_process_args_fa__
 
             p.__register__(self.r, self.fh)
-            i += 1
 
     def __move_process_to_top_of_queue__(self, lop: list, ptype: any) -> None:
         """Return a copy of lop where ptype has been moved to the top of lop"""
         p_copy = cp.copy(lop)
         for p in p_copy:  # loop over process list if provided during init
             if isinstance(p, ptype):
                 lop.remove(p)
@@ -695,38 +680,34 @@
 
         from esbmtk import (
             SaveFluxData,
             Source,
             Sink,
         )
 
-        if isinstance(self.r1, Source):
-            self.r = self.r2
-        else:
-            self.r = self.r1
-
+        self.r = self.r2 if isinstance(self.r1, Source) else self.r1
         # if signal is provided but rate is omitted
         if self.signal != "None" and self.rate == "None":
-            self._rate = "0 mmol/y"
+            self._rate = 0
 
         # if connection type is not set explicitly
         if self.ctype == "None" or self.ctype.casefold() == "regular":
             # set the fundamental flux type based on the flux arguments given
             if self.delta != "None" and self.rate != "None":
                 # self.__vardeltaout__()
                 pass  # if delta and rate are specified, do nothing
-            # variable flux with fixed delta
             elif self.delta != "None":  # if delta is set
                 self.__passivefluxfixeddelta__()
-            elif self.rate != "None":  # if rate is set
-                if self.delta != "None" and not isinstance(self.source, Sink):
-                    self.__vardeltaout__()  # variable delta with fixed flux
-            else:  # if neither are given -> default varflux type
+            elif self.rate == "None":  # if neither are given -> default varflux type
                 self._delta = 0
                 self.__passiveflux__()
+            # test for case where isotopes are true, but neither
+            # delta notr alpha are given
+            if self.delta == "None" and self.alpha == "None" and self.isotopes:
+                self._alpha = 0
 
         elif self.ctype == "scale_to_input":
             self.__scale_to_input__()
         elif self.ctype == "flux_diff":
             self.__vardeltaout__()
             self.__flux_diff__()
         elif self.ctype == "scale_with_flux":
@@ -748,17 +729,15 @@
         elif self.ctype == "flux_balance":
             self.__rateconstant__()
         elif self.ctype == "react_with":
             self.__reaction__()
         elif self.ctype == "monod_type_limit":
             # self.__vardeltaout__()
             self.__rateconstant__()
-        elif self.ctype == "manual":
-            pass
-        else:
+        elif self.ctype != "manual":
             print(f"Connection Type {self.ctype} is unknown")
             raise ValueError(f"Unknown connection type {self.ctype}")
 
         # Set optional flux processes
         if self.alpha != "None":
             self.__alpha__()  # Set optional flux processes
             # self.__vardeltaout__()
@@ -930,33 +909,28 @@
         from esbmtk import Fractionation
 
         ph = Fractionation(
             name="_Pa",
             reservoir=self.r,
             flux=self.fh,
             register=self.fh,
-            alpha=self.kwargs["alpha"],
+            alpha=self.alpha,
             model=self.mo,
         )
         self.lop.append(ph)  #
 
     def __rateconstant__(self) -> None:
         """Add rate constant type process"""
 
         from esbmtk import (
             ScaleRelativeToMass,
             ScaleRelativeToConcentration,
             weathering,
         )
 
-        # this process requires that we use the vardeltaout process
-        if self.mo.m_type != "mass_only":
-            # self.__vardeltaout__()
-            pass
-
         if self.ctype == "scale_with_mass":
             if self.k_value != "None":
                 self.scale = self.k_value
                 print(
                     f"\n Warning: use scale instead of k_value for scale with mass type\n"
                 )
 
@@ -1020,19 +994,15 @@
     def info(self, **kwargs) -> None:
         """Show an overview of the object properties.
         Optional arguments are
         index  :int = 0 this will show data at the given index
         indent :int = 0 indentation
 
         """
-        if "index" not in kwargs:
-            index = 0
-        else:
-            index = kwargs["index"]
-
+        index = 0 if "index" not in kwargs else kwargs["index"]
         if "indent" not in kwargs:
             indent = 0
             ind = ""
         else:
             indent = kwargs["indent"]
             ind = " " * indent
 
@@ -1210,41 +1180,48 @@
         self.defaults: dict[str, any] = {
             "id": ["None", (str)],
             "source": ["None", (str, SourceGroup, Reservoir, ReservoirGroup)],
             "sink": ["None", (str, SinkGroup, Reservoir, ReservoirGroup)],
             "delta": ["None", (str, dict, tuple, int, float)],
             "rate": ["None", (Q_, str, dict, tuple, int, float)],
             "pl": ["None", (str, dict, tuple)],
-            "signal": ["None", (str, Signal)],
+            "signal": ["None", (str, Signal, dict)],
             "alpha": ["None", (str, dict, tuple, int, float)],
             "species": ["None", (str, dict, tuple, Species)],
             "ctype": ["None", (str, dict, tuple)],
             "ref_reservoirs": ["None", (str, dict, tuple, Reservoir)],
             "ref_flux": ["None", (str, dict, tuple, Flux)],
             "plot": ["yes", (str, dict, tuple)],
             "scale": [1, (str, dict, tuple, int, float)],
             "bypass": ["None", (dict, tuple, str)],
             "register": ["None", (str, tuple, Model)],
             "save_flux_data": [False, (bool, tuple)],
         }
 
         # provide a list of absolutely required keywords
-        self.lrk: list = ["source", "sink", "register"]
+        self.lrk: list = ["source", "sink"]
         self.__initialize_keyword_variables__(kwargs)
 
+        if self.register == "None":
+            self.register = self.source.register
         if self.save_flux_data == "None":
             self.save_flux_data = self.register.save_flux_data
             self.kwargs.update({"save_flux_data": self.register.save_flux_data})
 
         # # self.source.lor is a  list with the object names in the group
         self.mo = self.sink.lor[0].mo
         self.model = self.mo
         self.loc: list = []  # list of connection objects
 
         self.name = f"CG_{self.source.name}_to_{self.sink.name}"
+        # fixme this results in duplicate names in the model namespace.
+        # probably related to the create connection function
+        # if self.id != "None":
+        #     self.name = f"{self.name}@{self.id}"
+
         self.base_name = self.name
         self.parent = self.register
         self.__register_name_new__()
         self.__create_connections__()
 
     def add_connections(self, **kwargs) -> None:
         """Add connections to the connection group"""
@@ -1254,55 +1231,65 @@
 
     def __create_connections__(self) -> None:
         """Create Connections"""
 
         # find all sub reservoirs which have been specified by the ctype keyword
         self.connections: list = []
         for r, t in self.ctype.items():
+            # r = species/Reservoir Name
+            # t = connnection type, i.e. regular etc.
             if t == "None":
                 raise ValueError(
                     f"Connectiongroup {self.name} must specify 'ctype'. See help(Connectiongroup)"
                 )
             self.connections.append(r)
 
         # now we need to create defaults for all connections
-        self.cd: dict = {}  # connection dictionary
-        # loop over speces
+        self.cd: dict = {}  # connection dictionary with defaults
+        # loop over species
         for sp in self.connections:  # ["SO4", "H2S"]
+            # print(f"found species: ----------- {sp.name} ------------")
             self.cd[sp.n] = {
                 # "cid": self.id,
                 "cid": "None",
                 "plot": "yes",
                 "delta": "None",
                 "alpha": "None",
                 "rate": "None",
                 "scale": "None",
                 "ctype": "None",
                 "ref_reservoirs": "None",
                 "ref_flux": "None",
                 "bypass": "None",
+                "signal": "None",
             }
 
-            # test defaults against actual keyword value
-            for kcd, vcd in self.cd[sp.n].items():
-                if kcd in self.kwargs:  # found entry like ctype
-                    if r in self.kwargs[kcd]:  # {SO4: xxx}
-                        # update the entry
-                        self.cd[sp.n][kcd] = self.kwargs[kcd][sp]
+            # print(f"c0:\n Testing for {self.name}, sp = {sp.n}")
+            # loop over entries in defaults dict
+            for kcd, vcd in self.cd[sp.name].items():
+                # print(f"c1: kcd = {kcd}, vcd = {vcd}")
+                # test if key in default dict is also specified as connection keyword
+                if kcd in self.kwargs and sp in self.kwargs[kcd]:
+                    # print(f"c2: found kcd = {kcd} in kwargs, sp = {sp.n}")
+                    # update the entry
+                    self.cd[sp.n][kcd] = self.kwargs[kcd][sp]
+                # else:
+                # print(f"c3: did not find kcd = {kcd}, r = {sp.n}")
 
             a = Connect(
                 source=getattr(self.source, sp.n),
                 sink=getattr(self.sink, sp.n),
                 rate=self.cd[sp.n]["rate"],
                 delta=self.cd[sp.n]["delta"],
                 alpha=self.cd[sp.n]["alpha"],
                 plot=self.cd[sp.n]["plot"],
                 ctype=self.cd[sp.n]["ctype"],
                 scale=self.cd[sp.n]["scale"],
                 bypass=self.cd[sp.n]["bypass"],
+                signal=self.cd[sp.n]["signal"],
                 ref_reservoirs=self.cd[sp.n]["ref_reservoirs"],
                 ref_flux=self.cd[sp.n]["ref_flux"],
                 save_flux_data=self.save_flux_data,
                 groupname=True,
                 id=self.id,
                 register=self,
             )
@@ -1335,15 +1322,15 @@
     ~~~~~~~~
 
     AirSeaExchange(
         gas_reservoir= must be a gasreservoir
         liquid_reservoir = must be a reservoir
         solubility= as returned by the swc object
         area = Ocean.area, [m^2]
-        piston_velocity = 4.8*365, [m/yr]
+        piston_velocity = "4.8 m/d",
         id = str, optional
         water_vapor_pressure=Ocean.swc.p_H2O,
         ref_quantity = optional
         register = Model
         )
 
     In some cases the gas flux does not depend on the main reservoir species
@@ -1419,29 +1406,33 @@
 
         # register flux with gas reservoir
         self.gr.lof.append(self.fh)
         self.gr.lio[self.fh] = -1  # flux direction
         # register with connection
         self.lof.append(self.fh)
 
-        if self.lr.register == "None":
-            swc = self.lr.swc
-        else:
-            swc = self.lr.register.swc
-
+        # kas = air-sea gas exchange coefficient
+        # esbmtk solubility in mol/(m^3 * atm)
+        # esbmtk piston velocity in  m/d needs to be converted to
+        # esbmtk pCO2 = atm 
+        # zeebe expresses kas as mol/(m^2 * uatm * yr)
+        self.kas = self.solubility * self.piston_velocity
+        self.kas_zeebe = self.kas * 1e-6
+        
+        swc = self.lr.swc if self.lr.register == "None" else self.lr.register.swc
         # initialize process instance
         ph = GasExchange(
             name="_PGex",
             gas=self.gr,  # gas reservoir
             liquid=self.lr,  # reservoir
             ref_species=self.ref_species,  # concentration
             flux=self.fh,  # flux handle
             register=self.fh,
-            scale=self.scale,
-            solubility=self.solubility,
+            scale=self.scale,  # piston_velocity * area
+            solubility=self.solubility, # mol/(m^3 * atm)
             water_vapor_pressure=self.water_vapor_pressure,
             seawaterconstants=swc,
             isotopes=True,
         )
 
         # register process with reservoir
         ph.__register__(self.lr, self.fh)
@@ -1471,23 +1462,17 @@
 
         if testv == "None":
             self.ref_species = self.species
 
         self.lr = self.liquid_reservoir
         self.gr = self.gas_reservoir
 
-        if self.species.name in ["CO2", "DIC", "O2"]:
-            pass
-        else:
+        if self.species.name not in ["CO2", "DIC", "O2"]:
             raise ValueError(f"{self.species.name} not implemented yet")
 
         # decide if this connection needs isotope calculations
-        if self.gas_reservoir.isotopes:
-            self.isotopes = True
-        else:
-            self.isotopes = False
-
+        self.isotopes = bool(self.gas_reservoir.isotopes)
         self.mo = self.species.mo
         self.model = self.mo
         self.ctype = "gas_exchange"
         self.source = self.liquid_reservoir
         self.sink = self.gas_reservoir
```

### Comparing `esbmtk-0.8.0.0/esbmtk/esbmtk.py` & `esbmtk-0.9.0.1/esbmtk/esbmtk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,182 +1,165 @@
 """
-     esbmtk: A general purpose Earth Science box model toolkit
-     Copyright (C), 2020 Ulrich G. Wortmann
+esbmtk: A general purpose Earth Science box model toolkit Copyright
+(C), 2020 Ulrich G.  Wortmann
 
-     This program is free software: you can redistribute it and/or modify
-     it under the terms of the GNU General Public License as published by
-     the Free Software Foundation, either version 3 of the License, or
-     (at your option) any later version.
-
-     This program is distributed in the hope that it will be useful,
-     but WITHOUT ANY WARRANTY; without even the implied warranty of
-     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-     GNU General Public License for more details.
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or (at
+your option) any later version.
+
+This program is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+General Public License for more details.
 
-     You should have received a copy of the GNU General Public License
-     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 from __future__ import annotations
 import typing as tp
 from pandas import DataFrame
 import time
 from time import process_time
-from numba.typed import List
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 import logging
 import os
 import psutil
-import collections as col
 from . import ureg, Q_
 
 from .esbmtk_base import esbmtkBase
 
 from .utility_functions import (
     show_data,
     plot_geometry,
     get_plot_layout,
     find_matching_strings,
 )
 from .solver import (
     get_l_mass,
     execute,
-    execute_e,
     get_delta_h,
+    get_delta_from_concentration,
 )
 
 
 if tp.TYPE_CHECKING:
     from .extended_classes import GasReservoir, ExternalData, DataField
     from .connections import Connection
     from .processes import Process
 
 
 class Model(esbmtkBase):
-    """This class is used to specify a new model
-
-    Example:
-
-          esbmtkModel(name   =  "Test_Model",
-                      start    = "0 yrs",    # optional: start time
-                      stop     = "10000 yrs", # end time
-                      timestep = "2 yrs",    # as a string "2 yrs"
-                      offset = "0 yrs",    # optional: time offset for plot
-                      mass_unit = "mol",   #required
-                      volume_unit = "l", #required
-                      time_label = optional, defaults to "Time"
-                      display_precision = optional, defaults to 0.01,
-                      m_type = "mass_only/both"
-                      plot_style = 'default', optional defaults to 'default'
-                      number_of_datapoints = optional, see below
-                      step_limit = optional, see below
-                      register = 'local', see below
-                      save_flux_data = False, see below
-                      ideal_water = False
-                      use_ode = False
-                    )
-
-    ref_time: will offset the time axis by the specified amount, when
-                 plotting the data, .i.e., the model time runs from to
-                 100, but you want to plot data as if where from 2000
-                 to 2100, you would specify a value of 2000. This is
-                 for display purposes only, and does not affect the
-                 model. Care must be taken that any external data
-                 references the model time domain, and not the display
-                 time.
-
-    display precision: affects the on-screen display of data. It is
-                       also cutoff for the graphicak output. I.e., the
-                       interval f the y-axis will not be smaller than
-                       the display_precision.
-
-    m_type: enables or disables isotope calculation for the entire
-            model.  The default value is "Not set" in this case
-            isotopes will only be calculaten for reservoirs which set
-            the isotope keyword. 'mass_only' 'both' will override the
-            reservoir settings
-
-    register = local/None. If set to 'None' all objects are registered
-               in the global namespace the default setting is local,
-               i.e. all objects are registered in the model namespace.
-
-    save_flux_data: Normally, flux data is not stored. Set this to True
-               for debugging puposes. Note, Fluxes with signals are always
-               stored. You can also enable this option for inidividual
-               connections (fluxes).
-
-    get_delta_values: Compute delta values as postprocessing step.
-
-    All of the above keyword values are available as variables with
-    Model_Name.keyword
+    """This class is used to specify a new model.  See the __init__()
+    method for a detailed explanation of the parameters
 
     The user facing methods of the model class are
-       - Model_Name.info()
-       - Model_Name.save_data()
-       - Model_Name.plot_data()
-       - Model_Name.plot_reservoirs() takes an optional filename as argument
-       - Model_Name.plot([sb.DIC, sb.TA]) plot any object in the list
-       - Model_Name.save_state() Save the model state
-       - Model_name.read_state() Initialize with a previous model state
-       - Model_Name.run(), there are 2 optional arguments here, solver="hybrid"
-         and solver = "numba". Both involve a 3 to 5 second overhead. The hybrid
-         solver is compatible with all connection types, and about 3 times faster
-         than the  regular solver. The numba solver is about 10 faster, but currently
-         only supports a limited set of connection types.
-       - Model_Name.list_species()
-       - Model_name.flux_summary()
-       - Model_Name.connection_summary()
 
+        - Model_Name.info()
 
-    User facing variable are Model_Name.time which contains the time
-    axis.
+        - Model_Name.save_data()
 
-    Optional, you can provide the element keyword which will setup a
-    default set of Species for Carbon and Sulfur. In this case, there
-    is no need to define elements or species. The argument to this
-    keyword are either "Carbon", or "Sulfur" or both as a list
-    ["Carbon", "Sulfur"].
+        - Model_Name.plot_data()
 
+        - Model_Name.plot_reservoirs() takes an optional filename as
+          argument
 
-    Dealing with large datasets:
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        - Model_Name.plot([sb.DIC, sb.TA]) plot any object in the list
 
-    1) Limiting the size of the data which is being saved with save_data()
+        - Model_Name.save_state() Save the model state
 
-         number_of_datapoints = 100 will only write every nth data point to file.
-                                where n = timesteps/ number_of_datapoints
+        - Model_name.read_state() Initialize with a previous model
+          state
 
-         this defaults to 1000 until set explicitly.
+        - Model_Name.run(),
 
-    2) Reducing the memory footprint
+        - Model_Name.list_species()
 
-    Models with a long runtime can easily exceed the available
-    computer memory, as much if it is goobled up storing the model
-    results. In this case, one can set the optional parameter
+        - Model_name.flux_summary()
 
-       step_limit = 1E6
+        - Model_Name.connection_summary()
 
-    The above will limit the total number of iterations to 1E6, then
-    save the data up to this point, and then restart the
-    model. Subsequent results will be appended to the results.
+    User facing variable are Model_Name.time which contains the time
+    axis.
 
-    Caveat Emptor: If your model uses a signal instance, all signal
-    data must fit into a single iteration set. At present, there is no
-    support for signals which extend beyond the step_limit.
+    Optional, you can provide the element keyword which will setup a
+    default set of Species for Carbon and Sulfur.  In this case, there
+    is no need to define elements or species.  The argument to this
+    keyword are either "Carbon", or "Sulfur" or both as a list
+    ["Carbon", "Sulfur"].
 
-    In order to prevent the creation of massive datafiles, number_of_datapoints
-    defaults to 1000. Modify as needed.
 
     """
 
     def __init__(self, **kwargs: dict[any, any]) -> None:
-        """Init Sequence"""
+        """Initialize a model instance
+
+        :param **kwargs: A dictionary with key value pairs.
+
+            .. Example::
 
-        # from . import ureg, Q_
+                    esbmtkModel(name   =  "Test_Model", # required
+                                start    = "0 yrs",    # optional: start time
+                                stop     = "10000 yrs", # end time
+                                timestep = "2 yrs",    # as a string "2 yrs"
+                                max_step = "1000 yrs", # str, optional
+                                offset = "0 yrs",    # optional: time offset for plot
+                                mass_unit = "mol",   #required
+                                volume_unit = "l", # required
+                                concentration_unit="mol/kg | mol/l", required
+                                element = ["Carbon", "Sulfur" ]
+                                time_label = #  optional, defaults to "Time"
+                                display_precision = #  optional, defaults to 0.01,
+                                m_type = "mass_only/both" # defaults to mass_only
+                                plot_style = #  optional defaults to 'default'
+                                save_flux_data = False, see below
+                                ideal_water = False,
+                                parse_model = True,
+                              )
+
+                :param mass_unit: only tested with mol
+
+                :param volume_unit: only tested with liter
+
+                :concentration_unit: only tested with mol/kg
+
+                :param element: list with one or more species names
+
+                :param max_step: Limit automatic step size increase, i.e., the time
+                resolution of the model. Optional, defaults to the model duration/100
+
+                :param m_type: enables or disables isotope calculation for the
+                entire model.  The default value is "Not set" in this case
+                isotopes will only be calculated for reservoirs which set
+                the isotope keyword.  'mass_only' 'both' will override the
+                reservoir settings
+
+                :param ref_time: will offset the time axis by the specified
+                amount, when plotting the data, .i.e., the model time runs
+                from to 100, but you want to plot data as if where from
+                2000 to 2100, you would specify a value of 2000.  This is
+                for display purposes only, and does not affect the model.
+                Care must be taken that any external data references the
+                model time domain, and not the display time.
+
+                :param display precision: affects the on-screen display of data.
+                It is also cutoff for the graphicak output.  I.e., the
+                interval f the y-axis will not be smaller than the
+                display_precision.
+
+                :param save_flux_data: Normally, flux data is not stored.  Set
+                this to True for debugging puposes.  Note, fluxes with
+                signals are always stored.  You can also enable this
+                option for inidividual connections (fluxes).
+
+                :param ideal_water: if set, ignore seawater density/chemisrty
+                 calculations
+        """
 
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["M", (str)],
             "start": ["0 yrs", (str, Q_)],
             "stop": ["None", (str, Q_)],
             "offset": ["0 yrs", (str, Q_)],
             "timestep": ["None", (str, Q_)],
@@ -193,41 +176,41 @@
             "register": ["local", (str)],
             "save_flux_data": [False, (bool)],
             "full_name": ["None", (str)],
             "parent": ["None", (str)],
             "isotopes": [False, (bool)],
             "debug": [False, (bool)],
             "ideal_water": [True, (bool)],
-            "use_ode": [False, (bool)],
+            "use_ode": [True, (bool)],
+            # "max_step": ["None", (str)],
+            "parse_model": [True, (bool)],
         }
 
         # provide a list of absolutely required keywords
         self.lrk: list[str] = [
             "name",
             "stop",
             "timestep",
             "mass_unit",
             "volume_unit",
             "concentration_unit",
         ]
         self.__initialize_keyword_variables__(kwargs)
 
-        # self.__validateandregister__(kwargs)  # initialize keyword values
-
         # empty list which will hold all reservoir references
         self.lmo: list = []
         self.lmo2: list = []
         self.dmo: dict = {}  # dict of all model objects. useful for name lookups
 
         # start a log file
         for handler in logging.root.handlers[:]:
             logging.root.removeHandler(handler)
 
         fn: str = f"{kwargs['name']}.log"
-        logging.basicConfig(filename=fn, filemode="w", level=logging.WARN)
+        logging.basicConfig(filename=fn, filemode="w", level=logging.CRITICAL)
         self.__register_name_new__()
 
         self.lor: list = []
         self.lic: list = []  # list of all reservoir type objects
         # empty list which will hold all connector references
         self.loc: set = set()  # set with connection handles
         self.lel: list = []  # list which will hold all element references
@@ -248,61 +231,59 @@
         # list of signals
         self.los: list = []
         self.first_start = True  # keep track of repeated solver calls
         self.lof: list = []  # list of fluxes
 
         # Parse the strings which contain unit information and convert
         # into model base units For this we setup 3 variables which define
-        if not (
-            self.concentration_unit == "mol/kg"
-            or self.concentration_unit == "mol/l"
-            or self.concentration_unit == "mol/liter"
-        ):
+        if self.concentration_unit not in ["mol/kg", "mol/l", "mol/liter"]:
             raise ValueError(
                 f"{self.concentration_unit} must be either mol/l or mol/kg"
             )
 
         self.l_unit = ureg.meter  # the length unit
         self.t_unit = Q_(self.timestep).units  # the time unit
         self.d_unit = Q_(self.stop).units  # display time units
         self.m_unit = Q_(self.mass_unit).units  # the mass unit
         self.c_unit = Q_(self.concentration_unit).units  # the mass unit
         self.v_unit = Q_(self.volume_unit).units  # the volume unit
         # the concentration unit (mass/volume)
 
         self.f_unit = self.m_unit / self.t_unit  # the flux unit (mass/time)
         self.r_unit = self.v_unit / self.t_unit  # flux as volume/time
+
         # this is now defined in __init__.py
         # ureg.define('Sverdrup = 1e6 * meter **3 / second = Sv = Sverdrups')
 
         # legacy variable names
 
         self.start = self.ensure_q(self.start).to(self.t_unit).magnitude
         self.stop = self.ensure_q(self.stop).to(self.t_unit).magnitude
         self.offset = self.ensure_q(self.offset).to(self.t_unit).magnitude
-        # self.start = self.start + self.offset
-        # self.stop = self.stop + self.offset
-
+        self.start = self.start + self.offset
+        self.stop = self.stop + self.offset
         self.bu = self.t_unit
         self.base_unit = self.t_unit
         self.dt = Q_(self.timestep).magnitude
+        self.max_step = self.dt
         self.tu = str(self.bu)  # needs to be a string
         self.n = self.name
         self.mo = self.name
         self.model = self
         self.plot_style: list = [self.plot_style]
 
         self.xl = f"Time [{self.bu}]"  # time axis label
         self.length = int(abs(self.stop - self.start))
         self.steps = int(abs(round(self.length / self.dt)))
-
-        if self.steps < self.number_of_datapoints:
-            self.number_of_datapoints = self.steps
+        # self.steps = 100
+        # if self.steps < self.number_of_datapoints:
+        #     self.number_of_datapoints = self.steps
 
         self.time = (np.arange(self.steps) * self.dt) + self.start
+        self.time_ode = np.linspace(self.start, self.stop - self.dt, num=100)
         self.timec = np.empty(0)
         self.state = 0
 
         # calculate stride
         self.stride = int(self.steps / self.number_of_datapoints)
         self.reset_stride = self.stride
 
@@ -348,25 +329,21 @@
         )
         print(warranty)
 
         # initialize the hypsometry class
         hypsometry(name="hyp", model=self, register=self)
 
     def info(self, **kwargs) -> None:
-        """Show an overview of the object properties.
-        Optional arguments are
-        index  :int = 0 this will show data at the given index
-        indent :int = 0 indentation
+        """Show an overview of the object properties.  Optional
+        arguments are (name/default/explanation)
 
+        :param index: int = 0 # this will show data at the given index
+        :param indent: int = 0 # print indentation
         """
         off: str = "  "
-        # if "index" not in kwargs:
-        #    index = 0
-        # else:
-        # index = kwargs["index"]
 
         if "indent" not in kwargs:
             indent = 0
             ind = ""
         else:
             indent = kwargs["indent"]
             ind = " " * indent
@@ -379,88 +356,69 @@
         for e in self.lel:
             print(f"{ind}{e}")
             print(f"{off} Defined Species:")
             for s in e.lsp:
                 print(f"{off}{off}{ind}{s.n}")
 
     def save_state(self) -> None:
-        """Save model state. Similar to save data, but only saves the last 10
-        time-steps
-
+        """Save model state.  Similar to save data, but only saves the
+        last 10 time-steps
         """
 
-        start: int = -10
-        stop: int = -1
+        start: int = -5
+        stop: int = None
         stride: int = 1
         prefix: str = "state_"
 
-        for r in self.lor:
+        for r in self.lor:  # loop over reservoirs
             r.__write_data__(prefix, start, stop, stride, False, "state")
 
-        for r in self.lvr:
-            r.__write_data__(prefix, start, stop, stride, False, "state")
+        # for r in self.lvr:
+        #    r.__write_data__(prefix, start, stop, stride, False, "state")
 
     def save_data(self, **kwargs) -> None:
         """Save the model results to a CSV file. Each reservoir will have
         their own CSV file
 
         Optional arguments:
-        stride = int  # every nth element
-        start = int   # start index
-        stop = int    # end index
-        append = True/False #
+        :param stride: int = 0  # every nth element
+        :param start: int  = 0  # start index
+        :param stop: int = self.steps # end index
+        :param append: bool = False #
 
         """
 
         for k, v in kwargs.items():
             if not isinstance(v, int):
                 print(f"{k} must be an integer number")
                 raise ValueError(f"{k} must be an integer number")
 
-        if "stride" in kwargs:
-            stride = kwargs["stride"]
-        else:
-            stride = self.stride
-
-        if "start" in kwargs:
-            start = kwargs["start"]
-        else:
-            start = 0
-
-        if "stop" in kwargs:
-            stop = kwargs["stop"]
-        else:
-            stop = self.steps
-
-        if "append" in kwargs:
-            append = kwargs["append"]
-        else:
-            append = False
-
+        stride = kwargs.get("stride", self.stride)
+        start = kwargs.get("start", 0)
+        stop = kwargs.get("stop", self.steps)
+        append = kwargs.get("append", False)
         prefix = ""
 
         print(f"start = {start}, stop = {stop}, stride={stride}, append ={append}")
         for r in self.lor:
             # print(f"R = {r.full_name}")
             # print(f"start = {start}, stop = {stop}, stride={stride}, append ={append}")
             r.__write_data__(prefix, start, stop, stride, append, "data")
 
         # save data fields
         # for r in self.ldf:
         #     r.__write_data__(prefix, start, stop, stride, append)
-        print("Writing virtual reservoir data")
-        for r in self.lvr:
-            r.__write_data__(prefix, start, stop, stride, append, "data")
+        # print("Writing virtual reservoir data")
+        # for r in self.lvr:
+        #    r.__write_data__(prefix, start, stop, stride, append, "data")
         print("done writing")
 
     def restart(self):
-        """Restart the model with result of the last run.
-        This is useful for long runs which otherwise would used
-        to much memory
-
+        """Restart the model with result of the last run.  This is
+        useful for long runs which otherwise would used to much memory
         """
 
         for r in self.lor:
             r.__reset_state__()
             for f in r.lof:
                 f.__reset_state__()
 
@@ -476,94 +434,102 @@
         self.time = (np.arange(self.steps) * self.dt) + self.start
         print(f"new start = {self.start}, new stop = {self.stop}")
         print(f"time[0] = {self.time[0]} time[-1] = {self.time[-1]}")
         # print(f"len of timec {len(self.timec)}")
         # self.time = (arange(self.steps) * self.dt) + self.start
 
     def read_state(self):
-        """This will initialize the model with the result of a previous model
-        run.  For this to work, you will need issue a
-        Model.save_state() command at then end of a model run. This
+        """This will initialize the model with the result of a
+        previous model run.  For this to work, you will need issue a
+        Model.save_state() command at then end of a model run.  This
         will create the necessary data files to initialize a
         subsequent model run.
-
         """
 
-        from esbmtk import Reservoir, GasReservoir
+        from esbmtk import Reservoir, GasReservoir  # GasReservoir
 
         for r in self.lor:
             if isinstance(r, (Reservoir, GasReservoir)):
-                # print(f" reading from {r.full_name}")
                 r.__read_state__("state")
 
-        for r in self.lvr:
-            # print(f"lvr  reading from {r.full_name}")
-            r.__read_state__("state")
+        # for r in self.lvr:
+        #     # print(f"lvr  reading from {r.full_name}")
+        #     r.__read_state__("state")
 
     def merge_temp_results(self):
-        """Replace the datafields which were used for an individual iteration
-        with the data we saved from the previous iterations
-
+        """Replace the datafields which were used for an individual
+        iteration with the data we saved from the previous iterations
         """
 
         self.time = self.timec
         for r in self.lor:
             r.__merge_temp_results__()
             for f in r.lof:
                 f.__merge_temp_results__()
 
         for r in self.lvr:
             r.__merge_temp_results__()
 
-    def plot(self, pl: list = [], **kwargs) -> None:
+    def plot(self, pl: list = None, **kwargs) -> None:
         """Plot all objects specified in pl
 
-        M.plot([sb.PO4, sb.DIC],fn=test.pdf)
+        Example::
 
-        fn is optional
-        """
+            M.plot([sb.PO4, sb.DIC], fn='test.pdf')
 
-        if "fn" in kwargs:
-            filename = kwargs["fn"]
-        else:
-            filename = f"{self.n}.pdf"
+        fn is optional and defaults to the Model Name
+        """
 
+        if pl is None:
+            pl = []
+        filename = kwargs.get("fn", f"{self.n}.pdf")
         noo: int = len(pl)
-        size, geo = plot_geometry(noo)  # adjust layout
-        fig, ax = plt.subplots(geo[0], geo[1])  # row, col
+        size, [row, col] = plot_geometry(noo)  # adjust layout
+        fig, ax = plt.subplots(row, col)  # row, col
         axs = [[], []]
 
         """ The shape of the ax value of subplots depends on the figure
         geometry. So we need to ensure we are dealing with a 2-D array
         """
-        if geo[0] == 1 and geo[1] == 1:  # row=1, col=1 only one window
-            axs[0].append(ax)
-        elif geo[0] > 1 and geo[1] == 1:  # mutiple rows, one column
-            for i in range(geo[0]):
-                axs[0].append(ax[i])
-        elif geo[0] == 1 and geo[1] > 1:  # 1 row, multiple columns
+        if row == 1 and col == 1:  # row=1, col=1 only one window
+            axs = ax
+        elif row > 1 and col == 1:  # mutiple rows, one column
+            axs = []
+            for i in range(row):
+                axs.append(ax[i])
+        elif row == 1 and col:  # 1 row, multiple columns
+            print(f"one row, mutiple cols")
             for i in range(geo[1]):
-                axs[1].append(ax[i])
+                axs.append(ax[i])
         else:
             axs = ax  # mutiple rows and mutiple columns
 
         # ste plot parameters
         plt.style.use(self.plot_style)
         fig.canvas.manager.set_window_title(f"{self.n} Reservoirs")
         fig.set_size_inches(size)
 
         i = 0  # loop over objects
-        for c in range(geo[0]):  # rows
-            for r in range(geo[1]):  # columns
-                if i < noo:
-                    pl[i].__plot__(self, axs[c][r])
-                    axs[c][r].set_title(pl[i].full_name)
-                    i = i + 1
-                else:
-                    axs[c][r].remove()
+        for c in range(row):  # rows
+            if col > 1:
+                for r in range(col):  # columns
+                    if i < noo:
+                        pl[i].__plot__(self, axs[c][r])
+                        axs[c][r].set_title(pl[i].full_name)
+                        i = i + 1
+                    else:
+                        axs[c][r].remove()
+            elif row > 1:
+                pl[i].__plot__(self, axs[c])
+                axs[c].set_title(pl[i].full_name)
+                i = i + 1
+            else:
+                pl[i].__plot__(self, axs)
+                axs.set_title(pl[i].full_name)
+                i = i + 1
 
         fig.subplots_adjust(top=0.88)
         fig.tight_layout()
         plt.show(block=False)  # create the plot windows
         fig.savefig(filename)
 
     def run(self, **kwargs) -> None:
@@ -574,79 +540,63 @@
         # this has nothing todo with self.time below!
         wts = time.time()
         start: float = process_time()
         # new: np.ndarray = np.zeros(4)
 
         # put direction dictionary into a list
         for r in self.lor:  # loop over reservoirs
-            r.lodir = []
-            for f in r.lof:  # loop over fluxes
-                a = r.lio[f]
-                r.lodir.append(a)
-
+            r.lodir = [r.lio[f] for f in r.lof]
         # take care of objects which require a delayed init
         for o in self.lto:
             o.__delayed_init__()
 
-        if "solver" not in kwargs:
-            solver = "python"
-        else:
-            solver = kwargs["solver"]
-
+        solver = "ode" if "solver" not in kwargs else kwargs["solver"]
         self.solver = solver
         if self.number_of_solving_iterations > 0:
-
             for i in range(self.number_of_solving_iterations):
                 print(
                     f"\n Iteration {i+1} out of {self.number_of_solving_iterations}\n"
                 )
                 self.__run_solver__(solver)
 
-                print(f"Restarting model")
+                print("Restarting model")
                 self.restart()
 
             print("Merge results")
             self.merge_temp_results()
             self.steps = self.number_of_datapoints
             # after merging, the model steps = number_of_datapoints
-        # print("Saving data")
-        # self.save_data(start=0, stop=self.number_of_datapoints, stride=1)
-        # print("Done Saving")
         else:
             self.__run_solver__(solver, kwargs)
 
-        # flag that the model has executed
-        self.state = 1
-
+        self.state = 1  # flag that the model has executed
         duration: float = process_time() - start
         wcd = time.time() - wts
-        print(f"\n Execution took {duration:.2e} cpu seconds, wt = {wcd:.2e}\n")
-
+        print(f"\n Execution took {duration:.2f} cpu seconds, wt = {wcd:.2f}\n")
         process = psutil.Process(os.getpid())
         print(f"This run used {process.memory_info().rss/1e9:.2f} Gbytes of memory \n")
 
     def get_delta_values(self):
-        """Calculate the isotope ratios in the usual delta notation"""
-
+        """Calculate masses and isotope ratios in the usual delta notation"""
         for r in self.lor:
             if r.isotopes:
+                r.m = r.c * r.volume
                 r.d = get_delta_h(r)
 
         # for vr in self.lvr:
         #     vr.d = get_delta_h(vr)
 
         # for f in self.lof:
         #     if f.save_flux_data:
         #         f.d = get_delta_h(f)
 
     def sub_sample_data(self):
-        """Subsample the data. No need to save 100k lines of data You need to
-        do this _after_ saving the state, but before plotting and
-        saving the data
-
+        """Subsample the data.  No need to save 100k lines of data You
+        need to do this _after_ saving the state, but before plotting
+        and saving the data
         """
 
         stride = int(len(self.time) / self.number_of_datapoints)
 
         if stride > 1:
             self.time = self.time[2:-2:stride]
 
@@ -655,183 +605,155 @@
 
             for vr in self.lvr:
                 vr.__sub_sample_data__(stride)
 
             for f in self.lof:
                 f.__sub_sample_data__(stride)
 
-        
     def __run_solver__(self, solver: str, kwargs: dict) -> None:
-        from .ODEINT_Solver import run_solver
-
-        if solver == "numba":
-            execute_e(
-                self,
-                self.lop,
-                self.lor,
-                self.lpc_f,
-                self.lpc_r,
-            )
-        elif solver == "odeint":
-            run_solver(self)
+        if solver == "ode":
+            print("Using ODE solver")
+            self.ode_solver(kwargs)
         elif solver == "ode_uli":
-            self.ode_uli(kwargs)
+            print("\n\n the solver type 'ode_uli' is deprecated, please use 'ode' \n\n")
+            self.ode_solver(kwargs)
         elif solver == "python":
+            print("\n\n the solver type 'python' is deprecated, please use 'ode' \n\n")
             execute(self.time, self.lop, self.lor, self.lpc_f, self.lpc_r)
         else:
             raise ValueError(
-                f"Solver={solver} is unkknown, use 'python/numba/odeint/ode_uli'"
+                f"Solver={self.solver} is unkknown, use 'python/numba/odeint/ode'"
             )
 
-    def ode_uli(self, kwargs):
-        """Use the ode solver based on Uli's approach"""
+    def ode_solver(self, kwargs):
+        """
+        Use the ode solver
+        """
         from esbmtk import Q_, write_equations_2, get_initial_conditions
-        from scipy.integrate import odeint, solve_ivp
+        from scipy.integrate import solve_ivp
         import sys
         import pathlib as pl
 
         # build equation file
-        R, icl, cpl, ipl = get_initial_conditions(self)
+        rtol = 1e-4
+        R, icl, cpl, ipl, atol = get_initial_conditions(self, rtol)
         self.R = R
         self.icl = icl
         self.cpl = cpl
         self.ipl = ipl
 
         # write equation system
-        eqs_file = write_equations_2(self, R, icl, cpl, ipl)
-        print(f"loc = {eqs_file.resolve()}")
+        if self.parse_model:
+            eqs_file = write_equations_2(self, R, icl, cpl, ipl)
+            # print(f"loc = {eqs_file.resolve()}")
+        else:
+            print("\n WARNING: Reusing equation file\n")
 
         # ensure that cwd is in the load path. Required for windows
         cwd: pl.Path = pl.Path.cwd()
         sys.path.append(cwd)
 
         # import equation system
         from equations import setup_ode
 
         ode_system = setup_ode(self)  # create ode system instance
-        self.ode_system = ode_system
-
-        if "method" in kwargs:
-            method = kwargs["method"]
-        else:
-            method = "RK23"
-
-        if "stype" in kwargs:
-            stype = kwargs["stype"]
-        else:
-            stype = "solve_ivp"
+        # self.ode_system = ode_system
+        method = kwargs["method"] if "method" in kwargs else "BDF"
+        stype = kwargs["stype"] if "stype" in kwargs else "solve_ivp"
 
         if stype == "solve_ivp":
-            results = solve_ivp(
+            self.results = solve_ivp(
                 ode_system.eqs,
                 (self.time[0], self.time[-1]),
                 R,
                 args=(self,),
                 method=method,
-                # t_eval=self.time,
-                atol=1e-12,
-                first_step=Q_("1 hour").to(self.t_unit).magnitude,
+                atol=atol,
+                rtol=1e-6,
+                t_eval=self.time_ode,
+                first_step=Q_("1 second").to(self.t_unit).magnitude,
                 # dense_output=True,
-                # max_step=1,
+                max_step=self.max_step,
             )
 
-            # interpolate signals into the ode time domain
-            # must be done before changing model time domain
-            for s in self.los:
-                s.data.m = np.interp(
+        self.post_process_data(self.results, ode_system)
+
+    def post_process_data(self, results, ode_system) -> None:
+        """Map solver results back into esbmtk structures
+
+        :param results: numpy arrays with solver results
+        """
+
+        # interpolate signals into the ode time domain
+        # must be done before changing model time domain
+        for s in self.los:
+            s.data.m = np.interp(
+                results.t,
+                self.time,
+                s.data.m,
+            )
+            if s.isotopes:
+                s.data.l = np.interp(
                     results.t,
                     self.time,
-                    s.data.m,
+                    s.data.l,
                 )
 
-            # interpolate external data into ode time domain
-            # must be done before changing model time domain
-            # for ed in self.led:
-            #     ed.y = np.interp(results.t, ed.x, ed.y)
-
-            # assign results to the esbmtk variables
-            for i, r in enumerate(icl):
-                r.c = results.y[i]
-            self.time = results.t
-
-            # interpolate intermediate results to match the model
-            # time scale. This only applies to data in virtual
-            # data fields
-            for gf in self.lpc_r:
-                # get cs instance handle
-                cs = getattr(gf.register, "cs")
-                for k, v in cs.vr_datafields.items():
-                    if "table" not in k:
-                        od = getattr(cs, k)  # get ode data
-                        # print(f"R = {gf.full_name} - {k}:\n"
-                        #       f"len(fp) = {len(od[0 : self.ode_system.i])}, "
-                        #       f"len(xp) = {len(self.ode_system.t)}, "
-                        #       f"i = {self.ode_system.i}")
-                        od = np.interp(
-                            self.time,
-                            self.ode_system.t,
-                            od[0 : self.ode_system.i],
-                        )
-                        setattr(cs, k, od)
-
-        else:
-            results = odeint(ode_system.eqs, R, t=self.time, args=(self,), tfirst=True)
-            # assign results
-            for i, r in enumerate(icl):
-                r.c = results[:, i]
-
-        self.results = results
-
-    def __step_process__(self, r: Reservoir, i: int) -> None:
-        """For debugging. Provide reservoir and step number,"""
-        for p in r.lop:  # loop over reservoir processes
-            print(f"{p.n}")
-            p(r, i)  # update fluxes
-
-    def __step_update_reservoir__(self, r: Reservoir, i: int) -> None:
-        """For debugging. Provide reservoir and step number,"""
-        flux_list = r.lof
-        # new = sum_fluxes(flux_list,r,i) # integrate all fluxes in self.lof
-
-        ms = ls = hs = 0
-        for f in flux_list:  # do sum of fluxes in this reservoir
-            direction = r.lio[f]
-            ms = ms + f.m[i] * direction  # current flux and direction
-            ls = ls + f.l[i] * direction  # current flux and direction
-            hs = hs + f.h[i] * direction  # current flux and direction
-
-        new = np.array([ms, ls, hs])
-        new = new * r.mo.dt  # get flux / timestep
-        new = new + r[i - 1]  # add to data from last time step
-        # new = new * (new > 0)  # set negative values to zero
-        r[i] = new  # update reservoir data
+        # interpolate external data into ode time domain
+        # must be done before changing model time domain
+        for ed in self.led:
+            ed.y = np.interp(results.t, ed.x, ed.y)
+        # assign results to the esbmtk variables
+        i = 0
+        for r in self.icl:
+            r.c = results.y[i]
+            # this needs fixing if we have variable volumes
+            r.m = results.y[i] * r.volume
+            i = i + 1
+            if r.isotopes:
+                r.l = results.y[i]
+                i = i + 1
+                r.d = get_delta_from_concentration(r.c, r.l, r.sp.r)
+
+        self.time = results.t
+
+        steps = len(results.t)  # get number of solver steps
+        for f in self.lof:
+            if f.save_flux_data:
+                f.m = f.m[0:steps]
+                if f.isotopes:
+                    f.l = f.l[0:steps]
+                    f.d = get_delta_h(f)
+
+        # self.results = results # save results for debugging
 
     def list_species(self):
         """List all  defined species."""
         for e in self.lel:
             print(f"{e.n}")
             e.list_species()
 
-    def flux_summary(self, **kwargs: dict) -> tuple:
+    def flux_summary(self, **kwargs: dict) -> [tuple | None]:
         """Show a summary of all model fluxes
 
         Optional parameters:
 
-        filter_by :str = filter on flux name or part of flux name
-                         words separated by blanks act as additional
-                         conditions, i.e., all words must occur in a given name
-
-        return_list: bool = False, if True return a list of fluxes matching the filter_by string.
+        :param filter_by: str = "" # filter on flux name or part of
+            flux name words separated by blanks act as additional
+            conditions, i.e., all words must occur in a given name
 
-        exclude:str = exclude all results matching this string
+        :param return_list: bool = False, # if True return a list of
+            fluxes matching the filter_by string.
 
-        Example:
+        :param exclude: str = "" # exclude all results matching this
+            string
 
-              names = M.flux_summary(filter_by="POP A_sb", return_list=True)
+            Example::
 
+                names = M.flux_summary(filter_by="POP A_sb", return_list=True)
         """
 
         fby = ""
         rl: list = []
         exclude: str = ""
         check_exlusion: bool = False
 
@@ -848,128 +770,124 @@
         if "return_list" in kwargs:
             return_list = True
         else:
             return_list = False
             print(f"\n --- Flux Summary -- filtered by {fby}\n")
 
         for f in self.lof:  # loop over flux list
-
-            if find_matching_strings(f.full_name, fby):
-                if check_exlusion:
-                    if exclude not in f.full_name:
-                        rl.append(f)
-                        if not return_list:
-                            print(f"{f.full_name}")
-                else:
-                    rl.append(f)
-                    if not return_list:
-                        print(f"{f.full_name}")
-
+            if find_matching_strings(f.full_name, fby) and (
+                check_exlusion and exclude not in f.full_name or not check_exlusion
+            ):
+                rl.append(f)
+                if not return_list:
+                    print(f"{f.full_name}")
         if not return_list:
             rl = None
 
         return rl
 
     def connection_summary(self, **kwargs: dict) -> None:
         """Show a summary of all connections
 
         Optional parameters:
 
-        filter_by :str = filter on flux name or part of flux name
-                         words separated by blanks act as additional conditions
-                         i.e., all words must occur in a given name
-
+        :param filter_by: str = "" # filter on flux name or part of
+            flux name words separated by blanks act as additional
+            conditions i.e., all words must occur in a given name
         """
 
+        rl = []
         if "filter_by" in kwargs:
             fby: list = kwargs["filter_by"].split(" ")
         else:
             fby: bool = False
 
         if "filter" in kwargs:
             raise ValueError("use filter_by instead of filter")
 
-        print(f"fby = {fby}")
-        self.cg_list: list = []
-        # extract all connection groups. Note that loc contains all connections
-        # i.e., not connection groups.
-        for c in list(self.loc):
-            # if "." in c.full_name:
-            # if c.register not in self.cg_list and c.register != "None":
-            if c not in self.cg_list and c.register != "None":
-                self.cg_list.append(c)
-            else:  # this is a regular connnection
-                self.cg_list.append(c)
-
-        print(f"\n --- Connection Group Summary -- filtered by {fby}\n")
-        print(f"       run the following command to see more details:\n")
+        if "silent" not in kwargs:
+            print(f"\n --- Connection Group Summary -- filtered by {fby}\n")
+            print(f"       run the following command to see more details:\n")
 
         # test if all words of the fby list occur in c.full_name. If yes,
-
+        self.cg_list: list = list(list(self.loc))
         for c in self.cg_list:
-            if not fby:
-                print(f"{c.full_name}.info()")
-            else:
-                if find_matching_strings(c.full_name, fby):
-                    print(f"{c.full_name}.info()")
-
-        print("")
+            if fby and find_matching_strings(c.full_name, fby) or not fby:
+                if "silent" in kwargs or "return_list" in kwargs:
+                    rl.append(c)
+                else:
+                    print(f"{c.full_name}.info()\n")
+        return rl
 
     def clear(self):
-        """delete all model objects"""
-
+        """
+        delete all model objects
+        """
         for o in self.lmo:
             print(f"deleting {o}")
             del __builtins__[o]
 
 
 class Element(esbmtkBase):
     """Each model, can have one or more elements.  This class sets
     element specific properties
 
     Example::
 
-            Element(name      = "S "           # the element name
-                    model     = Test_model     # the model handle
-                    mass_unit =  "mol",        # base mass unit
-                    li_label  =  "$^{32$S",    # Label of light isotope
-                    hi_label  =  "$^{34}S",    # Label of heavy isotope
-                    d_label   =  r"$\delta^{34}$S",  # Label for delta value
-                    d_scale   =  "VCDT",       # Isotope scale
-                    r         = 0.044162589,   # isotopic abundance ratio for element
-                  )
-
+        Element(name      = "S "           # the element name
+                model     = Test_model     # the model handle
+                mass_unit =  "mol",        # base mass unit
+                li_label  =  "$^{32$S",    # Label of light isotope
+                hi_label  =  "$^{34}S",    # Label of heavy isotope
+                d_label   =  r"$\delta^{34}$S",  # Label for delta value
+                d_scale   =  "VCDT",       # Isotope scale
+                r         = 0.044162589,   # isotopic abundance ratio for element
+              )
     """
 
     # set element properties
     def __init__(self, **kwargs) -> any:
-        """Initialize all instance variables"""
+        """Initialize all instance variables Defaults are as follows::
+
+            self.defaults: dict[str, list[any, tuple]] = {
+               "name": ["M", (str)],
+               "model": ["None", (str, Model)],
+               "register": ["None", (str, Model)],
+               "full_name": ["None", (str)],
+               "li_label": ["None", (str)],
+               "hi_label": ["None", (str)],
+               "d_label": ["None", (str)],
+               "d_scale": ["None", (str)],
+               "r": [1, (float, int)],
+               "mass_unit": ["None", (str, Q_)],
+               "parent": ["None", (str, Model)],
+
+        }
+
+        Required keywords: "name", "model", "mass_unit"
+        """
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["M", (str)],
             "model": ["None", (str, Model)],
             "register": ["None", (str, Model)],
             "full_name": ["None", (str)],
             "li_label": ["None", (str)],
             "hi_label": ["None", (str)],
             "d_label": ["None", (str)],
             "d_scale": ["None", (str)],
             "r": [1, (float, int)],
             "mass_unit": ["None", (str, Q_)],
             "parent": ["None", (str, Model)],
         }
 
-        # provide a list of absolutely required keywords
-        # provide a list of absolutely required keywords
+        # list of absolutely required keywords
         self.lrk: list = ["name", "model", "mass_unit"]
         self.__initialize_keyword_variables__(kwargs)
 
         self.parent = self.model
-        # self.__initerrormessages__()
-        # self.__validateandregister__(kwargs)  # initialize keyword values
-
         # legacy name aliases
         self.n: str = self.name  # display name of species
         self.mo: Model = self.model  # model handle
         self.mu: str = self.mass_unit  # display name of mass unit
         self.ln: str = self.li_label  # display name of light isotope
         self.hn: str = self.hi_label  # display name of heavy isotope
         self.dn: str = self.d_label  # display string for delta
@@ -979,36 +897,53 @@
 
         if self.mo.register == "local" and self.register == "None":
             self.register = self.mo
 
         self.__register_name_new__()
 
     def list_species(self) -> None:
-        """List all species which are predefined for this element"""
+        """
+        List all species which are predefined for this element
+        """
 
         for e in self.lsp:
             print(e.n)
 
     def __register_species_with_model__(self) -> None:
-        """Bit of  hack, but makes model code more readable"""
+        """
+        Bit of hack, but makes model code more readable
+        """
 
         for s in self.lsp:
             setattr(self.model, s.name, s)
 
 
 class Species(esbmtkBase):
-    """Each model, can have one or more species.  This class sets species
-    specific properties
+    """Each model, can have one or more species.  This class sets
+    species specific properties
 
-          Example::
+    Example::
+
+        Species(name = "SO4",
+                element = S,
 
-                Species(name = "SO4",
-                        element = S,
     )
 
+    Defaults::
+
+        self.defaults: dict[any, any] = {
+             "name": ["None", (str)],
+             "element": ["None", (Element, str)],
+             "display_as": [kwargs["name"], (str)],
+             "m_weight": [0, (int, float, str)],
+             "register": ["None", (Model, Element, Reservoir, GasReservoir)],
+             "parent": ["None", (Model, Element, Reservoir, GasReservoir)],
+         }
+
+    Required keywords: "name", "element"
     """
 
     # set species properties
     def __init__(self, **kwargs) -> None:
         """Initialize all instance variables"""
 
         from esbmtk import GasReservoir
@@ -1049,29 +984,31 @@
 
         if self.mo.register == "local" and self.register == "None":
             self.register = self.mo
         self.__register_name_new__()
 
 
 class ReservoirBase(esbmtkBase):
-    """Base class for all Reservoir objects"""
+    """
+    Base class for all Reservoir objects
+    """
 
     def __init__(self, **kwargs) -> None:
-
         raise NotImplementedError(
             "ReservoirBase should never be used. Use the derived classes"
         )
 
     def __set_legacy_names__(self, kwargs) -> None:
         """
         Move the below out of the way
         """
 
         from esbmtk import get_box_geometry_parameters
 
+        self.atol: list[float] = [1.0, 1.0]  # tolerances
         self.lof: list[Flux] = []  # flux references
         self.led: list[ExternalData] = []  # all external data references
         self.lio: dict[str, int] = {}  # flux name:direction pairs
         self.lop: list[Process] = []  # list holding all processe references
         self.loe: list[Element] = []  # list of elements in thiis reservoir
         self.doe: dict[Species, Flux] = {}  # species flux pairs
         self.loc: set[Connection] = set()  # set of connection objects
@@ -1108,84 +1045,83 @@
 
         # decide whether we use isotopes
         if self.mo.m_type == "both":
             self.isotopes = True
         elif self.mo.m_type == "mass_only":
             self.isotopes = False
 
-        if self.geometry != "None":
+        if self.geometry != "None" and self.geometry_unset:
             get_box_geometry_parameters(self)
 
         if self.display_precision == 0:
             self.display_precision = self.mo.display_precision
 
         self.parent = self.register
 
     # setup a placeholder setitem function
     def __setitem__(self, i: int, value: float):
         return self.__set_data__(i, value)
 
     def __call__(self) -> None:  # what to do when called as a function ()
-        pass
         return self
 
     def __getitem__(self, i: int) -> np.ndarray:
-        """Get flux data by index"""
+        """
+        Get flux data by index
+        """
 
         return np.array([self.m[i], self.l[i], self.c[i]])
 
     def __set_with_isotopes__(self, i: int, value: float) -> None:
-        """write data by index"""
+        """
+        :param i: index
+        :param value: array of [mass, li, hi, d]
 
+        """
         self.m[i]: float = value[0]
         # update concentration and delta next. This is computationally inefficient
         # but the next time step may depend on on both variables.
         self.c[i]: float = value[0] / self.v[i]  # update concentration
-        self.l[i]: float = value[1]
+        self.l[i]: float = value[1] / self.v[i]  # update concentration
 
     def __set_without_isotopes__(self, i: int, value: float) -> None:
-        """write data by index"""
+        """
+        :param i: index
+        :param value: array of [mass]
 
+        """
         self.m[i]: float = value[0]
         self.c[i]: float = self.m[i] / self.v[i]  # update concentration
 
     def __update_mass__() -> None:
-        """Place holder function"""
+        """
+        Place holder function
+        """
 
         raise NotImplementedError("__update_mass__ is not yet implmented")
 
-    def get_process_args(self):
-        """Provide the data structure which needs to be passed to the numba solver"""
-
-        print(f"Name = {self.full_name}")
-        data = List(
-            [
-                self.m,  # 0
-                self.l,  # 1
-                self.c,  # 2
-                self.v,  # 3
-            ]
-        )
-
-        func_name: col.Callable = self.__update_mass__
-        params = List([float(self.reservoir.species.element.r)])
-
-        return func_name, data, params
-
     def __write_data__(
         self,
         prefix: str,
         start: int,
         stop: int,
         stride: int,
         append: bool,
         directory: str,
     ) -> None:
-        """To be called by write_data and save_state"""
+        """Write data to file.  This function is called by the
+        write_data() and save_state() methods
 
+        :param prefix:
+        :param start:
+        :param stop:
+        :param stride:
+        :param append:
+        :param directory:
+        """
         from pathlib import Path
 
         p = Path(directory)
         p.mkdir(parents=True, exist_ok=True)
 
         # some short hands
         sn = self.sp.n  # species name
@@ -1211,59 +1147,41 @@
             )
 
         # build the dataframe
         df: pd.dataframe = DataFrame()
 
         df[f"{rn} Time [{mtu}]"] = self.mo.time[start:stop:stride]  # time
         df[f"{rn} {sn} [{smu}]"] = self.m[start:stop:stride]  # mass
-        df[f"{rn} {sp.ln} [{smu}]"] = self.l[start:stop:stride]  # light isotope
+        if self.isotopes:
+            df[f"{rn} {sp.ln} [{cmu}]"] = self.l[start:stop:stride]  # light isotope
         df[f"{rn} {sn} [{cmu}]"] = self.c[start:stop:stride]  # concentration
 
-        fullname: list = []
-
-        for f in self.lof:  # Assemble the headers and data for the reservoir fluxes
-            if f.full_name in fullname:
-                raise ValueError(f"{f.full_name} is a double")
-            fullname.append(f.full_name)
-
-            if f.save_flux_data:
-                df[f"{f.full_name} {sn} [{fmu}]"] = f.m[start:stop:stride]  # m
-                df[f"{f.full_name} {sn} [{sp.ln}]"] = f.l[start:stop:stride]  # l
-            else:
-                df[f"{f.full_name} {sn} [{fmu}]"] = f.fa[0]  # m
-                df[f"{f.full_name} {sn} [{sp.ln}]"] = f.fa[1]  # l
-
         file_path = Path(fn)
-        if append:
-            if file_path.exists():
-                df.to_csv(file_path, header=False, mode="a", index=False)
-            else:
-                df.to_csv(file_path, header=True, mode="w", index=False)
+        if append and file_path.exists():
+            df.to_csv(file_path, header=False, mode="a", index=False)
         else:
             df.to_csv(file_path, header=True, mode="w", index=False)
-
         return df
 
-    def __sub_sample_data__(self,stride) -> None:
-        """There is usually no need to keep more than a thousand data points
-        so we subsample the results before saving, or processing them
-
+    def __sub_sample_data__(self, stride) -> None:
+        """There is usually no need to keep more than a thousand data
+        points so we subsample the results before saving, or
+        processing them
         """
 
         # print(f"Reset data with {len(self.m)}, stride = {self.mo.reset_stride}")
         self.m = self.m[2:-2:stride]
         self.l = self.l[2:-2:stride]
         self.c = self.c[2:-2:stride]
 
     def __reset_state__(self) -> None:
-        """Copy the result of the last computation back to the beginning
-        so that a new run will start with these values
+        """Copy the result of the last computation back to the
+        beginning so that a new run will start with these values
 
         save the current results into the temp fields
-
         """
 
         # print(f"Reset data with {len(self.m)}, stride = {self.mo.reset_stride}")
         self.mc = np.append(self.mc, self.m[0 : -2 : self.mo.reset_stride])
         # self.dc = np.append(self.dc, self.d[0 : -2 : self.mo.reset_stride])
         self.cc = np.append(self.cc, self.c[0 : -2 : self.mo.reset_stride])
 
@@ -1271,37 +1189,42 @@
         self.m[0] = self.m[-2]
         self.l[0] = self.l[-2]
         # self.h[0] = self.h[-2]
         # self.d[0] = self.d[-2]
         self.c[0] = self.c[-2]
 
     def __merge_temp_results__(self) -> None:
-        """Once all iterations are done, replace the data fields
-        with the saved values
-
+        """Once all iterations are done, replace the data fields with
+        the saved values
         """
 
         self.m = self.mc
         self.c = self.cc
         # self.d = self.dc
 
     def __read_state__(self, directory: str) -> None:
         """read data from csv-file into a dataframe
 
         The CSV file must have the following columns
 
-        Model Time     t
-        Reservoir_Name m
-        Reservoir_Name l
-        Reservoir_Name h
-        Reservoir_Name d
-        Reservoir_Name c
-        Flux_name m
-        Flux_name l etc etc.
+            - Model Time t
 
+            - Reservoir_Name m
+
+            - Reservoir_Name l
+
+            - Reservoir_Name h
+
+            - Reservoir_Name d
+
+            - Reservoir_Name c
+
+            - Flux_name m
+
+            - Flux_name l etc etc.
         """
 
         from .utility_functions import is_name_in_list, get_object_from_list
 
         read: set = set()
         curr: set = set()
 
@@ -1318,17 +1241,17 @@
 
         if not os.path.exists(fn):
             raise FileNotFoundError(
                 f"Flux {fn} does not exist in Reservoir {self.full_name}"
             )
 
         # get a set of all current fluxes
-        for f in self.lof:
-            curr.add(f.full_name)
-            logging.debug(f"    Adding Flux {f.full_name} to list of fluxes to read")
+        # for f in self.lof:
+        #     curr.add(f.full_name)
+        #     logging.debug(f"    Adding Flux {f.full_name} to list of fluxes to read")
 
         self.df: pd.DataFrame = pd.read_csv(fn)
         self.headers: list = list(self.df.columns.values)
         df = self.df
         headers = self.headers
 
         # the headers contain the object name for each data in the
@@ -1346,76 +1269,75 @@
         for n in header_list:
             name = n.split(" ")[0]
             logging.debug(f"Looking for {name}")
             # this finds the reservoir name
             if name == self.full_name:
                 logging.debug(f"found reservoir data for {name}")
                 col = self.__assign_reservoir_data__(self, df, col, True)
-            # this loops over all fluxes in a reservoir
-            elif is_name_in_list(name, self.lof):
-                logging.debug(f"{name} is in {self.full_name}.lof")
-                obj = get_object_from_list(name, self.lof)
-                logging.debug(
-                    f"found object {obj.full_name} adding flux data for {name}"
-                )
-                read.add(obj.full_name)
-                col = self.__assign_flux_data__(obj, df, col, False)
-                i += 1
             else:
                 raise ValueError(f"Unable to find Flux {n} in {self.full_name}")
 
         # test if we missed any fluxes
         for f in list(curr.difference(read)):
             print(f"\n Warning: Did not find values for {f}\n in saved state")
 
     def __assign_flux_data__(
         self, obj: any, df: pd.DataFrame, col: int, res: bool
     ) -> int:
-        """
-        Assign the third last entry data to all values in flux
-
-        parameters: df = dataframe
-                    col = column number
-                    res = true if reservoir
+        """Assign the third last entry data to all values in flux
 
+        :param obj: # Flux
+        :param df: pd.dataframe
+        :param col: int # index into column position
+        :param res: bool = False # indicates whether obj is reservoir
+        :returns: int # index into last column
         """
 
         obj.fa[0] = df.iloc[0, col]
-        obj.fa[1] = df.iloc[0, col + 1]
-        # obj.fa[2] = df.iloc[0, col + 2]
-        # obj.fa[3] = df.iloc[0, col + 3]
-        col = col + 2
+
+        if obj.isotopes:
+            obj.fa[1] = df.iloc[0, col + 1]
+            # obj.fa[2] = df.iloc[0, col + 2]
+            col += 1
+        else:
+            col += 1
 
         return col
 
     def __assign_reservoir_data__(
         self, obj: any, df: pd.DataFrame, col: int, res: bool
     ) -> int:
-        """
-        Assign the third last entry data to all values in reservoir
-
-        parameters: df = dataframe
-                    col = column number
-                    res = true if reservoir
+        """Assign the third last entry data to all values in reservoir
 
-        """
-
-        obj.m[:] = df.iloc[-3, col]
-        obj.l[:] = df.iloc[-3, col + 1]
-        # obj.h[:] = df.iloc[-3, col + 2]
-        # obj.d[:] = df.iloc[-3, col + 3]
-        obj.c[:] = df.iloc[-3, col + 2]
-        col = col + 3
+        :param obj: # Reservoir
+        :param df: pd.dataframe
+        :param col: int # index into column position
+        :param res: True # indicates whether obj is reservoir
+
+        :returns: int # index into last column
+        """
+
+        # this may need fixing
+        if obj.isotopes:
+            obj.m[:] = df.iloc[-1, col]
+            obj.l[:] = df.iloc[-1, col + 1]
+            obj.c[:] = df.iloc[-1, col + 2]
+            col += 2
+        else:
+            obj.m[:] = df.iloc[-1, col]
+            obj.c[:] = df.iloc[-1, col + 1]
+            col += 1
 
         return col
 
     def __plot__(self, M: Model, ax) -> None:
-        """Plot instructions.
-        M: Model
-        ax: matplotlib axes handle
+        """Plot Model data
+
+        :param M: Model
+        :param ax: # graph axes handle
         """
 
         from esbmtk import set_y_limits
 
         # convert time and data to display units
         x = (M.time * M.t_unit).to(M.d_unit).magnitude
 
@@ -1438,22 +1360,17 @@
 
         # plot first axis
         ax.plot(x[1:-2], y1[1:-2], color="C0", label=y1_label)
         ax.set_xlabel(f"{M.time_label} [{M.d_unit:~P}]")
         ax.set_ylabel(f"{self.legend_left} [{M.c_unit:~P}]")
 
         # add any external data if present
-        for (
-            i,
-            d,
-        ) in enumerate(self.led):
-            time = (d.x * M.t_unit).to(M.d_unit).magnitude
-            yd = d.y.to(self.plt_units).magnitude
+        for (i, d) in enumerate(self.led):
             leg = f"{self.lm} {d.legend}"
-            ax.scatter(time[1:-2], yd[1:-2], color=f"C{i+1}", label=leg)
+            ax.scatter(d.x[1:-2], d.y[1:-2], color=f"C{i+2}", label=leg)
 
         ax.spines["top"].set_visible(False)
         handler1, label1 = ax.get_legend_handles_labels()
 
         if self.isotopes:
             axt = ax.twinx()
             y2 = self.d  # no conversion for isotopes
@@ -1469,26 +1386,23 @@
         else:
             ax.legend(handler1, label1)
             ax.spines["right"].set_visible(False)
             ax.yaxis.set_ticks_position("left")
             ax.xaxis.set_ticks_position("bottom")
 
     def info(self, **kwargs) -> None:
-        """Show an overview of the object properties.
-        Optional arguments are
-        index  :int = 0 this will show data at the given index
-        indent :int = 0 indentation
+        """Show an overview of the object properties.  Optional
+        arguments are
 
+        :param index: int = 0 # this will show data at the given index
+        :param indent: int = 0 # print indentation
         """
-        off: str = "  "
-        if "index" not in kwargs:
-            index = 0
-        else:
-            index = kwargs["index"]
 
+        off: str = "  "
+        index = 0 if "index" not in kwargs else kwargs["index"]
         if "indent" not in kwargs:
             indent = 0
             ind = ""
         else:
             indent = kwargs["indent"]
             ind = " " * indent
 
@@ -1511,101 +1425,152 @@
         print("Use the info method on any of the above connections")
         print("to see information on fluxes and processes")
 
 
 class Reservoir(ReservoirBase):
     """This object holds reservoir specific information.
 
-          Example::
+    Example::
+
+        Reservoir(name = "foo",      # Name of reservoir
+                  species = S,          # Species handle
+                  delta = 20,           # initial delta - optional (defaults  to 0)
+                  mass/concentration = "1 unit"  # species concentration or mass
+                  volume/geometry = "1E5 l",      # reservoir volume (m^3)
+                  plot = "yes"/"no", defaults to yes
+                  plot_transform_c = a function reference, optional (see below)
+                  legend_left = str, optional, useful for plot transform
+                  display_precision = number, optional, inherited from Model
+                  register = optional, use to register with Reservoir Group
+                  isotopes = True/False otherwise use Model.m_type
+                  seawater_parameters= dict, optional
+                  )
+
+    You must either give mass or concentration.  The result will
+    always be displayed as concentration though.
+
+    You must provide either the volume or the geometry keyword.  In
+    the latter case provide a list where the first entry is the upper
+    depth datum, the second entry is the lower depth datum, and the
+    third entry is the area percentage.  E.g., to specify the upper
+    200 meters of the entire ocean, you would write:
+
+    geometry=[0,-200,1]
+
+    the corresponding ocean volume will then be calculated by the
+    calc_volume method in this case the following instance variables
+    will also be set:
+
+    self.volume in model units (usually liter) self.are:a surface area
+    in m^2 at the upper bounding surface self.area_dz: area of
+    seafloor which is intercepted by this box.  self.area_fraction:
+    area of seafloor which is intercepted by this relative to the
+    total ocean floor area
+
+    Adding seawater_properties: ~~~~~~~~~~~~~~~~~~~~~~~~~~~ If this
+    optional parameter is specified, a SeaWaterConstants instance will
+    be registered for this Reservoir as Reservoir.swc See the
+    SeaWaterConstants class for details how to specify the parameters,
+    e.g.: seawater_parameters = {"temperature": 2, "pressure": 240,
+    "salinity" : 35},
 
-                  Reservoir(name = "foo",      # Name of reservoir
-                            species = S,          # Species handle
-                            delta = 20,           # initial delta - optional (defaults  to 0)
-                            mass/concentration = "1 unit"  # species concentration or mass
-                            volume/geometry = "1E5 l",      # reservoir volume (m^3)
-                            plot = "yes"/"no", defaults to yes
-                            plot_transform_c = a function reference, optional (see below)
-                            legend_left = str, optional, useful for plot transform
-                            display_precision = number, optional, inherited from Model
-                            register = optional, use to register with Reservoir Group
-                            isotopes = True/False otherwise use Model.m_type
-                            seawater_parameters= dict, optional
-                            )
-
-          You must either give mass or concentration.  The result will always be displayed
-          as concentration though.
-
-          You must provide either the volume or the geometry keyword. In the latter case
-          provide a list where the first entry is the upper depth datum, the second entry is
-          the lower depth datum, and the third entry is the area percentage. E.g., to specify
-          the upper 200 meters of the entire ocean, you would write:
-
-                 geometry=[0,-200,1]
-
-          the corresponding ocean volume will then be calculated by the calc_volume method
-          in this case the following instance variables will also be set:
-
-                 self.volume in model units (usually liter)
-                 self.are:a surface area in m^2 at the upper bounding surface
-                 self.area_dz: area of seafloor which is intercepted by this box.
-                 self.area_fraction: area of seafloor which is intercepted by this
-                                    relative to the total ocean floor area
-
-          Adding seawater_properties:
-          ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-          If this optional parameter is specified, a SeaWaterConstants instance will be registered
-          for this Reservoir as Reservoir.swc
-          See the  SeaWaterConstants class for details how to specify the parameters, e.g.:
-          seawater_parameters = {"temperature": 2, "pressure": 240, "salinity" : 35},
-
-          Using a transform function
-          ~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-          In some cases, it is useful to transform the reservoir
-          concentration data before plotting it.  A good example is the H+
-          concentration in water which is better displayed as pH.  We can
-          do this by specifying a function to convert the reservoir
-          concentration into pH units::
-
-              def phc(c :float) -> float:
-                  # Calculate concentration as pH. c can be a number or numpy array
-
-                  import numpy as np
-
-                  pH :float = -np.log10(c)
-                  return pH
-
-          this function can then be added to a reservoir as::
-
-          hplus.plot_transform_c = phc
-
-          You can modify the left legend to suit the transform via the legend_left keyword
-
-          Note, at present the plot_transform_c function will only take one
-          argument, which always defaults to the reservoir
-          concentration. The function must return a single argument which
-          will be interpreted as the transformed reservoir concentration.
+    Using a transform function ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-    Accesing Reservoir Data:
-    ~~~~~~~~~~~~~~~~~~~~~~~~
+    In some cases, it is useful to transform the reservoir
+    concentration data before plotting it.  A good example is the H+
+    concentration in water which is better displayed as pH.  We can do
+    this by specifying a function to convert the reservoir
+    concentration into pH units::
+
+        def phc(c :float) -> float:
+            # Calculate concentration as pH. c can be a number or numpy array
+
+            import numpy as np
+
+            pH :float = -np.log10(c)
+            return pH
+
+    this function can then be added to a reservoir as::
+
+
+    hplus.plot_transform_c = phc
+
+    You can modify the left legend to suit the transform via the
+    legend_left keyword
+
+    Note, at present the plot_transform_c function will only take one
+    argument, which always defaults to the reservoir concentration.
+    The function must return a single argument which will be
+    interpreted as the transformed reservoir concentration.
+
+    Accesing Reservoir Data: ~~~~~~~~~~~~~~~~~~~~~~~~
 
     You can access the reservoir data as:
 
-    - Name.m # mass
-    - Name.d # delta
-    - Name.c # concentration
+        - Name.m # mass
+
+        - Name.d # delta
+
+        - Name.c # concentration
 
     Useful methods include:
 
-    - Name.write_data() # save data to file
-    - Name.info()   # info Reservoir
+        - Name.write_data() # save data to file
+
+        - Name.info() # info Reservoir
     """
 
     def __init__(self, **kwargs) -> None:
-        """Initialize a reservoir."""
+        """Initialize a reservoir
+
+        Defaults::
+
+            self.defaults: dict[str, list[any, tuple]] = {
+              "name": ["None", (str)],
+              "species": ["None", (str, Species)],
+              "delta": ["None", (int, float, str)],
+              "concentration": ["None", (str, Q_, float)],
+              "mass": ["None", (str, Q_)],
+              "volume": ["None", (str, Q_)],
+              "geometry": ["None", (list, str)],
+              "plot_transform_c": ["None", (any)],
+              "legend_left": ["None", (str)],
+              "plot": ["yes", (str)],
+              "groupname": ["None", (str)],
+              "rtype": ["regular", (str)],
+              "function": ["None", (str, col.Callable)],
+              "display_precision": [0.01, (int, float)],
+              "register": [
+                  "None",
+                  (SourceGroup, SinkGroup, ReservoirGroup, ConnectionGroup, Model, str),
+              ],
+              "parent": [
+                  "None",
+                  (SourceGroup, SinkGroup, ReservoirGroup, ConnectionGroup, Model, str),
+              ],
+              "full_name": ["None", (str)],
+              "seawater_parameters": ["None", (dict, str)],
+              "isotopes": [False, (bool)],
+              "ideal_water": ["None", (str, bool)],
+              "has_cs1": [False, (bool)],
+              "has_cs2": [False, (bool)],
+
+        }
+
+        Required Keywords::
+
+            self.lrk: list = [
+              "name",
+              "species",
+              "register",
+              ["volume", "geometry"],
+              ["mass", "concentration"],
+
+        ]
+        """
 
         from esbmtk import (
             SourceGroup,
             SinkGroup,
             ReservoirGroup,
             ConnectionGroup,
             SeawaterConstants,
@@ -1622,15 +1587,15 @@
             "volume": ["None", (str, Q_)],
             "geometry": ["None", (list, str)],
             "plot_transform_c": ["None", (any)],
             "legend_left": ["None", (str)],
             "plot": ["yes", (str)],
             "groupname": ["None", (str)],
             "rtype": ["regular", (str)],
-            "function": ["None", (str, col.Callable)],
+            "function": ["None", (str, callable)],
             "display_precision": [0.01, (int, float)],
             "register": [
                 "None",
                 (SourceGroup, SinkGroup, ReservoirGroup, ConnectionGroup, Model, str),
             ],
             "parent": [
                 "None",
@@ -1644,46 +1609,44 @@
             "has_cs2": [False, (bool)],
         }
 
         # provide a list of absolutely required keywords
         self.lrk: list = [
             "name",
             "species",
-            "register",
             ["volume", "geometry"],
             ["mass", "concentration"],
         ]
 
-        # steps = kwargs["species"].mo.steps
-        # self.m: np.ndarray =np.zeros(steps) + self.mass
-
         self.__initialize_keyword_variables__(kwargs)
 
+        if self.register == "None":  # use a sensible default
+            self.register = self.species.element.register
         self.model = self.register
         self.parent = self.register
 
         self.__set_legacy_names__(kwargs)
 
         # geoemtry information
         if self.volume == "None":
             get_box_geometry_parameters(self)
 
         # convert units
         self.volume: tp.Union[int, float] = Q_(self.volume).to(self.mo.v_unit).magnitude
+        self.c_unit = self.model.c_unit
 
         # This should probably be species specific?
         self.mu: str = self.sp.e.mass_unit  # massunit xxxx
 
         self.ideal_water = self.mo.ideal_water
         if self.ideal_water:
             self.density = 1000
         else:
             if isinstance(self.parent, ReservoirGroup):
                 self.swc = self.parent.swc
-                self.density = self.swc.density
             else:
                 if isinstance(self.seawater_parameters, str):
                     temperature = 25
                     salinity = 35
                     pressure = 1
                 else:
                     if "temperature" in self.seawater_parameters:
@@ -1702,32 +1665,31 @@
                 SeawaterConstants(
                     name="swc",
                     temperature=temperature,
                     pressure=pressure,
                     salinity=salinity,
                     register=self,
                 )
-                self.density = self.swc.density
-
+            self.density = self.swc.density
         if self.mass == "None":
             if isinstance(self.concentration, (str, Q_)):
-                c = Q_(self.concentration)
-                self.plt_units = c.units
-                self._concentration: tp.Union[int, float] = c.to(
-                    self.mo.c_unit
-                ).magnitude
+                cc = Q_(self.concentration)
+                self.plt_units = cc.units
+                self._concentration: [int | float] = cc.to(self.mo.c_unit).magnitude
+                
             else:
-                c = self.concentration
+                cc = self.concentration
                 self.plt_units = self.mo.c_unit
-                self._concentration = c
+                self._concentration = cc
 
             self.mass: tp.Union[int, float] = (
                 self.concentration * self.volume * self.density / 1000
             )
             self.display_as = "concentration"
+            
         elif self.concentration == "None":
             m = Q_(self.mass)
             self.plt_units = self.mo.m_unit
             self.mass: tp.Union[int, float] = m.to(self.mo.m_unit).magnitude
             self.concentration = self.mass / self.volume
             self.display_as = "mass"
         else:
@@ -1741,15 +1703,15 @@
 
         # initialize mass vector
         self.m: np.ndarray = np.zeros(self.species.mo.steps) + self.mass
         self.l: np.ndarray = np.zeros(self.mo.steps)
         self.v: np.ndarray = np.zeros(self.mo.steps) + self.volume  # reservoir volume
 
         if self.delta != "None":
-            self.l = get_l_mass(self.m, self.delta, self.species.r)
+            self.l = get_l_mass(self.c, self.delta, self.species.r)
 
         # create temporary memory if we use multiple solver iterations
         if self.mo.number_of_solving_iterations > 0:
             self.mc = np.empty(0)
             self.cc = np.empty(0)
             self.dc = np.empty(0)
 
@@ -1793,51 +1755,83 @@
             self.m = self.m * 0 + self.mass
 
     @delta.setter
     def delta(self, d: float) -> None:
         if self.update and d != "None":
             self._delta: float = d
             self.isotopes = True
-            self.l = get_l_mass(self.m, d, self.species.r)
+            self.l = get_l_mass(self.c, d, self.species.r)
 
     @mass.setter
     def mass(self, m: float) -> None:
         if self.update and m != "None":
             self._mass: float = m
             self.m = np.zeros(self.species.mo.steps) + m
             self.c = self.m / self.volume
 
 
 class Flux(esbmtkBase):
-    """A class which defines a flux object. Flux objects contain
+    """A class which defines a flux object.  Flux objects contain
     information which links them to an species, describe things like
     the mass and time unit, and store data of the total flux rate at
-    any given time step. Similarly, they store the flux of the light
-    and heavy isotope flux, as well as the delta of the flux. This
-    is typically handled through the Connect object. If you set it up manually
-
-    Flux = (name = "Name" # optional, defaults to _F
-            species = species_handle,
-            delta = any number,
-            rate  = "12 mol/s" # must be a string
-            display_precision = number, optional, inherited from Model
+    any given time step.  Similarly, they store the flux of the light
+    and heavy isotope flux, as well as the delta of the flux.  This is
+    typically handled through the Connect object.  If you set it up
+    manually
+
+    Example::
+
+        Flux = (name = "Name" # optional, defaults to _F
+             species = species_handle,
+             delta = any number,
+             rate  = "12 mol/s" # must be a string
+             display_precision = number, optional, inherited from Model
+
     )
 
-     You can access the flux data as
-    - Name.m # mass
-    - Name.d # delta
-    - Name.c # concentration
+    You can access the flux data as
 
+        - Name.m # mass
+        - Name.d # delta
+        - Name.c # same as Name.m since flux has no concentration
     """
 
     def __init__(self, **kwargs: dict[str, any]) -> None:
         """
-        Initialize a flux. Arguments are the species name the flux rate
-        (mol/year), the delta value and unit
+        Initialize a flux.  Arguments are the species name the flux
+        rate (mol/year), the delta value and unit
+
+        Defaults::
 
+            self.defaults: dict[str, list[any, tuple]] = {
+              "name": ["None", (str)],
+              "species": ["None", (str, Species)],
+              "delta": [0, (str, int, float)],
+              "rate": ["None", (str, Q_, int, float)],
+              "plot": ["yes", (str)],
+              "display_precision": [0.01, (int, float)],
+              "isotopes": [False, (bool)],
+              "register": [
+                  "None",
+                  (
+                      str,
+                      Reservoir,
+                      GasReservoir,
+                      Connection,
+                      Connect,
+                      AirSeaExchange,
+                      Signal,
+                  ),
+              ],
+              "save_flux_data": [False, (bool)],
+              "id": ["None", (str)],
+
+        }
+
+        Required Keywords: "species", "rate", "register"
         """
 
         from esbmtk import (
             Q_,
             AirSeaExchange,
             Reservoir,
             GasReservoir,
@@ -1893,39 +1887,37 @@
 
         # model units
         self.plt_units = Q_(self.rate).units
         self.mu: str = f"{self.species.mu}/{self.mo.tu}"
 
         # and convert flux into model units
         if isinstance(self.rate, str):
-            fluxrate: float = Q_(self.rate).to(self.mo.f_unit).magnitude
+            self.rate: float = Q_(self.rate).to(self.mo.f_unit).magnitude
         elif isinstance(self.rate, Q_):
-            fluxrate: float = self.rate.to(self.mo.f_unit).magnitude
+            self.rate: float = self.rate.to(self.mo.f_unit).magnitude
         elif isinstance(self.rate, (int, float)):
-            fluxrate: float = self.rate
+            self.rate: float = self.rate
 
-        if self.delta:
-            li = get_l_mass(fluxrate, self.delta, self.sp.r)
-        else:
-            li = 0
-        self.fa: np.ndarray = np.array([fluxrate, li])
+        li = get_l_mass(self.rate, self.delta, self.sp.r) if self.delta else 0
+        self.fa: np.ndarray = np.array([self.rate, li])
 
         # in case we want to keep the flux data
         if self.save_flux_data:
-            self.m: np.ndarray = np.zeros(self.model.steps) + fluxrate  # add the flux
-            self.l: np.ndarray = np.zeros(self.model.steps)
+            self.m: np.ndarray = np.zeros(self.model.steps) + self.rate  # add the flux
+
+            if self.isotopes:
+                self.l: np.ndarray = np.zeros(self.model.steps)
+                if self.rate != 0:
+                    self.l = get_l_mass(self.m, self.delta, self.species.r)
+                    self.fa[1] = self.l[0]
 
             if self.mo.number_of_solving_iterations > 0:
                 self.mc = np.empty(0)
                 self.dc = np.empty(0)
 
-            if self.rate != 0:
-                self.l = get_l_mass(self.m, self.delta, self.species.r)
-                self.fa[1] = self.l[0]
-
         else:
             # setup dummy variables to keep existing numba data structures
             self.m = np.zeros(2)
             self.l = np.zeros(2)
 
             if self.rate != 0:
                 self.fa[1] = get_l_mass(self.fa[0], self.delta, self.species.r)
@@ -1969,94 +1961,106 @@
             # self.__get_data__ = self.__get_without_isotopes__
 
     # setup a placeholder setitem function
     def __setitem__(self, i: int, value: np.ndarray):
         return self.__set_data__(i, value)
 
     def __getitem__(self, i: int) -> np.ndarray:
-        """Get data by index"""
+        """
+        Get data by index
+        """
         # return self.__get_data__(i)
         return self.fa
 
     def __set_with_isotopes__(self, i: int, value: np.ndarray) -> None:
-        """Write data by index"""
+        """
+        Write data by index
+        """
 
         self.m[i] = value[0]
         self.l[i] = value[1]
-        self.fa = value[0:4]
+        self.fa = value[:4]
 
     def __set_without_isotopes__(self, i: int, value: np.ndarray) -> None:
-        """Write data by index"""
+        """
+        Write data by index
+        """
 
         self.fa = [value[0], 0]
         self.m[i] = value[0]
 
     def __call__(self) -> None:  # what to do when called as a function ()
         pass
         return
 
     def __add__(self, other):
-        """adding two fluxes works for the masses, but not for delta"""
+        """
+        adding two fluxes works for the masses, but not for delta
+        """
 
         self.fa = self.fa + other.fa
         self.m = self.m + other.m
         self.l = self.l + other.l
 
     def __sub__(self, other):
-        """substracting two fluxes works for the masses, but not for delta"""
+        """
+        substracting two fluxes works for the masses, but not for
+        delta
+        """
 
         self.fa = self.fa - other.fa
         self.m = self.m - other.m
         self.l = self.l - other.l
 
     def info(self, **kwargs) -> None:
-        """Show an overview of the object properties.
-        Optional arguments are
-        index  :int = 0 this will show data at the given index
-        indent :int = 0 indentation
+        """Show an overview of the object properties.  Optional
+        arguments are:
 
+        :param index: int = 0 this will show data at the given index
+        :param indent: int = 0 indentation
         """
-        off: str = "  "
-        if "index" not in kwargs:
-            index = 0
-        else:
-            index = kwargs["index"]
-
+        index = 0 if "index" not in kwargs else kwargs["index"]
         if "indent" not in kwargs:
             indent = 0
             ind = ""
         else:
             indent = kwargs["indent"]
             ind = " " * indent
 
         # print basic data bout this object
         print(f"{ind}{self.__str__(kwargs)}")
         print(f"{ind}Data sample:")
         show_data(self, index=index, indent=indent)
 
         if len(self.lop) > 0:
-            print(f"\n{ind}Process(es) acting on this flux:")
-            for p in self.lop:
-                print(f"{off}{ind}{p.__repr__()}")
-
-            print("")
-            print(
-                "Use help on the process name to get an explanation what this process does"
-            )
-            if self.register == "None":
-                print(f"e.g., help({self.lop[0].n})")
-            else:
-                print(f"e.g., help({self.register.name}.{self.lop[0].name})")
+            self._extracted_from_info_27(ind)
         else:
             print("There are no processes for this flux")
 
+    # TODO Rename this here and in `info`
+    def _extracted_from_info_27(self, ind):
+        print(f"\n{ind}Process(es) acting on this flux:")
+        off: str = "  "
+        for p in self.lop:
+            print(f"{off}{ind}{p.__repr__()}")
+
+        print("")
+        print(
+            "Use help on the process name to get an explanation what this process does"
+        )
+        if self.register == "None":
+            print(f"e.g., help({self.lop[0].n})")
+        else:
+            print(f"e.g., help({self.register.name}.{self.lop[0].name})")
+
     def __plot__(self, M: Model, ax) -> None:
         """Plot instructions.
-        M: Model
-        ax: matplotlib axes handle
+
+        :param M: Model
+        :param ax: matplotlib axes handle
         """
 
         from esbmtk import set_y_limits
 
         # convert time and data to display units
         x = (M.time * M.t_unit).to(M.d_unit).magnitude
         y1 = (self.m * M.m_unit).to(self.plt_units).magnitude
@@ -2091,62 +2095,84 @@
         else:
             ax.legend(handler1, label1)
             ax.spines["right"].set_visible(False)
             ax.yaxis.set_ticks_position("left")
             ax.xaxis.set_ticks_position("bottom")
 
     def __sub_sample_data__(self, stride) -> None:
-        """There is usually no need to keep more than a thousand data points
-        so we subsample the results before saving, or processing them
-
+        """There is usually no need to keep more than a thousand data
+        points so we subsample the results before saving, or
+        processing them
         """
 
         if self.save_flux_data:
             self.m = self.m[2:-2:stride]
             self.l = self.m[2:-2:stride]
 
     def __reset_state__(self) -> None:
-        """Copy the result of the last computation back to the beginning
-        so that a new run will start with these values.
+        """Copy the result of the last computation back to the
+        beginning so that a new run will start with these values.
 
         Also, copy current results into temp field
         """
 
         if self.save_flux_data:
             self.mc = np.append(self.mc, self.m[0 : -2 : self.mo.reset_stride])
             # copy last element to first position
             self.m[0] = self.m[-2]
             self.l[0] = self.l[-2]
 
     def __merge_temp_results__(self) -> None:
-        """Once all iterations are done, replace the data fields
-        with the saved values
-
+        """Once all iterations are done, replace the data fields with
+        the saved values
         """
 
         self.m = self.mc
 
 
 class SourceSink(esbmtkBase):
     """
-    This is a meta class to setup a Source/Sink objects. These are not
-    actual reservoirs, but we stil need to have them as objects
+    This is a meta class to setup a Source/Sink objects.  These are
+    not actual reservoirs, but we stil need to have them as objects
     Example::
 
-           Sink(name = "Pyrite",
-               species = SO4,
-               display_precision = number, optional, inherited from Model
-               delta = number or str. optional defaults to "None"
-           )
-
-    where the first argument is a string, and the second is a reservoir handle
+        Sink(name = "Pyrite",
+            species = SO4,
+            display_precision = number, optional, inherited from Model
+            delta = number or str. optional defaults to "None"
+        )
 
+    where the first argument is a string, and the second is a
+    reservoir handle
     """
 
     def __init__(self, **kwargs) -> None:
+        """
+        Defaults::
+
+            self.defaults: dict[str, list[any, tuple]] = {
+               "name": ["None", (str)],
+               "species": ["None", (str, Species)],
+               "display_precision": [0.01, (int, float)],
+               "register": [
+                   "None",
+                   (
+                       SourceGroup,
+                       SinkGroup,
+                       ReservoirGroup,
+                       ConnectionGroup,
+                       Model,
+                       str,
+                   ),
+               ],
+               "delta": ["None", (str, int, float)],
+               "isotopes": [False, (bool)],
+
+        Required Keywords: "name", "species"
+        """
 
         from esbmtk import (
             SourceGroup,
             SinkGroup,
             ReservoirGroup,
             ConnectionGroup,
         )
@@ -2166,39 +2192,43 @@
                     str,
                 ),
             ],
             "delta": ["None", (str, int, float)],
             "isotopes": [False, (bool)],
         }
         # provide a list of absolutely required keywords
-        self.lrk: list[str] = ["name", "species", "register"]
+        self.lrk: list[str] = ["name", "species"]
         self.__initialize_keyword_variables__(kwargs)
 
+        if self.register == "None":  # use a sensible default
+            self.register = self.species.element.register
+
         self.loc: set[Connection] = set()  # set of connection objects
 
         # legacy names
         # if self.register != "None":
         #    self.full_name = f"{self.name}.{self.register.name}"
         self.parent = self.register
         self.n = self.name
         self.sp = self.species
         self.mo = self.species.mo
         self.model = self.species.mo
         self.u = self.species.mu + "/" + str(self.species.mo.bu)
         self.lio: list = []
+        self.m = 1  # set default mass and concentration values
+        self.c = 1
         self.mo.lic.append(self)  # add source to list of res type objects
 
         if self.mo.register == "local" and self.register == "None":
             self.register = self.mo
+        elif self.register == "None":
+            self.pt = self.name
         else:
-            if self.register == "None":
-                self.pt = self.name
-            else:
-                self.pt: str = f"{self.register.name}_{self.n}"
-                self.groupname = self.register.name
+            self.pt: str = f"{self.register.name}_{self.n}"
+            self.groupname = self.register.name
 
         if self.display_precision == 0:
             self.display_precision = self.mo.display_precision
 
         self.__register_name_new__()
         self.mo.lic.remove(self)
 
@@ -2209,40 +2239,33 @@
     @delta.setter
     def delta(self, d):
         """Set/Update delta"""
         if d != "None":
             self._delta = d
             self.isotopes = True
             self.m = 1
-            self.l = get_l_mass(self.m, d, self.species.r)
-            self.c = self.l / (self.m - self.l)
+            self.c = 1
+            self.l = get_l_mass(self.c, d, self.species.r)
+            # self.c = self.l / (self.m - self.l)
             # self.provided_kwargs.update({"delta": d})
 
 
 class Sink(SourceSink):
     """
-    This is just a wrapper to setup a Sink object
-    Example::
+    This is just a wrapper to setup a Sink object Example::
 
-           Sink(name = "Pyrite",species =SO4)
+        Sink(name = "Pyrite",species =SO4)
 
-    where the first argument is a string, and the second is a species handle
+    where the first argument is a string, and the second is a species
+    handle
     """
 
 
 class Source(SourceSink):
     """
-    This is just a wrapper to setup a Source object
-    Example::
+    This is just a wrapper to setup a Source object Example::
 
-           Source(name = "SO4_diffusion", species ="SO4")
+        Source(name = "SO4_diffusion", species ="SO4")
 
-    where the first argument is a string, and the second is a species handle
+    where the first argument is a string, and the second is a species
+    handle
     """
-
-
-# from .extended_classes import *
-# from .connections import Connection, ConnectionGroup, Connect
-# from .processes import *
-# from .carbonate_chemistry import *
-# from .sealevel import *
-# from .solver import *
```

### Comparing `esbmtk-0.8.0.0/esbmtk/esbmtk_base.py` & `esbmtk-0.9.0.1/esbmtk/esbmtk_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,36 +58,32 @@
 
     def __check_mandatory_keywords__(self, lrk: list, kwargs: dict) -> None:
         """Verify that all elements of lrk have a corresponding key in
         kwargs.  If not, print error message"""
 
         for key in lrk:
             if isinstance(key, list):
-                has_key = 0
-                for k in key:
-                    if k in kwargs and kwargs[k] != "None":
-                        has_key += 1
+                has_key = sum(k in kwargs and kwargs[k] != "None" for k in key)
                 if has_key != 1:
                     raise ValueError(f"give only one of {key}")
-            else:
-                if key not in kwargs:
-                    raise ValueError(f"{key} is a mandatory keyword")
+            elif key not in kwargs:
+                raise ValueError(f"{key} is a mandatory keyword")
 
     def __register_variable_names__(
         self,
         defaults: dict[str, list[any, tuple]],
         kwargs: dict,
     ) -> None:
         """Register the key value[0] pairs as local instance variables.
         We register them with their actual variable name and as _variable_name
         in case we use setter and getter methods.
         to avoid name conflicts.
         """
         for key, value in defaults.items():
-            setattr(self, "_" + key, value[0])
+            setattr(self, f"_{key}", value[0])
             setattr(self, key, value[0])
 
         # save kwargs dict
         self.kwargs: dict = kwargs
 
     def __update_dict_entries__(
         self,
@@ -112,40 +108,49 @@
             if not isinstance(value, defaults[key][1]):
                 raise TypeError(
                     f"{value} for {key} must be of type {defaults[key][1]}, not {type(value)}"
                 )
 
             defaults[key][0] = value  # update defaults dictionary
             setattr(self, key, value)  # update instance variables
-            setattr(self, "_" + key, value)  # and their property shadows
+            setattr(self, f"_{key}", value)
 
     def __register_name_new__(self) -> None:
         """if self.parent is set, register self as attribute of self.parent,
         and set full name to parent.full-name + self.name
         if self.parent == "None", full_name = name
         """
 
         if self.parent == "None":
             self.full_name = self.name
             reg = self
         else:
-            self.full_name = self.parent.full_name + "." + self.name
+            self.full_name = f"{self.parent.full_name}.{self.name}"
             reg = self.parent.model
-            # check for naming conflicts
+            # self.full_name, reg.lmo = self.__test_and_resolve_duplicates__(self.full_name, reg.lmo)
             if self.full_name in reg.lmo:
                 raise NameError(f"{self.full_name} is a duplicate name in reg.lmo")
-            else:
-                # register with model
-                reg.lmo.append(self.full_name)
-                reg.lmo2.append(self)
-                reg.dmo.update({self.full_name: self})
-                setattr(self.parent, self.name, self)
-                self.kwargs["full_name"] = self.full_name
+            # register with model
+            reg.lmo.append(self.full_name)
+            reg.lmo2.append(self)
+            reg.dmo.update({self.full_name: self})
+            setattr(self.parent, self.name, self)
+            self.kwargs["full_name"] = self.full_name
         self.reg_time = time.monotonic()
 
+    def __test_and_resolve_duplicates__(self, name, lmo):
+        if name in lmo:
+            print(f"\n Warning, {name} is a duplicate, trying with {name}_1\n")
+            name = name + "_1"
+            name, lmo = self.__test_and_resolve_duplicates__(name, lmo)
+        else:
+            lmo.append(name)
+
+        return name, lmo
+
 
 class esbmtkBase(input_parsing):
     """The esbmtk base class template. This class handles keyword
     arguments, name registration and other common tasks
 
     Useful methods in this class:
 
@@ -182,71 +187,57 @@
         # do not echo input unless explicitly requestted
 
         m = f"{self.__class__.__name__}(\n"
         for k, v in self.kwargs.items():
             if not isinstance({k}, esbmtkBase):
                 # check if this is not another esbmtk object
                 if "esbmtk" in str(type(v)):
-                    m = m + f"    {k} = {v.name},\n"
-                # if this is a string
+                    m = f"{m}    {k} = {v.name},\n"
                 elif isinstance(v, str):
-                    m = m + f"    {k} = '{v}',\n"
-                # if this is a quantity
+                    m = f"{m}    {k} = '{v}',\n"
                 elif isinstance(v, Q_):
-                    m = m + f"    {k} = '{v}',\n"
-                # if this is a list
+                    m = f"{m}    {k} = '{v}',\n"
                 elif isinstance(v, (list, np.ndarray)):
-                    m = m + f"    {k} = '{v[0:3]}',\n"
-                # all other cases
+                    m = f"{m}    {k} = '{v[:3]}',\n"
                 else:
-                    m = m + f"    {k} = {v},\n"
-
-        m = m + ")"
-
-        if log == 0 and tdiff < 1:
-            m = ""
+                    m = f"{m}    {k} = {v},\n"
 
+        m = "" if log == 0 and tdiff < 1 else f"{m})"
         return m
 
-    def __str__(self, kwargs={}):
+    def __str__(self, kwargs=None):
         """Print the basic parameters for this class when called via the print method
         Optional arguments
 
         indent :int = 0 printing offset
 
         """
+        if kwargs is None:
+            kwargs = {}
         from esbmtk import Q_
 
         m: str = ""
         off: str = "  "
 
-        if "indent" in kwargs:
-            ind: str = kwargs["indent"] * " "
-        else:
-            ind: str = ""
-
-        if "index" in kwargs:
-            index = int(kwargs["index"])
-        else:
-            index = -2
-
+        ind: str = kwargs["indent"] * " " if "indent" in kwargs else ""
+        index = int(kwargs["index"]) if "index" in kwargs else -2
         m = f"{ind}{self.name} ({self.__class__.__name__})\n"
         for k, v in self.kwargs.items():
             if not isinstance({k}, esbmtkBase):
                 # check if this is not another esbmtk object
                 if "esbmtk" in str(type(v)):
                     pass
-                elif isinstance(v, str) and not (k == "name"):
-                    m = m + f"{ind}{off}{k} = {v}\n"
+                elif isinstance(v, str) and k != "name":
+                    m = f"{m}{ind}{off}{k} = {v}\n"
                 elif isinstance(v, Q_):
-                    m = m + f"{ind}{off}{k} = {v}\n"
+                    m = f"{m}{ind}{off}{k} = {v}\n"
                 elif isinstance(v, np.ndarray):
-                    m = m + f"{ind}{off}{k}[{index}] = {v[index]:.2e}\n"
+                    m = f"{m}{ind}{off}{k}[{index}] = {v[index]:.2e}\n"
                 elif k != "name":
-                    m = m + f"{ind}{off}{k} = {v}\n"
+                    m = f"{m}{ind}{off}{k} = {v}\n"
 
         return m
 
     def __lt__(self, other) -> None:
         """This is needed for sorting with sorted()"""
 
         return self.n < other.n
@@ -276,19 +267,19 @@
 
     def __aux_inits__(self) -> None:
         """Aux initialization code. Not normally used"""
 
         pass
 
     def ensure_q(self, arg):
-        """ Test that a given input argument is a quantity. If not convert
+        """Test that a given input argument is a quantity. If not convert
         into quantity
         """
         from esbmtk import Q_
-        
+
         if isinstance(arg, Q_):
             pass
         elif isinstance(arg, str):
             arg = Q_(arg)
         else:
             raise ValueError(f"{arg} must be string or Quantity, not {type(arg)}")
```

### Comparing `esbmtk-0.8.0.0/esbmtk/extended_classes.py` & `esbmtk-0.9.0.1/esbmtk/extended_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from __future__ import annotations
 from pandas import DataFrame
-from numba.typed import List
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 import logging
 import os
 import math
 import copy as cp
-import collections as col
 import typing as tp
 
 if tp.TYPE_CHECKING:
-    from esbmtk import Connection
+    from esbmtk import Connection, Model
 
 from .esbmtk_base import esbmtkBase
 from .esbmtk import ReservoirBase, Reservoir
 
 from .solver import (
     get_imass,
     get_delta,
@@ -42,16 +40,17 @@
 
         ReservoirGroup(name = "ShallowOcean",        # Name of reservoir group
                     volume/geometry = "1E5 l",       # see below
                     delta   = {DIC:0, TA:0, PO4:0]  # dict of delta values
                     mass/concentration = {DIC:"1 unit", TA: "1 unit"}
                     plot = {DIC:"yes", TA:"yes"}  defaults to yes
                     isotopes = {DIC: True/False} see Reservoir class for details
-                    seawater_parameter = dict, optional, see below
+                    seawater_parameters = dict, optional, see below
                     carbonate_system= False, see below
+                    register= model handle, required
                )
 
     Notes: - The subreservoirs are derived from the keys in the concentration or mass
              dictionary. Toward this end, the keys must be valid species handles and
              -- not species names -- !
 
     Connecting two reservoir groups requires that the names in both
@@ -103,17 +102,15 @@
         from esbmtk import (
             ExternalCode,
             Species,
             SeawaterConstants,
             Model,
             get_box_geometry_parameters,
             Q_,
-            calc_carbonates_2,
         )
-        from numba.typed import List
 
         # provide a dict of all known keywords and their type
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["None", (str)],
             "delta": ["None", (dict, str)],
             "concentration": ["None", (dict, str)],
             "mass": ["None", (str, dict)],
@@ -125,16 +122,16 @@
             "carbonate_system": [False, (bool)],
             "register": ["None", (str, Model)],
         }
 
         # provide a list of absolutely required keywords
         self.lrk: list = [
             "name",
-            ["volume", "geometry"],
             "register",
+            ["volume", "geometry"],
         ]
 
         if "concentration" in kwargs:
             self.species: list = list(kwargs["concentration"].keys())
         elif "mass" in kwargs:
             self.species: list = list(kwargs["mass"].keys())
         else:
@@ -149,22 +146,18 @@
         self.parent = self.register
         self.has_cs1 = False
         self.has_cs2 = False
 
         # geoemtry information
         if self.volume == "None":
             get_box_geometry_parameters(self)
-            # reset values, otherwise creation of Reservoir will complain
-            # about volume and geometry being defined
-            self.geometry = "None"
-        else:
-            if isinstance(self.volume, str):
-                self.volume = Q_(self.volume)
-            elif not isinstance(self.volume, Q_):
-                raise ValueError("Volume must be string or quantity")
+        elif isinstance(self.volume, str):
+            self.volume = Q_(self.volume)
+        elif not isinstance(self.volume, Q_):
+            raise ValueError("Volume must be string or quantity")
 
         # register this group object in the global namespace
         # if self.mo.register == "local" and self.register == "None":
         #     self.register = self.mo
         self.__register_name_new__()
 
         # register a seawater_parameter instance if necessary
@@ -200,20 +193,18 @@
                 "plot": "yes",
                 "isotopes": False,
             }
 
             # now we loop trough all keys for this reservoir and see
             # if we find a corresponding item in the kwargs
             for kcd, vcd in self.cd[s.name].items():  # kcd  = delta, plot, etc
-                if kcd in self.kwargs:  # found entry delta
-                    # test if delta relates to any species
-                    if s in self.kwargs[kcd]:  # {SO4: xxx}
-                        # update the entry with the value provided in kwargs
-                        # self.cd['SO4_name']['delta'] = self.kwargs['delta'][SO4]
-                        self.cd[s.name][kcd] = self.kwargs[kcd][s]
+                if kcd in self.kwargs and s in self.kwargs[kcd]:
+                    # update the entry with the value provided in kwargs
+                    # self.cd['SO4_name']['delta'] = self.kwargs['delta'][SO4]
+                    self.cd[s.name][kcd] = self.kwargs[kcd][s]
 
         self.lor: list = []  # list of reservoirs in this group.
         # loop over all entries in species and create the respective reservoirs
         for s in self.species:
             if not isinstance(s, Species):
                 raise ValueError(f"{s.n} needs to be a valid species name")
 
@@ -222,24 +213,22 @@
                 name=f"{s.name}",
                 register=self,
                 species=s,
                 delta=self.cd[s.n]["delta"],
                 mass=self.cd[s.n]["mass"],
                 concentration=self.cd[s.n]["concentration"],
                 volume=self.volume,
-                geometry=self.geometry,
+                # geometry=self.geometry,
                 plot=self.cd[s.n]["plot"],
                 groupname=self.name,
                 isotopes=self.cd[s.n]["isotopes"],
             )
             # register as part of this group
             self.lor.append(a)
 
-        # setup the carbonate system
-
         # depreceated
         if self.carbonate_system:
             # do some sanity checks:
             if not hasattr(self, "swc"):
                 raise AttributeError(
                     f"{self.full_name} has no seawaterconstants instance"
                 )
@@ -249,28 +238,28 @@
             if not hasattr(self, "TA"):
                 raise AttributeError(f"{self.full_name} has no TA reservoir")
 
             ExternalCode(
                 name="cs",
                 species=Model.CO2,
                 alias_list="H CA HCO3 CO3 CO2aq omega zsat".split(" "),
-                vr_datafields=List(
+                vr_datafields=list(
                     [
                         self.swc.hplus,
                         self.swc.ca,
                         self.swc.hco3,
                         self.swc.co3,
                         self.swc.co2,
                         0.0,  # omega
                         0.0,  # zsat
                     ]
                 ),
                 function=calc_carbonates_2,
-                function_input_data=List([self.DIC.c, self.TA.c]),
-                function_params=List(
+                function_input_data=list([self.DIC.c, self.TA.c]),
+                function_params=list(
                     [
                         self.swc.K1,  # 0
                         self.swc.K2,  # 1
                         self.swc.KW,  # 2
                         self.swc.KB,  # 3
                         self.swc.boron,  # 4
                         self.swc.hplus,  # 5
@@ -328,26 +317,14 @@
         self.parent = self.register
         self.n = self.name
         self.sp = self.species
         self.mo = self.species.mo
         self.u = self.species.mu + "/" + str(self.species.mo.bu)
         self.lio: list = []
 
-        # if self.register == "None":
-        #     self.pt = self.name
-        # else:
-        #     self.pt: str = f"{self.register.name}_{self.n}"
-        #     self.groupname = self.register.name
-
-        # if self.delta != "None":
-        #     self.isotopes = True
-
-        # if self.display_precision == 0:
-        #     self.display_precision = self.mo.display_precision
-
         self.__register_name_new__()
 
 
 class SourceSinkGroup(esbmtkBase):
     """
     This is a meta class to setup  Source/Sink Groups. These are not
     actual reservoirs, but we stil need to have them as objects
@@ -365,15 +342,15 @@
 
         from esbmtk import Model, Species, Source, Sink
 
         # provide a dict of all known keywords and their type
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["None", (str)],
             "species": ["None", (str, list)],
-            "delta": [dict(), (dict)],
+            "delta": [{}, dict],
             "register": ["None", (str, Model)],
         }
 
         # provide a list of absolutely required keywords
         self.lrk: list[str] = ["name", "species", "register"]
 
         self.__initialize_keyword_variables__(kwargs)
@@ -395,19 +372,15 @@
         self.lor: list = []  # list of sub reservoirs in this group
 
         # loop over species names and setup sub-objects
         for i, s in enumerate(self.species):
             if not isinstance(s, Species):
                 raise ValueError(f"{s.n} needs to be a valid species name")
 
-            if s in self.delta:
-                delta = self.delta[s]
-            else:
-                delta = "None"
-
+            delta = self.delta[s] if s in self.delta else "None"
             if type(self).__name__ == "SourceGroup":
                 a = Source(
                     name=f"{s.name}",
                     register=self,
                     species=s,
                     delta=delta,
                 )
@@ -547,27 +520,27 @@
             "source": ["None", (Source, Sink, Reservoir, str)],
             "legend_right": ["None", (str)],
             "register": ["None", (str, Model)],
             "isotopes": [False, (bool)],
         }
 
         # provide a list of absolutely required keywords
-        self.lrk: List[str] = [
+        self.lrk: list[str] = [
             "name",
             ["duration", "filename"],
             "species",
             ["shape", "filename"],
             ["magnitude", "mass", "filename"],
             "register",
         ]
 
         self.__initialize_keyword_variables__(kwargs)
 
         # list of signals we are based on
-        self.los: List[Signal] = []
+        self.los: list[Signal] = []
 
         # convert units to model units
         self.st: tp.Union[int, float] = int(
             Q_(self.start).to(self.species.mo.t_unit).magnitude
         )  # start time
 
         if "mass" in self.kwargs:
@@ -575,18 +548,21 @@
         elif "magnitude" in self.kwargs:
             self.magnitude = Q_(self.magnitude).to(self.species.mo.f_unit).magnitude
 
         self.duration = int(Q_(self.duration).to(self.species.mo.t_unit).magnitude)
 
         self.offset = Q_(self.offset).to(self.species.mo.t_unit).magnitude
 
-        if self.duration / self.species.mo.dt < 10:
+        if self.duration / self.species.mo.max_step < 10:
+            print("\n\n ------------------------------------------------\n")
             print("\n\n   W A R N I N G \n\n")
             print("Your signal duration is covered by less than 10")
-            print("Intergration steps. This may not be what you want\n\n")
+            print("Intergration steps. This may not be what you want")
+            print("Consider adjusting the max_step parameter of the model object\n\n")
+            print("\n\n ------------------------------------------------\n")
 
         # legacy name definitions
         self.full_name = ""
         self.l: int = self.duration
         self.n: str = self.name  # the name of the this signal
         self.sp: Species = self.species  # the species
         self.mo: Model = self.species.mo  # the model handle
@@ -599,14 +575,17 @@
         self.led: list = []
 
         if self.display_precision == 0:
             self.display_precision = self.mo.display_precision
 
         self.data = self.__init_signal_data__()
         self.m = self.data.m
+        if self.isotopes:
+            self.l = self.data.l
+
         self.data.n: str = self.name + "_data"  # update the name of the signal data
         self.legend_left = self.data.legend_left
         self.legend_right = self.data.legend_right
         # update isotope values
         # self.data.li = get_l_mass(self.data.m, self.data.d, self.sp.r)
         if self.mo.register == "local" and self.register == "None":
             self.register = self.mo
@@ -641,38 +620,39 @@
             self.__pyramid__(0, self.length)
         elif self.sh == "bell":
             self.__bell__(0, self.length)
         elif "filename" in self.kwargs:  # use an external data set
             self.length = self.__int_ext_data__()
         else:
             raise ValueError(
-                f"argument needs to be either square/pyramid, "
-                f"or an ExternalData object. "
+                "argument needs to be either square/pyramid, or an ExternalData object. "
             )
 
         # create a dummy flux we can act up
         self.nf: Flux = Flux(
             name=self.n + "_data",
             species=self.sp,
             rate=f"0 {self.sp.mo.f_unit}",
             delta=0,
+            isotopes=self.isotopes,
             save_flux_data=True,
             register=self,
         )
 
         # remove signal fluxes from global flux list
         self.mo.lof.remove(self.nf)
 
         # map into model space
         insert_start_time = self.st - self.mo.offset
         insert_stop_time = insert_start_time + self.duration
 
         dt1 = int((self.st - self.mo.offset - self.mo.start))
         dt2 = int((self.st + self.duration - self.mo.stop - self.mo.offset))
 
+        # This fails if actual model steps != dt
         model_start_index = int(max(insert_start_time / self.mo.dt, 0))
         model_stop_index = int(min((self.mo.steps + dt2 / self.mo.dt), self.mo.steps))
         signal_start_index = int(min(dt1, 0) * -1)
         signal_stop_index = int(self.length - max(0, dt2))
 
         if self.mo.debug:
             print(
@@ -686,18 +666,18 @@
                 f"signal num_steps = {signal_stop_index-signal_start_index}\n"
             )
 
         if signal_start_index < signal_stop_index:
             self.nf.m[model_start_index:model_stop_index] = self.s_m[
                 signal_start_index:signal_stop_index
             ]
-            self.nf.l[model_start_index:model_stop_index] = self.s_l[
-                signal_start_index:signal_stop_index
-            ]
-
+            if self.nf.isotopes:
+                self.nf.l[model_start_index:model_stop_index] = self.s_l[
+                    signal_start_index:signal_stop_index
+                ]
         return self.nf
 
     def __square__(self, s, e) -> None:
         """Create Square Signal"""
 
         self.s_m: np.ndarray = np.zeros(e - s)
         self.s_d: np.ndarray = np.zeros(e - s)
@@ -794,37 +774,50 @@
         from . import Q_
 
         if not os.path.exists(self.filename):  # check if the file is actually there
             raise FileNotFoundError(f"Cannot find file {self.filename}")
 
         # read external dataset
         df = pd.read_csv(self.filename)
+        # print(f"df = {df.head()}")
 
         # get unit information from each header
         xh = df.columns[0].split("[")[1].split("]")[0]
         yh = df.columns[1].split("[")[1].split("]")[0]
-        if len(df.columns) > 2:
-            zh = df.columns[2].split("[")[1].split("]")[0]
-        else:
-            zh = None
-
+        zh = df.columns[2].split("[")[1].split("]")[0] if len(df.columns) > 2 else None
         # create the associated quantities
         xq = Q_(xh)
         yq = Q_(yh)
 
         # add these to the data we are are reading
         self.s_time: np.ndarray = df.iloc[:, 0].to_numpy() * xq
         self.s_data: np.ndarray = df.iloc[:, 1].to_numpy() * yq
+
         if zh:
             # delta is assumed to be without units
             self.s_delta: np.ndarray = df.iloc[:, 2].to_numpy()
 
         # map into model units, and strip unit information
         self.s_time = self.s_time.to(self.mo.t_unit).magnitude
-        self.s_data = self.s_data.to(self.mo.f_unit).magnitude * self.scale
+        # self.s_data = self.s_data.to(self.mo.f_unit).magnitude * self.scale
+
+        if isinstance(yq, Q_):
+            # test what type of Quantity we have
+            if yq.check(["dimensionless"]):  # dimensionless
+                self.s_data = self.s_data.magnitude
+            elif yq.check(["volume]/[time"]):  # flux
+                self.s_data = self.s_data.to(self.mo.r_unit).magnitude
+            elif yq.check(["mass] / [time"]):  # flux
+                self.s_data = self.s_data.to(self.mo.f_unit).magnitude
+            elif yq.check(["[mass]/[volume]"]):  # concentration
+                self.s_data = self.s_data.to(self.mo.c_unit).magnitude
+            else:
+                ValueError(f"No conversion to model units for {self.scale} specified")
+
+        self.s_data = self.s_data * self.scale
 
         self.st: float = self.s_time[0]  # start time
         self.et: float = self.s_time[-1]  # end time
         self.duration = int(round((self.et - self.st)))
         num_steps = int(self.duration / self.mo.dt)
         # setup the points at which to interpolate
         xi = np.linspace(self.st, self.et, num_steps)
@@ -834,15 +827,15 @@
         )  # interpolate flux
         if zh:
             self.s_d: np.ndarray = np.interp(xi, self.s_time, self.s_delta)
             self.s_l = get_l_mass(self.s_m, self.s_d, self.sp.r)
         else:
             self.s_l: np.ndarray = np.zeros(num_steps)
 
-        return int(num_steps)
+        return num_steps
 
     def __apply_signal__(self) -> None:
         """In case we deal with a source  signal, we need
         to create a source, and connect signal, source and reservoir
         Maybe this logic should be me moved elsewhere?
         """
 
@@ -868,15 +861,15 @@
         # get delta of self
         sd = get_delta(self.data.l, self.data.m - self.data.l, self.data.sp.r)
         od = get_delta(other.data.l, other.data.m - other.data.l, other.data.sp.r)
         ns.data.m = self.data.m + other.data.m
         ns.data.l = get_l_mass(ns.data.m, sd + od, ns.data.sp.r)
 
         ns.n: str = self.n + "_and_" + other.n
-        print(f"adding {self.n} to {other.n}, returning {ns.n}")
+        # print(f"adding {self.n} to {other.n}, returning {ns.n}")
         ns.data.n: str = self.n + "_and_" + other.n + "_data"
         ns.st = min(self.st, other.st)
         ns.l = max(self.l, other.l)
         ns.sh = "compound"
         ns.los.append(self)
         ns.los.append(other)
 
@@ -904,28 +897,28 @@
         ns.stop: float = stop
         ns.offset: float = stop - start + offset
         ns.times: float = times
         ns.ms: np.ndarray = self.data.m[start:stop]  # get the data slice we are using
         ns.ds: np.ndarray = self.data.d[start:stop]
 
         diff = 0
-        for i in range(times):
-            start: int = start + ns.offset
-            stop: int = stop + ns.offset
+        for _ in range(times):
+            start += ns.offset
+            stop += ns.offset
             if start > len(self.data.m):
                 break
             elif stop > len(self.data.m):  # end index larger than data size
                 diff: int = stop - len(self.data.m)  # difference
-                stop: int = stop - diff  # new end index
+                stop -= diff
                 lds: int = len(ns.ds) - diff
             else:
                 lds: int = len(ns.ds)
 
-            ns.data.m[start:stop]: np.ndarray = ns.data.m[start:stop] + ns.ms[0:lds]
-            ns.data.d[start:stop]: np.ndarray = ns.data.d[start:stop] + ns.ds[0:lds]
+            ns.data.m[start:stop]: np.ndarray = ns.data.m[start:stop] + ns.ms[:lds]
+            ns.data.d[start:stop]: np.ndarray = ns.data.d[start:stop] + ns.ds[:lds]
 
         # and recalculate li and hi
         ns.data.l: np.ndarray
         ns.data.h: np.ndarray
         [ns.data.l, ns.data.h] = get_imass(ns.data.m, ns.data.d, ns.data.sp.r)
         return ns
 
@@ -938,27 +931,28 @@
         from esbmtk import Flux, Species
 
         self.fo: Flux = flux  # the flux handle
         self.sp: Species = flux.sp  # the species handle
         # list of processes
         flux.lop.append(self)
 
-    def __call__(self, t) -> list:
+    def __call__(self, t) -> list[float, float]:
         """Return Signal value at time t (mass and mass for light
         isotope). This will work as long a t is a multiple of dt, and i = t.
         may extend this by addding linear interpolation but that will
         be costly
 
         """
 
         import numpy as np
 
-        v = np.interp(t, self.mo.time, self.data.m)
+        m = np.interp(t, self.mo.time, self.data.m)
+        l = np.interp(t, self.mo.time, self.data.l)
 
-        return [v, 0]
+        return [m, l]
 
     def __plot__(self, M: Model, ax) -> None:
         """Plot instructions.
         M: Model
         ax: matplotlib axes handle
         """
 
@@ -967,15 +961,15 @@
         # convert time and data to display units
         x = (M.time * M.t_unit).to(M.d_unit).magnitude
         y1 = (self.data.m * M.f_unit).to(self.data.plt_units).magnitude
         legend = f"{self.legend_left} [{M.f_unit}]"
 
         # # test for plt_transform
         # if self.plot_transform_c != "None":
-        #     if callable(self.plot_transform_c):
+        #     if Callable(self.plot_transform_c):
         #         y1 = self.plot_transform_c(self.c)
         #     else:
         #         raise ValueError("Plot transform must be a function")
 
         # plot first axis
         ln1 = ax.plot(x[1:-2], y1[1:-2], color="C0", label=self.legend_left)
         ax.set_xlabel(f"{M.time_label} [{M.d_unit:~P}]")
@@ -1012,19 +1006,21 @@
     y axis.
 
     Example::
 
              DataField(name = "Name"
                        register = Model handle,
                        y1_data = np.Ndarray or list of arrays
-                       y1_label = Y-Axis label
-                       y1_legend = Data legend or list of legends
+                       y1_label = Data label(s)
+                       y1_legend = Y-Axis Label
+                       y1_type = "plot", | "scatter"
                        y2_data = np.Ndarray    # optional
-                       y2_label = Y-Axis label # optional
-                       y2_legend = Data legend # optional
+                       y2_legend = Y-Axis label # optional
+                       y2_label = Data legend(s) # optional
+                       y2_type = "plot", | "scatter"
                        common_y_scale = "no",  #optional, default "no"
                        display_precision = number, optional, inherited from Model
                        )
 
     Note that Datafield data is not mapped to model units. Care must be taken
     that the data units match the model units.
 
@@ -1066,20 +1062,22 @@
                     Reservoir_no_set,
                     VirtualReservoir,
                     ExternalCode,
                 ),
             ],
             "y1_data": ["None", (np.ndarray, list)],
             "x1_data": ["None", (np.ndarray, list, str)],
-            "y1_label": ["Not Provided", (str)],
-            "y1_legend": ["Not Provided", (str, list)],
+            "y1_label": ["Not Provided", (str, list)],
+            "y1_legend": ["Not Provided", (str)],
+            "y1_type": ["plot", (str, list)],
             "y2_data": ["None", (str, np.ndarray, list)],
             "x2_data": ["None", (np.ndarray, list, str)],
-            "y2_label": ["Not Provided", (str)],
-            "y2_legend": ["Not Provided", (str, list)],
+            "y2_label": ["Not Provided", (str, list)],
+            "y2_legend": ["Not Provided", (str)],
+            "y2_type": ["plot", (str, list)],
             "common_y_scale": ["no", (str)],
             "display_precision": [0.01, (int, float)],
         }
 
         # provide a list of absolutely required keywords
         self.lrk: list = ["name", ["register", "associated_with"], "y1_data"]
 
@@ -1097,65 +1095,37 @@
 
         # if self.associated_with == "None":
         #     self.associated_with = self.mo.lor[0]
 
         # self.mo = self.associated_with.mo
         self.mo = self.register.mo
         self.model = self.mo
+        if self.associated_with == "None":
+            if isinstance(self.register, Model):
+                self.associated_with = self.register.lor[0]
+            elif isinstance(self.register, Reservoir):
+                self.associated_with = self.register
+            else:
+                raise ValueError("Set associated_with or register to a reservoir name")
+
         if isinstance(self.associated_with, Reservoir):
             self.plt_units = self.associated_with.plt_units
         elif isinstance(self.associated_with, ReservoirGroup):
             self.plt_units = self.associated_with.lor[0].plt_units
         else:
             raise ValueError("This needs fixing")
 
-        if "self.y2_data" != "None":
-            self.d = self.y2_data
-            self.legend_right = self.y2_legend
-            self.ld = self.y2_label
+        # if not isinstance(self.y2_data, str):
+        #     self.d = self.y2_data
+        #     self.legend_right = self.y2_legend
+        #     self.ld = self.y2_label
 
         self.n = self.name
         self.led = []
 
-        if not isinstance(self.y1_data, list):
-            self.y1_data = [self.y1_data]
-
-        # if no x data provided, match with model
-        if self.x1_data == "None":
-            time = (self.mo.time * self.mo.t_unit).to(self.mo.d_unit).magnitude
-            self.x1_data = []
-            if isinstance(self.y1_data, list):
-                for i, e in enumerate(self.y1_data):
-                    self.x1_data.append(time)
-            else:
-                self.x1_data.append(time)
-        else:
-            if not isinstance(self.x1_data, list):
-                self.x1_data = [self.x1_data]
-
-        if self.x2_data == "None" and self.y2_data != "None":
-            self.x2_data = []
-            if isinstance(self.y2_data, list):
-                for i, e in enumerate(self.y2_data):
-                    self.x2_data.append(self.mo.time)
-            else:
-                self.x2_data.append(self.mo.time)
-        elif self.x2_data != "None":
-            if not isinstance(self.x2_data, list):
-                self.x2_data = [self.x2_data]
-
-        if not isinstance(self.y1_legend, list):
-            self.y1_legend = [self.y1_legend]
-
-        if not isinstance(self.y2_data, list):
-            self.y2_data = [self.y2_data]
-
-        if not isinstance(self.y2_legend, list):
-            self.y2_legend = [self.y2_legend]
-
         # register with reservoir
         # self.associated_with.ldf.append(self)
         # register with model. needed for print_reservoirs
         self.mo.ldf.append(self)
         if self.display_precision == 0:
             self.display_precision = self.mo.display_precision
 
@@ -1204,81 +1174,183 @@
                 f"Model register keyword must be 'None'/'local' not {self.sp.mo.register}"
             )
 
         # build the dataframe
         df: pd.dataframe = DataFrame()
 
         df[f"{self.n} Time [{mtu}]"] = self.mo.time[start:stop:stride]  # time
-        df[f"{self.n} {self.y1_label}"] = self.y1_data[start:stop:stride]  # y1 data
+        df[f"{self.n} {self.y1_legend}"] = self.y1_data[start:stop:stride]  # y1 data
 
         if self.y2_data != "None":
-            df[f"{self.n} {self.y1_label}"] = self.y2_data[start:stop:stride]  # y2_data
+            df[f"{self.n} {self.y2_legend}"] = self.y2_data[
+                start:stop:stride
+            ]  # y2_data
 
         file_path = Path(fn)
-        if append:
-            if file_path.exists():
-                df.to_csv(file_path, header=False, mode="a", index=False)
-            else:
-                df.to_csv(file_path, header=True, mode="w", index=False)
+        if append and file_path.exists():
+            df.to_csv(file_path, header=False, mode="a", index=False)
         else:
             df.to_csv(file_path, header=True, mode="w", index=False)
-
         return df
 
+    def __unify_data__(self, M: Model, x, y, label) -> tuple(list, list):
+        """The input data for the DataField Class can be either missing, be a
+        single array, or a list of arrays.  The module analyzes the data and
+        modifies is in such a way that it can be used by the __plot__ method
+        without further adjustments.
+
+        :param x: str, array, list, withe the x-data
+        :param y: str, array, list, withe the y-data
+
+        :return x,y: as list
+        """
+        import numpy as np
+
+        # print(f"ud0: type x = {type(x)}, len = {len(x)}")
+        # print(f"ud1: type y = {type(x)}, len = {len(y)}")
+        # consider the y-axis first
+        if isinstance(y, str):
+            ValueError("Provide at least one data-set")
+        elif isinstance(y, np.ndarray):
+            y = [y]
+            y_l = 1
+        elif isinstance(y, list):
+            y_l = len(y)
+        else:
+            raise ValueError("Y data needs to be array, numpy array or list")
+
+        # consider the x-axis next
+        if isinstance(x, str):  # no x-data has been provided
+            if y_l == 1:  # single y data
+                x = [M.time]
+                # print(f" no x-data y_l = {y_l}")
+            else:  # mutiple y data
+                # print(f" no x-data mutiple y-data y_l = {y_l}")
+                x = []
+                for e in range(y_l):
+                    x.append(M.time)
+
+        elif isinstance(x, np.ndarray):
+            # print(f"np_array, y_l = {y_l}")
+            xx = []
+            if y_l == 1:  # single y data
+                xx.append(x)
+            else:  # mutiple y data
+                # print(f" no x-data mutiple y-data y_l = {y_l}")
+                for e in range(y_l):
+                    xx.append(x)
+            x = xx
+            # print(f"after: {type(x)}")
+        elif isinstance(x, list):  # assume that lists match
+            if len(x) != len(y):
+                raise ValueError(f"Y data needs to match x data for {label}")
+        else:
+            raise ValueError(
+                f"Y data needs to be array, numpy array or list for {label}"
+            )
+
+        if y_l == 1:
+            if not isinstance(label, list):
+                label = [label]
+        elif y_l > 1:
+            if not isinstance(label, list):
+                ll = []
+                for e in y_l:
+                    ll.append(label)
+                label = ll
+
+        return x, y, label
+
+    def __plot_data__(self, ax, x, y, t, l, i) -> None:
+        """Plot data either as line of scatterplot
+
+        :param ax: axis handle
+        :param x: x data
+        :param y: y data
+        :param t: plot type
+        :param l: label str
+        :param i: index
+
+        """
+
+        if t == "plot":
+            ax.plot(x, y, color=f"C{i}", label=l)
+        else:
+            ax.scatter(x, y, color=f"C{i}", label=l)
+
     def __plot__(self, M: Model, ax) -> None:
         """Plot instructions.
         M: Model
         ax: matplotlib axes handle
         """
 
         from esbmtk import set_y_limits
 
+        # plot external data first
+        for (i, d) in enumerate(self.led):
+            time = (d.x * M.t_unit).to(M.d_unit).magnitude
+            # yd = (d.y * M.c_unit).to(self.plt_units).magnitude
+            leg = f"{d.legend}"
+            ax.scatter(time[1:-2], d.y[1:-2], color=f"C{i}", label=leg)
+
+        self.x1_data, self.y1_data, self.y1_label = self.__unify_data__(
+            M,
+            self.x1_data,
+            self.y1_data,
+            self.y1_label,
+        )
+
         for i, d in enumerate(self.y1_data):  # loop over datafield list
-            ax.plot(
+            # print(self.y1_legend)
+            self.__plot_data__(
+                ax,
                 self.x1_data[i],
                 self.y1_data[i],
-                color=f"C{i}",
-                label=self.y1_legend[i],
+                self.y1_type,
+                self.y1_label[i],
+                i,
             )
-
-        last_i = i
+            last_i = i
         # add any external data if present
-        for (i, d) in enumerate(self.led):
-            time = (d.x * M.t_unit).to(M.d_unit).magnitude
-            # yd = (d.y * M.c_unit).to(self.plt_units).magnitude
-            leg = f"{d.legend}"
-            ax.scatter(time[1:-2], d.y[1:-2], color=f"C{i+last_i}", label=leg)
 
         last_i = i
         ax.set_xlabel(f"{M.time_label} [{M.d_unit:~P}]")
-        ax.set_ylabel(self.y1_label)
+        ax.set_ylabel(self.y1_legend)
         # remove unnecessary frame species
         ax.spines["top"].set_visible(False)
         handler1, label1 = ax.get_legend_handles_labels()
 
-        if self.y2_data[0] != "None":
-            print(f"doing twinx for {self.full_name}")
+        # test if independeny y_data is present
+        if not isinstance(self.y2_data, str):
+            self.x2_data, self.y2_data, self.y2_label = self.__unify_data__(
+                M,
+                self.x2_data,
+                self.y2_data,
+                self.y2_label,
+            )
             axt = ax.twinx()
             for i, d in enumerate(self.y2_data):  # loop over datafield list
-                ax.plot(
-                    self.x1_data[i],
-                    self.y1_data[i],
-                    color=f"C{i+last_i}",
-                    label=self.y2_legend[i],
+                self.__plot_data__(
+                    axt,
+                    self.x2_data[i],
+                    self.y2_data[i],
+                    self.y2_type,
+                    self.y2_label[i],
+                    i + last_i + 1,
                 )
 
             axt.set_xlabel(f"{M.time_label} [{M.d_unit:~P}]")
-            axt.set_ylabel(self.y2_label)
+            axt.set_ylabel(self.y2_legend)
             # remove unnecessary frame species
             axt.spines["top"].set_visible(False)
             handler2, label2 = axt.get_legend_handles_labels()
             legend = axt.legend(handler1 + handler2, label1 + label2, loc=0).set_zorder(
                 6
             )
-            # axt.legend()
+            axt.legend()
         else:
             ax.legend(handler1, label1)
             ax.spines["right"].set_visible(False)
             ax.yaxis.set_ticks_position("left")
             ax.xaxis.set_ticks_position("bottom")
 
 
@@ -1306,30 +1378,30 @@
             ReservoirGroup,
         )
 
         # provide a dict of all known keywords and their type
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["None", (str)],
             "species": ["None", (str, Species)],
-            "plot_transform_c": ["None", (str, col.Callable)],
+            "plot_transform_c": ["None", (str, Callable)],
             "legend_left": ["None", (str)],
             "plot": ["yes", (str)],
             "groupname": ["None", (str)],
-            "function": ["None", (str, col.Callable)],
+            "function": ["None", (str, Callable)],
             "display_precision": [0.01, (int, float)],
             "register": [
                 "None",
                 (SourceGroup, SinkGroup, ReservoirGroup, ConnectionGroup, str),
             ],
             "full_name": ["None", (str)],
             "isotopes": [False, (bool)],
             "volume": ["None", (str, int, float)],
             "vr_datafields": [{}, (dict)],
-            "function_input_data": (List, str),
-            "function_params": [List(), (List, str)],
+            "function_input_data": (list, str),
+            "function_params": [list(), (list, str)],
             "geometry": ["None", (list, str)],
             "alias_list": ["None", (list, str)],
             "ref_flux": ["None", (list, str)],
         }
 
         # provide a list of absolutely required keywords
         self.lrk: list = [
@@ -1378,22 +1450,20 @@
 
                     data which will be computed by this function
                     provide alias name and default value
                     vr_datafields :dict ={"Hplus": self.swc.hplus,
                                           "Beta": 0.0},
 
                     function=calc_carbonates, # function reference, see below
-                    # A numba types List of one ore more np.arrays which are used
-                    # as input values for the user provided function
-                    function_input_data=List([self.DIC.c, self.TA.c]),
+                    function_input_data=list([self.DIC.c, self.TA.c]),
 
-                    # A numba types List of float parameters.
+                    # A list of float parameters.
                     alias_list = ["H", "CA", "HCO3", "CO3", "CO2aq"]
                     # Note that parameters must be individual float values
-                    function_params=List(
+                    function_params=list(
                         [
                             self.swc.K1,
                             self.swc.K2,
                             self.swc.KW,
                             self.swc.KB,
                             self.swc.boron,
                             self.swc.hplus,
@@ -1405,20 +1475,19 @@
 
         the dict keys of vr_datafields will be used to create alias
         names which can be used to access the respective variable
 
 
     The general template for a user defined function is a follows:
 
-    # @njit Add the njit decorator if you plan to use the numba solver
-    def calc_carbonates(i: int, input_data: List, vr_data: List, params: List) -> None:
+    def calc_carbonates(i: int, input_data: list, vr_data: list, params: list) -> None:
         # i = index of current timestep
-        # input_data = List of np.arrays, typically data from other Reservoirs
-        # vr_data = List of np.arrays created during instance creation (i.e. the vr data)
-        # params = List of float values (at least one!)
+        # input_data = list of np.arrays, typically data from other Reservoirs
+        # vr_data = list of np.arrays created during instance creation (i.e. the vr data)
+        # params = list of float values (at least one!)
 
         pass
 
     return
 
     Note that this function should not return any values, and that all input fields must have
     at least one entry!
@@ -1438,38 +1507,38 @@
             ConnectionGroup,
             GenericFunction,
             Species,
             SourceGroup,
             SinkGroup,
             ReservoirGroup,
         )
-        from numba.typed import List
+        from typing import Callable
 
         # provide a dict of all known keywords and their type
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["None", (str)],
             "species": ["None", (str, Species)],
-            "plot_transform_c": ["None", (str, col.Callable)],
+            "plot_transform_c": ["None", (str, Callable)],
             "legend_left": ["None", (str)],
             "plot": ["yes", (str)],
             "groupname": ["None", (str)],
-            "function": ["None", (col.Callable, str)],
+            "function": ["None", (Callable, str)],
             "display_precision": [0.01, (int, float)],
             "register": [
                 "None",
                 (SourceGroup, SinkGroup, ReservoirGroup, ConnectionGroup, str),
             ],
             "full_name": ["None", (str)],
             "isotopes": [False, (bool)],
             "volume": ["None", (str, int, float)],
             "vr_datafields": ["None", (dict, str)],
-            "function_input_data": ["None", (List, str)],
-            "function_params": ["None", (List, str)],
-            "geometry": ["None", (List, str)],
-            "alias_list": ["None", (List, str)],
+            "function_input_data": ["None", (list, str)],
+            "function_params": ["None", (list, str)],
+            "geometry": ["None", (list, str)],
+            "alias_list": ["None", (list, str)],
             "ftype": ["None", (str)],
             "ref_flux": ["None", (list, str)],
             "return_values": ["None", (str, dict)],
             "arguments": ["None", (str, list)],
             "r_s": ["None", (str, ReservoirGroup)],
             "r_d": ["None", (str, ReservoirGroup)],
         }
@@ -1494,15 +1563,15 @@
         self.state = 0
         name = f"{self.full_name}_generic_function".replace(".", "_")
         logging.info(f"creating {name}")
 
         self.alias_list = list(self.vr_datafields.keys())
 
         # initialize data fields
-        self.vr_data = List()
+        self.vr_data = list()
         for e in self.vr_datafields.values():
             if isinstance(e, (float, int)):
                 self.vr_data.append(np.full(self.mo.steps, e, dtype=float))
             else:
                 self.vr_data.append(e)
 
         self.gfh = GenericFunction(
@@ -1677,30 +1746,22 @@
             )
 
         df: pd.dataframe = DataFrame()
 
         df[f"{rn} Time [{mtu}]"] = self.mo.time[start:stop:stride]  # time
 
         for i, d in enumerate(self.vr_data):
-            if self.alias_list != "None":
-                h = self.alias_list[i]
-            else:
-                h = f"X{i}"
-
+            h = self.alias_list[i] if self.alias_list != "None" else f"X{i}"
             df[h] = d[start:stop:stride]
 
         file_path = Path(fn)
-        if append:
-            if file_path.exists():
-                df.to_csv(file_path, header=False, mode="a", index=False)
-            else:
-                df.to_csv(file_path, header=True, mode="w", index=False)
+        if append and file_path.exists():
+            df.to_csv(file_path, header=False, mode="a", index=False)
         else:
             df.to_csv(file_path, header=True, mode="w", index=False)
-
         return df
 
 
 class VirtualReservoir_no_set(ExternalCode):
     """Alias to ensure backwards compatibility"""
 
 
@@ -1730,22 +1791,14 @@
     as function of e.g., Alkalinity and DIC.
     Parameters:
      - name = name of process,
      - act_on = name of a reservoir this process will act upon
      - function  = a function reference
      - a1 to a3 function arguments
 
-    In order to be compatible with the numba solver, a1 and a2 must be
-    an array of 1-D numpy.arrays i.e., [m, l, h, c]. The array can have
-    any number of arrays though. a3 must be single array (or list).
-    The a3 array must be passed as List([...]), and List must be imported as
-
-    from numba.typed import List
-
-
     The function must return a list of numbers which correspond to the
     data which describe a reservoir i.e., mass, light isotope, heavy
     isotope, delta, and concentration
 
     In order to use this function we need first declare a function we plan to
     use with the generic function process. This function needs to follow this
     template::
@@ -1809,17 +1862,16 @@
         """
 
         allowed_keys: list = ["a1", "a2", "a3", "a4", "a5", "a6", "volume"]
         # loop over provided kwargs
         for key, value in kwargs.items():
             if key not in allowed_keys:
                 raise ValueError("you can only change a1 to a6")
-            else:
-                setattr(self, key, value)  # update self
-                setattr(self.gfh, key, value)  # update function
+            setattr(self, key, value)  # update self
+            setattr(self.gfh, key, value)  # update function
 
 
 class GasReservoir(ReservoirBase):
     """This object holds reservoir specific information similar to the Reservoir class
 
           Example::
 
@@ -1856,27 +1908,28 @@
     - Name.info()   # info Reservoir
     """
 
     def __init__(self, **kwargs) -> None:
         """Initialize a reservoir."""
 
         from esbmtk import Q_, Species, Model
+        from typing import Callable
 
         # provide a dict of all known keywords and their type
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["None", (str)],
             "species": ["None", (str, Species)],
             "delta": [0, (int, float)],
             "reservoir_mass": ["1.833E20 mol", (str, Q_)],
             "species_ppm": ["None", (str, Q_)],
-            "plot_transform_c": ["None", (str, col.Callable)],
+            "plot_transform_c": ["None", (str, Callable)],
             "legend_left": ["None", (str)],
             "plot": ["yes", (str)],
             "groupname": ["None", (str)],
-            "function": ["None", (str, col.Callable)],
+            "function": ["None", (str, Callable)],
             "display_precision": [0.01, (int, float)],
             "register": ["None", (str, Model)],
             "full_name": ["None", (str)],
             "isotopes": [False, (bool)],
             "geometry": ["None", (str, dict)],
             "rtype": ["regular", (str)],
         }
@@ -1921,15 +1974,16 @@
         self.m: np.ndarray = (
             np.zeros(self.species.mo.steps) + self.species_mass.magnitude
         )
         self.l: np.ndarray = np.zeros(self.mo.steps)
         # initialize concentration vector
         self.c: np.ndarray = self.m / self.volume
         # isotope mass
-        self.l = get_l_mass(self.m, self.delta, self.species.r)
+        # self.l = get_l_mass(self.m, self.delta, self.species.r)
+        self.l = get_l_mass(self.c, self.delta, self.species.r)
         # delta of reservoir
         self.v: float = np.zeros(self.mo.steps) + self.volume  # mass of atmosphere
 
         if self.mo.number_of_solving_iterations > 0:
             self.mc = np.empty(0)
             self.cc = np.empty(0)
             self.lc = np.empty(0)
@@ -1957,14 +2011,15 @@
         self.state = 0
 
     def __set_with_isotopes__(self, i: int, value: float) -> None:
         """write data by index"""
 
         self.m[i]: float = value[0]
         self.l[i]: float = value[1]
+        # self.c[i]: float = self.m[i] / self.v[i]  # update concentration
         # self.v[i]: float = self.v[i - 1] + value[0]
         # self.c[i]: float = self.m[i] / self.v[i]  # update concentration
         # self.h[i]: float = value[2]
         # self.d[i]: float = get_delta(self.l[i], self.h[i], self.sp.r)
 
     def __set_without_isotopes__(self, i: int, value: float) -> None:
         """write data by index"""
@@ -2032,21 +2087,20 @@
         from esbmtk import Q_, Model, Reservoir, DataField
 
         # dict of all known keywords and their type
         self.defaults: dict[str, list[any, tuple]] = {
             "name": ["None", (str)],
             "filename": ["None", (str)],
             "legend": ["None", (str)],
-            "reservoir": ["None", (str, Reservoir, DataField)],
+            "reservoir": ["None", (str, Reservoir, DataField, GasReservoir)],
             "offset": ["0 yrs", (Q_, str)],
             "display_precision": [0.01, (int, float)],
             "scale": [1, (int, float)],
-            "register": ["None", (str, Model, Reservoir, DataField)],
-            "convert_to": ["None", (Q_, str)],
-            "plot_transform_c": ["None", (str, col.Callable)],
+            "register": ["None", (str, Model, Reservoir, DataField, GasReservoir)],
+            "plot_transform_c": ["None", (str, callable)],
         }
 
         # provide a list of absolutely required keywords
         self.lrk: list = ["name", "filename", "legend", "reservoir"]
 
         self.__initialize_keyword_variables__(kwargs)
 
@@ -2071,31 +2125,34 @@
 
         if not os.path.exists(self.fn):  # check if the file is actually there
             raise FileNotFoundError(f"Cannot find file {self.fn}")
 
         self.df: pd.DataFrame = pd.read_csv(self.fn)  # read file
 
         ncols = len(self.df.columns)
-        if ncols != 3:  # test of we have 3 columns
-            raise ValueError("CSV file must have 3 columns")
+        if ncols < 2:  # test of we have at elast 2 columns
+            raise ValueError("CSV file must have at least 2 columns")
+        elif ncols == 2:
+            self.isotopes = False
+        elif ncols == 3:
+            self.isotopes = True
+        elif ncols > 3:
+            raise ValueError("External data only supports up to 2 Y columns")
+        else:
+            raise ValueError("ED: This should not happen")
 
         # print(f"Model = {self.mo.full_name}, t_unit = {self.mo.t_unit}")
         self.offset = self.ensure_q(self.offset)
         self.offset = self.offset.to(self.mo.t_unit).magnitude
 
         # get unit information
-        xq = Q_(get_string_between_brackets(self.df.columns[0]))
-        yq = Q_(get_string_between_brackets(self.df.columns[1]))
-        xs = xq.to(self.mo.t_unit).magnitude
-
-        if self.convert_to == "None":
-            ys = 1
-        else:
-            ys = yq.to(self.ensure_q(self.convert_to))
-            print(f"yq = {yq}, cvt= {self.convert_to}, ys = {ys}")
+        self.xq = Q_(get_string_between_brackets(self.df.columns[0]))
+        self.yq = Q_(get_string_between_brackets(self.df.columns[1]))
+        xs = self.xq.to(self.mo.d_unit).magnitude
+        ys = self.yq.to(self.register.plt_units).magnitude
 
         # scale input data into model  units
         self.x: np.ndarray = self.df.iloc[:, 0].to_numpy() * xs
         self.y: np.ndarray = self.df.iloc[:, 1].to_numpy() * ys
 
         # map into model space
         self.x = self.x - self.x[0] + self.offset
@@ -2103,17 +2160,16 @@
         # test for plt_transform
         if self.plot_transform_c != "None":
             if callable(self.plot_transform_c):
                 self.y = self.plot_transform_c(self.y)
             else:
                 raise ValueError("Plot transform must be a function")
 
-        # check if z-data is present
-        if ncols == 3:
-            # zh = self.df.columns[2]
+        # zh = self.df.columns[2]
+        if self.isotopes:
             self.z = self.df.iloc[:, 2].to_numpy()
 
         # register with reservoir
         self.__register__(self.reservoir)
 
         if self.mo.register == "local" and self.register == "None":
             self.register = self.mo
```

### Comparing `esbmtk-0.8.0.0/esbmtk/odeuli2.py` & `esbmtk-0.9.0.1/esbmtk/ode_backend.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,216 @@
 from __future__ import annotations
 import typing as tp
 
 if tp.TYPE_CHECKING:
-    from esbmtk import Flux, Reservoir, Model, Connection, Connect
+    from esbmtk import Flux, Reservoir, Model, Connection, Connect, numpy
 
 
-def get_initial_conditions(M: Model) -> tuple[list, list, list, list]:
-    """get list of initial conditions. THis list needs to match
-    the number of equations. We need to consider 3 types reservoirs:
-
-    1) Reservoirs that change as a result of physical fluxes
-       i.e. r.lof > 0. These require a flux statements and a
-       reservoir equation.
-
-    2) Reservoirs that do not have active fluxes but are computed
-       as a tracer, i.e.. HCO3. These only require a reservoir
-       equation
-
-    3) Reservoirs that do not change but are used as input. Those
-       should not happen in a well formed model, but we cannot
-       exclude the possibility. In this case, there is no flux
-       equation, and we state that dR/dt = 0
-
-    see also get_ic()
+def get_initial_conditions(
+    M: Model,
+    rtol: float,
+    atol_d: float = 1e-6,
+) -> tuple[list, dict, list, list, numpy.array]:
+    """Get list of initial conditions.  This list needs to match the
+    number of equations.
+
+    :param Model: The model handle
+    :param rtol: relative tolerance for BDF solver.
+    :param atol_d: default value for atol if c = 0
+
+    :return: R = list of initial conditions as floats
+    :return: icl = dict[Reservoir, list[int, int]] where reservoir
+             indicates the reservoir handle, and the list contains the
+             index into the reservoir data.  list[0] = concentration
+             list[1] concentration of the light isotope.
+    :return: cpl = list of reservoirs that use function to evaluate
+             reservoir data
+    :return: ipl = list of static reservoirs that serve as input
+    :return: rtol = array of tolerence values for ode solver
+
+        We need to consider 3 types of reservoirs:
+
+        1) Reservoirs that change as a result of physical fluxes i.e.
+        r.lof > 0.  These require a flux statements and a reservoir
+        equation.
+
+        2) Reservoirs that do not have active fluxes but are computed
+        as a tracer, i.e.. HCO3.  These only require a reservoir
+        equation
+
+        3) Reservoirs that do not change but are used as input.  Those
+        should not happen in a well formed model, but we cannot
+        exclude the possibility.  In this case, there is no flux
+        equation, and we state that dR/dt = 0
+
+        get_ic() will look up the index position of the
+        reservoir_handle on icl, and then use this index to retrieve
+        the correspinding value in R
 
+        Isotopes are handled by adding a second entry
     """
+    import numpy as np
 
     R = []  # list of initial conditions
-    icl: list = []  # list of reservoirs that depend on fluxes
+    atol: list = []  # list of tolerances for ode solver
+    # dict that contains the reservoir_handle as key and the index positions
+    # for c and l as a list
+    icl: dict[Reservoir, list[int, int]] = {}
     cpl: list = []  # list of reservoirs that are computed
     ipl: list = []  # list of static reservoirs that serve as input
 
+    i: int = 0
     for r in M.lic:
-        # print(f"R={r.full_name} lof = {len(r.lof)}")
-        if len(r.lof) > 0:  # list of reservoirs that depend on fluxes
-            R.append(r.c[0])
-            icl.append(r)
+        # collect all reservoirs that have initial conditions
+        if len(r.lof) > 0 or r.rtype == "computed" or r.rtype == "passive":
+            R.append(r.c[0])  # add initial condition
+            if r.c[0] > 0:
+                # compute tol such that tol < rtol * abs(y)
+                tol = rtol * abs(r.c[0]) / 10
+                atol.append(tol)
+                r.atol[0] = tol
+            else:
+                atol.append(atol_d)
+                r.atol[0] = atol_d
 
-        if r.rtype == "computed" or r.rtype == "passive":
-            R.append(r.c[0])
-            icl.append(r)
+            if r.isotopes:
+                if r.l[0] > 0:
+                    # compute tol such that tol < rtol * abs(y)
+                    tol = rtol * abs(r.l[0]) / 10
+                    atol.append(tol)
+                    r.atol[1] = tol
+                else:
+                    atol.append(atol_d)
+                    r.atol[1] = atol_d
+
+                R.append(r.l[0])  # add initial condition for l
+                icl[r] = [i, i + 1]
+                i += 2
+            else:
+                icl[r] = [i, i]
+                i += 1
 
-    return R, icl, cpl, ipl
+    return R, icl, cpl, ipl, np.array(atol)
 
 
-def write_reservoir_equations(
-    eqs,
-    M: Model,
-    rel: str,  # string with reservoir names used in return function
-    ind2: str,  # indent 2 times
-    ind3: str,  # indent 3 times
-) -> str:  # updated list of reservoirs
-    """Loop over reservoirs and their fluxes to build the reservoir equation"""
+def write_reservoir_equations(eqs, M: Model, rel: str, ind2: str, ind3: str) -> str:
+    """Loop over reservoirs and their fluxes to build the reservoir
+    equation
+
+    :param eqs: equation file handle
+    :param rel: string with reservoir names used in return function.
+        Note that these are the reervoir names as used by the
+        equations and not the reservoir names used by esbmtk. E.g.,
+        M1.R1.O2 will be M1_R1_O2,
+    :param ind2: string with indentation offset
+    :param ind3: string with indentation offset
+
+    :returns: rel = updated list of reservoirs names
+    """
 
     from esbmtk import ReservoirGroup
 
     for r in M.lor:  # loop over reservoirs
-        # Write equations for each reservoir
-        # create unique variable names. Reservoirs are typiclally called
-        # M.rg.r so we replace all dots with underscore
+        """
+        Write equations for each reservoir and create unique variable
+        names.  Reservoirs are typiclally called M.rg.r so we replace
+        all dots with underscore -> M_rg_r
+        """
 
         name = f'{r.full_name.replace(".", "_")}'
         fex = ""
 
         # add all fluxes
         for flux in r.lof:  # check if in or outflux
             if flux.parent.source == r:
                 sign = "-"
             elif flux.parent.sink == r:
                 sign = "+"
 
             fname = f'{flux.full_name.replace(".", "_")}'
-            fex = fex + f"{ind3}{sign} {fname}\n"
+            fex = f"{fex}{ind3}{sign} {fname}\n"
 
-        # check if reservoir requires carbonate burial fluxes
-        if isinstance(r.parent, ReservoirGroup):
-            if r.parent.has_cs2:
-                if r.species.name == "DIC" or r.species.name == "TA":
-                    fn = f"{r.full_name}.burial".replace(".", "_")
-                    fex = f"{fex}{ind3}- {fn}\n"
+        if (  # check if reservoir requires carbonate burial fluxes
+            isinstance(r.parent, ReservoirGroup)
+            and r.parent.has_cs2
+            and r.species.name in ["DIC", "TA"]
+        ):
+            fn = f"{r.full_name}.burial".replace(".", "_")
+            fex = f"{fex}{ind3}- {fn}\n"
 
-        # avoid reservoirs without active fluxes
-        if len(r.lof) > 0:
+        if len(r.lof) > 0:  # avoid reservoirs without active fluxes
             eqs.write(f"{ind2}{name} = (\n{fex}{ind2})/{r.full_name}.volume\n\n")
-            rel = rel + f"{ind3}{name},\n"
+            rel = f"{rel}{ind3}{name},\n"
 
     return rel
 
 
-def write_reservoir_equations_with_istopes(
+def write_reservoir_equations_with_isotopes(
     eqs,
     M: Model,
-    rel: str,  # string with reservoir names used in return function
+    rel: str,  # string with reservoir names returned by setup_ode
     ind2: str,  # indent 2 times
     ind3: str,  # indent 3 times
 ) -> str:  # updated list of reservoirs
     """Loop over reservoirs and their fluxes to build the reservoir equation"""
 
     from esbmtk import ReservoirGroup
 
     for r in M.lor:  # loop over reservoirs
         # Write equations for each reservoir
         # create unique variable names. Reservoirs are typiclally called
         # M.rg.r so we replace all dots with underscore
-
-        # need to query the connection and decide if isotopes are
-        # needed and then only write the isotope equation?  Ort do
-        # this on a per reservoir base
-
-        name = f'{r.full_name.replace(".", "_")}_l'
-        fex = ""
-
-        # add all fluxes
-        for flux in r.lof:  # check if in or outflux
-            if flux.parent.source == r:
-                sign = "-"
-            elif flux.parent.sink == r:
-                sign = "+"
-
-            fname = f'{flux.full_name.replace(".", "_")}_l'
-            fex = fex + f"{ind3}{sign} {fname}\n"
-
-        # check if reservoir requires carbonate burial fluxes
-        if isinstance(r.parent, ReservoirGroup):
-            if r.parent.has_cs2:
-                if r.species.name == "DIC" or r.species.name == "TA":
-                    fn = f"{r.full_name}.burial".replace(".", "_")
-                    fex = f"{fex}{ind3}- {fn}\n"
-
-        # avoid reservoirs without active fluxes
-        if len(r.lof) > 0:
-            eqs.write(f"{ind2}{name} = (\n{fex}{ind2})/{r.full_name}.volume\n\n")
-            rel = rel + f"{ind3}{name},\n"
+        if r.isotopes:
+            name = f'{r.full_name.replace(".", "_")}_l'
+            fex = ""
+            # add all fluxes
+            for flux in r.lof:  # check if in or outflux
+                if flux.parent.source == r:
+                    sign = "-"
+                elif flux.parent.sink == r:
+                    sign = "+"
+
+                fname = f'{flux.full_name.replace(".", "_")}_l'
+                fex = f"{fex}{ind3}{sign} {fname}\n"
+
+            # check if reservoir requires carbonate burial fluxes
+            if (
+                isinstance(r.parent, ReservoirGroup)
+                and r.parent.has_cs2
+                and r.species.name == "DIC"
+            ):
+                fn = f"{r.full_name}.burial".replace(".", "_")
+                fn = f"{fn}_l"
+                fex = f"{fex}{ind3}- {fn}\n"
+
+            # avoid reservoirs without active fluxes
+            if len(r.lof) > 0:
+                # print(f"Adding: {name} to rel")
+                eqs.write(f"{ind2}{name} = (\n{fex}{ind2})/{r.full_name}.volume\n\n")
+                rel = f"{rel}{ind3}{name},\n"
 
     return rel
 
 
 def write_equations_2(
-    M: Model, R: list[float], icl: list, cpl: list, ipl: list
+    M: Model, R: list[float], icl: dict, cpl: list, ipl: list
 ) -> tuple:
-    """Write file that contains the ode-equations for M
-    Returns the list R that contains the initial condition
-    for each reservoir
-
-    icl: list of reservoirs that have actual fluxes
-    cpl: list of reservoirs that hjave no fluxes but are computed based on other R's
-    ipl: list of reservoir that do not change in concentration
+    """Write file that contains the ode-equations for the Model
+    Returns the list R that contains the initial condition for each
+    reservoir
 
+    :param Model: Model handle
+    :param R: list of floats with the initial conditions for each
+              reservoir
+    :param icl: dict of reservoirs that have actual fluxes
+    :param cpl: list of reservoirs that have no fluxes but are
+        computed based on other reservoirs
+    :param ipl: list of reservoir that do not change in concentration
     """
-    from esbmtk import Model, ReservoirGroup
+    # from esbmtk import Model, ReservoirGroup
     import pathlib as pl
 
     # get pathlib object
     fn: str = "equations.py"  # file name
     cwd: pl.Path = pl.Path.cwd()  # get the current working directory
     fqfn: pl.Path = pl.Path(f"{cwd}/{fn}")  # fully qualified file name
 
@@ -172,438 +230,485 @@
 
     def __init__(self, M: Model)->None:
         ''' Use this method to initialize all variables that require the state
             t-1
         '''
         import numpy as np
 
-        self.i = 0
-        self.t = []
-        self.last_t = 0
-
     def eqs(self, t, R: list, M: Model) -> list:
         '''Auto generated esbmtk equations do not edit
         '''
 
         from esbmtk import carbonate_system_1_ode, carbonate_system_2_ode
-        from esbmtk import gas_exchange_ode, get_hplus
-
-        max_i = len(M.time)-1
+        from esbmtk import gas_exchange_ode, gas_exchange_ode_with_isotopes
 
         # flux equations
 """
 
+    from esbmtk import AirSeaExchange
+
     # """
     # write file
     with open(fqfn, "w", encoding="utf-8") as eqs:
-
         rel = ""  # list of return values
         # ind1 = 4 * " "
         ind2 = 8 * " "  # indention
         ind3 = 12 * " "  # indention
-
         eqs.write(header)
-
-        eqs.write(f"{ind2}{M.name} = M\n")
-
-        sep = "# ---------------- write computed reservoir equations -------- #\n"
-        sep = sep + "# that do not depend on fluxes"
-
+        # eqs.write(f"{ind2}{M.name} = M\n")
+        sep = (
+            "# ---------------- write computed reservoir equations -------- #\n"
+            + "# that do not depend on fluxes"
+        )
         eqs.write(f"\n{sep}\n")
 
         for r in M.lpc_r:  # All virtual reservoirs need to be in this list
-
             if r.ftype == "cs1":
                 rel = write_cs_1(eqs, r, icl, rel, ind2, ind3)
-            elif r.ftype == "cs2":
-                pass  # see below
-            else:
+            elif r.ftype != "cs2":
                 raise ValueError(f"{r.ftype} is undefined")
 
-        flist = list()
-
+        flist = []
         sep = "# ---------------- write all flux equations ------------------- #"
         eqs.write(f"\n{sep}\n")
-
         for flux in M.lof:  # loop over fluxes
             # fluxes belong to at least 2 reservoirs, so we need to avoid duplication
             # we cannot use a set, since we need to preserve order
             if flux not in flist:
-                ex, exl = get_flux(flux, M, R, icl)
+                flist.append(flux)  # add to list of fluxes already computed
+                ex, exl = get_flux(flux, M, R, icl)  # get flux expressions
                 fn = flux.full_name.replace(".", "_")
-                eqs.write(f"{ind2}{fn} = {ex}\n")
-                flist.append(flux)
 
-                # add equations for light isotope
-                if flux.parent.isotopes:
-                    fn = flux.full_name.replace(".", "_")
-                    eqs.write(f"{ind2}{fn}_l = {exl}\n")
-                    flist.append(flux)
+                # check for types that return isotope data as well
+                if isinstance(flux.parent, AirSeaExchange):
+                    if flux.parent.isotopes:  # add F_l if necessary
+                        fn = f"{fn}, {fn}_l"
+                    eqs.write(f"{ind2}{fn} = {ex}\n")
+
+                else:  # all others types
+                    eqs.write(f"{ind2}{fn} = {ex}\n")
+                    if flux.parent.isotopes:  # add line for isotopes
+                        eqs.write(f"{ind2}{fn}_l = {exl}\n")
+
+                if flux.save_flux_data:
+                    eqs.write(f"{ind2}{flux.full_name}.m[self.i] = {fn}\n")
+                    if flux.parent.isotopes:
+                        eqs.write(f"{ind2}{flux.full_name}.l[self.i] = {fn}_l\n")
+
+        sep = (
+            "# ---------------- write computed reservoir equations -------- #\n"
+            + "# that do depend on fluxes"
+        )
 
-        sep = "# ---------------- write computed reservoir equations -------- #\n"
-        sep = sep + "# that do depend on fluxes"
         eqs.write(f"\n{sep}\n")
 
         for r in M.lpc_r:  # All virtual reservoirs need to be in this list
-
             if r.ftype == "cs1":
                 pass  # see above
             elif r.ftype == "cs2":  #
                 rel = write_cs_2(eqs, r, icl, rel, ind2, ind3)
             else:
                 raise ValueError(f"{r.ftype} is undefined")
 
         sep = "# ---------------- write input only reservoir equations -------- #"
         eqs.write(f"\n{sep}\n")
-
         for r in ipl:
             rname = r.full_name.replace(".", "_")
             eqs.write(f"{ind2}{rname} = 0.0")
 
         sep = "# ---------------- write regular reservoir equations ------------ #"
         eqs.write(f"\n{sep}\n")
 
+        # rel = write_reservoir_equations(eqs, M, rel, ind2, ind3)
         rel = write_reservoir_equations(eqs, M, rel, ind2, ind3)
 
+        sep = "# ---------------- write isotope reservoir equations ------------ #"
+        eqs.write(f"\n{sep}\n")
+
+        # rel = write_reservoir_equations(eqs, M, rel, ind2, ind3)
+        rel = write_reservoir_equations_with_isotopes(eqs, M, rel, ind2, ind3)
+
         sep = "# ---------------- bits and pieces --------------------------- #"
         eqs.write(
             f"\n{sep}\n"
-            f"{ind2}self.i += 1\n"
-            f"{ind2}self.t.extend([t])\n"
-            f"{ind2}self.last_t = t\n"
             f"{ind2}return [\n"
         )
-        for i, r in enumerate(icl):
-            eqs.write(f"{ind3}{r.full_name.replace('.', '_')},  # {i}\n")
+        # Write all initial conditions that are recorded in icl
+        for k, v in icl.items():
+            eqs.write(f"{ind3}{k.full_name.replace('.', '_')},  # {v[0]}\n")
+            if k.isotopes:
+                eqs.write(f"{ind3}{k.full_name.replace('.', '_')}_l,  # {v[1]}\n")
 
         eqs.write(f"{ind2}]\n")
-
-        if len(R) != len(rel.split(",")) - 1:
-            raise ValueError(
-                f"number of initial conditions ({len(R)})"
-                f"does not match number of return values ({len(rel.split(','))-1}')\n\n"
-                f"R = {R}\n"
-                f"rv = {rel}\n"
-            )
-
+        # if len(R) != len(rel.split(",")) - 1:
+        #     raise ValueError(
+        #         f"number of initial conditions ({len(R)})"
+        #         f"does not match number of return values"
+        #         f"({len(rel.split(','))-1}')\n\n"
+        #     )
     return fqfn
 
 
-def get_flux(flux: Flux, M: Model, R: list[float], icl: list) -> tuple(str, str):
-    """Create formula expressions that describes the flux f
-    return expression ex as string
+def get_flux(flux: Flux, M: Model, R: list[float], icl: dict) -> tuple(str, str):
+    """Create formula expressions that calcultes the flux F.  Return
+    the equation expression as string
+
+    :param flux: The flux object for which we create the equation
+    :param M: The current model object
+    :param R: The list of initial conditions for each reservoir
+    :param icl: dict of reservoirs that have actual fluxes
+
+    :returns: A tuple where the first string is the equation for the
+              total flux, and the second string is the equation for
+              the flux of the light isotope
     """
 
     ind2 = 8 * " "  # indentation
     ind3 = 12 * " "  # indentation
 
     ex = ""  # expression string
     exl = ""  # expression string for light isotope
     c = flux.parent  # shorthand for the connection object
     cfn = flux.parent.full_name  # shorthand for the connection object name
 
     if c.ctype.casefold() == "regular":
-        ex, exl = get_regular_flux(flux, c, icl, ind2, ind3)
+        ex, exl = get_regular_flux_eq(flux, c, icl, ind2, ind3)
 
     elif c.ctype == "scale_with_concentration":
-        ex, exl = get_scale_with_concentration(flux, c, cfn, icl)
+        ex, exl = get_scale_with_concentration_eq(flux, c, cfn, icl, ind2, ind3)
 
     elif c.ctype == "scale_with_mass":
-        ex, exl = get_scale_with_concentration(flux, c, cfn, icl)
+        ex, exl = get_scale_with_concentration_eq(flux, c, cfn, icl, ind2, ind3)
 
     elif c.ctype == "scale_with_flux":
-        ex, exl = get_scale_with_flux(flux, c, cfn, icl)
+        ex, exl = get_scale_with_flux_eq(flux, c, cfn, icl, ind2, ind3)
 
     elif c.ctype == "weathering":
-        ex, exl = get_weathering(flux, c, cfn, icl, ind2, ind3)
+        ex, exl = get_weathering_eq(flux, c, cfn, icl, ind2, ind3)
 
     elif c.ctype == "gas_exchange":  # Gasexchange
         if c.isotopes:
-            ex, exl = get_gas_exchange_w_isotopes(flux, c, cfn, icl, ind2, ind3)
+            ex = get_gas_exchange_w_isotopes_eq(flux, c, cfn, icl, ind2, ind3)
         else:
-            ex = get_gas_exchange(flux, c, cfn, icl, ind2, ind3)
+            ex = get_gas_exchange_eq(flux, c, cfn, icl, ind2, ind3)
     else:
         raise ValueError(
             f"Connection type {c.ctype} for {c.full_name} is not implmented"
         )
 
     return ex, exl
 
 
-def check_signal_2(ex: str, c: tp.union(Connection, Connect)) -> str:
-    """Test if connection requires a signal"""
+def check_signal_2(ex: str, exl: str, c: Connection | Connect) -> (str, str):
+    """Test if connection is affected by a signal
+
+    :param ex: equation string
+    :param c: connection object
+
+    :returns: (modified) equation string
+    """
+
+    if c.signal != "None":  # get signal type
 
-    sign = ""
-    if c.signal != "None":
-        # get signal type
         if c.signal.stype == "addition":
             sign = "+"
-        elif c.signal.stype == "scale":
+        elif c.signal.stype == "multiplication":
             sign = "*"
         else:
             raise ValueError(f"stype={c.signal.stype} not implemented")
 
-        ex = ex + f" {sign} {c.signal.full_name}(t)[0]  # Signal"
+        ex += f" {sign} {c.signal.full_name}(t)[0]  # Signal"
+        if c.source.isotopes:
+            exl += f" {sign} {c.signal.full_name}(t)[1]  # Signal"
+        else:
+            exl += ""
 
-    return ex
+    return ex, exl
 
 
-def get_ic(r: Reservoir, icl: list, isotopes=False) -> str:
-    """Get initial condition. If r in icl, return index
-    expression into R. If r is not in index, return
-    Reservoir concentration a t=0
+def get_ic(r: Reservoir, icl: dict, isotopes=False) -> str:
+    """Get initial condition in a reservoir.  If the reservoir is icl,
+    return index expression into R.c. If the reservoir is not in the
+    index, return the Reservoir concentration a t=0
 
     In both cases return these a string
 
-    If the isotopes varibale is set to True, return the pointter to
-    the light isotope reser instead
+    If isotopes == True, return the pointer to the light isotope
+    concentration
+
+    :param r: A reservoir handle
+    :param icl: icl = dict[Reservoir, list[int, int]] where reservoir
+        indicates the reservoir handle, and the list contains the
+        index into the reservoir data.  list[0] = concentration
+        list[1] concentration of the light isotope.
+    :param isotopes: whether to return the total mass or the mass of
+        the light isotope
+
+    :raises ValueError: get_ic: can't find {r.full_name} in list of
+        initial conditions
+
+    :returns: the string s which is the full_name of the reservoir
+              concentration or isotope concentration
     """
+    from esbmtk import Source, Sink
 
     s = ""
 
-    if isotopes:
-        pass
+    if r in icl:
+        s = f"R[{icl[r][1]}]" if isotopes else f"R[{icl[r][0]}]"
+    elif isinstance(r, (Source, Sink)):
+        s = f"{r.full_name}.c"
+        if r.isotopes:
+            s = f"{r.full_name}.l"
     else:
-        if r in icl:
-            s = f"R[{icl.index(r)}]"
-        else:
-            raise ValueError(f"get_ic: this should not happen r = {r.full_name}")
-            s = f"{r.full_name}.c[0]"
+        #
+        raise ValueError(
+            f"get_ic: can't find {r.full_name} in list of initial conditions"
+        )
 
     return s
 
 
 # ------------------------ define processes ------------------------- #
 
 
-def write_cs_1(eqs, r: Reservoir, icl: list, rel: str, ind2: str, ind3: str) -> list:
-    """Write the python code that defines carbonate system 1"""
+def write_cs_1(eqs, r: Reservoir, icl: dict, rel: str, ind2: str, ind3: str) -> str:
+    """Write the python code that defines carbonate system 1, add the
+    name of the reservoir carbonate system to the string of reservoir
+    names in rel
+
+    :param eqs: equation file handle
+    :param r: reservoir_handle
+    :param icl: dict of reservoirs that have actual fluxes
+    :param rel: string with reservoir names returned by setup_ode
+    :param ind2: indent 2 times
+    :param ind3: indent 3 times
 
+    :returns: rel: modied string of reservoir names
+    """
     fname = f"{r.parent.full_name}.Hplus".replace(".", "_")
     cname = f"{r.parent.full_name}.CO2aq".replace(".", "_")
 
     eqs.write(
         f"{ind2}{fname}, {cname} = carbonate_system_1_ode(\n"
-        f"{ind3}{r.parent.full_name},\n"
+        f"{ind3}{r.parent.full_name}.swc,\n"
         f"{ind3}{get_ic(r.parent.DIC, icl)},\n"
         f"{ind3}{get_ic(r.parent.TA, icl)},\n"
         f"{ind3}{get_ic(r.parent.Hplus, icl)},\n"
-        f"{ind3}self.i,\n"
-        f"{ind3}max_i)  # cs1\n"
+        f"{ind2})  # cs1\n"
     )
-    rel = rel + f"{ind3}{fname},\n"
+    rel += f"{ind3}{fname},\n"
 
     return rel
 
 
-def write_cs_2(eqs, r: Reservoir, icl: list, rel: str, ind2: str, ind3: str) -> list:
-    """Write the python code that defines carbonate system 2"""
+def write_cs_2(eqs, r: Reservoir, icl: dict, rel: str, ind2: str, ind3: str) -> str:
+    """Write the python code that defines carbonate system 2, add the
+    name of the reservoir carbonate system to the string of reservoir
+    names in rel
+
+    :param eqs: equation file handle
+    :param r: reservoir_handle
+    :param icl: dict of reservoirs that have actual fluxes
+    :param rel: string with reservoir names returned by setup_ode
+    :param ind2: indent 2 times
+    :param ind3: indent 3 times
+
+    :returns: rel: modied string of reservoir names
+    """
 
     influx = r.parent.cs.ref_flux[0].full_name.replace(".", "_")
 
     # get DIC reservoir of the surface box
     sb_DIC = getattr(r.r_s, "DIC")
 
     if r.register.DIC.isotopes:
         source_m = get_ic(sb_DIC, icl)
         source_l = get_ic(sb_DIC, icl, isotopes=True)
     else:
-        print(f"sb_DIC = {sb_DIC.full_name}")
+        # print(f"sb_DIC = {sb_DIC.full_name}")
         source_m = get_ic(sb_DIC, icl)
         source_l = 1
 
     fn_dic = f"{r.register.DIC.full_name}.burial".replace(".", "_")
     fn_dic_l = f"{fn_dic}_l"
     fn_ta = f"{r.register.TA.full_name}.burial".replace(".", "_")
 
     fname = f"{r.parent.full_name}.Hplus".replace(".", "_")
     zname = f"{r.parent.full_name}.zsnow".replace(".", "_")
     zmax = r.parent.cs.function_params[15]
     eqs.write(
+        f"{ind2} # Limit zsnow >= zmax\n"
+        f"{ind2}if {get_ic(r.parent.zsnow, icl)} > {zmax}:"
+        f" {get_ic(r.parent.zsnow, icl)} = {zmax}\n"
         f"{ind2}{fn_dic}, {fn_dic_l}, {fname}, {zname} = carbonate_system_2_ode(\n"
-        f"{ind3}t, \n"  # current time
-        f"{ind3}{r.parent.full_name}, \n"  # Reservoir handle
-        f"{ind3}{influx}, \n"  # CaCO3 export flux
-        f"{ind3}{get_ic(r.parent.DIC, icl)}, \n"  # DIC in the deep box
-        f"{ind3}{get_ic(r.parent.TA, icl)}, \n"  # TA in the deep box
-        f"{ind3}{source_m}, \n"  # DIC in the surface box
-        f"{ind3}{source_l}, \n"  # DIC of the light isotope in the surface box
-        f"{ind3}{get_ic(r.parent.Hplus, icl)}, \n"  # H+ in the deep box at t-1
-        f"{ind3}{get_ic(r.parent.zsnow, icl)}, \n"  # zsnow in mbsl at t-1
-        f"{ind3}self.i, \n"  # current index
-        f"{ind3}max_i, \n"  # max is of vr data fields
-        f"{ind3}self.last_t, \n"  # t at t-1
+        f"{ind3}{r.parent.full_name},  # 2: Reservoirgroup handle\n"
+        f"{ind3}{influx},  # 3: CaCO3 export flux\n"
+        f"{ind3}{get_ic(r.parent.DIC, icl)},  # 4: DIC in the deep box\n"
+        f"{ind3}{get_ic(r.parent.TA, icl)},  # 5: TA in the deep box\n"
+        f"{ind3}{source_m},  # 6: DIC in the surface box\n"
+        f"{ind3}{source_l},  # 7: DIC of the light isotope in the surface box\n"
+        f"{ind3}{get_ic(r.parent.Hplus, icl)},  # 8: H+ in the deep box at t-1\n"
+        f"{ind3}{get_ic(r.parent.zsnow, icl)},  # 9: zsnow in mbsl at t-1\n"
         f"{ind2})  # cs2\n"
         # calculate the TA dissolution flux from DIc diss flux
         f"{ind2}{fn_ta} = {fn_dic} * 2  # cs2\n"
-        f"{ind2} # Limit zsnow >= zmax\n"
-        f"{ind2}if {get_ic(r.parent.zsnow, icl)} > {zmax}:"
-        f" {get_ic(r.parent.zsnow, icl)} = {zmax}\n"
     )
     # add Hplus to the list of return values
-    rel = rel + f"{ind3}{fname},\n"
-    rel = rel + f"{ind3}{zname},\n"
+    rel += f"{ind3}{fname},\n"
+    rel = f"{rel}{ind3}{zname},\n"
 
     return rel
 
 
-def get_regular_flux(
+def get_regular_flux_eq(
     flux: Flux,  # flux instance
-    c: Connect,  # connection instance
-    icl: list,  # list of initial conditions
+    c: Connect | Connection,  # connection instance
+    icl: dict,  # list of initial conditions
     ind2,  # indentation
     ind3,  # indentation
 ) -> tuple:
-    """Equation defining a fixed rate flux
-    Example:
+    """Create a string containing the equation for a regular (aka
+    fixed rate) connection
 
-    ex =  M1.C_Fw_to_CO2_At_DIC_volcanic_flux._F.rate
-    exl = M1.C_Fw_to_CO2_At_DIC_volcanic_flux._F.rate
+    :param flux: flux instance
+    :param c: connection object
+    :param icl: dict of reservoirs that have actual fluxes
+    :param ind2: indent 2 times
+    :param ind3: indent 3 times
+
+    :returns: two strings, where the first describes the equation for
+              the total flux, and the second describes the rate for
+              the light isotope
+    """
+    ex = f"{flux.full_name}.rate"  # get flux rate string
+    exl = check_isotope_effects(ex, c, icl, ind3, ind2)
+    ex, exl = check_signal_2(ex, exl, c)  # check if we hav to add a signal
 
-    """
+    return ex, exl
+
+
+def check_isotope_effects(
+    f_m: str,
+    c: Connection | Connect,
+    icl: dict,
+    ind3: str,
+    ind2: str,
+) -> str:
+    """Test if the connection involves any isotope effects
 
-    ex = f"{flux.full_name}.rate"
-    ex = check_signal_2(ex, c)
-    # ex = ex + "  # fixed rate"
+    :param f_m: string with the flux name
+    :param c: connection object
+    :param icl: dict of reservoirs that have actual fluxes
+    :param ind2: indent 2 times
+    :param ind3: indent 3 times
 
+    :returns eq: equation string
+    """
     if c.isotopes:
-        # r, d and a are typically only a few decimal places so we use them
-        # directly
+        r = c.source.species.r
+        s_c = get_ic(c.source, icl)
+        s_l = get_ic(c.source, icl, isotopes=True)
+        """ Calculate the flux of the light isotope (f_l) as a function of the isotope
+        ratios in the source reservoir soncentrations (s_c, s_l), and alpha (a) as
+        f_l = f_m * 1000/(r * (d + 1000) + 1000)
+
+        Note that the scale has already been applaied to f_m in the calling function.
+        """
         if c.delta != "None":
-            r = c.species.r
             d = c.delta
-            exl = (
-                f"(\n",
-                f"{ind3}{ex} * 1e3\n",
-                f"{ind3}/({r} * ({d} + 1000) + 1000)",
-                f"{ind2})",
-            )
+            # print(f"c-name = {c.name}, d= {d:.2f}")
+            eq = f"{f_m} * 1000 / ({r} * ({d} + 1000) + 1000)"
         elif c.alpha != "None":
-            if c.alpha > 1.1 or c.alpha < 0.9:
-                raise ValueError(
-                    "alpha needs to be given as fractional value not in permil"
-                )
-            r = c.species.r
-            a = c.alpha
-            s_c = get_ic(c.source, icl)
-            s_l = get_ic(c.source, icl, isotopes=True)
-
-            exl = (
-                f"(\n",
-                f"{ind3} - {s_l} * {s_c}\n",
-                f"{ind3}/({a} * {s_l} - {a} * {s_c} - {s_l})",
-                f"{ind2})",
-            )
+            a = c.alpha / 1000 + 1
+            eq = f"{s_l} * {f_m} / ({a} * {s_c} + {s_l} - {a} * {s_l})"
         else:
-            raise ValueError(
-                "A regular flux in an isotope system must specify"
-                "either delta, or alpha. Otherwise use a connection"
-                "that depends on the upstream reservoir delta, or"
-                "set the isotope flag to False"
-            )
-        # this will probably not work
-        exl = check_signal_2(exl, c)
-
+            eq = f"{f_m} * {s_l} / {s_c}"
     else:
-        exl = ""
+        eq = ""
 
-    return ex, exl
+    return eq
 
 
-def get_scale_with_concentration(
+def get_scale_with_concentration_eq(
     flux: Flux,  # flux instance
-    c: Connect,  # connection instance
+    c: Connect | Connection,  # connection instance
     cfn: str,  # full name of the connection instance
-    icl: list,  # list of initial conditions
+    icl: dict,  # list of initial conditions
+    ind2: str,  # whitespace
+    ind3: str,  # whitespace
 ) -> tuple(str, str):
-    """Equation defining a flux that scales with the concentration in the upstream
-    reservoir
+    """Create equation string defining a flux that scales with the
+    concentration in the upstream reservoir
 
-    Example:
+    Example: M1_CG_D_b_to_L_b_TA_thc__F =
+    M1.CG_D_b_to_L_b.TA_thc.scale * R[5]
 
-    M1_CG_D_b_to_L_b_TA_thc__F = M1.CG_D_b_to_L_b.TA_thc.scale * R[5]
+    :param flux: Flux object
+    :param c: connection instance
+    :param cfn: full name of the connection instance
+    :param icl: dict[Reservoir, list[int, int]] where reservoir
+        indicates the reservoir handle, and the list contains the
+        index into the reservoir data.  list[0] = concentration
+        list[1] concentration of the light isotope.
+
+    :returns: two strings with the respective equations for the change
+              in the total reservoir concentration and the
+              concentration of the light isotope
     """
-
     s_c = get_ic(c.source, icl)  # get index to concentration
     ex = f"{cfn}.scale * {s_c}"  # {c.id} scale with conc in {c.source.full_name}"
-    ex = check_signal_2(ex, c)
-    # ex = ex + "  # scale with concentration"
-
-    if c.isotopes:
-        # get c of light isotope in source
-        s_l = get_ic(c.source, icl, isotopes=True)  # R[x]
-        exl = f"{cfn}.scale * {s_l}"
-        exl = check_signal_2(exl, c)
-    else:
-        exl = ""
-
-    return ex, exl
-
-
-def get_scale_with_mass(
-    flux: Flux,  # flux instance
-    c: Connect,  # connection instance
-    cfn: str,  # full name of the connection instance
-    icl: list,  # list of initial conditions
-) -> tuple(str, str):
-    """Equation defining a flux that scales with the concentration in the upstream
-    reservoir
-
-    Example:
-
-    M1_CG_D_b_to_L_b_TA_thc__F = M1.CG_D_b_to_L_b.TA_thc.scale * R[5]
-    """
-
-    s_c = get_ic(c.source, icl)  # get index to concentration
-    ex = f"{cfn}.scale * {c.source.full_name}.volume * {s_c}"
-    ex = check_signal_2(ex, c)
-    # ex = ex + "  # scale with mass"
-    if c.isotopes:
-        s_l = get_ic(c.source, icl, isotopes=True)  # get index to concentration
-        exl = f"{cfn}.scale * {c.source.full_name}.volume * {s_l}"
-        exl = check_signal_2(exl, c)
-    else:
-        exl = ""
-
+    exl = check_isotope_effects(ex, c, icl, ind3, ind2)
+    ex, exl = check_signal_2(ex, exl, c)
     return ex, exl
 
 
-def get_scale_with_flux(
+def get_scale_with_flux_eq(
     flux: Flux,  # flux instance
-    c: Connect,  # connection instance
+    c: Connect | Connection,  # connection instance
     cfn: str,  # full name of the connection instance
-    icl: list,  # list of initial conditions
+    icl: dict,  # list of initial conditions
+    ind2: str,  # indentation
+    ind3: str,  # indentation
 ) -> tuple(str, str):
-    """Equation defining a flux that scales with strength of another flux
-    reservoir
-
-    Example:
+    """Equation defining a flux that scales with strength of another
+    flux. If isotopes are used, use the isotope ratio of the upstream reservoir.
 
-    M1_C_Fw_to_L_b_TA_wca_ta__F = M1.C_Fw_to_L_b_TA_wca_ta.scale * M1_C_Fw_to_L_b_DIC_Ca_W__F
+    :param flux: Flux object
+    :param c: connection instance
+    :param cfn: full name of the connection instance
+    :param icl: dict[Reservoir, list[int, int]] where reservoir
+        indicates the reservoir handle, and the list contains the
+        index into the reservoir data.  list[0] = concentration
+        list[1] concentration of the light isotope.
+
+    :returns: two strings with the respective equations for the change
+              in the total reservoir concentration and the
+              concentration of the light isotope
     """
 
+    # get the reference flux name
     p = flux.parent.ref_flux.parent
-    ex = f"{cfn}.scale * {p.full_name.replace('.', '_')}__F"
-    ex = check_signal_2(ex, c)
-    # ex = ex + "  # scale with flux"
-
-    if c.isotopes:
-        exl = f"{cfn}.scale * {p.full_name.replace('.', '_')}__F_l"
-        exl = check_signal_2(exl, c)
-    else:
-        exl = ""
-
+    fn = f"{p.full_name.replace('.', '_')}__F"
+    # get the equation string for the flux
+    ex = f"{cfn}.scale * {fn}"
+    """ The flux for the light isotope will computed as follows:
+    We will use the mass of the flux we or scaling, but that we will set the
+    delta|alpha according to isotope ratio of the reference flux
+    """
+    exl = check_isotope_effects(ex, c, icl, ind3, ind2)
+    ex, exl = check_signal_2(ex, exl, c)
     return ex, exl
 
 
-def get_weathering(
+def get_weathering_eq(
     flux: Flux,  # flux instance
-    c: Connect,  # connection instance
+    c: Connect | Connection,  # connection instance
     cfn: str,  # full name of the connection instance
-    icl: list,  # list of initial conditions
+    icl: dict,  # list of initial conditions
     ind2: str,
     ind3: str,
 ) -> tuple(str, str):
     """Equation defining a flux that scales with the concentration of pcO2
 
     F = F_0 (pcO2/pCO2_0) * c, see Zeebe, 2012, doi:10.5194/gmd-5-149-2012
 
@@ -612,67 +717,101 @@
      M1_C_Fw_to_L_b_DIC_Ca_W__F = (
             M1.C_Fw_to_L_b_DIC_Ca_W.rate
             * M1.C_Fw_to_L_b_DIC_Ca_W.scale
             * (R[10]/M1.C_Fw_to_L_b_DIC_Ca_W.pco2_0)
             **  M1.C_Fw_to_L_b_DIC_Ca_W.ex
         )
 
+    :param flux: Flux object
+    :param c: connection instance
+    :param cfn: full name of the connection instance
+    :param icl: dict[Reservoir, list[int, int]] where reservoir
+        indicates the reservoir handle, and the list contains the
+        index into the reservoir data.  list[0] = concentration
+        list[1] concentration of the light isotope.
+
+    :returns: two strings with the respective equations for the change
+              in the total reservoir concentration and the
+              concentration of the light isotope
+
     """
 
+    from esbmtk import Source, Sink
+
     s_c = get_ic(c.reservoir_ref, icl)
     ex = (
         f"(\n{ind3}{cfn}.rate\n"
         f"{ind3}* {cfn}.scale\n"
         f"{ind3}* ({s_c}/{cfn}.pco2_0)\n"
         f"{ind3}**  {cfn}.ex\n"
         f"{ind2})"
     )
-    ex = check_signal_2(ex, c)
-    ex = ex + "  # weathering\n"
 
     if c.isotopes:
         # get isotope ratio of source
-        s_c = get_ic(c.source, icl)  # get index to concentration
-        s_l = get_ic(c.source, icl, isotopes=True)  # get index to concentration l
+        if isinstance(c.source, (Source, Sink)):
+            s_c = f"{c.source.full_name}.c"
+            s_l = f"{c.source.full_name}.l"
+        else:
+            s_c = get_ic(c.source, icl)  # get index to concentration
+            s_l = get_ic(c.source, icl, isotopes=True)  # get index to concentration l
+
         fn = flux.full_name.replace(".", "_")
-        exl = f"{fn} * {s_l}/{s_c}"
+        exl = f"{fn} * {s_l} / {s_c}"
+        exl = f"{exl}  # weathering + isotopes"
     else:
         exl = ""
 
+    ex, exl = check_signal_2(ex, exl, c)
+
     return ex, exl
 
 
-def get_gas_exchange(
+def get_gas_exchange_eq(
     flux: Flux,  # flux instance
     c: Connect,  # connection instance
     cfn: str,  # full name of the connection instance
-    icl: list,  # list of initial conditions
+    icl: dict,  # list of initial conditions
     ind2: str,
     ind3: str,
-) -> tuple(str, str):
+) -> str:
     """Equation defining a flux that scales with the concentration of
     of the gas in the atmosphere versus the concentration of the gas
-    in solution. See Zeebe, 2012, doi:10.5194/gmd-5-149-2012
+    in solution.  See Zeebe, 2012, doi:10.5194/gmd-5-149-2012
+
+    ..Example::
 
-    M1_C_H_b_to_CO2_At_gex_hb_F = gas_exchange_ode(
-            M1.C_H_b_to_CO2_At.scale,
-            R[10],  # pco2 in atmosphere
-            M1.C_H_b_to_CO2_At.water_vapor_pressure,
-            M1.C_H_b_to_CO2_At.solubility,
-            M1_H_b_CO2aq, # [co2]aq
-            )  # gas_exchange
+        M1_C_H_b_to_CO2_At_gex_hb_F = gas_exchange_ode(
+             M1.C_H_b_to_CO2_At.scale,
+             R[10],  # pco2 in atmosphere
+             M1.C_H_b_to_CO2_At.water_vapor_pressure,
+             M1.C_H_b_to_CO2_At.solubility,
+             M1_H_b_CO2aq, # [co2]aq
+         )  # gas_exchange
+
+    :param flux: Flux object
+    :param c: connection instance
+    :param cfn: full name of the connection instance
+    :param icl: dict[Reservoir, list[int, int]] where reservoir
+        indicates the reservoir handle, and the list contains the
+        index into the reservoir data.  list[0] = concentration
+        list[1] concentration of the light isotope.
 
+    :returns: string with the gas exchange equation
     """
 
     # get co2_aq reference
     lrn = f"{c.liquid_reservoir.full_name}"
     sp = lrn.split(".")[-1]
     # test if we refer to CO2 or other gas species
     if sp == "DIC":
+        # here we reference the dyanamically calculated CO2aq from cs1,
+        # and not the vector field of cs1
         refsp = f"{c.liquid_reservoir.parent.full_name}.CO2aq".replace(".", "_")
+        # refsp = f"{c.liquid_reservoir.parent.full_name}.CO2aq"
     elif sp == "O2":
         s_c = get_ic(c.liquid_reservoir, icl)
         refsp = f"{s_c}"
     else:
         raise ValueError(f"Species{sp} has not definition for gex")
 
     # get atmosphere pcO2 reference
@@ -682,84 +821,92 @@
         f"{ind3}{cfn}.scale,\n"
         f"{ind3}{pco2},\n"
         f"{ind3}{cfn}.water_vapor_pressure,\n"
         f"{ind3}{cfn}.solubility,\n"
         f"{ind3}{refsp},\n"
         f"{ind2})"
     )
-    ex = check_signal_2(ex, c)
+    ex, exl = check_signal_2(ex, "", c)
     ex = ex + "  # gas_exchange\n"
 
     return ex
 
 
-def get_gas_exchange_w_isotopes(
+def get_gas_exchange_w_isotopes_eq(
     flux: Flux,  # flux instance
-    c: Connect,  # connection instance
+    c: Connect | Connection,  # connection instance
     cfn: str,  # full name of the connection instance
-    icl: list,  # list of initial conditions
+    icl: dict,  # list of initial conditions
     ind2: str,
     ind3: str,
 ) -> tuple(str, str):
     """Equation defining a flux that scales with the concentration of
     of the gas in the atmosphere versus the concentration of the gas
-    in solution. See Zeebe, 2012, doi:10.5194/gmd-5-149-2012
+    in solution.  See Zeebe, 2012, doi:10.5194/gmd-5-149-2012
 
-    M1_C_H_b_to_CO2_At_gex_hb_F, M1_C_H_b_to_CO2_At_gex_hb_F_l  = gas_exchange_ode(
-            M1.C_H_b_to_CO2_At.scale, # surface area in m^2
-            R[10],  # gas c in atmosphere
-            R[11],  # gas c_l in atmosphere
-            R[12],  # c of reference species, e.g., DIC
-            R[13],  # c_l reference species, e.g., DIC_12
-            M1.C_H_b_to_CO2_At.water_vapor_pressure,
-            M1.C_H_b_to_CO2_At.solubility,
-            M1_H_b_CO2aq, # gas concentration in liquid, e.g., [co2]aq
-            a_db,  # fractionation factor between dissolved CO2aq and HCO3-
-            a_gb,  # fractionation between CO2g HCO3-
-            )  # gas_exchange
+    ..Example::
 
-     source_l = get_ic(sb_DIC, icl, isotopes=True)
+        M1_C_H_b_to_CO2_At_gex_hb_F, M1_C_H_b_to_CO2_At_gex_hb_F_l  = gas_exchange_ode(
+           M1.C_H_b_to_CO2_At.scale, # surface area in m^2
+           R[10],  # gas c in atmosphere
+           R[11],  # gas c_l in atmosphere
+           R[12],  # c of main species, e.g., DIC
+           R[13],  # c_l of main species, e.g., DIC_12
+           M1.C_H_b_to_CO2_At.water_vapor_pressure,
+           M1.C_H_b_to_CO2_At.solubility,
+           M1_H_b_CO2aq, # gas concentration in liquid, e.g., [co2]aq
+           a_db,  # fractionation factor between dissolved CO2aq and HCO3-
+           a_gb,  # fractionation between CO2g HCO3-
+        )  # gas_exchange
+
+    :param flux: Flux object
+    :param c: connection instance
+    :param cfn: full name of the connection instance
+    :param icl: dict[Reservoir, list[int, int]] where reservoir
+        indicates the reservoir handle, and the list contains the
+        index into the reservoir data.  list[0] = concentration
+        list[1] concentration of the light isotope.
+
+    :returns: string with the gas exchange equation for the light
+              isotope
     """
 
     # get isotope data
     pco2 = get_ic(c.gas_reservoir, icl)
     pco2_l = get_ic(c.gas_reservoir, icl, isotopes=True)
     dic = get_ic(c.liquid_reservoir, icl)
     dic_l = get_ic(c.liquid_reservoir, icl, isotopes=True)
 
-    # get fractionation factors
-    swc = getattr(c.liquid_reservoir.parent, "swc")
-    a_db = swc.a_db  # fractionation factor between CO2aq and HCO3-
-    a_dg = swc.a_dg  # fractionation between CO2aq and CO2g
-    a_u = swc.a_u  # kinetic fractionation during gas exchange
+    a_db = f"{c.liquid_reservoir.parent.full_name}.swc.a_db"
+    a_dg = f"{c.liquid_reservoir.parent.full_name}.swc.a_dg"
+    a_u = f"{c.liquid_reservoir.parent.full_name}.swc.a_u"
 
     # get co2_aq reference
     lrn = f"{c.liquid_reservoir.full_name}"
     sp = lrn.split(".")[-1]
     # test if we refer to CO2 or other gas species
     if sp == "DIC":
+        # here we reference the dyanamically calculated CO2aq from cs1,
+        # and not the vector field of cs1
         refsp = f"{c.liquid_reservoir.parent.full_name}.CO2aq".replace(".", "_")
-    elif sp == "O2":
-        s_c = get_ic(c.liquid_reservoir, icl)
-        refsp = f"{s_c}"
+        # refsp = f"{c.liquid_reservoir.parent.full_name}.CO2aq"
     else:
-        raise ValueError(f"Species{sp} has not definition for gex")
+        raise ValueError(f"Species{sp} has no isotope definition for gas exchange")
 
-    ex, exl = (
+    ex = (
         f"gas_exchange_ode_with_isotopes(\n"
         f"{ind3}{cfn}.scale,\n"  # surface area in m^2
         f"{ind3}{pco2},\n"  # gas c in atmosphere
         f"{ind3}{pco2_l},\n"  # gas c_l in atmosphere
         f"{ind3}{dic},\n"  # c of reference species, e.g., DIC
         f"{ind3}{dic_l},\n"  # c_l reference species, e.g., DIC_12
         f"{ind3}{cfn}.water_vapor_pressure,\n"
         f"{ind3}{cfn}.solubility,\n"
         f"{ind3}{refsp},\n"  # gas concentration in liquid, e.g., [co2]aq
         f"{ind3}{a_db},\n"  # fractionation factor between dissolved CO2aq and HCO3-
         f"{ind3}{a_dg},\n"  # fractionation between CO2aq and CO2g
         f"{ind3}{a_u},\n"  # kinetic fractionation during gas exchange
         f"{ind2})"
     )
-    ex = check_signal_2(ex, c)
     ex = ex + "  # gas_exchange\n"
 
     return ex
```

### Comparing `esbmtk-0.8.0.0/esbmtk/processes-old.py` & `esbmtk-0.9.0.1/esbmtk/processes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-from numbers import Number
-from nptyping import *
-from typing import *
-from numpy import array, set_printoptions, arange, zeros, interp, mean
-from pandas import DataFrame
-from copy import deepcopy, copy
-from time import process_time
-from numba import njit
-from numba.typed import List
-
+from __future__ import annotations
 import numpy as np
-import matplotlib.pyplot as plt
-import pandas as pd
-
-import logging
-import time
-import builtins
+from . import Q_
+from .esbmtk_base import esbmtkBase  # , Reservoir, Flux, Source, Sink
+from .solver import get_l_mass
+import collections as col
 
 np.set_printoptions(precision=4)
-# from .utility_functions import *
-from .esbmtk import esbmtkBase, Reservoir, Flux, Signal, Source, Sink
-from .utility_functions import sort_by_type
-from .solver import get_imass, get_frac, get_delta, get_flux_data
-from . import ureg, Q_
-
 # from .connections import ConnnectionGroup
 
+# if tp.TYPE_CHECKING:
+#     from .esbmtk import Source, Reservoir, Sink, Flux, Model
+#     from .extended_classes import GasReservoir, ReservoirGroup
+#     from .connections import ConnectionGroup
+
 
 class Process(esbmtkBase):
-    """This class defines template for process which acts on one or more
+    """This class defines template for proycess which acts on one or more
     reservoir flux combinations. To use it, you need to create an
     subclass which defines the actual process implementation in their
     call method. See 'PassiveFlux as example'
 
     """
 
-    __slots__ = ("reservoir", "r", "flux", "r", "mo", "direction", "scale")
+    from .esbmtk import Source, Reservoir, Sink, Flux, Model
 
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
+    def __init__(self, **kwargs: dict[str, any]) -> None:
         """
         Create a new process object with a given process type and options
         """
 
         self.__defaultnames__()  # default kwargs names
         self.__initerrormessages__()  # default error messages
         self.bem.update({"rate": "a string"})
         self.bem.update({"scale": "Number or quantity"})
-        self.__validateandregister__(kwargs)  # initialize keyword values
+        self.__initialize_keyword_variables__(kwargs)  # initialize keyword values
 
         self.__postinit__()  # do some housekeeping
-        self.__register_name__()
+        self.parent = self.register
+        self.__register_name_new__()
 
     def __postinit__(self) -> None:
         """Do some housekeeping for the process class"""
 
+        from esbmtk import Reservoir, Model, Flux
+
         # legacy name aliases
         self.n: str = self.name  # display name of species
-        self.r: Reservoir = self.reservoir
+        if "reservoir" in self.kwargs:
+            self.r: Reservoir = self.reservoir
+
+        self.mo: Model = self.model
         self.f: Flux = self.flux
-        self.m: Model = self.r.sp.mo  # the model handle
-        self.mo: Model = self.m
 
         # self.rm0: float = self.r.m[0]  # the initial reservoir mass
-        if isinstance(self.r, Reservoir):
-            self.direction: Dict[Flux, int] = self.r.lio[self.f]
 
+        if "reservoir" in self.kwargs and isinstance(self.r, Reservoir):
+            self.direction: dict[Flux, int] = self.r.lio[self.f]
+
+        self.delta = self.kwargs["delta"] if "delta" in self.kwargs else "None"
         self.__misc_init__()
 
     def __delayed_init__(self) -> None:
         """
         Initialize stuff which is only known after the entire model has been defined.
         This will be executed just before running the model. You need to add the following
         two lines somewhere in the init procedure (preferably by redefining __misc_init__)
@@ -92,53 +86,64 @@
 
     def __defaultnames__(self) -> None:
         """Set up the default names and dicts for the process class. This
         allows us to extend these values without modifying the entire init process
 
         """
 
-        from .connections import ConnectionGroup
-        from esbmtk import Reservoir, ReservoirGroup, Flux, GasReservoir
+        from esbmtk import (
+            Reservoir,
+            ReservoirGroup,
+            Source,
+            Sink,
+            GasReservoir,
+            Flux,
+            ConnectionGroup,
+            Model,
+        )
 
         # provide a dict of known keywords and types
-        self.lkk: Dict[str, any] = {
-            "name":
-            str,
-            "reservoir": (Reservoir, Source, Sink, GasReservoir),
-            "flux":
-            Flux,
-            "rate": (Number, np.float64),
-            "delta": (Number, np.float64),
-            "lt":
-            Flux,
-            "alpha": (Number, np.float64),
-            "scale": (Number, np.float64),
-            "ref_reservoirs": (Flux, Reservoir, GasReservoir, list, str),
-            "register": (
-                str,
-                ConnectionGroup,
-                Reservoir,
-                ReservoirGroup,
-                GasReservoir,
-                Flux,
-            ),
+        self.defaults: dict[str, list[any, tuple]] = {
+            "name": ["None", (str)],
+            "reservoir": ["None", (str, Reservoir, Source, Sink, GasReservoir)],
+            "flux": ["None", (str, Flux)],
+            "ref_flux": ["None", (str, Flux)],
+            "rate": [0, (int, float, np.float64)],
+            "delta": ["None", (int, float, np.float64, str)],
+            "lt": ["None", (Flux)],
+            "alpha": [0, (int, float, np.float64)],
+            "scale": [1, (int, float, np.float64)],
+            "ref_reservoirs": ["None", (Flux, Reservoir, GasReservoir, list, str)],
+            "model": ["None", (str, Model)],
+            "source": ["None", (str, Source, Reservoir, GasReservoir)],
+            "register": [
+                "None",
+                (
+                    str,
+                    ConnectionGroup,
+                    Reservoir,
+                    ReservoirGroup,
+                    GasReservoir,
+                    Flux,
+                    Model,
+                ),
+            ],
         }
 
         # provide a list of absolutely required keywords
-        self.lrk: list[str] = ["name"]
-
-        # list of default values if none provided
-        self.lod: Dict[str, any] = {"scale": 1}
+        self.lrk: list[str] = ["name", "register"]
 
-    def __register__(self, reservoir: Reservoir, flux: Flux) -> None:
+    def __register__(self, reservoir, flux: Flux) -> None:
         """Register the flux/reservoir pair we are acting upon, and register
         the process with the reservoir
 
         """
 
+        from esbmtk import Flux, Reservoir
+
         # register the reservoir flux combination we are acting on
         self.f: Flux = flux
         self.r: Reservoir = reservoir
         # add this process to the list of processes acting on this reservoir
         reservoir.lop.append(self)
         flux.lop.append(self)
         # Add to model flux list
@@ -163,114 +168,60 @@
     function template of a user provided function.
 
     see calc_carbonates in the carbonate chemistry for an example how
     to write a function for this class.
 
     """
 
-    __slots__ = ("function", "input_data", "vr_data", "params")
-
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
+    def __init__(self, **kwargs: dict[str, any]) -> None:
         """
         Create a new process object with a given process type and options
 
         """
 
-        from . import Reservoir_no_set
-
+        from esbmtk import Model, ReservoirGroup
+        from typing import Callable
+        
         self.__defaultnames__()  # default kwargs names
 
         # list of allowed keywords
-        self.lkk: Dict[str, any] = {
-            "name": str,
-            "function": any,
-            "input_data": (List, str),
-            "vr_data": (List, str),
-            "function_params": (List, str),
-            "model": any,
+        defaults: dict[str, list[any, tuple]] = {
+            "function": ["None", (str, Callable)],
+            "input_data": ["None", (list, str)],
+            "vr_data": ["None", (list, str)],
+            "function_params": ["None", (list, str)],
+            "model": ["None", (str, Model)],
+            "ftype": ["None", (str)],
+            "r_s": ["None", (str, ReservoirGroup)],
+            "r_g": ["None", (str, ReservoirGroup)],
         }
 
+        self.defaults.update(defaults)
+        self.__initialize_keyword_variables__(kwargs)
         # required arguments
-        self.lrk: list = [
-            "name", "input_data", "vr_data", "function_params", "model"
-        ]
+        self.lrk: list = ["name", "input_data", "vr_data", "function_params", "model"]
 
-        # list of default values if none provided
-        self.lod: Dict[any, any] = {}
-
-        self.__initerrormessages__()  # default error messages
-        self.bem.update({
-            "function": "a function",
-            "input_data": "list of one or more numpy arrays",
-            "vr_data": "list of one or more numpy arrays",
-            "function_params": "a list of float values",
-        })
-        self.__validateandregister__(kwargs)  # initialize keyword values
         self.mo = self.model
-
-        if not callable(self.function):
-            raise ValueError(
-                "function must be defined before it can be used here")
+        self.parent = self.register
 
         self.__postinit__()  # do some housekeeping
 
         if self.mo.register == "local" and self.register == "None":
             self.register = self.mo
 
-        self.__register_name__()  #
+        self.__register_name_new__()  #
 
     def __call__(self, i: int) -> None:
         """Here we execute the user supplied function
         Where i = index of the current timestep
 
         """
 
         self.function(i, self.input_data, self.vr_data, self.function_params)
 
-    # redefine post init
-    def __postinit__(self) -> None:
-        """Do some housekeeping for the process class"""
-
-        self.__misc_init__()
-
-    def get_process_args(self) -> tuple:
-        """return the data associated with this object"""
-
-        self.func_name: function = self.function
-
-        return (
-            self.func_name,
-            self.input_data,
-            self.vr_data,
-            self.function_params,
-        )
-
-
-class LookupTable(Process):
-    """This process replaces the flux-values with values from a static
-    lookup table
-
-         Example::
-
-         LookupTable("name", upstream_reservoir_handle, lt=flux-object)
-
-         where the flux-object contains the mass, li, hi, and delta values
-         which will replace the current flux values.
-
-    """
-    def __call__(self, i: int) -> None:
-        """Here we replace the flux value with the value from the flux object
-        which we use as a lookup-table
-
-        """
-        self.m[i]: float = self.lt.m[i]
-        self.d[i]: float = self.lt.d[i]
-        self.l[i]: float = self.lt.l[i]
-        self.h[i]: float = self.lt.h[i]
-
 
 class AddSignal(Process):
     """This process adds values to the current flux based on the values provided by the signal object.
     This class is typically invoked through the connector object
 
      Example::
 
@@ -280,975 +231,453 @@
                lt = flux with lookup values)
 
      where - the upstream reservoir is the reservoir the process belongs too
              the flux is the flux to act upon
              lt= contains the flux object we lookup from
 
     """
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
+
+    def __init__(self, **kwargs: dict[str, any]) -> None:
         """
         Create a new process object with a given process type and options
         """
 
         # get default names and update list for this Process
         self.__defaultnames__()  # default kwargs names
         self.lrk.extend(["lt", "flux", "reservoir"])  # new required keywords
-
-        self.__initerrormessages__()
-        # self.bem.update({"rate": "a string"})
-        self.__validateandregister__(kwargs)  # initialize keyword values
+        self.__initialize_keyword_variables__(kwargs)  # initialize keyword values
 
         # legacy variables
         self.mo = self.reservoir.mo
         self.__postinit__()  # do some housekeeping
-        self.__register_name__()
-
-        # decide whichh call function to use
-        # if self.mo.m_type == "both":
+        self.parent = self.register
+        self.__register_name_new__()
 
-        if self.reservoir.isotopes:
-            self.__execute__ = self.__add_with_isotopes__
-        else:
-            self.__execute__ = self.__add_without_isotopes__
+        # defaults
+        self.__execute__ = self.__add_with_fi__
 
     # setup a placeholder call function
     def __call__(self, i: int):
         return self.__execute__(i)
 
     # use this when we do isotopes
-    def __add_with_isotopes__(self, i) -> None:
+    def __add_with_fi__(self, i) -> None:
         """Each process is associated with a flux (self.f). Here we replace
         the flux value with the value from the signal object which
         we use as a lookup-table (self.lt)
 
-        """
-        # add signal mass to flux mass
-
-        self.f.m[i] = self.f.m[i] + self.lt.m[i]
-        self.f.d[i] = self.f.d[i] + self.lt.d[i]
-        if self.f.m[i] != 0:
-            # self.f[i] = self.f[i] + self.lt[i]
-            self.f.l[i], self.f.h[i] = get_imass(self.f.m[i], self.f.d[i],
-                                                 self.r.rvalue)
-        # signals may have zero mass, but may have a delta offset. Thus, we do not know
-        # the masses for the light and heavy isotope. As such we have to calculate the masses
-        # after we add the signal to a flux
-
-    # use this when we do isotopes
-    def __add_without_isotopes__(self, i) -> None:
-        """Each process is associated with a flux (self.f). Here we replace
-        the flux value with the value from the signal object which
-        we use as a lookup-table (self.lt)
+        Note that the signal may also specify a delta value. Thus we
+        need to
+        1) get the mass of flux + signal
+        2) add the delta of flux and signal
+        3) calculate the new li and hi
 
         """
-        # add signal mass to flux mass
-        self.f.m[i] = self.f.m[i] + self.lt.m[i]
-
-    def get_process_args(self):
-
-        func_name: function = self.p_add_signal
 
-        print(f"flux_name = {self.flux.full_name}")
+        # add signal mass to flux mass
+        r = self.f.species.r
+        fm = self.f.m[i]  # flux rate
+        fl = self.f.l[i]  # flux rate light isotope
+        sm = self.lt.m[i]  # signal mass
+        sl = self.lt.l[i]  # signal li
+
+        # get signal delta
+        sd = 1000 * ((sm - sl) / sl - r) / r if sm > 0 else 0
+        # print(f"Signal delta = {sd}")
+
+        fd = 1000 * ((fm - fl) / fl - r) / r + sd if fm > 0 else sd
+        fm += sm  # add signal mass
+        fl = 1000.0 * fm / ((fd + 1000.0) * r + 1000.0)
 
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.lt.m,  # 4
-            self.lt.l,  # 5
-            self.lt.h,  # 6
-            self.lt.d,  # 7
-        ])
+        self.f.fa = np.array([fm, fl])
+        # print(f"fa = {self.f.fa}\n")
 
-        params = List([float(self.reservoir.species.element.r)])
+    def __add_with_fa__(self, i) -> None:
+        """same as above but use fa instead of flux data"""
 
-        return func_name, data, params
+        # add signal mass to flux mass
+        r = self.f.species.r
+        fm = self.f.fa[0]  # flux rate
+        fl = self.f.fa[1]  # flux rate light isotope
+        sm = self.lt.m[i]  # signal mass
+        sl = self.lt.l[i]  # signal li
+
+        # get signal delta
+        sd = 1000 * ((sm - sl) / sl - r) / r
+
+        fd = 1000 * ((fm - fl) / fl - r) / r + sd if fm > 0 else sd
+        # set new flux rate
+        fm += sm  # add signal mass
+        fl = 1000.0 * fm / ((fd + 1000.0) * r + 1000.0)
 
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
-    def p_add_signal(data, params, i) -> None:
+        self.f.fa = np.array([fm, fl])
 
+    def p_add_signal_fi(data, params, i) -> None:
         r: float = params[0]
+        fm: float = data[0][i]  # fm
+        fl: float = data[1][i]  # fl
+        sm: float = data[2][i]  # sm
+        sl: float = data[3][i]  # sd
+
+        # get signal delta
+        sd = 1000 * ((sm - sl) / sl - r) / r if sm > 0 else 0
+        fd = 1000 * ((fm - fl) / fl - r) / r + sd if fm > 0 else sd
+        # set new flux rate
+        fm += sm  # add signal mass
+        fl = 1000.0 * fm / ((fd + 1000.0) * r + 1000.0)
 
-        # flux masses and delta
-        # fm: float = data[0][i]
-        # fl: float = data[1][i]
-        # fh: float = data[2][i]
-        # fd: float = data[3][i]
-
-        # signal masses and delta
-        # sm: float = data[4][i]
-        # sl: float = data[5][i]
-        # sd: float = data[7][i]
-
-        # new masses and delta. Note that signals may have zero mass
-        # but a non-zero delta. So simply adding h and l won't work
-
-        data[0][i] = data[0][i] + data[4][i]
-        data[3][i] = data[3][i] + data[7][i]
-        # fl = (1000.0 * fm) / ((sd + 1000.0) * r + 1000.0)
-        data[1][i] = (1000.0 * data[0][i]) / (
-            (data[3][i] + 1000.0) * r + 1000.0)
-        data[2][i] = data[0][i] - data[1][i]
-
-
-class MultiplySignal(Process):
-    """This process mulitplies a given flux witthe the data in the signal.
-    This class is typically invoked through the connector object:
-
-    Note that this process will not modify the delta value of a given flux.
-    If you needto vary the delta value it is best to add a second signal which uses the
-    add signal type.
-
-     Example::
+        data[4][:] = [fm, fl]
 
-     MultiplySignal(name = "name",
-               reservoir = upstream_reservoir_handle,
-               flux = flux_to_act_upon,
-               lt = flux with lookup values)
+    def p_add_signal_fa(data, params, i) -> None:
+        r: float = params[0]
+        fm: float = data[2][0]
+        fl: float = data[2][1]
+        sm: float = data[0][i]
+        sl: float = data[1][i]
+
+        # get signal delta
+        sd = 1000 * ((sm - sl) / sl - r) / r if sm > 0 else 0
+        fd = 1000 * ((fm - fl) / fl - r) / r + sd if fm > 0 else sd
+        fm += sm  # add signal mass
+        fl = 1000.0 * fm / ((fd + 1000.0) * r + 1000.0)
+        data[2][:] = [fm, fl]
 
-     where - the upstream reservoir is the reservoir the process belongs too
-             the flux is the flux to act upon
-             lt= contains the flux object we lookup from
 
+class SaveFluxData(Process):
     """
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
-        """
-        Create a new process object with a given process type and options
-        """
-
-        # get default names and update list for this Process
-        self.__defaultnames__()  # default kwargs names
-        self.lrk.extend(["lt", "flux", "reservoir"])  # new required keywords
-
-        self.__initerrormessages__()
-        # self.bem.update({"rate": "a string"})
-        self.__validateandregister__(kwargs)  # initialize keyword values
-
-        # legacy variables
-        self.mo = self.reservoir.mo
-        self.__postinit__()  # do some housekeeping
-        self.__register_name__()
-
-        # decide whichh call function to use
-        # if self.mo.m_type == "both":
-
-        if self.reservoir.isotopes:
-            self.__execute__ = self.__multiply_with_isotopes__
-        else:
-            self.__execute__ = self.__multiply_without_isotopes__
-
-    # setup a placeholder call function
-    def __call__(self, i: int):
-        return self.__execute__(i)
-
-    # use this when we do isotopes
-    def __multiply_with_isotopes__(self, i) -> None:
-        """Each process is associated with a flux (self.f). Here we replace
-        the flux value with the value from the signal object which
-        we use as a lookup-table (self.lt)
-        """
-        # multiply flux mass with signal
-        self.f.m[i] = self.f.m[i] * self.lt.m[i]
-        self.f.l[i] = self.f.l[i] * self.lt.m[i]
-        self.f.h[i] = self.f.m[i] - self.f.l[i]
-
-    def __multiply_without_isotopes__(self, i) -> None:
-        """Each process is associated with a flux (self.f). Here we replace
-        the flux value with the value from the signal object which
-        we use as a lookup-table (self.lt)
-
-        """
-        # multiply flux mass with signal
-        self.f.m[i] = self.f.m[i] * self.lt.m[i]
-
-    def get_process_args(self):
-
-        func_name: function = self.p_multiply_signal
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.lt.m,  # 4
-            self.lt.l,  # 5
-            self.lt.h,  # 6
-            self.lt.d,  # 7
-        ])
-        params = List([float(self.reservoir.species.element.r)])
-
-        return func_name, data, params
-
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
-    def p_multiply_signal(data, params, i) -> None:
-
-        # flux masses and delta
-        # fm: float = data[0][i]
-        # fl: float = data[1][i]
-        # fh: float = data[2][i]
-        # fd: float = data[3][i]
-
-        # signal masses and delta
-        # sm: float = data[4][i]
-        # sl: float = data[5][i]
-        # sd: float = data[7][i]
-
-        data[0][i] = data[0][i] * data[4][i]
-        data[1][i] = data[1][i] * data[4][i]
-        data[2][i] = data[0][i] - data[1][i]
-
-
-class PassiveFlux(Process):
-    """This process sets the output flux from a reservoir to be equal to
-    the sum of input fluxes, so that the reservoir concentration does
-    not change. Furthermore, the isotopic ratio of the output flux
-    will be set equal to the isotopic ratio of the reservoir The init
-    and register methods are inherited from the process class. The
-    overall result can be scaled, i.e., in order to create a split flow etc.
+    This process stores the flux data from each iteration into a vector
     Example::
 
-    PassiveFlux(name = "name",
-                reservoir = upstream_reservoir_handle
-                scale = optional
-                flux = flux handle)
-
-    """
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
-        """ Initialize this Process """
-
-        # get default names and update list for this Process
-        self.__defaultnames__()  # default kwargs names
-        self.lrk.extend(["reservoir", "flux"])  # new required keywords
-        self.__initerrormessages__()
-        # self.bem.update({"rate": "a string"})
-        self.__validateandregister__(kwargs)  # initialize keyword values
-        # legacy variables
-        self.mo = self.reservoir.mo
-        self.__postinit__()  # do some housekeeping
-        self.__register_name__()
-
-    def __misc_init__(self) -> None:
-        """This is just a place holder method which will be called by default
-        in __post_init__() This can be overloaded to add additional
-        code to the init procedure without the need to redefine
-        init. This useful for processes which only define a call method.
-
-        """
-
-        # this process requires delayed init.
-        print(f"Added {self.name} to lto")
-        self.mo.lto.append(self)
-
-    def __delayed_init__(self) -> None:
-        """
-        Initialize stuff which is only known after the entire model has been defined.
-        This will be executed just before running the model.
-
-        """
-
-        # Create a list of fluxes wich excludes the flux this process
-        # will be acting upon
-
-        # print(f"delayed init for {self.name}")
-        self.fws: List[Flux] = self.r.lof.copy()
-        self.fws.remove(self.f)  # remove this handle
-
-    def __call__(self, i: int) -> None:
-        """Here we re-balance the flux. That is, we calculate the sum of all fluxes
-        excluding this flux. This sum will be equal to this flux. This will likely only
-        work for outfluxes though.
-
-        Should this be done for output fluxes as well?
-
-        """
-
-        new: float = 0.0
-
-        # calc sum of fluxes in fws. Note that at this point, not all fluxes
-        # will be known so we need to use the flux values from the previous times-step
-        for j, f in enumerate(self.fws):
-            # print(f"{f.n} = {f.m[i-1] * reservoir.lio[f]}")
-            new += f.m[i - 1] * self.reservoir.lio[f] * self.scale
-
-        # print(f"sum = {new:.0f}\n")
-
-        self.f[i] = get_flux_data(new, self.reservoir.d[i - 1],
-                                  self.reservoir.rvalue)
-
-
-class ScaleRelativeToInputFluxes(PassiveFlux):
-    """Scale output flux relative to the input fluxes"""
-    def __delayed_init__(self) -> None:
-        """
-        Initialize stuff which is only known after the entire model has been defined.
-        This will be executed just before running the model.
-
-        Specifically, find all input fluxes
-        """
-
-        print(f"delayed init for {self.name}")
-
-        self.in_fluxes: list = []
-        for i, f in enumerate(self.r.lof):
-            if self.r.lodir[i] > 0:
-                self.in_fluxes.append(f)
-
-    def __call__(self, i: int) -> None:
-        """Here we re-balance the flux. That is, we calculate the sum of all fluxes
-        excluding this flux. This sum will be equal to this flux. This will likely only
-        work for outfluxes though.
-
-        Should this be done for output fluxes as well?
-
-        """
-
-        new: float = 0.0
-
-        for j, f in enumerate(self.in_fluxes):
-            # print(f"{f.n} = {f.m[i-1] * reservoir.lio[f]}")
-            new += f.m[i - 1]
-
-        new = new * self.scale
-        # print(f"sum = {new:.0f}\n")
-        self.f[i] = [new, 1, 1, 1]
-
-
-class PassiveFlux_fixed_delta(Process):
-    """This process sets the output flux from a reservoir to be equal to
-    the sum of input fluxes, so that the reservoir concentration does
-    not change. However, the isotopic ratio of the output flux is set
-    at a fixed value. The init and register methods are inherited
-    from the process class. The overall result can be scaled, i.e.,
-    in order to create a split flow etc.  Example::
-
-    PassiveFlux_fixed_delta(name = "name",
-                            reservoir = upstream_reservoir_handle,
-                            flux handle,
-                            delta = delta offset)
-
-    """
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
-        """ Initialize this Process """
-
-        self.__defaultnames__()  # default kwargs names
-        self.lrk.extend(["reservoir", "delta",
-                         "flux"])  # new required keywords
-
-        self.__initerrormessages__()
-        # self.bem.update({"rate": "a string"})
-        self.__validateandregister__(kwargs)  # initialize keyword values
-        self.__postinit__()  # do some housekeeping
-
-        # legacy names
-        self.f: Flux = self.flux
-        # legacy variables
-        self.mo = self.reservoir.mo
-
-        print(
-            "\nn *** Warning, you selected the PassiveFlux_fixed_delta method ***\n "
-        )
-        print(
-            " This is not a particularly phyiscal process is this really what you want?\n"
-        )
-        print(self.__doc__)
-        self.__register_name__()
-
-    def __call__(self, i: int) -> None:
-        """Here we re-balance the flux. This code will be called by the
-        apply_flux_modifier method of a reservoir which itself is
-        called by the model execute method
-
-        """
-
-        r: float = self.reservoir.rvalue  # the isotope reference value
-
-        varflux: Flux = self.f
-        flux_list: List[Flux] = self.reservoir.lof.copy()
-        flux_list.remove(varflux)  # remove this handle
-
-        # sum up the remaining fluxes
-        newflux: float = 0
-        for f in flux_list:
-            newflux = newflux + f.m[i - 1] * self.reservoir.lio[f]
-
-        # set isotope mass according to keyword value
-        self.f[i] = np.array(get_flux_data(newflux, self.delta, r))
-
-
-class VarDeltaOut(Process):
-    """Unlike a passive flux, this process sets the flux istope ratio
-    equal to the isotopic ratio of the reservoir. The
-    init and register methods are inherited from the process
-    class.
-
-    VarDeltaOut(name = "name",
-                reservoir = upstream_reservoir_handle,
-                flux = flux handle,
-                rate = rate,)
-
-    """
-
-    __slots__ = ("rate", "flux", "reservoir")
-
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
-        """Initialize this Process"""
-
-        from . import ureg, Q_
-        from .connections import ConnectionGroup
-        from esbmtk import Flux, Reservoir, ReservoirGroup
-
-        # get default names and update list for this Process
-        self.__defaultnames__()
-        self.lkk: Dict[str, any] = {
-            "name": str,
-            "reservoir": (Reservoir, Source, Sink),
-            "flux": Flux,
-            "rate": (str, Q_),
-            "register":
-            (ConnectionGroup, ReservoirGroup, Reservoir, Flux, str),
-            "scale": (Number, np.float64, str),
-        }
-        self.lrk.extend(["reservoir", "flux"])  # new required keywords
-        self.__initerrormessages__()
-        self.__validateandregister__(kwargs)  # initialize keyword values
-        self.mo = self.reservoir.mo
-        self.__postinit__()  # do some housekeeping
-        self.__register_name__()
-
-        # decide which call function to use
-        # if self.mo.m_type == "both":
-        if self.reservoir.isotopes:
-            # print(
-            #    f"vardeltaout with isotopes for {self.reservoir.register.name}.{self.reservoir.name}"
-            # )
-            if isinstance(self.reservoir, Reservoir):
-                # print("Using reservoir")
-                self.__execute__ = self.__with_isotopes_reservoir__
-            elif isinstance(self.reservoir, Source):
-                # print("Using Source")
-                self.__execute__ = self.__with_isotopes_source__
-            else:
-                raise ValueError(
-                    f"{self.name}, reservoir must be of type Source or Reservoir, not {type(self.reservoir)}"
-                )
-        else:
-            self.__execute__ = self.__without_isotopes__
-
-    # setup a placeholder call function
-    def __call__(self, i: int):
-        return self.__execute__(i)
-
-    def __with_isotopes_reservoir__(self, i: int) -> None:
-        """Here we re-balance the flux. This code will be called by the
-        apply_flux_modifier method of a reservoir which itself is
-        called by the model execute method
-
-        """
-
-        m: float = self.flux.m[i]
-        if m != 0:
-            # if reservoir.register.name == "db":
-            #    print(f"{reservoir.name} d={reservoir.d[i-1]}")
-            r: float = self.reservoir.species.element.r
-            d: float = self.reservoir.d[i - 1]
-            l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-            h: float = m - l
-
-            self.flux[i] = [m, l, h, d]
-
-    def get_process_args(self):
-        """Provide the data structure which needs to be passed to the numba solver"""
-
-        # if upstream is a source, we only have a single delta value
-        # so we need to patch this. Maybe this should move to source?
-        if isinstance(self.reservoir, Source):
-            delta = self.reservoir.d
-        else:
-            delta = self.reservoir.d
-
-        func_name: function = self.p_vardeltaout
-
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            delta,  # 4
-        ])
-
-        params = List([float(reservoir.species.element.r)])
-
-        return func_name, data, params
-
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
-    def p_vardeltaout(data, params, i) -> None:
-        # concentration times scale factor
-
-        r: float = params[0]  # r-value
-        m: float = data[0][i - 1]  # flux mass
-        d: float = data[4][i - 1]  # reservoir delta
-        l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-
-        data[0][i] = m
-        data[1][i] = l
-        data[2][i] = m - l
-        data[3][i] = d
-
-    def __with_isotopes_source__(self, i: int) -> None:
-        """If the source of the flux is a source, there is only a single delta value.
-        Changes to the flux delta are applied through the Signal class.
-
-        """
-
-        m: float = self.flux.m[i]
-        if m != 0:
-            d: float = self.reservoir.delta
-            r: float = self.reservoir.species.element.r
-            l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-            h: float = m - l
-
-            self.flux[i] = [m, l, h, d]
-
-    def __without_isotopes__(self, i: int) -> None:
-        """Here we re-balance the flux. This code will be called by the
-        apply_flux_modifier method of a reservoir which itself is
-        called by the model execute method
-
-        """
-
-        pass
-
-
-class SaveFluxData(Process):
-    """This process scales the mass of a flux (m,l,h) relative to another
-    flux but does not affect delta. The scale factor "scale" and flux
-    reference must be present when the object is being initalized
-
-    Example::
-         ScaleFlux(name = "Name",
-                   flux = Flux Handle)
+         SaveFluxData(name = "Name",
+                   flux = Flux Handle
+    )
 
     """
 
-    __slots__ = ("flux")
-
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
+    def __init__(self, **kwargs: dict[str, any]) -> None:
         """Initialize this Process"""
         # get default names and update list for this Process
         self.__defaultnames__()  # default kwargs names
         self.lrk.extend(["flux"])  # new required keywords
 
-        self.__validateandregister__(kwargs)  # initialize keyword values
+        self.__initialize_keyword_variables__(kwargs)  # initialize keyword values
 
         # legacy variables
+        self.parent = self.register
         self.__postinit__()  # do some housekeeping
-        self.__register_name__()
+        self.__register_name_new__()
 
     # setup a placeholder call function
     def __call__(self, i: int):
-        self.f[i] = self.fa
-
-    def get_process_args(self):
-        """"""
-
-        func_name: function = self.p_save_flux
-
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.fa,  # 4
-        ])
-
-        params = List()
-
-        return func_name, data, params
-
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
-    def p_scale_flux(data, params, i) -> None:
-
-        r: float = params[0]  # r value
-        s: float = params[1]  # scale
+        self.f[i] = self.f.fa
 
-        m: float = data[4][i]  # mass of reference object
-        d: float = data[5][i - 1]  # delta of reservoir_ref
-
-        m = m * s
-        l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-        # print(f"ScaleFlux m = {m:.2e}, scale = {proc_const[1]}")
-
-        data[0][i] = data[4][0]
-        data[1][i] = data[4][1]
-        data[2][i] = data[4][2]
-        data[3][i] = data[4][3]
+    def p_save_flux(data, params, i) -> None:
+        data[0][i] = data[2][0]
+        data[1][i] = data[2][1]
 
 
 class ScaleFlux(Process):
-    """This process scales the mass of a flux (m,l,h) relative to another
-    flux but does not affect delta. The scale factor "scale" and flux
+    """This process scales the mass of a flux (m,l,h) relative to
+    another flux. Delta is either taken from the upstream reservoir
+    or set to a fixed value.  The scale factor "scale" and flux
     reference must be present when the object is being initalized
 
     Example::
          ScaleFlux(name = "Name",
                    reservoir = reservoir_handle (upstream or downstream)
                    scale = 1
-                   ref_reservoirs = flux we use for scale)
+                   ref_flux = flux we use for scale
+                   )
 
     """
 
-    __slots__ = ("rate", "scale", "ref_reservoirs", "reservoir", "flux")
-
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
+    def __init__(self, **kwargs: dict[str, any]) -> None:
         """Initialize this Process"""
+
+        from esbmtk import Source
+
         # get default names and update list for this Process
         self.__defaultnames__()  # default kwargs names
-        self.lrk.extend(["reservoir", "flux", "scale",
-                         "ref_reservoirs"])  # new required keywords
+        self.lrk.extend(["reservoir", "flux", "scale"])  # new required keywords
+        self.__initialize_keyword_variables__(kwargs)  # initialize keyword values
 
-        self.__validateandregister__(kwargs)  # initialize keyword values
+        if "ref_reservoirs" in kwargs:
+            self.ref_flux = kwargs["ref_reservoirs"]
+        elif "ref_flux" not in kwargs:
+            raise ValueError("You need to specify a value for ref_flux")
 
         # legacy variables
         self.mo = self.reservoir.mo
         self.__postinit__()  # do some housekeeping
-        self.__register_name__()
-
-        if self.ref_reservoirs == "None":
-            raise ValueError("You need reference to scale against")
+        self.parent = self.register
+        self.__register_name_new__()
 
-        # decide which call function to use
-        # if self.mo.m_type == "both":
-        if self.reservoir.isotopes:
+        """ Decide how to calculate isotopes (if)
+        If the connection specifies delta explicitly, this will
+        override any settings in the source.
+        """
+        self.c = 1
+        if self.delta != "None":
+            # delta explicitly provided
+            l = get_l_mass(1, self.delta, self.reservoir.species.element.r)
+            self.c = l / (1 - l)
+            self.__execute__ = self.__with_fixed_delta__
+        elif isinstance(self.source, Source):
+            if self.source.delta != "None":
+                self.delta = self.source.delta
+                l = get_l_mass(1, self.delta, self.reservoir.species.element.r)
+                self.c = l / (1 - l)
+                self.__execute__ = self.__with_fixed_delta__
+            else:
+                self.__execute__ = self.__without_isotopes__
+        elif self.source.isotopes:
             self.__execute__ = self.__with_isotopes__
         else:
             self.__execute__ = self.__without_isotopes__
 
+    # create stubs
+    def __with_source__():
+        raise NotImplementedError()
+
     # setup a placeholder call function
     def __call__(self, i: int):
         return self.__execute__(i)
 
     def __with_isotopes__(self, i: int) -> None:
         """Apply the scale factor. This is typically done through the the
         model execute method.
-        Note that this will use the mass of the reference object, but that we will set the
-        delta according to the reservoir
+        Note that this will use the mass of the flux we use for scaling, but that we will set the
+        delta according to reservoir this flux derives from
 
         """
 
-        m: float = self.ref_reservoirs.m[i] * self.scale
-        r: float = self.reservoir.species.element.r
-        d: float = self.reservoir.d[i - 1]
-        l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-
-        self.flux[i]: np.array = [m, l, m - l, d]
-
-    def __without_isotopes__(self, i: int) -> None:
-        """Apply the scale factor. This is typically done through the the
-        model execute method.
-        Note that this will use the mass of the reference object, but that we will set the
-        delta according to the reservoir (or the flux?)
+        # get reference flux
+        rm: float = self.ref_flux.fa[0] * self.scale
 
-        """
+        # get the target isotope ratio based on upstream delta
+        c = self.reservoir.l[i - 1] / (
+            self.reservoir.c[i - 1] - self.reservoir.l[i - 1]
+        )
 
-        self.f[i] = self.ref_reservoirs[i] * self.scale
+        fl: float = rm * c / (c + 1)
 
-    def get_process_args(self):
-        """"""
+        self.flux.fa[:] = [rm, fl]
 
-        func_name: function = self.p_scale_flux
+    def __with_fixed_delta__(self, i: int) -> None:
+        """similar to with isotopes, but this time we take the
+        isotope value of the source (which has no array, just a fixed
+        value"""
 
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.ref_reservoirs.m,  # 4
-            self.reservoir.d,  # 5
-        ])
+        # get reference flux
+        rm: float = self.ref_flux.fa[0] * self.scale
 
-        params = List(
-            [float(self.reservoir.species.element.r),
-             float(self.scale)])
+        # get the target isotope ratio based on upstream delta
+        c = self.c
 
-        return func_name, data, params
+        fl: float = rm * c / (c + 1)
 
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
-    def p_scale_flux(data, params, i) -> None:
+        self.flux.fa[:] = [rm, fl]
 
-        r: float = params[0]  # r value
-        s: float = params[1]  # scale
+    def __without_isotopes__(self, i: int) -> None:
+        """Apply the scale factor. This is typically done through the the
+        model execute method.
+        Note that this will use the mass of the reference object, but that we will set the
+        delta according to the reservoir (or the flux?)
 
-        m: float = data[4][i]  # mass of reference object
-        d: float = data[5][i - 1]  # delta of reservoir_ref
+        """
 
-        m = m * s
-        l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-        # print(f"ScaleFlux m = {m:.2e}, scale = {proc_const[1]}")
-
-        data[0][i] = m
-        data[1][i] = l
-        data[2][i] = m - l
-        data[3][i] = d
-
-
-class Reaction(ScaleFlux):
-    """This process approximates the effect of a chemical reaction between
-    two fluxes which belong to a differents species (e.g., S, and O).
-    The flux belonging to the upstream reservoir will simply be
-    scaled relative to the flux it reacts with. The scaling is given
-    by the ratio argument. So this function is equivalent to the
-    ScaleFlux class.
+        self.f.fa = np.array(
+            [
+                self.ref_flux.fa[0] * self.scale,
+                0,
+            ]
+        )
 
-    Example::
-
-       Connect(source=IW_H2S,
-               sink=S0,
-               ctype = "react_with",
-               scale=1,
-               ref_reservoirs = O2_diff_to_S0,
-               scale =1,
-       )
-    """
+    def p_scale_flux_r(data, params, i) -> None:
+        """delta is derived from upstream reservoir"""
 
+        # params
+        s: float = params[1]  # scale
 
-class FluxDiff(Process):
-    """The new flux will be the difference of two fluxes"""
-    """This process scales the mass of a flux (m,l,h) relative to another
-     flux but does not affect delta. The scale factor "scale" and flux
-     reference must be present when the object is being initalized
+        # data
+        mf: float = data[6][0] * s  # mass of reference flux
+        mr: float = data[3][i - 1]  # mass upstream reservoir
+        lr: float = data[4][i - 1]  # li upstream reservoir
+
+        # get the target isotope ratio based on upstream delta
+        c = lr / (mr - lr)
+        l = mf * c / (c + 1)
 
-     Example::
-          ScaleFlux(name = "Name",
-                    reservoir = upstream_reservoir_handle,
-                    scale = 1
-                    ref_reservoirs = flux we use for scale)
+        data[5][:] = [mf, l]
 
-     """
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
-        """Initialize this Process"""
-        # get default names and update list for this Process
-        self.__defaultnames__()  # default kwargs names
-        self.lrk.extend(["reservoir", "flux", "scale",
-                         "ref_reservoirs"])  # new required keywords
+    def p_scale_flux_fd(data, params, i) -> None:
+        """delta is set to a fixed value"""
 
-        self.__validateandregister__(kwargs)  # initialize keyword values
-        self.__postinit__()  # do some housekeeping
+        # params
+        s: float = params[1]  # scale
+        c: float = params[2]  # l/h ratio
 
-        # legacy variables
-        self.mo = self.reservoir.mo
-        self.__register_name__()
+        # data
+        mf: float = data[6][0] * s  # mass of reference flux
 
-    def __call__(self, i: int) -> None:
-        """Apply the scale factor. This is typically done through the the
-        model execute method.
-        Note that this will use the mass of the reference object, but that we will set the
-        delta according to the reservoir (or the flux?)
+        # get the target isotope ratio based on upstream delta
+        l = mf * c / (c + 1)
 
-        """
-        self.f[i] = (self.ref_reservoirs[0][i] -
-                     self.ref_reservoirs[1][i]) * self.scale
+        data[5][:] = [mf, l]
 
 
 class Fractionation(Process):
     """This process offsets the isotopic ratio of the flux by a given
        delta value. In other words, we add a fractionation factor
 
     Example::
          Fractionation(name = "Name",
                        reservoir = upstream_reservoir_handle,
                        flux = flux handle
                        alpha = 12 in permil (e.f)
 
     """
 
-    __slots__ = ("flux", "reservoir")
-
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
-        """ Initialize this Process """
+    def __init__(self, **kwargs: dict[str, any]) -> None:
+        """Initialize this Process"""
         # get default names and update list for this Process
         self.__defaultnames__()  # default kwargs names
-        self.lrk.extend(["reservoir", "flux",
-                         "alpha"])  # new required keywords
+        self.lrk.extend(["reservoir", "flux", "alpha"])  # new required keywords
 
-        self.__validateandregister__(kwargs)  # initialize keyword values
+        self.__initialize_keyword_variables__(kwargs)  # initialize keyword values
         self.__postinit__()  # do some housekeeping
 
         # alpha is given in permil, but the fractionation routine expects
         # it as 1 + permil, i.e., 70 permil would 1.007
 
         self.alp = 1 + self.alpha / 1000
         self.mo = self.reservoir.mo
-        self.__register_name__()
+        self.parent = self.register
+        self.__register_name_new__()
 
     def __call__(self, i: int) -> None:
         """
         Set flux isotope masses based on fractionation factor
+        relative to reservoir
 
         """
-        #print(f"self.f.m[i] =  {self.f.m[i]}")
-        if self.f.m[i] != 0:
-            # get target ratio based on reservoir ratio
-            c = (
-                self.reservoir.l[i - 1] /
-                (self.reservoir.m[i - 1] - self.reservoir.l[i - 1])) / self.alp
-
-            # calculate 32S in flux
-            self.f.l[i] = self.f.m[i] * c / (c + 1)
-            # retire the next two lines
-            self.f.h[i] = self.f.m[i] - self.f.l[i]
-            self.f.d[i] = get_delta(self.f.l[i], self.f.h[i],
-                                    self.reservoir.species.element.r)
-        return
 
-    def get_process_args(self):
+        # print(f"self.f.m[i] =  {self.f.m[i]}")
+        fm = self.f.fa[0]
+        if fm != 0:
+            rm = self.reservoir.m[i - 1]
+            rl = self.reservoir.l[i - 1]
+            a = self.alp
 
-        func_name: function = self.p_fractionation
-
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.reservoir.m,  # 4
-            self.reservoir.l,  # 5
-        ])
-        params = List(
-            [float(self.reservoir.species.element.r),
-             float(self.alp)])
+            fl = rl * fm / (a * rm + rl - a * rl)
+            self.f.fa[:] = [fm, fl]
+        else:
+            self.f.fa[:] = [
+                0,
+                0,
+            ]
 
-        return func_name, data, params
+        return
 
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
     def p_fractionation(data, params, i) -> None:
         # params
-        r: float = params[0]  # rvalue
         a: float = params[1]  # alpha
 
         # data
-        rm: float = data[4][i - 1]  # 4 reservoir mass
-        rl: float = data[5][i - 1]  # 4 reservoir light isotope
-        fm: float = data[0][i]  # flux mass
-
-        c = (rl / (rm - rl)) / a
-
-        data[1][i] = data[0][i] * c / (c + 1)  # flux li
-        data[2][i] = data[0][i] - data[1][i]  # flux hi
-        data[3][i] = 1000 * (data[2][i] / data[1][i] - r) / r  # flux d
+        fm: float = data[4][0]  # flux mass
+        rm: float = data[2][i - 1]  # 4 reservoir mass
+        rl: float = data[3][i - 1]  # 4 reservoir light isotope
+
+        fl = rl * fm / (a * rm + rl - a * rl)
+        data[4][:] = [fm, fl]
 
 
 class RateConstant(Process):
     """This is a wrapper for a variety of processes which depend on rate constants
     Please see the below class definitions for details on how to call them
     At present, the following processes are defined
 
-    ScaleRelativeToNormalizedConcentration
-    ScaleRelativeToConcentration
 
-    """
 
-    __slots__ = ("scale", "ref_value", "k_value", "flux", "reservoir")
+    """
 
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
+    def __init__(self, **kwargs: dict[str, any]) -> None:
         """Initialize this Process"""
 
-        from . import ureg, Q_
-        from .connections import SourceGroup, SinkGroup, ReservoirGroup
-        from .connections import ConnectionGroup, GasReservoir
-        from esbmtk import Flux
+        from esbmtk import (
+            SeawaterConstants,
+            GasReservoir,
+            Reservoir,
+            Source,
+            Sink,
+            Q_,
+        )
+        from typing import Callable
 
         # Note that self.lkk values also need to be added to the lkk
         # list of the connector object.
 
         # get default names and update list for this Process
         self.__defaultnames__()  # default kwargs names
 
         # update the allowed keywords
-        self.lkk: dict = {
-            "scale": (Number, np.float64),
-            "k_value": (Number, np.float64),
-            "name":
-            str,
-            "reservoir": (Reservoir, Source, Sink, GasReservoir, np.ndarray),
-            "flux":
-            Flux,
-            "ref_reservoirs":
-            list,
-            "reservoir_ref": (Reservoir, GasReservoir),
-            "left": (list, Reservoir, Number, np.float64, np.ndarray),
-            "right": (list, Reservoir, Number, np.ndarray),
-            "register": (
-                SourceGroup,
-                SinkGroup,
-                ReservoirGroup,
-                ConnectionGroup,
-                Flux,
-                str,
-            ),
-            "gas": (Reservoir, GasReservoir, Source, Sink, np.ndarray),
-            "liquid": (Reservoir, Source, Sink),
-            "solubility": (Number, np.float64),
-            "piston_velocity": (Number, np.float64),
-            "water_vapor_pressure": (Number, np.float64),
-            "ref_species":
-            np.ndarray,
-            "seawaterconstants":
-            any,
-            "isotopes":
-            bool,
-            "function_reference":
-            any,
-            "f_0": (str),
-            "pco2_0": (str),
-            "ex":
-            Number,
+        defaults: dict[str, list[any, tuple]] = {
+            "scale": [1, (int, float, np.float64)],
+            "k_value": [1, (int, float, np.float64)],
+            "ref_reservoirs": ["None", (str, list)],
+            "reservoir_ref": ["None", (str, Reservoir, GasReservoir)],
+            "left": [
+                "None",
+                (str, list, Reservoir, int, float, np.float64, np.ndarray),
+            ],
+            "right": ["None", (str, list, Reservoir, int, float, np.ndarray)],
+            "gas": [
+                "None",
+                (str, Reservoir, GasReservoir, Source, Sink, np.ndarray, float),
+            ],
+            "liquid": ["None", (Reservoir, Source, Sink, float)],
+            "solubility": ["None", (str, int, float, np.float64)],
+            "piston_velocity": ["None", (str, int, float, np.float64)],
+            "water_vapor_pressure": ["None", (str, int, float, np.float64)],
+            "ref_species": ["None", (str, np.ndarray, float)],
+            "seawaterconstants": ["None", (str, SeawaterConstants)],
+            "isotopes": [False, (bool)],
+            "function_reference": ["None", (str, Callable)],
+            "f_0": ["None", (str, Q_, float, int)],
+            "pco2_0": ["280 ppm", (str, Q_, float)],
+            "ex": [0.2, (int, float)],
+            "source": ["None", (str, Source, GasReservoir)],
         }
 
+        self.defaults.update(defaults)
         # new required keywords
-        self.lrk.extend([["reservoir", "atmosphere"], ["scale", "k_value"]])
+        # self.lrk.extend([["reservoir", "atmosphere"], ["scale", "k_value"], "register"])
 
-        # dict with default values if none provided
-        # self.lod = {r
-        self.lod: dict = {"isotopes": False, "function_reference": "None"}
-
-        self.__initerrormessages__()
-
-        # add these terms to the known error messages
-        self.bem.update({
-            "scale": "a number",
-            "reservoir": "Reservoir handle",
-            "ref_reservoirs": "List of Reservoir handle(s)",
-            "ref_value": "a number or flux quantity",
-            "name": "a string value",
-            "flux": "a flux handle",
-            "left": "list, reservoir or number",
-            "right": "list, reservoir or number",
-            "function_reference": "A function reference",
-        })
+        self.__initialize_keyword_variables__(kwargs)
 
-        # initialize keyword values
-        self.__validateandregister__(kwargs)
+        self.parent = self.register
         if "reservoir" in kwargs:
             self.mo = self.reservoir.mo
         elif "gas_reservoir" in kwargs:
             self.mo = self.gas_reservoir
 
         self.__misc_init__()
         self.__postinit__()  # do some housekeeping
         # legacy variables
 
-        self.__register_name__()
+        self.__register_name_new__()
 
+        self.c = 1
         if self.reservoir.isotopes or self.isotopes:
             self.__execute__ = self.__with_isotopes__
+            if self.delta != "None":
+                self.__execute__ = self.__with_fixed_delta__
+                l = get_l_mass(1, self.delta, self.reservoir.species.r)
+                self.c = l
+                # print(f"delta = {self.delta} setting c = {self.c}")
         else:
             self.__execute__ = self.__without_isotopes__
 
     def __postinit__(self) -> "None":
         self.mo = self.reservoir.mo
 
     # setup a placeholder call function
@@ -1273,176 +702,324 @@
                        reservoir = upstream_reservoir_handle,
                        reservoir_ref = reference_reservoir (Atmosphere)
                        flux = flux handle,
                        ex = exponent
                        pco2_0 = 280,
                        f_0 = 12 / 17e12
                        Scale =  1000,
+                       delta = 0,
+
     )
 
     """
+
     def __misc_init__(self):
         """
-        Scale the reference flux into the model flux units
+        Scale the flux relative to the pco2_0 concentration.
+        The delta values are derived from either:
+
+        - the upstream reservoir
+        - the upstream source
+        - set to a fixed value
+
         """
 
-        self.f_0: float = Q_(self.f_0).to(self.mo.f_unit).magnitude
-        self.pco2_0 = Q_(self.pco2_0).to("ppm").magnitude * 1e-6
+        from esbmtk import Source
+
+        if isinstance(self.f_0, str):
+            self.f_0: float = Q_(self.f_0).to(self.mo.f_unit).magnitude
+        elif isinstance(self.f_0, Q_):
+            self.f_0: float = self.f_0.to(self.mo.f_unit).magnitude
+
+        if isinstance(self.pco2_0, str):
+            self.pco2_0 = Q_(self.pco2_0).to("ppm").magnitude * 1e-6
+        elif isinstance(self.pco2_0, Q_):
+            self.pco2_0 = self.pco2_0.magnitude.to("ppm").magnitude * 1e-6
+
+        # if self.delta == "None" and  self.source.isotopes == False:
+        #      self.fixed = True
+        # delta provided explicitly
+        if self.delta != "None":
+            self.d = self.delta
+            self.isotopes = True
+            l = get_l_mass(1, self.d, self.source.species.element.r)
+            self.c = l / (1 - l)
+            self.func_name = self.p_weathering_fd
+            self.__execute__ = self.__with_fixed_delta__
+            self.fixed = True
+
+        # source is Source and has delta
+        elif self.source.isotopes and isinstance(self.source, Source):
+            self.isotopes = True
+            self.delta = self.source.delta
+            self.func_name = self.p_weathering_fd
+            self.__execute__ = self.__with_fixed_delta__
+            self.c = self.source.c
+            self.fixed = True
+
+        # source is reservoir
+        elif self.source.isotopes:
+            self.isotopes = True
+            self.func_name = self.p_weathering
+            self.__execute__ = self.__with_isotopes__
+            self.fixed = False
 
-    def __without_isotopes__(self, i: int) -> None:
+        # source is source, has no delta, and delta is not provided
+        else:
+            self.c = 1
+            self.isotopes = False
+            self.func_name = self.p_weathering_fd
+            self.__execute__ = self.__without_isotopes__
+            self.fixed = True
 
-        # print(
-        #    f"f_0={self.f_0}, scale={self.scale}, c={self.reservoir_ref.c[i-1]}, p0={self.pco2_0}, ex={self.ex}"
-        # )
-        self.flux.m[i] = (
-            self.f_0 *
-            (self.scale * self.reservoir_ref.c[i - 1] / self.pco2_0)**self.ex)
+    def __without_isotopes__(self, i: int) -> None:
+        f = self.scale * (
+            self.f_0 * (self.reservoir_ref.c[i - 1] / self.pco2_0) ** self.ex
+        )
+        self.flux.fa = np.array([f, 0])
 
     def __with_isotopes__(self, i: int) -> None:
         """
         C = M/V so we express this as relative to mass which allows us to
         use the isotope data.
 
         The below calculates the flux as function of reservoir concentration,
         rather than scaling the flux.
         """
 
-        raise NotImplementedError("weathering has currently no isotope method")
-        # c: float = self.reservoir.c[i - 1]
-        # if c > 0:  # otherwise there is no flux
-        #     m = c * self.scale
-        #     r: float = reservoir.species.element.r
-        #     d: float = reservoir.d[i - 1]
-        #     l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-        #     self.flux[i]: np.array = [m, l, m - l, d]
-
-    def get_process_args(self):
-
-        func_name: function = self.p_weathering
-
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.reservoir_ref.d,  # 4
-            self.reservoir_ref.c,  # 5
-            self.reservoir_ref.m,  # 6
-        ])
-        params = List([
-            float(self.reservoir.species.element.r),  # 0
-            float(self.scale),  # 1
-            float(self.f_0),  # 2
-            float(self.pco2_0),  # 3
-            float(self.ex),  # 4
-        ])
+        c = self.flux.fa[1] / self.flux.fa[0]
+        f = self.scale * (
+            self.f_0 * (self.reservoir_ref.c[i - 1] / self.pco2_0) ** self.ex
+        )
+        fl = f * c
+        self.flux.fa = np.array([f, fl])
+
+    def __with_fixed_delta__(self, i: int) -> None:
+        """ """
 
-        return func_name, data, params
+        f = self.scale * (
+            self.f_0 * (self.reservoir_ref.c[i - 1] / self.pco2_0) ** self.ex
+        )
+        fl = f * self.c
+        self.flux.fa = np.array([f, fl])
 
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
     def p_weathering(data, params, i) -> None:
-        # concentration times scale factor
+        """delta value depends on upstream reservoir"""
+        # params
         s: float = params[1]
         f_0: float = params[2]
         pco2_0: float = params[3]
         ex: float = params[4]
 
-        c: float = data[5][i - 1]
-        f: float = f_0 * (c * s / pco2_0)**ex
-        data[0][i] = f
-        # data[3][i] = data[4][i - 1]
-        # print(i)
-        # print(" ")
+        # data
+        cr = data[3][i - 1] / data[2][i - 1]
+        c: float = data[1][i - 1]
 
+        f: float = s * f_0 * (c / pco2_0) ** ex
+        fl: float = f * cr
+        data[0][:] = [f, fl]
 
-class ScaleRelativeToConcentration(RateConstant):
-    """This process calculates the flux as a function of the upstream
-     reservoir concentration C and a constant which describes thet
-     strength of relation between the reservoir concentration and
-     the flux scaling
+    def p_weathering_fd(data, params, i) -> None:
+        """delta value is fixed"""
+        # params
+        s: float = params[1]
+        f_0: float = params[2]
+        pco2_0: float = params[3]
+        ex: float = params[4]
+        cr = params[5]
 
-     F = C * k
+        c: float = data[1][i - 1]
+        f: float = s * f_0 * (c / pco2_0) ** ex
+        fl = f * cr
+        data[0][:] = [f, fl]
 
-     where C denotes the concentration in the ustream reservoir, k is a
-     constant. This process is typically called by the connector
-     instance. However you can instantiate it manually as
 
-     ScaleRelativeToConcentration(
-                       name = "Name",
-                       reservoir= upstream_reservoir_handle,
-                       flux = flux handle,
-                       Scale =  1000,
-    )
+class MultiplySignal(Process):
+    """This process mulitplies a given flux with the the data in the
+    signal.  This class is typically invoked through the connector
+    object: Note that this process will not modify the delta value of
+    a given flux.  If you needto vary the delta value it is best to
+    add a second signal which uses the add signal type.
+
+     Example::
+     MultiplySignal(name = "name",
+               reservoir = upstream_reservoir_handle,
+               flux = flux_to_act_upon,
+               lt = flux with lookup values)
+
+     where the upstream reservoir is the reservoir the process belongs
+             too the flux is the flux to act upon lt= contains the
+             flux object we lookup from
 
     """
-    def __without_isotopes__(self, i: int) -> None:
-        m: float = self.reservoir.m[i - 1]
-        if m > 0:  # otherwise there is no flux
-            # convert to concentration
-            c = m / self.reservoir.volume
-            f = c * self.scale
-            self.flux.m[i] = f
 
-    def __with_isotopes__(self, i: int) -> None:
+    def __init__(self, **kwargs: dict[str, any]) -> None:
+        """
+        Create a new process object with a given process type and options
         """
-        C = M/V so we express this as relative to mass which allows us to
-        use the isotope data.
 
-        The below calculates the flux as function of self.reservoir concentration,
-        rather than scaling the flux.
+        # get default names and update list for this Process
+        self.__defaultnames__()  # default kwargs names
+        self.lrk.extend(["lt", "flux", "reservoir"])  # new required keywords
+        self.__initialize_keyword_variables__(kwargs)  # initialize keyword values
+
+        # legacy variables
+        self.mo = self.reservoir.mo
+        self.__postinit__()  # do some housekeeping
+        self.parent = self.register
+        self.__register_name_new__()
+
+        # decide whichh call function to use
+        # if self.mo.m_type == "both":
+
+        # default
+        self.__execute__ = self.__multiply_with_flux_fi__
+
+    # setup a placeholder call function
+    def __call__(self, i: int):
+        return self.__execute__(i)
+
+    # use this when we do isotopes
+    def __multiply_with_flux_fi__(self, i) -> None:
+        """Each process is associated with a flux (self.f). Here we replace
+        the flux value with the value from the signal object which
+        we use as a lookup-table (self.lt)
+        """
+
+        # multiply flux mass with signal
+        c = self.lt.m[i]
+        m = self.f.m[i] * c
+        l = self.f.l[i] * c
+        # h = self.f.h[i] * c
+        # d = self.f.d[i]
+        self.flux.fa = np.array([m, l])
+        print(f"multiply fa {self.flux.fa}, f. = {self.f.m[i]}, c = {c} ")
+
+    def __multiply_with_flux_fa__(self, i) -> None:
+        """Each process is associated with a flux (self.f). Here we replace
+        the flux value with the value from the signal object which
+        we use as a lookup-table (self.lt)
         """
 
-        c: float = self.reservoir.c[i - 1]
-        if c > 0:  # otherwise there is no flux
-            m = c * self.scale
-            r: float = self.reservoir.species.element.r
-            d: float = self.reservoir.d[i - 1]
-            l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-            self.flux[i]: np.array = [m, l, m - l, d]
-
-    def get_process_args(self):
-
-        func_name: function = self.p_scale_relative_to_concentration
-
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.reservoir.d,  # 4
-            self.reservoir.c,  # 5
-            self.reservoir.m,  # 6
-        ])
-        params = List([
-            float(self.reservoir.species.element.r),
-            float(self.scale),
-            float(self.reservoir.v),
-        ])
+        # multiply flux mass with signal
+        c = self.lt.m[i]
+        m = self.f.fa[0] * c
+        l = self.f.fa[1] * c
+        self.flux.fa = np.array([m, l])
+
+    def p_multiply_signal_fi(data, params, i) -> None:
+        c = data[2][i]
+        m = data[0][i] * c
+        l = data[1][i] * c
+
+        data[3][:] = [m, l]
+
+    def p_multiply_signal_fa(data, params, i) -> None:
+        c = data[0][i]
+        m = data[1][0] * c  # m
+        l = data[1][1] * c  # l
 
-        return func_name, data, params
+        data[1][:] = [m, l]
 
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
-    def p_scale_relative_to_concentration(data, params, i) -> None:
+
+class VarDeltaOut(Process):
+    """Unlike a passive flux, this process sets the flux istope ratio
+    equal to the isotopic ratio of the reservoir. The
+    init and register methods are inherited from the process
+    class.
+    VarDeltaOut(name = "name",
+                reservoir = upstream_reservoir_handle,
+                flux = flux handle,
+                rate = rate,)
+    """
+
+    def __init__(self, **kwargs: dict[str, any]) -> None:
+        """Initialize this Process"""
+
+        from esbmtk import (
+            Reservoir,
+            Source,
+        )
+
+        # get default names and update list for this Process
+        self.__defaultnames__()
+
+        self.lrk.extend(["reservoir", "flux", "register"])  # required keywords
+
+        self.__initialize_keyword_variables__(kwargs)
+        self.mo = self.reservoir.mo
+        self.parent = self.register
+        self.__postinit__()  # do some housekeeping
+        self.__register_name_new__()
+
+        # decide which call function to use
+        # if self.mo.m_type == "both":
+        if self.reservoir.isotopes:
+            # print(
+            #    f"vardeltaout with isotopes for {self.reservoir.register.name}.{self.reservoir.name}"
+            # )
+            if isinstance(self.reservoir, Reservoir):
+                # print("Using reservoir")
+                self.__execute__ = self.__with_isotopes_reservoir__
+            elif isinstance(self.reservoir, Source):
+                # print("Using Source")
+                self.__execute__ = self.__with_isotopes_source__
+            else:
+                raise ValueError(
+                    f"{self.name}, reservoir must be of type Source or Reservoir, not {type(self.reservoir)}"
+                )
+        else:
+            self.__execute__ = self.__without_isotopes__
+
+    # setup a placeholder call function
+    def __call__(self, i: int):
+        return self.__execute__(i)
+
+    def __with_isotopes_reservoir__(self, i: int) -> None:
+        """Here we re-balance the flux. This code will be called by the
+        apply_flux_modifier method of a reservoir which itself is
+        called by the model execute method
+        """
+
+        m: float = self.flux.m[i]
+        if m != 0:
+            c = self.reservoir.l[i - 1] / (
+                self.reservoir.m[i - 1] - self.reservoir.l[i - 1]
+            )
+            self.flux.fa = [m, m * c]
+
+    def p_vardeltaout(data, params, i) -> None:
         # concentration times scale factor
-        r: float = params[0]
-        s: float = params[1]
-        m: float = data[6][i - 1]
-        v: float = params[2]
 
-        if m > 0:
-            c: float = m / v
-            f: float = c * s
-            d: float = data[4][i - 1]  # delta
-            l: float = (1000.0 * f) / ((d + 1000.0) * r + 1000.0)
-            data[0][i] = f
-            data[1][i] = l
-            data[2][i] = m - l
-            data[3][i] = d
+        mf: float = data[0][i - 1]  # flux mass
+        mr: float = data[1][i - 1]  # reservoir mass
+        lr: float = data[2][i - 1]  # reservoir l
+
+        c = lr / (mr - lr)
+        data[3][:] = [mf, mf * c]
+
+    def __with_isotopes_source__(self, i: int) -> None:
+        """If the source of the flux is a source, there is only a single delta value.
+        Changes to the flux delta are applied through the Signal class.
+        """
+
+        m: float = self.flux.m[i]
+        if m != 0:
+            c = self.reservoir.l[i - 1] / (
+                self.reservoir.m[i - 1] - self.reservoir.l[i - 1]
+            )
+            self.flux.fa = [m, m * c]
+
+    def __without_isotopes__(self, i: int) -> None:
+        """Here we re-balance the flux. This code will be called by the
+        apply_flux_modifier method of a reservoir which itself is
+        called by the model execute method
+        """
+
+        raise NotImplementedError("vardeltaout w/o isotopes is not defined")
 
 
 class ScaleRelativeToMass(RateConstant):
     """This process scales the flux as a function of the upstream
      reservoir Mass M and a constant which describes the
      strength of relation between the reservoir mass and
      the flux scaling
@@ -1464,200 +1041,48 @@
                        name = "Name",
                        reservoir= upstream_reservoir_handle,
                        flux = flux handle,
                        Scale =  1000,
     )
 
     """
+
     def __without_isotopes__(self, i: int) -> None:
         m: float = self.reservoir.m[i - 1] * self.scale
-        self.flux.m[i]: float = m
+        self.flux.fa = [m, 0, 0, 0]
 
     def __with_isotopes__(self, i: int) -> None:
         """
         this will be called by the Model.run() method
 
         """
         m: float = self.reservoir.m[i - 1] * self.scale
-        r: float = self.reservoir.species.element.r
-        d: float = self.reservoir.d[i - 1]
-        l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-        self.flux[i]: np.array = [m, l, m - l, d]
-
-    def get_process_args(self):
-        """return the data associated with this object"""
-
-        func_name: function = self.p_scale_relative_to_mass
-
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.reservoir.m,  # 4
-            self.reservoir.d,  # 5
-        ])
-
-        params = List([float(reservoir.species.element.r), float(self.scale)])
-
-        return func_name, data, params
+        # d: float = self.reservoir.d[i - 1]
+        c = self.reservoir.l[i - 1] / (
+            self.reservoir.m[i - 1] - self.reservoir.l[i - 1]
+        )
+        l = m * c / (c + 1)
+        self.flux.fa[:] = [m, l]
 
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
     def p_scale_relative_to_mass(data, params, i) -> None:
         # concentration times scale factor
+        # params
+        s: float = params[1]  # scale factor
 
-        r: float = params[0]
-        s: float = params[1]
-        m: float = data[0][i - 1] * s
-        d: float = data[1][i - 1]  # delta
-        l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-
-        data[0][i] = m
-        data[1][i] = l
-        data[2][i] = m - l
-        data[3][i] = d
-
-
-class ScaleRelative2otherReservoir(RateConstant):
-    """This process scales the flux as a function one or more reservoirs
-    constant which describes the
-    strength of relation between the reservoir concentration and
-    the flux scaling
-
-    F = C1 * C1 * k
-
-    where Mi denotes the concentration in one  or more reservoirs, k is one
-    or more constant(s). This process is typically called by the connector
-    instance when you specify the connection as
-
-    Connect(source =  upstream reservoir,
-              sink = downstream reservoir,
-              ctype = "scale_relative_to_multiple_reservoirs"
-              ref_reservoirs = [r1, r2, k etc] # you must provide at least one
-                                               # reservoir or constant
-              scale = a overall scaling factor
-           )
-    """
-    def __misc_init__(self) -> None:
-        """Test that self.reservoir only contains numbers and reservoirs"""
-
-        self.rs: list = []
-        self.constant: Number = 1
-
-        for r in self.ref_reservoirs:
-            if isinstance(r, (Reservoir)):
-                self.rs.append(r)
-            elif isinstance(r, (Number)):
-                self.constant = self.constant * r
-            else:
-                raise ValueError(
-                    f"{r} must be reservoir or number, not {type(r)}")
-
-    def __without_isotopes__(self, i: int) -> None:
-        c: float = 1
-        for r in self.rs:
-            c = c * r.c[i - 1]
-
-        scale: float = c * self.scale * self.constant
-
-        # scale = scale * (scale >= 0)  # prevent negative fluxes.
-        self.f[i] = [scale, scale, scale, 1]
-
-    def __with_isotopes__(self, i: int) -> None:
-        """
-        not sure that this correct WRT isotopes
-
-        """
-
-        raise NotImplementedError(
-            "Scale relative to multiple reservoirs is undefined for isotope calculations"
-        )
-
-        # c: float = 1
-        # for r in self.rs:
-        #     c = c * r.c[i - 1]
-
-        # scale: float = c * self.scale * self.constant
-
-        # # scale = scale * (scale >= 0)  # prevent negative fluxes.
-        # self.f[i] = [scale, scale, scale, 1]
-
-
-class Flux_Balance(RateConstant):
-    """This process calculates a flux between two reservoirs as a function
-    of multiple reservoir concentrations and constants.
-
-    Note that could result in negative fluxes. which might cause
-    issues with isotope ratios (untested)
-
-    This will work with equilibrium reactions between two reservoirs where the
-    reaction can be described as
-
-    K * [R1] = R[2] * [R3]
-
-    you can have more than two terms on each side as long as they are
-    constants or reservoirs
-
-    Equilibrium(
-                name = "Name",
-                reservoir = reservoir handle,
-                left = [] # list with reservoir names or constants
-                right = [] # list with reservoir names or constants
-                flux = flux handle,
-                k_value = a constant, defaults to 1
-    )
-
-    """
-
-    # redefine misc_init which is being called by post-init
-    def __misc_init__(self):
-        """Sort out input variables"""
-
-        Rl: List[Reservoir] = []
-        Rr: List[Reservoir] = []
-        Cl: List[float] = []
-        Cr: List[float] = []
-        # parse the left hand side
-
-        em = "left/right values must be constants or reservoirs"
-        [self.Rl, self.Cl] = sort_by_type(self.left, [Reservoir, Number], em)
-        [self.Rr, self.Cr] = sort_by_type(self.right, [Reservoir, Number], em)
-
-    def __without_isotopes__(self, i: int) -> None:
-
-        kl: np.ndarray = np.array([1.0, 1.0, 1.0, 1.0])
-        kr: np.ndarray = np.array([1.0, 1.0, 1.0, 1.0])
-        scale: np.ndarray = np.array([1.0, 1.0, 1.0, 1.0])
-
-        # calculate the product of reservoir concentrations for left side
-        for r in self.Rl:
-            kl *= r[i - 1]
-        # multiply with any any constants on the right
-        for c in self.Cl:
-            kl *= c
-
-        # calculate the product of reservoir concentrations for right side
-        for r in self.Rr:
-            kr *= r[i - 1]
-        # multiply with any any constants on the right
-        for c in self.Cr:
-            kr *= c
-
-        # set flux
-        self.f[i] = (kl - kr) * self.k_value
-
-    def __with_isotopes__(self, i: int) -> None:
-        """
-        not sure that this correct WRT isotopes
-
-        """
+        # data
+        rm = data[2][i - 1]
+        rl = data[3][i - 1]
+        # rd = data[6][i - 1]
+
+        m: float = rm * s  # new flux
+        c: float = rl / (rm - rl)
+        l: float = m * c / (c + 1)
+        # d: float = data[1][i - 1]  # flux delta
 
-        raise NotImplementedError(
-            "Flux Balance is undefined for isotope calculations")
+        data[4][:] = [m, l]
 
 
 class GasExchange(RateConstant):
     """
 
     GasExchange(
           gas =GasReservoir, #
@@ -1671,43 +1096,54 @@
     )
 
 
     """
 
     # redefine misc_init which is being called by post-init
     def __misc_init__(self):
-        """Sort out input variables"""
+        """Set up input variables"""
 
         self.p_H2O = self.seawaterconstants.p_H2O
         self.a_dg = self.seawaterconstants.a_dg
         self.a_db = self.seawaterconstants.a_db
         self.a_u = self.seawaterconstants.a_u
         self.rvalue = self.liquid.sp.r
         self.volume = self.gas.volume
 
-    def __without_isotopes__(self, i: int) -> None:
+    def ode(self) -> None:
+        return self.scale * (
+            self.gas.c * (1 - self.p_H2O) * self.solubility - self.ref_species * 1000
+        )  # area in m^2  # Atmosphere  # p_H2O  # SA_co2 = mol/(m^3 atm)  # [CO2]aq mol
 
+    def __without_isotopes__(self, i: int) -> None:
         # set flux
         # note that the sink delta is co2aq as returned by the carbonate VR
         # this equation is for mmol but esbmtk uses mol, so we need to
         # multiply by 1E3
 
-        a = self.scale * (  # area in m^2
-            self.gas.c[i - 1]  #  Atmosphere
+        f = self.scale * (  # area in m^2
+            self.gas.c[i - 1]  # Atmosphere
             * (1 - self.p_H2O)  # p_H2O
             * self.solubility  # SA_co2 = mol/(m^3 atm)
             - self.ref_species[i - 1] * 1000  # [CO2]aq mol
         )
         # print(self.gas.c[i - 1])
 
         # changes in the mass of CO2 also affect changes in the total mass
         # of the atmosphere. So we need to update the reservoir volume
         # variable which we use the store the total atmospheric mass
-        # reservoir.v[i] = reservoir.v[i] + a * reservoir.mo.dt
-        self.flux[i] = [a, 1, 1, 1]
+        """The solver will use f and f12 to update mass, light
+        isotope and concentration values in the Gas
+        reservoir. However, Gas reservoirs track total gas pressure
+        in the volume variable. This will not be updated by the
+        solver. So we need to do it ourseleves
+
+        """
+        # self.gas.v[i] = self.gas.v[i - 1] + f * self.gas.mo.dt
+        self.flux.fa[:] = [f, 1]
 
     def __with_isotopes__(self, i: int) -> None:
         """
         In the following I assume near neutral pH between 7 and 9, so that
         the isotopic composition of HCO3- is approximately equal to the isotopic
         ratio of DIC. The isotopic ratio of [CO2]aq can then be obtained from DIC via
         swc.e_db (swc.a_db)
@@ -1716,218 +1152,175 @@
 
         g = gaseous
         d = dissolved
         b = bicarbonate ion
         c = carbonate ion
 
         a_db is thus the fractionation factor between dissolved CO2aq and HCO3-
-        and a_gb between CO2g HCO3-
+        and a_dg between CO2aq and CO2g
+
+        ref_species = DIC.cs.CO2aq
+        liquid.m = DIC.m (used to get the isotope ratio)
+
+        gas.m = mass of CO2
+        gas.l = mass of 12CO2
+        gas.c = CO2 concentration
+        gas.v = total mass of atmosphere
+
         """
 
-        f = self.scale * (
+        # equilibrium concentration of CO2 in water based on pCO2
+        eco2_at = (
             self.gas.c[i - 1]  # p Atmosphere
             * (1 - self.p_H2O)  # p_H2O
-            * self.solubility  # SA_co2
-            - self.ref_species[i - 1] * 1000  # [CO2]aq
+            * self.solubility
         )
+        # equilibrium concentration of CO2 in water based on CO2aq
+        eco2_aq = self.ref_species[i - 1] * 1000
 
-        co2aq_c13 = self.ref_species[i - 1] * self.r.h[i - 1] / self.r.m[i - 1]
-        co2at_c13 = self.gas.h[i - 1] / self.gas.volume
+        #  flux
+        f = self.scale * (eco2_at - eco2_aq)
 
-        f13 = (
-            self.scale * self.a_u * (
-                self.a_dg * co2at_c13 * (1 - self.p_H2O)  # p_H2O
-                * self.solubility  # SA_co2
-                - self.a_db * co2aq_c13 * 1000))
-
-        # h = flux!
-        f12 = f - f13
-        d = (f13 / f12 / self.rvalue - 1) * 1000
-
-        # print(f"f={f:.2e}")
-        # print(f"P: f={f:.2e}, f12={f12:.2e}, f13={f13:.2e}, d={d:.2f}")
-        self.flux[i] = [f, f12, f13, d]
+        c13g = 1 - self.gas.l[i - 1] / self.gas.m[i - 1]
+        c13aq = 1 - self.liquid.l[i - 1] / self.liquid.m[i - 1]
+        # get 13C CO2 equlibrium concentration  CO2 in water based on pCO2
+        eco2_at_13 = (
+            self.gas.c[i - 1]
+            * c13g
+            * (1 - self.p_H2O)  # p_H2O
+            * self.solubility
+            * self.a_dg
+        )
 
-        # changes in the mass of CO2 also affect changes in the total mass
-        # of the atmosphere. So we need to update the reservoir volume
-        # variable which we use the store the total atmospheric mass
+        # get 13C equilibrium  CO2 in water based on DIC m & l
+        eco2_aq_13 = self.a_db * eco2_aq * c13aq
 
-        # print(f"Name = {reservoir.full_name}")
-        # reservoir.v[i] = reservoir.v[i] + f * reservoir.mo.dt
+        # 13C flux
+        f13 = self.scale * self.a_u * (eco2_at_13 - eco2_aq_13)
+        f12 = f - f13
 
-        # raise NotImplementedError()
+        self.flux.fa = [f, f12]
+        """The solver will use f and f12 to update mass, light
+        isotope and concentration values in the Gas
+        reservoir. However, Gas reservoirs track total gas pressure
+        in the volume variable. This will not be updated by the
+        solver. So we need to do it ourseleves
+
+        not working, see note below
+        """
+        self.gas.v[i] = self.gas.v[i - 1] + f * self.gas.mo.dt
+        return [f, f12]
+        # print()
 
     def __postinit__(self) -> None:
         """Do some housekeeping for the process class"""
 
         # legacy name aliases
         self.n: str = self.name  # display name of species
         self.r = self.liquid
         self.reservoir = self.liquid
 
-    def get_process_args(self):
-        """return the data associated with this object"""
-
-        func_name: function = self.p_gas_exchange
-
-        data = List([
-            self.flux.m,  # 0
-            self.flux.l,  # 1
-            self.flux.h,  # 2
-            self.flux.d,  # 3
-            self.liquid.m,  # 4
-            self.liquid.h,  # 5
-            self.ref_species,  # 6
-            self.gas.c,  # 7
-            self.gas.h,  # 8
-            self.gas.v,  # 9
-            self.r.m,  # 10
-            self.r.h,  # 11
-        ])
-
-        params = List([
-            float(self.scale),  # 0
-            float(self.solubility * (1 - self.p_H2O)),  # 1
-            float(self.rvalue),  # 2
-            float(self.gas.volume),  # 3
-            float(self.a_u),  # 4
-            float(self.a_dg),  # 5
-            float(self.a_db),  # 6
-            float(self.reservoir.mo.dt),  # 7
-            float(self.p_H2O),  # 8
-            float(self.solubility),  #9 
-        ])
-
-        self.params = params
-        return func_name, data, params
-
-    @staticmethod
-    @njit(fastmath=True, error_model="numpy")
-    def p_gas_exchange(data, params, i) -> None:
-        """the below equation moved as many constants as possible outside of
-        the function compared to the __with/without_isotopes__ method(s). See the
-        __get_process_args__ method for details
-
-        This process does not yet work with variable volumes
-
-        """
-
-        scale: float = params[0]  # scale
-        SA: float = params[1]  # solubility
-        r: float = params[2]  # r value
-        gv: float = params[3]  # gas volume
-        au: float = params[4]  #
-        dg: float = params[5]  #
-        db: float = params[6]  #
-        dt: float = params[7]  # dt
-        pH2O: float = params[8]  # p_H2O
-        solubility: float = params[9]  # solubility
-
-        rs = data[6][i - 1]  # ref species
-        rm = data[10][i - 1]
-        rh = data[11][i - 1]
-        gc = data[7][i - 1]
-        gh = data[8][i - 1]  # gas.h
-
-        f = scale * (gc * (1 - pH2O) * solubility - rs * 1000)
-        co2aq_c13 = rs * rh / rm  #
-        co2at_c13 = gh / gv
-
-        f13 = scale * au * (dg * co2at_c13 *
-                            (1 - pH2O) * solubility - db * co2aq_c13 * 1000)
-        f12 = f - f13
-        d = (f13 / f12 / r - 1) * 1000
-
-        data[0][i] = f
-        data[1][i] = f12
-        data[2][i] = f13
-        data[3][i] = d
-        data[9][i] = data[9][i] + f * dt
 
+class ScaleRelativeToConcentration(RateConstant):
+    """This process calculates the flux as a function of the upstream
+     reservoir concentration C and a constant which describes thet
+     strength of relation between the reservoir concentration and
+     the flux scaling
 
-class Monod(Process):
-    """This process scales the flux as a function of the upstream
-    reservoir concentration using a Michaelis Menten type
-    relationship
+     F = C * k
 
-    F = F * a * F0 x C/(b+C)
+     where C denotes the concentration in the ustream reservoir, k is a
+     constant. This process is typically called by the connector
+     instance. However you can instantiate it manually as
 
-    where F0 denotes the unscaled flux (i.e., at t=0), C denotes
-    the concentration in the ustream reservoir, and a and b are
-    constants.
+     ScaleRelativeToConcentration(
+                       name = "Name",
+                       reservoir= upstream_reservoir_handle,
+                       flux = flux handle,
+                       Scale =  1000,
+                       delta = "None",
+    )
 
-    Example::
-         Monod(name = "Name",
-               reservoir =  upstream_reservoir_handle,
-               flux = flux handle ,
-               ref_value = reference concentration
-               a_value = constant,
-               b_value = constant )
+    If delta is given the fluxes uses a ficed delta, If not it uses
+    the upestream delta
 
     """
-    def __init__(self, **kwargs: Dict[str, any]) -> None:
-        """"""
 
-        from . import ureg, Q_
-        """ Initialize this Process """
-        # get default names and update list for this Process
-        self.__defaultnames__()  # default kwargs names
-
-        # update the allowed keywords
-        self.lkk: dict = {
-            "a_value": (Number, np.float64),
-            "b_value": (Number, np.float64),
-            "ref_value": ((Number, np.float64), str, Q_),
-            "name":
-            str,
-            "reservoir": (Reservoir, Source, Sink),
-            "flux":
-            Flux,
-            "register":
-            (SourceGroup, SinkGroup, ReservoirGroup, ConnectionGroup, str),
-        }
+    def __without_isotopes__(self, i: int) -> None:
+        m: float = self.reservoir.m[i - 1]
+        if m > 0:  # otherwise there is no flux
+            # convert to concentration
+            c = m / self.reservoir.volume
+            f = c * self.scale
+            self.flux.fa = [
+                f,
+                0,
+            ]
 
-        self.lrk.extend(["reservoir", "a_value", "b_value",
-                         "ref_value"])  # new required keywords
+    def __with_isotopes__(self, i: int) -> None:
+        """
+        C = M/V so we express this as relative to mass which allows us to
+        use the isotope data.
 
-        self.__initerrormessages__()
-        self.bem.update({
-            "a_value": "a number",
-            "b_value": "a number",
-            "reservoir": "Reservoir handle",
-            "ref_value": "a number",
-            "name": "a string value",
-            "flux": "a flux handle",
-        })
+        The below calculates the flux as function of self.reservoir concentration,
+        rather than scaling the flux.
+        """
 
-        self.__validateandregister__(kwargs)  # initialize keyword values
-        self.__postinit__()  # do some housekeeping
-        # legacy variables
-        self.mo = self.reservoir.mo
-        self.__register_name__()
+        rc: float = self.reservoir.c[i - 1]
+        if rc > 0:  # otherwise there is no flux
+            c = self.reservoir.l[i - 1] / (
+                self.reservoir.m[i - 1] - self.reservoir.l[i - 1]
+            )
+            m = rc * self.scale
+            l = m * c / (c + 1)
+            self.f.fa = [m, l]
 
-    def __call__(self, i: int) -> None:
+    def __with_fixed_delta__(self, i: int) -> None:
         """
-        this willbe called by Model.execute apply_processes
+        C = M/V so we express this as relative to mass which allows us to
+        use the isotope data.
+
+        The below calculates the flux as function of self.reservoir concentration,
+        rather than scaling the flux.
         """
 
-        scale: float = (self.a_value *
-                        (self.ref_value * self.reservoir.c[i - 1]) /
-                        (self.b_value + self.reservoir.c[i - 1]))
+        rc: float = self.reservoir.c[i - 1]
+        if rc > 0:  # otherwise there is no flux
+            c = self.c
+            m = rc * self.scale
+            l = m * c / (c + 1)
+            self.f.fa = [m, l]
 
-        scale = scale * (scale >= 0)  # prevent negative fluxes.
-        self.f[i] + self.f[i] * scale
+    def p_scale_relative_to_concentration(data, params, i) -> None:
+        """delta depends on upstream delta"""
+        # data
+        rm: float = data[0][i - 1]  # res mass
+        if rm > 0:
+            # params
+            s: float = params[0]  # scale factor
+            v: float = params[1]  # res volume
+            fm: float = rm / v * s
+            rl: float = data[1][i - 1]  # res li
+
+            c: float = rl / (rm - rl)
+            fl: float = fm * c / (c + 1)
+            data[2][:] = [fm, fl]
 
-    def __plot__(self, start: int, stop: int, ref_reservoirs: float, a: float,
-                 b: float) -> None:
-        """Test the implementation"""
+        else:
+            data[2][:] = [0.0, 0.0]
 
-        y = []
-        x = range(start, stop)
+    def p_scale_relative_to_concentration_fd(data, params, i) -> None:
+        """delta depends fixed value"""
+        # data
+        rm: float = data[0][i - 1]  # res mass
 
-        for e in x:
-            y.append(a * ref_reservoirs * e / (b + e))
+        if rm > 0:
+            # params
+            s: float = params[1]  # scale factor
+            v: float = params[2]  # res volume
+            fm: float = rm / v * s
+            c: float = params[3]  # isotope ratio
+            fl: float = fm * c / (c + 1)
+            data[2][:] = [fm, fl]
 
-        fig, ax = plt.subplots()  #
-        ax.plot(x, y)
-        # Create a scatter plot for ax
-        plt.show()
+        else:
+            data[2][:] = [0.0, 0.0]
```

### Comparing `esbmtk-0.8.0.0/esbmtk/sealevel.py` & `esbmtk-0.9.0.1/esbmtk/sealevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,16 @@
         # required keywords
         self.lrk: list = [
             "name",
         ]
 
         self.__initialize_keyword_variables__(kwargs)
 
-        if self.register == "None":
-            if self.model != "None":
-                self.register = self.model
+        if self.register == "None" and self.model != "None":
+            self.register = self.model
 
         self.parent = self.register
 
         # legacy variables
         self.pfn = "spline_paramaters.txt"
         self.hfn = "Hypsometric_Curve_05m.csv"
         self.sa = 510067420e6  # total surfce area in square meters, http://www.physicalgeography.net/fundamentals/8o.html
@@ -112,17 +111,15 @@
         """
 
         u = abs(u)
         l = abs(l)
         if l < u:
             raise ValueError(f"hyp.volume: {l} must be higher than {u}")
 
-        v = np.sum(self.hypdata[u:l]) * self.sa
-
-        return v
+        return np.sum(self.hypdata[u:l]) * self.sa
 
     def area(self, depth: int) -> float:
         """Calculate the ocean area at a given depth
 
         depth must be an integer between 0 and 6000 mbsl, or a
         numpy array of integers between 0 and 6000 mbsl
 
@@ -153,17 +150,15 @@
         """
 
         if l < -6002:
             raise ValueError("area_dz() is only defined to a depth of 6000 mbsl")
 
         a: np.ndarray = sp.interpolate.splev([u, l], self.tck)
 
-        area: float = (a[0] - a[-1]) * self.sa
-
-        return area
+        return (a[0] - a[-1]) * self.sa
 
     def __init_curve__(self):
         """Initialize Spline Parameters. See  __bootstrap_curve__ if you want
         to change the default parameters
 
         """
         t = [
@@ -282,25 +277,28 @@
         Note that the numbers are in m^2
 
         """
 
         return np.diff(self.get_lookup_table(min_depth, max_depth))
 
 
-def get_box_geometry_parameters(box):
+def get_box_geometry_parameters(box) -> None:
     from esbmtk import Q_
 
+    box.geometry_unset = True
+
     if box.geometry != "None":
         if not isinstance(box.geometry, list):
             raise ValueError("geometry must be a list see the docs for details")
         box.area_percentage = box.geometry[2]
         volume = f"{box.mo.hyp.volume(box.geometry[0], box.geometry[1]) * box.area_percentage} m**3"
 
         box.volume = Q_(volume)
         box.area = box.mo.hyp.area(box.geometry[0]) * box.area_percentage
         box.area_dz = (
             box.mo.hyp.area_dz(box.geometry[0], box.geometry[1]) * box.area_percentage
         )
         box.area_fraction = box.area_dz / box.mo.hyp.oa
+        box.geometry_unset = False
 
     elif box.volume == "None":
         raise ValueError("You need to provide volume or geometry!")
```

### Comparing `esbmtk-0.8.0.0/esbmtk/solver.py` & `esbmtk-0.9.0.1/esbmtk/depreceated_code.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,199 +1,7 @@
-"""
-     esbmtk: A general purpose Earth Science box model toolkit
-     Copyright (C), 2020 Ulrich G. Wortmann
-
-     This program is free software: you can redistribute it and/or modify
-     it under the terms of the GNU General Public License as published by
-     the Free Software Foundation, either version 3 of the License, or
-     (at your option) any later version.
-
-     This program is distributed in the hope that it will be useful,
-     but WITHOUT ANY WARRANTY; without even the implied warranty of
-     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-     GNU General Public License for more details.
-
-     You should have received a copy of the GNU General Public License
-     along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-# from pint import UnitRegistry
-# from nptyping import *
-import time
-from time import process_time
-import numba
-from numba.core import types
-from numba import njit
-from numba.typed import List
-import numpy as np
-
-
-def get_l_mass(m: float, d: float, r: float) -> float:
-    """
-    Calculate the light isotope masses from bulk mass and delta value.
-    Arguments are m = mass, d= delta value, r = abundance ratio
-    """
-
-    l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-    return l
-
-
-def get_imass(m: float, d: float, r: float) -> [float, float]:
-    """
-    Calculate the isotope masses from bulk mass and delta value.
-    Arguments are m = mass, d= delta value, r = abundance ratio
-    species
-
-    """
-
-    l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-    h: float = m - l
-    return [l, h]
-
-
-# @njit()
-def get_frac(m: float, l: float, a: float) -> [float, float]:
-    """Calculate the effect of the istope fractionation factor alpha on
-    the ratio between the light and heavy isotope.
-
-    Note that alpha needs to be given as fractional value, i.e., 1.07 rather
-    than 70 (i.e., (alpha-1) * 1000
-
-    """
-
-    if a > 1.1 or a < 0.9:
-        raise ValueError("alpha needs to be given as fractional value not in permil")
-
-    li: float = -l * m / (a * l - a * m - l)
-    hi: float = m - li  # get the new heavy isotope value
-    return li, hi
-
-
-# @njit()
-def get_flux_data(m: float, d: float, r: float) -> np.ndarray:
-    """
-    Calculate the isotope masses from bulk mass and delta value.
-    Arguments are m = mass, d= delta value, r = abundance ratio
-    species. Unlike get_mass, this function returns the full array
-
-    """
-
-    l: float = (1000.0 * m) / ((d + 1000.0) * r + 1000.0)
-    h: float = m - l
-
-    return np.array([m, l, h, d])
-
-
-# @njit()
-def get_delta(l: np.ndarray, h: np.ndarray, r: float) -> np.ndarray:
-    """Calculate the delta from the mass of light and heavy isotope
-    Arguments are l and h which are the masses of the light and
-    heavy isotopes respectively, r = abundance ratio of the
-    respective element. Note that this equation can result in a
-    siginificant loss of precision (on the order of 1E-13). I
-    therefore round the results to numbers largers 1E12 (otherwise a
-    delta of zero may no longer be zero)
-
-    """
-
-    return 1000 * (h / l - r) / r
-
-
-def get_delta_i(l: float, h: float, r: float) -> float:
-    """Calculate the delta from the mass of light and heavy isotope
-    Arguments are l and h which are the masses of the light and
-    heavy isotopes respectively, r = abundance ratio of the
-    respective element. Note that this equation can result in a
-    siginificant loss of precision (on the order of 1E-13). I
-    therefore round the results to numbers largers 1E12 (otherwise a
-    delta of zero may no longer be zero)
-
-    """
-    # d = 1000 * (h / l - r) / r
-    if l > 0:
-        d: float = 1e3 * (h / l - r) / r
-    else:
-        d = 0
-    return d
-
-
-def get_flux_delta(f) -> float:
-    """Calculate the delta of flux f"""
-
-    m = f.fa[0]
-    l = f.fa[1]
-    h = m - l
-    r = f.species.r
-    d = 1e3 * (h / l - r) / r
-    return d
-
-
-def get_delta_h(h) -> float:
-    """Calculate the delta of a flux or reservoir from total mass
-    and mass of light isotope.
-
-    h = flux or reservoir handle
-
-    returns d a vector of delta values
-
-    """
-
-    r = h.species.r
-
-    d = np.where(h.l > 0, 1e3 * ((h.m - h.l) / h.l - r) / r, 0)
-
-    return d
-
-
-def execute(
-    time: np.ndarray,
-    lop: list,
-    lor: list,
-    lpc_f: list,
-    lpc_r: list,
-) -> None:
-    """This is the original object oriented solver"""
-
-    start: float = process_time()
-    i = 1  # some processes refer to the previous time step
-    for t in time[1:-1]:  # loop over the time vector except the first
-        # we first need to calculate all fluxes
-        # for r in lor:  # loop over all reservoirs
-        #     for p in r.lop:  # loop over reservoir processes
-        #         p(i)  # update fluxes
-
-        for p in lop:  # loop over reservoir processes
-            p(i)  # update fluxes
-
-        for p in lpc_f:  # update all process based fluxes.
-            p(i)
-
-        for r in lor:  # loop over all reservoirs
-            flux_list = r.lof
-
-            m = l = 0
-            for f in flux_list:  # do sum of fluxes in this reservoir
-                direction = r.lio[f]
-                m += f.fa[0] * direction  # current flux and direction
-                l += f.fa[1] * direction  # current flux and direction
-
-            r.m[i] = r.m[i - 1] + m * r.mo.dt
-            r.l[i] = r.l[i - 1] + l * r.mo.dt
-            r.c[i] = r.m[i] / r.v[i]
-
-        # update reservoirs which do not depend on fluxes but on
-        # functions
-        for p in lpc_r:
-            p(i)
-
-        i = i + 1
-
-    duration: float = process_time() - start
-    print(f"\n Execution time {duration:.2e} cpu seconds\n")
-
 
 def execute_e(model, lop, lor, lpc_f, lpc_r):
     """ """
 
     # numba.set_num_threads(2)
 
     # this has nothing todo with self.time below!
@@ -280,16 +88,17 @@
         )
 
     duration: float = process_time() - start
     wcd = time.time() - wts
     print(f"\n Total solver time {duration} cpu seconds, wt = {wcd}\n")
 
 
+
 # from numba import jit
-@njit(parallel=False, fastmath=True, error_model="numpy")
+# @njit(parallel=False, fastmath=True, error_model="numpy")
 def foo(fn_vr, input_data, vr_data, vr_params, fn, da, pc, a, b, c, d, e, maxt, dt):
     """
     fn = flux process list
     fn = typed list of functions (processes)
     da = process data
     pc = process parameters
     a = reservoir_list
@@ -297,18 +106,17 @@
     c = direction list
     d = virtual reservoir list
     e = r0 list ???
     """
 
     i = 1
     for t in maxt:
-
         # loop over function (process) list and compute fluxes
         j = 0
-        for f in enumerate(fn):
+        for _ in enumerate(fn):
             fn[j](da[j], pc[j], i)
             j = j + 1
 
         # calculate the resulting reservoir concentrations
         # summarize_fluxes(a, b, c, d, e, i, dt)
         r_steps: int = len(b)
         # loop over reservoirs
@@ -332,15 +140,15 @@
         # # functions
         for j, f in enumerate(fn_vr):
             fn_vr[j](i, input_data[j], vr_data[j], vr_params[j])
 
         i = i + 1  # next time step
 
 
-@njit(parallel=False, fastmath=True, error_model="numpy")
+# @njit(parallel=False, fastmath=True, error_model="numpy")
 def foo_no_p(fn_vr, input_data, vr_data, vr_params, fn, a, b, c, d, e, maxt, dt):
     """
     fn = flux process list
     fn = typed list of functions (processes)
     da = process data
     pc = process parameters
     a = reservoir_list
@@ -348,15 +156,14 @@
     c = direction list
     d = virtual reservoir list
     e = r0 list ???
     """
 
     i = 1
     for t in maxt:
-
         # calculate the resulting reservoir concentrations
         # summarize_fluxes(a, b, c, d, e, i, dt)
         r_steps: int = len(b)
         # loop over reservoirs
         for j in range(r_steps):
             # for j, r in enumerate(b):  # this will catch the list for each reservoir
 
@@ -377,15 +184,15 @@
         # # functions
         for j, f in enumerate(fn_vr):
             fn_vr[j](i, input_data[j], vr_data[j], vr_params[j])
 
         i = i + 1  # next time step
 
 
-@njit(parallel=False, fastmath=True, error_model="numpy")
+# @njit(parallel=False, fastmath=True, error_model="numpy")
 def foo_no_vr(fn, da, pc, a, b, c, d, e, maxt, dt):
     """Same as foo but no virtual reservoirs present
 
     fn = flux process list
     fn = typed list of functions (processes)
     da = process data
     pc = process parameters
@@ -394,18 +201,17 @@
     c = direction list
     d = virtual reservoir list
     e = r0 list ???
     """
 
     i = 1
     for t in maxt:
-
         # loop over processes
         j = 0
-        for f in enumerate(fn):
+        for _ in enumerate(fn):
             fn[j](da[j], pc[j], i)
             j = j + 1
 
         # calculate the resulting reservoir concentrations
         # summarize_fluxes(a, b, c, d, e, i, dt)
         r_steps: int = len(b)
         # loop over reservoirs
@@ -421,15 +227,15 @@
             a[j][0][i] = a[j][0][i - 1] + mass * dt  # mass
             a[j][1][i] = a[j][1][i - 1] + li * dt  # li
             a[j][2][i] = a[j][0][i] / a[j][3][i]  # c
 
         i = i + 1
 
 
-@njit(parallel=False, fastmath=True, error_model="numpy")
+# @njit(parallel=False, fastmath=True, error_model="numpy")
 def foo_no_vr_no_p(fn, a, b, c, d, e, maxt, dt):
     """Same as foo but no virtual reservoirs present
 
     fn = flux process list
     fn = typed list of functions (processes)
     da = process data
     pc = process parameters
@@ -437,19 +243,18 @@
     b = flux list
     c = direction list
     d = virtual reservoir list
     e = r0 list ???
     """
 
     i = 1
-    for t in maxt:
-
-        # calculate the resulting reservoir concentrations
-        # summarize_fluxes(a, b, c, d, e, i, dt)
-        r_steps: int = len(b)
+    # calculate the resulting reservoir concentrations
+    # summarize_fluxes(a, b, c, d, e, i, dt)
+    r_steps: int = len(b)
+    for _ in maxt:
         # loop over reservoirs
         for j in range(r_steps):
             mass = li = 0.0
             f_steps = len(b[j])
             for u in range(f_steps):
                 direction = c[j][u]
                 mass += b[j][u][0] * direction  # mass
@@ -480,15 +285,14 @@
             types.ListType(types.float64[::1]),
             types.ListType(types.float64),  # a3
         ).as_type()
     )
 
     count = 0
     for r in lvr:  # loop over reservoir processes
-
         func_name, in_d, vr_d, params = r.get_process_args()
         fn.append(func_name)
         input_data.append(in_d)
         vr_data.append(vr_d)
         vr_params.append(params)
         count = count + 1
 
@@ -543,15 +347,15 @@
     import numba
     from numba.core import types
 
     fn = List()  # List() # list of functions
     da = List()  # data
     pc = List()  # list of constants
 
-    print(f"Building Process List")
+    print("Building Process List")
 
     tfn = numba.typed.List.empty_list(
         types.ListType(types.void)(  # return value
             types.ListType(types.float64[::1]),  # data array
             types.ListType(types.float64),  # parameter list
             types.int64,  # parameter 4
         ).as_type()
@@ -568,7 +372,332 @@
         # print(f"working on {p.name}")
         func_name, data, proc_const = p.get_process_args()
         tfn.append(func_name)
         tda.append(data)
         tpc.append(proc_const)
 
     return tfn, tda, tpc
+
+
+def apply_fractionation(
+    f_m: str, c: Connection | Connect, icl: dict, ind3: str, ind2: str
+) -> str:
+    """If the connection involves isotope fractionation, add equation
+    string that calculates the fractionation effect.
+
+    :param f_m: string with the flux name
+    :param c: connection object
+    :param icl: dict of reservoirs that have actual fluxes
+    :param ind2: indent 2 times
+    :param ind3: indent 3 times
+
+    :raises ValueError: if alpha is not between 0.9 and 1.1
+
+    :returns eq: string with the fractionation equation
+
+    Calculate the flux of the light isotope (f_l) as a function of the isotope
+    ratios in the source reservoir soncentrations (s_c, s_l), and alpha (a) as
+
+    f_l = s_l * f_m/ (a * s_c + s_l - a * s_l)
+    """
+
+    a = c.alpha / 1000 + 1
+    s_c = get_ic(c.source, icl)
+    s_l = get_ic(c.source, icl, isotopes=True)
+
+    if int(c.alpha) != 0:
+        eq = f"(\n{ind3} {s_l} * {f_m}\n{ind3} / ({a} * {s_c} + {s_l} - {a} * {s_l}))"
+    else:
+        eq = f"(\n{ind3} {f_m} * {s_l} / {s_c})"
+    return eq
+
+
+def apply_delta(
+    f_m: str, c: Connection | Connect, icl: dict, ind3: str, ind2: str
+) -> str:
+    """If the connection involves a fixed deltae offset add equation
+    string according to the delta value
+
+    :param f_m: string with the flux name
+    :param c: connection object
+    :param icl: dict of reservoirs that have actual fluxes
+    :param ind2: indent 2 times
+    :param ind3: indent 3 times
+
+    :raises ValueError: if alpha is not between 0.9 and 1.1
+
+    :returns eq: string with the fractionation equation
+
+    Calculate the flux of the light isotope (f_l) as a function of the isotope
+    ratios in the source reservoir soncentrations (s_c, s_l), and alpha (a) as
+
+    f_l = f_m * 1000/(r * (d + 1000) + 1000)
+    """
+    r = c.source.species.r
+    d = c.delta
+    exl = f"(\n" f"{ind3}{f_m} * 1000\n" f"{ind3} / ({r} * ({d} + 1000) + 1000))\n"
+    return exl
+
+
+# @njit(parallel=False, fastmath=True, error_model="numpy")
+def calc_carbonates_1(i: int, input_data: List, vr_data: List, params: List) -> None:
+    """Calculates and returns the carbonate concentrations and saturation state
+     at the ith time-step of the model.
+
+    The function assumes that vr_data will be in the following order:
+        [H+, CA, HCO3, CO3, CO2(aq), omega]
+
+    LIMITATIONS:
+    - This in used in conjunction with ExternalCode objects!
+    - Assumes all concentrations are in mol/kg
+    - Assumes your Model is in mol/kg ! Otherwise, DIC and TA updating will not
+    be correct.
+
+    Calculations are based off equations from:
+    Boudreau et al., 2010, https://doi.org/10.1029/2009GB003654
+    Follows, 2006, doi:10.1016/j.ocemod.2005.05.004
+
+    See add_carbonate_system_1 in utility_functions.py on how to call this function
+
+    Author: M. Niazi & T. Tsan, 2021
+    """
+
+    k1 = params[0]  # K1
+    k2 = params[1]  # K2
+    KW = params[2]  # KW
+    KB = params[3]  # KB
+    boron = params[4]  # boron
+    ca2 = params[5]  # Ca2+
+    ksp = params[6]  # Ksp
+
+    dic: float = input_data[0][i - 1]
+    ta: float = input_data[1][i - 1]
+    hplus: float = vr_data[0][i - 1]
+
+    # calculates carbonate alkalinity (ca) based on H+ concentration from the
+    # previous time-step
+    oh: float = KW / hplus
+    boh4: float = boron * KB / (hplus + KB)
+    fg: float = hplus - oh - boh4
+    ca: float = ta + fg
+
+    # hplus
+    gamm: float = dic / ca
+    dummy: float = (1 - gamm) * (1 - gamm) * k1 * k1 - 4 * k1 * k2 * (1 - (2 * gamm))
+
+    hplus: float = 0.5 * ((gamm - 1) * k1 + (dummy**0.5))
+    # hco3 and co3
+    """ Since CA = [hco3] + 2[co3], can the below expression can be simplified
+    """
+    # co3: float = dic / (1 + (hplus / k2) + ((hplus ** 2) / (k1 * k2)))
+    hco3: float = dic / (1 + (hplus / k1) + (k2 / hplus))
+    co3: float = (ca - hco3) / 2
+    # co2 (aq)
+    """DIC = hco3 + co3 + co2 + H2CO3 The last term is however rather
+    small, so it may be ok to simply write co2aq = dic - hco3 + co3.
+    Let's test this once we have a case where pco2 is calculated from co2aq
+    """
+    #  co2aq: float = dic / (1 + (k1 / hplus) + (k1 * k2 / (hplus ** 2)))
+    co2aq: float = dic - hco3 - co3
+    # omega: float = ca2 * co3 / ksp
+
+    vr_data[0][i] = hplus
+    vr_data[1][i] = ca
+    vr_data[2][i] = hco3
+    vr_data[3][i] = co3
+    vr_data[4][i] = co2aq
+    # vr_data[5][i] = oh
+    # vr_data[5][i] = boh4
+    # vr_data[5][i] = omega
+
+
+# @njit(fastmath=True, error_model="numpy")
+def calc_carbonates_2(i: int, input_data: List, vr_data: List, params: List) -> None:
+    """Calculates and returns the carbonate concentrations and carbonate compensation
+    depth (zcc) at the ith time-step of the model.
+
+    The function assumes that vr_data will be in the following order:
+        [H+, CA, HCO3, CO3, CO2(aq), zsat, zcc, zsnow, Fburial,
+        B, BNS, BDS_under, BDS_resp, BDS, BCC, BPDC, BD,omega]
+
+    LIMITATIONS:
+    - This in used in conjunction with ExternalCode objects!
+    - Assumes all concentrations are in mol/kg
+    - Assumes your Model is in mol/kg ! Otherwise, DIC and TA updating will not
+    be correct.
+
+    Calculations are based off equations from:
+    Boudreau et al., 2010, https://doi.org/10.1029/2009GB003654
+    Follows, 2006, doi:10.1016/j.ocemod.2005.05.004
+
+    See add_carbonate_system_2 in utility_functions.py on how to call this function.
+    The input data is a follows
+
+        reservoir DIC.m,  # 0
+        reservoir DIC.l,  # 1
+        reservoir DIC.c,  # 2
+        reservoir TA.m,  # 3 TA mass
+        reservoir.TA.c,  # 4 TA concentration
+        Export_flux.fa,  # 5
+        area_table,  # 6
+        area_dz_table,  # 7
+        Csat_table,  # 8
+        reservoir.DIC.v,  # 9 reservoir volume
+
+    Author: M. Niazi & T. Tsan, 2021
+    """
+
+    # Parameters
+    k1 = params[0]
+    k2 = params[1]
+    KW = params[2]
+    KB = params[3]
+    boron = params[4]
+    ksp0 = params[5]
+    kc = params[6]
+    AD = params[8]
+    zsat0 = int(abs(params[9]))
+    ca2 = params[10]
+    dt = params[11]
+    I_caco3 = params[12]
+    alpha = params[13]
+    zsat_min = int(abs(params[14]))
+    zmax = int(abs(params[15]))
+    z0 = int(abs(params[16]))
+
+    # Data
+    dic: float = input_data[2][i - 1]  # DIC concentration [mol/kg]
+    ta: float = input_data[4][i - 1]  # TA concentration [mol/kg]
+    Bm: float = input_data[5][0]  # Carbonate Export Flux [mol/yr]
+    B12: float = input_data[5][1]  # Carbonate Export Flux light isotope
+    v: float = input_data[9][i - 1]  # volume
+    # lookup tables
+    depth_area_table: np.ndarray = input_data[6]  # depth look-up table
+    area_dz_table: np.ndarray = input_data[7]  # area_dz table
+    Csat_table: np.ndarray = input_data[8]  # Csat table
+
+    # vr_data
+    hplus: float = vr_data[0][i - 1]  # H+ concentration [mol/kg]
+    zsnow = vr_data[7][i - 1]  # previous zsnow
+
+    # calc carbonate alkalinity based t-1
+    oh: float = KW / hplus
+    boh4: float = boron * KB / (hplus + KB)
+    fg: float = hplus - oh - boh4
+    ca: float = ta + fg
+
+    # calculate carbon speciation
+    # The following equations are after Follows et al. 2006
+    gamm: float = dic / ca
+    dummy: float = (1 - gamm) * (1 - gamm) * k1 * k1 - 4 * k1 * k2 * (1 - (2 * gamm))
+
+    hplus: float = 0.5 * ((gamm - 1) * k1 + (dummy**0.5))
+    # co3: float = dic / (1 + (hplus / k2) + ((hplus ** 2) / (k1 * k2)))
+    hco3: float = dic / (1 + (hplus / k1) + (k2 / hplus))
+    co3: float = (ca - hco3) / 2
+    # DIC = hco3 + co3 + co2 + H2CO3 The last term is however rather
+    # small, so it may be ok to simply write co2aq = dic - hco3 + co3.
+    co2aq: float = dic - co3 - hco3
+    # co2aq: float = dic / (1 + (k1 / hplus) + (k1 * k2 / (hplus ** 2)))
+    # omega: float = (ca2 * co3) / ksp
+
+    # ---------- compute critical depth intervals eq after  Boudreau (2010)
+    # all depths will be positive to facilitate the use of lookup_tables
+
+    # prevent co3 from becoming zero
+    if co3 <= 0:
+        co3 = 1e-16
+
+    zsat = int(max((zsat0 * np.log(ca2 * co3 / ksp0)), zsat_min))  # eq2
+    if zsat < zsat_min:
+        zsat = int(zsat_min)
+
+    zcc = int(zsat0 * np.log(Bm * ca2 / (ksp0 * AD * kc) + ca2 * co3 / ksp0))  # eq3
+
+    # ---- Get fractional areas
+    B_AD = Bm / AD
+
+    if zcc > zmax:
+        zcc = int(zmax)
+    if zcc < zsat_min:
+        zcc = zsat_min
+
+    A_z0_zsat = depth_area_table[z0] - depth_area_table[zsat]
+    A_zsat_zcc = depth_area_table[zsat] - depth_area_table[zcc]
+    A_zcc_zmax = depth_area_table[zcc] - depth_area_table[zmax]
+
+    # ------------------------Calculate Burial Fluxes------------------------------------
+    # BCC = (A(zcc, zmax) / AD) * B, eq 7
+    BCC = A_zcc_zmax * B_AD
+
+    # BNS = alpha_RD * ((A(z0, zsat) * B) / AD) eq 8
+    BNS = alpha * A_z0_zsat * B_AD
+
+    # BDS_under = kc int(zcc,zsat) area' Csat(z,t) - [CO3](t) dz, eq 9a
+    diff_co3 = Csat_table[zsat:zcc] - co3
+    area_p = area_dz_table[zsat:zcc]
+
+    BDS_under = kc * area_p.dot(diff_co3)
+    BDS_resp = alpha * (A_zsat_zcc * B_AD - BDS_under)
+    BDS = BDS_under + BDS_resp
+
+    # BPDC =  kc int(zsnow,zcc) area' Csat(z,t) - [CO3](t) dz, eq 10
+    if zcc < zsnow:  # zcc cannot
+        if zsnow > zmax:  # zsnow cannot exceed ocean depth
+            zsnow = zmax
+
+        diff = Csat_table[zcc : int(zsnow)] - co3
+        area_p = area_dz_table[zcc : int(zsnow)]
+
+        BPDC = kc * area_p.dot(diff)
+        zold = BPDC / (area_dz_table[int(zsnow)] * I_caco3) * dt
+        # eq 4 dzsnow/dt = Bpdc(t) / (a'(zsnow(t)) * ICaCO3
+        zsnow = zsnow - BPDC / (area_dz_table[int(zsnow)] * I_caco3) * dt
+
+    else:  # zcc > zsnow
+        # there is no carbonate below zsnow, so BPDC = 0
+        zsnow = zcc
+        BPDC = 0
+
+    # BD & F_burial
+    BD: float = BDS + BCC + BNS + BPDC
+    Fburial = Bm - BD
+    Fburial_l = Fburial * input_data[1][i - 1] / input_data[0][i - 1]
+    diss = (Bm - Fburial) * dt  # dissolution flux
+    diss12 = (B12 - Fburial_l) * dt  # dissolution flux light isotope
+
+    # # print("{Fburial}.format(")
+    # print(Bm)
+    # print(Fburial)
+    # print(diss)
+    # print()
+    # # print('df ={:.2e}\n'.format(diss/dt))
+
+    """ Now that the fluxes are known we need to update the reservoirs.
+    The concentration in the in the DIC (and TA) of this box are
+    DIC.m[i] + Export Flux - Burial Flux, where the isotope ratio
+    the Export flux is determined by the overlying box, and the isotope ratio
+    of the burial flux is determined by the isotope ratio of this box
+    """
+
+    # Update DIC in the deep box
+    input_data[0][i] = input_data[0][i] + diss  # DIC
+    input_data[1][i] = input_data[1][i] + diss12  # 12C
+    input_data[2][i] = input_data[0][i] / v  # DIC concentration
+
+    # Update TA in deep box
+    input_data[3][i] = input_data[3][i] + 2 * diss  # TA
+    input_data[4][i] = input_data[3][i] / v  # TA concentration
+
+    # copy results into datafields
+    vr_data[0][i] = hplus  # 0
+    vr_data[1][i] = ca  # 1
+    vr_data[2][i] = hco3  # 2
+    vr_data[3][i] = co3  # 3
+    vr_data[4][i] = co2aq  # 4
+    vr_data[5][i] = zsat  # 5
+    vr_data[6][i] = zcc  # 6
+    vr_data[7][i] = zsnow  # 7
+    vr_data[8][i] = Fburial  # 8
+    vr_data[9][i] = Fburial_l  # 9
+    vr_data[10][i] = diss / dt  # 9
+    vr_data[11][i] = Bm  # 9
```

### Comparing `esbmtk-0.8.0.0/esbmtk/species_definitions.py` & `esbmtk-0.9.0.1/esbmtk/species_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,18 +187,19 @@
         name="BOH3", element=eh, display_as=r"B(OH)$_{3}$", register=eh
     )  # Boric Acid
     Species(
         name="BOH4", element=eh, display_as=r"B(OH)$_{4}^{-}$", register=eh
     )  # Borate
 
 
-def distance_variables(model):
+def misc_variables(model):
     eh = Element(
-        name="distance_variables",
+        name="misc_variables",
         model=model,  # model handle
         mass_unit="m",  # base mass unit
         register=model,
     )
 
     # add species
     Species(name="zsnow", element=eh, display_as="zsnow", register=eh)
+    Species(name="zcc", element=eh, display_as="zcc", register=eh)
     # Name & element handle
```

### Comparing `esbmtk-0.8.0.0/esbmtk/utility_functions.py` & `esbmtk-0.9.0.1/esbmtk/utility_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,68 +11,59 @@
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-# import typing as tp
-from numba.typed import List
+from __future__ import annotations
 import numpy as np
 import matplotlib.pyplot as plt
 import logging
 import typing as tp
 from collections import OrderedDict
 from esbmtk import Q_
 
-# import builtins
-# import math
+if tp.TYPE_CHECKING:
+    from esbmtk import Flux, Model, Connection, Connect
 
 np.set_printoptions(precision=4)
 
 
 def find_matching_strings(s: str, fl: list[str]) -> bool:
     """test if all elements of fl occur in s. Return True if yes,
     otherwise False
 
     """
-    for f in fl:
-        if f not in s:
-            return False
-
-    return True
+    return all(f in s for f in fl)
 
 
 def insert_into_namespace(name, value, name_space=globals()):
     name_space[name] = value
 
 
 def add_to(l, e):
     """
     add element e to list l, but check if the entry already exist. If so, throw
     exception. Otherwise add
     """
 
-    if not (e in l):  # if not present, append element
+    if e not in l:  # if not present, append element
         l.append(e)
 
 
 def get_plot_layout(obj):
     """Simple function which selects a row, column layout based on the number of
     objects to display.  The expected argument is a reservoir object which
     contains the list of fluxes in the reservoir
 
     """
 
-    noo = 1  # the reservoir is the fisrt object
-    for f in obj.lof:  # count numbert of fluxes
-        if f.plot == "yes":
-            noo += 1
-
-    for d in obj.ldf:  # count number of data fields
+    noo = 1 + sum(f.plot == "yes" for f in obj.lof)
+    for _ in obj.ldf:
         noo += 1
 
     # noo = len(obj.lof) + 1  # number of objects in this reservoir
     logging.debug(f"{noo} subplots for {obj.n} required")
 
     size, geo = plot_geometry(noo)
 
@@ -145,23 +136,16 @@
 
     index :int = 0 starting index
     indent :int = 0 indentation
     """
 
     off: str = "  "
 
-    if "index" not in kwargs:
-        index = 0
-    else:
-        index = kwargs["index"]
-
-    if "indent" in kwargs:
-        ind: str = kwargs["indent"] * " "
-    else:
-        ind: str = ""
+    index = 0 if "index" not in kwargs else kwargs["index"]
+    ind: str = kwargs["indent"] * " " if "indent" in kwargs else ""
 
     # show the first 4 entries
     # for i in range(index, index + 3):
     #     print(f"{off}{ind}i = {i}, Mass = {self.m[i]:.2e}, li= {self.l[i]:.2f}")
 
 
 def set_y_limits(ax: plt.Axes, obj: any) -> None:
@@ -174,19 +158,15 @@
         top = bottom + obj.display_precision
         ax.set_ylim(bottom, top)
 
 
 def is_name_in_list(n: str, l: list) -> bool:
     """Test if an object name is part of the object list"""
 
-    r: bool = False
-    for e in l:
-        if e.full_name == n:
-            r = True
-    return r
+    return any(e.full_name == n for e in l)
 
 
 def get_object_from_list(name: str, l: list) -> any:
     """Match a name to a list of objects. Return the object"""
 
     match: bool = False
     for o in l:
@@ -221,59 +201,61 @@
                 a.append(e)  # add to temporary list
                 lc.remove(e)  # remove this element
 
         rl.append(a)  # save the temporary list to rl
 
     # at this point, all elements of lc should have been processed
     # if not, lc contains element which are of a different type
-    if len(lc) > 0:
+    if lc:
         raise TypeError(m)
 
     return rl
 
 
-def get_object_handle(res, M):
-    """Test if we the key is a global reservoir handle
+def get_object_handle(res: list | string | Reservoir | ReservoirGroup, M: Model):
+    """Test if the key is a global reservoir handle
     or exists in the model namespace
 
-    res: list, str, or reservoir handle
-    M: Model handle
+    :param res: list of strings, or reservoir handles
+    :param M: Model handle
     """
 
-    rlist: list = []
+    r_list: list = []
 
     if not isinstance(res, list):
         res = [res]
-
     for o in res:
+        # print(f"goh0: looking up {o} of {type(o)}")
         if o in M.dmo:  # is object known in global namespace
-            rlist.append(M.dmo[o])
+            r_list.append(M.dmo[o])
+            # print(f"goh1: found {o} in dmo")
         elif o in M.__dict__:  # or does it exist in Model namespace
-            rlist.append(getattr(M, o))
+            r_list.append(getattr(M, o))
+            # print(f"goh2: found {o} in __dict__\n")
         else:
-            raise ValueError(f"{o} is not known for model {M.name}")
+            print(f"{o} is not known for model {M.name}")
+            # raise ValueError(f"{o} is not known for model {M.name}")
 
-    if len(rlist) == 1:
-        rlist = rlist[0]
+    if len(r_list) == 1:
+        r_list = r_list[0]
 
-    return rlist
+    return r_list
 
 
 def split_key(k: str, M: any) -> tp.Union[any, any, str]:
     """split the string k with letters _to_, and test if optional
     id string is present
 
     """
 
-    if "_to_" in k:
-        source = k.split("_to_")[0]
-        sinkandid = k.split("_to_")[1]
-    else:
+    if "_to_" not in k:
         raise ValueError("Name must follow 'Source_to_Sink' format")
 
+    source = k.split("_to_")[0]
+    sinkandid = k.split("_to_")[1]
     if "@" in sinkandid:
         sink = sinkandid.split("@")[0]
         cid = sinkandid.split("@")[1]
     else:
         sink = sinkandid
         cid = ""
 
@@ -284,35 +266,35 @@
 
 
 def make_dict(keys: list, values: list) -> dict:
     """Create a dictionary from a list and value, or from
     two lists
 
     """
-    d = dict()
+    d = {}
 
     if isinstance(values, list):
         if len(values) == len(keys):
             d: dict = dict(zip(keys, values))
         else:
             print(f"len values ={len(values)}, len keys ={len(keys)}")
             print(f"values = {values}")
             for k in keys:
                 print(f"key = {k}")
-            raise ValueError(f"key and value list must be of equal length")
+            raise ValueError("key and value list must be of equal length")
     else:
         values: list = [values] * len(keys)
         d: dict = dict(zip(keys, values))
 
     return d
 
 
 def get_typed_list(data: list) -> list:
 
-    tl = List()
+    tl = list()
     for x in data:
         tl.append(x)
     return tl
 
 
 def create_reservoirs(bn: dict, ic: dict, M: any) -> dict:
     """boxes are defined by area and depth interval here we use an ordered
@@ -349,15 +331,18 @@
     for k, v in bn.items():
         # test key format
         if M.name in k:
             k = k.split(".")[1]
 
         if "ty" in v:  # type is given
             if v["ty"] == "Source":
-                SourceGroup(name=k, species=v["sp"], register=M)
+                if "delta" in v:
+                    SourceGroup(name=k, species=v["sp"], delta=v["delta"], register=M)
+                else:
+                    SourceGroup(name=k, species=v["sp"], register=M)
             elif v["ty"] == "Sink":
                 SinkGroup(name=k, species=v["sp"], register=M)
             else:
                 raise ValueError("'ty' must be either Source or Sink")
 
         else:  # create reservoirs
 
@@ -406,21 +391,21 @@
     icd: dict = OrderedDict()
     td1: dict = {}  # temp dictionary
     td2: dict = {}  # temp dictionary
     td3: dict = {}  # temp dictionary
 
     # create the dicts for concentration and isotopes
     for k, v in cd.items():
-        td1.update({k: v[0]})
-        td2.update({k: v[1]})
-        td3.update({k: v[2]})
+        td1[k] = v[0]
+        td2[k] = v[1]
+        td3[k] = v[2]
 
     # box_names: list = bg.keys()
     for bn in box_names:  # loop over box names
-        icd.update({bn: [td1, td2, td3]})
+        icd[bn] = [td1, td2, td3]
 
     return icd
 
 
 def calc_volumes(bg: dict, M: any, h: any) -> list:
     """Calculate volume contained in a given depth interval
     bg is an ordered dictionary in the following format
@@ -441,15 +426,15 @@
 
     """
 
     # from esbmtk import hypsometry
 
     v: list = []  # list of volumes
 
-    for k, v in bg.items():
+    for v in bg.values():
         a = v[0]
         u = v[1]
         l = v[2]
 
         v.append(h.volume(u, l) * a)
 
     return v
@@ -461,28 +446,26 @@
     p_length = 0  # length of single parameter
     nl = 0  # number of lists
     ll = []
 
     # we need to cover the case where we have two lists of different length
     # this happens if we have a long list of tuples with matched references,
     # as well as a list of species
-    for k, v in d.items():
+    for v in d.values():
         if isinstance(v, list):
             nl = nl + 1
             if len(v) > l_length:
                 l_length = len(v)
                 ll.append(l_length)
 
         else:
             p_length = 1
 
-    if nl > 1:
-        # if lists have different lengths
-        if ll.count(l_length) != len(ll):
-            raise ValueError("Mapping for multiple lists is not supported")
+    if nl > 1 and ll.count(l_length) != len(ll):
+        raise ValueError("Mapping for multiple lists is not supported")
 
     if l_length > 0 and p_length == 0:
         case = 0  # Only lists present
     if l_length == 0 and p_length == 1:
         case = 1  # Only parameters present
     if l_length > 0 and p_length == 1:
         case = 2  # Lists and parameters present
@@ -495,33 +478,27 @@
     that they are all lists of equal length
 
     """
     cd = d.copy()
 
     for k, v in cd.items():
         if not isinstance(v, list):
-            p = []
-            for i in range(l):
-                p.append(v)
+            p = [v for _ in range(l)]
             d[k] = p
 
     return d
 
 
 def get_sub_key(d: dict, i: int) -> dict:
     """take a dict which has where the value is a list, and return the
     key with the n-th value of that list
 
     """
 
-    rd: dict = {}
-    for k, v in d.items():
-        rd[k] = v[i]
-
-    return rd
+    return {k: v[i] for k, v in d.items()}
 
 
 def expand_dict(d: dict, mt: str = "1:1") -> int:
     """Determine dict structure
 
     in case we have mutiple connections with mutiple species, the
     default action is to map connections to species (t = '1:1'). If
@@ -589,43 +566,42 @@
 
                 for t in ck:  # apply the entire nd dict to all connections
                     rd[t] = nd
             else:
                 raise ValueError(f"{mt} is not defined. must be '1:1' or '1:N'")
 
         else:
-            if case == 0:  # only lists present, case 3
-                nd = cd
-            elif case == 1:  # only parameters present
+            if case in [0, 1]:  # only lists present, case 3
                 nd = cd
             elif case == 2:  # list and parameters present case 4
                 nd = convert_to_lists(cd, length)
             rd[ck] = nd
 
         # update the overall dict and move to the next entry
-        r.update(rd)
+        r |= rd
 
     return r
 
 
-def create_bulk_connections(ct: dict, M: any, mt: int = "1:1") -> None:
+def create_bulk_connections(ct: dict, M: Model, mt: int = "1:1") -> dict:
     """Create connections from a dictionary. The dict can have the following keys
     following format:
 
     mt = mapping type. See below for explanation
 
     # na: names, tuple or str. If lists, all list elements share the same properties
     # sp: species list or species
     # ty: type, str
     # ra: rate, Quantity
     # sc: scale, Number
     # re: reference, optional
     # al: alpha, optional
     # de: delta, optional
     # bp: bypass, see scale_with_flux
+    # si: signal
     # mx: True, optional defaults to False. If set, it will create forward
           and backward fluxes (i.e. mixing)
 
     There are 6 different cases how to specify connections
 
     Case 1 One connection, one set of parameters
            ct1 = {"sb2hb": {"ty": "scale", 'ra'....}}
@@ -680,60 +656,63 @@
             for c in k:
                 create_connection(c, v, M)
         elif isinstance(k, str):
             create_connection(k, v, M)
         else:
             raise ValueError(f"{c} must be string or tuple")
 
-    return ct
-
+    return c_ct
 
-def create_connection(n: str, p: dict, M: any) -> None:
-    """called by create_bulk_connections in order to create a connection
-    group It is assumed that all rates are in liter/year or mol per
-    year. This may not be what you want or need.
-
-    n: a connection key e.g., sb2db@mix which will be
-    interpreted as mixing a connection between sb and db and thus
-    create connections in both directions
-
-    p: a dictionary holding  the connection properties
-
-    M: the model handle
 
+def create_connection(n: str, p: dict, M: Model) -> None:
+    """called by create_bulk_connections in order to create a connection group
+    It is assumed that all rates are in liter/year or mol per year.  This may
+    not be what you want or need.
+
+    :param n: a connection key.  if the mix flag is given interpreted as mixing
+              a connection between sb and db and thus create connections in both
+              directions
+    :param p: a dictionary holding the connection properties
+    :param M: the model handle
     """
 
     from esbmtk import ConnectionGroup, Q_
 
+    # print(f"cc00: {n}",flush=True)
     # get the reservoir handles by splitting the key
     source, sink, cid = split_key(n, M)
+    # print(f"cc0: type of key {type(n)}", flush=True)
+    # print(f"cc1: key = {n}, source = {source}, sink = {sink}", flush=True)
+
     # create default connections parameters and replace with values in
     # the parameter dict if present.
     los = list(p["sp"]) if isinstance(p["sp"], list) else [p["sp"]]
     ctype = "None" if "ty" not in p else p["ty"]
     scale = 1 if "sc" not in p else p["sc"]
     rate = Q_("0 mol/a") if "ra" not in p else p["ra"]
     ref_flux = "None" if "re" not in p else p["re"]
     alpha = "None" if "al" not in p else p["al"]
     delta = "None" if "de" not in p else p["de"]
     cid = f"{cid}"
     bypass = "None" if "bp" not in p else p["bp"]
     species = "None" if "sp" not in p else p["sp"]
+    signal = "None" if "si" not in p else p["si"]
 
     if isinstance(scale, Q_):
         scale = scale.to("l/a").magnitude
 
     # expand arguments
     ctype = make_dict(los, ctype)
     scale = make_dict(los, scale)  # get rate from dictionary
     rate = make_dict(los, rate)
     ref_flux = make_dict(los, ref_flux)
     alpha = make_dict(los, alpha)
     delta = make_dict(los, delta)
     bypass = make_dict(los, bypass)
+    signal = make_dict(los, signal)
 
     # name of connectiongroup
     name = f"{M.name}.CG_{source.name}_to_{sink.name}"
     if f"{name}" in M.lmo:  # Test if CG exists
         # retriece CG object
         cg = getattr(M, name.split(".")[1])
         cg.add_connections(
@@ -743,75 +722,64 @@
             scale=scale,  # get rate from dictionary
             rate=rate,
             ref_flux=ref_flux,
             alpha=alpha,
             delta=delta,
             bypass=bypass,
             register=M,
+            signal=signal,
             id=cid,  # get id from dictionary
         )
     else:  # Create New ConnectionGroup
         cg = ConnectionGroup(
             source=source,
             sink=sink,
             ctype=ctype,
             scale=scale,  # get rate from dictionary
             rate=rate,
             ref_flux=ref_flux,
             alpha=alpha,
             delta=delta,
             bypass=bypass,
             register=M,
+            signal=signal,
             id=cid,  # get id from dictionary
         )
 
 
 def get_name_only(o: any) -> any:
     """Test if item is an esbmtk type. If yes, extract the name"""
 
     from esbmtk import Flux, Reservoir, ReservoirGroup, Species
 
-    # from esbmtk import Sink, Source, SourceGroup, SinkGroup
-    # from esbmtk import Process, DataField, VirtualReservoir
-
-    if isinstance(o, (Flux, Reservoir, ReservoirGroup, Species)):
-        r = o.full_name
-    else:
-        r = o
-
-    return r
+    return (
+        o.full_name if isinstance(o, (Flux, Reservoir, ReservoirGroup, Species)) else o
+    )
 
 
 def get_simple_list(l: list) -> list:
     """return a list which only has the full name
     rather than all the object properties
 
     """
 
-    r: list = []
-    for e in l:
-        r.append(get_name_only(e))
-
-    return r
+    return [get_name_only(e) for e in l]
 
 
 def show_dict(d: dict, mt: str = "1:1") -> None:
     """show dict entries in an organized manner"""
 
     from esbmtk import expand_dict, get_simple_list, get_name_only
 
     ct = expand_dict(d, mt)
     for ck, cv in ct.items():
         print(f"{ck}")
 
         for pk, pv in cv.items():
-            if isinstance(pv, list):
-                x = get_simple_list(pv)
-            else:
-                x = get_name_only(pv)
+            x = get_simple_list(pv) if isinstance(pv, list) else get_name_only(pv)
             print(f"     {pk} : {x}")
 
 
 def find_matching_fluxes(l: list, filter_by: str, exclude: str) -> list:
     """Loop over all reservoir in l, and extract the names of all fluxes
     which match the filter string. Return the list of names (not objects!)
 
@@ -826,132 +794,132 @@
 
     return list(lof)
 
 
 def reverse_key(key: str) -> str:
     """reverse a connection key e.g., sb2db@POM becomes db2sb@POM"""
 
-    # print(f"key = {key}")
-    l = key.split("@")
-    left = l[0]
-    # right = l[1]
+    left = key.split("@")
+    left = left[0]
     rs = left.split("_to_")
     r1 = rs[0]
     r2 = rs[1]
 
     return f"{r2}_to_{r1}"
 
 
 def get_connection_keys(
-    s: set, fstr: str, nstr: str, inverse: bool, exclude: str
-) -> list:
-    """extract connection keys from set of flux names, replace fstr with
-    nstr so that the key can be used in create_bulk_connnections()
+    f_list: set,
+    ref_id: str,
+    target_id: str,
+    inverse: bool,
+    exclude: str,
+) -> list[str]:
+    """
+    extract connection keys from set of flux names, replace ref_id with
+    target_id so that the key can be used in create_bulk_connnections()
+
+    :param f_list: a set with flux objects
+    :param ref_id: string with the reference id
+    :param target_id: string with the target_id
+    :param inverse: Bool, optional, defaults to false
+
+    :return cnc_l: a list of connection keys (str)
 
     The optional inverse parameter, can be used where in cases where the
     flux direction needs to be reversed, i.e., the returned key will not read
     sb2db@POM, but db2s@POM
-
-    E.g., if
-
-    s = ( M4.CG_P_sb2P_ib.PO4.POP_F)
-    fstr = "POP"
-    nstr = "POM_DIC"
-
-    M4.CG_P_sb2P_ib.PO4.POP_F will become
-
-    P_sb_to_P_ib@POM_DIC
-
     """
 
-    cl: list = []
+    cnc_l: list = []  # list of connection keys
 
-    for n in s:
+    for f in f_list:
         # get connection and flux name
-        l = n.full_name.split(".")
-        cn = l[1][3:]  # get key without leadinf C_
+        fns = f.full_name.split(".")
+        cnc = fns[1][3:]  # get key without leadinf C_
+        # print()
+        # print(f"gck0: flux = {f.full_name}, key = {cnc}")
+        # print(f"gck1: ref_id = {ref_id}, target_id = {target_id}")
         if inverse:
-            cn = reverse_key(cn)
-        cn.replace(fstr, nstr)
-        cn = f"{cn}_to_{nstr}"
-        cl.append(cn)
-
-    return cl
-
+            cnc = reverse_key(cnc)
 
-def gen_dict_entries(M: any, **kwargs) -> tuple:
-    """find all fluxes which contain the reference string, and create
-    matching keys which contain the target string. The function will
-    return two lists, which can be used to create a dict for the
-    create_bulk_connnection function.
+        cnc.replace(ref_id, target_id)
+        # create new cnc string
+        cnc = f"{cnc}_to_{target_id}"
+        # fix id vs connection Name
+        # parts = cnc.split('_to_')
+        # cnc = f"{parts[0]}@{parts[1]}"
+        # print(f"gck3: cnc = {cnc}")
+        cnc_l.append(cnc)
+
+    return cnc_l
+
+
+def gen_dict_entries(M: Model | list, **kwargs) -> tuple(tuple, list):
+    """Find all fluxes that contain the reference string, and create a new
+    Connection instance that connects the flux matching ref_id, with a flux
+    matching target_id.  The function will a tuple containig the new connection
+    keys that can be used by the create bulk_connection() function.  The second
+    return value is a list containing the reference fluxes.
 
-    E.g., to create a dict which will create new fluxes based on
-    existing fluxes
-
-    dk:list, fl:list = gen_dict_entries(ref_id = 'POP', target_id = 'POM')
-
-    this will find all fluxes with the POP-id and put these into
-    fl. It will also generate a list with suitable connections keys
-    (dk) which contain the 'POM' id.
-
-    The optional inverse parameter, can be used where in cases where the
-    flux direction needs to be reversed, i.e., the returned key will not read
+    The optional inverse parameter, can be used where in cases where the flux
+    direction needs to be reversed, i.e., the returned key will not read
     sb_to_dbPOM, but db_to_sb@POM
 
+    :param M: Model or list
+    :param **kwargs: keyword dictionary, known keys are ref_id, and raget_id,
+        inverse
+
+    :return f_list: List of fluxes that match ref_id
+    :return k_tuples: tuple of connection keys
     """
 
     from esbmtk import Model
 
-    reference = kwargs["ref_id"]
-    target = kwargs["target_id"]
-    if "inverse" in kwargs:
-        inverse = kwargs["inverse"]
-    else:
-        inverse = False
-
-    if "exclude" in kwargs:
-        exclude_str = kwargs["exclude"]
-    else:
-        exclude_str = "None"
+    ref_id = kwargs["ref_id"]
+    target_id = kwargs["target_id"]
+    inverse = kwargs.get("inverse", False)
+    exclude_str = kwargs.get("exclude", "None")
 
+    # find matching fluxes
     if isinstance(M, Model):
-        flist: list = find_matching_fluxes(
-            M.loc, filter_by=reference, exclude=exclude_str
+        f_list: list = find_matching_fluxes(
+            M.loc,
+            filter_by=ref_id,
+            exclude=exclude_str,
         )
     elif isinstance(M, list):
-        flist: list = find_matching_fluxes(
+        f_list: list = find_matching_fluxes(
             M,
-            filter_by=reference,
+            filter_by=ref_id,
             exclude=exclude_str,
         )
     else:
         raise ValueError(f"gen_dict_entries: M must be list or Model, not {type(M)}")
 
-    klist: list = get_connection_keys(flist, reference, target, inverse, exclude_str)
+    k_tuples: list = get_connection_keys(
+        f_list,
+        ref_id,
+        target_id,
+        inverse,
+        exclude_str,
+    )
 
-    return tuple(klist), flist
+    return tuple(k_tuples), f_list
 
 
 def build_ct_dict(d: dict, p: dict) -> dict:
     """build a connection dictionary from a dict containing connection
     keys, and a dict containing connection properties. This is most
     useful for connections which a characterized by a fixed rate but
     apply to many species. E.g., mixing fluxes in a complex model etc.
 
     """
 
-    ct: dict = {}
-
-    for k, v in d.items():
-        td: dict = {}  # temp dict for scale
-        td["sc"] = v
-        td.update(p)
-        ct[k] = td
-
-    return ct
+    return {k: {"sc": v} | p for k, v in d.items()}
 
 
 def get_string_between_brackets(s: str) -> str:
     """Parse string and extract substring between square brackets"""
 
     s = s.split("[")
     if len(s) < 2:
@@ -974,18 +942,16 @@
 
     """
 
     from esbmtk import Q_
 
     if isinstance(kw, str):
         kw = Q_(kw)
-    elif isinstance(kw, Q_):
-        pass
-    else:
-        raise ValueError(f"kw must be string or Quantity")
+    elif not isinstance(kw, Q_):
+        raise ValueError("kw must be string or Quantity")
 
     return kw
 
 
 def map_units(v: any, *args) -> float:
     """parse v to see if it is a string. if yes, map to quantity.
     parse v to see if it is a quantity, if yes, map to model units
@@ -1039,15 +1005,14 @@
     The respective data fields are available as rgs.r.cs.xxx where xxx stands
     for a given key key in the  vr_datafields dictionary (i.e., H, CA, etc.)
 
     """
 
     from esbmtk import (
         ExternalCode,
-        calc_carbonates_1,
         carbonate_system_1_ode,
         Reservoir,
     )
 
     # get object handle even if it defined in model namespace
     # rgs = get_object_handle(rgs)
 
@@ -1065,99 +1030,97 @@
                     vr_datafields={
                         "H": rg.swc.hplus,
                         "CA": rg.swc.ca,  # 1
                         "HCO3": rg.swc.hco3,  # 2
                         "CO3": rg.swc.co3,  # 3
                         "CO2aq": rg.swc.co2,  # 4
                     },
-                    function_input_data=List(),
-                    function_params=List(),
+                    function_input_data=list(),
+                    function_params=list(),
                     register=rg,
                     return_values={"Hplus": rg.swc.hplus},
                 )
                 for n, v in ec.return_values.items():
                     rt = Reservoir(
                         name=n,
                         species=getattr(model, n),
                         concentration=f"{v} mol/kg",
                         register=rg,
                         volume=rg.volume,
                         rtype="computed",
                     )
                     rg.lor.append(rt)
-        else:
-            if hasattr(rg, "DIC") and hasattr(rg, "TA"):
-                ec = ExternalCode(
-                    name="cs",
-                    species=species,
-                    function=calc_carbonates_1,
-                    ftype="cs1",
-                    vr_datafields={
-                        "H": rg.swc.hplus,  # 0
-                        "CA": rg.swc.ca,  # 1
-                        "HCO3": rg.swc.hco3,  # 2
-                        "CO3": rg.swc.co3,  # 3
-                        "CO2aq": rg.swc.co2,  # 4
-                    },
-                    function_input_data=List([rg.DIC.c, rg.TA.c]),
-                    function_params=List(
-                        [
-                            rg.swc.K1,  # 0
-                            rg.swc.K2,  # 1
-                            rg.swc.KW,  # 2
-                            rg.swc.KB,  # 3
-                            rg.swc.boron,  # 4
-                            rg.swc.ca2,  # 5
-                            rg.swc.Ksp,  # 6
-                            rg.swc.hplus,  #
-                        ]
-                    ),
-                    # return_values="H CA HCO3 CO3 CO2aq".split(" "),
-                    register=rg,
-                )
-                rg.has_cs1 = True
+        elif hasattr(rg, "DIC") and hasattr(rg, "TA"):
+            ec = ExternalCode(
+                name="cs",
+                species=species,
+                function=calc_carbonates_1,
+                ftype="cs1",
+                vr_datafields={
+                    "H": rg.swc.hplus,  # 0
+                    "CA": rg.swc.ca,  # 1
+                    "HCO3": rg.swc.hco3,  # 2
+                    "CO3": rg.swc.co3,  # 3
+                    "CO2aq": rg.swc.co2,  # 4
+                },
+                function_input_data=list([rg.DIC.c, rg.TA.c]),
+                function_params=list(
+                    [
+                        rg.swc.K1,  # 0
+                        rg.swc.K2,  # 1
+                        rg.swc.KW,  # 2
+                        rg.swc.KB,  # 3
+                        rg.swc.boron,  # 4
+                        rg.swc.ca2,  # 5
+                        rg.swc.Ksp,  # 6
+                        rg.swc.hplus,  #
+                    ]
+                ),
+                # return_values="H CA HCO3 CO3 CO2aq".split(" "),
+                register=rg,
+            )
+            rg.has_cs1 = True
 
-            else:
-                raise AttributeError(f"{rg.full_name} must have a TA and DIC reservoir")
+        else:
+            raise AttributeError(f"{rg.full_name} must have a TA and DIC reservoir")
 
 
 def add_carbonate_system_2(**kwargs) -> None:
     """Creates a new carbonate system virtual reservoir
-        which will compute carbon species, saturation, compensation,
-        and snowline depth, and compute the associated carbonate burial fluxes
+    which will compute carbon species, saturation, compensation,
+    and snowline depth, and compute the associated carbonate burial fluxes
 
-        Required keywords:
-            r_sb: list of ReservoirGroup objects in the surface layer
-            r_db: list of ReservoirGroup objects in the deep layer
-            carbonate_export_fluxes: list of flux objects which mus match the
-                                     list of ReservoirGroup objects.
-            zsat_min = depth of the upper boundary of the deep box
-            z0 = upper depth limit for carbonate burial calculations
-                 typically zsat_min
-
-        Optional Parameters:
-
-            zsat = initial saturation depth (m)
-            zcc = initial carbon compensation depth (m)
-            zsnow = initial snowline depth (m)
-            zsat0 = characteristic depth (m)
-            Ksp0 = solubility product of calcite at air-water interface (mol^2/kg^2)
-            kc = heterogeneous rate constant/mass transfer coefficient for calcite dissolution (kg m^-2 yr^-1)
-            Ca2 = calcium ion concentration (mol/kg)
-            pc = characteristic pressure (atm)
-            pg = seawater density multiplied by gravity due to acceleration (atm/m)
-            I = dissolvable CaCO3 inventory
-            co3 = CO3 concentration (mol/kg)
-    q        Ksp = solubility product of calcite at in situ sea water conditions (mol^2/kg^2)
+    Required keywords:
+        r_sb: list of ReservoirGroup objects in the surface layer
+        r_db: list of ReservoirGroup objects in the deep layer
+        carbonate_export_fluxes: list of flux objects which must match the
+                                 list of ReservoirGroup objects.
+        zsat_min = depth of the upper boundary of the deep box
+        z0 = upper depth limit for carbonate burial calculations
+             typically zsat_min
+
+    Optional Parameters:
+
+        zsat = initial saturation depth (m)
+        zcc = initial carbon compensation depth (m)
+        zsnow = initial snowline depth (m)
+        zsat0 = characteristic depth (m)
+        Ksp0 = solubility product of calcite at air-water interface (mol^2/kg^2)
+        kc = heterogeneous rate constant/mass transfer coefficient for calcite dissolution (kg m^-2 yr^-1)
+        Ca2 = calcium ion concentration (mol/kg)
+        pc = characteristic pressure (atm)
+        pg = seawater density multiplied by gravity due to acceleration (atm/m)
+        I = dissolvable CaCO3 inventory
+        co3 = CO3 concentration (mol/kg)
+        Ksp = solubility product of calcite at in situ sea water conditions (mol^2/kg^2)
 
     """
 
     from esbmtk import (
         ExternalCode,
-        calc_carbonates_2,
         carbonate_system_2_ode,
         Reservoir,
     )
 
     # list of known keywords
     lkk: dict = {
         "r_db": list,  # list of deep reservoirs
@@ -1175,14 +1138,15 @@
         "pc": (float, int),
         "pg": (float, int),
         "I_caco3": (float, int),
         "alpha": float,
         "zmax": (float, int),
         "z0": (float, int),
         "Ksp": (float, int),
+        # "BM": (float, int),
     }
     # provide a list of absolutely required keywords
     lrk: list[str] = ["r_db", "r_sb", "carbonate_export_fluxes", "zsat_min", "z0"]
 
     # we need the reference to the Model in order to set some
     # default values.
 
@@ -1200,14 +1164,15 @@
         "AD": model.hyp.area_dz(-200, -6000),
         "alpha": 0.6,  # 0.928771302395292, #0.75,
         "pg": 0.103,  # pressure in atm/m
         "pc": 511,  # characteristic pressure after Boudreau 2010
         "I_caco3": 529,  # dissolveable CaCO3 in mol/m^2
         "zmax": -6000,  # max model depth
         "Ksp": reservoir.swc.Ksp,  # mol^2/kg^2
+        # "BM": 0.0,
     }
 
     # make sure all mandatory keywords are present
     __checkkeys__(lrk, lkk, kwargs)
 
     # add default values for keys which were not specified
     kwargs = __addmissingdefaults__(lod, kwargs)
@@ -1226,16 +1191,15 @@
     pc = kwargs["pc"]
     z0 = kwargs["z0"]
     Ksp = kwargs["Ksp"]
 
     # test if corresponding surface reservoirs have been defined
     if len(r_sb) == 0:
         raise ValueError(
-            f"Please update your call to add_carbonate_system_2"
-            f"and add the list of of corresponding surface reservoirs"
+            "Please update your call to add_carbonate_system_2and add the list of of corresponding surface reservoirs"
         )
 
     # C saturation(z) after Boudreau 2010
     Csat_table: np.ndarray = (Ksp0 / ca2) * np.exp((depths * pg) / pc)
     area_table = model.hyp.get_lookup_table(0, -6002)  # area in m^2(z)
     area_dz_table = model.hyp.get_lookup_table_area_dz(0, -6002) * -1  # area'
     AD = model.hyp.area_dz(z0, -6000)  # Total Ocean Area
@@ -1261,23 +1225,25 @@
                     "H": rg.swc.hplus,  # 0 H+
                     "CA": rg.swc.ca,  # 1 carbonate alkalinity
                     "HCO3": rg.swc.hco3,  # 2 HCO3
                     "CO3": rg.swc.co3,  # 3 CO3
                     "CO2aq": rg.swc.co2,  # 4 CO2aq
                     "zsat": abs(kwargs["zsat"]),  # 5 zsat
                     "zcc": abs(kwargs["zcc"]),  # 6 zcc
-                    # "zsnow": abs(kwargs["zsnow"]),  # 7 zsnow
+                    "zsnow": abs(kwargs["zsnow"]),  # 7 zsnow
                     "depth_area_table": area_table,
                     "area_dz_table": area_dz_table,
                     "Csat_table": Csat_table,
                     "Fburial": 0.0,
+                    "Fburial_l": 0.0,
+                    # "BM": 0.0,
                 },
                 ref_flux=kwargs["carbonate_export_fluxes"],
-                function_input_data=List(),
-                function_params=List(
+                function_input_data=list(),
+                function_params=list(
                     [
                         rg.swc.K1,  # 0
                         rg.swc.K2,  # 1
                         rg.swc.KW,  # 2
                         rg.swc.KB,  # 3
                         rg.swc.boron,  # 4
                         Ksp0,  # 5
@@ -1293,15 +1259,15 @@
                         float(abs(kwargs["zmax"])),  # 15
                         float(abs(kwargs["z0"])),  # 16
                         Ksp,  # 17
                         rg.swc.hplus,  # 18
                         float(abs(kwargs["zsnow"])),  # 19
                     ]
                 ),
-                return_values={
+                return_values={  # these must be known speces definitions
                     "Hplus": rg.swc.hplus,
                     "zsnow": float(abs(kwargs["zsnow"])),
                 },
                 register=rg,
             )
             for n, v in ec.return_values.items():
                 rt = Reservoir(
@@ -1329,33 +1295,33 @@
                     "HCO3": rg.swc.hco3,  # 2 HCO3
                     "CO3": rg.swc.co3,  # 3 CO3
                     "CO2aq": rg.swc.co2,  # 4 CO2aq
                     "zsat": kwargs["zsat"],  # 5 zsat
                     "zcc": kwargs["zcc"],  # 6 zcc
                     "zsnow": kwargs["zsnow"],  # 7 zsnow
                     "Fburial": 0.0,  # 8 carbonate burial
-                    "Fburial12": 0.0,  # 9 carbonate burial 12C
+                    "Fburial_l": 0.0,  # 9 carbonate burial 12C
                     "diss": 0.0,  # dissolution flux
                     "Bm": 0.0,
                 },
-                function_input_data=List(
+                function_input_data=list(
                     [
                         rg.DIC.m,  # 0 DIC mass db
                         rg.DIC.l,  # 1 DIC light isotope mass db
                         rg.DIC.c,  # 2 DIC concentration db
                         rg.TA.m,  # 3 TA mass db
                         rg.TA.c,  # 4 TA concentration db
                         kwargs["carbonate_export_fluxes"][i].fa,  # 5
                         area_table,  # 6
                         area_dz_table,  # 7
                         Csat_table,  # 8
                         rg.DIC.v,  # 9 reservoir volume
                     ]
                 ),
-                function_params=List(
+                function_params=list(
                     [
                         rg.swc.K1,  # 0
                         rg.swc.K2,  # 1
                         rg.swc.KW,  # 2
                         rg.swc.KB,  # 3
                         rg.swc.boron,  # 4
                         Ksp0,  # 5
@@ -1421,21 +1387,19 @@
 
     k: any
     v: any
 
     # loop over provided keywords
     for k, v in pv.items():
         # check av if provided value v is of correct type
-        if av[k] != any:
-            # print(f"key = {k}, value  = {v}")
-            if not isinstance(v, av[k]):
-                # print(f"k={k}, v= {v}, av[k] = {av[k]}")
-                raise TypeError(
-                    f"{type(v)} is the wrong type for '{k}', should be '{av[k]}'"
-                )
+        if av[k] != any and not isinstance(v, av[k]):
+            # print(f"k={k}, v= {v}, av[k] = {av[k]}")
+            raise TypeError(
+                f"{type(v)} is the wrong type for '{k}', should be '{av[k]}'"
+            )
 
 
 def __checkkeys__(lrk: list, lkk: list, kwargs: dict) -> None:
     """check if the mandatory keys are present
 
     lrk = list of required keywords
     lkk = list of all known keywords
@@ -1446,46 +1410,41 @@
     k: str
     v: any
     # test if the required keywords are given
     for k in lrk:  # loop over required keywords
         if isinstance(k, list):  # If keyword is a list
             s: int = 0  # loop over allowed substitutions
             for e in k:  # test how many matches are in this list
-                if e in kwargs:
-                    # print(self.kwargs[e])
-                    if not isinstance(e, (np.ndarray, np.float64, list)):
-                        # print (type(self.kwargs[e]))
-                        if kwargs[e] != "None":
-                            s = s + 1
+                if (
+                    e in kwargs
+                    and not isinstance(e, (np.ndarray, np.float64, list))
+                    and kwargs[e] != "None"
+                ):
+                    s = s + 1
             if s > 1:  # if more than one match
                 raise ValueError(f"You need to specify exactly one from this list: {k}")
 
-        else:  # keyword is not in list
-            if k not in kwargs:
-                raise ValueError(f"You need to specify a value for {k}")
-
-    tl: List[str] = []
-    # create a list of known keywords
-    for k, v in lkk.items():
-        tl.append(k)
+        elif k not in kwargs:
+            raise ValueError(f"You need to specify a value for {k}")
 
+    tl: list[str] = [k for k, v in lkk.items()]
     # test if we know all keys
-    for k, v in kwargs.items():
+    for k in kwargs:
         if k not in lkk:
             raise ValueError(f"{k} is not a valid keyword. \n Try any of \n {tl}\n")
 
 
 def __addmissingdefaults__(lod: dict, kwargs: dict) -> dict:
     """
     test if the keys in lod exist in kwargs, otherwise add them with the default values
     from lod
 
     """
 
     new: dict = {}
-    if len(lod) > 0:
+    if lod:
         for k, v in lod.items():
             if k not in kwargs:
-                new.update({k: v})
+                new[k] = v
 
-    kwargs.update(new)
+    kwargs |= new
     return kwargs
```

### Comparing `esbmtk-0.8.0.0/esbmtk.egg-info/SOURCES.txt` & `esbmtk-0.9.0.1/esbmtk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 Documentation/C_Cycle_Ocean.csv
 Documentation/test-data.csv
-esbmtk/Constructor.py
-esbmtk/Equation_Terms.py
 esbmtk/Hypsometric_Curve_05m.csv
-esbmtk/ODEINT_Solver.py
 esbmtk/__init__.py
 esbmtk/carbonate_chemistry.py
 esbmtk/carbonate_chemistry_2.py
 esbmtk/connections.py
+esbmtk/depreceated_code.py
 esbmtk/esbmtk.py
 esbmtk/esbmtk_base.py
 esbmtk/extended_classes.py
-esbmtk/odeuli2.py
-esbmtk/processes-old.py
+esbmtk/ode_backend.py
+esbmtk/ode_backend_2.py
+esbmtk/post_processing.py
 esbmtk/processes.py
 esbmtk/sealevel.py
 esbmtk/solver.py
 esbmtk/species_definitions.py
 esbmtk/utility_functions.py
 esbmtk.egg-info/PKG-INFO
 esbmtk.egg-info/SOURCES.txt
 esbmtk.egg-info/dependency_links.txt
 esbmtk.egg-info/top_level.txt
 examples/one-box-ocean/C_Cycle_Ocean.csv
 examples/one-box-ocean/emissions-full.csv
 examples/one-box-ocean/emissions.csv
 examples/one-box-ocean/measured_c_isotopes.csv
-tests/measured_c_isotopes.csv
+tests/measured_c_isotopes.csv
+tests/test_esbmtk.py
```

### Comparing `esbmtk-0.8.0.0/examples/one-box-ocean/C_Cycle_Ocean.csv` & `esbmtk-0.9.0.1/examples/one-box-ocean/C_Cycle_Ocean.csv`

 * *Files identical despite different names*

### Comparing `esbmtk-0.8.0.0/examples/one-box-ocean/emissions-full.csv` & `esbmtk-0.9.0.1/examples/one-box-ocean/emissions-full.csv`

 * *Files identical despite different names*

### Comparing `esbmtk-0.8.0.0/examples/one-box-ocean/emissions.csv` & `esbmtk-0.9.0.1/examples/one-box-ocean/emissions.csv`

 * *Files identical despite different names*

### Comparing `esbmtk-0.8.0.0/setup.cfg` & `esbmtk-0.9.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = esbmtk
-version = 0.8.0.0
+version = 0.9.0.1
 author = Ulrich G. Wortmann
 license = GPL-3.0-or-later
 author_email = uli.wortmann@utoronto.ca
 description = An Earth Sciences Box Modeling Toolkit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/uliw/esbmtk
```

