# Comparing `tmp/fermi_stacking-0.1.4a0.tar.gz` & `tmp/fermi_stacking-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fermi_stacking-0.1.4a0.tar", last modified: Tue Apr 23 13:50:36 2024, max compression
+gzip compressed data, was "fermi_stacking-0.1.5a0.tar", last modified: Thu May  2 19:44:01 2024, max compression
```

## Comparing `fermi_stacking-0.1.4a0.tar` & `fermi_stacking-0.1.5a0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.953118 fermi_stacking-0.1.4a0/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    11357 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/LICENSE
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-04-23 13:50:36.952118 fermi_stacking-0.1.4a0/PKG-INFO
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2323 2024-02-29 15:18:01.000000 fermi_stacking-0.1.4a0/README.md
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.878117 fermi_stacking-0.1.4a0/fermi_stacking/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      188 2024-02-22 20:54:20.000000 fermi_stacking-0.1.4a0/fermi_stacking/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.907118 fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    34113 2024-04-23 13:36:07.000000 fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/AnalyzeResults.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       36 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/__init__.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     1395 2024-02-28 21:29:53.000000 fermi_stacking-0.1.4a0/fermi_stacking/client.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      476 2024-02-28 21:13:42.000000 fermi_stacking-0.1.4a0/fermi_stacking/make_new_run.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.929118 fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    29992 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/PopStudies.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       26 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.933118 fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    24664 2024-02-29 14:45:18.000000 fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/Preprocess.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       42 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.947118 fermi_stacking-0.1.4a0/fermi_stacking/science_tools/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)     3890 2024-02-28 21:30:25.000000 fermi_stacking-0.1.4a0/fermi_stacking/science_tools/BinnedAnalysis.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       47 2024-02-23 19:10:27.000000 fermi_stacking-0.1.4a0/fermi_stacking/science_tools/__init__.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.950118 fermi_stacking-0.1.4a0/fermi_stacking/stacking/
--rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    21750 2024-04-23 13:28:52.000000 fermi_stacking-0.1.4a0/fermi_stacking/stacking/Stack.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       29 2024-02-08 20:27:23.000000 fermi_stacking-0.1.4a0/fermi_stacking/stacking/__init__.py
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2333 2024-02-28 20:58:50.000000 fermi_stacking-0.1.4a0/fermi_stacking/submit_fermi_stacking_jobs.py
-drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-04-23 13:50:36.951118 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/PKG-INFO
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      797 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/SOURCES.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)        1 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/dependency_links.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       71 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/entry_points.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       14 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/requires.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       15 2024-04-23 13:50:36.000000 fermi_stacking-0.1.4a0/fermi_stacking.egg-info/top_level.txt
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       38 2024-04-23 13:50:36.954118 fermi_stacking-0.1.4a0/setup.cfg
--rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      501 2024-04-23 13:46:07.000000 fermi_stacking-0.1.4a0/setup.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:01.113185 fermi_stacking-0.1.5a0/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    11357 2024-02-08 20:27:23.000000 fermi_stacking-0.1.5a0/LICENSE
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-05-02 19:44:01.112185 fermi_stacking-0.1.5a0/PKG-INFO
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2323 2024-02-29 15:18:01.000000 fermi_stacking-0.1.5a0/README.md
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:00.994183 fermi_stacking-0.1.5a0/fermi_stacking/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      199 2024-04-24 15:01:37.000000 fermi_stacking-0.1.5a0/fermi_stacking/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:01.046184 fermi_stacking-0.1.5a0/fermi_stacking/analyze_results/
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    34952 2024-05-01 14:18:50.000000 fermi_stacking-0.1.5a0/fermi_stacking/analyze_results/AnalyzeResults.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       36 2024-02-08 20:27:23.000000 fermi_stacking-0.1.5a0/fermi_stacking/analyze_results/__init__.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     1966 2024-05-01 14:26:11.000000 fermi_stacking-0.1.5a0/fermi_stacking/client.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      476 2024-02-28 21:13:42.000000 fermi_stacking-0.1.5a0/fermi_stacking/make_new_run.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:01.060184 fermi_stacking-0.1.5a0/fermi_stacking/pop_studies/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    29992 2024-02-08 20:27:23.000000 fermi_stacking-0.1.5a0/fermi_stacking/pop_studies/PopStudies.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       26 2024-02-08 20:27:23.000000 fermi_stacking-0.1.5a0/fermi_stacking/pop_studies/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:01.085184 fermi_stacking-0.1.5a0/fermi_stacking/preprocessing/
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    25514 2024-05-01 13:30:33.000000 fermi_stacking-0.1.5a0/fermi_stacking/preprocessing/Preprocess.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       42 2024-02-08 20:27:23.000000 fermi_stacking-0.1.5a0/fermi_stacking/preprocessing/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:01.088184 fermi_stacking-0.1.5a0/fermi_stacking/science_tools/
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)     3890 2024-02-28 21:30:25.000000 fermi_stacking-0.1.5a0/fermi_stacking/science_tools/BinnedAnalysis.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       47 2024-02-23 19:10:27.000000 fermi_stacking-0.1.5a0/fermi_stacking/science_tools/__init__.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:01.109185 fermi_stacking-0.1.5a0/fermi_stacking/stacking/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)    12310 2024-05-01 14:16:47.000000 fermi_stacking-0.1.5a0/fermi_stacking/stacking/AlphaBeta.py
+-rwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)    24975 2024-05-01 15:37:39.000000 fermi_stacking-0.1.5a0/fermi_stacking/stacking/Stack.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       66 2024-04-24 15:01:14.000000 fermi_stacking-0.1.5a0/fermi_stacking/stacking/__init__.py
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)     2333 2024-02-28 20:58:50.000000 fermi_stacking-0.1.5a0/fermi_stacking/submit_fermi_stacking_jobs.py
+drwxr-xr-x   0 ckarwin  (376607) cuuser   (10000)        0 2024-05-02 19:44:01.111185 fermi_stacking-0.1.5a0/fermi_stacking.egg-info/
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      304 2024-05-02 19:44:00.000000 fermi_stacking-0.1.5a0/fermi_stacking.egg-info/PKG-INFO
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      834 2024-05-02 19:44:00.000000 fermi_stacking-0.1.5a0/fermi_stacking.egg-info/SOURCES.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)        1 2024-05-02 19:44:00.000000 fermi_stacking-0.1.5a0/fermi_stacking.egg-info/dependency_links.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       71 2024-05-02 19:44:00.000000 fermi_stacking-0.1.5a0/fermi_stacking.egg-info/entry_points.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       14 2024-05-02 19:44:00.000000 fermi_stacking-0.1.5a0/fermi_stacking.egg-info/requires.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       15 2024-05-02 19:44:00.000000 fermi_stacking-0.1.5a0/fermi_stacking.egg-info/top_level.txt
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)       38 2024-05-02 19:44:01.114185 fermi_stacking-0.1.5a0/setup.cfg
+-rw-r--r--   0 ckarwin  (376607) cuuser   (10000)      501 2024-05-02 19:40:53.000000 fermi_stacking-0.1.5a0/setup.py
```

### Comparing `fermi_stacking-0.1.4a0/LICENSE` & `fermi_stacking-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.4a0/README.md` & `fermi_stacking-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking/analyze_results/AnalyzeResults.py` & `fermi_stacking-0.1.5a0/fermi_stacking/analyze_results/AnalyzeResults.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,36 @@
 from matplotlib import ticker, cm
 from scipy.stats.contingency import margins
 import fermi_stacking.pop_studies as PS
 from IntegralUpperLimit import calc_int
 from UpperLimits import UpperLimits
 from SummedLikelihood import *
 from astropy.io import fits
+from matplotlib.ticker import FormatStrFormatter
 
 class Analyze():    
     
     """Analyzes stacked results."""
 
-    def plot_final_array(self,savefig,array,use_index="default"):
+    def plot_final_array(self,savefig,array,use_index="default",stack_mode="flux_index"):
 
         """Plots the stacked profile.
 	 
         Parameters
         ----------
 	savefig : str
             Name of image file to be saved. 
 	array : str
             Name of input array to plot. Must include ".npy".
 	use_index : float, optional
             Option to calculate flux for specified index (default is 
             best-fit index).
+        stack_mode : str, optional
+            Mode of stacking. Default is flux_index. Other options are
+            alpha_beta or alpha_beta_interp. 
         """
         
         # Make print statement:
         print()
         print("Plotting final_array...")
         print()
         
@@ -67,15 +71,17 @@
         
         # Setup figure:
         fig = plt.figure(figsize=(9,9))
         ax = plt.gca()
         
         # Upload summed array:
         summed_array = np.load(array_file)
-        
+        if stack_mode == "alpha_beta_interp":
+            summed_array = summed_array.T
+
         # Get min and max:
         max_value = np.amax(summed_array)
         min_value = np.amin(summed_array)
         
         # Corresponding sigma for 2 dof:
         num_pars = 2
         sigma = stats.norm.ppf(1.-stats.distributions.chi2.sf(max_value,num_pars)/2.)
@@ -87,20 +93,26 @@
         
         # Find indices for max values:
         ind = np.unravel_index(np.argmax(summed_array,axis=None),summed_array.shape)
         best_index_value = ind[0]
         best_flux_value = ind[1]
         
         # Get best index:
-        index_list = np.arange(self.index_min,self.index_max+0.1,0.1)     
+        if stack_mode == "flux_index":
+            index_list = np.arange(self.index_min,self.index_max+0.1,0.1)     
+        if stack_mode in ["alpha_beta","alpha_beta_interp"]:
+            index_list = self.alpha_range
         best_index = index_list[ind[0]]
         
         # Get best flux:
-        flux_list=np.linspace(self.flux_min,self.flux_max,num=40,endpoint=True)
-        flux_list = 10**flux_list 
+        if stack_mode == "flux_index":
+            flux_list=np.linspace(self.flux_min,self.flux_max,num=40,endpoint=True)
+            flux_list = 10**flux_list 
+        if stack_mode in ["alpha_beta","alpha_beta_interp"]:
+            flux_list = self.beta_range
         best_flux = flux_list[ind[1]]
         
         # Option to calculate flux for specified index:
         if use_index != "default":
             index_list = np.around(index_list,decimals=1)
             best_index_value = np.where(index_list==use_index)[0][0]
             ind = np.unravel_index(np.argmax(summed_array[best_index_value],axis=None),summed_array.shape)
@@ -121,15 +133,16 @@
 	# Method 1
         def plot_method_1():
             
             img = ax.pcolormesh(flux_list,index_list,summed_array,cmap="inferno",vmin=0,vmax=max_value)
             plt.contour(flux_list,index_list,summed_array,levels = (third,second,first),
                     colors='limegreen',linestyles=["-.",'--',"-"], alpha=1,linewidths=2)
             plt.plot(best_flux,best_index,marker="+",ms=12,color="black")
-            ax.set_xscale('log')
+            if stack_mode == "flux_index":
+                ax.set_xscale('log')
             plt.xticks(fontsize=16)
             plt.yticks(fontsize=16)
             
             return img
 
 	# Method 2 
         def plot_method_2():
@@ -159,16 +172,20 @@
         img = plot_method_1()
         
         # Plot colorbar
         cbar = plt.colorbar(img,fraction=0.045)
         cbar.set_label("TS",size=16,labelpad=12)
         cbar.ax.tick_params(labelsize=12)
         
-        plt.ylabel('Photon Index',fontsize=22)
-        plt.xlabel(r'$\mathregular{\gamma}$-Ray Flux [ph $\mathrm{cm^2}$  s$\mathregular{^{-1}}$]',fontsize=22) #for flux
+        if stack_mode == "flux_index":
+            plt.ylabel('Photon Index',fontsize=22)
+            plt.xlabel(r'$\mathregular{\gamma}$-Ray Flux [ph $\mathrm{cm^2}$  s$\mathregular{^{-1}}$]',fontsize=22)
+        if stack_mode in ["alpha_beta","alpha_beta_interp"]:
+            plt.ylabel(r"$\alpha$",fontsize=22)
+            plt.xlabel(r"$\beta$",fontsize=22)
         ax.set_aspect('auto')
         ax.tick_params(axis='both',which='major',length=9)
         ax.tick_params(axis='both',which='minor',length=5)
         
         plt.savefig(savefig,bbox_inches='tight')
         
         if self.show_plots == True:
```

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking/client.py` & `fermi_stacking-0.1.5a0/fermi_stacking/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Imports:
 from fermi_stacking.stacking.Stack import MakeStack
 from fermi_stacking.science_tools.BinnedAnalysis import MakeBinnedAnalysis
+from fermi_stacking.stacking.AlphaBeta import MakeAlphaBeta
 import sys 
 
 def main(cmd_line):
 
     # Code can be ran with batch system or from command line
 
     # For batch system:
@@ -25,22 +26,32 @@
 
     # For pre-computed ltcube:
     #binned_instance = MakeBinnedAnalysis("inputs.yaml")
     #binned_instance.gtselect()
     #binned_instance.maketime()
     #binned_instance.expCube()
 
-    # Stacking routines:
+    # Standard Stacking routines:
     #instance.run_preprocessing(srcname,ra,dec)
     #instance.make_preprocessing_summary() 
     #instance.run_stacking(srcname,psf)
     #instance.combine_likelihood(exclusion_list,savefile)
     #instance.plot_final_array("name.png","name.npy")
     #instance.evolution_plot([0,1],exclude_list=exclusion_list)
     #instance.make_butterfly(name)
     #instance.get_stack_UL95("name.npy")
     #instance.calc_upper_limit(srcname,emin,emax)
+    
+    # Alpha-Beta stacking:
+    #instance = MakeAlphaBeta("inputs.yaml")
+    #instance.alpha_beta_data(index, name_list, d_list, lum_list)
+    #instance.interpolate_array_alpha_beta("run_name")
+    #instance.run_stacking(srcname,psf,indir=preproceesing_dir)
+    #instance.combine_likelihood(exclusion_list,"full_sample",\
+    #        stack_mode="alpha_beta",likelihood_home=likelihood_dir)
+    #instance.plot_final_array("full_sample.png","full_sample.npy",\
+    #        stack_mode="alpha_beta")
     ###########################################
 
 ########################
 if __name__=="__main__":
         main(sys.argv)
```

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking/pop_studies/PopStudies.py` & `fermi_stacking-0.1.5a0/fermi_stacking/pop_studies/PopStudies.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking/preprocessing/Preprocess.py` & `fermi_stacking-0.1.5a0/fermi_stacking/preprocessing/Preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,27 @@
     index_max : float
         Maximum index for stacking scan (absolute value).
     flux_min : float
         Power of min flux for stacking scan.
     flux_max : float
         Power of max flux for stacking scan.
     num_flux_bins : int
-        Number of flux bins to use.
+        Number of flux bins to use. 
+    alpha_low : float
+        Lower bound of alpha range. 
+    alpha_high : float
+        Upper bound of alpha range.
+    alpha_step : float
+        Step size of alpha list
+    beta_low : float
+        Log of Lower bound of beta range,
+    beta_high : float
+        Log of Upper bound of beta range (non-inclusive)
+    beta_step : float
+        step size of beta list
     calc_sed : bool
         If True will calculate SED. 
     sed_logEbins : list
         Log of energy bin edges for SED calculation. 
     delete_4fgl : bool
         Option to run 4FGL source. If True, must provide 
         "remove_list.csv" file in run directory, with col1=sample_name, 
@@ -177,14 +189,24 @@
         self.zmax = inputs["zmax"]
         self.index_min = inputs["index_min"]
         self.index_max = inputs["index_max"]
         self.flux_min = inputs["flux_min"]
         self.flux_max = inputs["flux_max"]
         self.num_flux_bins = inputs["num_flux_bins"]
 
+        # Parameters for alpha-beta stack
+        self.alpha_low = inputs["alpha_low"]
+        self.alpha_high = inputs["alpha_high"]
+        self.alpha_step = inputs["alpha_step"]
+        self.beta_low = inputs["beta_low"]
+        self.beta_high = inputs["beta_high"]
+        self.beta_step = inputs["beta_step"]
+        self.alpha_range = np.arange(self.alpha_low,self.alpha_high,self.alpha_step)
+        self.beta_range = np.arange(self.beta_low,self.beta_high,self.beta_step)
+
         # Option to run 4FGL sources:
         # Note: If True, must provide "remove_list.csv" file in run directory, with col1=sample_name, col2=4fgl_name, and no header.
         self.delete_4fgl = inputs["delete_4fgl"]
         if self.delete_4fgl == True:
             df = pd.read_csv("remove_list.csv",names=["col0","col1"])
             self.delete_sample_name = np.array(df["col0"].tolist())
             self.delete_4fgl_name = np.array(df["col1"].tolist())
```

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking/science_tools/BinnedAnalysis.py` & `fermi_stacking-0.1.5a0/fermi_stacking/science_tools/BinnedAnalysis.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking/stacking/Stack.py` & `fermi_stacking-0.1.5a0/fermi_stacking/stacking/Stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             Name of source. 
         
         Returns
         ------
         Fit : BinnedAnalysis.  
         """
 
-        Fit[name].funcs['Spectrum'].getParam('Integral').setBounds(1e-17,1e7)
+        Fit[name].funcs['Spectrum'].getParam('Integral').setBounds(1e-50,1e100)
         Fit[name].funcs['Spectrum'].getParam('Integral').setScale(1.0)
         Fit[name].funcs['Spectrum'].getParam('Integral').setValue(1.0)
         Fit[name].funcs['Spectrum'].getParam('Integral').setFree(False)
         Fit[name].funcs['Spectrum'].getParam('Index').setBounds(-10,0)
         Fit[name].funcs['Spectrum'].getParam('Index').setScale(1.0)
         Fit[name].funcs['Spectrum'].getParam('Index').setValue(-2.0)
         Fit[name].funcs['Spectrum'].getParam('Index').setFree(False)
@@ -157,15 +157,15 @@
             
                 os.chdir(this_scratch_dir)        
    
         shutil.copy2('%s/srcmap_0%s.fits' %(indir,PSF), 'srcmap_0%s.fits' %PSF)
         shutil.copy2('%s/bexpmap_0%s.fits' %(indir,PSF), 'bexpmap_0%s.fits' %PSF)
         shutil.copy2('%s/fit_model_3_0%s.xml' %(indir,PSF), 'fit_model_3_0%s.xml' %PSF)
 	
-        obs = BinnedObs(srcMaps='srcmap_0%s.fits' %PSF,expCube=self.ltcube,binnedExpMap='bexpmap_0%s.fits' %PSF,irfs='P8R3_SOURCE_V2')
+        obs = BinnedObs(srcMaps='srcmap_0%s.fits' %PSF,expCube=self.ltcube,binnedExpMap='bexpmap_0%s.fits' %PSF,irfs=self.irfs)
 	
         # Define index range for scan:
         index = -1.0*np.arange(self.index_min,self.index_max+0.1,0.1)
         index = np.around(index,decimals=1)
         index = index.tolist()
 
         for i in range(len(index)):
@@ -176,15 +176,15 @@
             	
             LOG_LIKE=[]
             Fit_Qual=[]
             Conv=[]
             Flux=[]
             Index=[]
 
-            # Define flux range for scane:
+            # Define flux range for scan:
             flux=np.linspace(self.flux_min,self.flux_max,num=self.num_flux_bins,endpoint=True)
 		
             for j in range(len(flux)):
 				
                 Index+=['%.1f' %np.fabs(index[i])]
                 Flux+=['%.2e' %(10**flux[j])]
                 like1 = BinnedAnalysis(obs,'fit_model_3_0%s.xml' %PSF,optimizer='DRMNFB')
@@ -236,25 +236,32 @@
             del Flux,Index,LOG_LIKE,Fit_Qual,Conv
             gc.collect() #dump unused memory to speed up calculation
 	
         os.chdir(self.home)
         
         return
 
-    def combine_likelihood(self, exclusion_list, savefile):
+    def combine_likelihood(self, exclusion_list, savefile, \
+            stack_mode="flux_index", likelihood_home="default"):
 	
         """Make 2D TS profiles for each source and add to get stacked profile.
 
 	Parameters
         ----------
         exclusion_list : list
             List of sources to exclude from stacked profile.
 	Savefile : str
             Prefix of array to be saved. Do not include ".npy" at the 
             end of the name; it's already included.
+        stack_mode : str, optional
+            Type of stacking being performed. Default is flux_index. 
+            Other option is alpha_beta. 
+        likelihood_home : str, optional
+            Full path to run directory of preprocessing, where null
+            likelihood has been calculated (default is current working directory).
         """
         
         # Make print statement:
         print()
         print("Combining likelihood...")
         print()
 
@@ -271,27 +278,31 @@
         if os.path.exists(individual_array_main_dir) == False:  
             os.system("mkdir %s" %individual_array_main_dir)
         
         image_main_dir = os.path.join(adding_main_dir,"Images")
         if os.path.exists(image_main_dir) == False:
             os.system("mkdir %s" %image_main_dir)
 
+        # Define default likelihood directory:
+        if likelihood_home == "default":
+            likelihood_home = self.home
+
         if self.JLA == False:
 
 	    # Define counters and lists:
             counter = 0
             print_list = []
             max_TS_list = []
 
 	    # Iterate through sources:
             for s in range(0,len(self.sample_name_list)):
 			
                 srcname = self.sample_name_list[s]
 
-                likelihood_dir = os.path.join(self.home,"Preprocessed_Sources",srcname,"output/null_likelihood_0.txt")
+                likelihood_dir = os.path.join(likelihood_home,"Preprocessed_Sources",srcname,"output/null_likelihood_0.txt")
                 stacking_dir = os.path.join(self.home,"Stacked_Sources",srcname)
 	
                 if os.path.exists(stacking_dir) == False or os.path.exists(likelihood_dir) == False:
                     print() 
                     print('Does not exist: ' + srcname)
                     print()
 
@@ -300,18 +311,23 @@
                     os.chdir(stacking_dir)
 	            
                     print_list.append(srcname)
 		
                     array_list = []
     
                     # Define index list of scan:
-                    index_list = np.arange(self.index_min,self.index_max+0.1,0.1)
-                    index_list = np.around(index_list,decimals=1)
-                    index_list = index_list.tolist()
-            
+                    if stack_mode == "flux_index":
+                        index_list = np.arange(self.index_min,self.index_max+0.1,0.1)
+                        index_list = np.around(index_list,decimals=1)
+                        index_list = index_list.tolist()
+                    if stack_mode == "alpha_beta":
+                        # Index implies alpha.
+                        # Flux implies beta.
+                        index_list = self.alpha_beta
+
                     # Read null likelihood:
                     f = open(likelihood_dir,'r')
                     lines = f.readlines()
                     null = float(lines[0])
 
                     for i in range(0,len(index_list)):
                         this_index = str(index_list[i])
@@ -366,15 +382,15 @@
                 srcname = self.sample_name_list[s]
                 counter = 0
 
                 j_counter = 0
                 for j in [0,1,2,3]:
             
                     likelihood_dir = "Preprocessed_Sources/%s/output/null_likelihood_%s.txt" %(srcname,str(j))
-                    likelihood_dir = os.path.join(self.home,likelihood_dir)
+                    likelihood_dir = os.path.join(likelihood_home,likelihood_dir)
                     stacking_dir = "Stacked_Sources/Likelihood_%s/%s" %(str(j),srcname)
                     stacking_dir = os.path.join(self.home,stacking_dir)
 
                     if os.path.exists(stacking_dir) == False or os.path.exists(likelihood_dir) == False:
                         print() 
                         print('Does not exist: ' + srcname + "_%s" %str(j))
                         print() 
@@ -383,18 +399,21 @@
                     if srcname not in exclusion_list and os.path.exists(likelihood_dir) == True and os.path.exists(stacking_dir) == True:
 				
                         os.chdir(stacking_dir)
 
                         array_list = []
 
                         # Define index list of scan:
-                        index_list = np.arange(self.index_min,self.index_max+0.1,0.1)
-                        index_list = np.around(index_list,decimals=1)
-                        index_list = index_list.tolist()
-                        
+                        if stack_mode == "flux_index":
+                            index_list = np.arange(self.index_min,self.index_max+0.1,0.1)
+                            index_list = np.around(index_list,decimals=1)
+                            index_list = index_list.tolist()
+                        if stack_mode == "alpha_beta":
+                            index_list = self.alpha_range
+
                         # Read null likelihood:
                         f = open(likelihood_dir,'r')
                         lines = f.readlines()
                         null = float(lines[0])
                         
                         for i in range(0,len(index_list)):
                             this_index = str(index_list[i])
@@ -442,49 +461,71 @@
             np.save(array_file,total_summed_array)
 
         # Return to home:
         os.chdir(self.home)
 		
         return 
 
-    def evolution_plot(self, skip_rows, exclude_list=None, use_src_names=False):
+    def evolution_plot(self, skip_rows, savefile, preprocess_home="default",\
+            exclude_list=None, use_src_names=False, stack_mode="flux_index",\
+            show_index=False, show_flux=False):
 
         """Plot max TS as a funtion of source.
         
         Parameters
         ----------
-        skip_rows : list of ints
-            Rows to skip when readying txt file.
+        skip_rows : list
+            List of rows to skip when reading preprocessing summary.
+        savefile : str
+            Prefix of output image. 
+        preprocess_home : str, optional
+            Full path to run directory of preprocessing.
         exlude_list : list of str, optional
             Names of sources to exclude.
         use_src_names : bool, optional
             Option to use source names in x-axis of plot 
             (default is False).
+        stack_mode : str, optional
+            Stacking mode to use. Default is flux_index. The other 
+            option is alpha_beta.
+        show_index : bool, optional
+            Show index evolution (default is False).
+        show_flux : bool, optional
+            Show flux evolution (default is False).
         """
 
 	# Make print statement:
         print()
         print("Running evolution_plot...")
         print()
 
-        name_file = os.path.join(self.home, "Preprocessed_Sources", 
+        # Define default preprocessing home:
+        if preprocess_home == "default":
+            preprocess_home = self.home
+
+        name_file = os.path.join(preprocess_home, "Preprocessed_Sources", 
                 "preprocessing_summary_" + self.run_name + ".txt")
         df = pd.read_csv(name_file,sep='\s+',skiprows=skip_rows)
         name_list = df["name"]
         ts_list = df["TS"]
 
         # Exclude sources:
         if exclude_list != None:
             keep_index = ~np.isin(name_list,exclude_list)
             name_list = name_list[keep_index].tolist()
             ts_list = ts_list[keep_index].tolist()
 
-        index_scan = np.arange(self.index_min,self.index_max,0.1)
-        flux_scan = np.linspace(self.flux_min,self.flux_max,num=41,endpoint=True)
-        flux_scan = 10**flux_scan
+        if stack_mode == "flux_index":
+            index_scan = np.arange(self.index_min,self.index_max,0.1)
+            flux_scan = np.linspace(self.flux_min,self.flux_max,num=41,endpoint=True)
+            flux_scan = 10**flux_scan
+        
+        if stack_mode == "alpha_beta":
+            index_scan = self.alpha_range
+            flux_scan = self.beta_range
 
         max_list = []
         index_list = []
         flux_list = []
         name_plot_list = []
         for s in range(0,len(name_list)):
             index = len(name_list) - s - 1
@@ -495,14 +536,17 @@
             # Check that source name has not been changed:
             if this_name not in self.sample_name_list:
                 print("WARNING: Name has been updated and will not be included: %s" %this_name)
                 continue
     
             plot_name = this_name		
             this_file = "Add_Stacking/Numpy_Arrays/Individual_Sources/" + this_name + ".npy"
+            if os.path.exists(this_file) == False:
+                print("WARNING: File does not exists: %s" %this_file)
+                continue 
             this_array = np.load(this_file)
             name_plot_list.append(this_name)
 
             # Add array
             if s == 0:
                 total_array = this_array
             if s > 0:
@@ -526,15 +570,15 @@
 
         # Plot
         fig = plt.figure(figsize=(8,6))
         ax = plt.gca()
         
         plot_range = np.arange(0,len(name_plot_list),1)
 
-        plt.plot(plot_range,max_list,marker='s',ls="--",ms=8,color="black",label="Max TS (for stack)")
+        plt.plot(plot_range,max_list,marker='s',ls="--",ms=8,color="black",zorder=10,label="Max TS (for stack)")
 
         plt.grid(color="grey",ls="-",alpha=0.5)
         plt.yticks(fontsize=12)
         plt.xticks(fontsize=12)
 
         # Option to use source names for x axis:
         if use_src_names == True:
@@ -545,14 +589,39 @@
         ax.tick_params(axis='both',which='major',length=9)
         ax.tick_params(axis='both',which='minor',length=5)
         plt.xlabel("Number of Stacked Sources (TS ranked)", fontsize=14)
         plt.ylabel("Max TS",fontsize=14,color="black")
         ax.tick_params(axis='y',labelcolor="black")
         plt.xlim(0,len(max_list)+10)
 
+        # Plot second twin axis:
+        if show_index == True:
+            ax2 = ax.twinx()
+            ax2.plot(plot_range,index_list,marker='^',ls="-",ms=10,color="blue",alpha=0.6,label="Spectral Index")
+            ax2.tick_params(axis='y',labelcolor="blue")
+            if stack_mode == "flux_index":
+                plt.ylabel("Index",fontsize=16,color="blue")
+            if stack_mode == "alpha_beta":
+                plt.ylabel("Alpha",fontsize=16,color="blue")
+            plt.yticks(fontsize=12)
+        
+        # Plot third twin axis:
+        if show_flux == True:
+            ax3 = ax.twinx()
+            ax3.plot(plot_range,flux_list,marker='o',ls="-",ms=10,color="darkorange",alpha=0.6,label="Flux")
+            ax3.tick_params(axis='y',labelcolor="darkorange")
+            if stack_mode == "flux_index":
+                plt.ylabel("flux [$\mathrm{ph \ cm^{-2} \ s^{-1}}$]",fontsize=16,color="darkorange")
+            if stack_mode == "alpha_beta":
+                plt.ylabel("Beta",fontsize=16,color="darkorange")
+            plt.yticks(fontsize=12)
+            # Offset axis if also showing index:
+            if show_index == True:
+                ax3.spines.right.set_position(("axes", 1.2))
+
         plt.tight_layout()
 
-        plt.savefig("Add_Stacking/Images/TS_evolution_full.pdf")
+        plt.savefig("Add_Stacking/Images/%s.pdf" %savefile)
         plt.show()	
 
         return
```

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking/submit_fermi_stacking_jobs.py` & `fermi_stacking-0.1.5a0/fermi_stacking/submit_fermi_stacking_jobs.py`

 * *Files identical despite different names*

### Comparing `fermi_stacking-0.1.4a0/fermi_stacking.egg-info/SOURCES.txt` & `fermi_stacking-0.1.5a0/fermi_stacking.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 fermi_stacking/analyze_results/__init__.py
 fermi_stacking/pop_studies/PopStudies.py
 fermi_stacking/pop_studies/__init__.py
 fermi_stacking/preprocessing/Preprocess.py
 fermi_stacking/preprocessing/__init__.py
 fermi_stacking/science_tools/BinnedAnalysis.py
 fermi_stacking/science_tools/__init__.py
+fermi_stacking/stacking/AlphaBeta.py
 fermi_stacking/stacking/Stack.py
 fermi_stacking/stacking/__init__.py
```

