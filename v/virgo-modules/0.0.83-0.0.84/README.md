# Comparing `tmp/virgo_modules-0.0.83.tar.gz` & `tmp/virgo_modules-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.83.tar", last modified: Sat Apr 27 12:42:06 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.84.tar", last modified: Thu May  2 07:45:51 2024, max compression
```

## Comparing `virgo_modules-0.0.83.tar` & `virgo_modules-0.0.84.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.508839 virgo_modules-0.0.83/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.83/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-27 12:42:06.506838 virgo_modules-0.0.83/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.83/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 12:42:06.509840 virgo_modules-0.0.83/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-27 12:41:59.000000 virgo_modules-0.0.83/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.390043 virgo_modules-0.0.83/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.420221 virgo_modules-0.0.83/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.493450 virgo_modules-0.0.83/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    71652 2024-04-27 12:41:59.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   144162 2024-04-20 13:56:03.000000 virgo_modules-0.0.83/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-27 12:42:06.468445 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-27 12:42:05.000000 virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.564259 virgo_modules-0.0.84/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.84/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-05-02 07:45:51.555098 virgo_modules-0.0.84/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.84/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 07:45:51.565260 virgo_modules-0.0.84/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-05-02 07:45:11.000000 virgo_modules-0.0.84/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.460379 virgo_modules-0.0.84/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.496394 virgo_modules-0.0.84/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.550093 virgo_modules-0.0.84/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    71652 2024-04-27 12:41:59.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.84/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:45:51.521894 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-02 07:45:50.000000 virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.83/LICENSE` & `virgo_modules-0.0.84/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.83/PKG-INFO` & `virgo_modules-0.0.84/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.83
+Version: 0.0.84
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.83/setup.py` & `virgo_modules-0.0.84/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.83",
+    version="0.0.84",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.83/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.84/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.83/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.84/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.83/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.84/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.83/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.84/virgo_app/virgo_modules/src/re_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.83/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.84/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
 from feature_engine.encoding import OneHotEncoder
 from feature_engine.selection import DropFeatures, DropCorrelatedFeatures
 from feature_engine.timeseries.forecasting import LagFeatures
 from feature_engine.imputation import MeanMedianImputer
 from feature_engine.discretisation import EqualWidthDiscretiser
 
+from sklearn.linear_model import HuberRegressor
+
 from .aws_utils import upload_file_to_aws
 
 import logging
 
 class InverseHyperbolicSine(BaseEstimator, TransformerMixin):
 
     """
@@ -3066,18 +3068,18 @@
 
 class analyse_index(stock_eda_panel):
     """
     class that is going to train hmm models to perform feature selection
 
     Attributes
     ----------
-    data  : pd.DataFrame
-        symbol of the asset
-    index : str
+    data_index : pd.DataFrame
          name of the index
+    indexes: list
+        list of indexes
     asset : str
          name of the asset
     n_obs : int
          number of rows to extract
     lag : int
          lag to apply
     data_window : str
@@ -3100,253 +3102,209 @@
     process_data():
         using stock_eda_panel, get data and merge data
     plot_betas(sample_size=int, offset=int, subsample_ts=int):
         display beta analysis plot
     get_betas(subsample_ts=int)
         get general beta and last sample beta, correlation score is included too
     """
-
-    def __init__(self, index, asset, n_obs, lag, data_window = '5y', show_plot = True, save_path = False, save_aws = False, aws_credentials = False):
+    def __init__(self, index_data, asset, n_obs, lag, data_window = '5y', show_plot = False, save_path = False, save_aws = False, aws_credentials = False, return_fig = False):
         """
         Initialize object
 
         Parameters
         ----------
-        index (str): name of the index
+        index_data (pd.DataFrame or str): index data dataframe or index string
         asset (str): name of the asset
         n_obs (int): number of rows to extract
         lag (int): lag to apply
         data_window (str): 5y 10y 15y
         show_plot (bool): If True, show plots
         save_path (str): local path for saving e.g r'C:/path/to/the/file/'
         save_aws (str): remote key in s3 bucket path e.g. 'path/to/file/'
         aws_credentials (dict): dict with the aws credentials
 
         Returns
         -------
         None
         """
 
-        self.index = index
+        
+        if type(index_data) != str:
+            index_data['Date'] = pd.to_datetime(index_data['Date'])
+            self.index_data = index_data
+            self.indexes = [ x for x in list(index_data.columns) if x != 'Date']
+        else:
+            self.indexes = [index_data]
+            
+        self.index_data = index_data
         self.asset = asset
         self.n_obs = n_obs
         self.data_window = data_window
         self.lag = lag
 
         self.show_plot = show_plot
+        self.return_fig = return_fig
         self.save_path = save_path
         self.save_aws = save_aws
 
     def process_data(self):
         """
         using stock_eda_panel, get data and merge data
-
+    
         Parameters
         ----------
         None
-
+    
         Returns
         -------
         None
         """
-        index = stock_eda_panel(self.index, self.n_obs, self.data_window)
-        index.get_data()
-        index.df['shift'] = index.df.Close.shift(self.lag)
-        index.df['index_return'] = index.df.Close/index.df['shift'] - 1
-
-        asset =  stock_eda_panel(self.asset, self.n_obs, self.data_window)
+        asset =  stock_eda_panel(self.asset, self.n_obs, data_window=self.data_window)
         asset.get_data()
-        asset.df['shift'] = asset.df.Close.shift(self.lag)
-        asset.df['asset_return'] = asset.df.Close/asset.df['shift'] - 1
-
-        df1 = index.df[['Date','index_return']]
-        df2 = asset.df[['Date','asset_return','Close']]
-        merger = df1.merge(df2, on = 'Date', how = 'inner')
-        merger.dropna(inplace = True)
-        self.merger_df = merger
+        df = asset.df[['Date','Close']]
+        
+        if type(self.index_data) != str:
+            df_merge = df.merge(self.index_data, on = ['Date'], how = 'left').sort_values('Date')
+            
+        else:
+            indx =  stock_eda_panel(self.index_data, self.n_obs, data_window=self.data_window)
+            indx.get_data()
+            indx_df = indx.df[['Date','Close']].rename(columns = {'Close':self.index_data})
+            df_merge = df.merge(indx_df, on = ['Date'], how = 'left').sort_values('Date')
+            
+        for colx in ['Close'] + self.indexes:
+            df_merge[f'{colx}_pct'] = df_merge[colx]/df_merge[colx].shift(self.lag) - 1
+            
+        df_merge.dropna(inplace = True)
+        self.merger_df = df_merge.rename(columns = {'Close_pct': 'asset_return'})
 
-    def plot_betas(self,sample_size, offset, subsample_ts =False):
+    def plot_betas(self,sample_size, offset, subsample_ts =False, index = False):
         """
         display beta analysis plot
 
         Parameters
         ----------
         sample_size (int): number of days or window size to calculate beta
         offset (int): overlap between windows
         subsample_ts (int): subsample size of data 
 
         Returns
         -------
         None
         """
-        ### extracting data
-
-        self.process_data()
-
-         ### ploting analysis
+        if (type(self.index_data) == str) & (index != False):
+            raise Exception("No need of index argument")
+        else:
+            index = self.indexes[0]
+            
+        index_pct = f'{index}_pct'
+        ### ploting analysis
         figure, ax = plt.subplot_mosaic(
             [["scatter_total", "scatter_sample",'ts','ts']],
             layout="constrained",
             figsize=(18, 5)
         )
 
-        ax['scatter_total'].scatter(self.merger_df.asset_return, self.merger_df.index_return)
-        b, a = np.polyfit(self.merger_df.asset_return, self.merger_df.index_return, 1)
+        ax['scatter_total'].scatter(self.merger_df.asset_return, self.merger_df[index_pct])
+    
+        huber_regr = HuberRegressor(fit_intercept = True)
+        huber_regr.fit(self.merger_df.asset_return.values.reshape(-1,1), self.merger_df[index_pct].values.reshape(-1,1))
+        b, a = huber_regr.coef_[0], huber_regr.intercept_
+    
+        # b, a = np.polyfit(self.merger_df.asset_return, self.merger_df[index_pct], 1)
         ax['scatter_total'].plot(self.merger_df.asset_return, b*self.merger_df.asset_return+a, color='red')
 
         ax['ts'].plot(self.merger_df.Date, self.merger_df.Close, color = 'grey', alpha = 0.3)
 
         if subsample_ts:
             self.merger_df = self.merger_df.iloc[-subsample_ts:,:].dropna()
 
         for i in range(0,len(self.merger_df)-sample_size,offset):
 
             merger_ = self.merger_df.sort_values('Date', ascending = False).iloc[i:i+sample_size,:]
-            x = merger_.index_return
+            x = merger_[index_pct]
             y = merger_.asset_return
-            b, a = np.polyfit(x,y, 1)
-
+            # b, a = np.polyfit(x,y, 1)
+            huber_regr = HuberRegressor(fit_intercept = True)
+            huber_regr.fit(x.values.reshape(-1,1), y.values.reshape(-1,1))
+            b, a = huber_regr.coef_[0], huber_regr.intercept_
+            
             normalize = mcolors.Normalize(vmin=-1, vmax=1)
             colormap = cm.jet
 
             ax['scatter_sample'].plot(x, y,'o', color = 'blue', alpha = 0.1)
             ax['scatter_sample'].plot(x, b*x+a, color=colormap(normalize(b)))
             ax['scatter_sample'].set_xlim(-0.06, 0.06)
             ax['scatter_sample'].set_ylim(-0.06, 0.06)
 
             plot = ax['ts'].scatter(merger_.Date, merger_.Close, color=colormap(normalize(b)), s = 10)
 
         scalarmappaple = cm.ScalarMappable(norm=normalize, cmap=colormap)
         scalarmappaple.set_array(x)
 
-        plt.title(f'{self.asset} using index: {self.index}')
+        plt.title(f'{self.asset} using index: {index}')
         plt.colorbar(scalarmappaple)
 
         if self.show_plot:
             plt.show()
+            
         if self.save_path:
             result_plot_name = f'market_best_fit.png'
             figure.savefig(self.save_path+result_plot_name)
 
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.asset}/'+result_plot_name,input_path = self.save_path+result_plot_name)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_plot_name, input_path = self.save_path + result_plot_name, aws_credentials = self.aws_credentials)
+            
         if not self.show_plot:
-            plt.close()
-
+            plt.close() 
+            
+        if self.return_fig:
+            return figure
+            
     def get_betas(self,subsample_ts=False):
         """
         get general beta and last sample beta, correlation score is included too
-
+    
         Parameters
         ----------
         subsample_ts (int): subsample size of data 
-
-        Returns
-        -------
-        None
-        """
-        self.process_data()
-        general_beta, a = np.polyfit(self.merger_df.asset_return, self.merger_df.index_return, 1)
-        general_r = stats.mstats.pearsonr(self.merger_df.asset_return, self.merger_df.index_return)[0]
-
-        self.process_data()
-        if subsample_ts:
-            self.merger_df = self.merger_df.iloc[-subsample_ts:,:].dropna()
-        sample_beta, a = np.polyfit(self.merger_df.asset_return, self.merger_df.index_return, 1)
-        sample_r = stats.mstats.pearsonr(self.merger_df.asset_return, self.merger_df.index_return)[0]
-
-        result = {
-            'general_beta':general_beta,
-            'general_r':general_r,
-            'sample_beta':sample_beta,
-            'sample_r':sample_r
-        }
-
-        self.states_result = result
-
-class evaluate_markets(analyse_index):
-    """
-    object that is going to evaluate multiple indexes
-
-    Attributes
-    ----------
-    stock_code : str
-        asset to assess
-    indexes : list
-        list of indexes
-    best_result : dict
-        best result beta and correlation
-
-    Methods
-    -------
-    process_data():
-        using stock_eda_panel, get data and merge data
-    plot_betas(sample_size=int, offset=int, subsample_ts=int):
-        display beta analysis plot
-    get_betas(subsample_ts=int)
-        get general beta and last sample beta, correlation score is included too
-    evaluate_best_market_fit(sample_size=int, offset=int,lag=int, n_obs=int, verbose=boolean, plot_best=boolean):
-        iterate every index in the index list and get results
-    """
-
-    def __init__(self, stock_code, indexes):
-        """
-        Initialize object
-
-        Parameters
-        ----------
-        stock_code  (str): asset to assess
-        indexes (list): list of indexes
-
+    
         Returns
         -------
         None
         """
-        self.stock_code = stock_code
-        self.indexes = indexes
-    def evaluate_best_market_fit(self,sample_size, offset,lag= 3, n_obs = 3500, verbose = False, plot_best = False):
-        """
-        iterate every index in the index list and get results
-
-        Parameters
-        ----------
-        sample_size (int): sample size to get betas
-        offset (int): overlap size
-        lag (int): number of lags of the returns
-        n_obs (int): number of observations of the data extraction
-        verbose (boolean): if true, print results
-        plot_best (boolean): if true, display plot of the best result
-
-        Returns
-        -------
-        None
-        """
-        results_dicts = dict()
+        result = list()
         for index in self.indexes:
-            betex = analyse_index(index = index,asset = self.stock_code,n_obs = n_obs, lag = lag)
-            betex.get_betas(sample_size)
-            results_dicts[index] = betex.states_result
-        pd_result = pd.DataFrame(results_dicts).T
-        pd_result['gen_r2'] = pd_result.general_r ** 2
-        pd_result['sampl_r2'] = pd_result.sample_r ** 2
-        self.stat_results = pd_result
-
-        best_result = pd_result.sort_values('gen_r2',ascending = False).head(2).sort_values('sampl_r2',ascending = False).head(1)
-        best_fit_index = best_result.index.values[0]
-
-        self.stat_results = self.stat_results.drop(columns = ['gen_r2','sampl_r2'])
-
-        if verbose:
-            print(best_result)
-        if plot_best:
-            betex = analyse_index(index = best_fit_index,asset = self.stock_code, n_obs = n_obs, lag = lag)
-            betex.plot_betas(sample_size = sample_size, offset = offset, subsample_ts = False)
+            
+            index_pct = f'{index}_pct'
+            huber_regr = HuberRegressor(fit_intercept = True)
+            huber_regr.fit(self.merger_df.asset_return.values.reshape(-1,1), self.merger_df[index_pct].values.reshape(-1,1))
+            general_beta, a = huber_regr.coef_[0], huber_regr.intercept_
+            general_r = stats.mstats.pearsonr(self.merger_df.asset_return, self.merger_df[index])[0]
+
+            dict_res = {
+                    'index':index,
+                    'general_beta':general_beta,
+                    'general_r':general_r,
+                }
+    
+            if subsample_ts:
+                tmp_df = self.merger_df.iloc[-subsample_ts:,:].dropna()
+                huber_regr = HuberRegressor(fit_intercept = True)
+                huber_regr.fit(tmp_df.asset_return.values.reshape(-1,1), tmp_df[index_pct].values.reshape(-1,1))
+                sample_beta, a = huber_regr.coef_[0], huber_regr.intercept_
+                sample_r = stats.mstats.pearsonr(tmp_df.asset_return, tmp_df[index])[0]
+                dict_res['sample_beta'] = sample_beta
+                dict_res['sample_r'] = sample_r
+                
+            result.append(dict_res)
+    
+        self.states_result = result
 
-        self.best_result = best_result
 
 def get_relevant_beta(data_market, ticket_name,  show_plot = True, save_path = False, save_aws = False, aws_credentials = False):
     '''
     select relevant beta result data of a given asset
 
             Parameters:
                     data_market (pd.DataFrame): dataframe of the market results
```

### Comparing `virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.83
+Version: 0.0.84
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.83/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.84/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

