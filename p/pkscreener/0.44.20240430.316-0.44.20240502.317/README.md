# Comparing `tmp/pkscreener-0.44.20240430.316.tar.gz` & `tmp/pkscreener-0.44.20240502.317.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240430.316.tar", last modified: Tue Apr 30 12:07:20 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240502.317.tar", last modified: Thu May  2 07:26:48 2024, max compression
```

## Comparing `pkscreener-0.44.20240430.316.tar` & `pkscreener-0.44.20240502.317.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 12:07:20.399627 pkscreener-0.44.20240430.316/
--rw-rw-rw-   0        0        0     1086 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-30 12:07:20.399627 pkscreener-0.44.20240430.316/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 12:07:20.384003 pkscreener-0.44.20240430.316/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:07:20.399627 pkscreener-0.44.20240430.316/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25815 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7288 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29455 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    20421 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8124 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   116796 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    51837 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82018 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-30 12:07:10.000000 pkscreener-0.44.20240430.316/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   123118 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    42912 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    25897 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:07:20.384003 pkscreener-0.44.20240430.316/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-30 12:07:20.000000 pkscreener-0.44.20240430.316/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-30 12:07:20.000000 pkscreener-0.44.20240430.316/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 12:07:20.000000 pkscreener-0.44.20240430.316/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-30 12:07:20.000000 pkscreener-0.44.20240430.316/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-30 12:07:20.000000 pkscreener-0.44.20240430.316/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-30 12:07:20.000000 pkscreener-0.44.20240430.316/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-30 12:07:20.399627 pkscreener-0.44.20240430.316/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-30 12:01:02.000000 pkscreener-0.44.20240430.316/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.451769 pkscreener-0.44.20240502.317/
+-rw-rw-rw-   0        0        0     1086 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-02 07:26:48.451769 pkscreener-0.44.20240502.317/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.436155 pkscreener-0.44.20240502.317/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.436155 pkscreener-0.44.20240502.317/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25810 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7496 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29455 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    21093 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20691 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8124 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   117763 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82304 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-02 07:26:39.000000 pkscreener-0.44.20240502.317/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123195 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    42912 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    25897 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:26:48.436155 pkscreener-0.44.20240502.317/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-02 07:26:48.000000 pkscreener-0.44.20240502.317/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-02 07:26:48.451769 pkscreener-0.44.20240502.317/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-05-02 07:21:56.000000 pkscreener-0.44.20240502.317/setup.py
```

### Comparing `pkscreener-0.44.20240430.316/LICENSE` & `pkscreener-0.44.20240502.317/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/LICENSE-Others` & `pkscreener-0.44.20240502.317/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/PKG-INFO` & `pkscreener-0.44.20240502.317/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240430.316
+Version: 0.44.20240502.317
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240430.316.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.317.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240430.316/README.md` & `pkscreener-0.44.20240502.317/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/__init__.py` & `pkscreener-0.44.20240502.317/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 6
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:2,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:23,X:12:24,X:12:10,X:12:12:i 1m,X:12:12:i 5m,X:12:13:i 1m"
+        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:5:0:30,X:12:6:3,X:12:6:7:1,X:12:6:8,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m"
 
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/MarketMonitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,24 +33,26 @@
 class MarketMonitor(SingletonMixin, metaclass=SingletonType):
     def __init__(self,monitors=[], maxNumResultsPerRow=5,maxNumColsInEachResult=6,maxNumRowsInEachResult=10):
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
             self.monitors = monitors
             self.monitorIndex = 0
             self.monitorPositions = {}
+            # self.monitorNames = {}
             # We are going to present the dataframes in a 3x3 matrix with limited set of columns
             rowIndex = 0
             colIndex = 0
             self.maxNumRowsInEachResult = maxNumRowsInEachResult
             self.maxNumColsInEachResult = maxNumColsInEachResult
             self.maxNumResultsPerRow = maxNumResultsPerRow
             maxColIndex = self.maxNumColsInEachResult * self.maxNumResultsPerRow - 1
             self.lines = 0
             for monitorKey in monitors:
                 self.monitorPositions[monitorKey] = [rowIndex,colIndex]
+                # self.monitorNames[monitorKey] = ""
                 colIndex += self.maxNumColsInEachResult
                 if colIndex > maxColIndex:
                     colIndex = 0
                     rowIndex += self.maxNumRowsInEachResult
             columns = []
             colNameIndex = 0
             maxColIndex = min(maxColIndex,len(self.monitorPositions)*self.maxNumColsInEachResult -1)
@@ -120,19 +122,20 @@
                 _, startColIndex= monitorPosition
                 rowIndex += 1
                 colIndex = 0
                 highlightRows.append(startRowIndex+1)
                 startRowIndex += 1
 
         self.monitor_df = self.monitor_df.replace(np.nan, "-", regex=True)
+        # self.monitorNames[screenOptions] = f"(Dashboard) > {chosenMenu}"
+        latestScanMenuOption = f"[+] {dbTimestamp} (Dashboard) > " + f"{chosenMenu} [{screenOptions}]"
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
-            + f"[+] {dbTimestamp} (Dashboard) > "
-            + f"{chosenMenu} [{screenOptions}]"
+            + latestScanMenuOption
             + colorText.END
             , enableMultipleLineOutput=True
         )
         tabulated_results = colorText.miniTabulator().tabulate(
             self.monitor_df, tablefmt=colorText.No_Pad_GridFormat,
             highlightCharacter=colorText.HEAD+"="+colorText.END,
             showindex=False,
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,17 @@
         #                       columns=allDailyCandles[stock]["columns"],
         #                       index=[allDailyCandles[stock]["index"][-1]])
         #         latestDailyCandle[stock] = df.to_dict("split")
         #     except:
         #         continue
         return allDailyCandles
     
-    def getIntradayCandleFromMorning(int_cache_file):
+    def getIntradayCandleFromMorning(int_cache_file=None,candle1MinuteNumberSinceMarketStarted=0):
+        if candle1MinuteNumberSinceMarketStarted <= 0:
+            candle1MinuteNumberSinceMarketStarted = PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber
         morningIntradayCandle = None
         intradayDB = PKIntradayStockDataDB(fileName=int_cache_file)
         allDailyIntradayCandles = intradayDB.pickler.pickler.unpickle(fileName=intradayDB.pickler.fileName)
         PKMarketOpenCloseAnalyser.allIntradayCandles = allDailyIntradayCandles
         morningIntradayCandle = {}
         stocks = list(allDailyIntradayCandles.keys())
         numOfCandles = PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber
@@ -177,17 +179,17 @@
                 # OHLCV and replace the last daily candle with this one candle to
                 # simulate the scan outcome from morning.
                 df = pd.DataFrame(data=allDailyIntradayCandles[stock]["data"],
                                 columns=allDailyIntradayCandles[stock]["columns"],
                                 index=allDailyIntradayCandles[stock]["index"])
                 df = df.head(numOfCandles)
                 try:
-                    df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
+                    df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+candle1MinuteNumberSinceMarketStarted}:00+05:30').to_datetime64()]
                 except:
-                    df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30', utc=True)]
+                    df = df[df.index <=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+candle1MinuteNumberSinceMarketStarted}:00+05:30', utc=True)]
                     pass
                 if df is not None and len(df) > 0:
                     combinedCandle = {"Open":PKMarketOpenCloseAnalyser.getMorningOpen(df), "High":max(df["High"]), 
                                     "Low":min(df["Low"]),"Close":PKMarketOpenCloseAnalyser.getMorningClose(df),
                                     "Adj Close":df["Adj Close"][-1],"Volume":sum(df["Volume"])}
                     tradingDate = df.index[-1] #PKDateUtilities.tradingDate()
                     timestamp = datetime.datetime.strptime(tradingDate.strftime("%Y-%m-%d %H:%M:%S"),"%Y-%m-%d %H:%M:%S")
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/PKScanRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         for worker in consumers:
             worker.objectDictionaryPrimary = stockDictPrimary
             worker.objectDictionarySecondary = stockDictSecondary
             worker.refreshDatabase = True
             
     def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb,tasks_queue, results_queue, consumers,logging_queue):
         if tasks_queue is None or results_queue is None or consumers is None:
-            tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items)
+            tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(menuOption,keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items)
             try:
                 if logging_queue is not None:
                     log_queue_reader = LogQueueReader(logging_queue)
                     log_queue_reader.start()
             except:
                 pass
         # else:
@@ -284,40 +284,42 @@
         if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options):
             # Don't terminate the multiprocessing clients if we're 
             # going to pipe the results from an earlier run
             # or we're running in monitoring mode
             PKScanRunner.terminateAllWorkers(consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
-    def prepareToRunScan(keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items):
+    def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items):
         tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
         sec_cache_file = cache_file if "intraday_" in cache_file else f"intraday_{cache_file}"
         consumers = [
                     PKMultiProcessorClient(
                         StockScreener().screenStocks,
                         tasks_queue,
                         results_queue,
                         logging_queue,
                         screenCounter,
                         screenResultsCounter,
                         stockDictPrimary,
                         stockDictSecondary,
+                        # (stockDictPrimary if menuOption not in ["C"] else None),
+                        # (stockDictSecondary if menuOption not in ["C"] else None),
                         PKScanRunner.fetcher.proxyServer,
                         keyboardInterruptEvent,
                         default_logger(),
                         PKScanRunner.fetcher,
                         PKScanRunner.configManager,
                         PKScanRunner.candlePatterns,
                         scr,
                         None,
                         None
-                        #cache_file if exists else None,
-                        #sec_cache_file,
+                        # (cache_file if (exists and menuOption in ["C"]) else None),
+                        # (sec_cache_file if (exists and menuOption in ["C"]) else None),
                     )
                     for _ in range(totalConsumers)
                 ]
         PKScanRunner.startWorkers(consumers)
         return tasks_queue,results_queue,consumers,logging_queue
 
     def startWorkers(consumers):
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -745,40 +745,48 @@
             if filter not in [2,4]: # SqZ/All
                 return False
             screenDict["Pattern"] = f'{saved[0]}{colorText.BOLD}{colorText.WARN}TTM-SQZ{colorText.END}'
             saveDict["Pattern"] = f'{saved[1]}TTM-SQZ'
             return True
         return False
 
-    def findMACDCrossover(self, df, afterTimestamp=None, nthCrossover=1, upDirection=True):
+    def findMACDCrossover(self, df, afterTimestamp=None, nthCrossover=1, upDirection=True, minRSI=60):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         data = data[::-1]  # Reverse the dataframe so that its the oldest date first
         macdLine, macdSignal, macdHist = pktalib.MACD(data["Close"], 12, 26, 9)
+        # rsi_df = pktalib.RSI(data["Close"], 14)
         line_df = pd.DataFrame(macdLine)
         signal_df = pd.DataFrame(macdSignal)
         diff_df = pd.concat([line_df, signal_df, signal_df-line_df], axis=1)
         diff_df.columns = ["line","signal","diff"]
+        # brokerSqrOfftime = None
         try:
-            # Let's only consider those candles that are after the alert issue-time in the mornings
-            diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber}:00+05:30').to_datetime64()]
+            # Let's only consider those candles that are after the alert issue-time in the mornings + 2 candles (for buy/sell)
+            diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber + 2}:00+05:30').to_datetime64()]
+            # brokerSqrOfftime = pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 15:14:00+05:30').to_datetime64()
         except:
-            diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber}:00+05:30', utc=True)]
+            diff_df = diff_df[diff_df.index >=  pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+self.configManager.morninganalysiscandlenumber + 2}:00+05:30', utc=True)]
+            # brokerSqrOfftime = pd.to_datetime(f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 15:14:00+05:30', utc=True)
             pass
         index = len(diff_df)
         crossOver = 0
+        
+        # Loop until we've found the nth crossover for MACD or we've reached the last point in time
         while (crossOver < nthCrossover and index >=0):
-            if diff_df["diff"][index-1] < 0:
-                while(diff_df["diff"][index-1] < 0 and index >=0):
+            if diff_df["diff"][index-1] < 0: # Signal line has not crossed yet and is below the zero line
+                while((diff_df["diff"][index-1] < 0 and index >=0)): # and diff_df.index <= brokerSqrOfftime): # or diff_df["rsi"][index-1] <= minRSI):
+                    # Loop while Signal line has not crossed yet and is below the zero line and we've not reached the last point
                     index -= 1
             else:
-                while(diff_df["diff"][index-1] >= 0 and index >=0):
+                while((diff_df["diff"][index-1] >= 0 and index >=0)): # and diff_df.index <= brokerSqrOfftime): # or diff_df["rsi"][index-1] <= minRSI):
+                    # Loop until signal line has not crossed yet and is above the zero line
                     index -= 1
             crossOver += 1
         ts = diff_df.tail(len(diff_df)-index +1).head(1).index[-1]
         return ts, df[df.index == ts] #df.head(len(df) -index +1).tail(1)
     
     # Find stock showing RSI crossing with RSI 9 SMA
     def findRSICrossingMA(self, df, screenDict, saveDict,lookFor=1, maLength=9, rsiKey="RSI"):
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/StockScreener.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,19 +126,21 @@
                     intraday_processedData = intraday_processedData.head(len(processedData))
                     data = data.tail(len(intraday_data))
                     intraday_data = intraday_data.tail(len(data))
                     # Indexes won't match. Hence, we'd need to fallback on tolist
                     processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
                     fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
                 else:
-                    processedData.loc[:,"RSIi"] = np.nan
-                    fullData.loc[:,"RSIi"] = np.nan
+                    with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
+                        processedData.loc[:,"RSIi"] = np.nan
+                        fullData.loc[:,"RSIi"] = np.nan
             else:
-                    processedData.loc[:,"RSIi"] = np.nan
-                    fullData.loc[:,"RSIi"] = np.nan
+                    with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
+                        processedData.loc[:,"RSIi"] = np.nan
+                        fullData.loc[:,"RSIi"] = np.nan
 
             def returnLegibleData(exceptionMessage=None):
                 if backtestDuration == 0 or menuOption not in ["B"]:
                     raise ScreeningStatistics.EligibilityConditionNotMet(exceptionMessage)
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
                     screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,18 +123,26 @@
             if userArgs is not None and userArgs.v:
                 os.environ["RUNNER"]="LOCAL_RUN_SCANNER"
             return
         elif (userArgs is not None and userArgs.runintradayanalysis):
             return
         if clearAlways or OutputControls().enableMultipleLineOutput:
             if platform.system() == "Windows":
-                # os.system('color 0f') # sets the background to black with white forerground
+                try:
+                    os.system('color 0f') # sets the background to black with white forerground
+                except:
+                    pass
                 os.system("cls")
+            elif "Darwin" in platform.system():
+                try:
+                    os.system('setterm -background black -foreground white -store')
+                except:
+                    pass
+                os.system("clear")
             else:
-                # os.system('setterm -background black -foreground white -store')
                 os.system("clear")
         try:
             if clearAlways or OutputControls().enableMultipleLineOutput:
                 art = colorText.GREEN + artText + colorText.END + f" | {marketStatus()}"
                 OutputControls().printOutput(art.encode('utf-8').decode(STD_ENCODING), enableMultipleLineOutput=True)
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
@@ -430,15 +438,16 @@
         filename,
         label,
         backtestSummary=None,
         backtestDetail=None,
         addendum=None,
         addendumLabel=None,
         summaryLabel = None,
-        detailLabel = None
+        detailLabel = None,
+        legendPrefixText = ""
     ):
         if "PKDevTools_Default_Log_Level" not in os.environ.keys():
             if (("RUNNER" in os.environ.keys() and os.environ["RUNNER"] == "LOCAL_RUN_SCANNER")):
                 return
         warnings.filterwarnings("ignore", category=DeprecationWarning)
         ART_FONT_SIZE = 30
         STD_FONT_SIZE = 60
@@ -474,15 +483,15 @@
             stdfont_addendumtext_width , stdfont_addendumtext_height = stdfont.getsize_multiline(unstyled_addendum)
             titleLabels.append(addendumLabel)
             dfs_to_print.append(addendum)
             unstyled_dfs.append(unstyled_addendum)
 
         repoText = tools.getRepoHelpText(table,backtestSummary)
         artfont_repotext_width, artfont_repotext_height = artfont.getsize_multiline(repoText)
-        legendText = tools.getLegendHelpText(table,backtestSummary)
+        legendText = legendPrefixText + tools.getLegendHelpText(table,backtestSummary)
         _, artfont_legendtext_height = artfont.getsize_multiline(legendText)
         column_separator = "|"
         line_separator = "+"
         stdfont_sep_width, _ = stdfont.getsize_multiline(column_separator)
 
         startColValue = 100
         xVertical = startColValue
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/classes/keys.py` & `pkscreener-0.44.20240502.317/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/courbd.ttf` & `pkscreener-0.44.20240502.317/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/globals.py` & `pkscreener-0.44.20240502.317/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -2035,14 +2035,15 @@
     pngExtension,
     addendum=None,
     addendumLabel=None,
     backtestSummary="",
     backtestDetail="",
     summaryLabel = None,
     detailLabel = None,
+    legendPrefixText = ""
 ):
     if "PKDevTools_Default_Log_Level" not in os.environ.keys():
         if (("RUNNER" not in os.environ.keys()) or ("RUNNER" in os.environ.keys() and os.environ["RUNNER"] == "LOCAL_RUN_SCANNER")):
             return
     try:
         Utility.tools.tableToImage(
             markdown_results,
@@ -2050,15 +2051,16 @@
             pngName + pngExtension,
             menuChoiceHierarchy,
             backtestSummary=backtestSummary,
             backtestDetail=backtestDetail,
             addendum=addendum,
             addendumLabel=addendumLabel,
             summaryLabel = summaryLabel,
-            detailLabel = detailLabel
+            detailLabel = detailLabel,
+            legendPrefixText = legendPrefixText
         )
         sendMessageToTelegramChannel(
             message=None,
             document_filePath=pngName + pngExtension,
             caption=caption,
             user=user,
         )
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240502.317/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240502.317/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240502.317/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240502.317/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240430.316
+Version: 0.44.20240502.317
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240430.316.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240502.317.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.315/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240430.316/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240430.316/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240502.317/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240430.316/setup.py` & `pkscreener-0.44.20240502.317/setup.py`

 * *Files identical despite different names*

