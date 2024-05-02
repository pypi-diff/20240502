# Comparing `tmp/SNeSCOPE-1.0.2.tar.gz` & `tmp/SNeSCOPE-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SNeSCOPE-1.0.2.tar", last modified: Tue Apr  9 12:56:02 2024, max compression
+gzip compressed data, was "dist\SNeSCOPE-1.0.3.tar", last modified: Thu May  2 09:11:58 2024, max compression
```

## Comparing `SNeSCOPE-1.0.2.tar` & `SNeSCOPE-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/
--rw-rw-rw-   0        0        0    11544 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      321 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1683 2024-04-02 22:21:58.000000 SNeSCOPE-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      829 2024-04-09 12:55:42.000000 SNeSCOPE-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/SNeSCOPE/
--rw-rw-rw-   0        0        0   100299 2024-04-09 12:06:26.000000 SNeSCOPE-1.0.2/SNeSCOPE/blackbody_tools.py
--rw-rw-rw-   0        0        0    28973 2024-04-01 10:29:56.000000 SNeSCOPE-1.0.2/SNeSCOPE/PhotoUtils.py
--rw-rw-rw-   0        0        0        0 2024-03-28 15:42:27.000000 SNeSCOPE-1.0.2/SNeSCOPE/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/SNeSCOPE.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/SNeSCOPE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      321 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/SNeSCOPE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       73 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/SNeSCOPE.egg-info/requires.txt
--rw-rw-rw-   0        0        0      272 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/SNeSCOPE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 12:56:02.000000 SNeSCOPE-1.0.2/SNeSCOPE.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 09:11:58.000000 SNeSCOPE-1.0.3/
+-rw-rw-rw-   0        0        0    11544 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      321 2024-05-02 09:11:58.000000 SNeSCOPE-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1683 2024-04-02 22:21:58.000000 SNeSCOPE-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 09:11:58.000000 SNeSCOPE-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      829 2024-05-02 09:09:42.000000 SNeSCOPE-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:11:58.000000 SNeSCOPE-1.0.3/SNeSCOPE/
+-rw-rw-rw-   0        0        0   100276 2024-05-02 09:01:56.000000 SNeSCOPE-1.0.3/SNeSCOPE/blackbody_tools.py
+-rw-rw-rw-   0        0        0    28973 2024-04-01 10:29:56.000000 SNeSCOPE-1.0.3/SNeSCOPE/PhotoUtils.py
+-rw-rw-rw-   0        0        0        0 2024-03-28 15:42:27.000000 SNeSCOPE-1.0.3/SNeSCOPE/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:11:58.000000 SNeSCOPE-1.0.3/SNeSCOPE.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-02 09:11:57.000000 SNeSCOPE-1.0.3/SNeSCOPE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      321 2024-05-02 09:11:57.000000 SNeSCOPE-1.0.3/SNeSCOPE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2024-05-02 09:11:57.000000 SNeSCOPE-1.0.3/SNeSCOPE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      272 2024-05-02 09:11:57.000000 SNeSCOPE-1.0.3/SNeSCOPE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 09:11:57.000000 SNeSCOPE-1.0.3/SNeSCOPE.egg-info/top_level.txt
```

### Comparing `SNeSCOPE-1.0.2/LICENSE` & `SNeSCOPE-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SNeSCOPE-1.0.2/pyproject.toml` & `SNeSCOPE-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SNeSCOPE-1.0.2/README.md` & `SNeSCOPE-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `SNeSCOPE-1.0.2/setup.py` & `SNeSCOPE-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 description='SNeSCOPE is a python package for modeling supernova light curves using the analytic models of Morag et al 2023 and Morag et al 2024.',
 long_description=open('README.md').read(),
 long_description_content_type='text/markdown',
 
 setup(
     name='SNeSCOPE',
-    version='1.0.2',
+    version='1.0.3',
     description='Published version (April 2024)',  
     author='Ido Irani',
     author_email='idoirani@gmail.com', 
     url = 'https://github.com/idoirani/shock_cooling',
     keywords='astronomy',  
     packages=["SNeSCOPE"],
     #packages=find_packages(),
```

### Comparing `SNeSCOPE-1.0.2/SNeSCOPE/blackbody_tools.py` & `SNeSCOPE-1.0.3/SNeSCOPE/blackbody_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1466,15 +1466,15 @@
 		u,d,v = np.linalg.svd(resids_cov)
 		A = u[:,:3] @ np.diag(d[:3]) @ v[:3,:]  
 		if (np.linalg.eig(A+cov_obs)[0]<0).any():
 			import ipdb; ipdb.set_trace
 		cov_est = A+cov_obs
 		inv_cov = np.linalg.inv(cov_est)
 	else: 
-		cov_obs = np.diagflat(np.array(data[data['t_rest']<=t_max]['AB_MAG_ERR'])**2+ sys_err**2)   
+		cov_obs = np.diagflat(np.array(data['AB_MAG_ERR'])**2+ sys_err**2)   
 		cov_est = cov_obs  
 		inv_cov = np.linalg.inv(cov_obs)
 	return inv_cov,cov_est
 
 
 def get_sim_params(sn_inds,**kwargs):
 	inputs = {    'path_mat'    :  '/home/idoi/Dropbox/Objects/ZTF infant sample/Multigroup simulations/Multigroup simulations/RSG_batch_R03_20_removed_lines_Z1.mat'
```

### Comparing `SNeSCOPE-1.0.2/SNeSCOPE/PhotoUtils.py` & `SNeSCOPE-1.0.3/SNeSCOPE/PhotoUtils.py`

 * *Files identical despite different names*

