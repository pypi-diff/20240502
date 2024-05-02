# Comparing `tmp/pren_flawas-0.0.8.tar.gz` & `tmp/pren_flawas-0.0.9.tar.gz`

## Comparing `pren_flawas-0.0.8.tar` & `pren_flawas-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.idea/Python-Shelly-Statistics.iml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/__init__.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/DataPreparation.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/DataSend.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/DataVerify.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/Display.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/Energy.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/Engine.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/__init__.py
--rw-r--r--   0        0        0  5177387 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/pic/Font.ttc
--rw-r--r--   0        0        0   120054 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/pic/background.bmp
--rw-r--r--   0        0        0   160138 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/pic/qrcode.bmp
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/waveshare_epd/epd1in54_V2.py
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/src/PREN_flawas/waveshare_epd/epdconfig.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/tests/testDataPreparation.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/tests/testDataSend.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/tests/testDataVerify.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/tests/testEnergyTest.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/tests/testEngine.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/LICENSE
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pren_flawas-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.idea/.gitignore
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.idea/Python-Shelly-Statistics.iml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/DataPreparation.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/DataSend.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/DataVerify.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/Display.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/Energy.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/Engine.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/__init__.py
+-rw-r--r--   0        0        0  5177387 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/pic/Font.ttc
+-rw-r--r--   0        0        0   120054 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/pic/background.bmp
+-rw-r--r--   0        0        0   160138 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/pic/qrcode.bmp
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/waveshare_epd/epd1in54_V2.py
+-rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/src/PREN_flawas/waveshare_epd/epdconfig.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/tests/testDataPreparation.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/tests/testDataSend.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/tests/testDataVerify.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/tests/testEnergyTest.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/tests/testEngine.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/LICENSE
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 pren_flawas-0.0.9/PKG-INFO
```

### Comparing `pren_flawas-0.0.8/.github/workflows/python-publish.yml` & `pren_flawas-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/DataPreparation.py` & `pren_flawas-0.0.9/src/PREN_flawas/DataPreparation.py`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/DataVerify.py` & `pren_flawas-0.0.9/src/PREN_flawas/DataVerify.py`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/Display.py` & `pren_flawas-0.0.9/src/PREN_flawas/Display.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     epd.Clear(0xFF)
     epd.sleep()
 
 def drawInitialDisplay(epd, background):
     logging.info("Display draw initial display")
     try:
         epd.init(1)
-        updateDisplay(10, 10, 'PREN TEAM 33', backgroundBMP=background)
+        updateDisplay(epd, 10, 10, 'PREN TEAM 33', backgroundBMP=background)
         # self.updateDisplay(10, 30, 'Initialisierung')
-        updateDisplay(10, 80, 'Beanspruchte Zeit', backgroundBMP=background)
+        updateDisplay(epd, 10, 80, 'Beanspruchte Zeit', backgroundBMP=background)
         # self.updateDisplay(10, 100, 'Sekunden')
-        updateDisplay(10, 150, 'Stromverbrauch', backgroundBMP=background)
+        updateDisplay(epd, 10, 150, 'Stromverbrauch', backgroundBMP=background)
         # self.updateDisplay(10, 170, 'kW')
 
     except IOError as e:
         logging.error(e)
 
     except KeyboardInterrupt:
         logging.warning("ctrl + c:")
```

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/Energy.py` & `pren_flawas-0.0.9/src/PREN_flawas/Energy.py`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/Engine.py` & `pren_flawas-0.0.9/src/PREN_flawas/Engine.py`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/pic/Font.ttc` & `pren_flawas-0.0.9/src/PREN_flawas/pic/Font.ttc`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/pic/qrcode.bmp` & `pren_flawas-0.0.9/src/PREN_flawas/pic/qrcode.bmp`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/waveshare_epd/epd1in54_V2.py` & `pren_flawas-0.0.9/src/PREN_flawas/waveshare_epd/epd1in54_V2.py`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/src/PREN_flawas/waveshare_epd/epdconfig.py` & `pren_flawas-0.0.9/src/PREN_flawas/waveshare_epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/tests/testDataPreparation.py` & `pren_flawas-0.0.9/tests/testDataPreparation.py`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/LICENSE` & `pren_flawas-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pren_flawas-0.0.8/pyproject.toml` & `pren_flawas-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/PREN_flawas"]
 
 [project]
 name = "PREN_flawas"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Flavio Waser", email="waserflavio@gmail.com" },
 ]
 description = "A small package used for a project at HSLU Luzern."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pren_flawas-0.0.8/PKG-INFO` & `pren_flawas-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PREN_flawas
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small package used for a project at HSLU Luzern.
 Project-URL: Homepage, https://github.com/flawas/PREN_Module
 Project-URL: Issues, https://github.com/flawas/PREN_Module/issues
 Author-email: Flavio Waser <waserflavio@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

