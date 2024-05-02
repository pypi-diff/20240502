# Comparing `tmp/spelunker-1.1.8.tar.gz` & `tmp/spelunker-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spelunker-1.1.8.tar", last modified: Tue Mar 19 15:43:41 2024, max compression
+gzip compressed data, was "spelunker-1.1.9.tar", last modified: Wed Mar 20 02:03:45 2024, max compression
```

## Comparing `spelunker-1.1.8.tar` & `spelunker-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 galagabits  (1000) galagabits  (1000)        0 2024-03-19 15:43:41.213552 spelunker-1.1.8/
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)     1085 2024-03-17 15:44:18.000000 spelunker-1.1.8/LICENSE
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)     4926 2024-03-19 15:43:41.213552 spelunker-1.1.8/PKG-INFO
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)     4319 2024-03-19 04:25:54.000000 spelunker-1.1.8/README.md
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)      160 2024-03-19 15:43:41.213552 spelunker-1.1.8/setup.cfg
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)      926 2024-03-19 15:40:26.000000 spelunker-1.1.8/setup.py
-drwxr-xr-x   0 galagabits  (1000) galagabits  (1000)        0 2024-03-19 15:43:41.213552 spelunker-1.1.8/spelunker.egg-info/
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)     4926 2024-03-19 15:43:41.000000 spelunker-1.1.8/spelunker.egg-info/PKG-INFO
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)      281 2024-03-19 15:43:41.000000 spelunker-1.1.8/spelunker.egg-info/SOURCES.txt
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)        1 2024-03-19 15:43:41.000000 spelunker-1.1.8/spelunker.egg-info/dependency_links.txt
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)        1 2024-03-19 15:43:41.000000 spelunker-1.1.8/spelunker.egg-info/not-zip-safe
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)       74 2024-03-19 15:43:41.000000 spelunker-1.1.8/spelunker.egg-info/requires.txt
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)       10 2024-03-19 15:43:41.000000 spelunker-1.1.8/spelunker.egg-info/top_level.txt
-drwxr-xr-x   0 galagabits  (1000) galagabits  (1000)        0 2024-03-19 15:43:41.213552 spelunker-1.1.8/src/
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)       84 2024-03-18 07:05:21.000000 spelunker-1.1.8/src/__init__.py
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)       21 2024-03-19 15:42:21.000000 spelunker-1.1.8/src/_version.py
--rw-r--r--   0 galagabits  (1000) galagabits  (1000)    89554 2024-03-19 15:05:41.000000 spelunker-1.1.8/src/spelunker.py
+drwxr-xr-x   0 galagabits  (1000) galagabits  (1000)        0 2024-03-20 02:03:45.419827 spelunker-1.1.9/
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)     1085 2024-03-17 15:44:18.000000 spelunker-1.1.9/LICENSE
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)     5962 2024-03-20 02:03:45.419827 spelunker-1.1.9/PKG-INFO
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)     5355 2024-03-19 23:30:13.000000 spelunker-1.1.9/README.md
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)      160 2024-03-20 02:03:45.419827 spelunker-1.1.9/setup.cfg
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)      926 2024-03-19 15:40:26.000000 spelunker-1.1.9/setup.py
+drwxr-xr-x   0 galagabits  (1000) galagabits  (1000)        0 2024-03-20 02:03:45.419827 spelunker-1.1.9/spelunker.egg-info/
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)     5962 2024-03-20 02:03:45.000000 spelunker-1.1.9/spelunker.egg-info/PKG-INFO
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)      281 2024-03-20 02:03:45.000000 spelunker-1.1.9/spelunker.egg-info/SOURCES.txt
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)        1 2024-03-20 02:03:45.000000 spelunker-1.1.9/spelunker.egg-info/dependency_links.txt
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)        1 2024-03-20 02:03:45.000000 spelunker-1.1.9/spelunker.egg-info/not-zip-safe
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)       74 2024-03-20 02:03:45.000000 spelunker-1.1.9/spelunker.egg-info/requires.txt
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)       10 2024-03-20 02:03:45.000000 spelunker-1.1.9/spelunker.egg-info/top_level.txt
+drwxr-xr-x   0 galagabits  (1000) galagabits  (1000)        0 2024-03-20 02:03:45.419827 spelunker-1.1.9/src/
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)       84 2024-03-18 07:05:21.000000 spelunker-1.1.9/src/__init__.py
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)       21 2024-03-20 02:03:24.000000 spelunker-1.1.9/src/_version.py
+-rw-r--r--   0 galagabits  (1000) galagabits  (1000)    89675 2024-03-20 01:58:25.000000 spelunker-1.1.9/src/spelunker.py
```

### Comparing `spelunker-1.1.8/LICENSE` & `spelunker-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spelunker-1.1.8/PKG-INFO` & `spelunker-1.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 1.1.8
+Version: 1.1.9
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
 Requires-Python: >=3.10
@@ -68,47 +68,55 @@
 plt.ylabel('Counts')
 
 ```
 <p align='center'>
     <img src="plots/timeseries.png"  width=100% height=80%>
 </p>
 
-(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). We can even make a plot of the tracked guidestars within this Program ID:
+(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). 
+
+We can even make a plot of the tracked guidestars within this Program ID. Within a selected Program ID, multiple guidestars could be used for each observation. Each star or object comes from the Guide Star Catalog (GSC) and is pre-selected depending on [telescope pointing and suitability of the star](https://jwst-docs.stsci.edu/jwst-observatory-characteristics/jwst-guide-stars). In the generated figure from `spk.guidestar_plot`, the guidestar positions (marked with an X) in the given Program ID are plotted from the *START* to the end of the program. A line (`gs track`) is traced between each guidestar to order each used target overtime.
 
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/):
+
+
+Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/). Here, use `spk.mnemonics` to access engineering telemetry for `SA_ZHAGUPST` as a matplotlib `axes` object:
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
 
-ax = spk.mnemonics_local('GUIDESTAR')
-ax = spk.mnemonics('SA_ZHGAUPST', 60067.84, 60067.9) 
+ax = spk.mnemonics_local('GUIDESTAR') # plots when the JWST tracks onto a new guidestars as a vertical line
+ax = spk.mnemonics('SA_ZHGAUPST', 60067.84, 60067.9) # plots the start and end of high gain antenna movement
+
 ax.plot(spk.fg_time, spk.fg_flux)
 plt.legend(loc=3)
 plt.xlim(60067.84, 60067.9)
 plt.show()
 ```
+
+
 <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/mnemonics.png">
 
 For more information on the tools under `spelunker` and how to get started, visit the [quickstart guide](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker_quickstart.ipynb) or checkout our [readthedocs](https://jwst-fgs-spelunker.readthedocs.io). Get acquainted with `spelunker` with the following example notebooks:
 
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
 - [TSOS Guidestar Demo](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker-and-tsos.ipynb)
 
+This software is currently under development on [GitHub](https://github.com). To report bugs or to send feature requests, send us an email or [open an issue](https://github.com/GalagaBits/JWST-FGS-Spelunker/issues) on GitHub.
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
 
 ## Acknowledgments
```

### Comparing `spelunker-1.1.8/README.md` & `spelunker-1.1.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -45,47 +45,55 @@
 plt.ylabel('Counts')
 
 ```
 <p align='center'>
     <img src="plots/timeseries.png"  width=100% height=80%>
 </p>
 
-(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). We can even make a plot of the tracked guidestars within this Program ID:
+(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). 
+
+We can even make a plot of the tracked guidestars within this Program ID. Within a selected Program ID, multiple guidestars could be used for each observation. Each star or object comes from the Guide Star Catalog (GSC) and is pre-selected depending on [telescope pointing and suitability of the star](https://jwst-docs.stsci.edu/jwst-observatory-characteristics/jwst-guide-stars). In the generated figure from `spk.guidestar_plot`, the guidestar positions (marked with an X) in the given Program ID are plotted from the *START* to the end of the program. A line (`gs track`) is traced between each guidestar to order each used target overtime.
 
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/):
+
+
+Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/). Here, use `spk.mnemonics` to access engineering telemetry for `SA_ZHAGUPST` as a matplotlib `axes` object:
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
 
-ax = spk.mnemonics_local('GUIDESTAR')
-ax = spk.mnemonics('SA_ZHGAUPST', 60067.84, 60067.9) 
+ax = spk.mnemonics_local('GUIDESTAR') # plots when the JWST tracks onto a new guidestars as a vertical line
+ax = spk.mnemonics('SA_ZHGAUPST', 60067.84, 60067.9) # plots the start and end of high gain antenna movement
+
 ax.plot(spk.fg_time, spk.fg_flux)
 plt.legend(loc=3)
 plt.xlim(60067.84, 60067.9)
 plt.show()
 ```
+
+
 <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/mnemonics.png">
 
 For more information on the tools under `spelunker` and how to get started, visit the [quickstart guide](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker_quickstart.ipynb) or checkout our [readthedocs](https://jwst-fgs-spelunker.readthedocs.io). Get acquainted with `spelunker` with the following example notebooks:
 
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
 - [TSOS Guidestar Demo](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker-and-tsos.ipynb)
 
+This software is currently under development on [GitHub](https://github.com). To report bugs or to send feature requests, send us an email or [open an issue](https://github.com/GalagaBits/JWST-FGS-Spelunker/issues) on GitHub.
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
 
 ## Acknowledgments
```

### Comparing `spelunker-1.1.8/setup.py` & `spelunker-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `spelunker-1.1.8/spelunker.egg-info/PKG-INFO` & `spelunker-1.1.9/spelunker.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spelunker
-Version: 1.1.8
+Version: 1.1.9
 Summary: spelunker: a library to extract guidestar data and observe technical and stellar events
 Home-page: https://github.com/GalagaBits/JWST-FGS-Spelunker
 Author: Derod Deal
 Author-email: dealderod@ufl.edu
 License: MIT
 Keywords: guidestars
 Requires-Python: >=3.10
@@ -68,47 +68,55 @@
 plt.ylabel('Counts')
 
 ```
 <p align='center'>
     <img src="plots/timeseries.png"  width=100% height=80%>
 </p>
 
-(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). We can even make a plot of the tracked guidestars within this Program ID:
+(See below on more information that can be extracted, including fitting 2D gaussians to each FGS integration!). 
+
+We can even make a plot of the tracked guidestars within this Program ID. Within a selected Program ID, multiple guidestars could be used for each observation. Each star or object comes from the Guide Star Catalog (GSC) and is pre-selected depending on [telescope pointing and suitability of the star](https://jwst-docs.stsci.edu/jwst-observatory-characteristics/jwst-guide-stars). In the generated figure from `spk.guidestar_plot`, the guidestar positions (marked with an X) in the given Program ID are plotted from the *START* to the end of the program. A line (`gs track`) is traced between each guidestar to order each used target overtime.
 
 ```python
 spk.guidestar_plot()
 ```
 <p align='center'>
     <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/guidestar_positions.png"  width=80% height=80%>
 </p>
 
-Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/):
+
+
+Mnemonics from JWST technical events can be overplotted on any timeseries, such as high-gain antenna (HGA) movement or to identify if the FGS tracks a new guidestar [if the `jwstuser` package is also installed](https://github.com/spacetelescope/jwstuser/). Here, use `spk.mnemonics` to access engineering telemetry for `SA_ZHAGUPST` as a matplotlib `axes` object:
 
 ```python
 import matplotlib.pyplot as plt
 
 spk.mast_api_token = 'insert a token from auth.MAST here'
 
 fig, ax = plt.subplots(figsize=(12,4),dpi=200)
 
-ax = spk.mnemonics_local('GUIDESTAR')
-ax = spk.mnemonics('SA_ZHGAUPST', 60067.84, 60067.9) 
+ax = spk.mnemonics_local('GUIDESTAR') # plots when the JWST tracks onto a new guidestars as a vertical line
+ax = spk.mnemonics('SA_ZHGAUPST', 60067.84, 60067.9) # plots the start and end of high gain antenna movement
+
 ax.plot(spk.fg_time, spk.fg_flux)
 plt.legend(loc=3)
 plt.xlim(60067.84, 60067.9)
 plt.show()
 ```
+
+
 <img src="https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/plots/mnemonics.png">
 
 For more information on the tools under `spelunker` and how to get started, visit the [quickstart guide](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker_quickstart.ipynb) or checkout our [readthedocs](https://jwst-fgs-spelunker.readthedocs.io). Get acquainted with `spelunker` with the following example notebooks:
 
 - [Guidestar Targets](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/guidestar_targets.ipynb)
 - [Pixel centroid changes and mnemonics](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/examples/pixel_centroid_mnemonics.ipynb)
 - [TSOS Guidestar Demo](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/notebooks/fgs-spelunker-and-tsos.ipynb)
 
+This software is currently under development on [GitHub](https://github.com). To report bugs or to send feature requests, send us an email or [open an issue](https://github.com/GalagaBits/JWST-FGS-Spelunker/issues) on GitHub.
 
 ## Licence and attribution
 
 This project is under the MIT License, which can be viewed [here](https://github.com/GalagaBits/JWST-FGS-Spelunker/blob/main/LICENSE).
 
 ## Acknowledgments
```

### Comparing `spelunker-1.1.8/src/spelunker.py` & `spelunker-1.1.9/src/spelunker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1458,34 +1458,36 @@
         are used, a line is created between the positions of the guidestar.
 
         Returns
         -------
 
             This function returns a matplotlib ``axes`` object of the guidestar plot. Additionally, the function outputs guidestar track plot.
         '''
-        coords = SkyCoord(self.object_properties['ra'], self.object_properties['dec'], unit='deg')
+        filted_properties = self.object_properties[self.object_properties['ra'].astype(bool)]
+
+        coords = SkyCoord(filted_properties['ra'], filted_properties['dec'], unit='deg')
         target = SkyCoord(np.mean(coords.ra),np.mean(coords.dec),unit='deg')
 
         distance = []
         for coord in coords:
             distance.append(np.sqrt(  (target.ra.value - coord.ra.value)**2
                                 + (target.dec.value - coord.dec.value)**2  ))
 
-        fov_radius = np.mean(distance)*u.deg + 2.5*np.std(distance)*u.deg
-        fov_radius = 4 * u.deg if fov_radius > 4 * u.deg else fov_radius
+        fov_radius = 0.5*np.mean(distance)*u.deg + 1*np.std(distance)*u.deg
+        fov_radius = 3 * u.deg if fov_radius > 3 * u.deg else fov_radius
 
         if fov_radius.value == 0: fov_radius = 2*u.deg # from https://github.com/GalagaBits/JWST-FGS-Spelunker/issues/19
 
         fig, ax1 = plt.subplots(figsize=(6,6),dpi=200)
         ax, hdu = plot_finder_image(target, survey='DSS', fov_radius=fov_radius,)
 
         ax1.set_axis_off()
 
-        ax.scatter(coords.ra, coords.dec,  color='darkorange', marker='x', s=100, linewidth=1.5, transform=ax.get_transform('fk5'), label='guidestars')
-        ax.plot(coords.ra, coords.dec,  color='gold', linewidth=1, transform=ax.get_transform('fk5'), label='gs track')
+        ax.scatter(coords.ra, coords.dec,  color='darkorange',marker='$\u25EF$', s=160, linewidth=0.5, alpha=0.4, transform=ax.get_transform('fk5'), label='guidestars')
+        ax.plot(coords.ra, coords.dec,  color='orange', linewidth=1.2, alpha = 0.3, transform=ax.get_transform('fk5'), label='gs track')
         ax.text(coords.ra[0].value, coords.dec[0].value, s='start   ', horizontalalignment='right' , verticalalignment='center', weight='bold', transform=ax.get_transform('fk5'),)
 
         ax.set_title("Guidestar positions — "+str(self.pid))
         ax.legend()
 
         return ax
```

