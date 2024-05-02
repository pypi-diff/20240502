# Comparing `tmp/pyqqq-0.8.9.tar.gz` & `tmp/pyqqq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.8.9.tar", max compression
+gzip compressed data, was "pyqqq-0.9.0.tar", max compression
```

## Comparing `pyqqq-0.8.9.tar` & `pyqqq-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.8.9/README.md
--rw-r--r--   0        0        0      769 2024-04-29 05:38:30.660303 pyqqq-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      668 2024-04-16 05:13:25.694767 pyqqq-0.8.9/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.8.9/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.8.9/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    41866 2024-04-26 06:58:08.897413 pyqqq-0.8.9/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.8.9/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.8.9/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.8.9/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.8.9/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.8.9/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.8.9/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.8.9/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.8.9/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.8.9/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.8.9/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.8.9/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6717 2024-04-23 09:10:34.476708 pyqqq-0.8.9/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     8856 2024-04-29 05:35:42.398052 pyqqq-0.8.9/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.8.9/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4230 2024-04-22 04:52:35.362865 pyqqq-0.8.9/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.8.9/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.8.9/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.8.9/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.8.9/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.8.9/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3235 2024-04-23 09:07:35.908506 pyqqq-0.8.9/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.8.9/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.8.9/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.8.9/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.8.9/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.8.9/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.8.9/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.8.9/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 pyqqq-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.0/README.md
+-rw-r--r--   0        0        0      791 2024-05-02 09:31:16.839861 pyqqq-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.0/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.0/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.0/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    41866 2024-04-26 06:58:08.897413 pyqqq-0.9.0/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.0/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.0/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.0/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.0/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.9.0/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.0/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.0/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.0/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.0/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.0/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.0/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6717 2024-04-30 07:00:37.173273 pyqqq-0.9.0/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     9312 2024-05-02 09:25:25.974592 pyqqq-0.9.0/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.9.0/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4230 2024-04-22 04:52:35.362865 pyqqq-0.9.0/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.0/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.0/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.0/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.0/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.0/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.0/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.0/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.0/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.0/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.0/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.0/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.0/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.0/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.0/PKG-INFO
```

### Comparing `pyqqq-0.8.9/README.md` & `pyqqq-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyproject.toml` & `pyqqq-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.8.9"
+version = "0.9.0"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
@@ -13,18 +13,19 @@
 tinydb = "^4.8.0"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
 websockets = "^12.0"
 pandas = "^2.0.3"
 cssutils = "^2.10.2"
 cachetools = "^5.3.3"
+sphinx = "^7.3.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 sphinx = "^7.2.6"
 myst-parser = "^2.0.0"
-sphinx-rtd-theme = "^2.0.0"
 ipykernel = "^6.29.4"
+pydata-sphinx-theme = "^0.15.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.9.0/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.9.0/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.9.0/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.9.0/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.9.0/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.9.0/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.9.0/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.9.0/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.9.0/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/data/domestic.py` & `pyqqq-0.9.0/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/data/minutes.py` & `pyqqq-0.9.0/pyqqq/data/minutes.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,34 @@
     for data in rows:
         time = data["time"].replace("Z", "+00:00")
         time = dtm.datetime.fromisoformat(time).astimezone(tz).replace(tzinfo=None)
         data["time"] = time
 
     df = pd.DataFrame(rows)
     if not df.empty:
+        dtypes = df.dtypes
+
+        for k in [
+            "open",
+            "high",
+            "low",
+            "close",
+            "volume",
+            "change",
+            "totofferrem",
+            "totbidrem",
+        ]:
+            if k in dtypes:
+                dtypes[k] = np.dtype("int64")
+
+        for k in ["diff", "chdegree"]:
+            if k in dtypes:
+                dtypes[k] = np.dtype("float64")
+
+        df = df.astype(dtypes)
         df.set_index("code", inplace=True)
 
     return df
 
 
 def get_all_day_data(
     date: dtm.date,
```

### Comparing `pyqqq-0.8.9/pyqqq/data/realtime.py` & `pyqqq-0.9.0/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/data/ticks.py` & `pyqqq-0.9.0/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/datatypes.py` & `pyqqq-0.9.0/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/executors/hook.py` & `pyqqq-0.9.0/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/utils/compute.py` & `pyqqq-0.9.0/pyqqq/utils/compute.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         etf_etn (bool): 가격이 ETF 또는 ETN 상품인 경우 True, 그 외는 False.
         rounding (str, optional): 반올림 방식('round', 'ceil', 'floor'). 기본값은 'floor'.
 
     Returns:
         int: 반올림된 가격.
 
     Raises:
-        ValueError: `rounding`이 지정된 세 가지 옵션 중 하나가 아닐 경우 오류를 발생시킵니다.
+        ValueError: rounding이 지정된 세 가지 옵션 중 하나가 아닐 경우 오류를 발생시킵니다.
 
     Examples:
         >>> quantize_krx_price(Decimal('1520.75'), False, 'round')
         1521
         >>> quantize_krx_price(Decimal('1520.75'), True, 'ceil')
         1521
         >>> quantize_krx_price(Decimal('1520.75'), False, 'floor')
@@ -51,25 +51,25 @@
 
 
 def get_krx_tick_size(price: float, etf_etn: bool) -> int:
     """
     주어진 가격과 금융 상품 유형에 따라 적절한 틱 사이즈를 반환합니다.
 
     한국거래소(KRX)의 틱 사이즈 규칙에 따라, 특정 가격대의 주식 또는 ETF/ETN의 최소 가격 변동 단위(틱 사이즈)를 결정합니다.
-    입력된 `price`가 각 가격대의 최소값 미만일 경우 해당하는 틱 사이즈를 반환하며, 모든 조건에 부합하지 않는 경우 최대 가격을 반환합니다.
+    입력된 price가 각 가격대의 최소값 미만일 경우 해당하는 틱 사이즈를 반환하며, 모든 조건에 부합하지 않는 경우 최대 가격을 반환합니다.
 
     Args:
         price (float): 상품의 가격.
         etf_etn (bool): 상품이 ETF 또는 ETN인 경우 True, 아니면 False.
 
     Returns:
         int: 결정된 틱 사이즈.
 
     Raises:
-        AssertionError: `price`가 0 이하일 경우 오류를 발생시킵니다.
+        AssertionError: price가 0 이하일 경우 오류를 발생시킵니다.
 
     Examples:
         >>> get_krx_tick_size(1500, False)
         1
         >>> get_krx_tick_size(2500, False)
         5
         >>> get_krx_tick_size(2500, True)
```

### Comparing `pyqqq-0.8.9/pyqqq/utils/display.py` & `pyqqq-0.9.0/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/utils/kvstore.py` & `pyqqq-0.9.0/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/utils/market_schedule.py` & `pyqqq-0.9.0/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/pyqqq/utils/mock_api.py` & `pyqqq-0.9.0/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.9/PKG-INFO` & `pyqqq-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.8.9
+Version: 0.9.0
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (>=5.3.3,<6.0.0)
 Requires-Dist: cssutils (>=2.10.2,<3.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sphinx (>=7.3.7,<8.0.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
 
 # PyQQQ SDK
```

