# Comparing `tmp/calc_ultra-1.3.4.tar.gz` & `tmp/calc_ultra-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calc_ultra-1.3.4.tar", last modified: Sat Apr 20 14:13:33 2024, max compression
+gzip compressed data, was "calc_ultra-1.3.5.tar", last modified: Thu May  2 10:12:50 2024, max compression
```

## Comparing `calc_ultra-1.3.4.tar` & `calc_ultra-1.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.601904 calc_ultra-1.3.4/
--rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.4/LICENSE
--rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.4/MANIFEST.in
--rw-r--r--   0 Huatao     (502) staff       (20)     4443 2024-04-20 14:13:33.601584 calc_ultra-1.3.4/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)     3712 2024-04-20 14:13:03.000000 calc_ultra-1.3.4/README.md
--rw-r--r--   0 Huatao     (502) staff       (20)      862 2024-04-20 14:11:37.000000 calc_ultra-1.3.4/pyproject.toml
--rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-04-20 14:13:33.601971 calc_ultra-1.3.4/setup.cfg
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.596156 calc_ultra-1.3.4/src/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-04-20 14:11:29.000000 calc_ultra-1.3.4/src/.DS_Store
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.597346 calc_ultra-1.3.4/src/calc_ultra/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-04-13 13:31:29.000000 calc_ultra-1.3.4/src/calc_ultra/.DS_Store
--rw-r--r--   0 Huatao     (502) staff       (20)      128 2024-02-05 08:04:02.000000 calc_ultra-1.3.4/src/calc_ultra/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)    36559 2024-04-20 14:13:02.000000 calc_ultra-1.3.4/src/calc_ultra/main.py
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.600786 calc_ultra-1.3.4/src/calc_ultra/texts/
--rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.4/src/calc_ultra/texts/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)      546 2024-03-19 08:27:24.000000 calc_ultra-1.3.4/src/calc_ultra/texts/algcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      740 2024-03-06 07:59:13.000000 calc_ultra-1.3.4/src/calc_ultra/texts/derivacalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      761 2024-04-14 10:36:05.000000 calc_ultra-1.3.4/src/calc_ultra/texts/intecalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      531 2024-03-06 07:59:34.000000 calc_ultra-1.3.4/src/calc_ultra/texts/limcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)     1212 2024-04-14 10:36:57.000000 calc_ultra-1.3.4/src/calc_ultra/texts/main_screen.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      232 2024-04-14 10:37:09.000000 calc_ultra-1.3.4/src/calc_ultra/texts/settings.txt
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-04-20 14:13:33.601173 calc_ultra-1.3.4/src/calc_ultra.egg-info/
--rw-r--r--   0 Huatao     (502) staff       (20)     4443 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)      562 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/SOURCES.txt
--rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/dependency_links.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       71 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/requires.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-04-20 14:13:33.000000 calc_ultra-1.3.4/src/calc_ultra.egg-info/top_level.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.463678 calc_ultra-1.3.5/
+-rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.5/LICENSE
+-rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.5/MANIFEST.in
+-rw-r--r--   0 Huatao     (502) staff       (20)     4331 2024-05-02 10:12:50.463468 calc_ultra-1.3.5/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)     3562 2024-05-02 06:15:42.000000 calc_ultra-1.3.5/README.md
+-rw-r--r--   0 Huatao     (502) staff       (20)      892 2024-05-02 06:00:00.000000 calc_ultra-1.3.5/pyproject.toml
+-rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-05-02 10:12:50.463726 calc_ultra-1.3.5/setup.cfg
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.459610 calc_ultra-1.3.5/src/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-02 10:10:35.000000 calc_ultra-1.3.5/src/.DS_Store
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.460410 calc_ultra-1.3.5/src/calc_ultra/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-04-28 11:10:07.000000 calc_ultra-1.3.5/src/calc_ultra/.DS_Store
+-rw-r--r--   0 Huatao     (502) staff       (20)      128 2024-02-05 08:04:02.000000 calc_ultra-1.3.5/src/calc_ultra/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)    42581 2024-05-02 10:00:41.000000 calc_ultra-1.3.5/src/calc_ultra/main.py
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.462792 calc_ultra-1.3.5/src/calc_ultra/texts/
+-rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.5/src/calc_ultra/texts/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)      546 2024-03-19 08:27:24.000000 calc_ultra-1.3.5/src/calc_ultra/texts/algcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      740 2024-03-06 07:59:13.000000 calc_ultra-1.3.5/src/calc_ultra/texts/derivacalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      761 2024-04-14 10:36:05.000000 calc_ultra-1.3.5/src/calc_ultra/texts/intecalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      531 2024-03-06 07:59:34.000000 calc_ultra-1.3.5/src/calc_ultra/texts/limcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      706 2024-05-01 04:38:23.000000 calc_ultra-1.3.5/src/calc_ultra/texts/main_screen.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      232 2024-04-14 10:37:09.000000 calc_ultra-1.3.5/src/calc_ultra/texts/settings.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-02 10:12:50.463212 calc_ultra-1.3.5/src/calc_ultra.egg-info/
+-rw-r--r--   0 Huatao     (502) staff       (20)     4331 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)      562 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/SOURCES.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/dependency_links.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       94 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/requires.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-05-02 10:12:50.000000 calc_ultra-1.3.5/src/calc_ultra.egg-info/top_level.txt
```

### Comparing `calc_ultra-1.3.4/LICENSE` & `calc_ultra-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.4/PKG-INFO` & `calc_ultra-1.3.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,105 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.4
+Version: 1.3.5
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sympy>=1.12
 Requires-Dist: numpy>=1.26.2
-Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: rich>=13.7.1
-Requires-Dist: scipy>=1.12.0
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: prompt_toolkit>=3.0.43
 
 # calc-ultra
 
-[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.4-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.5-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
 
 > **Calculus made easy**
 
-(Turn on dark mode for a better aesthetic)
+(Turn on dark mode for a better aesthetic) 📲
 
-The Calc-Ultra calculus calculator, but as a module!
-
-- Little Python background knowledge is needed!
+Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
 
 Supports:
 
 - Derivatives
 - Partials
 - Implicit differentiation
+- Limits
 - Antiderivatives
 - Definite integrals
 - Improper integrals
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
-## Note
+## Chinese version
 
-This is the module package of the Calc-Ultra calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
+Want to check out the Chinese version? Visit <https://github.com/sudoer-Huatao/calc_ultra-chinese>! 🇨🇳
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
-Command line: `pip3 install calc-ultra`.
-Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
+Use the following command to download Calc-Ultra (pip should be installed):
+
+`pip3 install calc-ultra`
+
+Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra".
 
-To run the calculator, import Calc-ULTRA as `calc_ultra` like so:
+Import Calc-Ultra like so to use:
 
 `from calc_ultra import main`
 
-Make sure you have the latest version installed. To update calc-ultra, run `pip3 install --upgrade calc-ultra`.
+Please make sure you have the latest version installed. To update calc-ultra, run the following command:
 
-## Requirements
+`pip3 install --upgrade calc-ultra`
 
-This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built into most Python IDEs.
+## Requirements
 
-## Warnings
+Calc-Ultra requires these modules/packages:
 
-### Function limitations
+- `sympy`
+- `numpy`
+- `matplotlib`
+- `scipy`
+- `rich`
+- `prompt-toolkit`
 
-Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions is also limited due to SymPy limitations. While some composed functions work, others don't. 😟
+If you do not have them installed, there is no need to worry. The modules needed should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
 
 ## Test PYPI
 
-Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>.
+Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>. 💾
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
-A general thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️
-And... a SPECIAL THANK-YOU to @Haobot for troubleshooting and feedback! 👍❤️
+A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
+The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
+
+- @Haobot for troubleshooting and feedback!
+- Fanbo for feedback and ideas for improvement!
 
-This program was made using SymPy and Scipy for calculation and Matplotlib and NumPy for graphing.
+This program was made using `sympy` for calculation and `numpy`, `scipy`, and `matplotlib` for graphing.
 
-## Gallery
+## Gallery (Demos)
 
 DerivaCalc derivative with graph demo:
 ![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
 ![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
```

### Comparing `calc_ultra-1.3.4/README.md` & `calc_ultra-1.3.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 # calc-ultra
 
-[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.4-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.5-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
 
 > **Calculus made easy**
 
-(Turn on dark mode for a better aesthetic)
+(Turn on dark mode for a better aesthetic) 📲
 
-The Calc-Ultra calculus calculator, but as a module!
-
-- Little Python background knowledge is needed!
+Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
 
 Supports:
 
 - Derivatives
 - Partials
 - Implicit differentiation
+- Limits
 - Antiderivatives
 - Definite integrals
 - Improper integrals
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
-## Note
+## Chinese version
 
-This is the module package of the Calc-Ultra calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
+Want to check out the Chinese version? Visit <https://github.com/sudoer-Huatao/calc_ultra-chinese>! 🇨🇳
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
-Command line: `pip3 install calc-ultra`.
-Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
+Use the following command to download Calc-Ultra (pip should be installed):
+
+`pip3 install calc-ultra`
+
+Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra".
 
-To run the calculator, import Calc-ULTRA as `calc_ultra` like so:
+Import Calc-Ultra like so to use:
 
 `from calc_ultra import main`
 
-Make sure you have the latest version installed. To update calc-ultra, run `pip3 install --upgrade calc-ultra`.
+Please make sure you have the latest version installed. To update calc-ultra, run the following command:
 
-## Requirements
+`pip3 install --upgrade calc-ultra`
 
-This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built into most Python IDEs.
+## Requirements
 
-## Warnings
+Calc-Ultra requires these modules/packages:
 
-### Function limitations
+- `sympy`
+- `numpy`
+- `matplotlib`
+- `scipy`
+- `rich`
+- `prompt-toolkit`
 
-Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions is also limited due to SymPy limitations. While some composed functions work, others don't. 😟
+If you do not have them installed, there is no need to worry. The modules needed should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
 
 ## Test PYPI
 
-Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>.
+Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>. 💾
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
-A general thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️
-And... a SPECIAL THANK-YOU to @Haobot for troubleshooting and feedback! 👍❤️
+A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
+The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
+
+- @Haobot for troubleshooting and feedback!
+- Fanbo for feedback and ideas for improvement!
 
-This program was made using SymPy and Scipy for calculation and Matplotlib and NumPy for graphing.
+This program was made using `sympy` for calculation and `numpy`, `scipy`, and `matplotlib` for graphing.
 
-## Gallery
+## Gallery (Demos)
 
 DerivaCalc derivative with graph demo:
 ![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
 ![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
```

### Comparing `calc_ultra-1.3.4/pyproject.toml` & `calc_ultra-1.3.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 build-backend = "setuptools.build_meta"
 
 [wheel]
 supported_platforms = ["macos"]
 
 [project]
 name = "calc_ultra"
-version = "1.3.4"
+version = "1.3.5"
 dependencies = [
   "sympy >= 1.12",
   "numpy >= 1.26.2",
-  "matplotlib >= 3.8.3",
+  "matplotlib >= 3.8.4",
   "rich >= 13.7.1",
-  "scipy >= 1.12.0"
+  "scipy >= 1.13.0",
+  "prompt_toolkit >= 3.0.43"
 ]
 requires-python = ">=3.8"
 authors = [
   { name="Huatao", email="huatao.xue@outlook.com" },
 ]
 maintainers = [
   { name="Huatao", email="huatao.xue@outlook.com "}
```

### Comparing `calc_ultra-1.3.4/src/.DS_Store` & `calc_ultra-1.3.5/src/.DS_Store`

 * *Files 22% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 00000230: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
 00000240: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00000250: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
 00000260: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00000270: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 00000280: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 00000290: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-000002a0: 1018 7b7b 3431 362c 2033 3339 7d2c 207b  ..{{416, 339}, {
-000002b0: 3835 352c 2034 3339 7d7d 0908 1523 2f3b  855, 439}}...#/;
+000002a0: 1018 7b7b 3339 352c 2034 3734 7d2c 207b  ..{{395, 474}, {
+000002b0: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
 000002c0: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
 000002d0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 000002e0: 0000 0000 0000 008b 0000 000a 0063 0061  .............c.a
 000002f0: 006c 0063 005f 0075 006c 0074 0072 0061  .l.c._.u.l.t.r.a
 00000300: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.4/src/calc_ultra/.DS_Store` & `calc_ultra-1.3.5/src/calc_ultra/.DS_Store`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 00000120: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00000130: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00000140: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00000150: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000160: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000170: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000180: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000190: 7208 0908 095f 1018 7b7b 3438 302c 2032  r...._..{{480, 2
-000001a0: 3636 7d2c 207b 3932 302c 2034 3336 7d7d  66}, {920, 436}}
+00000190: 7208 0908 095f 1018 7b7b 3432 392c 2033  r...._..{{429, 3
+000001a0: 3432 7d2c 207b 3835 352c 2034 3339 7d7d  42}, {855, 439}}
 000001b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 000001c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 000001e0: 0005 0074 0065 0078 0074 0073 7653 726e  ...t.e.x.t.svSrn
 000001f0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.4/src/calc_ultra/main.py` & `calc_ultra-1.3.5/src/calc_ultra/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+###########
+# Imports #
+###########
+
 from sympy.core.numbers import pi, E, oo
 from math import floor, ceil
-import math as mt
-from scipy.special import gamma, polygamma, erf
+from scipy.special import polygamma, gammainc, gammaincc, erf, erfc
+import scipy.special as ss
 from rich import print
 from rich.progress import (
     Progress,
     SpinnerColumn,
     BarColumn,
     MofNCompleteColumn,
     TimeElapsedColumn,
     TextColumn,
 )
+from prompt_toolkit import prompt
+from prompt_toolkit.key_binding import KeyBindings
 from numpy import (
     linspace,
     exp,
     log,
     sqrt,
     abs,
     sin,
@@ -29,174 +35,298 @@
     arcsinh,
     arccosh,
     arctanh,
     array,
     cross,
 )
 from numpy.linalg import norm, det
-import numpy as np
-
-# Sympy uses symbolic Pi and e, which cannot be graphed by matplotlib
-# so later np.pi np.e are explicitly used instead.
 from sympy import (
     diff,
     idiff,
     Integral,
     integrate,
     limit,
     solve,
     linsolve,
     pprint,
     simplify,
     symbols,
+    gamma,
+    lowergamma,
+    uppergamma,
+    zeta,
 )
 import matplotlib.pyplot as plt
-import datetime, logging, random, os, time, warnings
+import datetime, logging, random, readline, os, time, warnings
 
 
-# Disable auto Python warnings
+###########
+# Presets #
+###########
 
 warnings.filterwarnings("ignore")
 
+readline.parse_and_bind("tab: complete")
+
+x, y, z = symbols("x, y, z")
+
+history = []  # Stores calculation history
+
+input = prompt
+
+key_bindings = KeyBindings()
+
+idx = 1
+
+expr_replace = [
+    ("^", "**"),
+    ("E1**", "exp"),
+    ("E1xp", "exp"),
+    ("E1rf", "erf"),
+    ("pE1r", "per"),
+    ("wE1r", "wer"),
+    ("ln", "log"),
+    ("arc", "a"),
+    ("abs", "Abs"),
+    ("pi", "3.141592653589793"),
+    ("E1", "2.718281828459045"),
+]
+
+graph_replace = [
+    ("asin", "arcsin"),
+    ("acos", "arccos"),
+    ("atan", "arctan"),
+    ("asinh", "arcsinh"),
+    ("acosh", "arccosh"),
+    ("atanh", "arctanh"),
+    ("csc", "1/sin"),
+    ("sec", "1/cos"),
+    ("cot", "1/tan"),
+    ("Abs", "fabs"),
+    ("gamma", "ss.gamma"),
+    ("polyss.gamma", "polygamma"),
+    ("lowergamma", "gammainc"),
+    ("uppergamma", "gammaincc"),
+]
+
+
+# Custom up/down key bindings
+
+
+@key_bindings.add("up")
+def _(event):
+    global idx
+
+    if idx != -1:
+        idx -= 1
+        buffer = event.app.current_buffer
+        buffer.text = history[idx]
+        buffer.cursor_position = len(buffer.text)
+        idx = idx % len(history)
+    else:
+        idx = 0
+        buffer = event.app.current_buffer
+        buffer.text = history[idx]
+        buffer.cursor_position = len(buffer.text)
+
+
+@key_bindings.add("down")
+def _(event):
+    global idx
+
+    if idx != len(history):
+        idx += 1
+        idx = idx % len(history)
+        buffer = event.app.current_buffer
+        buffer.text = history[idx]
+        buffer.cursor_position = len(buffer.text)
+
+    else:
+        idx = len(history) - 1
+        buffer = event.app.current_buffer
+        buffer.text = history[idx]
+        buffer.cursor_position = len(buffer.text)
+
+
+#####################
+# Calculation funcs #
+#####################
+
 
 def simp():
     print(
         '\n[bold bright_green](Current Screen: Simple Calculation Screen)[/bold bright_green]\n("q" to quit)\nEnter any expression to start:\n'
     )
 
     while True:
-        expr = input()
+        expr = input(key_bindings=key_bindings)
 
         try:
             if expr != "q":
                 # Easy to exit unlike VIM ;)
-                result = eval(trig_rep(expr))
-                print("\n[bright_yellow]Result: [/bright_yellow]", end="")
+                result = eval(replace_graph(expr))
+                history.append(str(result))
+                print("\n[bright_yellow]Result:[/bright_yellow]", end="")
                 pprint(result)
                 print()
 
             else:
                 break
 
         except:
             print()
-            logging.error(f'Could not parse: "{expr}"\n')
+            logging.error(f'Could not parse: "{expr}".\n')
 
 
 def derive(function: str, order: str):
+    """Calculates the derivative of a function.
+
+    Takes a function and an order of differentiation and
+    returns the derivative of the function with the given order.
+    Graph option available.
+    """
+
     calc = replace_expr(function)
 
-    if check_order(order) is True:
-        global df
-        df = diff(calc, x, order)
+    check_order(order)
 
-        print(
-            f"\nDerivative of [bright_magenta]{trig_rep(function)}[/bright_magenta] with order {order} is:\n"
-        )
-        print_expr(df)
+    global df
+    df = diff(calc, x, order)
 
-        check_simp(df)
+    print(
+        f"\nDerivative of [bright_magenta]{replace_graph(function)}[/bright_magenta] with order {order} is:\n"
+    )
+    print_expr(df)
 
-        df = trig_rep(str(df))
+    df = replace_expr(str(df))
+    check_simp(df)
+    history.append(df)
 
-        print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
-        show = input("(Exit the graph window when you are finished to continue) ")
+    df = replace_graph(df)
 
-        if show == "y":
-            try:
-                print()
-                with Progress(
-                    SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
-                    TextColumn("[bright_yellow]Loading graph...[/bright_yellow]"),
-                    BarColumn(),
-                    TimeElapsedColumn(),
-                    transient=False,
-                ) as progress:
-                    task = progress.add_task("", total=100)
-
-                    while not progress.finished:
-                        progress.update(task, advance=2)
-                        time.sleep(random.randint(2, 5) / 1000)
-
-                x_array = linspace(-50, 50, 200000)
-
-                def f(x):
-                    return eval(trig_rep(calc))
-
-                def dif(x):
-                    return eval(df)
-
-                title = "Function (red) and derivative (blue)"
-                plt.title(title)
-                plt.xlabel("x", weight="bold")
-                plt.ylabel("y", rotation=0, weight="bold")
-                plt.plot(x_array, f(x_array), color="red", label="Function")
-                plt.plot(x_array, dif(x_array), color="blue", label="Derivative")
-                plt.axis([-7.5, 7.5, -7.5, 7.5])
-                plt.legend(loc="lower left")
-                plt.grid()
-                plt.show()
+    print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
+    show = input("(Exit the graph window when you are finished to continue) ")
 
-                print("\nExited graph.\n")
+    if show == "y":
+        try:
+            print()
+            with Progress(
+                SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
+                TextColumn("[bright_yellow]Loading graph...[/bright_yellow]"),
+                BarColumn(),
+                TimeElapsedColumn(),
+                transient=False,
+            ) as progress:
+                task = progress.add_task("", total=100)
 
-            except:
-                plt.close()
-                print("\n")
-                logging.warning("Could not graph function.")
-                print("\nExited graph.")
+                while not progress.finished:
+                    progress.update(task, advance=2)
+                    time.sleep(random.randint(2, 5) / 1000)
+
+            x_arr = linspace(-100, 100, 200000)
+
+            def f(x: array):
+                return eval(replace_graph(calc))
+
+            def dif(x: array):
+                return eval(df)
+
+            title = "Function (red) and derivative (blue)"
+            plt.title(title)
+            plt.xlabel("x", weight="bold")
+            plt.ylabel("y", rotation=0, weight="bold")
+            plt.plot(x_arr, f(x_arr), color="red", label="Function")
+            plt.plot(x_arr, dif(x_arr), color="blue", label="Derivative")
+            plt.axis([-7.5, 7.5, -7.5, 7.5])
+            plt.legend(loc="lower left")
+            plt.grid()
+            plt.show()
+
+            print("\nExited graph.\n")
+
+        except:
+            plt.close()
+            print("\n")
+            logging.warning("Could not graph function.")
+            print("\nExited graph.")
 
 
 def partial_derive(function: str, var: str, order: str):
+    """Calculates the partial derivative of a function.
+
+    Takes a function, a variable, and an order of differentiation and
+    returns the partial derivative of the function in respect
+    to the variable with the order.
+    """
+
     calc = replace_expr(function)
 
-    if check_order(order) is True:
-        df = diff(calc, var, order)
+    check_order(order)
 
-        print(
-            f"\nPartial derivative of [bright_magenta]{trig_rep(function)}[/bright_magenta] in respect to {var} of order {order} is:\n"
-        )
-        print_expr(df)
+    df = diff(calc, var, order)
+
+    print(
+        f"\nPartial derivative of [bright_magenta]{replace_graph(function)}[/bright_magenta] in respect to {var} of order {order} is:\n"
+    )
+    print_expr(df)
 
-        check_simp(df)
+    df = replace_expr(str(df))
+    check_simp(df)
+    history.append(df)
 
 
 def implicit_derive(circ: str, order: str):
+    """Calculates the implicit derivative of an equation.
+
+    Takes an equation and an order of differentiation and
+    returns the implicit derivative of an equation with the given order.
+    """
+
     calc = replace_expr(circ)
     left = eval(calc[: calc.find("=")])
     right = eval(calc[calc.find("=") + 1 :])
 
-    if check_order(order) is True:
-        df = idiff(left - right, y, x, order)
+    check_order(order)
 
-        print(
-            f"\nDerivative of [bright_magenta]{circ}[/bright_magenta] with order {order} is:\n"
-        )
-        print_expr(df)
+    df = idiff(left - right, y, x, order)
 
-        if str(simplify(df, evaluate=False)) != str(df):
-            print("\nSimplify/rewrite:\n")
-            print_expr(simplify(df, evaluate=False))
+    print(
+        f"\nDerivative of [bright_magenta]{circ}[/bright_magenta] with order {order} is:\n"
+    )
+    print_expr(df)
+
+    df = replace_expr(str(df))
+    check_simp(df)
+    history.append(df)
 
 
 def antiderive(function: str):
+    """Calculates the antiderivative of a function.
+
+    Takes a function and returns the antiderivative of the function.
+    Graph option available.
+    """
+
     calc = replace_expr(function)
     F = Integral(calc, x).doit()
 
     if "Integral" in str(F):
         logging.warning("Cannot compute integral.\n")
         return ""
 
     print(
-        f"\nAntiderivative of [bright_magenta]{trig_rep(function)}[/bright_magenta] is:\n"
+        f"\nAntiderivative of [bright_magenta]{replace_graph(function)}[/bright_magenta] is:\n"
     )
     print_expr(F)
 
+    F = replace_expr(str(F))
     check_simp(F)
+    history.append(F)
 
-    F = trig_rep(str(F))
+    F = replace_graph(F)
 
     print("\n[bold]Don't forget to add a constant![/bold]\n")
 
     print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
     show = input("(Exit the graph window when you are finished to continue) ")
 
     if show == "y":
@@ -211,28 +341,28 @@
             ) as progress:
                 task = progress.add_task("", total=100)
 
                 while not progress.finished:
                     progress.update(task, advance=2)
                     time.sleep(random.randint(2, 5) / 1000)
 
-            x_array = linspace(-100, 100, 200000)
+            x_arr = linspace(-100, 100, 200000)
 
-            def f(x):
-                return eval(trig_rep(calc))
+            def f(x: array):
+                return eval(replace_graph(calc))
 
-            def af(x):
+            def af(x: array):
                 return eval(F)
 
             title = "Function (red) and antiderivative (blue, C = 0)"
             plt.title(title)
             plt.xlabel("x", weight="bold")
             plt.ylabel("y", rotation=0, weight="bold")
-            plt.plot(x_array, f(x_array), color="red", label="Function")
-            plt.plot(x_array, af(x_array), color="blue", label="Antiderivative")
+            plt.plot(x_arr, f(x_arr), color="red", label="Function")
+            plt.plot(x_arr, af(x_arr), color="blue", label="Antiderivative")
             plt.axis([-7.5, 7.5, -7.5, 7.5])
             plt.legend(loc="lower left")
 
             plt.grid()
             plt.show()
 
             print("\nExited graph.\n")
@@ -241,47 +371,56 @@
             plt.close()
             print("\n")
             logging.warning("Could not graph function.")
             print("\nExited graph.\n")
 
 
 def def_int(function: str, low: str, up: str):
-    x = symbols("x")
+    """Calculates the definite integral of a function.
+
+    Takes a function and a lower and upper bound and
+    returns the definite integral from the lower bound to
+    the upper bound of the function.
+    Graph option available.
+    """
+
     calc = replace_expr(function)
 
-    check_bound(low)
+    check_num(low)
 
-    clow = eval(replace_expr(low))
+    calc_low = eval(replace_expr(low))
 
-    check_bound(up)
+    check_num(up)
 
-    cup = eval(replace_expr(up))
+    calc_up = eval(replace_expr(up))
 
-    result = integrate(calc, (x, clow, cup))
+    result = integrate(calc, (x, calc_low, calc_up))
 
-    gup = eval(replace_bound(str(cup)))
-    glow = eval(replace_bound(str(clow)))
+    graph_up = eval(replace_expr(str(calc_up)))
+    graph_low = eval(replace_expr(str(calc_low)))
 
-    num_result = integrate(calc, (x, glow, gup)).evalf()
+    num_result = integrate(calc, (x, graph_low, graph_up)).evalf()
     # Composite functions usually do not have primitive antiderivatives
     # so calc-ultra is equipped with both symbolic and numerical answers.
 
     if (
         (str(result) == "nan")
-        or ("I" in str(result))
+        or ("i" in str(result))
         and ("Integral" not in str(result))
     ):
         logging.warning("Cannot compute integral because integral does not converge.")
         return ""
 
     if "Integral" not in str(result):
         print(
-            f"\nCalculated integral of [bright_magenta]{trig_rep(function)}[/bright_magenta] from {low} to {up}. Final area is:\n"
+            f"\nCalculated integral of [bright_magenta]{replace_graph(function)}[/bright_magenta] from {low} to {up}. Final area is:\n"
         )
         print_expr(result)
+        result = replace_expr(str(result))
+        history.append(result)
 
     else:
         print("\nCannot express result symbolically.")
 
     nprint("\nNumeral evaluation/approximation:\n")
     print_expr(num_result)
 
@@ -301,73 +440,86 @@
             ) as progress:
                 task = progress.add_task("", total=100)
 
                 while not progress.finished:
                     progress.update(task, advance=2)
                     time.sleep(random.randint(2, 5) / 1000)
 
-            x_array = linspace(-100, 100, 200000)
+            x_arr = linspace(-100, 100, 200000)
 
             if "log" in function:
-                x_array = linspace(
-                    0.00000001,
+                x_arr = linspace(
+                    0.0001,
                     100,
                     200000,
                 )
 
+            # The factorial is just the gamma function shifted one unit left
+            # Of course, the factorial is only defined for x >= 0
+
             if "factorial" in function:
-                x_array = linspace(
+                x_arr = linspace(
                     0,
                     100,
                     200000,
                 )
 
-            # This is just the gamma function shifted one unit left
-            # Of course, the factorial is only defined for x >= 0
-
-            def f(x):
-                return eval(trig_rep(calc))
+            def f(x: array):
+                return eval(replace_graph(calc))
 
             title = "Shaded area beneath function"
             plt.title(title)
             plt.xlabel("x", weight="bold")
             plt.ylabel("y", rotation=0, weight="bold")
-            plt.plot(x_array, f(x_array), color="red", label="Function")
+            plt.plot(x_arr, f(x_arr), color="red", label="Function")
 
             plt.fill_between(
-                x_array,
-                f(x_array),
-                where=[(x_array > clow) and (x_array < cup) for x_array in x_array],
+                x_arr,
+                f(x_arr),
+                where=[(x_arr > calc_low) and (x_arr < calc_up) for x_arr in x_arr],
                 color="blue",
             )
 
             try:
                 if graph_option == "f":
                     plt.axis([-7.5, 7.5, -7.5, 7.5])
 
                 elif graph_option == "a":
                     # Adjusted graph view is sometimes better for
                     # large graphs with large bounds.
-                    if (float(f(glow)) != 0) and (float(f(gup)) != 0):
+                    if (float(f(graph_low)) != 0) and (float(f(graph_up)) != 0):
                         plt.axis(
                             [
-                                glow - 5,
-                                gup + 5,
-                                float(f(round(glow)))
-                                - (float(f(round(glow))) + float(f(round(gup)))) / 2
+                                graph_low - 5,
+                                graph_up + 5,
+                                float(f(round(graph_low)))
+                                - (
+                                    float(f(round(graph_low)))
+                                    + float(f(round(graph_up)))
+                                )
+                                / 2
                                 - 1,
-                                float(f(round(gup)))
-                                + (float(f(round(glow))) + float(f(round(gup)))) / 2
+                                float(f(round(graph_up)))
+                                + (
+                                    float(f(round(graph_low)))
+                                    + float(f(round(graph_up)))
+                                )
+                                / 2
                                 + 1,
                             ]
                         )
 
-                    elif (float(f(glow)) == 0) or (float(f(gup)) == 0):
+                    elif (float(f(graph_low)) == 0) or (float(f(graph_up)) == 0):
                         plt.axis(
-                            [glow - 5, gup + 5, -(gup - glow) / 2, (gup + glow) / 2]
+                            [
+                                graph_low - 5,
+                                graph_up + 5,
+                                -(graph_up - graph_low) / 2,
+                                (graph_up + graph_low) / 2,
+                            ]
                         )
 
             except:
                 plt.axis([-7.5, 7.5, -7.5, 7.5])
 
             plt.legend(loc="lower left")
             plt.grid()
@@ -382,165 +534,206 @@
             return "\nExited graph.\n"
 
     else:
         return "\n[bright_yellow]Exiting Definite Integral Screen ... ... ...[/bright_yellow]\n"
 
 
 def improp_int(function: str, low: str, up: str):
+    """Calculates the improper integral of a function.
+
+    Takes a function and a lower and upper bound (can be inf)
+    and returns the improper integral from the lower bound to
+    the upper bound of the function. Uses Cauchy principal value
+    for integrals with infinite bounds and standard integration
+    for integrals with singularities.
+    """
+
     function = replace_expr(function)
 
-    check_bound(low)
+    check_num(low)
 
-    clow = eval(replace_expr(low))
+    calc_low = eval(replace_expr(low))
 
-    check_bound(up)
+    check_num(up)
 
-    cup = eval(replace_expr(up))
+    calc_up = eval(replace_expr(up))
 
     try:
         improper_area = Integral(
-            function, (x, clow, cup)
+            function, (x, calc_low, calc_up)
         ).principal_value()  # Cauchy Principal Value
 
-        if "Integral" not in str(improper_area):
-            print(
-                f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
-            )
-            print_expr(improper_area)
+        if "Integral" in str(improper_area):
+            logging.warning("Cannot compute improper integral.\n")
+            return ""
 
-        else:
-            print("Cannot compute improper integral.")
+        print(
+            f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
+        )
+        print_expr(improper_area)
+        improper_area = replace_expr(str(improper_area))
+        history.append(improper_area)
 
     except ValueError:
-        improper_area = integrate(function, (x, clow, cup))
+        improper_area = integrate(function, (x, calc_low, calc_up))
 
-        if "Integral" not in str(improper_area):
-            print(
-                f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
-            )
-            print_expr(improper_area)
+        if "Integral" in str(improper_area):
+            logging.warning("Cannot compute improper integral.\n")
+            return ""
 
-        else:
-            print("Cannot compute improper integral.")
+        print(
+            f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
+        )
+        print_expr(improper_area)
+        improper_area = replace_expr(str(improper_area))
+        history.append(improper_area)
 
     print()
 
 
 def double_int(function: str, out_low: str, out_up: str, in_low: str, in_up: str):
+    """Calculates the double integral of a function over region R.
+
+    Takes a function and outer lower and upper and
+    inner lower and upper bounds (that define region R)
+    and returns the integral of the function over R.
+    """
+
     function = replace_expr(function)
 
-    check_bound(out_low)
+    check_num(out_low)
 
     out_low = eval(replace_expr(out_low))
 
-    check_bound(out_up)
+    check_num(out_up)
 
     out_up = eval(replace_expr(out_up))
 
     in_low = eval(replace_expr(in_low))
 
     in_up = eval(replace_expr(in_up))
 
-    out_up = eval(replace_bound(str(out_up)))
-    out_low = eval(replace_bound(str(out_low)))
-    in_up = eval(replace_bound(str(in_up)))
-    in_low = eval(replace_bound(str(in_low)))
+    out_up = eval(replace_expr(str(out_up)))
+    out_low = eval(replace_expr(str(out_low)))
+    in_up = eval(replace_expr(str(in_up)))
+    in_low = eval(replace_expr(str(in_low)))
 
     result = integrate(function, (y, in_low, in_up), (x, out_low, out_up))
 
     if "Integral" in str(result):
         logging.warning("Cannot compute integral.\n")
         return ""
 
     print(
         f"\nDouble integral of [bright_magenta]{function}[/bright_magenta] with inner bounds [bright_cyan]{in_low}[/bright_cyan] and [bright_cyan]{in_up}[/bright_cyan] and outer bounds {out_low} and {out_up} is:\n"
     )
     print_expr(result)
+    result = replace_expr(str(result))
+    history.append(result)
     print("")
 
-    check_simp(result)
 
+def lim(function: str, value: str):
+    """Calculates limit of a function at a value.
+
+    Takes a function and a value and
+    returns the limit of the function at the point.
+    """
 
-def lim(expr: str, value: str):
-    expr = replace_expr(expr)
+    function = replace_expr(function)
 
-    check_bound(value)
+    check_num(value)
 
-    value = float(eval(replace_bound(value)))
+    value = float(eval(replace_expr(value)))
 
-    l = limit(expr, x, value)
+    l = limit(function, x, value)
 
     if "Limit" in str(l):
         logging.warning("Cannot compute limit.")
         return ""
 
-    if limit(expr, x, value, "+") != limit(expr, x, value, "-"):
-        print(
-            "\nThe limit does not exist (i.e., the limit approaching from the right does not equal the limit approaching from the left)."
+    if limit(function, x, value, "+") != limit(function, x, value, "-"):
+        logging.warning(
+            "\nThe limit does not exist (the limit approaching from the right does not equal the limit approaching from the left)."
         )
         print(
-            "Use the one-side limit calculation of LimCalc to calculate the limit at one side.\n"
+            "[bright_red]Use one-side limit calculation to calculate the limit from one direction.[/bright_red]\n"
         )
+        return ""
+
+    print(
+        f"\nLimit of [bright_magenta]{function}[/bright_magenta] as x approaches {value} is:\n"
+    )
+    print_expr(l)
+    l = replace_expr(str(l))
+    history.append(l)
 
-    else:
-        print(
-            f"\nLimit of [bright_magenta]{expr}[/bright_magenta] as x approaches {value} is:\n"
-        )
-        print_expr(l)
-        check_simp(l)
 
+def side_lim(function: str, value: str, direction: str):
+    """Calculates limit of a function at a value.
 
-def side_lim(expr: str, value: str, direction: str):
-    expr = replace_expr(expr)
+    Takes a function and a value and
+    returns the limit of the function at the point.
+    """
+    function = replace_expr(function)
 
-    check_bound(value)
+    check_num(value)
 
-    value = float(eval(replace_bound(value)))
+    value = float(eval(replace_expr(value)))
 
     if direction == "left" or direction == "Left":
         direction_sign = "-"
 
     elif direction == "right" or direction == "Right":
         direction_sign = "+"
 
     else:
         print()
-        logging.error("\nTypeError: Direction is neither right or left.")
+        logging.error("\nDirection is neither right or left.")
         return ""
 
-    l = limit(expr, x, value, dir=direction_sign)
+    l = limit(function, x, value, dir=direction_sign)
 
     if "Limit" in str(l):
         logging.warning("\nCannot compute limit.")
         return ""
 
     print(
-        f"\nLimit of [bright_magenta]{expr}[/bright_magenta] as x approaches {value} from the [bright_cyan]{direction}[/bright_cyan] is:\n"
+        f"\nLimit of [bright_magenta]{function}[/bright_magenta] as x approaches {value} from the [bright_cyan]{direction}[/bright_cyan] is:\n"
     )
     print_expr(l)
+    l = replace_expr(str(l))
+    history.append(l)
+
+
+def eq_solve(mode: str):
+    """Solves an/a set of equation(s).
 
+    Takes a mode to determine the number of equations
+    to solve (1 to 3) and returns the values of the variables.
+    """
 
-def eq_solve(mode: int):
     eq_list = []
 
-    if mode == 1:
+    if mode == "1":
         eq1 = input("\nEnter equation: ")
         left = eval(eq1[: eq1.find("=")])
         right = eval(eq1[eq1.find("=") + 1 :])
         eq_set = solve(left - right)
         if len(eq_set) == 0:
             print()
-            logging.error("UnknownError: Cannot solve equation")
+            logging.error("Cannot solve equation")
         else:
             print("\nx:\n")
             for i in range(0, len(eq_set)):
                 pprint(eq_set[i])
+                history.append(replace_expr(str(eq_set[i])))
                 print()
 
-    elif mode == 2:
+    elif mode == "2":
         eq1 = input("Enter first equation: ")
         left1 = eval(eq1[: eq1.find("=")])
         right1 = eval(eq1[eq1.find("=") + 1 :])
 
         eq2 = input("Enter second equation: ")
         left2 = eval(eq2[: eq2.find("=")])
         right2 = eval(eq2[eq2.find("=") + 1 :])
@@ -550,15 +743,15 @@
         for value in eqs:
             eq_list.append(value)
 
         result = "".join(eq_list)
         print("\nx, y:\n")
         pprint(result)
 
-    elif mode == 3:
+    elif mode == "3":
         eq1 = input("Enter equation 1: ")
         left1 = eval(eq1[: eq1.find("=")])
         right1 = eval(eq1[eq1.find("=") + 1 :])
 
         eq2 = input("Enter equation 2: ")
         left2 = eval(eq2[: eq2.find("=")])
         right2 = eval(eq2[eq2.find("=") + 1 :])
@@ -577,159 +770,151 @@
             eq_list.append(value)
 
         result = "".join(eq_list)
         print("\nx, y, z:\n")
         pprint(result)
 
 
-def check_simp(expr) -> bool:
-    if str(simplify(expr, evaluate=False)) != str(expr):
+################
+# Helper funcs #
+################
+
+
+# These assistant functions sanatize inputs and prevent errors
+
+
+def check_simp(expr: str) -> bool:
+    """Check for simplification of an expression.
+
+    Takes an expression and simplifies/rewrites it
+    if possible. Otherwise returns boolean value False.
+    """
+
+    if str(simplify(expr, evaluate=False)) != expr:
         print("\nSimplify/rewrite:\n")
         print_expr(simplify(expr, evaluate=False))
 
     else:
         return False
 
 
-def check_order(order: str) -> bool:
+def check_order(order: str):
+    """Check if the order of differentiation is valid.
+
+    Takes the order of differentiation and gives an error
+    if it is invalid.
+    """
+
     if ("." in order) or (order.isnumeric() == False):
         print()
-        logging.error(
-            "OrderError: Order of derivative calculation is not a valid number."
-        )
-        return False
+        logging.error("Invalid order of differentiation.")
 
-    else:
-        return True
 
+def check_num(num: str):
+    """Checks if a string is numerical (valid).
+
+    Takes a numerical valid string and gives an error
+    if it is invalid.
+    """
 
-def check_bound(bound: str):
     if (
-        (bound.isnumeric() is False)
-        and ("pi" not in bound)
-        and ("e" not in bound)
-        and ("E" not in bound)
-        and ("-" not in bound)
-        and ("." not in bound)
-        and ("sqrt" not in bound)
-        and ("oo" not in bound)
-        and ("/" not in bound)
+        (num.isnumeric() is False)
+        and ("pi" not in num)
+        and ("e" not in num)
+        and ("E" not in num)
+        and ("-" not in num)
+        and ("." not in num)
+        and ("sqrt" not in num)
+        and ("oo" not in num)
+        and ("/" not in num)
     ):
         print()
-        logging.error("TypeError: Integration bound is not a number.")
+        logging.error("Invalid integration bound/numerical expression.")
 
 
 def replace_expr(expr: str) -> str:
-    expr = expr.strip(" ")
+    """Sanatizes an expression from input.
 
-    if "^" in expr:
-        expr = expr.replace("^", "**")
+    Takes a string and sanatizes input for calculation.
+    """
 
-    if "e" in expr:
-        expr = expr.replace("e", "E")
+    expr = expr.strip(" ")
 
-    if "E**" in expr:
-        expr = expr.replace("E**", "exp")
+    # The extra 1 at the end is to recognize whether the "e"
+    # is part of an expression or a constant on it's own.
 
-    if "ln" in expr:
-        expr = expr.replace("ln", "log")
+    if "E" in expr:
+        expr = expr.replace("E", "E1")
 
-    if "arc" in expr:
-        expr = expr.replace("arc", "a")
+    if "e" in expr:
+        expr = expr.replace("e", "E1")
 
-    if "abs" in expr:
-        expr = expr.replace("abs", "Abs")
+    for r in expr_replace:
+        expr = expr.replace(*r)
 
     return expr
 
 
-def replace_bound(bound: str) -> str:
-    if "pi" in bound:
-        bound = bound.replace("pi", str(np.pi))
-
-    if "E" in bound:
-        bound = bound.replace("E", str(np.e))
-
-    return bound
-
-
-def factorial(x):
-    return gamma(x + 1)
-
-
-def trig_rep(function: str) -> str:
-    # Sympy and Numpy trig functions are vastly different
-    # and uses different prefixes. Thus this replacement
-    # algorithm is needed.
-    if "asin" in function:
-        function = function.replace("asin", "arcsin")
-
-    if "acos" in function:
-        function = function.replace("acos", "arccos")
-
-    if "atan" in function:
-        function = function.replace("atan", "arctan")
-
-    if "asinh" in function:
-        function = function.replace("asinh", "arcsinh")
-
-    if "acosh" in function:
-        function = function.replace("acosh", "arccosh")
+def replace_graph(function: str) -> str:
+    """Replaces an expression (function) for graphing.
 
-    if "atanh" in function:
-        function = function.replace("atanh", "arctanh")
-
-    if "csc" in function:
-        function = function.replace("csc", "1/sin")
-
-    # Unfortunately, Numpy does not have an implemented csc,
-    # sec, cot, csch, etc. so we have to implement our own.
-
-    if "sec" in function:
-        function = function.replace("sec", "1/cos")
-
-    if "cot" in function:
-        function = function.replace("cot", "1/tan")
-
-    if "csch" in function:
-        function = function.replace("csch", "1/sinh")
-
-    if "sech" in function:
-        function = function.replace("sech", "1/cosh")
-
-    if "coth" in function:
-        function = function.replace("coth", "1/tanh")
-
-    if "Abs" in function:
-        function = function.replace("Abs", "fabs")
+    Takes a string and sanatizes it for graphing.
+    This replacement includes changing prefixes of trig
+    functions (since Sympy and Numpy trig functions uses
+    different prefixes) and an implementation of csc, sec,
+    cot, etc. (since Numpy does not provide them).
+    """
 
     if "log" in function and ",x)" in function:
         function = function.replace("log", "mt.log")
 
+    # Graph constant functions
+
     if "x" not in function:
         function = "0 * x + " + function
 
+    for r in graph_replace:
+        function = function.replace(*r)
+
     return function
 
 
 def print_expr(text: str):
+    """Selects printing method.
+
+    Linked to the printing settings option in settings.
+    Chooses either normal print or Sympy pretty print.
+    """
+
     printing_methods = {"p": lambda t: pprint(text), "n": lambda t: print(text)}
 
     try:
         printing_methods[print_option](text)
 
     except NameError:
         printing_methods["p"](text)
 
 
+def factorial(x):
+    """Simple implementation of a factorial function."""
+
+    # Define our own factorial
+    return ss.gamma(x + 1)
+
+
 def nprint(text: str):
     print(text)
     time.sleep(0.04)
 
 
+####################
+# Driving programs #
+####################
+
+
 def main():
     with Progress(
         SpinnerColumn(finished_text="[bright_green]√[/bright_green]"),
         TextColumn("[green]Handling imports[/green]..."),
         BarColumn(),
         MofNCompleteColumn(),
         TimeElapsedColumn(),
@@ -737,16 +922,15 @@
     ) as progress:
         task = progress.add_task("", total=50)
 
         while not progress.finished:
             progress.update(task, advance=1)
             time.sleep(random.randint(2, 5) / 100)
 
-    global x, y, z
-    x, y, z = symbols("x, y, z")
+    global x, y, z, history, expr_replace, graph_replace
 
     while True:
         instruct_path = (
             os.path.dirname(os.path.abspath(__file__))
             + "/texts/main_screen.txt"
             # TODO: make the PATH compatible with Windows
         )
@@ -764,15 +948,15 @@
             elif date_option == "2":
                 now = (datetime.datetime.now()).strftime("%Y/%m/%d %H:%M:%S")
         except:
             now = (datetime.datetime.now()).strftime("%Y/%m/%d %H:%M:%S")
 
         print(f"\n(Time now is: {now})\n")
         print("[bold bright_green](Current Screen: Main Screen)[/bold bright_green]\n")
-        print("[bright_magenta]Enter Command: [/bright_magenta]", end="")
+        print("[purple]Enter Command: [/purple]", end="")
         cmd = input()
 
         if cmd == "1":
             simp()
 
         elif cmd == "2":
             derivacalc()
@@ -790,14 +974,15 @@
             settings()
 
         elif cmd == "7":
             nprint("\n[bright_yellow]Exiting Calc-ULTRA ... ... ...[/bright_yellow]\n")
             break
 
         else:
+            print("\n")
             logging.warning(f'Invalid command:"{cmd}"\n')
 
 
 """
 If you find this message, type 'hi' in the general discussions - sudoer-Huatao
 """
 
@@ -814,57 +999,72 @@
     print()
 
     while True:
         try:
             nprint(
                 "\n[bold bright_green](Current Screen: DerivaCalc Main Screen)[/bold bright_green]\n"
             )
-            print("[bright_magenta]Enter Command: [/bright_magenta]", end="")
+            print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
                 nprint(
                     "\n[bold bright_green](Current Screen: Derivative Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ")
-                order = input("Enter order of derivative calculation: ")
+                function = input("Enter a function: ", key_bindings=key_bindings)
+                order = input(
+                    "Enter order of derivative calculation: ", key_bindings=key_bindings
+                )
                 derive(function, order)
 
             elif cmd == "2":
                 nprint(
                     "\n[bold bright_green](Current Screen: Partial Derivative Screen)[/bold bright_green]\n"
                 )
                 function = input(
-                    "Enter a function containing x and y or x and y and z: "
+                    "Enter a function containing x and y or x and y and z: ",
+                    key_bindings=key_bindings,
+                )
+                var = input(
+                    "Enter variable to differentiate in respect to: ",
+                    key_bindings=key_bindings,
                 )
-                var = input("Enter variable to differentiate in respect to: ")
                 if var != "x" and var != "y" and var != "z":
                     print()
-                    logging.error("Variable to differentite in respect to is invalid.")
+                    logging.error("Invalid variable to differentite in respect to.")
                 else:
-                    order = input("Enter the order of partial derivative calculation: ")
+                    order = input(
+                        "Enter the order of partial derivative calculation: ",
+                        key_bindings=key_bindings,
+                    )
                     partial_derive(function, var, order)
 
             elif cmd == "3":
                 nprint(
                     "\n[bold bright_green](Current Screen: Implicit Derivative Screen)[/bold bright_green]\n"
                 )
-                circ = input("Enter an equation containing x and y:")
-                order = input("Enter order of implicit derivative calculation: ")
+                circ = input(
+                    "Enter an equation containing x and y:", key_bindings=key_bindings
+                )
+                order = input(
+                    "Enter order of implicit derivative calculation: ",
+                    key_bindings=key_bindings,
+                )
                 implicit_derive(circ, order)
 
             elif cmd == "4":
                 print("\n[bright_yellow]Exiting DerivaCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
+                print("\n")
                 logging.warning(f'Invalid command:"{cmd}"')
         except:
             print("\n")
-            logging.error("UnknownError: An unknown error occured.")
+            logging.error("An unknown error occured.")
             nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def intecalc():
     instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/intecalc.txt"
     intecalc = open(instruct_path, mode="r")
     for line in intecalc.readlines():
@@ -876,62 +1076,79 @@
     print()
 
     while True:
         try:
             nprint(
                 "[bold bright_green](Current Screen: InteCalc Main Screen)[/bold bright_green]\n"
             )
-            print("[bright_magenta]Enter Command: [/bright_magenta]", end="")
+            print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
                 nprint(
                     "\n[bold bright_green](Current Screen: Antiderivative Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ")
+                function = input("Enter a function: ", key_bindings=key_bindings)
                 antiderive(function)
 
             elif cmd == "2":
                 nprint(
                     "\n[bold bright_green](Current Screen: Definite Integral Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ")
-                lower_bound = input("\nEnter the lower bound: ")
-                upper_bound = input("Enter the upper bound: ")
+                function = input("Enter a function: ", key_bindings=key_bindings)
+                lower_bound = input(
+                    "\nEnter the lower bound: ", key_bindings=key_bindings
+                )
+                upper_bound = input(
+                    "Enter the upper bound: ", key_bindings=key_bindings
+                )
                 print(def_int(function, lower_bound, upper_bound))
 
             elif cmd == "3":
                 nprint(
                     "\n[bold bright_green](Current Screen: Improper Integral Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ")
-                lower_bound = input("\nEnter the lower bound: ")
-                upper_bound = input("Enter the upper bound: ")
+                function = input("Enter a function: ", key_bindings=key_bindings)
+                lower_bound = input(
+                    "\nEnter the lower bound: ", key_bindings=key_bindings
+                )
+                upper_bound = input(
+                    "Enter the upper bound: ", key_bindings=key_bindings
+                )
                 improp_int(function, lower_bound, upper_bound)
 
             elif cmd == "4":
                 nprint(
                     "\n[bold bright_green](Current Screen: Double Integral Screen)[/bold bright_green]\n"
                 )
                 function = input("Enter a function: ")
-                outer_low = input("\nEnter the lower outer bound: ")
-                outer_up = input("Enter the upper outer bound: ")
-                inner_low = input("\nEnter the lower inner bound: ")
-                inner_up = input("Enter the upper inner bound: ")
+                outer_low = input(
+                    "\nEnter the lower outer bound: ", key_bindings=key_bindings
+                )
+                outer_up = input(
+                    "Enter the upper outer bound: ", key_bindings=key_bindings
+                )
+                inner_low = input(
+                    "\nEnter the lower inner bound: ", key_bindings=key_bindings
+                )
+                inner_up = input(
+                    "Enter the upper inner bound: ", key_bindings=key_bindings
+                )
                 double_int(function, outer_low, outer_up, inner_low, inner_up)
 
             elif cmd == "5":
                 print("\n[bright_yellow]Exiting InteCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
+                print("\n")
                 logging.warning(f'Invalid command: "{cmd}"')
         except:
             print("\n")
-            logging.error("UnknownError: An unknown error occured.")
+            logging.error("An unknown error occured.")
             nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def limcalc():
     instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/limcalc.txt"
     limcalc = open(instruct_path, mode="r")
     for line in limcalc.readlines():
@@ -950,37 +1167,38 @@
             print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
                 nprint(
                     "\n[bold bright_green](Current screen: Limit Screen)[/bold bright_green]\n"
                 )
-                expr = input("Enter an expression: ")
-                value = input("Enter point of evaluation: ")
+                expr = input("Enter an expression: ", key_bindings=key_bindings)
+                value = input("Enter point of evaluation: ", key_bindings=key_bindings)
                 lim(expr, value)
 
             elif cmd == "2":
                 nprint(
                     "\n[bold bright_green](Current screen: One-sided Limit Screen)[/bold bright_green]\n"
                 )
-                expr = input("Enter an expression: ")
-                value = input("Enter point of evaluation: ")
+                expr = input("Enter an expression: ", key_bindings=key_bindings)
+                value = input("Enter point of evaluation: ", key_bindings=key_bindings)
                 direction = input("Enter direction of limit ('left' or 'right'): ")
                 side_lim(expr, value, direction)
 
             elif cmd == "3":
                 print("\n[bright_yellow]Exiting LimCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
+                print("\n")
                 logging.warning(f'Invalid command: "{cmd}"')
 
         except:
             print("\n")
-            logging.error("UnknownError: An unknown error occured.")
+            logging.error("An unknown error occured.")
             nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def algcalc():
     instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/algcalc.txt"
     algcalc = open(instruct_path, mode="r")
     for line in algcalc.readlines():
@@ -999,20 +1217,23 @@
             print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
                 nprint(
                     "\n[bold bright_green](Current screen: Equation Solver Screen)[/bold bright_green]\n"
                 )
-                print(
-                    "Enter mode: 1 for one set equation, 2 for two, and 3 for three: ",
-                    end="",
-                )
-                mode = int(input())
-                eq_solve(mode)
+                mode = ""
+
+                while mode != "q":
+                    print(
+                        'Enter mode: 1 for one set equation, 2 for two, and 3 for three ("q" to quit): ',
+                        end="",
+                    )
+                    mode = input()
+                    eq_solve(mode)
 
             elif cmd == "2":
                 nprint(
                     "\n[bold bright_green](Current screen: Vector Calculation Screen)[/bold bright_green]\n"
                 )
 
                 print("Write a vector like [1, 2, 3], then perform operations!")
@@ -1022,27 +1243,27 @@
                 print("- cross(smth, smth) to calculate the cross product")
                 print(
                     "- A pair of [bright_magenta]< >[/bright_magenta]s encasing a vector to calculate it's norm!"
                 )
                 print('Enter any expression to start ("q" to quit):\n')
 
                 while True:
-                    expr = input()
+                    expr = input(key_bindings=key_bindings)
                     try:
                         if expr != "q":
                             expr = (
                                 (
                                     (
                                         (expr.replace("[", "array([")).replace(
                                             "]", "])"
                                         )
                                     ).replace("<", "norm(")
                                 ).replace(">", ")")
                             ).strip(" ")
-                            result = eval(trig_rep(expr))
+                            result = eval(replace_graph(expr))
                             print("\n[bright_yellow]Result: [/bright_yellow]", end="")
                             pprint(result)
                             print()
 
                         else:
                             break
                     except:
@@ -1061,27 +1282,27 @@
                 )
                 print(
                     "- A pair of [bright_magenta]| |[/bright_magenta] to calculate the determinant."
                 )
                 print('Enter any expression to start ("q" to quit):\n')
 
                 while True:
-                    expr = input()
+                    expr = input(key_bindings=key_bindings)
                     try:
                         if expr != "q":
                             expr = (
                                 (
                                     (
                                         (expr.replace("[[", "array([[")).replace(
                                             "]]", "]])"
                                         )
                                     ).replace("|a", "det(a")
                                 ).replace(")|", "))")
                             ).strip(" ")
-                            result = eval(trig_rep(expr))
+                            result = eval(replace_graph(expr))
                             print("\n[bright_yellow]Result: [/bright_yellow]\n")
                             pprint(result)
                             print()
 
                         else:
                             break
                     except:
@@ -1089,19 +1310,20 @@
                         logging.error(f'Could not parse: "{expr}"\n')
 
             elif cmd == "4":
                 print("\n[bright_yellow]Exiting AlgCalc ... ... ...[/bright_yellow]")
                 break
 
             else:
+                print("\n")
                 logging.warning(f'Invalid command: "{cmd}"')
 
         except:
             print("\n")
-            logging.error("UnknownError: An unknown error occured.")
+            logging.error("An unknown error occured.")
             nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def settings():
     while True:
         settings_path = (
             os.path.dirname(os.path.abspath(__file__)) + "/texts/settings.txt"
@@ -1111,15 +1333,15 @@
         for line in settings.readlines():
             line = line.rstrip()
             if ("---" in line) or ("|" in line):
                 nprint("[gold1]" + line + " [/gold1]")
             else:
                 nprint(line)
         print("\n[bold green](Current Screen: Settings Screen)[/bold green]\n")
-        print("[bright_magenta]Enter Command: [/bright_magenta]", end="")
+        print("[purple]Enter Command: [/purple]", end="")
         cmd = input()
 
         if cmd == "print":
             print(
                 "\n[bold bright_green](Current Screen: Print Settings Screen)[/bold bright_green]\n"
             )
 
@@ -1169,11 +1391,13 @@
             print(f'Graph style set to "{style}".')
 
         elif cmd == "exit":
             print("\n[bright_yellow]Exiting settings ... ... ...[/bright_yellow]")
             break
 
         else:
+            print("\n")
             logging.warning(f'Invalid command:"{cmd}"')
 
 
 main()
+# You've reached the end of the file!
```

### Comparing `calc_ultra-1.3.4/src/calc_ultra/texts/algcalc.txt` & `calc_ultra-1.3.5/src/calc_ultra/texts/algcalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.4/src/calc_ultra/texts/derivacalc.txt` & `calc_ultra-1.3.5/src/calc_ultra/texts/derivacalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.4/src/calc_ultra/texts/intecalc.txt` & `calc_ultra-1.3.5/src/calc_ultra/texts/intecalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.4/src/calc_ultra/texts/limcalc.txt` & `calc_ultra-1.3.5/src/calc_ultra/texts/limcalc.txt`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.4/src/calc_ultra.egg-info/PKG-INFO` & `calc_ultra-1.3.5/src/calc_ultra.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,105 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.4
+Version: 1.3.5
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sympy>=1.12
 Requires-Dist: numpy>=1.26.2
-Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: rich>=13.7.1
-Requires-Dist: scipy>=1.12.0
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: prompt_toolkit>=3.0.43
 
 # calc-ultra
 
-[![GPLv3 License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.4-blue.svg)](https://github.com/sudoer-Huatao/Calc-ULTRA_Calculus-Calculator)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.5-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
 
 > **Calculus made easy**
 
-(Turn on dark mode for a better aesthetic)
+(Turn on dark mode for a better aesthetic) 📲
 
-The Calc-Ultra calculus calculator, but as a module!
-
-- Little Python background knowledge is needed!
+Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
 
 Supports:
 
 - Derivatives
 - Partials
 - Implicit differentiation
+- Limits
 - Antiderivatives
 - Definite integrals
 - Improper integrals
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
-## Note
+## Chinese version
 
-This is the module package of the Calc-Ultra calculator. For the Python script of this package, visit <https://github.com/sudoer-Huatao/Calc-ULTRA> (**unmaintained**).
+Want to check out the Chinese version? Visit <https://github.com/sudoer-Huatao/calc_ultra-chinese>! 🇨🇳
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
-Command line: `pip3 install calc-ultra`.
-Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra" when you need to use the calculator.
+Use the following command to download Calc-Ultra (pip should be installed):
+
+`pip3 install calc-ultra`
+
+Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra".
 
-To run the calculator, import Calc-ULTRA as `calc_ultra` like so:
+Import Calc-Ultra like so to use:
 
 `from calc_ultra import main`
 
-Make sure you have the latest version installed. To update calc-ultra, run `pip3 install --upgrade calc-ultra`.
+Please make sure you have the latest version installed. To update calc-ultra, run the following command:
 
-## Requirements
+`pip3 install --upgrade calc-ultra`
 
-This program requires the `sympy`,  `numpy`, `rich`, `matplotlib`, and `scipy` modules installed. Other required modules are built into most Python IDEs.
+## Requirements
 
-## Warnings
+Calc-Ultra requires these modules/packages:
 
-### Function limitations
+- `sympy`
+- `numpy`
+- `matplotlib`
+- `scipy`
+- `rich`
+- `prompt-toolkit`
 
-Due to limitations of the SymPy module, **some functions cannot be integrated**. The Error Function `erf(x)` can be integrated in both indefinite integral and definite integral calculation, but the Absolute Value and Factorial functions are only available to definite integral calculations. Integration of composed functions is also limited due to SymPy limitations. While some composed functions work, others don't. 😟
+If you do not have them installed, there is no need to worry. The modules needed should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
 
 ## Test PYPI
 
-Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>.
+Previous test versions of this project are on Test PYPI. View on <https://test.pypi.org/project/calc-ultra/>. 💾
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
-A general thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️
-And... a SPECIAL THANK-YOU to @Haobot for troubleshooting and feedback! 👍❤️
+A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
+The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
+
+- @Haobot for troubleshooting and feedback!
+- Fanbo for feedback and ideas for improvement!
 
-This program was made using SymPy and Scipy for calculation and Matplotlib and NumPy for graphing.
+This program was made using `sympy` for calculation and `numpy`, `scipy`, and `matplotlib` for graphing.
 
-## Gallery
+## Gallery (Demos)
 
 DerivaCalc derivative with graph demo:
 ![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
 ![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
```

### Comparing `calc_ultra-1.3.4/src/calc_ultra.egg-info/SOURCES.txt` & `calc_ultra-1.3.5/src/calc_ultra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

