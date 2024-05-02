# Comparing `tmp/sitesyncro-0.9.2.tar.gz` & `tmp/sitesyncro-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesyncro-0.9.2.tar", last modified: Sat Apr 27 23:13:15 2024, max compression
+gzip compressed data, was "sitesyncro-0.9.3.tar", last modified: Thu May  2 21:15:18 2024, max compression
```

## Comparing `sitesyncro-0.9.2.tar` & `sitesyncro-0.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 23:13:15.838783 sitesyncro-0.9.2/
--rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.2/LICENSE
--rw-rw-rw-   0        0        0    22386 2024-04-27 23:13:15.838783 sitesyncro-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    21452 2024-04-27 23:04:14.000000 sitesyncro-0.9.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 23:13:15.838783 sitesyncro-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1712 2024-04-27 23:09:08.000000 sitesyncro-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 23:13:15.807541 sitesyncro-0.9.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 23:13:15.807541 sitesyncro-0.9.2/src/sitesyncro/
--rw-rw-rw-   0        0        0    21070 2024-04-27 23:02:38.000000 sitesyncro-0.9.2/src/sitesyncro/Model.py
--rw-rw-rw-   0        0        0    10674 2024-04-27 21:54:51.000000 sitesyncro-0.9.2/src/sitesyncro/Sample.py
--rw-rw-rw-   0        0        0      200 2024-04-27 23:09:18.000000 sitesyncro-0.9.2/src/sitesyncro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 23:13:15.823161 sitesyncro-0.9.2/src/sitesyncro/utils/
--rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.2/src/sitesyncro/utils/__init__.py
--rw-rw-rw-   0        0        0     9848 2024-04-27 20:33:07.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_cluster.py
--rw-rw-rw-   0        0        0      961 2024-04-23 15:45:23.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_data.py
--rw-rw-rw-   0        0        0     5486 2024-04-27 21:42:17.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_load.py
--rw-rw-rw-   0        0        0     1566 2024-04-27 20:28:19.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_mp.py
--rw-rw-rw-   0        0        0     8982 2024-04-27 22:05:16.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_oxcal.py
--rw-rw-rw-   0        0        0     8939 2024-04-27 23:03:00.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_phase.py
--rw-rw-rw-   0        0        0     4909 2024-04-27 22:24:52.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_plot.py
--rw-rw-rw-   0        0        0     2173 2024-04-23 17:46:49.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_radiocarbon.py
--rw-rw-rw-   0        0        0     6620 2024-04-27 19:28:03.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_simulate.py
--rw-rw-rw-   0        0        0     4037 2024-04-27 21:34:34.000000 sitesyncro-0.9.2/src/sitesyncro/utils/fnc_stat.py
-drwxrwxrwx   0        0        0        0 2024-04-27 23:13:15.838783 sitesyncro-0.9.2/src/sitesyncro.egg-info/
--rw-rw-rw-   0        0        0    22386 2024-04-27 23:13:15.000000 sitesyncro-0.9.2/src/sitesyncro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      668 2024-04-27 23:13:15.000000 sitesyncro-0.9.2/src/sitesyncro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 23:13:15.000000 sitesyncro-0.9.2/src/sitesyncro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-04-27 23:13:15.000000 sitesyncro-0.9.2/src/sitesyncro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 23:13:15.000000 sitesyncro-0.9.2/src/sitesyncro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.793726 sitesyncro-0.9.3/
+-rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0    11296 2024-05-02 21:15:18.792662 sitesyncro-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10362 2024-05-02 21:07:04.000000 sitesyncro-0.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:15:18.793726 sitesyncro-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1712 2024-04-28 08:59:27.000000 sitesyncro-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.739438 sitesyncro-0.9.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.755927 sitesyncro-0.9.3/src/sitesyncro/
+-rw-rw-rw-   0        0        0    39559 2024-05-02 21:00:25.000000 sitesyncro-0.9.3/src/sitesyncro/Model.py
+-rw-rw-rw-   0        0        0    19654 2024-05-02 20:25:50.000000 sitesyncro-0.9.3/src/sitesyncro/Sample.py
+-rw-rw-rw-   0        0        0      201 2024-05-02 14:33:18.000000 sitesyncro-0.9.3/src/sitesyncro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.789612 sitesyncro-0.9.3/src/sitesyncro/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.3/src/sitesyncro/utils/__init__.py
+-rw-rw-rw-   0        0        0    16865 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_cluster.py
+-rw-rw-rw-   0        0        0     2425 2024-05-02 14:21:12.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_data.py
+-rw-rw-rw-   0        0        0     8495 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_load.py
+-rw-rw-rw-   0        0        0     3485 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_mp.py
+-rw-rw-rw-   0        0        0    11396 2024-05-02 14:33:18.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_oxcal.py
+-rw-rw-rw-   0        0        0    13621 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_phase.py
+-rw-rw-rw-   0        0        0     5882 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_plot.py
+-rw-rw-rw-   0        0        0     2572 2024-05-02 14:41:27.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_radiocarbon.py
+-rw-rw-rw-   0        0        0     9217 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_simulate.py
+-rw-rw-rw-   0        0        0     6192 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_stat.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.791663 sitesyncro-0.9.3/src/sitesyncro.egg-info/
+-rw-rw-rw-   0        0        0    11296 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      668 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/top_level.txt
```

### Comparing `sitesyncro-0.9.2/LICENSE` & `sitesyncro-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.2/setup.py` & `sitesyncro-0.9.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="sitesyncro",
-    version="0.9.2",
+    version="0.9.3",
     description="SiteSyncro - Site-specific chronological modeling and synchronization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/demjanp/SiteSyncro",
     author="Peter Demjan",
     author_email="peter.demjan@gmail.com",
     classifiers=[
```

### Comparing `sitesyncro-0.9.2/src/sitesyncro/utils/fnc_oxcal.py` & `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_oxcal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import os
 import re
 import zipfile
-import requests
-import subprocess
-import numpy as np
-from tqdm import tqdm
 from collections import defaultdict
+from typing import Dict, Any
+
+import numpy as np
+import requests
+import unicodedata
 from scipy.interpolate import interp1d
+from tqdm import tqdm
 
-def download_oxcal(url = None):
-	
+
+def download_oxcal(url: str = None) -> bool:
+	"""
+	Download and unzip OxCal from a specified URL.
+
+	This function checks if OxCal is already downloaded. If not, it downloads and unzips OxCal from a specified URL to
+	the current directory.
+
+	Parameters:
+	url (str, optional): The URL to download OxCal from. If not provided, the default OxCal distribution URL is used.
+
+	Returns:
+	bool: True if OxCal is successfully downloaded and unzipped, False otherwise.
+	"""
 	if os.path.isfile("OxCal\\bin\\OxCalWin.exe"):
 		return True
 	# Download and unzip OxCal from url to the current directory
 	
 	if url is None:
 		url = "https://c14.arch.ox.ac.uk/OxCalDistribution.zip"
 	
@@ -22,15 +36,15 @@
 	# get filename from url
 	local_zip = os.path.basename(url)
 	
 	# Download the file from `url` and save it locally under `local_zip`:
 	try:
 		response = requests.get(url, stream=True)
 	except requests.exceptions.RequestException as e:
-		print (f"Error: Unable to connect to {url}. Please check the URL or your internet connection.")
+		print(f"Error: Unable to connect to {url}. Please check the URL or your internet connection.")
 		return False
 	
 	total_size_in_bytes = int(response.headers.get('content-length', 0))
 	progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
 	
 	with open(local_zip, 'wb') as f:
 		for chunk in response.iter_content(chunk_size=8192):
@@ -44,50 +58,72 @@
 		zip_ref.extractall()
 	
 	# Remove the zip file
 	os.remove(local_zip)
 	
 	return True
 
-def oxcal_date(name, age, uncertainty, date_type, outlier):
+
+def oxcal_date(name: str, age: float, uncertainty: float, date_type: str, long_lived: bool, outlier: bool) -> str:
+	"""
+	Generate an OxCal date string.
+
+	This function generates an OxCal date string based on the provided parameters.
+
+	Parameters:
+	name (str): The name of the date.
+	age (float): The age of the date.
+	uncertainty (float): The uncertainty of the date.
+	date_type (str): The type of the date. It should be 'R' or 'U'.
+	long_lived (bool): Whether the date is long-lived.
+	outlier (bool): Whether the date is an outlier.
+
+	Returns:
+	str: The generated OxCal date string.
+
+	Raises:
+	Exception: If an invalid date type is specified.
+	"""
 	txt = None
 	if date_type == 'R':
 		txt = '''R_Date("%s", %f, %f)''' % (name, age, uncertainty)
 	elif date_type == 'U':
 		txt = '''Date("%s", U(CE(%f), CE(%f)))''' % (name, -(age + uncertainty - 1950), -(age - uncertainty - 1950))
 	if txt is None:
 		raise Exception("Invalid date type specified: %s (must be 'R' or 'U')" % (date_type))
 	if outlier:
-		txt += "{Outlier(1);};"
+		txt += '''{Outlier("General", 1);};'''
+	elif long_lived:
+		txt += '''{Outlier("Charcoal", 1);};'''
 	else:
 		txt += ";"
 	return txt
 
-def gen_sequence(name, data):
-	
+
+def gen_sequence(name: str, data: Dict[int, str]) -> str:
 	txt = ""
 	for phase in sorted(list(data.keys())):
 		txt += '''
 		Boundary("Start %(name)s-%(phase)d");
 		Phase("%(name)s-%(phase)d")
 		{
 			%(dates)s
 		};
 		Boundary("End %(name)s-%(phase)d");
-		''' % dict(name = name, phase = phase, dates = data[phase])
+		''' % dict(name=name, phase=phase, dates=data[phase])
 	
 	return '''
 	Sequence(%s)
 	{
 		%s
 	};
 	''' % (name, txt)
-	
-def gen_contiguous(name, data):
-	
+
+
+def gen_contiguous(name: str, data: Dict[int, str]) -> str:
 	txt = ""
 	last_phase = None
 	for phase in sorted(list(data.keys())):
 		if last_phase is None:
 			txt += '''
 		Boundary("Start %s-%d");
 			''' % (name, phase)
@@ -109,94 +145,127 @@
 	return '''
 	Sequence(%s)
 	{
 		%s
 	};
 	''' % (name, txt)
 
-def gen_overlapping(name, data):
-	
+
+def gen_overlapping(name: str, data: Dict[int, str]) -> str:
 	txt = ""
 	for phase in sorted(list(data.keys())):
 		txt += '''
 		Sequence()
 		{
 			Boundary("Start %(name)s-%(phase)d");
 			Phase("%(name)s-%(phase)d")
 			{
 				%(dates)s
 			};
 			Boundary("End %(name)s-%(phase)d");
 		};
-		''' % dict(name = name, phase = phase, dates = data[phase])
+		''' % dict(name=name, phase=phase, dates=data[phase])
 	return '''
 	Phase(%s)
 	{
 		%s
 	};
 	''' % (name, txt)
 
-def gen_none(name, data):
-	
+
+def gen_none(name: str, data: Dict[int, str]) -> str:
 	txt = ""
 	for phase in sorted(list(data.keys())):
 		txt += '''
 		Label("%s-%d");
 		%s
 		''' % (name, phase, data[phase])
 	return txt
 
-def gen_oxcal_model(model):
-	
+
+def gen_oxcal_model(model: object) -> str:
+	"""
+	Generate an OxCal model string.
+
+	This function generates an OxCal model string based on the provided model object.
+
+	Parameters:
+	model (Model): The Model object.
+
+	Returns:
+	str: The generated OxCal model string.
+
+	Raises:
+	Exception: If an invalid phase model is specified.
+	"""
 	model_fncs = {
 		'sequence': gen_sequence,
 		'contiguous': gen_contiguous,
 		'overlapping': gen_overlapping,
 		'none': gen_none,
 	}
 	if model.phase_model not in model_fncs:
 		raise Exception("Invalid model specified: %s" % (model.phase_model))
 	
 	txt = ''
 	groups = model.groups
 	for group in groups:
 		data = defaultdict(list)
 		for name in groups[group]:
-			if model.samples[name].outlier:
-				continue
 			data[model.samples[name].phase].append(model.samples[name])
 		data = dict(data)
 		for phase in data:
-			data[phase] = sorted(data[phase], key = lambda sample: sum(sample.likelihood_range))
-			data[phase] = "\n".join([sample.to_oxcal() for sample in data[phase]])
+			data_phase = sorted(data[phase], key=lambda sample: sum(sample.get_range()))
+			data[phase] = "\n".join([sample.to_oxcal() for sample in data_phase])
 		txt += model_fncs[model.phase_model]("Gr.%d" % (group), data)
 	
-	return '''
+	txt = '''
 Curve("%s","%s");
 Plot()
 {
+	Outlier_Model("Charcoal",Exp(1,-10,0),U(0,3),"t");
+	Outlier_Model("General",T(5),U(0,4),"t");
 	%s
 };
 	''' % (model.curve_name, model.curve_name, txt)
+	
+	# Replace non-ASCII characters with their closest ASCII equivalent
+	txt = ''.join(c for c in unicodedata.normalize('NFKD', txt) if unicodedata.category(c) != 'Mn')
+	return txt
 
-def load_oxcal_data(fname):
+
+def load_oxcal_data(fname: str) -> Dict:
+	"""
+	Load OxCal data from a file.
+
+	This function loads OxCal data from a specified file.
+
+	Parameters:
+	fname (str): The name of the file to load the data from.
+
+	Returns:
+	Dict: The loaded OxCal data.
+
+	Raises:
+	Exception: If the data file is not found.
+	"""
 	
 	def replace_colons_in_braces(s):
 		# Find the innermost braces
 		inner_braces = re.findall(r'\{[^{}]*\}', s)
 		if not inner_braces:
 			return s
 		
 		for brace in inner_braces:
 			# Replace colons in the innermost braces
 			s = s.replace(brace, "dict(%s)" % brace.replace(':', '=')[1:-1])
 		
 		# Recursively process the modified string
 		return replace_colons_in_braces(s)
-
+	
 	def read_js_file(file_path):
 		
 		data = {}
 		
 		with (open(file_path, 'r') as file):
 			for line in file:
 				if line.startswith('if('):
@@ -215,15 +284,15 @@
 				
 				value = replace_colons_in_braces(value)
 				
 				# Replace NaN (only if whole word) with None
 				value = re.sub(r'\bNaN\b', 'None', value)
 				
 				# Parse value using python eval
-				value = eval(value)
+				value = eval(value, dict(true=True, false=False))
 				if value == []:
 					value = {}
 				
 				keys = key.split('.')
 				collect = []
 				for key in keys:
 					index1 = None
@@ -247,28 +316,36 @@
 					if i == len(keys) - 1:
 						current[key] = value
 					elif key not in current:
 						current[key] = {}
 					current = current[key]
 		
 		return data
-
 	
 	if not os.path.isfile(fname):
 		raise Exception("Data file %s not found" % (fname))
 	
 	return read_js_file(fname)
 
-def get_distributions(data, curve):
-	# data = OxCal data (from load_oxcal_data)
-	# curve = np.array([[calendar year BP, C-14 year, uncertainty], ...]), sorted by calendar years
-	#
-	# returns likelihoods, posteriors
-	# likelihoods = {name: [distribution, mean, rng], ...}
-	# posteriors = {name: [distribution, mean, rng, agreement], ...}
+
+def get_distributions(data: Dict, curve: np.ndarray) -> (Dict[str, Any], Dict[str, Any]):
+	"""
+	Get distributions from OxCal data.
+
+	This function gets likelihoods and posteriors from OxCal data unified to match the range and calendar ages on the calibration curve.
+
+	Parameters:
+	data (Dict): The OxCal data (from load_oxcal_data).
+	curve: np.array([[calendar year BP, C-14 year, uncertainty], ...]), sorted by calendar years. The radiocarbon calibration curve.
+
+	Returns:
+	(likelihoods, posteriors)
+		- likelihoods = {name: [distribution, mean, rng], ...}
+		- posteriors = {name: [distribution, mean, rng, agreement], ...}
+	"""
 	
 	def _get_params(params_data):
 		mean = None
 		if 'mean' in params_data:
 			mean = 1950 - params_data['mean']
 		prob = params_data['prob']
 		start = params_data['start']
@@ -282,15 +359,15 @@
 				L = min(L, params_data['range'][2][key][0])
 				U = max(U, params_data['range'][2][key][1])
 			rng = (1950 - L, 1950 - U)
 		return mean, rng, prob, years
 	
 	def _unify(dist, years, curve):
 		# years are in CE
-		all_years = curve[:,0]
+		all_years = curve[:, 0]
 		years = 1950 - np.array(years)
 		# Make sure years are in the correct order
 		if np.sign(years[-1] - years[0]) != np.sign(all_years[-1] - all_years[0]):
 			years = years[::-1]
 			dist = dist[::-1]
 		years = np.concatenate(([all_years[0]], years, [all_years[-1]]))
 		dist = np.concatenate(([0], dist, [0]))
@@ -339,8 +416,7 @@
 			mean, rng, prob, years = _get_params(data['ocd'][i]['posterior'])
 			result[name] = [_unify(prob, years, curve), mean, rng, agreement]
 		return result
 	
 	likelihoods = _load_likelihoods(data)
 	posteriors = _load_posteriors(data)
 	return likelihoods, posteriors
-
```

### Comparing `sitesyncro-0.9.2/src/sitesyncro/utils/fnc_plot.py` & `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,178 @@
-from matplotlib import pyplot
 import numpy as np
-import os
+from matplotlib import pyplot
+
+
+def plot_randomized(model: object, fname: str, show: bool = False) -> None:
+	"""
+	Plots the randomization test results.
+
+	Parameters:
+	model (Model): The Model object containing the samples.
+	fname (str): The filename where the plot will be saved.
+	show (bool): If True, the plot will be displayed. Default is False.
 
-def plot_randomized(model, fplot = None):
-	# Plot the randomization test results
+	Returns:
+	None
+	"""
 	
 	if model.random_p < model.p_value:
 		null_hypothesis_txt = "Dates are not %s distributed." % ("uniformly" if model.uniform else "normally")
 	else:
 		null_hypothesis_txt = "Dates are %s distributed." % ("uniformly" if model.uniform else "normally")
 	
 	perc_lower = (model.p_value * 100) / 2
 	perc_upper = 100 - perc_lower
 	
-	fig = pyplot.figure(figsize = (15, 4))
-	pyplot.fill_between(model.years - 1950, model.random_lower, model.random_upper, color = "lightgrey", label = "%0.2f%% of randomized dates" % (perc_upper - perc_lower))
-	pyplot.plot(model.years - 1950, model.summed, color = "k", label = "Observed dates")
+	fig = pyplot.figure(figsize=(15, 4))
+	pyplot.fill_between(model.years - 1950, model.random_lower, model.random_upper, color="lightgrey",
+	                    label="%0.2f%% of randomized dates" % (perc_upper - perc_lower))
+	pyplot.plot(model.years - 1950, model.summed, color="k", label="Observed dates")
 	idxs = np.where(model.random_upper > 0)[0]
 	idx1, idx2 = idxs.min(), idxs.max()
 	pyplot.xlim(model.years[int(idx1)] - 1950, model.years[int(idx2)] - 1950)
 	pyplot.gca().invert_xaxis()
 	pyplot.xlabel("Calendar age (yrs BC)")
 	pyplot.ylabel("Summed p")
-	pyplot.annotate("p: %0.5f\n%s" % (model.random_p, null_hypothesis_txt), xy = (0.05, 0.95), xycoords = "axes fraction", fontsize = 12, horizontalalignment = "left", verticalalignment = "top")
+	pyplot.annotate("p: %0.5f\n%s" % (model.random_p, null_hypothesis_txt), xy=(0.05, 0.95), xycoords="axes fraction",
+	                fontsize=12, horizontalalignment="left", verticalalignment="top")
 	pyplot.legend()
 	pyplot.tight_layout()
-	if fplot is None:
+	pyplot.savefig(fname)
+	if show:
 		pyplot.show()
-	else:
-		pyplot.savefig(fplot)
 	pyplot.close()
 
-def plot_clusters(model, fplot = None):
-	# Plot Silhouette and p-value for solutions with different numbers of clusters
+
+def plot_clusters(model: object, fname: str, show: bool = False) -> None:
+	"""
+	Plots Silhouette and p-value for solutions with different numbers of clusters.
+
+	Parameters:
+	model (Model): The Model object containing the samples.
+	fname (str): The filename where the plot will be saved.
+	show (bool): If True, the plot will be displayed. Default is False.
+
+	Returns:
+	None
+	"""
 	
-	clu_ns = np.array(sorted(list(model.clusters.keys())), dtype = int)
+	clu_ns = np.array(sorted(list(model.clusters.keys())), dtype=int)
 	ps_plot = np.array([model.cluster_ps[clu_n] for clu_n in clu_ns])
 	sils_plot = np.array([model.cluster_sils[clu_n] for clu_n in clu_ns])
 	
 	color1 = "#414487"
 	color2 = "#7AD151"
 	color3 = "#FDE725"
 	
 	fig, ax1 = pyplot.subplots()
 	
 	ax1.set_xlabel("Clusters")
-	ax1.set_ylabel("Mean Silhouette Coefficient", color = color1)
-	ax1.plot(clu_ns, sils_plot, color = color1)
-	ax1.plot(clu_ns, sils_plot, ".", color = color1)
-	ax1.tick_params(axis = "y", labelcolor = color1)
+	ax1.set_ylabel("Mean Silhouette Coefficient", color=color1)
+	ax1.plot(clu_ns, sils_plot, color=color1)
+	ax1.plot(clu_ns, sils_plot, ".", color=color1)
+	ax1.tick_params(axis="y", labelcolor=color1)
 	
 	ax2 = ax1.twinx()
-	ax2.set_ylabel("p", color = color2)
-	ax2.plot(clu_ns, ps_plot, color = color2)
-	ax2.plot(clu_ns, ps_plot, ".", color = color2)
+	ax2.set_ylabel("p", color=color2)
+	ax2.plot(clu_ns, ps_plot, color=color2)
+	ax2.plot(clu_ns, ps_plot, ".", color=color2)
 	if model.cluster_opt_n is not None:
-		ax2.plot([model.cluster_opt_n, model.cluster_opt_n], [0, max(ps_plot.max(), sils_plot.max())], color = color3, linewidth = 0.7, label = "Optimal no. of clusters")
+		ax2.plot([model.cluster_opt_n, model.cluster_opt_n], [0, max(ps_plot.max(), sils_plot.max())], color=color3,
+		         linewidth=0.7, label="Optimal no. of clusters")
 	if model.p_value is not None:
-		ax2.plot([clu_ns[0], clu_ns[-1]], [model.p_value, model.p_value], "--", color = color2, linewidth = 0.7)
-		ax2.annotate("p = %0.3f" % (model.p_value), xy = (clu_ns.mean(), model.p_value), xytext = (0, -3), textcoords = "offset pixels", va = "top", ha = "center", color = color2)
-	ax2.tick_params(axis = "y", labelcolor = color2)
+		ax2.plot([clu_ns[0], clu_ns[-1]], [model.p_value, model.p_value], "--", color=color2, linewidth=0.7)
+		ax2.annotate("p = %0.3f" % (model.p_value), xy=(clu_ns.mean(), model.p_value), xytext=(0, -3),
+		             textcoords="offset pixels", va="top", ha="center", color=color2)
+	ax2.tick_params(axis="y", labelcolor=color2)
 	
 	pyplot.xticks(clu_ns, clu_ns)
 	pyplot.legend()
 	
 	fig.tight_layout()
-	if fplot is None:
+	pyplot.savefig(fname)
+	if show:
 		pyplot.show()
-	else:
-		pyplot.savefig(fplot)
 	pyplot.close()
 
-def save_outliers(model, fname):
-	
-	txt = ""
+
+def save_outliers(model: object, fname: str) -> None:
+	"""
+	Saves the outliers and outlier candidates to a file.
+
+	Parameters:
+	model (Model): The Model object containing the samples.
+	fname (str): The filename where the outliers will be saved.
+
+	Returns:
+	None
+	"""
+	txt = "Eliminated outliers:\n"
 	outliers = model.outliers
 	if outliers:
-		txt += "Eliminated outliers:\n"
 		txt += "%s\n" % (", ".join(outliers))
+	else:
+		txt += "None\n"
+	txt += "\nOutlier candidates:\n"
 	candidates = model.outlier_candidates
 	if candidates:
-		txt += "\nOutlier candidates:\n"
 		txt += "%s\n" % (", ".join(candidates))
+	else:
+		txt += "None\n"
 	
 	with open(fname, "w") as file:
 		file.write(txt)
 
-def save_results_csv(model, fcsv):
-	# Save results to a CSV file
+
+def save_results_csv(model: object, fcsv: str) -> None:
+	"""
+	Saves the results to a CSV file.
+
+	Parameters:
+	model (Model): The Model object containing the samples.
+	fcsv (str): The filename where the results will be saved.
+
+	Returns:
+	None
+	"""
 	
 	def _format_year(value):
 		
 		if value is None:
 			return "None"
 		return "%0.2f" % (-(value - 1950))
 	
 	samples = list(model.samples.keys())
 	
 	def _sum_range(rng):
 		if None in rng:
 			return -1
 		return sum(rng)
 	
-	samples = sorted(samples, key = lambda name: [
-		model.samples[name].group, 
-		model.samples[name].phase, 
+	samples = sorted(samples, key=lambda name: [
+		model.samples[name].group,
+		model.samples[name].phase,
 		_sum_range(model.samples[name].likelihood_range)
 	])
 	
 	cluster = dict([(name, None) for name in samples])
 	if model.is_clustered:
 		m_clusters = model.clusters[model.cluster_opt_n]
 		for clu in m_clusters:
 			for name in m_clusters[clu]:
 				cluster[name] = clu
 	
 	with open(fcsv, "w") as file:
-		file.write("Name;Context;Area;C-14 Date;C-14 Uncertainty;Long-Lived;Redeposited;Outlier;Group;Phase;Cluster;Unmodeled From (CE);Unmodeled To (CE);Modeled From (CE);Modeled To (CE)\n")
+		file.write(
+			"Name;Context;Area;C-14 Date;C-14 Uncertainty;Long-Lived;Redeposited;Outlier;Group;Phase;Cluster;Unmodeled From (CE);Unmodeled To (CE);Modeled From (CE);Modeled To (CE)\n")
 		for name in samples:
 			likelihood_min, likelihood_max = model.samples[name].likelihood_range
 			posterior_min, posterior_max = model.samples[name].posterior_range
 			file.write('''"%s";"%s";"%s";%0.2f;%0.2f;%s;%s;%s;%s;%s;%s;%s;%s;%s;%s\n''' % (
-				name, model.samples[name].context, model.samples[name].area, 
-				model.samples[name].age, model.samples[name].uncertainty, 
-				int(model.samples[name].long_lived), int(model.samples[name].redeposited), int(model.samples[name].outlier), 
-				model.samples[name].group, model.samples[name].phase, cluster[name], 
+				name, model.samples[name].context, model.samples[name].area,
+				model.samples[name].age, model.samples[name].uncertainty,
+				int(model.samples[name].long_lived), int(model.samples[name].redeposited),
+				int(model.samples[name].outlier),
+				model.samples[name].group, model.samples[name].phase, cluster[name],
 				_format_year(likelihood_min), _format_year(likelihood_max),
 				_format_year(posterior_min), _format_year(posterior_max)
 			))
-
```

### Comparing `sitesyncro-0.9.2/src/sitesyncro/utils/fnc_radiocarbon.py` & `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_radiocarbon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import os
+
 import numpy as np
 from scipy.interpolate import interp1d
 
-def get_curve(curve_name = 'intcal20.14c'):
-	# Load calibration curve
-	# returns: [[calendar year BP, C-14 year, uncertainty], ...], sorted by calendar years
+
+def get_curve(curve_name: str = 'intcal20.14c') -> np.ndarray:
+	"""
+	Load a calibration curve.
+
+	Parameters:
+	curve_name (str): The name of the calibration curve file. Default is 'intcal20.14c'.
+
+	Returns:
+	np.ndarray: A 2D array containing the calibration curve data. Each row represents a calendar year BP, C-14 year, and uncertainty.
+	"""
 	
 	fcurve = os.path.join("OxCal\\bin", curve_name)
 	
 	if not os.path.isfile(fcurve):
 		raise ValueError("Calibration curve not found")
 	
 	with open(fcurve, "r", encoding="latin1") as f:
@@ -18,44 +27,50 @@
 	for line in data:
 		line = line.strip()
 		if not line:
 			continue
 		if line.startswith("#"):
 			continue
 		cal_curve.append([np.float64(value) for value in line.split(",")])
-	cal_curve = np.array(cal_curve, dtype = np.float64)
-	cal_curve = cal_curve[np.argsort(cal_curve[:,0])]
+	cal_curve = np.array(cal_curve, dtype=np.float64)
+	cal_curve = cal_curve[np.argsort(cal_curve[:, 0])]
 	
-	years = np.arange(np.floor(cal_curve[:,0].min()), np.ceil(cal_curve[:,0].max()) + 1, 1)
+	years = np.arange(np.floor(cal_curve[:, 0].min()), np.ceil(cal_curve[:, 0].max()) + 1, 1)
 	cal_curve = np.vstack((
 		years,
-		interp1d(cal_curve[:,0], cal_curve[:,1], kind = "quadratic")(years),
-		interp1d(cal_curve[:,0], cal_curve[:,2], kind = "linear")(years),
+		interp1d(cal_curve[:, 0], cal_curve[:, 1], kind="quadratic")(years),
+		interp1d(cal_curve[:, 0], cal_curve[:, 2], kind="linear")(years),
 	)).T
 	
 	return cal_curve.astype(np.float64)
 
-def calibrate(age, uncert, curve, date_type = 'R'):
-	# Calibrate a C-14 date
-	# Calibration formula as defined by Bronk Ramsey 2008, doi: 10.1111/j.1475-4754.2008.00394.x
-	#
-	# age: C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U'
-	# uncert: uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U'
-	# curve: [[calendar year BP, C-14 year, uncertainty], ...]
-	# date_type: 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution
-	#
-	# returns np.array([p, ...]), where p is the probability of the calendar year
+
+def calibrate(age: float, uncertainty: float, curve: np.ndarray, date_type: str = 'R') -> np.ndarray:
+	"""
+	Calibrate a C-14 date.
+	
+	Calibration formula as defined by Bronk Ramsey 2008, doi: 10.1111/j.1475-4754.2008.00394.x.
+	
+	Parameters:
+	age (float): C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U'.
+	uncertainty (float): Uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U'.
+	curve (np.ndarray): A 2D array containing the calibration curve data. Each row represents a calendar year BP, C-14 year, and uncertainty.
+	date_type (str): 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution. Default is 'R'.
+
+	Returns:
+	np.ndarray: An array of probabilities for each calendar year.
+	"""
 	
 	if date_type == 'R':
-		sigma_sum = uncert**2 + curve[:,2]**2
-		dist = (np.exp(-(age - curve[:,1])**2 / (2 * sigma_sum)) / np.sqrt(sigma_sum))
+		sigma_sum = uncertainty ** 2 + curve[:, 2] ** 2
+		dist = (np.exp(-(age - curve[:, 1]) ** 2 / (2 * sigma_sum)) / np.sqrt(sigma_sum))
 	elif date_type == 'U':
-		dist = np.ones(curve.shape[0], dtype = np.float64)
-		dist[curve[:,0] < age - uncertainty] = 0
-		dist[curve[:,0] > age + uncertainty] = 0
+		dist = np.ones(curve.shape[0], dtype=np.float64)
+		dist[curve[:, 0] < age - uncertainty] = 0
+		dist[curve[:, 0] > age + uncertainty] = 0
 	else:
 		raise Exception("Invalid date type specified: %s (must be 'R' or 'U')" % (date_type))
 	
 	s = dist.sum()
 	if s > 0:
 		dist /= s
```

### Comparing `sitesyncro-0.9.2/src/sitesyncro/utils/fnc_simulate.py` & `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_simulate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,87 @@
-from sitesyncro.utils.fnc_radiocarbon import (calibrate)
-from sitesyncro.utils.fnc_stat import (calc_sum, calc_mean_std, calc_percentiles, samples_to_distributions)
-from sitesyncro.utils.fnc_mp import (process_mp)
+from typing import Any, List
 
 import numpy as np
-from tqdm import tqdm
 from scipy.stats import norm
+from tqdm import tqdm
+
+from sitesyncro.utils.fnc_mp import (process_mp)
+from sitesyncro.utils.fnc_radiocarbon import (calibrate)
+from sitesyncro.utils.fnc_stat import (calc_sum, calc_mean_std, calc_percentiles, samples_to_distributions)
 
-def generate_random_distributions(dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform):
-	# Generate sets of randomized distributions based on observed distributions
-	#
-	# dates_n: number of dates to generate
-	# t_param1: mean or median of the calendar ages
-	# t_param2: standard deviation or range of the calendar ages
-	# uncertainties: [uncertainty, ...] pool of uncertainties to simulate C-14 dates
-	# uncertainty_base: base uncertainty to calculate uncertainty based on C-14 age if pool is not available
-	# curve: [[CalBP, ConvBP, CalSigma], ...]
-	# uniform: flag indicating whether to use a uniform distribution for the calendar ages
+
+def generate_random_distributions(dates_n: int, t_param1: float, t_param2: float, uncertainties: List[float],
+                                  uncertainty_base: float, curve: np.ndarray, uniform: bool,
+                                  max_iterations: int = 10000) -> List[np.ndarray]:
+	"""
+	Generate sets of randomized distributions based on observed distributions.
+
+	Parameters:
+	dates_n (int): Number of dates to generate.
+	t_param1 (float): Mean or median of the calendar ages.
+	t_param2 (float): Standard deviation or range of the calendar ages.
+	uncertainties (list): Pool of uncertainties to simulate C-14 dates.
+	uncertainty_base (float): Base uncertainty to calculate uncertainty based on C-14 age if pool is not available.
+	curve (np.ndarray): A 2D array containing the calibration curve data. Each row represents a calendar year BP, C-14 year, and uncertainty.
+	uniform (bool): Flag indicating whether to use a uniform distribution for the calendar ages.
+	max_iterations (int): Maximum number of iterations for the adjustment process. Default is 10000.
+
+	Returns:
+	List[np.ndarray]: List of generated distributions.
+	"""
 	
-	def _sim_age():
+	def _sim_age(t_param1, t_param2, uniform, curve):
 		# Generate a random calendar age
 		if uniform:
 			t = np.random.uniform(t_param1 - t_param2, t_param1 + t_param2)
 		else:
 			t = np.random.normal(t_param1, t_param2)
 		# Find the closest index in the calibration curve
 		idx = np.argmin(np.abs(curve[:, 0] - t))
 		# Get the corresponding radiocarbon age
 		age = curve[idx, 1]
 		return age
 	
-	dates = []
-	distributions = []
-	for i in range(dates_n):
-		# Generate a random calendar age
-		age = _sim_age()
-		# Calculate the standard deviation for the date
-		if uncertainties:
-			stdev = np.random.choice(uncertainties)
-		else:
-			stdev = uncertainty_base * np.exp(age / (2 * 8033))
-		# Append the date and its standard deviation to the dates list
-		dates.append([age, stdev])
-		# Calibrate the date and append the distribution to the distributions list
-		distribution = calibrate(age, stdev, curve)
-		distributions.append(distribution)
+	def _gen_distributions(dates_n, uncertainties, uncertainty_base, t_param1, t_param2, uniform, curve):
+		dates = []
+		distributions = []
+		for i in range(dates_n):
+			# Generate a random calendar age
+			age = _sim_age(t_param1, t_param2, uniform, curve)
+			# Calculate the standard deviation for the date
+			if uncertainties:
+				stdev = np.random.choice(uncertainties)
+			else:
+				stdev = uncertainty_base * np.exp(age / (2 * 8033))
+			# Append the date and its standard deviation to the dates list
+			dates.append([age, stdev])
+			# Calibrate the date and append the distribution to the distributions list
+			distribution = calibrate(age, stdev, curve)
+			distributions.append(distribution)
+		return dates, distributions
 	
-	# Sum the distributions of the generated dates
-	dist_summed = calc_sum(distributions)
+	def _analyze(distributions, uniform, curve):
+		# Sum the distributions
+		dist_summed = calc_sum(distributions)
+		median_sum, range_sum, mean_sum, std_sum = None, None, None, None
+		if uniform:
+			# Calculate weighted median and range
+			median_sum = np.average(curve[:, 0], weights=dist_summed)
+			range_sum = np.sqrt(np.average((curve[:, 0] - median_sum) ** 2, weights=dist_summed))
+		else:
+			# Calculate the mean and standard deviation of the summed distribution
+			mean_sum, std_sum = calc_mean_std(curve[:, 0], dist_summed)
+		return median_sum, range_sum, mean_sum, std_sum
 	
-	if uniform:
-		# Calculate weighted median and range
-		median_sum = np.average(curve[:, 0], weights=dist_summed)
-		range_sum = np.sqrt(np.average((curve[:, 0] - median_sum) ** 2, weights=dist_summed))
-	else:
-		# Calculate the mean and standard deviation of the summed distribution
-		mean_sum, std_sum = calc_mean_std(curve[:, 0], dist_summed)
+	dates, distributions = _gen_distributions(dates_n, uncertainties, uncertainty_base, t_param1, t_param2, uniform,
+	                                          curve)
+	median_sum, range_sum, mean_sum, std_sum = _analyze(distributions, uniform, curve)
 	
-	curve_min = curve[:,1].min()
-	curve_max = curve[:,1].max()
+	curve_min = curve[:, 1].min()
+	curve_max = curve[:, 1].max()
 	
 	# Adjust the dates until the mean and standard deviation of the summed distribution are close to the desired values
 	iteration = 0
 	scaling_factor = 1.0
 	if uniform:
 		c_threshold = t_param2 * 0.01
 	else:
@@ -72,110 +92,142 @@
 		else:
 			c = max(abs(mean_sum - t_param1), abs(std_sum - t_param2))
 		
 		if c <= c_threshold:
 			break
 		
 		iteration += 1
+		if iteration > max_iterations:
+			# Re-initialize
+			dates, distributions = _gen_distributions(dates_n, uncertainties, uncertainty_base, t_param1, t_param2,
+			                                          uniform, curve)
+			median_sum, range_sum, mean_sum, std_sum = _analyze(distributions, uniform, curve)
+			iteration = 0
+			scaling_factor = 1.0
+			continue
 		
 		# Randomly select a date to adjust
 		i = np.random.choice(dates_n)
 		age_new = dates[i][0]
 		if uniform:
 			age_new += 1 * (t_param1 - median_sum)
 			age_new *= 1 + scaling_factor * ((t_param2 / range_sum) - 1)
 		else:
 			age_new += (t_param1 - mean_sum)
 			age_new *= 1 + scaling_factor * ((t_param2 / std_sum) - 1)
 		if (age_new < curve_min) or (age_new > curve_max):
-			age_new = _sim_age()
+			age_new = _sim_age(t_param1, t_param2, uniform, curve)
 		dates[i][0] = age_new
 		distributions[i] = calibrate(dates[i][0], dates[i][1], curve)
-		
 		# Recalculate the sum of the distributions and their mean or median
-		dist_summed = calc_sum(distributions)
-		if uniform:
-			median_sum = np.average(curve[:, 0], weights=dist_summed)
-			range_sum = np.sqrt(np.average((curve[:, 0] - median_sum) ** 2, weights=dist_summed))
-		else:
-			mean_sum, std_sum = calc_mean_std(curve[:, 0], dist_summed)
+		median_sum, range_sum, mean_sum, std_sum = _analyze(distributions, uniform, curve)
 		# Decrease the scaling factor
 		scaling_factor *= 0.999
 	
 	return distributions
 
-def calculate_parameters(years, distribution, uniform):
+
+def calculate_parameters(years: np.ndarray, distribution: np.ndarray, uniform: bool) -> (float, float):
+	"""
+	Calculate parameters based on the given distribution.
+
+	Parameters:
+	years (np.ndarray): Array of years.
+	distribution (np.ndarray): Array of probabilities for each year.
+	uniform (bool): Flag indicating whether to use a uniform distribution for the calendar ages.
+
+	Returns:
+	(t_param1, t_param2)
+		- t_param1: Mean or median of the calendar ages.
+		- t_param2: Standard deviation or range of the calendar ages.
+	"""
 	if uniform:
 		# Calculate weighted median and range of the summed distribution
 		t_median = np.average(years, weights=distribution)
 		t_range = np.sqrt(np.average((years - t_median) ** 2, weights=distribution))
 		t_param1, t_param2 = t_median, t_range
 	else:
 		# Calculate the mean and standard deviation of the summed distribution
 		t_mean, t_std = calc_mean_std(years, distribution)
 		t_param1, t_param2 = t_mean, t_std
-
+	
 	return t_param1, t_param2
 
 
-def worker_fnc(params, dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform):
-	
-	return generate_random_distributions(dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform)
+def worker_fnc(params: Any, dates_n: int, t_param1: float, t_param2: float, uncertainties: List[float],
+               uncertainty_base: float, curve: np.ndarray, uniform: bool) -> np.ndarray:
+	return calc_sum(
+		generate_random_distributions(dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform))
 
-def collect_fnc(data, results, pbar):
-	
-	# data = distributions
-	# distributions = [[p, ...], ...]
-	
+
+def collect_fnc(data: np.ndarray, results: List[np.ndarray], pbar: tqdm) -> None:
+	# data = dist_sum
+	# dist_sum = [p, ...]
 	pbar.update(1)
 	results.append(data)
 
-def test_distributions(model, max_cpus = -1, max_queue_size = 100):
+
+def test_distributions(model: object, max_cpus: int = -1, max_queue_size: int = -1) -> (
+		np.ndarray, np.ndarray, np.ndarray, float):
+	"""
+	Test if the samples in the model are distributed uniformly / normally in time
+
+	Parameters:
+	model (Model): The Model object containing the samples.
+	max_cpus (int): Maximum number of CPUs to use for multiprocessing. Default is -1 (use all available CPUs).
+	max_queue_size (int): Maximum size of the queue for multiprocessing. Default is -1 (no limit).
+
+	Returns:
+	(sum_obs, sums_rnd_lower, sums_rnd_upper, p)
+		- sum_obs: Sum of the observed probability distributions of the sample dates.
+		- sums_rnd_lower: Lower bound of the randomized sum of the probability distributions.
+		- sums_rnd_upper: Upper bound of the randomized sum of the probability distributions.
+		- p: P-value for the test.
+	"""
 	
 	distributions, _, _ = samples_to_distributions(model.samples.values())
 	
 	dates_n = len(distributions)
 	
 	if dates_n < 3:
 		raise Exception("Insufficient number samples for testing.")
 	
 	print("Testing %d distributions" % dates_n)
 	
 	sum_obs = calc_sum(distributions)
 	years = model.curve[:, 0]
 	t_param1, t_param2 = calculate_parameters(years, sum_obs, model.uniform)
 	
-	distributions_rnd = []
 	sums = []
 	sums_prev = None
 	c = 0
 	todo = model.npass
-	params_list = list(range(model.npass))
-	with tqdm(total=todo) as pbar:
-		pbar.total = model.npass*2
+	with tqdm(total=todo * 2) as pbar:
 		pbar.set_description("Convergence: %0.3f" % (c))
 		while True:
-			process_mp(worker_fnc, params_list, [dates_n, t_param1, t_param2, model.uncertainties, model.uncertainty_base, model.curve, model.uniform],
-		           collect_fnc = collect_fnc, collect_args = [distributions_rnd, pbar],
-		           max_cpus = max_cpus, max_queue_size = max_queue_size)
-			if len(distributions_rnd) >= todo:
-				sums += [calc_sum(dists) for dists in distributions_rnd[-(len(distributions_rnd) - len(sums)):]]
-				sums_m = np.array(sums).mean(axis = 0)
+			process_mp(worker_fnc, range(max(4, (todo - len(sums)) + 1)),
+			           [dates_n, t_param1, t_param2, model.uncertainties, model.uncertainty_base, model.curve,
+			            model.uniform],
+			           collect_fnc=collect_fnc, collect_args=[sums, pbar],
+			           max_cpus=max_cpus, max_queue_size=max_queue_size)
+			if len(sums) >= todo:
+				sums_m = np.array(sums).mean(axis=0)
 				if sums_prev is not None:
-					c = ((sums_prev * sums_m).sum()**2) / ((sums_prev**2).sum() * (sums_m**2).sum())
+					c = ((sums_prev * sums_m).sum() ** 2) / ((sums_prev ** 2).sum() * (sums_m ** 2).sum())
 					pbar.set_description("Convergence: %0.3f" % (c))
 				sums_prev = sums_m.copy()
 				if c >= model.convergence:
 					break
 				todo *= 2
-				pbar.total = max(todo, model.npass*2)
+				pbar.total = max(todo, model.npass * 2)
+				pbar.refresh()
 	
 	sums_rnd = np.array(sums)
 	
-	mask = (sums_rnd.std(axis = 0) > 0)
-	p = (1 - norm(sums_rnd[:,mask].mean(axis = 0), sums_rnd[:,mask].std(axis = 0)).cdf(sum_obs[mask])).min()
+	mask = (sums_rnd.std(axis=0) > 0)
+	p = (1 - norm(sums_rnd[:, mask].mean(axis=0), sums_rnd[:, mask].std(axis=0)).cdf(sum_obs[mask])).min()
 	
 	perc_lower = (model.p_value * 100) / 2
 	perc_upper = 100 - perc_lower
 	sums_rnd_lower, sums_rnd_upper = calc_percentiles(sums_rnd, perc_lower, perc_upper)
 	
 	return sum_obs, sums_rnd_lower, sums_rnd_upper, p
```

### Comparing `sitesyncro-0.9.2/src/sitesyncro.egg-info/SOURCES.txt` & `sitesyncro-0.9.3/src/sitesyncro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

