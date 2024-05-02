# Comparing `tmp/fin_maestro_kin-0.2.6.tar.gz` & `tmp/fin_maestro_kin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fin_maestro_kin-0.2.6.tar", max compression
+gzip compressed data, was "fin_maestro_kin-0.3.0.tar", max compression
```

## Comparing `fin_maestro_kin-0.2.6.tar` & `fin_maestro_kin-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.6/fin_maestro_kin/__init__.py
--rw-r--r--   0        0        0     1872 2024-04-26 21:46:47.948773 fin_maestro_kin-0.2.6/fin_maestro_kin/constants.py
--rw-r--r--   0        0        0     1007 2024-04-27 07:19:02.530376 fin_maestro_kin-0.2.6/fin_maestro_kin/main.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/__init__.py
--rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 22:03:36.979909 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
--rw-r--r--   0        0        0    42792 2024-04-26 22:09:51.476037 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/nse/nse_operations.py
--rw-r--r--   0        0        0        0 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
--rw-r--r--   0        0        0     9242 2024-04-26 23:38:54.845857 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/sentiment_analysis/__init__.py
--rw-r--r--   0        0        0     3840 2024-04-27 07:12:00.425708 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/trend_detector/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-27 07:21:06.631998 fin_maestro_kin-0.2.6/fin_maestro_kin/modules/trend_detector/trend_detector.py
--rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.6/LICENSE
--rw-r--r--   0        0        0      614 2024-04-27 07:27:19.793888 fin_maestro_kin-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5508 2024-04-26 18:16:29.525503 fin_maestro_kin-0.2.6/README.md
--rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.3.0/fin_maestro_kin/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-26 21:46:47.948773 fin_maestro_kin-0.3.0/fin_maestro_kin/constants.py
+-rw-r--r--   0        0        0     1007 2024-05-01 09:03:08.466931 fin_maestro_kin-0.3.0/fin_maestro_kin/main.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/__init__.py
+-rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/data_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 22:03:36.979909 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
+-rw-r--r--   0        0        0    42790 2024-05-02 06:19:54.716683 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/data_toolkit/nse/nse_operations.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:37:31.671927 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
+-rw-r--r--   0        0        0     9242 2024-05-01 05:53:09.802944 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/sentiment_analysis/__init__.py
+-rw-r--r--   0        0        0     4777 2024-05-01 11:38:57.424919 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/trend_detector/__init__.py
+-rw-r--r--   0        0        0     2263 2024-05-01 05:53:10.439789 fin_maestro_kin-0.3.0/fin_maestro_kin/modules/trend_detector/trend_detector.py
+-rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.3.0/LICENSE
+-rw-r--r--   0        0        0      632 2024-05-02 07:07:58.141011 fin_maestro_kin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5508 2024-04-26 18:16:29.525503 fin_maestro_kin-0.3.0/README.md
+-rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 fin_maestro_kin-0.3.0/PKG-INFO
```

### Comparing `fin_maestro_kin-0.2.6/fin_maestro_kin/constants.py` & `fin_maestro_kin-0.3.0/fin_maestro_kin/constants.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.6/fin_maestro_kin/main.py` & `fin_maestro_kin-0.3.0/fin_maestro_kin/main.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/nse/nse_operations.py` & `fin_maestro_kin-0.3.0/fin_maestro_kin/modules/data_toolkit/nse/nse_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
             raise HTTPException(status_code=500, detail=f"Error fetching historical data: {e}")
         
     def index_pe_pb_div(self, symbol, start_date, end_date):
         start_date = datetime.datetime.strptime(start_date, "%d-%b-%Y").strftime("%d %b %Y")
         end_date = datetime.datetime.strptime(end_date, "%d-%b-%Y").strftime("%d %b %Y")
         
         data = {"cinfo": f"{{'name':'{symbol}','startDate':'{start_date}','endDate':'{end_date}'}}"}
-        payload = requests.post('https://niftyindices.com/Backpage.aspx/getpepbHistoricaldataDBtoString', headers=self.niftyindices_headers,  json=data).json()
+        payload = requests.post('https://niftyindices.com/Backpage.aspx/getpepbHistoricaldataDBtoString', headers=self.niftyindices_headers, json=data).json()
         payload = json.loads(payload["d"])
         
         if not payload:
             raise HTTPException(status_code=404, detail="No historical data found.")
         
         payload=pd.DataFrame.from_records(payload)
         return payload
@@ -399,15 +399,15 @@
             raise HTTPException(status_code=500, detail=f"Error fetching historical ratios data: {e}")
         
     def index_total_returns(self, symbol,start_date,end_date):
         start_date = datetime.datetime.strptime(start_date, "%d-%b-%Y").strftime("%d %b %Y")
         end_date = datetime.datetime.strptime(end_date, "%d-%b-%Y").strftime("%d %b %Y")
         
         data = {"cinfo": f"{{'name':'{symbol}','startDate':'{start_date}','endDate':'{end_date}'}}"}
-        payload = requests.post('https://niftyindices.com/Backpage.aspx/getTotalReturnIndexString', headers=self.niftyindices_headers,  json=data).json()
+        payload = requests.post('https://niftyindices.com/Backpage.aspx/getTotalReturnIndexString', headers=self.niftyindices_headers, json=data).json()
         payload = json.loads(payload["d"])
         
         if not payload:
             raise HTTPException(status_code=404, detail="No historical data found.")
         
         payload=pd.DataFrame.from_records(payload)
         return payload
```

### Comparing `fin_maestro_kin-0.2.6/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py` & `fin_maestro_kin-0.3.0/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.6/fin_maestro_kin/modules/trend_detector/trend_detector.py` & `fin_maestro_kin-0.3.0/fin_maestro_kin/modules/trend_detector/trend_detector.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.6/LICENSE` & `fin_maestro_kin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.6/pyproject.toml` & `fin_maestro_kin-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fin-maestro-kin"
-version = "0.2.6"
+version = "0.3.0"
 description = "Seamless Finance: Docker Deployed APIs for Smart Investments."
 authors = ["DEV_FINWIZ <devjuneja43@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -13,14 +13,15 @@
 pydantic = "^2.5.3"
 requests = "^2.31.0"
 yfinance = "^0.2.35"
 matplotlib = "^3.8.2"
 pandas = "^2.1.4"
 numpy = "^1.26.3"
 beautifulsoup4 = "^4.12.3"
+redis = "^5.0.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fin_maestro_kin-0.2.6/README.md` & `fin_maestro_kin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.6/PKG-INFO` & `fin_maestro_kin-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fin-maestro-kin
-Version: 0.2.6
+Version: 0.3.0
 Summary: Seamless Finance: Docker Deployed APIs for Smart Investments.
 License: MIT
 Author: DEV_FINWIZ
 Author-email: devjuneja43@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: redis (>=5.0.4,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.25.0,<0.26.0)
 Requires-Dist: yfinance (>=0.2.35,<0.3.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://fin-maestro-kin.apidog.io/"><img src="https://github.com/devfinwiz/Fin-Maestro-Kin/assets/78873223/eb0f030e-5c6c-4457-9713-97d0487ae59c" alt="Fin Maestro Kin"></a>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.6 Summary: Seamless
+Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.3.0 Summary: Seamless
 Finance: Docker Deployed APIs for Smart Investments. License: MIT Author:
 DEV_FINWIZ Author-email: devjuneja43@gmail.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) Requires-Dist: fastapi
 (>=0.109.0,<0.110.0) Requires-Dist: matplotlib (>=3.8.2,<4.0.0) Requires-Dist:
 numpy (>=1.26.3,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist:
-pydantic (>=2.5.3,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
-Dist: uvicorn (>=0.25.0,<0.26.0) Requires-Dist: yfinance (>=0.2.35,<0.3.0)
-Description-Content-Type: text/markdown
+pydantic (>=2.5.3,<3.0.0) Requires-Dist: redis (>=5.0.4,<6.0.0) Requires-Dist:
+requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn (>=0.25.0,<0.26.0) Requires-
+Dist: yfinance (>=0.2.35,<0.3.0) Description-Content-Type: text/markdown
                                _[_F_i_n_ _M_a_e_s_t_r_o_ _K_i_n_]
          SSeeaammlleessss FFiinnaannccee:: DDoocckkeerr--DDeeppllooyyeedd AAPPIIss ffoorr SSmmaarrtt IInnvveessttmmeennttss..
                          ************ FFiinn--MMaaeessttrroo--KKiinn ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_d_e_v_f_i_n_w_i_z_/_f_i_n_-_m_a_e_s_t_r_o_-_k_i_n_?_s_t_y_l_e_=_f_o_r_-
    _t_h_e_-_b_a_d_g_e_][https://img.shields.io/badge/Python-3.9.1-blue&?style=for-the-
 badge&color=brown]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-
      _K_i_n_?_c_o_l_o_r_=_p_u_r_p_l_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
```

