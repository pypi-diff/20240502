# Comparing `tmp/iapws-1.5.3.tar.gz` & `tmp/iapws-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iapws-1.5.3.tar", last modified: Wed Sep 28 16:08:00 2022, max compression
+gzip compressed data, was "iapws-1.5.4.tar", last modified: Thu May  2 20:23:46 2024, max compression
```

## Comparing `iapws-1.5.3.tar` & `iapws-1.5.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)        0 2022-09-28 16:08:00.823321 iapws-1.5.3/
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    35120 2017-06-13 13:35:34.000000 iapws-1.5.3/LICENSE
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)       57 2022-09-28 15:01:18.000000 iapws-1.5.3/MANIFEST.in
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     6790 2022-09-28 16:08:00.823321 iapws-1.5.3/PKG-INFO
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     4659 2022-09-28 15:01:18.000000 iapws-1.5.3/README.rst
-drwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)        0 2022-09-28 16:08:00.823321 iapws-1.5.3/iapws/
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)        6 2022-09-28 15:02:20.000000 iapws-1.5.3/iapws/VERSION
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     9195 2022-09-28 15:01:18.000000 iapws-1.5.3/iapws/__init__.py
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    51049 2022-09-28 15:01:18.000000 iapws-1.5.3/iapws/_iapws.py
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     9890 2022-09-28 15:01:18.000000 iapws-1.5.3/iapws/_utils.py
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    20925 2022-09-28 15:40:23.000000 iapws-1.5.3/iapws/ammonia.py
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    32961 2022-09-28 15:40:26.000000 iapws-1.5.3/iapws/humidAir.py
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    23930 2022-09-28 15:01:18.000000 iapws-1.5.3/iapws/iapws08.py
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)   101514 2022-09-28 15:40:23.000000 iapws-1.5.3/iapws/iapws95.py
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)   166331 2022-09-28 15:40:23.000000 iapws-1.5.3/iapws/iapws97.py
-drwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)        0 2022-09-28 16:08:00.823321 iapws-1.5.3/iapws.egg-info/
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     6790 2022-09-28 16:08:00.000000 iapws-1.5.3/iapws.egg-info/PKG-INFO
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)      333 2022-09-28 16:08:00.000000 iapws-1.5.3/iapws.egg-info/SOURCES.txt
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)        1 2022-09-28 16:08:00.000000 iapws-1.5.3/iapws.egg-info/dependency_links.txt
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)       11 2022-09-28 16:08:00.000000 iapws-1.5.3/iapws.egg-info/requires.txt
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)        6 2022-09-28 16:08:00.000000 iapws-1.5.3/iapws.egg-info/top_level.txt
--rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)       38 2022-09-28 16:08:00.823321 iapws-1.5.3/setup.cfg
--rwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)     1577 2022-09-28 15:01:18.000000 iapws-1.5.3/setup.py
+drwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)        0 2024-05-02 20:23:46.484059 iapws-1.5.4/
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    35120 2017-06-13 13:35:34.000000 iapws-1.5.4/LICENSE
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)       57 2020-06-19 19:19:26.000000 iapws-1.5.4/MANIFEST.in
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     5803 2024-05-02 20:23:46.484059 iapws-1.5.4/PKG-INFO
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     4801 2023-09-03 19:47:56.000000 iapws-1.5.4/README.rst
+drwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)        0 2024-05-02 20:23:46.480059 iapws-1.5.4/iapws/
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)        6 2024-05-02 20:06:04.000000 iapws-1.5.4/iapws/VERSION
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     9195 2021-03-26 17:10:24.000000 iapws-1.5.4/iapws/__init__.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    51781 2024-05-01 20:21:54.000000 iapws-1.5.4/iapws/_iapws.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    44566 2023-09-03 19:47:56.000000 iapws-1.5.4/iapws/_iapws97Constants.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     9996 2023-09-03 19:47:56.000000 iapws-1.5.4/iapws/_utils.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    21034 2023-09-03 19:47:56.000000 iapws-1.5.4/iapws/ammonia.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    33565 2023-09-03 19:47:56.000000 iapws-1.5.4/iapws/humidAir.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)    24518 2023-09-03 19:47:56.000000 iapws-1.5.4/iapws/iapws08.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)   102678 2024-04-20 10:19:16.000000 iapws-1.5.4/iapws/iapws95.py
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)   136918 2024-05-02 18:20:08.000000 iapws-1.5.4/iapws/iapws97.py
+drwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)        0 2024-05-02 20:23:46.480059 iapws-1.5.4/iapws.egg-info/
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)     5803 2024-05-02 20:23:46.000000 iapws-1.5.4/iapws.egg-info/PKG-INFO
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)      360 2024-05-02 20:23:46.000000 iapws-1.5.4/iapws.egg-info/SOURCES.txt
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)        1 2024-05-02 20:23:46.000000 iapws-1.5.4/iapws.egg-info/dependency_links.txt
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)       11 2024-05-02 20:23:46.000000 iapws-1.5.4/iapws.egg-info/requires.txt
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)        6 2024-05-02 20:23:46.000000 iapws-1.5.4/iapws.egg-info/top_level.txt
+-rw-r--r--   0 jjgomera  (1000) jjgomera  (1000)       38 2024-05-02 20:23:46.484059 iapws-1.5.4/setup.cfg
+-rwxr-xr-x   0 jjgomera  (1000) jjgomera  (1000)     1577 2023-09-03 19:47:56.000000 iapws-1.5.4/setup.py
```

### Comparing `iapws-1.5.3/LICENSE` & `iapws-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iapws-1.5.3/README.rst` & `iapws-1.5.4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-.. image:: https://api.travis-ci.org/jjgomera/iapws.svg?branch=master
-    :target: https://travis-ci.org/jjgomera/iapws
+.. image:: https://dl.circleci.com/status-badge/img/gh/jjgomera/iapws/tree/master.svg?style=svg
+    :target: https://dl.circleci.com/status-badge/redirect/gh/jjgomera/iapws/tree/master
     :alt: Build Status
 
 .. image:: https://ci.appveyor.com/api/projects/status/a128sh8e50cjsiya?svg=true
     :target: https://ci.appveyor.com/project/jjgomera/iapws
     :alt: Windows Build Status
 
 .. image:: https://coveralls.io/repos/github/jjgomera/iapws/badge.svg?branch=master
     :target: https://coveralls.io/github/jjgomera/iapws?branch=master
     :alt: coveralls.io analysis
 
 .. image:: https://codecov.io/gh/jjgomera/iapws/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jjgomera/iapws
     :alt: codecov.io analysis
 
-.. image:: https://landscape.io/github/jjgomera/iapws/master/landscape.svg?style=flat
-   :target: https://landscape.io/github/jjgomera/iapws/master
-   :alt: Code Health
+.. image:: https://app.codacy.com/project/badge/Grade/bb92d537dfa1461d919a0782f3c398b9
+    :target: https://www.codacy.com/gh/jjgomera/iapws/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jjgomera/iapws&amp;utm_campaign=Badge_Grade
+    :alt: Code Quality
 
 .. image:: http://readthedocs.org/projects/iapws/badge/?version=latest
     :target: http://iapws.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4744318.svg
    :target: https://doi.org/10.5281/zenodo.4744318
@@ -123,15 +123,14 @@
     state = SeaWater(T=300, P=0.101325, S=0.001)    #Seawater with 0.1% Salinity
     print(state.cp)                                 # Get cp
 
 
 TODO
 ====
 
-* FIXME: Electrolytic conductiviy
 * TODO: Improve convergence in two phase region for IAPWS95 and D2O class
 * TODO: Implement SBTL method for fast calculation
 * TODO: Implement TTSE method for fast calculation
 
 Ammonia-water mixture:
 
 * TODO: Add equilibrium routine
```

### Comparing `iapws-1.5.3/iapws/__init__.py` & `iapws-1.5.4/iapws/__init__.py`

 * *Files identical despite different names*

### Comparing `iapws-1.5.3/iapws/_iapws.py` & `iapws-1.5.4/iapws/_iapws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
+# pylint: disable=invalid-name
+# pylint: disable=too-many-lines, too-many-locals, too-many-statements
+# pylint: disable=too-many-branches, too-many-boolean-expressions
+
 """
 Miscelaneous IAPWS standards. This module include:
 
     * :func:`_Ice`: Ice Ih state equation
     * :func:`_Liquid`: Properties of liquid water at 0.1 MPa
     * :func:`_Supercooled`: Thermodynamic properties of supercooled water
     * :func:`_Sublimation_Pressure`: Sublimation pressure correlation
@@ -126,15 +130,15 @@
         # Ice Ih limit upper pressure
         raise NotImplementedError("Incoming out of bound")
     elif P < Pt:
         Psub = _Sublimation_Pressure(T)
         if Psub > P:
             # Zone Gas
             warnings.warn("Metastable ice in vapor region")
-    elif 251.165 < T:
+    elif T > 251.165:
         Pmel = _Melting_Pressure(T)
         if Pmel < P:
             # Zone Liquid
             warnings.warn("Metastable ice in liquid region")
 
     Tr = T/Tt
     Pr = P/Pt
@@ -237,15 +241,15 @@
             * vt: [∂v/∂T]P, [m³/kgK]
             * vtt: [∂²v/∂T²]P, [m³/kgK²]
             * vp: [∂v/∂P]T, [m³/kg/MPa]
             * vtp: [∂²v/∂T∂P], [m³/kg/MPa]
             * alfav: Cubic expansion coefficient, [1/K]
             * xkappa : Isothermal compressibility, [1/MPa]
             * ks: Isentropic compressibility, [1/MPa]
-            * mu: Viscosity, [mPas]
+            * mu: Viscosity, [Pas]
             * k: Thermal conductivity, [W/mK]
             * epsilon: Dielectric constant, [-]
 
     Notes
     -----
     Raise :class:`NotImplementedError` if input isn't in limit:
 
@@ -262,19 +266,19 @@
     ----------
     IAPWS, Revised Supplementary Release on Properties of Liquid Water at 0.1
     MPa, http://www.iapws.org/relguide/LiquidWater.html
     """
     # Check input in range of validity
     if T <= 253.15 or T >= 383.15 or P < 0.1 or P > 0.3:
         raise NotImplementedError("Incoming out of bound")
-    elif P != 0.1:
+    if P != 0.1:
         # Raise a warning if the P value is extrapolated
         warnings.warn("Using extrapolated values")
 
-    R = 0.46151805   # kJ/kgK
+    Rg = 0.46151805   # kJ/kgK
     Po = 0.1
     Tr = 10
     tau = T/Tr
     alfa = Tr/(593-T)
     beta = Tr/(T-232)
 
     a = [None, -1.661470539e5, 2.708781640e6, -1.557191544e8, None,
@@ -288,53 +292,53 @@
          -4.8510101e-5]
     c = [None, -2.452093414e2, 3.869269598e1, -8.983025854]
     n = [None, 4, 5, 7, None, None, 4, 5, 7, 8, 9, 1, 3, 5, 6, 7]
     m = [None, 2, 3, 4, 5, 1, 2, 3, 4, 5, 6, 1, 3, 4, 5, 6, 7, 9]
 
     suma1 = sum(a[i]*alfa**n[i] for i in range(1, 4))
     suma2 = sum(b[i]*beta**m[i] for i in range(1, 5))
-    go = R*Tr*(c[1]+c[2]*tau+c[3]*tau*log(tau)+suma1+suma2)
+    go = Rg*Tr*(c[1]+c[2]*tau+c[3]*tau*log(tau)+suma1+suma2)
 
     suma1 = sum(a[i]*alfa**n[i] for i in range(6, 11))
     suma2 = sum(b[i]*beta**m[i] for i in range(5, 11))
-    vo = R*Tr/Po/1000*(a[5]+suma1+suma2)
+    vo = Rg*Tr/Po/1000*(a[5]+suma1+suma2)
 
     suma1 = sum(a[i]*alfa**n[i] for i in range(11, 16))
     suma2 = sum(b[i]*beta**m[i] for i in range(11, 18))
-    vpo = R*Tr/Po**2/1000*(suma1+suma2)
+    vpo = Rg*Tr/Po**2/1000*(suma1+suma2)
 
     suma1 = sum(n[i]*a[i]*alfa**(n[i]+1) for i in range(1, 4))
     suma2 = sum(m[i]*b[i]*beta**(m[i]+1) for i in range(1, 5))
-    so = -R*(c[2]+c[3]*(1+log(tau))+suma1-suma2)
+    so = -Rg*(c[2]+c[3]*(1+log(tau))+suma1-suma2)
 
     suma1 = sum(n[i]*(n[i]+1)*a[i]*alfa**(n[i]+2) for i in range(1, 4))
     suma2 = sum(m[i]*(m[i]+1)*b[i]*beta**(m[i]+2) for i in range(1, 5))
-    cpo = -R*(c[3]+tau*suma1+tau*suma2)
+    cpo = -Rg*(c[3]+tau*suma1+tau*suma2)
 
     suma1 = sum(n[i]*a[i]*alfa**(n[i]+1) for i in range(6, 11))
     suma2 = sum(m[i]*b[i]*beta**(m[i]+1) for i in range(5, 11))
-    vto = R/Po/1000*(suma1-suma2)
+    vto = Rg/Po/1000*(suma1-suma2)
 
     # This properties are only neccessary for computing thermodynamic
     # properties at pressures different from 0.1 MPa
     suma1 = sum(n[i]*(n[i]+1)*a[i]*alfa**(n[i]+2) for i in range(6, 11))
     suma2 = sum(m[i]*(m[i]+1)*b[i]*beta**(m[i]+2) for i in range(5, 11))
-    vtto = R/Tr/Po/1000*(suma1+suma2)
+    vtto = Rg/Tr/Po/1000*(suma1+suma2)
 
     suma1 = sum(n[i]*a[i]*alfa**(n[i]+1) for i in range(11, 16))
     suma2 = sum(m[i]*b[i]*beta**(m[i]+1) for i in range(11, 18))
-    vpto = R/Po**2/1000*(suma1-suma2)
+    vpto = Rg/Po**2/1000*(suma1-suma2)
 
     if P != 0.1:
         go += vo*(P-0.1)
         so -= vto*(P-0.1)
         cpo -= T*vtto*(P-0.1)
         vo -= vpo*(P-0.1)
         vto += vpto*(P-0.1)
-        vppo = 3.24e-10*R*Tr/0.1**3
+        vppo = 3.24e-10*Rg*Tr/0.1**3
         vpo += vppo*(P-0.1)
 
     h = go+T*so
     u = h-P*vo
     a = go-P*vo
     cv = cpo+T*vto**2/vpo
     xkappa = -vpo/vo
@@ -448,25 +452,25 @@
         Th = 172.82+0.03718*P+3.403e-5*P**2-1.573e-8*P**3
         if T < Th or T > 300 or P > 1000:
             raise NotImplementedError("Incoming out of bound")
 
     # Parameters, Table 1
     Tll = 228.2
     rho0 = 1081.6482
-    R = 0.461523087
-    pi0 = 300e3/rho0/R/Tll
+    Rg = 0.461523087
+    pi0 = 300e3/rho0/Rg/Tll
     omega0 = 0.5212269
     L0 = 0.76317954
     k0 = 0.072158686
     k1 = -0.31569232
     k2 = 5.2992608
 
     # Reducing parameters, Eq 2
     tau = T/Tll-1
-    p = P*1000/rho0/R/Tll
+    p = P*1000/rho0/Rg/Tll
     tau_ = tau+1
     p_ = p+pi0
 
     # Eq 3
     ci = [-8.1570681381655, 1.2875032, 7.0901673598012, -3.2779161e-2,
           7.3703949e-1, -2.1628622e-1, -5.1782479, 4.2293517e-4, 2.3592109e-2,
           4.3773754, -2.9967770e-3, -9.6558018e-1, 3.7595286, 1.2632441,
@@ -552,29 +556,29 @@
     # Eq 13
     prop["rho"] = rho0/((tau+1)/2*(omega0/2*(1-fi**2)+Lp*(fi+1))+phirp)
 
     # Eq 1
     prop["g"] = phir+(tau+1)*(x*L+x*log(x)+(1-x)*log(1-x)+omega*x*(1-x))
 
     # Eq 14
-    prop["s"] = -R*((tau+1)/2*Lt*(fi+1)
+    prop["s"] = -Rg*((tau+1)/2*Lt*(fi+1)
                     + (x*L+x*log(x)+(1-x)*log(1-x)+omega*x*(1-x))+phirt)
 
     # Basic derived state properties
     prop["h"] = prop["g"]+T*prop["s"]
     prop["u"] = prop["h"]+P/prop["rho"]
     prop["a"] = prop["u"]-T*prop["s"]
 
     # Eq 15
-    prop["xkappa"] = prop["rho"]/rho0**2/R*1000/Tll*(
+    prop["xkappa"] = prop["rho"]/rho0**2/Rg*1000/Tll*(
         (tau+1)/2*(Xi*(Lp-omega0*fi)**2-(fi+1)*Lpp)-phirpp)
     prop["alfap"] = prop["rho"]/rho0/Tll*(
         Ltp/2*(tau+1)*(fi+1) + (omega0*(1-fi**2)/2+Lp*(fi+1))/2
         - (tau+1)*Lt/2*Xi*(Lp-omega0*fi) + phirtp)
-    prop["cp"] = -R*(tau+1)*(Lt*(fi+1)+(tau+1)/2*(Ltt*(fi+1)-Lt**2*Xi)+phirtt)
+    prop["cp"] = -Rg*(tau+1)*(Lt*(fi+1)+(tau+1)/2*(Ltt*(fi+1)-Lt**2*Xi)+phirtt)
 
     # Eq 16
     prop["cv"] = prop["cp"]-T*prop["alfap"]**2/prop["rho"]/prop["xkappa"]*1e3
 
     # Eq 17
     prop["w"] = (prop["rho"]*prop["xkappa"]*1e-6*prop["cv"]/prop["cp"])**-0.5
     return prop
@@ -613,16 +617,16 @@
         Tita = T/Tt
         suma = 0
         a = [-0.212144006e2, 0.273203819e2, -0.61059813e1]
         expo = [0.333333333e-2, 1.20666667, 1.70333333]
         for ai, expi in zip(a, expo):
             suma += ai*Tita**expi
         return exp(suma/Tita)*Pt
-    else:
-        raise NotImplementedError("Incoming out of bound")
+
+    raise NotImplementedError("Incoming out of bound")
 
 
 def _Melting_Pressure(T, ice="Ih"):
     """Melting Pressure correlation
 
     Parameters
     ----------
@@ -742,15 +746,15 @@
     Hij = [0.520094, 0.850895e-1, -0.108374e1, -0.289555, 0.222531, 0.999115,
            0.188797e1, 0.126613e1, 0.120573, -0.281378, -0.906851, -0.772479,
            -0.489837, -0.257040, 0.161913, 0.257399, -0.325372e-1, 0.698452e-1,
            0.872102e-2, -0.435673e-2, -0.593264e-3]
     mu1 = exp(Dr*sum((1/Tr-1)**i*h*(Dr-1)**j for i, j, h in zip(li, lj, Hij)))
 
     # Critical enhancement
-    if fase and drho:
+    if rho and fase and drho:
         qc = 1/1.9
         qd = 1/1.1
 
         # Eq 21
         DeltaX = Pc*Dr**2*(fase.drhodP_T/rho-drho/rho*1.5/Tr)
         if DeltaX < 0:
             DeltaX = 0
@@ -835,16 +839,16 @@
            0.0832827019, -0.00719201245, 2.19650529, -4.54580785, 3.55777244,
            -1.40944978, 0.275418278, -0.0205938816, -1.21051378, 1.60812989,
            -0.621178141, 0.0716373224, -2.7203370, 4.57586331, -3.18369245,
            1.1168348, -0.19268305, 0.012913842]
     k1 = exp(d*sum((1/Tr-1)**i*n*(d-1)**j for i, j, n in zip(li, lj, nij)))
 
     # Critical enhancement
-    if fase:
-        R = 0.46151805
+    if rho and fase:
+        Rg = 0.46151805
 
         if not drho:
             # Industrial formulation
             # Eq 25
             if d <= 0.310559006:
                 ai = [6.53786807199516, -5.61149954923348, 3.39624167361325,
                       -2.27492629730878, 10.2631854662709, 1.97815050331519]
@@ -873,15 +877,15 @@
         if y < 1.2e-7:
             Z = 0
         else:
             Z = 2/pi/y*(((1-1/fase.cp_cv)*atan(y)+y/fase.cp_cv)-(
                 1-exp(-1/(1/y+y**2/3/d**2))))
 
         # Eq 18
-        k2 = 177.8514*d*fase.cp/R*Tr/fase.mu*1e-6*Z
+        k2 = 177.8514*d*fase.cp/Rg*Tr/fase.mu*1e-6*Z
 
     else:
         # No critical enhancement
         k2 = 0
 
     # Eq 10
     k = k0*k1+k2
@@ -922,16 +926,16 @@
     """
     if 248.15 <= T <= Tc:
         tau = 1-T/Tc
         sigma = 235.8 * tau**1.256 * (1-0.625*tau)
 
         # The equation give surface tension in mN/m², converted to N/m²
         return 1e-3*sigma
-    else:
-        raise NotImplementedError("Incoming out of bound")
+
+    raise NotImplementedError("Incoming out of bound")
 
 
 def _Dielectric(rho, T):
     """Equation for the Dielectric constant
 
     Parameters
     ----------
@@ -1131,31 +1135,45 @@
 
     References
     ----------
     IAPWS, Electrolytic Conductivity (Specific Conductance) of Liquid and Dense
     Supercritical Water from 0°C to 800°C and Pressures up to 1000 MPa,
     http://www.iapws.org/relguide/conduct.pdf
     """
-    # FIXME: Dont work
+    # density in g/l
     rho_ = rho/1000
-    kw = 10**-_Kw(rho, T)
+
+    # This guideline predates the current standard on the ionization constant,
+    # therefore the standard accepted at that time must be used in order to
+    # obtain the values of the tables for testing.
+    # Marshall, W.L., Franck, E.U.
+    # Ion product of water substance, 0-1000ºC, 1-10,000 bars New International
+    # Formulation and its background
+    # J. Phys. Chem. Ref. Data 10(2) (1981) 295-304
+    # doi: 10.1063/1.555643
+
+    # Eq 4
+    kw = 10**(-4.098 - 3245.2/T + 2.2362e5/T**2 - 3.984e7/T**3 +
+              (13.957 - 1262.3/T + 8.5641e5/T**2)*log10(rho_))
+
+    # kw = 10**-_Kw(rho, T)
 
     A = [1850., 1410., 2.16417e-6, 1.81609e-7, -1.75297e-9, 7.20708e-12]
     B = [16., 11.6, 3.26e-4, -2.3e-6, 1.1e-8]
     t = T-273.15
 
-    Loo = A[0]-1/(1/A[1]+sum(A[i+2]*t**(i+1) for i in range(4)))      # Eq 5
-    rho_h = B[0]-1/(1/B[1]+sum(B[i+2]*t**(i+1) for i in range(3)))    # Eq 6
+    Loo = A[0]-1/(1/A[1] + A[2]*t + A[3]*t**2 + A[4]*t**3 + A[5]*t**4)   # Eq 5
+    rho_h = B[0]-1/(1/B[1] + B[2]*t + B[3]*t**2 + B[4]*t**3)             # Eq 6
 
     # Eq 4
     L_o = (rho_h-rho_)*Loo/rho_h
 
     # Eq 1
-    k = 100*1e-3*L_o*kw**0.5*rho_
-    return k
+    k = 1e-3*L_o*kw**0.5*rho_
+    return k*1e2
 
 
 # Heavy water transport properties
 def _D2O_Viscosity(rho, T, fase=None, drho=None):
     """Equation for the Viscosity of heavy water
 
     Parameters
@@ -1205,15 +1223,15 @@
            -0.108354, -0.00481265, -1.545710, -0.0570938, -0.0753783, 0.553080,
            -0.0650201]
 
     arr = [(1/Tr-1)**i*(rhor-1)**j*hij for i, j, hij in zip(hi, hj, Hij)]
     mu1 = exp(rhor*sum(arr))
 
     # Critical enhancement
-    if fase and drho:
+    if rho and fase and drho:
         qc = 1/1.9
         qd = 1/0.4
 
         # Eq 21
         DeltaX = Pc_D2O*rhor**2*(fase.drhodP_T/rho-drho/rho*1.5/Tr)
         if DeltaX < 0:
             DeltaX = 0
@@ -1299,16 +1317,16 @@
            0.224691518, -0.322191265, 0.0596204654, 2.06156007, -3.48612456,
            1.47962309, 0.625101458, -0.56123225, 0.0974446139, -2.06105687,
            0.416240028, 2.92524513, -2.81703583, 1.00551476, -0.127884416]
 
     k1 = exp(d*sum((1/Tr-1)**i * n*(d-1)**j for i, j, n in zip(li, lj, nij)))
 
     # Critical enhancement
-    if fase and drho:
-        R = 0.415151994
+    if rho and fase and drho:
+        Rg = 0.415151994
         DeltaX = d*(Pc_D2O/rhoc_D2O*fase.drhodP_T-Pc_D2O/rhoc_D2O*drho*1.5/Tr)
         if DeltaX < 0:
             DeltaX = 0
 
         X = 0.13*(DeltaX/0.06)**(0.63/1.239)                            # Eq 22
         y = X/0.36                                                      # Eq 20
 
@@ -1316,15 +1334,15 @@
         if y < 1.2e-7:
             Z = 0
         else:
             Z = 2/pi/y*(((1-1/fase.cp_cv)*atan(y)+y/fase.cp_cv)-(
                 1-exp(-1/(1/y+y**2/3/d**2))))
 
         # Eq 18
-        k2 = 175.987*d*fase.cp/R*Tr/fase.mu*1e-6*Z
+        k2 = 175.987*d*fase.cp/Rg*Tr/fase.mu*1e-6*Z
 
     else:
         # No critical enhancement
         k2 = 0
 
     # Eq 15
     k = k0*k1+k2
@@ -1361,16 +1379,16 @@
     ----------
     IAPWS, Release on Surface Tension of Heavy Water Substance,
     http://www.iapws.org/relguide/surfd2o.pdf
     """
     Tr = T/643.847
     if 269.65 <= T < 643.847:
         return 1e-3*(238*(1-Tr)**1.25*(1-0.639*(1-Tr)))
-    else:
-        raise NotImplementedError("Incoming out of bound")
+
+    raise NotImplementedError("Incoming out of bound")
 
 
 def _D2O_Sublimation_Pressure(T):
     """Sublimation Pressure correlation for heavy water
 
     Parameters
     ----------
@@ -1402,16 +1420,16 @@
         Tita = T/276.969
         suma = 0
         ai = [-0.1314226e2, 0.3212969e2]
         ti = [-1.73, -1.42]
         for a, t in zip(ai, ti):
             suma += a*(1-Tita**t)
         return exp(suma)*0.00066159
-    else:
-        raise NotImplementedError("Incoming out of bound")
+
+    raise NotImplementedError("Incoming out of bound")
 
 
 def _D2O_Melting_Pressure(T, ice="Ih"):
     """Melting Pressure correlation for heavy water
 
     Parameters
     ----------
@@ -1532,42 +1550,42 @@
         "Ar(D2O)": (288.30, 583.76),
         "Kr(D2O)": (288.19, 523.06),
         "Xe(D2O)": (295.39, 574.85),
         "D2(D2O)": (288.17, 581.00),
         "CH4(D2O)": (288.16, 517.46)}
 
     # Check input parameters
-    if liquid != "D2O" and liquid != "H2O":
+    if liquid not in ("D2O", "H2O"):
         raise NotImplementedError("Solvent liquid unsupported")
     if gas not in limit:
         raise NotImplementedError("Gas unsupported")
 
     Tmin, Tmax = limit[gas]
     if T < Tmin or T > Tmax:
         warnings.warn("Temperature out of data of correlation")
 
     if liquid == "D2O":
-        Tc = 643.847
-        Pc = 21.671
+        Tc_ = Tc_D2O
+        Pc_ = 21.671
     else:
-        Tc = 647.096
-        Pc = 22.064
+        Tc_ = Tc
+        Pc_ = Pc
 
-    Tr = T/Tc
+    Tr = T/Tc_
     tau = 1-Tr
 
     # Eq 4
     if liquid == "H2O":
         ai = [-7.85951783, 1.84408259, -11.7866497, 22.6807411, -15.9618719,
               1.80122502]
         bi = [1, 1.5, 3, 3.5, 4, 7.5]
     else:
         ai = [-7.896657, 24.73308, -27.81128, 9.355913, -9.220083]
         bi = [1, 1.89, 2, 3, 3.6]
-    ps = Pc*exp(1/Tr*sum(a*tau**b for a, b in zip(ai, bi)))
+    ps = Pc_*exp(1/Tr*sum(a*tau**b for a, b in zip(ai, bi)))
 
     # Select values from Table 2
     par = {
         "He": (-3.52839, 7.12983, 4.47770),
         "Ne": (-3.18301, 5.31448, 5.43774),
         "Ar": (-8.40954, 4.29587, 10.52779),
         "Kr": (-8.97358, 3.61508, 11.29963),
@@ -1657,29 +1675,29 @@
         "Ar(D2O)": (288.30, 583.76),
         "Kr(D2O)": (288.19, 523.06),
         "Xe(D2O)": (295.39, 574.85),
         "D2(D2O)": (288.17, 581.00),
         "CH4(D2O)": (288.16, 517.46)}
 
     # Check input parameters
-    if liquid != "D2O" and liquid != "H2O":
+    if liquid not in ("D2O", "H2O"):
         raise NotImplementedError("Solvent liquid unsupported")
     if gas not in limit:
         raise NotImplementedError("Gas unsupported")
 
     Tmin, Tmax = limit[gas]
     if T < Tmin or T > Tmax:
         warnings.warn("Temperature out of data of correlation")
 
     if liquid == "D2O":
-        Tc = 643.847
+        Tc_ = Tc_D2O
     else:
-        Tc = 647.096
+        Tc_ = Tc
 
-    Tr = T/Tc
+    Tr = T/Tc_
     tau = 1-Tr
 
     # Eq 6
     if liquid == "H2O":
         ci = [1.99274064, 1.09965342, -0.510839303, -1.75493479, -45.5170352,
               -6.7469445e5]
         di = [1/3, 2/3, 5/3, 16/3, 43/3, 110/3]
```

### Comparing `iapws-1.5.3/iapws/_utils.py` & `iapws-1.5.4/iapws/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
+# pylint: disable=invalid-name, too-many-branches, too-many-statements
+# pylint: disable=too-many-arguments
+
 """
 Miscelaneous internal utilities. This module include:
 
     * :func:`getphase`: Get phase string of state
     * :class:`_fase`: Base class to define a phase state
     * :func:`deriv_H`: Calculate generic partial derivative with a fundamental
       Helmholtz free energy equation of state
@@ -307,15 +310,15 @@
     elif x == "T":
         dPdx = 0.0
         dTdx = 1.0
     elif x == "v":
         dPdx = -fase.v*fase.xkappa
         dTdx = fase.v*fase.alfav
     elif x == "u":
-        dPdx = fase.v*(state.P*1000.0*fase.xkappa-state.T*fase.alfav),
+        dPdx = fase.v*(state.P*1000.0*fase.xkappa-state.T*fase.alfav)
         dTdx = fase.cp-state.P*1000.0*fase.v*fase.alfav
     elif x == "h":
         dPdx = fase.v*(1.0-state.T*fase.alfav)
         dTdx = fase.cp
     elif x == "s":
         dPdx = -fase.v * fase.alfav
         dTdx = fase.cp/state.T
@@ -334,15 +337,15 @@
     elif y == "T":
         dPdy = 0.0
         dTdy = 1.0
     elif y == "v":
         dPdy = -fase.v*fase.xkappa
         dTdy = fase.v*fase.alfav
     elif y == "u":
-        dPdy = fase.v*(state.P*1000.0*fase.xkappa-state.T*fase.alfav),
+        dPdy = fase.v*(state.P*1000.0*fase.xkappa-state.T*fase.alfav)
         dTdy = fase.cp-state.P*1000.0*fase.v*fase.alfav
     elif y == "h":
         dPdy = fase.v*(1.0-state.T*fase.alfav)
         dTdy = fase.cp
     elif y == "s":
         dPdy = -fase.v * fase.alfav
         dTdy = fase.cp/state.T
@@ -361,15 +364,15 @@
     elif z == "T":
         dPdz = 0.0
         dTdz = 1.0
     elif z == "v":
         dPdz = -fase.v*fase.xkappa
         dTdz = fase.v*fase.alfav
     elif z == "u":
-        dPdz = fase.v*(state.P*1000.0*fase.xkappa-state.T*fase.alfav),
+        dPdz = fase.v*(state.P*1000.0*fase.xkappa-state.T*fase.alfav)
         dTdz = fase.cp-state.P*1000.0*fase.v*fase.alfav
     elif z == "h":
         dPdz = fase.v*(1.0-state.T*fase.alfav)
         dTdz = fase.cp
     elif z == "s":
         dPdz = -fase.v * fase.alfav
         dTdz = fase.cp/state.T
```

### Comparing `iapws-1.5.3/iapws/ammonia.py` & `iapws-1.5.4/iapws/ammonia.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
+# pylint: disable=invalid-name
+# pylint: disable=too-many-locals, too-many-statements
+
 """
 Module with Ammonia-water mixture properties and related properties. The module
 include:
 
     * :class:`NH3`: Multiparameter equation of state for ammonia
     * :class:`H2ONH3`:  Thermodynamic properties of ammonia-water mixtures
     * :class:`Ttr`: Triple point of ammonia-water mixtures
@@ -241,15 +244,15 @@
 
         References
         ----------
         IAPWS, Guideline on the IAPWS Formulation 2001 for the Thermodynamic
         Properties of Ammonia-Water Mixtures,
         http://www.iapws.org/relguide/nh3h2o.pdf, Table 4
         """
-        # FIXME: The values are good, bad difer by 1%, a error I can find
+        # FIXME: The values are good, bad difer by 1%, a error I can´t find
         # In Pressure happen and only use fird
 
         M = (1-x)*IAPWS95.M + x*NH3.M
         R = 8.314471/M
 
         phio = self._phi0(rho, T, x)
         fio = phio["fio"]
@@ -283,15 +286,16 @@
                         / (1+2*delta*fird+delta**2*firdd))
         prop["w"] = (R*T*1000*(1+2*delta*fird+delta**2*firdd
                                + (1+delta*fird-delta*tau*firdt)**2 / cvR))**0.5
         prop["fugH2O"] = Z*exp(fir+delta*fird-x*F)
         prop["fugNH3"] = Z*exp(fir+delta*fird+(1-x)*F)
         return prop
 
-    def _phi0(self, rho, T, x):
+    @staticmethod
+    def _phi0(rho, T, x):
         """Ideal gas Helmholtz energy of binary mixtures and derivatives
 
         Parameters
         ----------
         rho : float
             Density, [kg/m³]
         T : float
@@ -466,15 +470,16 @@
         prop["firdd"] = (1-x)*phi1["firdd"] + x*phi2["firdd"] + Dphi["firdd"]
         prop["firdt"] = (1-x)*phi1["firdt"] + x*phi2["firdt"] + Dphi["firdt"]
         prop["firx"] = -phi1["fir"] + phi2["fir"] + Dphi["firx"]
         prop["F"] = prop["firx"] - delta/rhon*drhonx*prop["fird"] + \
             tau/Tn*dTnx*prop["firt"]
         return prop
 
-    def _Dphir(self, tau, delta, x):
+    @staticmethod
+    def _Dphir(tau, delta, x):
         """Departure function to the residual contribution to the free
         Helmholtz energy
 
         Parameters
         ----------
         tau : float
             Adimensional temperature, [-]
@@ -599,17 +604,17 @@
     References
     ----------
     IAPWS, Guideline on the IAPWS Formulation 2001 for the Thermodynamic
     Properties of Ammonia-Water Mixtures,
     http://www.iapws.org/relguide/nh3h2o.pdf, Eq 9
     """
     if 0 <= x <= 0.33367:
-        Ttr = 273.16*(1-0.3439823*x-1.3274271*x**2-274.973*x**3)
+        Tr = 273.16*(1-0.3439823*x-1.3274271*x**2-274.973*x**3)
     elif 0.33367 < x <= 0.58396:
-        Ttr = 193.549*(1-4.987368*(x-0.5)**2)
+        Tr = 193.549*(1-4.987368*(x-0.5)**2)
     elif 0.58396 < x <= 0.81473:
-        Ttr = 194.38*(1-4.886151*(x-2/3)**2+10.37298*(x-2/3)**3)
+        Tr = 194.38*(1-4.886151*(x-2/3)**2+10.37298*(x-2/3)**3)
     elif 0.81473 < x <= 1:
-        Ttr = 195.495*(1-0.323998*(1-x)-15.87560*(1-x)**4)
+        Tr = 195.495*(1-0.323998*(1-x)-15.87560*(1-x)**4)
     else:
         raise NotImplementedError("Incoming out of bound")
-    return Ttr
+    return Tr
```

### Comparing `iapws-1.5.3/iapws/humidAir.py` & `iapws-1.5.4/iapws/humidAir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
+# pylint: disable=invalid-name
+# pylint: disable=too-many-lines, too-many-locals, too-many-statements
+# pylint: disable=too-many-instance-attributes, too-many-boolean-expressions
+
 """
 Module with Air-water mixture properties and related properties. The module
 include:
 
     * :func:`_virial`: Virial equations for humid air
     * :func:`_fugacity`: Fugacity equation for humid air
     * :class:`MEoSBlend`: Special MEoS subclass to implement pseudocomponent
@@ -196,41 +200,43 @@
     References
     ----------
     IAPWS, Guideline on a Virial Equation for the Fugacity of H2O in Humid Air,
     http://www.iapws.org/relguide/VirialFugacity.html
     """
     # Check input parameters
     if T < 193 or T > 473 or P < 0 or P > 5 or x < 0 or x > 1:
-        raise(NotImplementedError("Input not in range of validity"))
+        raise NotImplementedError("Input not in range of validity")
 
-    R = 8.314462  # J/molK
+    Rg = 8.314462  # J/molK
 
     # Virial coefficients
     vir = _virial(T)
 
     # Eq 3
     beta = x*(2-x)*vir["Bww"]+(1-x)**2*(2*vir["Baw"]-vir["Baa"])
 
     # Eq 4
     gamma = x**2*(3-2*x)*vir["Cwww"] + \
         (1-x)**2*(6*x*vir["Caww"]+3*(1-2*x)*vir["Caaw"]-2*(1-x)*vir["Caaa"]) +\
         (x**2*vir["Bww"]+2*x*(1-x)*vir["Baw"]+(1-x)**2*vir["Baa"]) * \
         (x*(3*x-4)*vir["Bww"]+2*(1-x)*(3*x-2)*vir["Baw"]+3*(1-x)**2*vir["Baa"])
 
     # Eq 2
-    fv = x*P*exp(beta*P*1e6/R/T+0.5*gamma*(P*1e6/R/T)**2)
+    fv = x*P*exp(beta*P*1e6/Rg/T+0.5*gamma*(P*1e6/Rg/T)**2)
     return fv
 
 
 class MEoSBlend(MEoS):
     """
     Special meos class to implement pseudocomponent blend and defining its
     ancillary dew and bubble point
     """
 
+    _blend = {}
+
     @classmethod
     def _dewP(cls, T):
         """Using ancillary equation return the pressure of dew point"""
         c = cls._blend["dew"]
         Tj = cls._blend["Tj"]
         Pj = cls._blend["Pj"]
         Tita = 1-T/Tj
@@ -582,14 +588,44 @@
               "xa": None,
               "W": None,
               "xw": None,
               "HR": None}
 
     status = 0
     msg = "Undefined"
+    _mode = None
+    _composition = None
+
+    T = None
+    rho = None
+    v = None
+    P = None
+    s = None
+    cp = None
+    h = None
+    g = None
+    u = None
+    alfav = None
+    betas = None
+    xkappa = None
+    ks= None
+    w = None
+
+    A = None
+    W = None
+    mu = None
+    muw = None
+    M = None
+    HR = None
+    xa = None
+    xw = None
+    Pv = None
+
+    xa_sat = None
+    RH = None
 
     def __init__(self, **kwargs):
         """Constructor, define common constant and initinialice kwargs"""
         self.kwargs = HumidAir.kwargs.copy()
         self.__call__(**kwargs)
 
     def __call__(self, **kwargs):
@@ -746,19 +782,20 @@
             return gw-muw, rho**2*fa["fird"]/1000-P
 
         air = Air(T=T, P=P)
         rinput = fsolve(f, [air.rho, ao], full_output=True)
         Asat = rinput[0][1]
         if rinput[2] == 1 and 0 <= Asat <= 1:
             return Asat
-        else:
-            warnings.warn("Convergence failed")
-            print(rinput)
 
-    def _prop(self, T, rho, fav):
+        warnings.warn("Convergence failed")
+        print(rinput)
+
+    @staticmethod
+    def _prop(T, rho, fav):
         """Thermodynamic properties of humid air
 
         Parameters
         ----------
         T : float
             Temperature, [K]
         rho : float
@@ -802,15 +839,16 @@
         prop["xkappa"] = 1e3/(rho**2*(2*fav["fird"]+rho*fav["firdd"]))  # Eq T8
         prop["ks"] = 1000*fav["firtt"]/rho**2/(                         # Eq T9
             fav["firtt"]*(2*fav["fird"]+rho*fav["firdd"])-rho*fav["firdt"]**2)
         prop["w"] = (rho**2*1000*(fav["firtt"]*fav["firdd"]-fav["firdt"]**2)
                      / fav["firtt"]+2*rho*fav["fird"]*1000)**0.5       # Eq T10
         return prop
 
-    def _coligative(self, rho, A, fav):
+    @staticmethod
+    def _coligative(rho, A, fav):
         """Miscelaneous properties of humid air
 
         Parameters
         ----------
         rho : float
             Density, [kg/m³]
         A : float
@@ -914,15 +952,16 @@
         prop["firtt"] = (1-A)*fv["firtt"]+A*fa["firtt"]+fmix["firtt"]
         # Eq T19
         prop["firdt"] = (1-A)**2*fv["firdt"]+A**2*fa["firdt"]+fmix["firdt"]
         # Eq T20
         prop["firdd"] = (1-A)**3*fv["firdd"]+A**3*fa["firdd"]+fmix["firdd"]
         return prop
 
-    def _fmix(self, T, rho, A):
+    @staticmethod
+    def _fmix(T, rho, A):
         r"""Specific Helmholtz energy of air-water interaction
 
         Parameters
         ----------
         T : float
             Temperature, [K]
         rho : float
@@ -948,54 +987,54 @@
 
         References
         ----------
         IAPWS, Guideline on an Equation of State for Humid Air in Contact with
         Seawater and Ice, Consistent with the IAPWS Formulation 2008 for the
         Thermodynamic Properties of Seawater, Table 10,
         http://www.iapws.org/relguide/SeaAir.html
-        """  # noqa
-        Ma = Air.M/1000
+        """
+        ma = Air.M/1000
         Mw = IAPWS95.M/1000
         vir = _virial(T)
         Baw = vir["Baw"]
         Bawt = vir["Bawt"]
         Bawtt = vir["Bawtt"]
         Caaw = vir["Caaw"]
         Caawt = vir["Caawt"]
         Caawtt = vir["Caawtt"]
         Caww = vir["Caww"]
         Cawwt = vir["Cawwt"]
         Cawwtt = vir["Cawwtt"]
 
         # Eq T45
-        f = 2*A*(1-A)*rho*R*T/Ma/Mw*(Baw+3*rho/4*(A/Ma*Caaw+(1-A)/Mw*Caww))
+        f = 2*A*(1-A)*rho*R*T/ma/Mw*(Baw+3*rho/4*(A/ma*Caaw+(1-A)/Mw*Caww))
         # Eq T46
-        fa = 2*rho*R*T/Ma/Mw*((1-2*A)*Baw+3*rho/4*(
-            A*(2-3*A)/Ma*Caaw+(1-A)*(1-3*A)/Mw*Caww))
+        fa = 2*rho*R*T/ma/Mw*((1-2*A)*Baw+3*rho/4*(
+            A*(2-3*A)/ma*Caaw+(1-A)*(1-3*A)/Mw*Caww))
         # Eq T47
-        ft = 2*A*(1-A)*rho*R/Ma/Mw*(
-            Baw+T*Bawt+3*rho/4*(A/Ma*(Caaw+T*Caawt)+(1-A)/Mw*(Caww+T*Cawwt)))
+        ft = 2*A*(1-A)*rho*R/ma/Mw*(
+            Baw+T*Bawt+3*rho/4*(A/ma*(Caaw+T*Caawt)+(1-A)/Mw*(Caww+T*Cawwt)))
         # Eq T48
-        fd = A*(1-A)*R*T/Ma/Mw*(2*Baw+3*rho*(A/Ma*Caaw+(1-A)/Mw*Caww))
+        fd = A*(1-A)*R*T/ma/Mw*(2*Baw+3*rho*(A/ma*Caaw+(1-A)/Mw*Caww))
         # Eq T49
-        faa = rho*R*T/Ma/Mw*(-4*Baw+3*rho*((1-3*A)/Ma*Caaw-(2-3*A)/Mw*Caww))
+        faa = rho*R*T/ma/Mw*(-4*Baw+3*rho*((1-3*A)/ma*Caaw-(2-3*A)/Mw*Caww))
         # Eq T50
-        fat = 2*rho*R/Ma/Mw*(1-2*A)*(Baw+T*Bawt)+3*rho**2*R/2/Ma/Mw*(
-            A*(2-3*A)/Ma*(Caaw+T*Caawt)+(1-A)*(1-3*A)/Mw*(Caww+T*Cawwt))
+        fat = 2*rho*R/ma/Mw*(1-2*A)*(Baw+T*Bawt)+3*rho**2*R/2/ma/Mw*(
+            A*(2-3*A)/ma*(Caaw+T*Caawt)+(1-A)*(1-3*A)/Mw*(Caww+T*Cawwt))
         # Eq T51
-        fad = 2*R*T/Ma/Mw*((1-2*A)*Baw+3/2*rho*(
-            A*(2-3*A)/Ma*Caaw+(1-A)*(1-3*A)/Mw*Caww))
+        fad = 2*R*T/ma/Mw*((1-2*A)*Baw+3/2*rho*(
+            A*(2-3*A)/ma*Caaw+(1-A)*(1-3*A)/Mw*Caww))
         # Eq T52
-        ftt = 2*A*(1-A)*rho*R/Ma/Mw*(2*Bawt+T*Bawtt+3*rho/4*(
-            A/Ma*(2*Caawt+T*Caawtt)+(1-A)/Mw*(2*Cawwt+T*Cawwtt)))
+        ftt = 2*A*(1-A)*rho*R/ma/Mw*(2*Bawt+T*Bawtt+3*rho/4*(
+            A/ma*(2*Caawt+T*Caawtt)+(1-A)/Mw*(2*Cawwt+T*Cawwtt)))
         # Eq T53
-        ftd = 2*A*(1-A)*R/Ma/Mw*(Baw+T*Bawt+3*rho/2*(
-            A/Ma*(Caaw+T*Caawt)+(1-A)/Mw*(Caww+T*Cawwt)))
+        ftd = 2*A*(1-A)*R/ma/Mw*(Baw+T*Bawt+3*rho/2*(
+            A/ma*(Caaw+T*Caawt)+(1-A)/Mw*(Caww+T*Cawwt)))
         # Eq T54
-        fdd = 3*A*(1-A)*R*T/Ma/Mw*(A/Ma*Caaw+(1-A)/Mw*Caww)
+        fdd = 3*A*(1-A)*R*T/ma/Mw*(A/ma*Caaw+(1-A)/Mw*Caww)
 
         prop = {}
         prop["fir"] = f/1000
         prop["fira"] = fa/1000
         prop["firt"] = ft/1000
         prop["fird"] = fd/1000
         prop["firaa"] = faa/1000
```

### Comparing `iapws-1.5.3/iapws/iapws08.py` & `iapws-1.5.4/iapws/iapws08.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
+# pylint: disable=invalid-name
+# pylint: disable=too-many-instance-attributes, too-many-boolean-expressions
+# pylint: disable=too-many-locals
+
 """
 IAPWS standard for Seawater IAPWS08 and related functionality. The module
 include:
 
 :class:`SeaWater`: Global module class with all the functionality integrated
 
 Other functionality:
@@ -21,15 +25,15 @@
 from __future__ import division
 from math import exp, log
 import warnings
 
 from scipy.optimize import fsolve
 
 from .iapws95 import IAPWS95
-from .iapws97 import IAPWS97, _Region1, _Region2
+from .iapws97 import IAPWS97, _Region1, _Region2, _TSat_P
 from ._iapws import _ThCond, Tc, Pc, rhoc, _Ice, _Tension
 from ._utils import deriv_G
 
 
 # Constants
 Rm = 8.314472
 Sn = 0.03516504
@@ -166,14 +170,39 @@
               "P": 0.0,
               "S": None,
               "fast": False,
               "IF97": False}
     status = 0
     msg = "Undefined"
 
+    T = None
+    P = None
+    rho = None
+    v = None
+    s = None
+    cp = None
+    cv = None
+    h = None
+    u = None
+    a = None
+    alfav = None
+    betas = None
+    xkappa = None
+    ks = None
+    w = None
+    k = None
+
+    sigma = None
+    m = None
+    mu = None
+    muw = None
+    mus = None
+    osm = None
+    haline = None
+
     def __init__(self, **kwargs):
         """Constructor, initinialice kwargs"""
         self.kwargs = SeaWater.kwargs.copy()
         self.__call__(**kwargs)
 
     def __call__(self, **kwargs):
         """Make instance callable to can add input parameter one to one"""
@@ -194,15 +223,15 @@
         self.m = S/(1-S)/Ms
         if self.kwargs["fast"] and T <= 313.15:
             pw = self._waterSupp(T, P)
         elif self.kwargs["IF97"]:
             pw = self._waterIF97(T, P)
         else:
             pw = self._water(T, P)
-        ps = self._saline(T, P, S)
+        ps = self.saline(T, P, S)
 
         prop = {}
         for key in ps:
             prop[key] = pw[key]+ps[key]
             self.__setattr__(key, prop[key])
 
         self.T = T
@@ -233,28 +262,22 @@
         except NotImplementedError:
             self.k = None
 
         # Surface tension calculation
         try:
             self.sigma = _Tension_SeaWater(T, S)
         except NotImplementedError:
-            self.sigma = None
+            pass
 
         if S:
             self.mu = prop["gs"]
             self.muw = prop["g"]-S*prop["gs"]
             self.mus = prop["g"]+(1-S)*prop["gs"]
             self.osm = -(ps["g"]-S*prop["gs"])/self.m/Rm/T
             self.haline = -prop["gsp"]/prop["gp"]
-        else:
-            self.mu = None
-            self.muw = None
-            self.mus = None
-            self.osm = None
-            self.haline = None
 
     def derivative(self, z, x, y):
         """
         Wrapper derivative for custom derived properties
         where x, y, z can be: P, T, v, u, h, s, g, a
         """
         return deriv_G(self, z, x, y, self)
@@ -340,21 +363,20 @@
         prop["gtp"] = gtp/40/100*1e-6
         prop["gpp"] = gpp/100**2*1e-6
         prop["gs"] = 0
         prop["gsp"] = 0
         return prop
 
     @classmethod
-    def _saline(cls, T, P, S):
+    def saline(cls, T, P, S):
         """Eq 4"""
         # Check input in range of validity
         if T <= 261 or T > 353 or P <= 0 or P > 100 or S < 0 or S > 0.12:
             warnings.warn("Incoming out of bound")
 
-        S_ = 0.03516504*40/35
         X = (S/S_)**0.5
         tau = (T-273.15)/40
         pi = (P-0.101325)/100
 
         Li = [1, 2, 3, 4, 5, 6, 7, 1, 2, 3, 4, 5, 6, 2, 3, 4, 2, 3, 4, 2, 3, 4,
               2, 4, 2, 2, 3, 4, 5, 2, 3, 4, 2, 3, 2, 3, 2, 3, 2, 3, 4, 2, 3, 2,
               3, 2, 2, 2, 3, 4, 2, 3, 2, 3, 2, 2, 2, 3, 2, 2, 2, 2, 2, 2]
@@ -448,19 +470,25 @@
     def f(T):
         pw = _Region1(T, P)
         gw = pw["h"]-T*pw["s"]
 
         pv = _Region2(T, P)
         gv = pv["h"]-T*pv["s"]
 
-        ps = SeaWater._saline(T, P, S)
+        ps = SeaWater.saline(T, P, S)
         return -ps["g"]+S*ps["gs"]-gw+gv
 
-    Tb = fsolve(f, 300)[0]
-    return Tb
+    try:
+        to = _TSat_P(P)
+    except NotImplementedError:
+        to = 300
+    rinput = fsolve(f, to, full_output=True)
+    Tb = fsolve(f, to)[0]
+    if rinput[2] == 1:
+        return Tb
 
 
 def _Tf(P, S):
     """Procedure to calculate the freezing temperature of seawater
 
     Parameters
     ----------
@@ -482,19 +510,25 @@
     def f(T):
         T = float(T)
         pw = _Region1(T, P)
         gw = pw["h"]-T*pw["s"]
 
         gih = _Ice(T, P)["g"]
 
-        ps = SeaWater._saline(T, P, S)
+        ps = SeaWater.saline(T, P, S)
         return -ps["g"]+S*ps["gs"]-gw+gih
 
-    Tf = fsolve(f, 300)[0]
-    return Tf
+    try:
+        to = _TSat_P(P)
+    except NotImplementedError:
+        to = 300
+    rinput = fsolve(f, to, full_output=True)
+    Tf = fsolve(f, to)[0]
+    if rinput[2] == 1:
+        return Tf
 
 
 def _Triple(S):
     """Procedure to calculate the triple point pressure and temperature for
     seawater
 
     Parameters
@@ -520,15 +554,15 @@
         pw = _Region1(T, P)
         gw = pw["h"]-T*pw["s"]
 
         pv = _Region2(T, P)
         gv = pv["h"]-T*pv["s"]
 
         gih = _Ice(T, P)["g"]
-        ps = SeaWater._saline(T, P, S)
+        ps = SeaWater.saline(T, P, S)
 
         return -ps["g"]+S*ps["gs"]-gw+gih, -ps["g"]+S*ps["gs"]-gw+gv
 
     Tt, Pt = fsolve(f, [273, 6e-4])
 
     prop = {}
     prop["Tt"] = Tt
@@ -560,15 +594,15 @@
     """
     pw = _Region1(T, P)
     gw = pw["h"]-T*pw["s"]
 
     def f(Posm):
         pw2 = _Region1(T, P+Posm)
         gw2 = pw2["h"]-T*pw2["s"]
-        ps = SeaWater._saline(T, P+Posm, S)
+        ps = SeaWater.saline(T, P+Posm, S)
         return -ps["g"]+S*ps["gs"]-gw+gw2
 
     Posm = fsolve(f, 0)[0]
     return Posm
 
 
 def _ThCond_SeaWater(T, P, S):
```

### Comparing `iapws-1.5.3/iapws/iapws95.py` & `iapws-1.5.4/iapws/iapws95.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
+# pylint: disable=invalid-name
+# pylint: disable=too-many-lines, too-many-locals, too-many-instance-attributes
+# pylint: disable=too-many-branches, too-many-statements
 
 """
 Implemented multiparameter equation of state as a Helmholtz free energy:
 
     * :class:`MEoS`: Base class of multiparameter equation of state
     * :class:`IAPWS95`: 2016 revision of 1995 formulation for ordinaty water
     * :class:`D2O`: 2017 formulation for heavy water.
@@ -365,33 +368,73 @@
 
         * Z_rho: :math:`(Z-1)/\rho`, [m³/kg]
         * IntP: Internal pressure, [MPa]
         * invT: Negative reciprocal temperature, [1/K]
         * hInput: Specific heat input, [kJ/kg]
     """
 
-    CP = None
-    _Pv = None
-    _rhoL = None
-    _rhoG = None
+    Fi0 = {}
+    _constants = {}
+    _Pv = {}
+    _rhoL = {}
+    _rhoG = {}
+    _surf = {}
 
     kwargs = {"T": 0.0,
               "P": 0.0,
               "rho": 0.0,
               "v": 0.0,
               "h": None,
               "s": None,
               "u": None,
               "x": None,
               "l": 0.5893,
               "rho0": None,
               "T0": None,
               "x0": 0.5}
+
+    name = None
+    M = None
+    Tc = None
+    Pc = None
+    rhoc = None
+    Tt = None
+
     status = 0
     msg = "Undefined"
+    _mode = None
+
+    Liquid = None
+    Gas = None
+
+    T = None
+    Tr = None
+    P = None
+    Pr = None
+    x = None
+    phase = None
+
+    sigma = None
+    virialB = None
+    virialC = None
+    Hvap = None
+    Svap = None
+    invT = None
+
+    v0 = None
+    rho0 = None
+    h0 = None
+    u0 = None
+    s0 = None
+    a0 = None
+    g0 = None
+    cp0 = None
+    cv0 = None
+    cp0_cv = None
+    gamma0 = None
 
     def __init__(self, **kwargs):
         """Constructor, define common constant and initinialice kwargs"""
         self.R = self._constants["R"]/self._constants.get("M", self.M)
         self.Zc = self.Pc/self.rhoc/self.R/self.Tc
         self.kwargs = MEoS.kwargs.copy()
         self.__call__(**kwargs)
@@ -414,15 +457,15 @@
             try:
                 self.status = 1
                 self.calculo()
                 self.msg = ""
             except RuntimeError as err:
                 self.status = 0
                 self.msg = err.args[0]
-                raise(err)
+                raise err
 
             # Add msg for extrapolation state
             if self.name == "water" and 130 <= self.T < 273.15:
                 self.msg = "Extrapolated state"
                 self.status = 3
                 warnings.warn("Using extrapolated values")
             elif self.name == "water" and 50 <= self.T < 130:
@@ -502,41 +545,41 @@
                     To = st0.T
                     rhoo = st0.rho
                 else:
                     To = 300
                     rhoo = 900
 
         self.R = self._constants["R"]/self._constants.get("M", self.M)
-        rhoc = self._constants.get("rhoref", self.rhoc)
-        Tc = self._constants.get("Tref", self.Tc)
+        rho_c = self._constants.get("rhoref", self.rhoc)
+        T_c = self._constants.get("Tref", self.Tc)
 
         propiedades = None
 
         if self._mode not in ("Tx", "Px"):
             # Method with iteration necessary to get x
             if self._mode == "TP":
                 try:
                     if self.name != "water":
                         raise NotImplementedError
                     st0 = IAPWS97(**self.kwargs)
                     rhoo = st0.rho
                 except NotImplementedError:
                     if rho0:
                         rhoo = rho0
-                    elif T < self.Tc and P < self.Pc and \
-                            self._Vapor_Pressure(T) < P:
+                    elif T < self.Tc and \
+                            self._Vapor_Pressure(T) < P < self.Pc:
                         rhoo = self._Liquid_Density(T)
                     elif T < self.Tc and P < self.Pc:
                         rhoo = self._Vapor_Density(T)
                     else:
                         rhoo = self.rhoc*3
 
                 def f(rho):
-                    delta = rho/rhoc
-                    tau = Tc/T
+                    delta = rho/rho_c
+                    tau = T_c/T
 
                     fird = _phird(tau, delta, self._constants)
                     Po = (1+delta*fird)*self.R*T*rho
                     return Po-P*1000
 
                 rho = fsolve(f, rhoo)[0]
 
@@ -551,34 +594,34 @@
 
                     if Ps > P:
                         x = 1
                     else:
                         x = 0
 
             elif self._mode == "Th":
-                tau = Tc/T
+                tau = T_c/T
                 ideal = self._phi0(tau, 1)
                 fiot = ideal["fiot"]
 
                 def f(rho):
-                    delta = rho/rhoc
+                    delta = rho/rho_c
                     fird = _phird(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     ho = self.R*T*(1+tau*(fiot+firt)+delta*fird)
                     return ho-h
 
                 if T >= self.Tc:
                     rhoo = self.rhoc
                     rho = fsolve(f, rhoo)[0]
                 else:
                     x0 = self.kwargs["x0"]
                     rhov = self._Vapor_Density(T)
                     rhol = self._Liquid_Density(T)
-                    deltaL = rhol/rhoc
-                    deltaG = rhov/rhoc
+                    deltaL = rhol/rho_c
+                    deltaG = rhov/rho_c
 
                     firdL = _phird(tau, deltaL, self._constants)
                     firtL = _phirt(tau, deltaL, self._constants)
                     firdG = _phird(tau, deltaG, self._constants)
                     firtG = _phirt(tau, deltaG, self._constants)
                     hl = self.R*T*(1+tau*(fiot+firtL)+deltaL*firdL)
                     hv = self.R*T*(1+tau*(fiot+firtG)+deltaG*firdG)
@@ -595,20 +638,20 @@
                         if h > hv:
                             rhoo = rhov
                         else:
                             rhoo = rhol
                         rho = fsolve(f, rhoo)[0]
 
             elif self._mode == "Ts":
-                tau = Tc/T
+                tau = T_c/T
 
                 def f(rho):
                     if rho < 0:
                         rho = 1e-20
-                    delta = rho/rhoc
+                    delta = rho/rho_c
 
                     ideal = self._phi0(tau, delta)
                     fio = ideal["fio"]
                     fiot = ideal["fiot"]
                     fir = _phir(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     so = self.R*(tau*(fiot+firt)-fio-fir)
@@ -616,16 +659,16 @@
 
                 if T >= self.Tc:
                     rhoo = self.rhoc
                     rho = fsolve(f, rhoo)[0]
                 else:
                     rhov = self._Vapor_Density(T)
                     rhol = self._Liquid_Density(T)
-                    deltaL = rhol/rhoc
-                    deltaG = rhov/rhoc
+                    deltaL = rhol/rho_c
+                    deltaG = rhov/rho_c
 
                     idealL = self._phi0(tau, deltaL)
                     idealG = self._phi0(tau, deltaG)
                     fioL = idealL["fio"]
                     fioG = idealG["fio"]
                     fiot = idealL["fiot"]
                     firL = _phir(tau, deltaL, self._constants)
@@ -648,36 +691,36 @@
                         if s > sv:
                             rhoo = rhov
                         else:
                             rhoo = rhol
                         rho = fsolve(f, rhoo)[0]
 
             elif self._mode == "Tu":
-                tau = Tc/T
+                tau = T_c/T
                 ideal = self._phi0(tau, 1)
                 fiot = ideal["fiot"]
 
                 def f(rho):
-                    delta = rho/rhoc
+                    delta = rho/rho_c
 
                     fird = _phird(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     Po = (1+delta*fird)*self.R*T*rho
                     ho = self.R*T*(1+tau*(fiot+firt)+delta*fird)
 
                     return ho-Po/rho-u
 
                 if T >= self.Tc:
                     rhoo = self.rhoc
                     rho = fsolve(f, rhoo)[0]
                 else:
                     rhov = self._Vapor_Density(T)
                     rhol = self._Liquid_Density(T)
-                    deltaL = rhol/rhoc
-                    deltaG = rhov/rhoc
+                    deltaL = rhol/rho_c
+                    deltaG = rhov/rho_c
 
                     firdL = _phird(tau, deltaL, self._constants)
                     firtL = _phirt(tau, deltaL, self._constants)
                     firdG = _phird(tau, deltaG, self._constants)
                     firtG = _phirt(tau, deltaG, self._constants)
                     PoL = (1+deltaL*firdL)*self.R*T*rhol
                     PoG = (1+deltaG*firdG)*self.R*T*rhov
@@ -699,31 +742,31 @@
                         if u > uv:
                             rhoo = rhov
                         else:
                             rhoo = rhol
                         rho = fsolve(f, rhoo)[0]
 
             elif self._mode == "Prho":
-                delta = rho/rhoc
+                delta = rho/rho_c
 
                 def f(T):
-                    tau = Tc/T
+                    tau = T_c/T
 
                     fird = _phird(tau, delta, self._constants)
                     Po = (1+delta*fird)*self.R*T*rho
                     return Po-P*1000
 
                 T = fsolve(f, To)[0]
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if T == To or rhov <= rho <= rhol:
 
                     def f(parr):
                         T, rhol, rhog = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         firL = _phir(tau, deltaL, self._constants)
                         firdL = _phird(tau, deltaL, self._constants)
                         firG = _phir(tau, deltaG, self._constants)
                         firdG = _phird(tau, deltaG, self._constants)
@@ -743,26 +786,26 @@
                         T, rhoL, rhoG = sol[0]
                         x = (1./rho-1/rhoL)/(1/rhoG-1/rhoL)
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "Ph":
                 def funcion(parr):
                     rho, T = parr
-                    delta = rho/rhoc
-                    tau = Tc/T
+                    delta = rho/rho_c
+                    tau = T_c/T
 
                     ideal = self._phi0(tau, delta)
                     fiot = ideal["fiot"]
                     fird = _phird(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     Po = (1+delta*fird)*self.R*T*rho
                     ho = self.R*T*(1+tau*(fiot+firt)+delta*fird)
@@ -771,15 +814,15 @@
                 rho, T = fsolve(funcion, [rhoo, To])
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if rho == rhoo or rhov <= rho <= rhol:
 
                     def f(parr):
                         T, rhol, rhog, x = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         ideal = self._phi0(tau, deltaL)
                         fiot = ideal["fiot"]
 
                         firL = _phir(tau, deltaL, self._constants)
@@ -807,15 +850,15 @@
                         sol = fsolve(f, [to, rLo, rGo, 0.5], full_output=True)
                         T, rhoL, rhoG, x = sol[0]
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "Ps":
@@ -823,16 +866,16 @@
                     x0 = st0.x
                 except NameError:
                     x0 = None
 
                 if x0 is None or x0 == 0 or x0 == 1:
                     def f(parr):
                         rho, T = parr
-                        delta = rho/rhoc
-                        tau = Tc/T
+                        delta = rho/rho_c
+                        tau = T_c/T
 
                         ideal = self._phi0(tau, delta)
                         fio = ideal["fio"]
                         fiot = ideal["fiot"]
                         fird = _phird(tau, delta, self._constants)
                         fir = _phir(tau, delta, self._constants)
                         firt = _phirt(tau, delta, self._constants)
@@ -857,16 +900,16 @@
                     sv = vapor["s"]
                     sl = liquido["s"]
                     x = (s-sl)/(sv-sl)
 
             elif self._mode == "Pu":
                 def f(parr):
                     rho, T = parr
-                    delta = rho/rhoc
-                    tau = Tc/T
+                    delta = rho/rho_c
+                    tau = T_c/T
 
                     ideal = self._phi0(tau, delta)
                     fiot = ideal["fiot"]
                     fird = _phird(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     Po = (1+delta*fird)*self.R*T*rho
                     ho = self.R*T*(1+tau*(fiot+firt)+delta*fird)
@@ -876,15 +919,15 @@
                 rho, T = sol[0]
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if rho == rhoo or sol[2] != 1:
 
                     def f(parr):
                         T, rhol, rhog, x = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         ideal = self._phi0(tau, deltaL)
                         fiot = ideal["fiot"]
 
                         firL = _phir(tau, deltaL, self._constants)
@@ -913,41 +956,41 @@
                         sol = fsolve(f, [to, rLo, rGo, 0.5], full_output=True)
                         T, rhoL, rhoG, x = sol[0]
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "rhoh":
-                delta = rho/rhoc
+                delta = rho/rho_c
 
                 def f(T):
-                    tau = Tc/T
+                    tau = T_c/T
 
                     ideal = self._phi0(tau, delta)
                     fiot = ideal["fiot"]
                     fird = _phird(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     ho = self.R*T*(1+tau*(fiot+firt)+delta*fird)
                     return ho-h
 
                 T = fsolve(f, To)[0]
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if T == To or rhov <= rho <= rhol:
                     def f(parr):
                         T, rhol, rhog = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         ideal = self._phi0(tau, deltaL)
                         fiot = ideal["fiot"]
                         firL = _phir(tau, deltaL, self._constants)
                         firdL = _phird(tau, deltaL, self._constants)
@@ -973,26 +1016,26 @@
                         T, rhoL, rhoG = sol[0]
                         x = (1./rho-1/rhoL)/(1/rhoG-1/rhoL)
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "rhos":
-                delta = rho/rhoc
+                delta = rho/rho_c
 
                 def f(T):
-                    tau = Tc/T
+                    tau = T_c/T
                     ideal = self._phi0(tau, delta)
                     fio = ideal["fio"]
                     fiot = ideal["fiot"]
                     fir = _phir(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     so = self.R*(tau*(fiot+firt)-fio-fir)
                     return so-s
@@ -1000,15 +1043,15 @@
                 T = fsolve(f, To)[0]
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if T == To or rhov <= rho <= rhol:
 
                     def f(parr):
                         T, rhol, rhog = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         idealL = self._phi0(tau, deltaL)
                         fioL = idealL["fio"]
                         fiot = idealL["fiot"]
                         idealG = self._phi0(tau, deltaG)
@@ -1038,26 +1081,26 @@
                         T, rhoL, rhoG = sol[0]
                         x = (1./rho-1/rhoL)/(1/rhoG-1/rhoL)
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "rhou":
-                delta = rho/rhoc
+                delta = rho/rho_c
 
                 def f(T):
-                    tau = Tc/T
+                    tau = T_c/T
 
                     ideal = self._phi0(tau, delta)
                     fiot = ideal["fiot"]
                     fird = _phird(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     Po = (1+delta*fird)*self.R*T*rho
                     ho = self.R*T*(1+tau*(fiot+firt)+delta*fird)
@@ -1065,15 +1108,15 @@
 
                 T = fsolve(f, To)[0]
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if T == To or rhov <= rho <= rhol:
                     def f(parr):
                         T, rhol, rhog = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         ideal = self._phi0(tau, deltaL)
                         fiot = ideal["fiot"]
                         firL = _phir(tau, deltaL, self._constants)
                         firdL = _phird(tau, deltaL, self._constants)
@@ -1102,26 +1145,26 @@
                         T, rhoL, rhoG = sol[0]
                         x = (1./rho-1/rhoL)/(1/rhoG-1/rhoL)
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "hs":
                 def f(parr):
                     rho, T = parr
-                    delta = rho/rhoc
-                    tau = Tc/T
+                    delta = rho/rho_c
+                    tau = T_c/T
 
                     ideal = self._phi0(tau, delta)
                     fio = ideal["fio"]
                     fiot = ideal["fiot"]
                     fird = _phird(tau, delta, self._constants)
                     fir = _phir(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
@@ -1132,15 +1175,15 @@
                 rho, T = fsolve(f, [rhoo, To])
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if rhov <= rho <= rhol:
 
                     def f(parr):
                         T, rhol, rhog, x = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         idealL = self._phi0(tau, deltaL)
                         fiot = idealL["fiot"]
                         fioL = idealL["fio"]
                         idealG = self._phi0(tau, deltaG)
@@ -1171,26 +1214,26 @@
                         sol = fsolve(f, [to, rLo, rGo, 0.5], full_output=True)
                         T, rhoL, rhoG, x = sol[0]
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "hu":
                 def f(parr):
                     rho, T = parr
-                    delta = rho/rhoc
-                    tau = Tc/T
+                    delta = rho/rho_c
+                    tau = T_c/T
 
                     ideal = self._phi0(tau, delta)
                     fiot = ideal["fiot"]
                     fird = _phird(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
                     Po = (1+delta*fird)*self.R*T*rho
                     ho = self.R*T*(1+tau*(fiot+firt)+delta*fird)
@@ -1201,15 +1244,15 @@
                 rho, T = sol[0]
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if sol[2] != 1 or rhov <= rho <= rhol:
 
                     def f(parr):
                         T, rhol, rhog, x = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         ideal = self._phi0(tau, deltaL)
                         fiot = ideal["fiot"]
 
                         firL = _phir(tau, deltaL, self._constants)
@@ -1240,26 +1283,26 @@
                         sol = fsolve(f, [to, rLo, rGo, 0.5], full_output=True)
                         T, rhoL, rhoG, x = sol[0]
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "su":
                 def f(parr):
                     rho, T = parr
-                    delta = rho/rhoc
-                    tau = Tc/T
+                    delta = rho/rho_c
+                    tau = T_c/T
 
                     ideal = self._phi0(tau, delta)
                     fio = ideal["fio"]
                     fiot = ideal["fiot"]
                     fird = _phird(tau, delta, self._constants)
                     fir = _phir(tau, delta, self._constants)
                     firt = _phirt(tau, delta, self._constants)
@@ -1272,15 +1315,15 @@
                 rho, T = sol[0]
                 rhol = self._Liquid_Density(T)
                 rhov = self._Vapor_Density(T)
                 if sol[2] != 1 or rhov <= rho <= rhol:
 
                     def f(parr):
                         T, rhol, rhog, x = parr
-                        tau = Tc/T
+                        tau = T_c/T
                         deltaL = rhol/self.rhoc
                         deltaG = rhog/self.rhoc
 
                         idealL = self._phi0(tau, deltaL)
                         fiot = idealL["fiot"]
                         fioL = idealL["fio"]
                         idealG = self._phi0(tau, deltaG)
@@ -1316,15 +1359,15 @@
                         sol = fsolve(f, [to, rLo, rGo, 0.5], full_output=True)
                         T, rhoL, rhoG, x = sol[0]
                         if sol[2] == 1 and 0 <= x <= 1 and \
                                 sum(abs(sol[1]["fvec"])) < 1e-5:
                             break
 
                     if sum(abs(sol[1]["fvec"])) > 1e-5:
-                        raise(RuntimeError(sol[3]))
+                        raise RuntimeError(sol[3])
 
                     liquido = self._Helmholtz(rhoL, T)
                     vapor = self._Helmholtz(rhoG, T)
                     P = self.R*T*rhoL*rhoG/(rhoL-rhoG)*(
                         liquido["fir"]-vapor["fir"]+log(rhoL/rhoG))/1000
 
             elif self._mode == "Trho":
@@ -1374,15 +1417,15 @@
             def f(T):
                 rhol = self._Liquid_Density(T)
                 rhog = self._Vapor_Density(T)
 
                 deltaL = rhol/self.rhoc
                 deltaG = rhog/self.rhoc
 
-                tau = Tc/T
+                tau = T_c/T
 
                 firL = _phir(tau, deltaL, self._constants)
                 firG = _phir(tau, deltaG, self._constants)
                 Ps = self.R*T*rhol*rhog/(rhol-rhog)*(
                     firL-firG+log(deltaL/deltaG))
                 return Ps/1000-P
 
@@ -1408,14 +1451,19 @@
         self.x = x
         if self._mode in ["Tx", "Px"] or 0 < x < 1:
             region = 4
         else:
             region = 0
         self.phase = getphase(self.Tc, self.Pc, self.T, self.P, self.x, region)
 
+        if 0 < x < 1:
+            rho = vapor["rho"]
+        else:
+            rho = propiedades["rho"]
+
         self.Liquid = _fase()
         self.Gas = _fase()
         if x == 0:
             # liquid phase
             self.fill(self.Liquid, propiedades)
             self.fill(self, propiedades)
         elif x == 1:
@@ -1457,17 +1505,17 @@
         else:
             self.Hvap = None
             self.Svap = None
 
         self.invT = -1/self.T
 
         # Ideal properties
-        cp0 = self._prop0(self.rho, self.T)
         self.v0 = self.R*self.T/self.P/1000
         self.rho0 = 1./self.v0
+        cp0 = self._prop0(self.rho0, self.T)
         self.h0 = cp0.h
         self.u0 = self.h0-self.P*self.v0
         self.s0 = cp0.s
         self.a0 = self.u0-self.T*self.s0
         self.g0 = self.h0-self.T*self.s0
         self.cp0 = cp0.cp
         self.cv0 = cp0.cv
@@ -1510,15 +1558,16 @@
 
         fase.joule = self.derivative("T", "P", "h", fase)*1e3
         fase.Gruneisen = fase.v/fase.cv*self.derivative("P", "T", "v", fase)
         fase.alfav = self.derivative("v", "T", "P", fase)/fase.v
         fase.kappa = -self.derivative("v", "P", "T", fase)/fase.v*1e3
         fase.betas = self.derivative("T", "P", "s", fase)
 
-        fase.gamma = -fase.v/self.P*self.derivative("P", "v", "s", fase)*1e-3
+        fase.gamma = -fase.v/self.P \
+            * self.derivative("P", "v", "T", fase)*fase.cp_cv*1e-3
         fase.kt = -fase.v/self.P*self.derivative("P", "v", "T", fase)*1e-3
         fase.ks = -self.derivative("v", "P", "s", fase)/fase.v*1e3
         fase.Kt = -fase.v*self.derivative("P", "v", "s", fase)*1e-3
         fase.Ks = -fase.v*self.derivative("P", "v", "T", fase)*1e-3
         fase.dhdT_rho = self.derivative("h", "T", "rho", fase)
         fase.dhdT_P = self.derivative("h", "T", "P", fase)
         fase.dhdP_T = self.derivative("h", "P", "T", fase)*1e3
@@ -1558,28 +1607,28 @@
         Wrapper derivative for custom derived properties
         where x, y, z can be: P, T, v, rho, u, h, s, g, a
         """
         return deriv_H(self, z, x, y, fase)
 
     def _saturation(self, T):
         """Saturation calculation for two phase search"""
-        rhoc = self._constants.get("rhoref", self.rhoc)
-        Tc = self._constants.get("Tref", self.Tc)
+        rho_c = self._constants.get("rhoref", self.rhoc)
+        T_c = self._constants.get("Tref", self.Tc)
 
-        if T > Tc:
-            T = Tc
-        tau = Tc/T
+        if T > T_c:
+            T = T_c
+        tau = T_c/T
 
         rhoLo = self._Liquid_Density(T)
         rhoGo = self._Vapor_Density(T)
 
         def f(parr):
             rhol, rhog = parr
-            deltaL = rhol/rhoc
-            deltaG = rhog/rhoc
+            deltaL = rhol/rho_c
+            deltaG = rhog/rho_c
             phirL = _phir(tau, deltaL, self._constants)
             phirG = _phir(tau, deltaG, self._constants)
             phirdL = _phird(tau, deltaL, self._constants)
             phirdG = _phird(tau, deltaG, self._constants)
             Jl = deltaL*(1+deltaL*phirdL)
             Jv = deltaG*(1+deltaG*phirdG)
             Kl = deltaL*phirdL+phirL+log(deltaL)
@@ -1634,18 +1683,18 @@
             rho = rho[0]
         if isinstance(T, ndarray):
             T = T[0]
         if rho < 0:
             rho = 1e-20
         if T < 50:
             T = 50
-        rhoc = self._constants.get("rhoref", self.rhoc)
-        Tc = self._constants.get("Tref", self.Tc)
-        delta = rho/rhoc
-        tau = Tc/T
+        rho_c = self._constants.get("rhoref", self.rhoc)
+        T_c = self._constants.get("Tref", self.Tc)
+        delta = rho/rho_c
+        tau = T_c/T
         ideal = self._phi0(tau, delta)
         fio = ideal["fio"]
         fiot = ideal["fiot"]
         fiott = ideal["fiott"]
 
         res = self._phir(tau, delta)
         fir = res["fir"]
@@ -1669,18 +1718,18 @@
         propiedades["alfap"] = (1-delta*tau*firdt/(1+delta*fird))/T
         propiedades["betap"] = rho*(
             1+(delta*fird+delta**2*firdd)/(1+delta*fird))
         return propiedades
 
     def _prop0(self, rho, T):
         """Ideal gas properties"""
-        rhoc = self._constants.get("rhoref", self.rhoc)
-        Tc = self._constants.get("Tref", self.Tc)
-        delta = rho/rhoc
-        tau = Tc/T
+        rho_c = self._constants.get("rhoref", self.rhoc)
+        T_c = self._constants.get("Tref", self.Tc)
+        delta = rho/rho_c
+        tau = T_c/T
         ideal = self._phi0(tau, delta)
         fio = ideal["fio"]
         fiot = ideal["fiot"]
         fiott = ideal["fiott"]
 
         propiedades = _fase()
         propiedades.h = self.R*T*(1+tau*fiot)
@@ -1901,16 +1950,16 @@
         Returns
         -------
         prop : dict
             Dictionary with residual adimensional helmholtz energy:
                 * B: ∂fir/∂δ|δ->0
                 * C: ∂²fir/∂δ²|δ->0
         """
-        Tc = self._constants.get("Tref", self.Tc)
-        tau = Tc/T
+        T_c = self._constants.get("Tref", self.Tc)
+        tau = T_c/T
         B = C = 0
         delta = 1e-200
 
         # Polinomial terms
         nr1 = self._constants.get("nr1", [])
         d1 = self._constants.get("d1", [])
         t1 = self._constants.get("t1", [])
@@ -2014,18 +2063,18 @@
             prop["fird"] = 0
             prop["firtt"] = 0
             prop["firdt"] = 0
             prop["firdd"] = 0
             return prop
 
         R = self._constants.get("R")/self._constants.get("M", self.M)
-        rhoc = self._constants.get("rhoref", self.rhoc)
-        Tc = self._constants.get("Tref", self.Tc)
-        delta = rho/rhoc
-        tau = Tc/T
+        rho_c = self._constants.get("rhoref", self.rhoc)
+        T_c = self._constants.get("Tref", self.Tc)
+        delta = rho/rho_c
+        tau = T_c/T
 
         ideal = self._phi0(tau, delta)
         fio = ideal["fio"]
         fiot = ideal["fiot"]
         fiott = ideal["fiott"]
         fiod = ideal["fiod"]
         fiodd = ideal["fiodd"]
@@ -2037,18 +2086,18 @@
         fird = res["fird"]
         firdd = res["firdd"]
         firdt = res["firdt"]
 
         prop = {}
         prop["fir"] = R*T*(fio+fir)
         prop["firt"] = R*(fio+fir-(fiot+firt)*tau)
-        prop["fird"] = R*T/rhoc*(fiod+fird)
+        prop["fird"] = R*T/rho_c*(fiod+fird)
         prop["firtt"] = R*tau**2/T*(fiott+firtt)
-        prop["firdt"] = R/rhoc*(fiod+fird-firdt*tau)
-        prop["firdd"] = R*T/rhoc**2*(fiodd+firdd)
+        prop["firdt"] = R/rho_c*(fiod+fird-firdt*tau)
+        prop["firdd"] = R*T/rho_c**2*(fiodd+firdd)
         return prop
 
     def _surface(self, T):
         """Generic equation for the surface tension
 
         Parameters
         ----------
@@ -2088,14 +2137,19 @@
 
         References
         ----------
         IAPWS, Revised Supplementary Release on Saturation Properties of
         Ordinary Water Substance September 1992,
         http://www.iapws.org/relguide/Supp-sat.html, Eq.1
         """
+        if T < cls.Tt:
+            T = cls.Tt
+        elif T > cls.Tc:
+            T = cls.Tc
+
         Tita = 1-T/cls.Tc
         suma = 0
         for n, x in zip(cls._Pv["ao"], cls._Pv["exp"]):
             suma += n*Tita**x
         Pr = exp(cls.Tc/T*suma)
         Pv = Pr*cls.Pc
         return Pv
@@ -2116,14 +2170,19 @@
 
         References
         ----------
         IAPWS, Revised Supplementary Release on Saturation Properties of
         Ordinary Water Substance September 1992,
         http://www.iapws.org/relguide/Supp-sat.html, Eq.2
         """
+        if T < cls.Tt:
+            T = cls.Tt
+        elif T > cls.Tc:
+            T = cls.Tc
+
         eq = cls._rhoL["eq"]
         Tita = 1-T/cls.Tc
         if eq == 2:
             Tita = Tita**(1./3)
         suma = 0
         for n, x in zip(cls._rhoL["ao"], cls._rhoL["exp"]):
             suma += n*Tita**x
@@ -2147,14 +2206,19 @@
 
         References
         ----------
         IAPWS, Revised Supplementary Release on Saturation Properties of
         Ordinary Water Substance September 1992,
         http://www.iapws.org/relguide/Supp-sat.html, Eq.3
         """
+        if T < cls.Tt:
+            T = cls.Tt
+        elif T > cls.Tc:
+            T = cls.Tc
+
         eq = cls._rhoG["eq"]
         Tita = 1-T/cls.Tc
         if eq == 4:
             Tita = Tita**(1./3)
         suma = 0
         for n, x in zip(cls._rhoG["ao"], cls._rhoG["exp"]):
             suma += n*Tita**x
```

### Comparing `iapws-1.5.3/setup.py` & `iapws-1.5.4/setup.py`

 * *Files identical despite different names*

