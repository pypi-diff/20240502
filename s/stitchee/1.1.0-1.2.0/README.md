# Comparing `tmp/stitchee-1.1.0.tar.gz` & `tmp/stitchee-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchee-1.1.0.tar", max compression
+gzip compressed data, was "stitchee-1.2.0.tar", max compression
```

## Comparing `stitchee-1.1.0.tar` & `stitchee-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-23 18:53:07.650636 stitchee-1.1.0/LICENSE
--rw-r--r--   0        0        0     4286 2024-04-23 18:53:07.650636 stitchee-1.1.0/README.md
--rw-r--r--   0        0        0       92 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/__init__.py
--rw-r--r--   0        0        0     8580 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/attribute_handling.py
--rw-r--r--   0        0        0    14343 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/dataset_and_group_handling.py
--rw-r--r--   0        0        0     5388 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/dimension_cleanup.py
--rw-r--r--   0        0        0      282 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/file_ops.py
--rw-r--r--   0        0        0        0 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/__init__.py
--rw-r--r--   0        0        0      882 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/cli.py
--rw-r--r--   0        0        0     3578 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/download_worker.py
--rw-r--r--   0        0        0     7569 2024-04-23 18:53:07.650636 stitchee-1.1.0/concatenator/harmony/service_adapter.py
--rw-r--r--   0        0        0     3817 2024-04-23 18:53:07.654636 stitchee-1.1.0/concatenator/harmony/util.py
--rw-r--r--   0        0        0     9134 2024-04-23 18:53:07.654636 stitchee-1.1.0/concatenator/run_stitchee.py
--rw-r--r--   0        0        0     7741 2024-04-23 18:53:07.654636 stitchee-1.1.0/concatenator/stitchee.py
--rw-r--r--   0        0        0     1419 2024-04-23 18:53:25.774613 stitchee-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5385 1970-01-01 00:00:00.000000 stitchee-1.1.0/setup.py
--rw-r--r--   0        0        0     5123 1970-01-01 00:00:00.000000 stitchee-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 15:35:44.748047 stitchee-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4634 2024-05-01 15:35:44.748047 stitchee-1.2.0/README.md
+-rw-r--r--   0        0        0       92 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/__init__.py
+-rw-r--r--   0        0        0     8580 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/attribute_handling.py
+-rw-r--r--   0        0        0    14694 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/dataset_and_group_handling.py
+-rw-r--r--   0        0        0     5388 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/dimension_cleanup.py
+-rw-r--r--   0        0        0      282 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/file_ops.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/harmony/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/harmony/cli.py
+-rw-r--r--   0        0        0     3578 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/harmony/download_worker.py
+-rw-r--r--   0        0        0     7569 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/harmony/service_adapter.py
+-rw-r--r--   0        0        0     3817 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/harmony/util.py
+-rw-r--r--   0        0        0     9134 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/run_stitchee.py
+-rw-r--r--   0        0        0     7739 2024-05-01 15:35:44.748047 stitchee-1.2.0/concatenator/stitchee.py
+-rw-r--r--   0        0        0     1427 2024-05-01 15:35:58.192178 stitchee-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 stitchee-1.2.0/setup.py
+-rw-r--r--   0        0        0     5471 1970-01-01 00:00:00.000000 stitchee-1.2.0/PKG-INFO
```

### Comparing `stitchee-1.1.0/LICENSE` & `stitchee-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/README.md` & `stitchee-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,20 @@
     </a>
     <a href="https://github.com/python/black" target="_blank">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">
     </a>
     <a href="http://mypy-lang.org/" target="_blank">
         <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">
     </a>
+    <a href="https://pypi.org/project/stitchee/" target="_blank">
+        <img src="https://img.shields.io/pypi/pyversions/stitchee.svg" alt="Python Versions">
+    </a>
+<a href="https://pypi.org/project/stitchee" target="_blank">
+    <img src="https://img.shields.io/pypi/v/stitchee?color=%2334D058label=pypi%20package" alt="Package version">
+</a>
     <a href="https://codecov.io/gh/nasa/stitchee">
      <img src="https://codecov.io/gh/nasa/stitchee/graph/badge.svg?token=WDj92iN7c4" alt="Code coverage">
     </a>
 </p>
 
 [//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
   [stitchee, a python package for concatenating netCDF data along an existing
                                   dimension]
 _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
-     _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
+_i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_a_c_k_a_g_e
+                            _v_e_r_s_i_o_n_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
 [//]: # (Using deprecated `align="center"` for the logo image and badges above,
 because of https://stackoverflow.com/a/62383408) # Overview _____ _STITCHEE_
 (STITCH by Extending a dimEnsion) is used for concatenating netCDF data *along
 an existing dimension*, and it is deigned as both a standalone utility and for
 use as a service in [Harmony](https://harmony.earthdata.nasa.gov/). ## Getting
 started, with poetry 1. Follow the instructions for installing `poetry` [here]
 (https://python-poetry.org/docs/). 2. Install `stitchee`, with its
```

### Comparing `stitchee-1.1.0/concatenator/attribute_handling.py` & `stitchee-1.2.0/concatenator/attribute_handling.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/concatenator/dataset_and_group_handling.py` & `stitchee-1.2.0/concatenator/dataset_and_group_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,20 +228,25 @@
                     chunk_sizes = _calculate_chunks(dim_sizes, default_low_dim_chunksize=4000)
 
                 # Do the variable creation
                 if var.dtype == "O":
                     vartype = "S1"
                 else:
                     vartype = str(var.dtype)
+
+                compression: str | None = "zlib"
+                if vartype.startswith("<U") and len(var.shape) == 1 and var.shape[0] < 10:
+                    compression = None
+
                 var_group.createVariable(
                     new_var_name,
                     vartype,
                     dimensions=new_var_dims,
                     chunksizes=chunk_sizes,
-                    compression="zlib",
+                    compression=compression,
                     complevel=7,
                     shuffle=shuffle,
                     fill_value=fill_value,
                 )
 
                 # copy variable attributes all at once via dictionary
                 var_group[new_var_name].setncatts(var.attrs)
@@ -313,26 +318,30 @@
                 break
 
     if dim_size is None:
         print(f"Dimension {dim_name} not found when searching for sizes!")
     return dim_size
 
 
-def validate_workable_files(files_to_concat, logger) -> tuple[list[str], int]:
+def validate_workable_files(files, logger) -> tuple[list[str], int]:
     """Remove files from list that are not open-able as netCDF or that are empty."""
     workable_files = []
-    for file in files_to_concat:
+    for file in files:
         try:
             with nc.Dataset(file, "r") as dataset:
                 is_empty = _is_file_empty(dataset)
                 if is_empty is False:
                     workable_files.append(file)
         except OSError:
             logger.debug("Error opening <%s> as a netCDF dataset. Skipping.", file)
 
+    # addressing the issue 153: propagate first empty file if all input files are empty
+    if (len(workable_files)) == 0 and (len(files) > 0):
+        workable_files.append(files[0])
+
     number_of_workable_files = len(workable_files)
 
     return workable_files, number_of_workable_files
 
 
 def _is_file_empty(parent_group: nc.Dataset | nc.Group) -> bool:
     """Check if netCDF dataset is empty or not.
```

### Comparing `stitchee-1.1.0/concatenator/dimension_cleanup.py` & `stitchee-1.2.0/concatenator/dimension_cleanup.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/concatenator/harmony/cli.py` & `stitchee-1.2.0/concatenator/harmony/cli.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/concatenator/harmony/download_worker.py` & `stitchee-1.2.0/concatenator/harmony/download_worker.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/concatenator/harmony/service_adapter.py` & `stitchee-1.2.0/concatenator/harmony/service_adapter.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/concatenator/harmony/util.py` & `stitchee-1.2.0/concatenator/harmony/util.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/concatenator/run_stitchee.py` & `stitchee-1.2.0/concatenator/run_stitchee.py`

 * *Files identical despite different names*

### Comparing `stitchee-1.1.0/concatenator/stitchee.py` & `stitchee-1.2.0/concatenator/stitchee.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 combined_ds = xr.combine_by_coords(
                     xrdataset_list,
                     data_vars="minimal",
                     coords="minimal",
                     **concat_kwargs,
                 )
             else:
-                raise ValueError("Unexpected concatenation method, <%s>." % concat_method)
+                raise ValueError(f"Unexpected concatenation method, <{concat_method}>.")
 
             benchmark_log["concatenating"] = time.time() - start_time
 
             if write_tmp_flat_concatenated:
                 logger.info("Writing concatenated flattened temporary file to disk...")
                 # Concatenated, yet still flat, file is written to disk for debugging.
                 tmp_flat_concatenated_path = add_label_to_path(
```

### Comparing `stitchee-1.1.0/pyproject.toml` & `stitchee-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stitchee"
-version = "1.1.0"
+version = "1.2.0"
 description = "NetCDF4 Along-existing-dimension Concatenation Service"
 authors = ["Daniel Kaufman <daniel.kaufman@nasa.gov>"]
 readme = "README.md"
 repository = "https://github.com/nasa/stitchee"
 license = "Apache-2.0"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -24,15 +24,15 @@
 dask = "^2024.4.1"
 harmony-service-lib = "^1.0.25"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 mypy = "^1.9.0"
 black = "^24.4.0"
-ruff = "^0.3.7"
+ruff = ">=0.3.7,<0.5.0"
 coverage = "^7.4.4"
 pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stitchee-1.1.0/setup.py` & `stitchee-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['stitchee = concatenator.run_stitchee:main',
                      'stitchee_harmony = concatenator.harmony.cli:main']}
 
 setup_kwargs = {
     'name': 'stitchee',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'NetCDF4 Along-existing-dimension Concatenation Service',
-    'long_description': '<p align="center">\n    <img alt="stitchee, a python package for concatenating netCDF data along an existing dimension"\n    src="https://github.com/danielfromearth/stitchee/assets/114174502/58052dfa-b6e1-49e5-96e5-4cb1e8d14c32" width="250"\n    />\n</p>\n\n<p align="center">\n    <a href="https://www.repostatus.org/#active" target="_blank">\n        <img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed">\n    </a>\n    <a href="https://github.com/python/black" target="_blank">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">\n    </a>\n    <a href="http://mypy-lang.org/" target="_blank">\n        <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">\n    </a>\n    <a href="https://codecov.io/gh/nasa/stitchee">\n     <img src="https://codecov.io/gh/nasa/stitchee/graph/badge.svg?token=WDj92iN7c4" alt="Code coverage">\n    </a>\n</p>\n\n[//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)\n\n# Overview\n_____\n\n_STITCHEE_ (STITCH by Extending a dimEnsion) is used for concatenating netCDF data *along an existing dimension*,\nand it is deigned as both a standalone utility and for use as a service in [Harmony](https://harmony.earthdata.nasa.gov/).\n\n## Getting started, with poetry\n\n1. Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n2. Install `stitchee`, with its dependencies, by running the following from the repository directory:\n\n```shell\npoetry install\n```\n\n## How to test `stitchee` locally\n\n```shell\npoetry run pytest tests/\n```\n\n## Usage\n\n```shell\n$ poetry run stitchee --help\nusage: stitchee [-h] -o OUTPUT_PATH [--no_input_file_copies] [--keep_tmp_files] [--concat_method {xarray-concat,xarray-combine}] [--concat_dim CONCAT_DIM]\n                [--xarray_arg_compat XARRAY_ARG_COMPAT] [--xarray_arg_combine_attrs XARRAY_ARG_COMBINE_ATTRS] [--xarray_arg_join XARRAY_ARG_JOIN] [-O]\n                [-v]\n                path/directory or path list [path/directory or path list ...]\n\nRun the along-existing-dimension concatenator.\n\noptions:\n  -h, --help            show this help message and exit\n  --no_input_file_copies\n                        By default, input files are copied into a temporary directory to avoid modification of input files. This is useful for testing,\n                        but uses more disk space. By specifying this argument, no copying is performed.\n  --keep_tmp_files      Prevents removal, after successful execution, of (1) the flattened concatenated file and (2) the input directory copy if created\n                        by \'--make_dir_copy\'.\n  --concat_method {xarray-concat,xarray-combine}\n                        Whether to use the xarray concat method or the combine-by-coords method.\n  --concat_dim CONCAT_DIM\n                        Dimension to concatenate along, if possible. This is required if using the \'xarray-concat\' method\n  --xarray_arg_compat XARRAY_ARG_COMPAT\n                        \'compat\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  --xarray_arg_combine_attrs XARRAY_ARG_COMBINE_ATTRS\n                        \'combine_attrs\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  --xarray_arg_join XARRAY_ARG_JOIN\n                        \'join\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  -O, --overwrite       Overwrite output file if it already exists.\n  -v, --verbose         Enable verbose output to stdout; useful for debugging\n\nRequired:\n  path/directory or path list\n                        Files to be concatenated, specified via a (1) single directory containing the files to be concatenated, (2) single text file\n                        containing linebreak-separated paths of the files to be concatenated, or (3) multiple filepaths of the files to be concatenated.\n  -o OUTPUT_PATH, --output_path OUTPUT_PATH\n                        The output filename for the merged output.\n```\n\nFor example:\n\n```shell\npoetry run stitchee /path/to/netcdf/directory/ -o /path/to/output.nc\n```\n\n---\nThis package is NASA Software Release Authorization (SRA) # LAR-20433-1\n',
+    'long_description': '<p align="center">\n    <img alt="stitchee, a python package for concatenating netCDF data along an existing dimension"\n    src="https://github.com/danielfromearth/stitchee/assets/114174502/58052dfa-b6e1-49e5-96e5-4cb1e8d14c32" width="250"\n    />\n</p>\n\n<p align="center">\n    <a href="https://www.repostatus.org/#active" target="_blank">\n        <img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed">\n    </a>\n    <a href="https://github.com/python/black" target="_blank">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">\n    </a>\n    <a href="http://mypy-lang.org/" target="_blank">\n        <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">\n    </a>\n    <a href="https://pypi.org/project/stitchee/" target="_blank">\n        <img src="https://img.shields.io/pypi/pyversions/stitchee.svg" alt="Python Versions">\n    </a>\n<a href="https://pypi.org/project/stitchee" target="_blank">\n    <img src="https://img.shields.io/pypi/v/stitchee?color=%2334D058label=pypi%20package" alt="Package version">\n</a>\n    <a href="https://codecov.io/gh/nasa/stitchee">\n     <img src="https://codecov.io/gh/nasa/stitchee/graph/badge.svg?token=WDj92iN7c4" alt="Code coverage">\n    </a>\n</p>\n\n[//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)\n\n# Overview\n_____\n\n_STITCHEE_ (STITCH by Extending a dimEnsion) is used for concatenating netCDF data *along an existing dimension*,\nand it is deigned as both a standalone utility and for use as a service in [Harmony](https://harmony.earthdata.nasa.gov/).\n\n## Getting started, with poetry\n\n1. Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n2. Install `stitchee`, with its dependencies, by running the following from the repository directory:\n\n```shell\npoetry install\n```\n\n## How to test `stitchee` locally\n\n```shell\npoetry run pytest tests/\n```\n\n## Usage\n\n```shell\n$ poetry run stitchee --help\nusage: stitchee [-h] -o OUTPUT_PATH [--no_input_file_copies] [--keep_tmp_files] [--concat_method {xarray-concat,xarray-combine}] [--concat_dim CONCAT_DIM]\n                [--xarray_arg_compat XARRAY_ARG_COMPAT] [--xarray_arg_combine_attrs XARRAY_ARG_COMBINE_ATTRS] [--xarray_arg_join XARRAY_ARG_JOIN] [-O]\n                [-v]\n                path/directory or path list [path/directory or path list ...]\n\nRun the along-existing-dimension concatenator.\n\noptions:\n  -h, --help            show this help message and exit\n  --no_input_file_copies\n                        By default, input files are copied into a temporary directory to avoid modification of input files. This is useful for testing,\n                        but uses more disk space. By specifying this argument, no copying is performed.\n  --keep_tmp_files      Prevents removal, after successful execution, of (1) the flattened concatenated file and (2) the input directory copy if created\n                        by \'--make_dir_copy\'.\n  --concat_method {xarray-concat,xarray-combine}\n                        Whether to use the xarray concat method or the combine-by-coords method.\n  --concat_dim CONCAT_DIM\n                        Dimension to concatenate along, if possible. This is required if using the \'xarray-concat\' method\n  --xarray_arg_compat XARRAY_ARG_COMPAT\n                        \'compat\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  --xarray_arg_combine_attrs XARRAY_ARG_COMBINE_ATTRS\n                        \'combine_attrs\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  --xarray_arg_join XARRAY_ARG_JOIN\n                        \'join\' argument passed to xarray.concat() or xarray.combine_by_coords().\n  -O, --overwrite       Overwrite output file if it already exists.\n  -v, --verbose         Enable verbose output to stdout; useful for debugging\n\nRequired:\n  path/directory or path list\n                        Files to be concatenated, specified via a (1) single directory containing the files to be concatenated, (2) single text file\n                        containing linebreak-separated paths of the files to be concatenated, or (3) multiple filepaths of the files to be concatenated.\n  -o OUTPUT_PATH, --output_path OUTPUT_PATH\n                        The output filename for the merged output.\n```\n\nFor example:\n\n```shell\npoetry run stitchee /path/to/netcdf/directory/ -o /path/to/output.nc\n```\n\n---\nThis package is NASA Software Release Authorization (SRA) # LAR-20433-1\n',
     'author': 'Daniel Kaufman',
     'author_email': 'daniel.kaufman@nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nasa/stitchee',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['concatenator', 'concatenator.harmony'] package_data = \ {'': ['*']}
 install_requires = \ ['dask>=2024.4.1,<2025.0.0', 'harmony-service-
 lib>=1.0.25,<2.0.0', 'netcdf4>=1.6.5,<2.0.0', 'xarray>=2024.3.0,<2025.0.0']
 entry_points = \ {'console_scripts': ['stitchee = concatenator.run_stitchee:
 main', 'stitchee_harmony = concatenator.harmony.cli:main']} setup_kwargs =
-{ 'name': 'stitchee', 'version': '1.1.0', 'description': 'NetCDF4 Along-
+{ 'name': 'stitchee', 'version': '1.2.0', 'description': 'NetCDF4 Along-
 existing-dimension Concatenation Service', 'long_description': '
     \n n src="https://github.com/danielfromearth/stitchee/assets/114174502/
            58052dfa-b6e1-49e5-96e5-4cb1e8d14c32" width="250"\n />\n
 \n\n
   \n _\_n_ _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e
    _s_t_a_t_e_ _a_n_d_ _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_\_n_ \n _\_n_ _[_C_o_d_e_ _s_t_y_l_e_]_\_n_ \n _\_n_ _[_M_y_p_y
-                     _c_h_e_c_k_e_d_]_\_n_ \n _\_n_ _[_C_o_d_e_ _c_o_v_e_r_a_g_e_]_\_n_ \n
+   _c_h_e_c_k_e_d_]_\_n_ \n _\_n_ _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_\_n_ \n_\_n_ _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_\_n\n _\_n_ _[_C_o_d_e
+                                _c_o_v_e_r_a_g_e_]_\_n_ \n
 \n\n[//]: # (Using deprecated `align="center"` for the logo image and badges
 above, because of https://stackoverflow.com/a/62383408)\n\n#
 Overview\n_____\n\n_STITCHEE_ (STITCH by Extending a dimEnsion) is used for
 concatenating netCDF data *along an existing dimension*,\nand it is deigned as
 both a standalone utility and for use as a service in [Harmony](https://
 harmony.earthdata.nasa.gov/).\n\n## Getting started, with poetry\n\n1. Follow
 the instructions for installing `poetry` [here](https://python-poetry.org/docs/
```

### Comparing `stitchee-1.1.0/PKG-INFO` & `stitchee-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stitchee
-Version: 1.1.0
+Version: 1.2.0
 Summary: NetCDF4 Along-existing-dimension Concatenation Service
 Home-page: https://github.com/nasa/stitchee
 License: Apache-2.0
 Author: Daniel Kaufman
 Author-email: daniel.kaufman@nasa.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,14 +31,20 @@
     </a>
     <a href="https://github.com/python/black" target="_blank">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style">
     </a>
     <a href="http://mypy-lang.org/" target="_blank">
         <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="Mypy checked">
     </a>
+    <a href="https://pypi.org/project/stitchee/" target="_blank">
+        <img src="https://img.shields.io/pypi/pyversions/stitchee.svg" alt="Python Versions">
+    </a>
+<a href="https://pypi.org/project/stitchee" target="_blank">
+    <img src="https://img.shields.io/pypi/v/stitchee?color=%2334D058label=pypi%20package" alt="Package version">
+</a>
     <a href="https://codecov.io/gh/nasa/stitchee">
      <img src="https://codecov.io/gh/nasa/stitchee/graph/badge.svg?token=WDj92iN7c4" alt="Code coverage">
     </a>
 </p>
 
 [//]: # (Using deprecated `align="center"` for the logo image and badges above, because of https://stackoverflow.com/a/62383408)
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: stitchee Version: 1.1.0 Summary: NetCDF4 Along-
+Metadata-Version: 2.1 Name: stitchee Version: 1.2.0 Summary: NetCDF4 Along-
 existing-dimension Concatenation Service Home-page: https://github.com/nasa/
 stitchee License: Apache-2.0 Author: Daniel Kaufman Author-email:
 daniel.kaufman@nasa.gov Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Dist: dask (>=2024.4.1,<2025.0.0)
 Requires-Dist: harmony-service-lib (>=1.0.25,<2.0.0) Requires-Dist: netcdf4
 (>=1.6.5,<2.0.0) Requires-Dist: xarray (>=2024.3.0,<2025.0.0) Project-URL:
 Repository, https://github.com/nasa/stitchee Description-Content-Type: text/
 markdown
   [stitchee, a python package for concatenating netCDF data along an existing
                                   dimension]
 _[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
-     _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
+_i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_]_[_C_o_d_e_ _s_t_y_l_e_]_[_M_y_p_y_ _c_h_e_c_k_e_d_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_P_a_c_k_a_g_e
+                            _v_e_r_s_i_o_n_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]
 [//]: # (Using deprecated `align="center"` for the logo image and badges above,
 because of https://stackoverflow.com/a/62383408) # Overview _____ _STITCHEE_
 (STITCH by Extending a dimEnsion) is used for concatenating netCDF data *along
 an existing dimension*, and it is deigned as both a standalone utility and for
 use as a service in [Harmony](https://harmony.earthdata.nasa.gov/). ## Getting
 started, with poetry 1. Follow the instructions for installing `poetry` [here]
 (https://python-poetry.org/docs/). 2. Install `stitchee`, with its
```

