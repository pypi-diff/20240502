# Comparing `tmp/cheminterface_ppchem-2.0.tar.gz` & `tmp/cheminterface_ppchem-2.1.tar.gz`

## Comparing `cheminterface_ppchem-2.0.tar` & `cheminterface_ppchem-2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/insaturation.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/molecule_image.png
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/preliminary.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/project_CH200.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/setup.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/subgroups.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.github/workflows/requirements.txt
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/misc.xml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/vcs.xml
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/workspace.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Bokeh try.py
--rw-r--r--   0        0        0    53534 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Double plot bokeh.html
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Double plot bokeh.py
--rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Functional groups SMILES
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Functional_group_finder.py
--rw-r--r--   0        0        0    27677 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mass spectro display.html
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mass spectro display.py
--rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mol_display.html
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mol_display.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/callback.html
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/molecule_image.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Cheminterface/Tkinter_interface.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.html
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/copy_file.py
--rw-r--r--   0        0        0    17100 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/molecule_image.png
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/names.txt
--rw-r--r--   0        0        0    19608 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0    49000 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Thomas_return.html
--rw-r--r--   0        0        0    27616 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.html
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/functions.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/random_tests.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/tests.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/data/abundance.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/notebooks/test.ipynb
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/src/ChemInterface_ppchem/ChemInterface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/src/ChemInterface_ppchem/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/LICENSE.txt
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/README.md
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/pyproject.toml
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/PKG-INFO
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/insaturation.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/molecule_image.png
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/preliminary.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/project_CH200.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/setup.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/subgroups.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/.github/workflows/requirements.txt
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/.idea/misc.xml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Bokeh try.py
+-rw-r--r--   0        0        0    53534 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Double plot bokeh.html
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Double plot bokeh.py
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Functional groups SMILES
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Functional_group_finder.py
+-rw-r--r--   0        0        0    27677 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Mass spectro display.html
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Mass spectro display.py
+-rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Mol_display.html
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/Mol_display.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/callback.html
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Bokeh/molecule_image.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Cheminterface/Tkinter_interface.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/Mol_display.html
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/Mol_display.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/Preliminary_v2.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/abundance.txt
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/abundance_simplified.txt
+-rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/copy_file.py
+-rw-r--r--   0        0        0    17100 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/functions.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/molecule_image.png
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/names.txt
+-rw-r--r--   0        0        0    19608 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/THOMAS_IS_BEST/test.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Thomas/Copy_spectrometer.py
+-rw-r--r--   0        0        0    49000 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Thomas/Thomas_return.html
+-rw-r--r--   0        0        0    27616 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Thomas/Thomas_return_pyplot.html
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Thomas/Thomas_return_pyplot.py
+-rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Thomas/functions.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Thomas/random_tests.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/Thomas/tests.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/data/abundance.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/notebooks/test.ipynb
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/src/ChemInterface_ppchem/ChemInterface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/src/ChemInterface_ppchem/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/README.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/pyproject.toml
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.1/PKG-INFO
```

### Comparing `cheminterface_ppchem-2.0/insaturation.py` & `cheminterface_ppchem-2.1/insaturation.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/molecule_image.png` & `cheminterface_ppchem-2.1/molecule_image.png`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/preliminary.py` & `cheminterface_ppchem-2.1/preliminary.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/project_CH200.yml` & `cheminterface_ppchem-2.1/project_CH200.yml`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/subgroups.py` & `cheminterface_ppchem-2.1/subgroups.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/.idea/workspace.xml` & `cheminterface_ppchem-2.1/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Bokeh try.py` & `cheminterface_ppchem-2.1/Bokeh/Bokeh try.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Double plot bokeh.html` & `cheminterface_ppchem-2.1/Bokeh/Double plot bokeh.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Double plot bokeh.py` & `cheminterface_ppchem-2.1/Bokeh/Double plot bokeh.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Functional groups SMILES` & `cheminterface_ppchem-2.1/Bokeh/Functional groups SMILES`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Functional_group_finder.py` & `cheminterface_ppchem-2.1/Bokeh/Functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Mass spectro display.html` & `cheminterface_ppchem-2.1/Bokeh/Mass spectro display.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Mass spectro display.py` & `cheminterface_ppchem-2.1/Bokeh/Mass spectro display.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Mol_display.html` & `cheminterface_ppchem-2.1/Bokeh/Mol_display.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/Mol_display.py` & `cheminterface_ppchem-2.1/Bokeh/Mol_display.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/callback.html` & `cheminterface_ppchem-2.1/Bokeh/callback.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Bokeh/molecule_image.png` & `cheminterface_ppchem-2.1/Bokeh/molecule_image.png`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.html` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/Mol_display.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.py` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/Mol_display.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/Preliminary_v2.py` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/Preliminary_v2.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance.txt` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/abundance.txt`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance_simplified.txt` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/abundance_simplified.txt`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/copy_file.py` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/copy_file.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/functions.py` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/functions.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/molecule_image.png` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/molecule_image.png`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/THOMAS_IS_BEST/test.py` & `cheminterface_ppchem-2.1/THOMAS_IS_BEST/test.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Thomas/Copy_spectrometer.py` & `cheminterface_ppchem-2.1/Thomas/Copy_spectrometer.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Thomas/Thomas_return.html` & `cheminterface_ppchem-2.1/Thomas/Thomas_return.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.html` & `cheminterface_ppchem-2.1/Thomas/Thomas_return_pyplot.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.py` & `cheminterface_ppchem-2.1/Thomas/Thomas_return_pyplot.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Thomas/functions.html` & `cheminterface_ppchem-2.1/Thomas/functions.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/Thomas/tests.py` & `cheminterface_ppchem-2.1/Thomas/tests.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/data/abundance.txt` & `cheminterface_ppchem-2.1/data/abundance.txt`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/src/ChemInterface_ppchem/ChemInterface.py` & `cheminterface_ppchem-2.1/src/ChemInterface_ppchem/ChemInterface.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/LICENSE.txt` & `cheminterface_ppchem-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/README.md` & `cheminterface_ppchem-2.1/README.md`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-2.0/PKG-INFO` & `cheminterface_ppchem-2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,21 @@
 Metadata-Version: 2.3
 Name: ChemInterface_ppchem
-Version: 2.0
+Version: 2.1
 Summary: ...
 Project-URL: Homepage, https://github.com/ThomasCsson/ppchem-project-Christiansson-Gonteri-Humery.git
 Author-email: Thomas Christianson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: Mass spectroscopy,unsaturation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: bzip2==1.0.8
-Requires-Dist: ca-certificates==2024.3.11
-Requires-Dist: libffi==3.4.4
-Requires-Dist: openssl==3.0.13
-Requires-Dist: pip==23.3.1
-Requires-Dist: python==3.10.12
-Requires-Dist: setuptools==68.2.2
-Requires-Dist: sqlite==3.45.3
-Requires-Dist: tk==8.6.12
-Requires-Dist: vc==14.2
-Requires-Dist: vs2015-runtime==14.27.29016
-Requires-Dist: wheel==0.41.2
-Requires-Dist: xz==5.4.6
-Requires-Dist: zlib==1.2.13
 Description-Content-Type: text/markdown
 
 # - ChemInterface package for applied mass spectrometry -
 #### Project in practical programming in chemistry course
 #### EPFL CH-200
 
 This repository provides the user with a package which will display an interactive interface where the user will be able to input the SMILEs of a molecule. The interface will be able to give specific information about the molecule such as its molecular mass, its organic functional groups or its degree of insaturation. The most important part of the package will provide a way to simulate the mass spectrum of the given molecule.
```

