# Comparing `tmp/deepdog-0.8.1.tar.gz` & `tmp/deepdog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.8.1.tar", max compression
+gzip compressed data, was "deepdog-1.0.0.tar", max compression
```

## Comparing `deepdog-0.8.1.tar` & `deepdog-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      605 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0     7661 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/bayes_run_with_ss.py
--rw-r--r--   0        0        0        0 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/cli/__init__.py
--rw-r--r--   0        0        0       80 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/cli/probs/__init__.py
--rw-r--r--   0        0        0     1730 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/cli/probs/args.py
--rw-r--r--   0        0        0     6244 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/cli/probs/dicts.py
--rw-r--r--   0        0        0     2823 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/cli/probs/main.py
--rw-r--r--   0        0        0      161 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/direct_monte_carlo/__init__.py
--rw-r--r--   0        0        0      461 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/direct_monte_carlo/compose_filter.py
--rw-r--r--   0        0        0     5103 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/direct_monte_carlo/direct_mc.py
--rw-r--r--   0        0        0     3920 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/direct_monte_carlo/dmc_filters.py
--rw-r--r--   0        0        0     1700 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/indexify/__init__.py
--rw-r--r--   0        0        0     2432 2024-04-28 09:29:13.797283 deepdog-0.8.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       73 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/meta.py
--rw-r--r--   0        0        0    13688 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     4777 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/results/__init__.py
--rw-r--r--   0        0        0     5846 2024-04-28 09:29:13.809284 deepdog-0.8.1/deepdog/results/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      110 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0      297 2024-04-28 09:29:13.789283 deepdog-0.8.1/deepdog/subset_simulation/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9024 2024-04-28 09:29:13.793283 deepdog-0.8.1/deepdog/subset_simulation/__pycache__/subset_simulation_impl.cpython-39.pyc
--rw-r--r--   0        0        0    11428 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2024-04-28 09:28:40.203611 deepdog-0.8.1/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0     1084 2024-04-28 09:28:40.207611 deepdog-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 deepdog-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      605 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0     7661 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/bayes_run_with_ss.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/cli/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/cli/probs/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/cli/probs/args.py
+-rw-r--r--   0        0        0     6243 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/cli/probs/dicts.py
+-rw-r--r--   0        0        0     2945 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/cli/probs/main.py
+-rw-r--r--   0        0        0      161 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/direct_monte_carlo/__init__.py
+-rw-r--r--   0        0        0      461 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/direct_monte_carlo/compose_filter.py
+-rw-r--r--   0        0        0     9069 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/direct_monte_carlo/direct_mc.py
+-rw-r--r--   0        0        0     7127 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/direct_monte_carlo/dmc_filters.py
+-rw-r--r--   0        0        0     1700 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/indexify/__init__.py
+-rw-r--r--   0        0        0     2432 2024-05-01 20:51:06.758696 deepdog-1.0.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       73 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/meta.py
+-rw-r--r--   0        0        0    12392 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     4858 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/results/__init__.py
+-rw-r--r--   0        0        0     5927 2024-05-01 20:51:06.774697 deepdog-1.0.0/deepdog/results/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      110 2024-05-01 20:50:35.273014 deepdog-1.0.0/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-01 20:51:06.750696 deepdog-1.0.0/deepdog/subset_simulation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9024 2024-05-01 20:51:06.754696 deepdog-1.0.0/deepdog/subset_simulation/__pycache__/subset_simulation_impl.cpython-39.pyc
+-rw-r--r--   0        0        0    11428 2024-05-01 20:50:35.277014 deepdog-1.0.0/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2024-05-01 20:50:35.277014 deepdog-1.0.0/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0     1084 2024-05-01 20:50:35.277014 deepdog-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.0.0/PKG-INFO
```

### Comparing `deepdog-0.8.1/deepdog/__init__.py` & `deepdog-1.0.0/deepdog/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.8.1/deepdog/bayes_run.py` & `deepdog-1.0.0/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.8.1/deepdog/bayes_run_simulpairs.py` & `deepdog-1.0.0/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.8.1/deepdog/bayes_run_with_ss.py` & `deepdog-1.0.0/deepdog/bayes_run_with_ss.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.8.1/deepdog/cli/probs/args.py` & `deepdog-1.0.0/deepdog/cli/probs/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,26 +27,14 @@
 	)
 	parser.add_argument(
 		"--indexify-json",
 		help="A json file with the indexify config for parsing job indexes. Will skip if not present",
 		default="",
 	)
 	parser.add_argument(
-		"--seed-index",
-		type=int,
-		help='take an integer to append as a "seed" key with range at end of indexify dict. Skip if <= 0',
-		default=0,
-	)
-	parser.add_argument(
-		"--seed-fieldname",
-		type=str,
-		help='if --seed-index is set, the fieldname to append to the indexifier. "seed" by default',
-		default="seed",
-	)
-	parser.add_argument(
 		"--coalesced-keys",
 		type=str,
 		help="A comma separated list of strings over which to coalesce data. By default coalesce over all fields within model names, ignore file level names",
 		default="",
 	)
 	parser.add_argument(
 		"--uncoalesced-outfile",
```

### Comparing `deepdog-0.8.1/deepdog/cli/probs/dicts.py` & `deepdog-1.0.0/deepdog/cli/probs/dicts.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 	first_value = next(iter(next(iter(uncoalesced_model_dict.values())).values()))
 	model_field_names = set(first_value["_model_key_dict"].keys())
 	calculation_field_names = set(first_value["_calculation_key_dict"].keys())
 	if not (set(model_field_names).isdisjoint(calculation_field_names)):
 		_logger.info(f"Detected model field names {model_field_names}")
 		_logger.info(f"Detected calculation field names {calculation_field_names}")
-		raise ValueError(
+		_logger.warning(
 			f"model field names {model_field_names} and calculation {calculation_field_names} have an overlap, which is possibly a problem"
 		)
 	collected_fieldnames = list(model_field_names)
 	collected_fieldnames.extend(calculation_field_names)
 	collected_fieldnames.extend(["success", "count"])
 	_logger.info(f"Full uncoalesced fieldnames are {collected_fieldnames}")
 	with open(uncoalesced_output_filename, "w", newline="") as uncoalesced_output_file:
```

### Comparing `deepdog-0.8.1/deepdog/cli/probs/main.py` & `deepdog-1.0.0/deepdog/cli/probs/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,17 +47,21 @@
 		except AttributeError:
 			# we don't care if this is missing because we don't actually want it to be there
 			pass
 
 		indexifier = None
 		if args.indexify_json:
 			with open(args.indexify_json, "r") as indexify_json_file:
-				indexify_data = json.load(indexify_json_file)
-				if args.seed_index > 0:
-					indexify_data[args.seed_fieldname] = list(range(args.seed_index))
+				indexify_spec = json.load(indexify_json_file)
+				indexify_data = indexify_spec["indexes"]
+				if "seed_spec" in indexify_spec:
+					seed_spec = indexify_spec["seed_spec"]
+					indexify_data[seed_spec["field_name"]] = list(
+						range(seed_spec["num_seeds"])
+					)
 				# _logger.debug(f"Indexifier data looks like {indexify_data}")
 				indexifier = deepdog.indexify.Indexifier(indexify_data)
 
 		bayes_dir = pathlib.Path(args.bayesrun_directory)
 		out_files = [f for f in bayes_dir.iterdir() if f.name.endswith("bayesrun.csv")]
 		_logger.info(
 			f"Reading {len(out_files)} bayesrun.csv files in directory {args.bayesrun_directory}"
```

### Comparing `deepdog-0.8.1/deepdog/indexify/__init__.py` & `deepdog-1.0.0/deepdog/indexify/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.8.1/deepdog/indexify/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.0.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 09:28:40 2024 UTC, .py size: 1700 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 c816 2e66 a406 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 1bab 3266 a406 0000  a.........2f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6503 a005 6506 a101 5a07 6403 6404  Z.e...e...Z.d.d.
 00000060: 8400 5a08 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
 00000070: 5a09 6402 5300 2907 7ac7 0a50 726f 6261  Z.d.S.).z..Proba
@@ -40,16 +40,16 @@
 00000270: 5d18 7d01 7400 7401 8800 a002 a100 7c01  ].}.t.t.......|.
 00000280: 8302 8301 5600 0100 7102 6400 5300 a901  ....V...q.d.S...
 00000290: 4e29 03da 0464 6963 74da 037a 6970 da04  N)...dict..zip..
 000002a0: 6b65 7973 2902 da02 2e30 da01 78a9 01da  keys)....0..x...
 000002b0: 0564 6963 7473 a900 fa56 2f68 6f6d 652f  .dicts...V/home/
 000002c0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 000002d0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
-000002e0: 7973 6963 735f 6465 6570 646f 675f 302e  ysics_deepdog_0.
-000002f0: 382e 312f 6465 6570 646f 672f 696e 6465  8.1/deepdog/inde
+000002e0: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
+000002f0: 302e 302f 6465 6570 646f 672f 696e 6465  0.0/deepdog/inde
 00000300: 7869 6679 2f5f 5f69 6e69 745f 5f2e 7079  xify/__init__.py
 00000310: da09 3c67 656e 6578 7072 3e17 0000 00f3  ..<genexpr>.....
 00000320: 0000 0000 7a20 5f64 6963 745f 7072 6f64  ....z _dict_prod
 00000330: 7563 742e 3c6c 6f63 616c 733e 2e3c 6765  uct.<locals>.<ge
 00000340: 6e65 7870 723e 2904 da04 6c69 7374 da09  nexpr>)...list..
 00000350: 6974 6572 746f 6f6c 73da 0770 726f 6475  itertools..produ
 00000360: 6374 da06 7661 6c75 6573 7208 0000 0072  ct..valuesr....r
```

### Comparing `deepdog-0.8.1/deepdog/real_spectrum_run.py` & `deepdog-1.0.0/deepdog/real_spectrum_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,67 +108,14 @@
 		pair_inputs,
 		pair_phase_lows,
 		pair_phase_highs,
 		monte_carlo_count,
 		seed,
 	) = input
 
-	def fast_s_spin_qubit_tarucha_nonlocal_dipoleses(
-		dot_pair_inputs: numpy.ndarray, dipoleses: numpy.ndarray
-	) -> numpy.ndarray:
-		"""
-		No error correction here baby.
-		"""
-		ps = dipoleses[:, :, 0:3]
-		ss = dipoleses[:, :, 3:6]
-		ws = dipoleses[:, :, 6]
-
-		r1s = dot_pair_inputs[:, 0, 0:3]
-		r2s = dot_pair_inputs[:, 1, 0:3]
-		f1s = dot_pair_inputs[:, 0, 3]
-		# don't actually need, because we're assuming they're the same frequencies across the pair
-		# f2s = dot_pair_inputs[:, 1, 3]
-
-		diffses1 = r1s[:, None] - ss[:, None, :]
-		diffses2 = r2s[:, None] - ss[:, None, :]
-
-		norms1 = numpy.linalg.norm(diffses1, axis=3)
-		norms2 = numpy.linalg.norm(diffses2, axis=3)
-
-		alphses1 = (
-			(
-				3
-				* numpy.transpose(
-					numpy.transpose(
-						numpy.einsum("abcd,acd->abc", diffses1, ps) / (norms1**2)
-					)
-					* numpy.transpose(diffses1)
-				)[:, :, :, 0]
-			)
-			- ps[:, numpy.newaxis, :, 0]
-		) / (norms1**3)
-		alphses2 = (
-			(
-				3
-				* numpy.transpose(
-					numpy.transpose(
-						numpy.einsum("abcd,acd->abc", diffses2, ps) / (norms2**2)
-					)
-					* numpy.transpose(diffses2)
-				)[:, :, :, 0]
-			)
-			- ps[:, numpy.newaxis, :, 0]
-		) / (norms2**3)
-
-		bses = (1 / numpy.pi) * (
-			ws[:, None, :] / (f1s[:, None] ** 2 + ws[:, None, :] ** 2)
-		)
-
-		return numpy.einsum("...j->...", alphses1 * alphses2 * bses)
-
 	rng = numpy.random.default_rng(seed)
 	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
 	sample_dipoles = model.get_monte_carlo_dipole_inputs(
 		monte_carlo_count, None, rng_to_use=rng
 	)
 
 	current_sample = sample_dipoles
@@ -182,15 +129,15 @@
 		###
 		# vals = pdme.util.fast_nonlocal_spectrum.signarg(
 		# 	pdme.util.fast_nonlocal_spectrum.fast_s_nonlocal_dipoleses(
 		# 		numpy.array([pi]), current_sample
 		# 	)
 		#
 		vals = pdme.util.fast_nonlocal_spectrum.signarg(
-			fast_s_spin_qubit_tarucha_nonlocal_dipoleses(
+			pdme.util.fast_nonlocal_spectrum.fast_s_spin_qubit_tarucha_nonlocal_dipoleses(
 				numpy.array([pi]), current_sample
 			)
 		)
 		current_sample = current_sample[
 			numpy.all(
 				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
 				axis=1,
```

### Comparing `deepdog-0.8.1/deepdog/results/__init__.py` & `deepdog-1.0.0/deepdog/results/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 MODEL_REGEXES = [
 	r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)"
 ]
 
 FILE_SLUG_REGEXES = [
 	r"mock_tarucha-(?P<job_index>\d+)",
+	r"(?:(?P<mock>mock)_)?tarucha(?:_(?P<tarucha_run_id>\d+))?-(?P<job_index>\d+)",
 ]
 
 
 @dataclasses.dataclass
 class BayesrunOutputFilename:
 	timestamp: str
 	filename_slug: str
```

### Comparing `deepdog-0.8.1/deepdog/results/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.0.0/deepdog/results/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 09:28:40 2024 UTC, .py size: 4777 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,366 +1,371 @@
-00000000: 610d 0d0a 0000 0000 c816 2e66 a912 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 1bab 3266 fa12 0000  a.........2f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 3601 0000 6400  .....@...s6...d.
+00000020: 0005 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c07 5a07 6503 a008 6509 a101 5a0a  d.l.Z.e...e...Z.
-00000070: 6402 5a0b 6403 6701 5a0c 6404 6701 5a0d  d.Z.d.g.Z.d.g.Z.
-00000080: 6500 6a0e 4700 6405 6406 8400 6406 8302  e.j.G.d.d...d...
-00000090: 8301 5a0f 6500 6a0e 4700 6407 6408 8400  ..Z.e.j.G.d.d...
-000000a0: 6408 8302 8301 5a10 6500 6a0e 4700 6409  d.....Z.e.j.G.d.
-000000b0: 640a 8400 640a 8302 8301 5a11 6500 6a0e  d...d.....Z.e.j.
-000000c0: 4700 640b 640c 8400 640c 8302 8301 5a12  G.d.d...d.....Z.
-000000d0: 641f 640e 640f 8401 5a13 6514 6502 6a15  d.d.d...Z.e.e.j.
-000000e0: 6510 1900 6410 9c02 6411 6412 8404 5a16  e...d...d.d...Z.
-000000f0: 6502 6a17 6514 6514 6602 1900 6502 6a18  e.j.e.e.f...e.j.
-00000100: 6511 1900 6413 9c02 6414 6415 8404 5a19  e...d...d.d...Z.
-00000110: 6506 6a1a 650f 6416 9c02 6417 6418 8404  e.j.e.d...d.d...
-00000120: 5a1b 6514 6502 6a15 6502 6a17 6514 6514  Z.e.e.j.e.j.e.e.
-00000130: 6602 1900 1900 6419 9c02 641a 641b 8404  f.....d...d.d...
-00000140: 5a1c 6506 6a1a 6502 6a15 6505 6a1d 6a1e  Z.e.j.e.j.e.j.j.
-00000150: 1900 6512 641c 9c03 641d 641e 8404 5a1f  ..e.d...d.d...Z.
-00000160: 6401 5300 2920 e900 0000 004e 7a56 283f  d.S.) .....NzV(?
-00000170: 503c 7469 6d65 7374 616d 703e 5c64 7b38  P<timestamp>\d{8
-00000180: 7d2d 5c64 7b36 7d29 2d28 3f50 3c66 696c  }-\d{6})-(?P<fil
-00000190: 656e 616d 655f 736c 7567 3e2e 2a29 5c2e  ename_slug>.*)\.
-000001a0: 7265 616c 6461 7461 5c2e 6661 7374 5f66  realdata\.fast_f
-000001b0: 696c 7465 725c 2e62 6179 6573 7275 6e5c  ilter\.bayesrun\
-000001c0: 2e63 7376 7aca 6765 6f6d 5f28 3f50 3c78  .csvz.geom_(?P<x
-000001d0: 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50 3c78  min>-?\d+)_(?P<x
-000001e0: 6d61 783e 2d3f 5c64 2b29 5f28 3f50 3c79  max>-?\d+)_(?P<y
-000001f0: 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50 3c79  min>-?\d+)_(?P<y
-00000200: 6d61 783e 2d3f 5c64 2b29 5f28 3f50 3c7a  max>-?\d+)_(?P<z
-00000210: 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50 3c7a  min>-?\d+)_(?P<z
-00000220: 6d61 783e 2d3f 5c64 2b29 2d6f 7269 656e  max>-?\d+)-orien
-00000230: 7461 7469 6f6e 5f28 3f50 3c6f 7269 656e  tation_(?P<orien
-00000240: 7461 7469 6f6e 3e66 7265 657c 6669 7865  tation>free|fixe
-00000250: 6478 797c 6669 7865 647a 292d 6469 706f  dxy|fixedz)-dipo
-00000260: 6c65 5f63 6f75 6e74 5f28 3f50 3c61 7667  le_count_(?P<avg
-00000270: 5f66 696c 6c65 643e 5c64 2b29 5f28 3f50  _filled>\d+)_(?P
-00000280: 3c66 6965 6c64 5f6e 616d 653e 5c77 2a29  <field_name>\w*)
-00000290: 7a1f 6d6f 636b 5f74 6172 7563 6861 2d28  z.mock_tarucha-(
-000002a0: 3f50 3c6a 6f62 5f69 6e64 6578 3e5c 642b  ?P<job_index>\d+
-000002b0: 2963 0000 0000 0000 0000 0000 0000 0000  )c..............
-000002c0: 0000 0300 0000 4000 0000 7328 0000 0065  ......@...s(...e
-000002d0: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
-000002e0: 0065 0365 0464 023c 0065 056a 0665 0464  .e.e.d.<.e.j.e.d
-000002f0: 033c 0064 0453 0029 05da 1642 6179 6573  .<.d.S.)...Bayes
-00000300: 7275 6e4f 7574 7075 7446 696c 656e 616d  runOutputFilenam
-00000310: 65da 0974 696d 6573 7461 6d70 da0d 6669  e..timestamp..fi
-00000320: 6c65 6e61 6d65 5f73 6c75 67da 0470 6174  lename_slug..pat
-00000330: 684e 2907 da08 5f5f 6e61 6d65 5f5f da0a  hN)...__name__..
-00000340: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000350: 616c 6e61 6d65 5f5f da03 7374 72da 0f5f  alname__..str.._
-00000360: 5f61 6e6e 6f74 6174 696f 6e73 5f5f da07  _annotations__..
-00000370: 7061 7468 6c69 62da 0450 6174 68a9 0072  pathlib..Path..r
-00000380: 0d00 0000 720d 0000 00fa 552f 686f 6d65  ....r.....U/home
-00000390: 2f6a 656e 6b69 6e73 2f61 6765 6e74 2f77  /jenkins/agent/w
-000003a0: 6f72 6b73 7061 6365 2f67 6974 6561 2d70  orkspace/gitea-p
-000003b0: 6879 7369 6373 5f64 6565 7064 6f67 5f30  hysics_deepdog_0
-000003c0: 2e38 2e31 2f64 6565 7064 6f67 2f72 6573  .8.1/deepdog/res
-000003d0: 756c 7473 2f5f 5f69 6e69 745f 5f2e 7079  ults/__init__.py
-000003e0: 7202 0000 0016 0000 0073 0600 0000 0a02  r........s......
-000003f0: 0801 0801 7202 0000 0063 0000 0000 0000  ....r....c......
-00000400: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000410: 0000 7330 0000 0065 005a 0164 005a 0264  ..s0...e.Z.d.Z.d
-00000420: 015a 0365 046a 0565 0665 0666 0219 0064  .Z.e.j.e.e.f...d
-00000430: 029c 0164 0364 0484 045a 0764 0564 0684  ...d.d...Z.d.d..
-00000440: 005a 0864 0753 0029 08da 1442 6179 6573  .Z.d.S.)...Bayes
-00000450: 7275 6e43 6f6c 756d 6e50 6172 7365 647a  runColumnParsedz
-00000460: 490a 0963 6c61 7373 2066 6f72 2070 6172  I..class for par
-00000470: 7369 6e67 2061 2062 6179 6573 7275 6e20  sing a bayesrun 
-00000480: 7768 696c 6520 7075 6c6c 696e 6720 6365  while pulling ce
-00000490: 7274 6169 6e20 7370 6563 6961 6c20 6669  rtain special fi
-000004a0: 656c 6473 206f 7574 0a09 2901 da09 6772  elds out..)...gr
-000004b0: 6f75 7064 6963 7463 0200 0000 0000 0000  oupdictc........
-000004c0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-000004d0: 7322 0000 007c 0164 0119 007c 005f 0064  s"...|.d...|._.d
-000004e0: 0264 0384 007c 01a0 01a1 0044 0083 017c  .d...|.....D...|
-000004f0: 005f 0264 0053 0029 044e da0a 6669 656c  ._.d.S.).N..fiel
-00000500: 645f 6e61 6d65 6301 0000 0000 0000 0000  d_namec.........
-00000510: 0000 0003 0000 0004 0000 0053 0000 0073  ...........S...s
-00000520: 1e00 0000 6900 7c00 5d16 5c02 7d01 7d02  ....i.|.].\.}.}.
-00000530: 7c01 6400 6b03 7204 7c01 7c02 9302 7104  |.d.k.r.|.|...q.
-00000540: 5300 2901 7211 0000 0072 0d00 0000 2903  S.).r....r....).
-00000550: da02 2e30 da01 6bda 0176 720d 0000 0072  ...0..k..vr....r
-00000560: 0d00 0000 720e 0000 00da 0a3c 6469 6374  ....r......<dict
-00000570: 636f 6d70 3e25 0000 0073 0200 0000 0601  comp>%...s......
-00000580: 7a31 4261 7965 7372 756e 436f 6c75 6d6e  z1BayesrunColumn
-00000590: 5061 7273 6564 2e5f 5f69 6e69 745f 5f2e  Parsed.__init__.
-000005a0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-000005b0: 6d70 3e29 03da 0c63 6f6c 756d 6e5f 6669  mp>)...column_fi
-000005c0: 656c 64da 0569 7465 6d73 da10 6d6f 6465  eld..items..mode
-000005d0: 6c5f 6669 656c 645f 6469 6374 2902 da04  l_field_dict)...
-000005e0: 7365 6c66 7210 0000 0072 0d00 0000 720d  selfr....r....r.
-000005f0: 0000 0072 0e00 0000 da08 5f5f 696e 6974  ...r......__init
-00000600: 5f5f 2300 0000 7308 0000 0000 010a 0106  __#...s.........
-00000610: 0106 ff7a 1d42 6179 6573 7275 6e43 6f6c  ...z.BayesrunCol
-00000620: 756d 6e50 6172 7365 642e 5f5f 696e 6974  umnParsed.__init
-00000630: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00000640: 0000 0005 0000 0043 0000 0073 1600 0000  .......C...s....
-00000650: 6401 7c00 6a00 9b00 6402 7c00 6a01 9b00  d.|.j...d.|.j...
-00000660: 6403 9d05 5300 2904 4e7a 1542 6179 6573  d...S.).Nz.Bayes
-00000670: 7275 6e43 6f6c 756d 6e50 6172 7365 645b  runColumnParsed[
-00000680: 7a02 3a20 da01 5d29 0272 1600 0000 7218  z.: ..]).r....r.
-00000690: 0000 0029 0172 1900 0000 720d 0000 0072  ...).r....r....r
-000006a0: 0d00 0000 720e 0000 00da 075f 5f73 7472  ....r......__str
-000006b0: 5f5f 2900 0000 7302 0000 0000 017a 1c42  __)...s......z.B
-000006c0: 6179 6573 7275 6e43 6f6c 756d 6e50 6172  ayesrunColumnPar
-000006d0: 7365 642e 5f5f 7374 725f 5f4e 2909 7206  sed.__str__N).r.
-000006e0: 0000 0072 0700 0000 7208 0000 00da 075f  ...r....r......_
-000006f0: 5f64 6f63 5f5f da06 7479 7069 6e67 da04  _doc__..typing..
-00000700: 4469 6374 7209 0000 0072 1a00 0000 721c  Dictr....r....r.
-00000710: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-00000720: 0000 720e 0000 0072 0f00 0000 1d00 0000  ..r....r........
-00000730: 7306 0000 0008 0204 0418 0672 0f00 0000  s..........r....
-00000740: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000750: 0003 0000 0040 0000 0073 3000 0000 6500  .....@...s0...e.
-00000760: 5a01 6400 5a02 5500 6503 6a04 6505 6505  Z.d.Z.U.e.j.e.e.
-00000770: 6602 1900 6506 6401 3c00 6507 6506 6402  f...e.d.<.e.e.d.
-00000780: 3c00 6507 6506 6403 3c00 6404 5300 2905  <.e.e.d.<.d.S.).
-00000790: da13 4261 7965 7372 756e 4d6f 6465 6c52  ..BayesrunModelR
-000007a0: 6573 756c 74da 1170 6172 7365 645f 6d6f  esult..parsed_mo
-000007b0: 6465 6c5f 6b65 7973 da07 7375 6363 6573  del_keys..succes
-000007c0: 73da 0563 6f75 6e74 4e29 0872 0600 0000  s..countN).r....
-000007d0: 7207 0000 0072 0800 0000 721e 0000 0072  r....r....r....r
-000007e0: 1f00 0000 7209 0000 0072 0a00 0000 da03  ....r....r......
-000007f0: 696e 7472 0d00 0000 720d 0000 0072 0d00  intr....r....r..
-00000800: 0000 720e 0000 0072 2000 0000 2d00 0000  ..r....r ...-...
-00000810: 7306 0000 000a 0212 0108 0172 2000 0000  s..........r ...
-00000820: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000830: 0003 0000 0040 0000 0073 3800 0000 6500  .....@...s8...e.
-00000840: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000850: 6505 6a06 6402 6505 6a07 6602 1900 6504  e.j.d.e.j.f...e.
-00000860: 6403 3c00 6505 6a08 6509 1900 6504 6404  d.<.e.j.e...e.d.
-00000870: 3c00 6405 5300 2906 da0e 4261 7965 7372  <.d.S.)...Bayesr
-00000880: 756e 4f75 7470 7574 da08 6669 6c65 6e61  unOutput..filena
-00000890: 6d65 7209 0000 00da 0464 6174 61da 0772  mer......data..r
-000008a0: 6573 756c 7473 4e29 0a72 0600 0000 7207  esultsN).r....r.
-000008b0: 0000 0072 0800 0000 7202 0000 0072 0a00  ...r....r....r..
-000008c0: 0000 721e 0000 0072 1f00 0000 da03 416e  ..r....r......An
-000008d0: 79da 0853 6571 7565 6e63 6572 2000 0000  y..Sequencer ...
-000008e0: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-000008f0: 0e00 0000 7225 0000 0034 0000 0073 0600  ....r%...4...s..
-00000900: 0000 0a02 0801 1401 7225 0000 00e9 0100  ........r%......
-00000910: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00000920: 0000 0007 0000 0063 0000 0073 3600 0000  .......c...s6...
-00000930: 7400 6401 7401 7c00 8301 7c01 8303 4400  t.d.t.|...|...D.
-00000940: 5d20 7d02 7c00 7c02 7402 7c02 7c01 1700  ] }.|.|.t.|.|...
-00000950: 7401 7c00 8301 8302 8502 1900 5600 0100  t.|.........V...
-00000960: 7110 6402 5300 2903 7a46 0a09 7574 696c  q.d.S.).zF..util
-00000970: 6974 7920 666f 7220 6261 7463 6869 6e67  ity for batching
-00000980: 2062 6179 6573 7275 6e20 6669 6c65 7320   bayesrun files 
-00000990: 7768 6572 6520 636f 6c75 6d6e 7320 6170  where columns ap
-000009a0: 7065 6172 2069 6e20 7468 7265 6573 0a09  pear in threes..
-000009b0: 7201 0000 004e 2903 da05 7261 6e67 65da  r....N)...range.
-000009c0: 036c 656e da03 6d69 6e29 03da 0869 7465  .len..min)...ite
-000009d0: 7261 626c 65da 016e 5a03 6e64 7872 0d00  rable..nZ.ndxr..
-000009e0: 0000 720d 0000 0072 0e00 0000 da1b 5f62  ..r....r......_b
-000009f0: 6174 6368 5f69 7465 7261 626c 655f 696e  atch_iterable_in
-00000a00: 746f 5f63 6875 6e6b 733b 0000 0073 0400  to_chunks;...s..
-00000a10: 0000 0004 1401 7231 0000 0029 02da 0663  ......r1...)...c
-00000a20: 6f6c 756d 6eda 0672 6574 7572 6e63 0100  olumn..returnc..
-00000a30: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00000a40: 0000 4300 0000 732e 0000 0074 0044 005d  ..C...s....t.D.]
-00000a50: 247d 0174 01a0 027c 017c 00a1 027d 027c  $}.t...|.|...}.|
-00000a60: 0272 0474 037c 02a0 04a1 0083 0102 0001  .r.t.|..........
-00000a70: 0053 0071 0464 0153 0029 027a a30a 0954  .S.q.d.S.).z...T
-00000a80: 7269 6573 206f 6e65 2062 7920 6f6e 6520  ries one by one 
-00000a90: 616c 6c20 6f66 2061 2070 7265 6465 6669  all of a predefi
-00000aa0: 6e65 6420 6c69 7374 206f 6620 7265 6765  ned list of rege
-00000ab0: 7865 7320 7468 6174 2049 206d 6967 6874  xes that I might
-00000ac0: 2068 6176 6520 7573 6564 2069 6e20 7468   have used in th
-00000ad0: 6520 7061 7374 2e0a 0952 6574 7572 6e73  e past...Returns
-00000ae0: 2074 6865 2067 726f 7570 6469 6374 2066   the groupdict f
-00000af0: 6f72 2074 6865 2066 6972 7374 206d 6174  or the first mat
-00000b00: 6368 2c20 6f72 204e 6f6e 6520 6966 206e  ch, or None if n
-00000b10: 6f20 6d61 7463 6820 666f 756e 642e 0a09  o match found...
-00000b20: 4e29 05da 0d4d 4f44 454c 5f52 4547 4558  N)...MODEL_REGEX
-00000b30: 4553 da02 7265 da05 6d61 7463 6872 0f00  ES..re..matchr..
-00000b40: 0000 7210 0000 0029 0372 3200 0000 da07  ..r....).r2.....
-00000b50: 7061 7474 6572 6e72 3600 0000 720d 0000  patternr6...r...
-00000b60: 0072 0d00 0000 720e 0000 00da 165f 7061  .r....r......_pa
-00000b70: 7273 655f 6261 7965 7372 756e 5f63 6f6c  rse_bayesrun_col
-00000b80: 756d 6e43 0000 0073 0a00 0000 0007 0801  umnC...s........
-00000b90: 0c01 0401 1202 7238 0000 0029 02da 0372  ......r8...)...r
-00000ba0: 6f77 7233 0000 0063 0100 0000 0000 0000  owr3...c........
-00000bb0: 0000 0000 0900 0000 0800 0000 0300 0000  ................
-00000bc0: 73f2 0000 0067 007d 0174 0074 0188 00a0  s....g.}.t.t....
-00000bd0: 02a1 0083 0164 0183 027d 027c 0244 005d  .....d...}.|.D.]
-00000be0: d27d 0364 0264 0384 007c 0344 0083 017d  .}.d.d...|.D...}
-00000bf0: 0487 0066 0164 0464 0384 087c 0344 0083  ...f.d.d...|.D..
-00000c00: 017d 057c 0464 0519 0064 0075 0072 5874  .}.|.d...d.u.rXt
-00000c10: 0364 067c 039b 009d 0283 0182 017c 0464  .d.|.........|.d
-00000c20: 0719 0064 0075 0072 7274 0364 087c 039b  ...d.u.rrt.d.|..
-00000c30: 009d 0283 0182 017c 0464 0519 006a 0464  .......|.d...j.d
-00000c40: 096b 0372 9474 0364 0a7c 0364 0519 009b  .k.r.t.d.|.d....
-00000c50: 0064 0b9d 0383 0182 017c 0464 0719 006a  .d.......|.d...j
-00000c60: 0464 0c6b 0372 b674 0364 0a7c 0364 0719  .d.k.r.t.d.|.d..
-00000c70: 009b 0064 0d9d 0383 0182 017c 0464 0519  ...d.......|.d..
-00000c80: 006a 057d 0674 067c 0564 0519 0083 017d  .j.}.t.|.d.....}
-00000c90: 0774 067c 0564 0719 0083 017d 087c 01a0  .t.|.d.....}.|..
-00000ca0: 0774 087c 067c 077c 0864 0e8d 03a1 0101  .t.|.|.|.d......
-00000cb0: 0071 1a7c 0153 0029 0f4e e903 0000 0063  .q.|.S.).N.....c
-00000cc0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000cd0: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000ce0: 005d 0c7d 0174 007c 0183 0191 0271 0453  .].}.t.|.....q.S
-00000cf0: 0072 0d00 0000 2901 7238 0000 00a9 0272  .r....).r8.....r
-00000d00: 1200 0000 7232 0000 0072 0d00 0000 720d  ....r2...r....r.
-00000d10: 0000 0072 0e00 0000 da0a 3c6c 6973 7463  ...r......<listc
-00000d20: 6f6d 703e 5900 0000 f300 0000 007a 275f  omp>Y........z'_
-00000d30: 7061 7273 655f 6261 7965 7372 756e 5f72  parse_bayesrun_r
-00000d40: 6f77 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ow.<locals>.<lis
-00000d50: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
-00000d60: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00000d70: 1400 0000 6700 7c00 5d0c 7d01 8800 7c01  ....g.|.].}...|.
-00000d80: 1900 9102 7104 5300 720d 0000 0072 0d00  ....q.S.r....r..
-00000d90: 0000 723b 0000 00a9 0172 3900 0000 720d  ..r;.....r9...r.
-00000da0: 0000 0072 0e00 0000 723c 0000 005a 0000  ...r....r<...Z..
-00000db0: 0072 3d00 0000 7201 0000 007a 256e 6f20  .r=...r....z%no 
-00000dc0: 7669 6162 6c65 2073 7563 6365 7373 2072  viable success r
-00000dd0: 6f77 2066 6f75 6e64 2066 6f72 206b 6579  ow found for key
-00000de0: 7320 722b 0000 007a 236e 6f20 7669 6162  s r+...z#no viab
-00000df0: 6c65 2063 6f75 6e74 2072 6f77 2066 6f75  le count row fou
-00000e00: 6e64 2066 6f72 206b 6579 7320 7222 0000  nd for keys r"..
-00000e10: 007a 0b54 6865 2063 6f6c 756d 6e20 7a17  .z.The column z.
-00000e20: 2069 7320 6e6f 7420 6120 7375 6363 6573   is not a succes
-00000e30: 7320 6669 656c 6472 2300 0000 7a15 2069  s fieldr#...z. i
-00000e40: 7320 6e6f 7420 6120 636f 756e 7420 6669  s not a count fi
-00000e50: 656c 6429 0372 2100 0000 7222 0000 0072  eld).r!...r"...r
-00000e60: 2300 0000 2909 7231 0000 00da 046c 6973  #...).r1.....lis
-00000e70: 74da 046b 6579 73da 0a56 616c 7565 4572  t..keys..ValueEr
-00000e80: 726f 7272 1600 0000 7218 0000 0072 2400  rorr....r....r$.
-00000e90: 0000 da06 6170 7065 6e64 7220 0000 0029  ....appendr ...)
-00000ea0: 0972 3900 0000 7228 0000 005a 0c62 6174  .r9...r(...Z.bat
-00000eb0: 6368 6564 5f6b 6579 735a 0a6d 6f64 656c  ched_keysZ.model
-00000ec0: 5f6b 6579 73da 0670 6172 7365 64da 0676  _keys..parsed..v
-00000ed0: 616c 7565 735a 0b70 6172 7365 645f 6b65  aluesZ.parsed_ke
-00000ee0: 7973 7222 0000 0072 2300 0000 720d 0000  ysr"...r#...r...
-00000ef0: 0072 3e00 0000 720e 0000 00da 135f 7061  .r>...r......_pa
-00000f00: 7273 655f 6261 7965 7372 756e 5f72 6f77  rse_bayesrun_row
-00000f10: 5200 0000 7330 0000 0000 0404 0112 0108  R...s0..........
-00000f20: 010e 0112 010c 010e 010c 010e 010e 0114  ................
-00000f30: 010e 0114 010a 010c 010c 0104 0102 0102  ................
-00000f40: 0102 0102 fd04 ff06 0772 4500 0000 2902  .........rE...).
-00000f50: da04 6669 6c65 7233 0000 0063 0100 0000  ..filer3...c....
-00000f60: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00000f70: 4300 0000 7342 0000 007c 006a 007d 0174  C...sB...|.j.}.t
-00000f80: 01a0 0274 037c 01a1 027d 027c 0273 2474  ...t.|...}.|.s$t
-00000f90: 047c 019b 0064 019d 0283 0182 017c 02a0  .|...d.......|..
-00000fa0: 05a1 007d 0374 067c 0364 0219 007c 0364  ...}.t.|.d...|.d
-00000fb0: 0319 007c 0064 048d 0353 0029 054e 7a20  ...|.d...S.).Nz 
-00000fc0: 2077 6173 206e 6f74 2061 2076 616c 6964   was not a valid
-00000fd0: 2062 6179 6573 7275 6e20 6f75 7470 7574   bayesrun output
-00000fe0: 7203 0000 0072 0400 0000 2903 7203 0000  r....r....).r...
-00000ff0: 0072 0400 0000 7205 0000 0029 07da 046e  .r....r....)...n
-00001000: 616d 6572 3500 0000 7236 0000 00da 0e46  amer5...r6.....F
-00001010: 494c 454e 414d 455f 5245 4745 5872 4100  ILENAME_REGEXrA.
-00001020: 0000 7210 0000 0072 0200 0000 2904 7246  ..r....r....).rF
-00001030: 0000 0072 2600 0000 7236 0000 00da 0667  ...r&...r6.....g
-00001040: 726f 7570 7372 0d00 0000 720d 0000 0072  roupsr....r....r
-00001050: 0e00 0000 da16 5f70 6172 7365 5f6f 7574  ......_parse_out
-00001060: 7075 745f 6669 6c65 6e61 6d65 7000 0000  put_filenamep...
-00001070: 7310 0000 0000 0106 010c 0104 010e 0108  s...............
-00001080: 0102 010e ff72 4a00 0000 2902 da04 736c  .....rJ...)...sl
-00001090: 7567 7233 0000 0063 0100 0000 0000 0000  ugr3...c........
-000010a0: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-000010b0: 732a 0000 0074 0044 005d 207d 0174 01a0  s*...t.D.] }.t..
-000010c0: 027c 017c 00a1 027d 027c 0272 047c 02a0  .|.|...}.|.r.|..
-000010d0: 03a1 0002 0001 0053 0071 0464 0053 0029  .......S.q.d.S.)
-000010e0: 014e 2904 da11 4649 4c45 5f53 4c55 475f  .N)...FILE_SLUG_
-000010f0: 5245 4745 5845 5372 3500 0000 7236 0000  REGEXESr5...r6..
-00001100: 0072 1000 0000 2903 724b 0000 0072 3700  .r....).rK...r7.
-00001110: 0000 7236 0000 0072 0d00 0000 720d 0000  ..r6...r....r...
-00001120: 0072 0e00 0000 da10 5f70 6172 7365 5f66  .r......_parse_f
-00001130: 696c 655f 736c 7567 7b00 0000 730a 0000  ile_slug{...s...
-00001140: 0000 0108 010c 0104 010e 0272 4d00 0000  ...........rM...
-00001150: 2903 7246 0000 00da 0a69 6e64 6578 6966  ).rF.....indexif
-00001160: 6965 7272 3300 0000 6302 0000 0000 0000  ierr3...c.......
-00001170: 0000 0000 000d 0000 0008 0000 0043 0000  .............C..
-00001180: 0073 2c01 0000 7400 7c00 8301 0400 7d02  .s,...t.|.....}.
-00001190: 7d03 7401 7c02 6900 6700 6401 8d03 7d04  }.t.|.i.g.d...}.
-000011a0: 7c04 6a02 a003 7404 a005 7c03 a101 a101  |.j...t...|.....
-000011b0: 0100 7406 7c02 6a07 8301 7d05 7c05 6400  ..t.|.j...}.|.d.
-000011c0: 7500 7252 7408 a009 6402 7c03 9b00 6403  u.rRt...d.|...d.
-000011d0: 9d03 a101 0100 6e60 7c04 6a02 a003 7c05  ......n`|.j...|.
-000011e0: a101 0100 7c01 6400 7501 72b2 7a26 7c05  ....|.d.u.r.z&|.
-000011f0: 6404 1900 7d06 7c01 a00a 740b 7c06 8301  d...}.|...t.|...
-00001200: a101 7d07 7c04 6a02 a003 7c07 a101 0100  ..}.|.j...|.....
-00001210: 5700 6e24 0400 740c 79b0 0100 0100 0100  W.n$..t.y.......
-00001220: 7408 a009 6405 7c05 9b00 6406 9d03 a101  t...d.|...d.....
-00001230: 0100 5900 6e02 3000 7c00 a00d a100 8f4e  ..Y.n.0.|......N
-00001240: 7d08 740e a00f 7c08 a101 7d09 6407 6408  }.t...|...}.d.d.
-00001250: 8400 7c09 4400 8301 7d0a 7410 7c0a 8301  ..|.D...}.t.|...
-00001260: 6409 6b02 72ea 7c0a 640a 1900 7d0b 6e10  d.k.r.|.d...}.n.
-00001270: 7411 640b 7c00 6a12 9b00 9d02 8301 8201  t.d.|.j.........
-00001280: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
-00001290: 9001 7310 3000 0100 0100 0100 5900 0100  ..s.0.......Y...
-000012a0: 7413 7c0b 8301 7d0c 7c0c 7c04 5f14 7c04  t.|...}.|.|._.|.
-000012b0: 5300 290c 4e29 0372 2600 0000 7227 0000  S.).N).r&...r'..
-000012c0: 0072 2800 0000 7a10 436f 756c 6420 6e6f  .r(...z.Could no
-000012d0: 7420 7061 7273 6520 7a38 2061 6761 696e  t parse z8 again
-000012e0: 7374 2061 6e79 206d 6174 6368 696e 6720  st any matching 
-000012f0: 7265 6765 7865 732e 2047 6f69 6e67 2074  regexes. Going t
-00001300: 6f20 736b 6970 2074 6167 2070 6172 7369  o skip tag parsi
-00001310: 6e67 da09 6a6f 625f 696e 6465 787a 0e50  ng..job_indexz.P
-00001320: 6172 7365 6420 7461 6720 746f 207a 522c  arsed tag to zR,
-00001330: 2061 6e64 2061 7474 656d 7074 6564 2074   and attempted t
-00001340: 6f20 696e 6465 7869 6679 2062 7574 206e  o indexify but n
-00001350: 6f20 6a6f 625f 696e 6465 7820 6b65 7920  o job_index key 
-00001360: 7761 7320 666f 756e 642e 2073 6b69 7070  was found. skipp
-00001370: 696e 6720 616e 6420 6d6f 7669 6e67 206f  ing and moving o
-00001380: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
-00001390: 0000 0300 0000 5300 0000 7310 0000 0067  ......S...s....g
-000013a0: 007c 005d 087d 017c 0191 0271 0453 0072  .|.].}.|...q.S.r
-000013b0: 0d00 0000 720d 0000 0029 0272 1200 0000  ....r....).r....
-000013c0: da01 7272 0d00 0000 720d 0000 0072 0e00  ..rr....r....r..
-000013d0: 0000 723c 0000 00a0 0000 0072 3d00 0000  ..r<.......r=...
-000013e0: 7a24 7265 6164 5f6f 7574 7075 745f 6669  z$read_output_fi
-000013f0: 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  le.<locals>.<lis
-00001400: 7463 6f6d 703e 722b 0000 0072 0100 0000  tcomp>r+...r....
-00001410: 7a27 436f 6e66 7573 6564 2061 626f 7574  z'Confused about
-00001420: 2068 6176 696e 6720 6d75 6c74 6970 6c65   having multiple
-00001430: 2072 6f77 7320 696e 2029 1572 4a00 0000   rows in ).rJ...
-00001440: 7225 0000 0072 2700 0000 da06 7570 6461  r%...r'.....upda
-00001450: 7465 da0b 6461 7461 636c 6173 7365 73da  te..dataclasses.
-00001460: 0661 7364 6963 7472 4d00 0000 7204 0000  .asdictrM...r...
-00001470: 00da 075f 6c6f 6767 6572 da07 7761 726e  ..._logger..warn
-00001480: 696e 67da 0869 6e64 6578 6966 7972 2400  ing..indexifyr$.
-00001490: 0000 da08 4b65 7945 7272 6f72 da04 6f70  ....KeyError..op
-000014a0: 656e da03 6373 76da 0a44 6963 7452 6561  en..csv..DictRea
-000014b0: 6465 7272 2d00 0000 7241 0000 0072 4700  derr-...rA...rG.
-000014c0: 0000 7245 0000 0072 2800 0000 290d 7246  ..rE...r(...).rF
-000014d0: 0000 0072 4e00 0000 5a0f 7061 7273 6564  ...rN...Z.parsed
-000014e0: 5f66 696c 656e 616d 65da 0374 6167 da03  _filename..tag..
-000014f0: 6f75 745a 0a70 6172 7365 645f 7461 6772  outZ.parsed_tagr
-00001500: 4f00 0000 5a0a 696e 6465 7869 6669 6564  O...Z.indexified
-00001510: 5a0a 696e 7075 745f 6669 6c65 da06 7265  Z.input_file..re
-00001520: 6164 6572 da04 726f 7773 7239 0000 0072  ader..rowsr9...r
-00001530: 2800 0000 720d 0000 0072 0d00 0000 720e  (...r....r....r.
-00001540: 0000 00da 1072 6561 645f 6f75 7470 7574  .....read_output
-00001550: 5f66 696c 6584 0000 0073 3600 0000 0004  _file....s6.....
-00001560: 0c01 0e02 1201 0a01 0801 0401 0aff 0604  ................
-00001570: 0c01 0801 0201 0801 0e01 1001 0c02 0401  ................
-00001580: 0aff 0a04 0a01 0a01 0e01 0c01 0a02 3001  ..............0.
-00001590: 0802 0602 725f 0000 0029 0172 2b00 0000  ....r_...).r+...
-000015a0: 2920 7252 0000 0072 3500 0000 721e 0000  ) rR...r5...r...
-000015b0: 00da 076c 6f67 6769 6e67 da10 6465 6570  ...logging..deep
-000015c0: 646f 672e 696e 6465 7869 6679 da07 6465  dog.indexify..de
-000015d0: 6570 646f 6772 0b00 0000 7259 0000 00da  epdogr....rY....
-000015e0: 0967 6574 4c6f 6767 6572 7206 0000 0072  .getLoggerr....r
-000015f0: 5400 0000 7248 0000 0072 3400 0000 724c  T...rH...r4...rL
-00001600: 0000 00da 0964 6174 6163 6c61 7373 7202  .....dataclassr.
-00001610: 0000 0072 0f00 0000 7220 0000 0072 2500  ...r....r ...r%.
-00001620: 0000 7231 0000 0072 0900 0000 da08 4f70  ..r1...r......Op
-00001630: 7469 6f6e 616c 7238 0000 0072 1f00 0000  tionalr8...r....
-00001640: 722a 0000 0072 4500 0000 720c 0000 0072  r*...rE...r....r
-00001650: 4a00 0000 724d 0000 0072 5600 0000 da0a  J...rM...rV.....
-00001660: 496e 6465 7869 6669 6572 725f 0000 0072  Indexifierr_...r
-00001670: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00001680: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001690: 0073 4000 0000 0801 0801 0801 0801 0801  .s@.............
-000016a0: 0801 0802 0a02 0403 02ff 0405 02ff 0405  ................
-000016b0: 0401 1006 0401 100f 0401 1006 0401 1006  ................
-000016c0: 0a09 0201 08fe 0c10 0c01 08fe 0c1e 120b  ................
-000016d0: 200a 1001 02fe                            .....
+00000070: 6402 5a0b 6403 6701 5a0c 6404 6405 6702  d.Z.d.g.Z.d.d.g.
+00000080: 5a0d 6500 6a0e 4700 6406 6407 8400 6407  Z.e.j.G.d.d...d.
+00000090: 8302 8301 5a0f 6500 6a0e 4700 6408 6409  ....Z.e.j.G.d.d.
+000000a0: 8400 6409 8302 8301 5a10 6500 6a0e 4700  ..d.....Z.e.j.G.
+000000b0: 640a 640b 8400 640b 8302 8301 5a11 6500  d.d...d.....Z.e.
+000000c0: 6a0e 4700 640c 640d 8400 640d 8302 8301  j.G.d.d...d.....
+000000d0: 5a12 6420 640f 6410 8401 5a13 6514 6502  Z.d d.d...Z.e.e.
+000000e0: 6a15 6510 1900 6411 9c02 6412 6413 8404  j.e...d...d.d...
+000000f0: 5a16 6502 6a17 6514 6514 6602 1900 6502  Z.e.j.e.e.f...e.
+00000100: 6a18 6511 1900 6414 9c02 6415 6416 8404  j.e...d...d.d...
+00000110: 5a19 6506 6a1a 650f 6417 9c02 6418 6419  Z.e.j.e.d...d.d.
+00000120: 8404 5a1b 6514 6502 6a15 6502 6a17 6514  ..Z.e.e.j.e.j.e.
+00000130: 6514 6602 1900 1900 641a 9c02 641b 641c  e.f.....d...d.d.
+00000140: 8404 5a1c 6506 6a1a 6502 6a15 6505 6a1d  ..Z.e.j.e.j.e.j.
+00000150: 6a1e 1900 6512 641d 9c03 641e 641f 8404  j...e.d...d.d...
+00000160: 5a1f 6401 5300 2921 e900 0000 004e 7a56  Z.d.S.)!.....NzV
+00000170: 283f 503c 7469 6d65 7374 616d 703e 5c64  (?P<timestamp>\d
+00000180: 7b38 7d2d 5c64 7b36 7d29 2d28 3f50 3c66  {8}-\d{6})-(?P<f
+00000190: 696c 656e 616d 655f 736c 7567 3e2e 2a29  ilename_slug>.*)
+000001a0: 5c2e 7265 616c 6461 7461 5c2e 6661 7374  \.realdata\.fast
+000001b0: 5f66 696c 7465 725c 2e62 6179 6573 7275  _filter\.bayesru
+000001c0: 6e5c 2e63 7376 7aca 6765 6f6d 5f28 3f50  n\.csvz.geom_(?P
+000001d0: 3c78 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50  <xmin>-?\d+)_(?P
+000001e0: 3c78 6d61 783e 2d3f 5c64 2b29 5f28 3f50  <xmax>-?\d+)_(?P
+000001f0: 3c79 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50  <ymin>-?\d+)_(?P
+00000200: 3c79 6d61 783e 2d3f 5c64 2b29 5f28 3f50  <ymax>-?\d+)_(?P
+00000210: 3c7a 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50  <zmin>-?\d+)_(?P
+00000220: 3c7a 6d61 783e 2d3f 5c64 2b29 2d6f 7269  <zmax>-?\d+)-ori
+00000230: 656e 7461 7469 6f6e 5f28 3f50 3c6f 7269  entation_(?P<ori
+00000240: 656e 7461 7469 6f6e 3e66 7265 657c 6669  entation>free|fi
+00000250: 7865 6478 797c 6669 7865 647a 292d 6469  xedxy|fixedz)-di
+00000260: 706f 6c65 5f63 6f75 6e74 5f28 3f50 3c61  pole_count_(?P<a
+00000270: 7667 5f66 696c 6c65 643e 5c64 2b29 5f28  vg_filled>\d+)_(
+00000280: 3f50 3c66 6965 6c64 5f6e 616d 653e 5c77  ?P<field_name>\w
+00000290: 2a29 7a1f 6d6f 636b 5f74 6172 7563 6861  *)z.mock_tarucha
+000002a0: 2d28 3f50 3c6a 6f62 5f69 6e64 6578 3e5c  -(?P<job_index>\
+000002b0: 642b 297a 4b28 3f3a 283f 503c 6d6f 636b  d+)zK(?:(?P<mock
+000002c0: 3e6d 6f63 6b29 5f29 3f74 6172 7563 6861  >mock)_)?tarucha
+000002d0: 283f 3a5f 283f 503c 7461 7275 6368 615f  (?:_(?P<tarucha_
+000002e0: 7275 6e5f 6964 3e5c 642b 2929 3f2d 283f  run_id>\d+))?-(?
+000002f0: 503c 6a6f 625f 696e 6465 783e 5c64 2b29  P<job_index>\d+)
+00000300: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000310: 0003 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
+00000320: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000330: 6503 6504 6402 3c00 6505 6a06 6504 6403  e.e.d.<.e.j.e.d.
+00000340: 3c00 6404 5300 2905 da16 4261 7965 7372  <.d.S.)...Bayesr
+00000350: 756e 4f75 7470 7574 4669 6c65 6e61 6d65  unOutputFilename
+00000360: da09 7469 6d65 7374 616d 70da 0d66 696c  ..timestamp..fil
+00000370: 656e 616d 655f 736c 7567 da04 7061 7468  ename_slug..path
+00000380: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000390: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000003a0: 6c6e 616d 655f 5fda 0373 7472 da0f 5f5f  lname__..str..__
+000003b0: 616e 6e6f 7461 7469 6f6e 735f 5fda 0770  annotations__..p
+000003c0: 6174 686c 6962 da04 5061 7468 a900 720d  athlib..Path..r.
+000003d0: 0000 0072 0d00 0000 fa55 2f68 6f6d 652f  ...r.....U/home/
+000003e0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
+000003f0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
+00000400: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
+00000410: 302e 302f 6465 6570 646f 672f 7265 7375  0.0/deepdog/resu
+00000420: 6c74 732f 5f5f 696e 6974 5f5f 2e70 7972  lts/__init__.pyr
+00000430: 0200 0000 1700 0000 7306 0000 000a 0208  ........s.......
+00000440: 0108 0172 0200 0000 6300 0000 0000 0000  ...r....c.......
+00000450: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000460: 0073 3000 0000 6500 5a01 6400 5a02 6401  .s0...e.Z.d.Z.d.
+00000470: 5a03 6504 6a05 6506 6506 6602 1900 6402  Z.e.j.e.e.f...d.
+00000480: 9c01 6403 6404 8404 5a07 6405 6406 8400  ..d.d...Z.d.d...
+00000490: 5a08 6407 5300 2908 da14 4261 7965 7372  Z.d.S.)...Bayesr
+000004a0: 756e 436f 6c75 6d6e 5061 7273 6564 7a49  unColumnParsedzI
+000004b0: 0a09 636c 6173 7320 666f 7220 7061 7273  ..class for pars
+000004c0: 696e 6720 6120 6261 7965 7372 756e 2077  ing a bayesrun w
+000004d0: 6869 6c65 2070 756c 6c69 6e67 2063 6572  hile pulling cer
+000004e0: 7461 696e 2073 7065 6369 616c 2066 6965  tain special fie
+000004f0: 6c64 7320 6f75 740a 0929 01da 0967 726f  lds out..)...gro
+00000500: 7570 6469 6374 6302 0000 0000 0000 0000  updictc.........
+00000510: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00000520: 2200 0000 7c01 6401 1900 7c00 5f00 6402  "...|.d...|._.d.
+00000530: 6403 8400 7c01 a001 a100 4400 8301 7c00  d...|.....D...|.
+00000540: 5f02 6400 5300 2904 4eda 0a66 6965 6c64  _.d.S.).N..field
+00000550: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
+00000560: 0000 0300 0000 0400 0000 5300 0000 731e  ..........S...s.
+00000570: 0000 0069 007c 005d 165c 027d 017d 027c  ...i.|.].\.}.}.|
+00000580: 0164 006b 0372 047c 017c 0293 0271 0453  .d.k.r.|.|...q.S
+00000590: 0029 0172 1100 0000 720d 0000 0029 03da  .).r....r....)..
+000005a0: 022e 30da 016b da01 7672 0d00 0000 720d  ..0..k..vr....r.
+000005b0: 0000 0072 0e00 0000 da0a 3c64 6963 7463  ...r......<dictc
+000005c0: 6f6d 703e 2600 0000 7302 0000 0006 017a  omp>&...s......z
+000005d0: 3142 6179 6573 7275 6e43 6f6c 756d 6e50  1BayesrunColumnP
+000005e0: 6172 7365 642e 5f5f 696e 6974 5f5f 2e3c  arsed.__init__.<
+000005f0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+00000600: 703e 2903 da0c 636f 6c75 6d6e 5f66 6965  p>)...column_fie
+00000610: 6c64 da05 6974 656d 73da 106d 6f64 656c  ld..items..model
+00000620: 5f66 6965 6c64 5f64 6963 7429 02da 0473  _field_dict)...s
+00000630: 656c 6672 1000 0000 720d 0000 0072 0d00  elfr....r....r..
+00000640: 0000 720e 0000 00da 085f 5f69 6e69 745f  ..r......__init_
+00000650: 5f24 0000 0073 0800 0000 0001 0a01 0601  _$...s..........
+00000660: 06ff 7a1d 4261 7965 7372 756e 436f 6c75  ..z.BayesrunColu
+00000670: 6d6e 5061 7273 6564 2e5f 5f69 6e69 745f  mnParsed.__init_
+00000680: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000690: 0000 0500 0000 4300 0000 7316 0000 0064  ......C...s....d
+000006a0: 017c 006a 009b 0064 027c 006a 019b 0064  .|.j...d.|.j...d
+000006b0: 039d 0553 0029 044e 7a15 4261 7965 7372  ...S.).Nz.Bayesr
+000006c0: 756e 436f 6c75 6d6e 5061 7273 6564 5b7a  unColumnParsed[z
+000006d0: 023a 20da 015d 2902 7216 0000 0072 1800  .: ..]).r....r..
+000006e0: 0000 2901 7219 0000 0072 0d00 0000 720d  ..).r....r....r.
+000006f0: 0000 0072 0e00 0000 da07 5f5f 7374 725f  ...r......__str_
+00000700: 5f2a 0000 0073 0200 0000 0001 7a1c 4261  _*...s......z.Ba
+00000710: 7965 7372 756e 436f 6c75 6d6e 5061 7273  yesrunColumnPars
+00000720: 6564 2e5f 5f73 7472 5f5f 4e29 0972 0600  ed.__str__N).r..
+00000730: 0000 7207 0000 0072 0800 0000 da07 5f5f  ..r....r......__
+00000740: 646f 635f 5fda 0674 7970 696e 67da 0444  doc__..typing..D
+00000750: 6963 7472 0900 0000 721a 0000 0072 1c00  ictr....r....r..
+00000760: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000770: 0072 0e00 0000 720f 0000 001e 0000 0073  .r....r........s
+00000780: 0600 0000 0802 0404 1806 720f 0000 0063  ..........r....c
+00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007a0: 0300 0000 4000 0000 7330 0000 0065 005a  ....@...s0...e.Z
+000007b0: 0164 005a 0255 0065 036a 0465 0565 0566  .d.Z.U.e.j.e.e.f
+000007c0: 0219 0065 0664 013c 0065 0765 0664 023c  ...e.d.<.e.e.d.<
+000007d0: 0065 0765 0664 033c 0064 0453 0029 05da  .e.e.d.<.d.S.)..
+000007e0: 1342 6179 6573 7275 6e4d 6f64 656c 5265  .BayesrunModelRe
+000007f0: 7375 6c74 da11 7061 7273 6564 5f6d 6f64  sult..parsed_mod
+00000800: 656c 5f6b 6579 73da 0773 7563 6365 7373  el_keys..success
+00000810: da05 636f 756e 744e 2908 7206 0000 0072  ..countN).r....r
+00000820: 0700 0000 7208 0000 0072 1e00 0000 721f  ....r....r....r.
+00000830: 0000 0072 0900 0000 720a 0000 00da 0369  ...r....r......i
+00000840: 6e74 720d 0000 0072 0d00 0000 720d 0000  ntr....r....r...
+00000850: 0072 0e00 0000 7220 0000 002e 0000 0073  .r....r .......s
+00000860: 0600 0000 0a02 1201 0801 7220 0000 0063  ..........r ...c
+00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000880: 0300 0000 4000 0000 7338 0000 0065 005a  ....@...s8...e.Z
+00000890: 0164 005a 0255 0065 0365 0464 013c 0065  .d.Z.U.e.e.d.<.e
+000008a0: 056a 0664 0265 056a 0766 0219 0065 0464  .j.d.e.j.f...e.d
+000008b0: 033c 0065 056a 0865 0919 0065 0464 043c  .<.e.j.e...e.d.<
+000008c0: 0064 0553 0029 06da 0e42 6179 6573 7275  .d.S.)...Bayesru
+000008d0: 6e4f 7574 7075 74da 0866 696c 656e 616d  nOutput..filenam
+000008e0: 6572 0900 0000 da04 6461 7461 da07 7265  er......data..re
+000008f0: 7375 6c74 734e 290a 7206 0000 0072 0700  sultsN).r....r..
+00000900: 0000 7208 0000 0072 0200 0000 720a 0000  ..r....r....r...
+00000910: 0072 1e00 0000 721f 0000 00da 0341 6e79  .r....r......Any
+00000920: da08 5365 7175 656e 6365 7220 0000 0072  ..Sequencer ...r
+00000930: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00000940: 0000 0072 2500 0000 3500 0000 7306 0000  ...r%...5...s...
+00000950: 000a 0208 0114 0172 2500 0000 e901 0000  .......r%.......
+00000960: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+00000970: 0000 0700 0000 6300 0000 7336 0000 0074  ......c...s6...t
+00000980: 0064 0174 017c 0083 017c 0183 0344 005d  .d.t.|...|...D.]
+00000990: 207d 027c 007c 0274 027c 027c 0117 0074   }.|.|.t.|.|...t
+000009a0: 017c 0083 0183 0285 0219 0056 0001 0071  .|.........V...q
+000009b0: 1064 0253 0029 037a 460a 0975 7469 6c69  .d.S.).zF..utili
+000009c0: 7479 2066 6f72 2062 6174 6368 696e 6720  ty for batching 
+000009d0: 6261 7965 7372 756e 2066 696c 6573 2077  bayesrun files w
+000009e0: 6865 7265 2063 6f6c 756d 6e73 2061 7070  here columns app
+000009f0: 6561 7220 696e 2074 6872 6565 730a 0972  ear in threes..r
+00000a00: 0100 0000 4e29 03da 0572 616e 6765 da03  ....N)...range..
+00000a10: 6c65 6eda 036d 696e 2903 da08 6974 6572  len..min)...iter
+00000a20: 6162 6c65 da01 6e5a 036e 6478 720d 0000  able..nZ.ndxr...
+00000a30: 0072 0d00 0000 720e 0000 00da 1b5f 6261  .r....r......_ba
+00000a40: 7463 685f 6974 6572 6162 6c65 5f69 6e74  tch_iterable_int
+00000a50: 6f5f 6368 756e 6b73 3c00 0000 7304 0000  o_chunks<...s...
+00000a60: 0000 0414 0172 3100 0000 2902 da06 636f  .....r1...)...co
+00000a70: 6c75 6d6e da06 7265 7475 726e 6301 0000  lumn..returnc...
+00000a80: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000a90: 0043 0000 0073 2e00 0000 7400 4400 5d24  .C...s....t.D.]$
+00000aa0: 7d01 7401 a002 7c01 7c00 a102 7d02 7c02  }.t...|.|...}.|.
+00000ab0: 7204 7403 7c02 a004 a100 8301 0200 0100  r.t.|...........
+00000ac0: 5300 7104 6401 5300 2902 7aa3 0a09 5472  S.q.d.S.).z...Tr
+00000ad0: 6965 7320 6f6e 6520 6279 206f 6e65 2061  ies one by one a
+00000ae0: 6c6c 206f 6620 6120 7072 6564 6566 696e  ll of a predefin
+00000af0: 6564 206c 6973 7420 6f66 2072 6567 6578  ed list of regex
+00000b00: 6573 2074 6861 7420 4920 6d69 6768 7420  es that I might 
+00000b10: 6861 7665 2075 7365 6420 696e 2074 6865  have used in the
+00000b20: 2070 6173 742e 0a09 5265 7475 726e 7320   past...Returns 
+00000b30: 7468 6520 6772 6f75 7064 6963 7420 666f  the groupdict fo
+00000b40: 7220 7468 6520 6669 7273 7420 6d61 7463  r the first matc
+00000b50: 682c 206f 7220 4e6f 6e65 2069 6620 6e6f  h, or None if no
+00000b60: 206d 6174 6368 2066 6f75 6e64 2e0a 094e   match found...N
+00000b70: 2905 da0d 4d4f 4445 4c5f 5245 4745 5845  )...MODEL_REGEXE
+00000b80: 53da 0272 65da 056d 6174 6368 720f 0000  S..re..matchr...
+00000b90: 0072 1000 0000 2903 7232 0000 00da 0770  .r....).r2.....p
+00000ba0: 6174 7465 726e 7236 0000 0072 0d00 0000  atternr6...r....
+00000bb0: 720d 0000 0072 0e00 0000 da16 5f70 6172  r....r......_par
+00000bc0: 7365 5f62 6179 6573 7275 6e5f 636f 6c75  se_bayesrun_colu
+00000bd0: 6d6e 4400 0000 730a 0000 0000 0708 010c  mnD...s.........
+00000be0: 0104 0112 0272 3800 0000 2902 da03 726f  .....r8...)...ro
+00000bf0: 7772 3300 0000 6301 0000 0000 0000 0000  wr3...c.........
+00000c00: 0000 0009 0000 0008 0000 0003 0000 0073  ...............s
+00000c10: f200 0000 6700 7d01 7400 7401 8800 a002  ....g.}.t.t.....
+00000c20: a100 8301 6401 8302 7d02 7c02 4400 5dd2  ....d...}.|.D.].
+00000c30: 7d03 6402 6403 8400 7c03 4400 8301 7d04  }.d.d...|.D...}.
+00000c40: 8700 6601 6404 6403 8408 7c03 4400 8301  ..f.d.d...|.D...
+00000c50: 7d05 7c04 6405 1900 6400 7500 7258 7403  }.|.d...d.u.rXt.
+00000c60: 6406 7c03 9b00 9d02 8301 8201 7c04 6407  d.|.........|.d.
+00000c70: 1900 6400 7500 7272 7403 6408 7c03 9b00  ..d.u.rrt.d.|...
+00000c80: 9d02 8301 8201 7c04 6405 1900 6a04 6409  ......|.d...j.d.
+00000c90: 6b03 7294 7403 640a 7c03 6405 1900 9b00  k.r.t.d.|.d.....
+00000ca0: 640b 9d03 8301 8201 7c04 6407 1900 6a04  d.......|.d...j.
+00000cb0: 640c 6b03 72b6 7403 640a 7c03 6407 1900  d.k.r.t.d.|.d...
+00000cc0: 9b00 640d 9d03 8301 8201 7c04 6405 1900  ..d.......|.d...
+00000cd0: 6a05 7d06 7406 7c05 6405 1900 8301 7d07  j.}.t.|.d.....}.
+00000ce0: 7406 7c05 6407 1900 8301 7d08 7c01 a007  t.|.d.....}.|...
+00000cf0: 7408 7c06 7c07 7c08 640e 8d03 a101 0100  t.|.|.|.d.......
+00000d00: 711a 7c01 5300 290f 4ee9 0300 0000 6301  q.|.S.).N.....c.
+00000d10: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000d20: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00000d30: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
+00000d40: 720d 0000 0029 0172 3800 0000 a902 7212  r....).r8.....r.
+00000d50: 0000 0072 3200 0000 720d 0000 0072 0d00  ...r2...r....r..
+00000d60: 0000 720e 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00000d70: 6d70 3e5a 0000 00f3 0000 0000 7a27 5f70  mp>Z........z'_p
+00000d80: 6172 7365 5f62 6179 6573 7275 6e5f 726f  arse_bayesrun_ro
+00000d90: 772e 3c6c 6f63 616c 733e 2e3c 6c69 7374  w.<locals>.<list
+00000da0: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
+00000db0: 0000 0200 0000 0400 0000 1300 0000 7314  ..............s.
+00000dc0: 0000 0067 007c 005d 0c7d 0188 007c 0119  ...g.|.].}...|..
+00000dd0: 0091 0271 0453 0072 0d00 0000 720d 0000  ...q.S.r....r...
+00000de0: 0072 3b00 0000 a901 7239 0000 0072 0d00  .r;.....r9...r..
+00000df0: 0000 720e 0000 0072 3c00 0000 5b00 0000  ..r....r<...[...
+00000e00: 723d 0000 0072 0100 0000 7a25 6e6f 2076  r=...r....z%no v
+00000e10: 6961 626c 6520 7375 6363 6573 7320 726f  iable success ro
+00000e20: 7720 666f 756e 6420 666f 7220 6b65 7973  w found for keys
+00000e30: 2072 2b00 0000 7a23 6e6f 2076 6961 626c   r+...z#no viabl
+00000e40: 6520 636f 756e 7420 726f 7720 666f 756e  e count row foun
+00000e50: 6420 666f 7220 6b65 7973 2072 2200 0000  d for keys r"...
+00000e60: 7a0b 5468 6520 636f 6c75 6d6e 207a 1720  z.The column z. 
+00000e70: 6973 206e 6f74 2061 2073 7563 6365 7373  is not a success
+00000e80: 2066 6965 6c64 7223 0000 007a 1520 6973   fieldr#...z. is
+00000e90: 206e 6f74 2061 2063 6f75 6e74 2066 6965   not a count fie
+00000ea0: 6c64 2903 7221 0000 0072 2200 0000 7223  ld).r!...r"...r#
+00000eb0: 0000 0029 0972 3100 0000 da04 6c69 7374  ...).r1.....list
+00000ec0: da04 6b65 7973 da0a 5661 6c75 6545 7272  ..keys..ValueErr
+00000ed0: 6f72 7216 0000 0072 1800 0000 7224 0000  orr....r....r$..
+00000ee0: 00da 0661 7070 656e 6472 2000 0000 2909  ...appendr ...).
+00000ef0: 7239 0000 0072 2800 0000 5a0c 6261 7463  r9...r(...Z.batc
+00000f00: 6865 645f 6b65 7973 5a0a 6d6f 6465 6c5f  hed_keysZ.model_
+00000f10: 6b65 7973 da06 7061 7273 6564 da06 7661  keys..parsed..va
+00000f20: 6c75 6573 5a0b 7061 7273 6564 5f6b 6579  luesZ.parsed_key
+00000f30: 7372 2200 0000 7223 0000 0072 0d00 0000  sr"...r#...r....
+00000f40: 723e 0000 0072 0e00 0000 da13 5f70 6172  r>...r......_par
+00000f50: 7365 5f62 6179 6573 7275 6e5f 726f 7753  se_bayesrun_rowS
+00000f60: 0000 0073 3000 0000 0004 0401 1201 0801  ...s0...........
+00000f70: 0e01 1201 0c01 0e01 0c01 0e01 0e01 1401  ................
+00000f80: 0e01 1401 0a01 0c01 0c01 0401 0201 0201  ................
+00000f90: 0201 02fd 04ff 0607 7245 0000 0029 02da  ........rE...)..
+00000fa0: 0466 696c 6572 3300 0000 6301 0000 0000  .filer3...c.....
+00000fb0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+00000fc0: 0000 0073 4200 0000 7c00 6a00 7d01 7401  ...sB...|.j.}.t.
+00000fd0: a002 7403 7c01 a102 7d02 7c02 7324 7404  ..t.|...}.|.s$t.
+00000fe0: 7c01 9b00 6401 9d02 8301 8201 7c02 a005  |...d.......|...
+00000ff0: a100 7d03 7406 7c03 6402 1900 7c03 6403  ..}.t.|.d...|.d.
+00001000: 1900 7c00 6404 8d03 5300 2905 4e7a 2020  ..|.d...S.).Nz  
+00001010: 7761 7320 6e6f 7420 6120 7661 6c69 6420  was not a valid 
+00001020: 6261 7965 7372 756e 206f 7574 7075 7472  bayesrun outputr
+00001030: 0300 0000 7204 0000 0029 0372 0300 0000  ....r....).r....
+00001040: 7204 0000 0072 0500 0000 2907 da04 6e61  r....r....)...na
+00001050: 6d65 7235 0000 0072 3600 0000 da0e 4649  mer5...r6.....FI
+00001060: 4c45 4e41 4d45 5f52 4547 4558 7241 0000  LENAME_REGEXrA..
+00001070: 0072 1000 0000 7202 0000 0029 0472 4600  .r....r....).rF.
+00001080: 0000 7226 0000 0072 3600 0000 da06 6772  ..r&...r6.....gr
+00001090: 6f75 7073 720d 0000 0072 0d00 0000 720e  oupsr....r....r.
+000010a0: 0000 00da 165f 7061 7273 655f 6f75 7470  ....._parse_outp
+000010b0: 7574 5f66 696c 656e 616d 6571 0000 0073  ut_filenameq...s
+000010c0: 1000 0000 0001 0601 0c01 0401 0e01 0801  ................
+000010d0: 0201 0eff 724a 0000 0029 02da 0473 6c75  ....rJ...)...slu
+000010e0: 6772 3300 0000 6301 0000 0000 0000 0000  gr3...c.........
+000010f0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+00001100: 2a00 0000 7400 4400 5d20 7d01 7401 a002  *...t.D.] }.t...
+00001110: 7c01 7c00 a102 7d02 7c02 7204 7c02 a003  |.|...}.|.r.|...
+00001120: a100 0200 0100 5300 7104 6400 5300 2901  ......S.q.d.S.).
+00001130: 4e29 04da 1146 494c 455f 534c 5547 5f52  N)...FILE_SLUG_R
+00001140: 4547 4558 4553 7235 0000 0072 3600 0000  EGEXESr5...r6...
+00001150: 7210 0000 0029 0372 4b00 0000 7237 0000  r....).rK...r7..
+00001160: 0072 3600 0000 720d 0000 0072 0d00 0000  .r6...r....r....
+00001170: 720e 0000 00da 105f 7061 7273 655f 6669  r......_parse_fi
+00001180: 6c65 5f73 6c75 677c 0000 0073 0a00 0000  le_slug|...s....
+00001190: 0001 0801 0c01 0401 0e02 724d 0000 0029  ..........rM...)
+000011a0: 0372 4600 0000 da0a 696e 6465 7869 6669  .rF.....indexifi
+000011b0: 6572 7233 0000 0063 0200 0000 0000 0000  err3...c........
+000011c0: 0000 0000 0d00 0000 0800 0000 4300 0000  ............C...
+000011d0: 732c 0100 0074 007c 0083 0104 007d 027d  s,...t.|.....}.}
+000011e0: 0374 017c 0269 0067 0064 018d 037d 047c  .t.|.i.g.d...}.|
+000011f0: 046a 02a0 0374 04a0 057c 03a1 01a1 0101  .j...t...|......
+00001200: 0074 067c 026a 0783 017d 057c 0564 0075  .t.|.j...}.|.d.u
+00001210: 0072 5274 08a0 0964 027c 039b 0064 039d  .rRt...d.|...d..
+00001220: 03a1 0101 006e 607c 046a 02a0 037c 05a1  .....n`|.j...|..
+00001230: 0101 007c 0164 0075 0172 b27a 267c 0564  ...|.d.u.r.z&|.d
+00001240: 0419 007d 067c 01a0 0a74 0b7c 0683 01a1  ...}.|...t.|....
+00001250: 017d 077c 046a 02a0 037c 07a1 0101 0057  .}.|.j...|.....W
+00001260: 006e 2404 0074 0c79 b001 0001 0001 0074  .n$..t.y.......t
+00001270: 08a0 0964 057c 059b 0064 069d 03a1 0101  ...d.|...d......
+00001280: 0059 006e 0230 007c 00a0 0da1 008f 4e7d  .Y.n.0.|......N}
+00001290: 0874 0ea0 0f7c 08a1 017d 0964 0764 0884  .t...|...}.d.d..
+000012a0: 007c 0944 0083 017d 0a74 107c 0a83 0164  .|.D...}.t.|...d
+000012b0: 096b 0272 ea7c 0a64 0a19 007d 0b6e 1074  .k.r.|.d...}.n.t
+000012c0: 1164 0b7c 006a 129b 009d 0283 0182 0157  .d.|.j.........W
+000012d0: 0064 0004 0004 0083 0301 006e 1231 0090  .d.........n.1..
+000012e0: 0173 1030 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
+000012f0: 137c 0b83 017d 0c7c 0c7c 045f 147c 0453  .|...}.|.|._.|.S
+00001300: 0029 0c4e 2903 7226 0000 0072 2700 0000  .).N).r&...r'...
+00001310: 7228 0000 007a 1043 6f75 6c64 206e 6f74  r(...z.Could not
+00001320: 2070 6172 7365 207a 3820 6167 6169 6e73   parse z8 agains
+00001330: 7420 616e 7920 6d61 7463 6869 6e67 2072  t any matching r
+00001340: 6567 6578 6573 2e20 476f 696e 6720 746f  egexes. Going to
+00001350: 2073 6b69 7020 7461 6720 7061 7273 696e   skip tag parsin
+00001360: 67da 096a 6f62 5f69 6e64 6578 7a0e 5061  g..job_indexz.Pa
+00001370: 7273 6564 2074 6167 2074 6f20 7a52 2c20  rsed tag to zR, 
+00001380: 616e 6420 6174 7465 6d70 7465 6420 746f  and attempted to
+00001390: 2069 6e64 6578 6966 7920 6275 7420 6e6f   indexify but no
+000013a0: 206a 6f62 5f69 6e64 6578 206b 6579 2077   job_index key w
+000013b0: 6173 2066 6f75 6e64 2e20 736b 6970 7069  as found. skippi
+000013c0: 6e67 2061 6e64 206d 6f76 696e 6720 6f6e  ng and moving on
+000013d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000013e0: 0003 0000 0053 0000 0073 1000 0000 6700  .....S...s....g.
+000013f0: 7c00 5d08 7d01 7c01 9102 7104 5300 720d  |.].}.|...q.S.r.
+00001400: 0000 0072 0d00 0000 2902 7212 0000 00da  ...r....).r.....
+00001410: 0172 720d 0000 0072 0d00 0000 720e 0000  .rr....r....r...
+00001420: 0072 3c00 0000 a100 0000 723d 0000 007a  .r<.......r=...z
+00001430: 2472 6561 645f 6f75 7470 7574 5f66 696c  $read_output_fil
+00001440: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+00001450: 636f 6d70 3e72 2b00 0000 7201 0000 007a  comp>r+...r....z
+00001460: 2743 6f6e 6675 7365 6420 6162 6f75 7420  'Confused about 
+00001470: 6861 7669 6e67 206d 756c 7469 706c 6520  having multiple 
+00001480: 726f 7773 2069 6e20 2915 724a 0000 0072  rows in ).rJ...r
+00001490: 2500 0000 7227 0000 00da 0675 7064 6174  %...r'.....updat
+000014a0: 65da 0b64 6174 6163 6c61 7373 6573 da06  e..dataclasses..
+000014b0: 6173 6469 6374 724d 0000 0072 0400 0000  asdictrM...r....
+000014c0: da07 5f6c 6f67 6765 72da 0777 6172 6e69  .._logger..warni
+000014d0: 6e67 da08 696e 6465 7869 6679 7224 0000  ng..indexifyr$..
+000014e0: 00da 084b 6579 4572 726f 72da 046f 7065  ...KeyError..ope
+000014f0: 6eda 0363 7376 da0a 4469 6374 5265 6164  n..csv..DictRead
+00001500: 6572 722d 0000 0072 4100 0000 7247 0000  err-...rA...rG..
+00001510: 0072 4500 0000 7228 0000 0029 0d72 4600  .rE...r(...).rF.
+00001520: 0000 724e 0000 005a 0f70 6172 7365 645f  ..rN...Z.parsed_
+00001530: 6669 6c65 6e61 6d65 da03 7461 67da 036f  filename..tag..o
+00001540: 7574 5a0a 7061 7273 6564 5f74 6167 724f  utZ.parsed_tagrO
+00001550: 0000 005a 0a69 6e64 6578 6966 6965 645a  ...Z.indexifiedZ
+00001560: 0a69 6e70 7574 5f66 696c 65da 0672 6561  .input_file..rea
+00001570: 6465 72da 0472 6f77 7372 3900 0000 7228  der..rowsr9...r(
+00001580: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00001590: 0000 da10 7265 6164 5f6f 7574 7075 745f  ....read_output_
+000015a0: 6669 6c65 8500 0000 7336 0000 0000 040c  file....s6......
+000015b0: 010e 0212 010a 0108 0104 010a ff06 040c  ................
+000015c0: 0108 0102 0108 010e 0110 010c 0204 010a  ................
+000015d0: ff0a 040a 010a 010e 010c 010a 0230 0108  .............0..
+000015e0: 0206 0272 5f00 0000 2901 722b 0000 0029  ...r_...).r+...)
+000015f0: 2072 5200 0000 7235 0000 0072 1e00 0000   rR...r5...r....
+00001600: da07 6c6f 6767 696e 67da 1064 6565 7064  ..logging..deepd
+00001610: 6f67 2e69 6e64 6578 6966 79da 0764 6565  og.indexify..dee
+00001620: 7064 6f67 720b 0000 0072 5900 0000 da09  pdogr....rY.....
+00001630: 6765 744c 6f67 6765 7272 0600 0000 7254  getLoggerr....rT
+00001640: 0000 0072 4800 0000 7234 0000 0072 4c00  ...rH...r4...rL.
+00001650: 0000 da09 6461 7461 636c 6173 7372 0200  ....dataclassr..
+00001660: 0000 720f 0000 0072 2000 0000 7225 0000  ..r....r ...r%..
+00001670: 0072 3100 0000 7209 0000 00da 084f 7074  .r1...r......Opt
+00001680: 696f 6e61 6c72 3800 0000 721f 0000 0072  ionalr8...r....r
+00001690: 2a00 0000 7245 0000 0072 0c00 0000 724a  *...rE...r....rJ
+000016a0: 0000 0072 4d00 0000 7256 0000 00da 0a49  ...rM...rV.....I
+000016b0: 6e64 6578 6966 6965 7272 5f00 0000 720d  ndexifierr_...r.
+000016c0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000016d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000016e0: 7342 0000 0008 0108 0108 0108 0108 0108  sB..............
+000016f0: 0108 020a 0204 0302 ff04 0502 0102 fe04  ................
+00001700: 0604 0110 0604 0110 0f04 0110 0604 0110  ................
+00001710: 060a 0902 0108 fe0c 100c 0108 fe0c 1e12  ................
+00001720: 0b20 0a10 0102 fe                        . .....
```

### Comparing `deepdog-0.8.1/deepdog/subset_simulation/__pycache__/subset_simulation_impl.cpython-39.pyc` & `deepdog-1.0.0/deepdog/subset_simulation/__pycache__/subset_simulation_impl.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 09:28:40 2024 UTC, .py size: 11428 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 c816 2e66 a42c 0000  a..........f.,..
+00000000: 610d 0d0a 0000 0000 1bab 3266 a42c 0000  a.........2f.,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a03 6400 6402 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6500 a00c 650d a101 5a0e  m.Z...e...e...Z.
@@ -33,15 +33,15 @@
 00000200: 7175 616c 6e61 6d65 5f5f 7202 0000 0072  qualname__r....r
 00000210: 0300 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
 00000220: 6f6e 735f 5f72 0400 0000 da05 666c 6f61  ons__r......floa
 00000230: 74a9 0072 1200 0000 7212 0000 00fa 6d2f  t..r....r.....m/
 00000240: 686f 6d65 2f6a 656e 6b69 6e73 2f61 6765  home/jenkins/age
 00000250: 6e74 2f77 6f72 6b73 7061 6365 2f67 6974  nt/workspace/git
 00000260: 6561 2d70 6879 7369 6373 5f64 6565 7064  ea-physics_deepd
-00000270: 6f67 5f30 2e38 2e31 2f64 6565 7064 6f67  og_0.8.1/deepdog
+00000270: 6f67 5f31 2e30 2e30 2f64 6565 7064 6f67  og_1.0.0/deepdog
 00000280: 2f73 7562 7365 745f 7369 6d75 6c61 7469  /subset_simulati
 00000290: 6f6e 2f73 7562 7365 745f 7369 6d75 6c61  on/subset_simula
 000002a0: 7469 6f6e 5f69 6d70 6c2e 7079 7206 0000  tion_impl.pyr...
 000002b0: 000d 0000 0073 0c00 0000 0a02 0c01 0c01  .....s..........
 000002c0: 0c01 0c01 0c01 7206 0000 0063 0000 0000  ......r....c....
 000002d0: 0000 0000 0000 0000 0000 0000 0c00 0000  ................
 000002e0: 4000 0000 7354 0000 0065 005a 0164 005a  @...sT...e.Z.d.Z
@@ -290,15 +290,15 @@
 00001210: 7465 7263 0100 0000 0000 0000 0000 0000  terc............
 00001220: 0300 0000 0400 0000 5300 0000 7314 0000  ........S...s...
 00001230: 0067 007c 005d 0c5c 027d 017d 027c 0291  .g.|.].\.}.}.|..
 00001240: 0271 0453 0072 1200 0000 7212 0000 00a9  .q.S.r....r.....
 00001250: 0372 2200 0000 724b 0000 00da 0173 7212  .r"...rK.....sr.
 00001260: 0000 0072 1200 0000 7213 0000 0072 2400  ...r....r....r$.
 00001270: 0000 9800 0000 7225 0000 007a 0c67 6f74  ......r%...z.got
-00001280: 2073 7464 6576 733a 2072 1600 0000 da01   stdevs: r......
+00001280: 2073 7464 6576 733a 2072 1600 0000 fa01   stdevs: r......
 00001290: 097a 233a 2064 6f69 6e67 206c 6f6e 6720  .z#: doing long 
 000012a0: 6368 6169 6e20 6f6e 2074 6865 206e 6578  chain on the nex
 000012b0: 7420 7365 6564 69e8 0300 0029 02da 0c69  t seedi....)...i
 000012c0: 6e69 7469 616c 5f63 6f73 74da 0772 6e67  nitial_cost..rng
 000012d0: 5f61 7267 5a16 6c6f 6e67 5f63 6861 696e  _argZ.long_chain
 000012e0: 5f67 656e 6572 6174 696f 6e5f 7249 0000  _generation_rI..
 000012f0: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
```

### Comparing `deepdog-0.8.1/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-1.0.0/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.8.1/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-1.0.0/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.8.1/pyproject.toml` & `deepdog-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.8.1"
+version = "1.0.0"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
-pdme = "^0.9.3"
+pdme = "^1.0.0"
 numpy = "1.22.3"
 scipy = "1.10"
 tqdm = "^4.66.2"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.1"
```

