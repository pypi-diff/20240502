# Comparing `tmp/py_replay_bg-0.0.8.tar.gz` & `tmp/py_replay_bg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_replay_bg-0.0.8.tar", last modified: Wed Mar 20 12:49:22 2024, max compression
+gzip compressed data, was "py_replay_bg-0.0.9.tar", last modified: Thu Mar 28 14:27:33 2024, max compression
```

## Comparing `py_replay_bg-0.0.8.tar` & `py_replay_bg-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.992140 py_replay_bg-0.0.8/
--rwx------   0 cappe      (501) staff       (20)    35149 2023-09-05 13:43:30.000000 py_replay_bg-0.0.8/COPYING.md
--rw-r--r--   0 cappe      (501) staff       (20)     3720 2024-03-20 12:49:22.991974 py_replay_bg-0.0.8/PKG-INFO
--rwx------   0 cappe      (501) staff       (20)     1006 2023-09-05 13:43:30.000000 py_replay_bg-0.0.8/README.md
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.987872 py_replay_bg-0.0.8/py_replay_bg/
--rwx------   0 cappe      (501) staff       (20)        0 2023-05-25 12:10:33.000000 py_replay_bg-0.0.8/py_replay_bg/__init__.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.988565 py_replay_bg-0.0.8/py_replay_bg/data/
--rwx------   0 cappe      (501) staff       (20)    10457 2024-01-17 13:08:33.000000 py_replay_bg-0.0.8/py_replay_bg/data/__init__.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.989156 py_replay_bg-0.0.8/py_replay_bg/dss/
--rwx------   0 cappe      (501) staff       (20)     7811 2024-01-17 13:25:46.000000 py_replay_bg-0.0.8/py_replay_bg/dss/__init__.py
--rwx------   0 cappe      (501) staff       (20)    18438 2024-01-15 09:05:00.000000 py_replay_bg-0.0.8/py_replay_bg/dss/default_dss_handlers.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.989558 py_replay_bg-0.0.8/py_replay_bg/environment/
--rwx------   0 cappe      (501) staff       (20)     8300 2024-01-18 15:09:53.000000 py_replay_bg-0.0.8/py_replay_bg/environment/__init__.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.986343 py_replay_bg-0.0.8/py_replay_bg/example/
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.989849 py_replay_bg-0.0.8/py_replay_bg/example/code/
--rw-r--r--   0 cappe      (501) staff       (20)     1432 2024-01-29 14:02:01.000000 py_replay_bg-0.0.8/py_replay_bg/example/code/quick-start.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.990165 py_replay_bg-0.0.8/py_replay_bg/identification/
--rwx------   0 cappe      (501) staff       (20)        0 2023-06-13 15:43:37.000000 py_replay_bg-0.0.8/py_replay_bg/identification/__init__.py
--rwx------   0 cappe      (501) staff       (20)    23841 2024-03-14 11:33:05.000000 py_replay_bg-0.0.8/py_replay_bg/identification/mcmc.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.990291 py_replay_bg-0.0.8/py_replay_bg/input_validation/
--rwx------   0 cappe      (501) staff       (20)    24364 2024-03-20 12:25:44.000000 py_replay_bg-0.0.8/py_replay_bg/input_validation/__init__.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.990513 py_replay_bg-0.0.8/py_replay_bg/model/
--rwx------   0 cappe      (501) staff       (20)        0 2023-06-11 09:14:18.000000 py_replay_bg-0.0.8/py_replay_bg/model/__init__.py
--rwx------   0 cappe      (501) staff       (20)    55448 2024-03-20 12:18:09.000000 py_replay_bg-0.0.8/py_replay_bg/model/t1d_model.py
--rwx------   0 cappe      (501) staff       (20)    40045 2024-03-20 12:22:48.000000 py_replay_bg-0.0.8/py_replay_bg/py_replay_bg.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.990667 py_replay_bg-0.0.8/py_replay_bg/replay/
--rwx------   0 cappe      (501) staff       (20)     6047 2024-03-14 11:39:55.000000 py_replay_bg-0.0.8/py_replay_bg/replay/__init__.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.990804 py_replay_bg-0.0.8/py_replay_bg/sensors/
--rwx------   0 cappe      (501) staff       (20)     8207 2024-01-15 08:20:04.000000 py_replay_bg-0.0.8/py_replay_bg/sensors/__init__.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.991074 py_replay_bg-0.0.8/py_replay_bg/tests/
--rwx------   0 cappe      (501) staff       (20)        0 2023-05-25 12:28:05.000000 py_replay_bg-0.0.8/py_replay_bg/tests/__init__.py
--rwx------   0 cappe      (501) staff       (20)     1565 2024-03-20 12:46:11.000000 py_replay_bg-0.0.8/py_replay_bg/tests/test_replay_bg.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.991301 py_replay_bg-0.0.8/py_replay_bg/utils/
--rwx------   0 cappe      (501) staff       (20)        0 2023-09-21 11:06:08.000000 py_replay_bg-0.0.8/py_replay_bg/utils/__init__.py
--rwx------   0 cappe      (501) staff       (20)     2294 2024-01-15 08:30:23.000000 py_replay_bg-0.0.8/py_replay_bg/utils/stats.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.991425 py_replay_bg-0.0.8/py_replay_bg/visualizer/
--rwx------   0 cappe      (501) staff       (20)     7714 2024-01-15 08:34:43.000000 py_replay_bg-0.0.8/py_replay_bg/visualizer/__init__.py
-drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-20 12:49:22.991740 py_replay_bg-0.0.8/py_replay_bg.egg-info/
--rw-r--r--   0 cappe      (501) staff       (20)     3720 2024-03-20 12:49:22.000000 py_replay_bg-0.0.8/py_replay_bg.egg-info/PKG-INFO
--rw-r--r--   0 cappe      (501) staff       (20)      872 2024-03-20 12:49:22.000000 py_replay_bg-0.0.8/py_replay_bg.egg-info/SOURCES.txt
--rw-r--r--   0 cappe      (501) staff       (20)        1 2024-03-20 12:49:22.000000 py_replay_bg-0.0.8/py_replay_bg.egg-info/dependency_links.txt
--rw-r--r--   0 cappe      (501) staff       (20)     1070 2024-03-20 12:49:22.000000 py_replay_bg-0.0.8/py_replay_bg.egg-info/requires.txt
--rw-r--r--   0 cappe      (501) staff       (20)       13 2024-03-20 12:49:22.000000 py_replay_bg-0.0.8/py_replay_bg.egg-info/top_level.txt
--rwx------   0 cappe      (501) staff       (20)     1000 2024-03-20 12:47:10.000000 py_replay_bg-0.0.8/pyproject.toml
--rwx------   0 cappe      (501) staff       (20)     1070 2024-01-18 15:37:09.000000 py_replay_bg-0.0.8/requirements.txt
--rw-r--r--   0 cappe      (501) staff       (20)       38 2024-03-20 12:49:22.992171 py_replay_bg-0.0.8/setup.cfg
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.635393 py_replay_bg-0.0.9/
+-rwx------   0 cappe      (501) staff       (20)    35149 2023-09-05 13:43:30.000000 py_replay_bg-0.0.9/COPYING.md
+-rw-r--r--   0 cappe      (501) staff       (20)     4556 2024-03-28 14:27:33.635247 py_replay_bg-0.0.9/PKG-INFO
+-rwx------   0 cappe      (501) staff       (20)     1006 2023-09-05 13:43:30.000000 py_replay_bg-0.0.9/README.md
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.630617 py_replay_bg-0.0.9/py_replay_bg/
+-rwx------   0 cappe      (501) staff       (20)        0 2023-05-25 12:10:33.000000 py_replay_bg-0.0.9/py_replay_bg/__init__.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.631384 py_replay_bg-0.0.9/py_replay_bg/data/
+-rwx------   0 cappe      (501) staff       (20)    10457 2024-01-17 13:08:33.000000 py_replay_bg-0.0.9/py_replay_bg/data/__init__.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.632004 py_replay_bg-0.0.9/py_replay_bg/dss/
+-rwx------   0 cappe      (501) staff       (20)     7811 2024-01-17 13:25:46.000000 py_replay_bg-0.0.9/py_replay_bg/dss/__init__.py
+-rwx------   0 cappe      (501) staff       (20)    18438 2024-01-15 09:05:00.000000 py_replay_bg-0.0.9/py_replay_bg/dss/default_dss_handlers.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.632433 py_replay_bg-0.0.9/py_replay_bg/environment/
+-rwx------   0 cappe      (501) staff       (20)     8300 2024-01-18 15:09:53.000000 py_replay_bg-0.0.9/py_replay_bg/environment/__init__.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.629099 py_replay_bg-0.0.9/py_replay_bg/example/
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.632760 py_replay_bg-0.0.9/py_replay_bg/example/code/
+-rw-r--r--   0 cappe      (501) staff       (20)     1432 2024-01-29 14:02:01.000000 py_replay_bg-0.0.9/py_replay_bg/example/code/quick-start.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.633084 py_replay_bg-0.0.9/py_replay_bg/identification/
+-rwx------   0 cappe      (501) staff       (20)        0 2023-06-13 15:43:37.000000 py_replay_bg-0.0.9/py_replay_bg/identification/__init__.py
+-rwxr-xr-x   0 cappe      (501) staff       (20)    23872 2024-03-28 13:58:47.000000 py_replay_bg-0.0.9/py_replay_bg/identification/mcmc.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.633203 py_replay_bg-0.0.9/py_replay_bg/input_validation/
+-rwx------   0 cappe      (501) staff       (20)    24364 2024-03-20 12:25:44.000000 py_replay_bg-0.0.9/py_replay_bg/input_validation/__init__.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.633674 py_replay_bg-0.0.9/py_replay_bg/model/
+-rwx------   0 cappe      (501) staff       (20)        0 2023-06-11 09:14:18.000000 py_replay_bg-0.0.9/py_replay_bg/model/__init__.py
+-rwx------   0 cappe      (501) staff       (20)    55448 2024-03-20 12:18:09.000000 py_replay_bg-0.0.9/py_replay_bg/model/t1d_model.py
+-rwx------   0 cappe      (501) staff       (20)    40046 2024-03-28 13:52:51.000000 py_replay_bg-0.0.9/py_replay_bg/py_replay_bg.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.633809 py_replay_bg-0.0.9/py_replay_bg/replay/
+-rwx------   0 cappe      (501) staff       (20)     6047 2024-03-14 11:39:55.000000 py_replay_bg-0.0.9/py_replay_bg/replay/__init__.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.634071 py_replay_bg-0.0.9/py_replay_bg/sensors/
+-rwx------   0 cappe      (501) staff       (20)     8207 2024-01-15 08:20:04.000000 py_replay_bg-0.0.9/py_replay_bg/sensors/__init__.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.634462 py_replay_bg-0.0.9/py_replay_bg/tests/
+-rwx------   0 cappe      (501) staff       (20)        0 2023-05-25 12:28:05.000000 py_replay_bg-0.0.9/py_replay_bg/tests/__init__.py
+-rwx------   0 cappe      (501) staff       (20)     1566 2024-03-28 14:25:23.000000 py_replay_bg-0.0.9/py_replay_bg/tests/test_replay_bg.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.634620 py_replay_bg-0.0.9/py_replay_bg/utils/
+-rwx------   0 cappe      (501) staff       (20)        0 2023-09-21 11:06:08.000000 py_replay_bg-0.0.9/py_replay_bg/utils/__init__.py
+-rwx------   0 cappe      (501) staff       (20)     2294 2024-01-15 08:30:23.000000 py_replay_bg-0.0.9/py_replay_bg/utils/stats.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.634708 py_replay_bg-0.0.9/py_replay_bg/visualizer/
+-rwx------   0 cappe      (501) staff       (20)     7714 2024-01-15 08:34:43.000000 py_replay_bg-0.0.9/py_replay_bg/visualizer/__init__.py
+drwxr-xr-x   0 cappe      (501) staff       (20)        0 2024-03-28 14:27:33.634989 py_replay_bg-0.0.9/py_replay_bg.egg-info/
+-rw-r--r--   0 cappe      (501) staff       (20)     4556 2024-03-28 14:27:33.000000 py_replay_bg-0.0.9/py_replay_bg.egg-info/PKG-INFO
+-rw-r--r--   0 cappe      (501) staff       (20)      872 2024-03-28 14:27:33.000000 py_replay_bg-0.0.9/py_replay_bg.egg-info/SOURCES.txt
+-rw-r--r--   0 cappe      (501) staff       (20)        1 2024-03-28 14:27:33.000000 py_replay_bg-0.0.9/py_replay_bg.egg-info/dependency_links.txt
+-rw-r--r--   0 cappe      (501) staff       (20)     1546 2024-03-28 14:27:33.000000 py_replay_bg-0.0.9/py_replay_bg.egg-info/requires.txt
+-rw-r--r--   0 cappe      (501) staff       (20)       13 2024-03-28 14:27:33.000000 py_replay_bg-0.0.9/py_replay_bg.egg-info/top_level.txt
+-rwx------   0 cappe      (501) staff       (20)     1000 2024-03-28 14:26:09.000000 py_replay_bg-0.0.9/pyproject.toml
+-rwx------   0 cappe      (501) staff       (20)     1546 2024-03-24 15:58:57.000000 py_replay_bg-0.0.9/requirements.txt
+-rw-r--r--   0 cappe      (501) staff       (20)       38 2024-03-28 14:27:33.635426 py_replay_bg-0.0.9/setup.cfg
```

### Comparing `py_replay_bg-0.0.8/COPYING.md` & `py_replay_bg-0.0.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/README.md` & `py_replay_bg-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/data/__init__.py` & `py_replay_bg-0.0.9/py_replay_bg/data/__init__.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/dss/__init__.py` & `py_replay_bg-0.0.9/py_replay_bg/dss/__init__.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/dss/default_dss_handlers.py` & `py_replay_bg-0.0.9/py_replay_bg/dss/default_dss_handlers.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/environment/__init__.py` & `py_replay_bg-0.0.9/py_replay_bg/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/example/code/quick-start.py` & `py_replay_bg-0.0.9/py_replay_bg/example/code/quick-start.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/identification/mcmc.py` & `py_replay_bg-0.0.9/py_replay_bg/identification/mcmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         # Initialize and run the sampler
         pool = None
         if rbg.environment.parallelize:
             pool = Pool(processes=rbg.environment.n_processes)
 
         posterior_func = self.model.log_posterior_single_meal if self.model.is_single_meal else self.model.log_posterior_multi_meal
         sampler = zeus.EnsembleSampler(self.n_walkers, self.n_dim, posterior_func, args=[rbg_data],
-                                       verbose=rbg.environment.verbose, pool=pool, maxsteps=1000)
+                                       verbose=rbg.environment.verbose, pool=pool, maxsteps=1000, moves=zeus.moves.GlobalMove())
         if rbg.environment.plot_mode:
             plot_callback = PlotCallBack(ncheck=self.callback_ncheck, ndim=self.n_dim, rbg=rbg, data=data)
             sampler.run_mcmc(start, self.n_steps, callbacks=[cb0, cb1, cb2, plot_callback])
             pylab.close()
         else:
             sampler.run_mcmc(start, self.n_steps, callbacks=[cb0, cb1, cb2])
         sampler.summary  # Print summary diagnostics
```

### Comparing `py_replay_bg-0.0.8/py_replay_bg/input_validation/__init__.py` & `py_replay_bg-0.0.9/py_replay_bg/input_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/model/t1d_model.py` & `py_replay_bg-0.0.9/py_replay_bg/model/t1d_model.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/py_replay_bg.py` & `py_replay_bg-0.0.9/py_replay_bg/py_replay_bg.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
         # Initialize sensors
         sensors = self.__init_sensors(cgm_model, model)
 
         # Initialize MCMC
         mcmc = MCMC(model,
                     n_steps=n_steps,
                     save_chains=save_chains,
-                    callback_ncheck=100)
+                    callback_ncheck=1000)
 
         # Initialize DSS
         dss = DSS(bw=bw, CR=CR, CF=CF, GT=GT,
                   meal_generator_handler=meal_generator_handler,
                   meal_generator_handler_params=meal_generator_handler_params,
                   bolus_calculator_handler=bolus_calculator_handler,
                   bolus_calculator_handler_params=bolus_calculator_handler_params,
```

### Comparing `py_replay_bg-0.0.8/py_replay_bg/replay/__init__.py` & `py_replay_bg-0.0.9/py_replay_bg/replay/__init__.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/sensors/__init__.py` & `py_replay_bg-0.0.9/py_replay_bg/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/tests/test_replay_bg.py` & `py_replay_bg-0.0.9/py_replay_bg/tests/test_replay_bg.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,24 @@
         df.t = pd.to_datetime(df['t'])
 
     return df
 
 def test_replay_bg():
 
     # Get test data
-    data = load_test_data(real=False, single_meal=False)
+    data = load_test_data(real=True, single_meal=False)
 
     # Set other parameters for identification
     modality = 'identification'
     bw = 100
     scenario = 'multi-meal'
     save_name = 'multi-meal_fake'
     n_steps = 10000
     save_suffix = ''
     save_folder = os.path.abspath('')
 
     # Instantiate ReplayBG
     rbg = ReplayBG(modality=modality, data=data, bw=bw, scenario=scenario, save_name=save_name, save_folder=save_folder, save_suffix=save_suffix,
-                   cgm_model='CGM', n_steps=n_steps, parallelize=False, save_workspace=False, analyze_results=False, verbose=True, plot_mode=True)
+                   cgm_model='CGM', n_steps=n_steps, parallelize=False, save_workspace=False, analyze_results=False, verbose=False, plot_mode=False)
 
     # Run it
     results = rbg.run(data=data, bw=bw, n_replay=1)
```

### Comparing `py_replay_bg-0.0.8/py_replay_bg/utils/stats.py` & `py_replay_bg-0.0.9/py_replay_bg/utils/stats.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg/visualizer/__init__.py` & `py_replay_bg-0.0.9/py_replay_bg/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/py_replay_bg.egg-info/SOURCES.txt` & `py_replay_bg-0.0.9/py_replay_bg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_replay_bg-0.0.8/pyproject.toml` & `py_replay_bg-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_replay_bg"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Giacomo Cappon", email="cappongiacomo@gmail.com" },
 ]
 description = "ReplayBG is a digital twin-based methodology to assess new strategies for type 1 diabetes management."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

