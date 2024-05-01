# Comparing `tmp/fintoolkit-0.0.8.tar.gz` & `tmp/fintoolkit-0.0.9.tar.gz`

## Comparing `fintoolkit-0.0.8.tar` & `fintoolkit-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_black_scholes.py
--rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_cboe_margin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_data.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_famafrench.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_fixed_income.py
--rw-r--r--   0        0        0    18014 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_functional.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_portfolio.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/tests/test_visualization.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/__init__.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/asset_class.py
--rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/black_scholes.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/cboe_margin.py
--rw-r--r--   0        0        0    10690 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/data.py
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/fixed_income.py
--rw-r--r--   0        0        0    53112 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/functional.py
--rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/portfolio.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/toolkit/visualization.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/.gitignore
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 fintoolkit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_black_scholes.py
+-rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_cboe_margin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_data.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_famafrench.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_fixed_income.py
+-rw-r--r--   0        0        0    18014 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_functional.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_portfolio.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/tests/test_visualization.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/__init__.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/asset_class.py
+-rw-r--r--   0        0        0    17726 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/black_scholes.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/cboe_margin.py
+-rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/data.py
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/fixed_income.py
+-rw-r--r--   0        0        0    53112 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/functional.py
+-rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/portfolio.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/toolkit/visualization.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/.gitignore
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 fintoolkit-0.0.9/PKG-INFO
```

### Comparing `fintoolkit-0.0.8/tests/test_black_scholes.py` & `fintoolkit-0.0.9/tests/test_black_scholes.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/tests/test_cboe_margin.py` & `fintoolkit-0.0.9/tests/test_cboe_margin.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/tests/test_famafrench.py` & `fintoolkit-0.0.9/tests/test_famafrench.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/tests/test_fixed_income.py` & `fintoolkit-0.0.9/tests/test_fixed_income.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/tests/test_functional.py` & `fintoolkit-0.0.9/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/tests/test_portfolio.py` & `fintoolkit-0.0.9/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/toolkit/asset_class.py` & `fintoolkit-0.0.9/toolkit/asset_class.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/toolkit/black_scholes.py` & `fintoolkit-0.0.9/toolkit/black_scholes.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/toolkit/cboe_margin.py` & `fintoolkit-0.0.9/toolkit/cboe_margin.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/toolkit/data.py` & `fintoolkit-0.0.9/toolkit/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,29 +123,31 @@
             / 100,
             how="inner",
         )
     return factors.join(rfr, how="inner")
 
 
 # Yahoo
-def get_yahoo(ticker: str = "^GSPC") -> pd.Series:
+def get_yahoo(ticker: str = "^GSPC", period: str = "max") -> pd.Series:
     """Download the historical adjusted closing price of a security with
     ticker `ticker`.
 
     Args:
         ticker (str): Yahoo! ticker of the security, by default "^GSPC", i.e. S&P 500
+    period : str, optional
+        Length of track record to download, by default 'max'
 
     Returns:
         pd.Series: Time series of the prices of the security
     """
     t = yf.Ticker(ticker)
     # Some securities e.g. crypto trades on weekends
-    s = t.history(period="max")["Close"]
+    s = t.history(period=period)["Close"]
     s.name = ticker
-    return s
+    return s.asfreq("D")
 
 
 def get_yahoo_bulk(tickers: list = ["^GSPC"], period: str = "max") -> pd.DataFrame:
     """Download the historical adjusted closing price of multiple securities
     with ticker in the `tickers` list.
 
     Parameters
@@ -157,15 +159,15 @@
 
     Returns
     -------
     pd.DataFrame
         Time series of the prices of the securities
     """
     # Columns are already the tickers, note some securities like crypto trades in non-business days
-    return yf.download(" ".join(tickers), period=period)["Adj Close"]
+    return yf.download(" ".join(tickers), period=period)["Adj Close"].asfreq('D')
 
 
 def get_msci(
         codes: list = [990100],
         end_date: str = None,
         fx: str = "USD",
         variant: str = "STRD",
```

### Comparing `fintoolkit-0.0.8/toolkit/fixed_income.py` & `fintoolkit-0.0.9/toolkit/fixed_income.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/toolkit/functional.py` & `fintoolkit-0.0.9/toolkit/functional.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/toolkit/portfolio.py` & `fintoolkit-0.0.9/toolkit/portfolio.py`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/.gitignore` & `fintoolkit-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/README.md` & `fintoolkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fintoolkit-0.0.8/pyproject.toml` & `fintoolkit-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fintoolkit"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Chris Cheng", email="kc1116@gmail.com" },
 ]
 description = "Financial Toolkit"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fintoolkit-0.0.8/PKG-INFO` & `fintoolkit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fintoolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Financial Toolkit
 Project-URL: Homepage, https://github.com/chris-kc-cheng/financial-toolkit
 Project-URL: Bug Tracker, https://github.com/chris-kc-cheng/financial-toolkit/issues
 Author-email: Chris Cheng <kc1116@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

