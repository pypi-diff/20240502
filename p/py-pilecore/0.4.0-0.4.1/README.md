# Comparing `tmp/py-pilecore-0.4.0.tar.gz` & `tmp/py_pilecore-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-pilecore-0.4.0.tar", last modified: Tue Mar 12 20:16:05 2024, max compression
+gzip compressed data, was "py_pilecore-0.4.1.tar", last modified: Thu May  2 13:28:31 2024, max compression
```

## Comparing `py-pilecore-0.4.0.tar` & `py_pilecore-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:16:05.950549 py-pilecore-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-03-12 20:16:05.950549 py-pilecore-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 20:16:05.950549 py-pilecore-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:16:05.942549 py-pilecore-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:16:05.946549 py-pilecore-0.4.0/src/py_pilecore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-03-12 20:16:05.000000 py-pilecore-0.4.0/src/py_pilecore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-12 20:16:05.000000 py-pilecore-0.4.0/src/py_pilecore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 20:16:05.000000 py-pilecore-0.4.0/src/py_pilecore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-12 20:16:05.000000 py-pilecore-0.4.0/src/py_pilecore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 20:16:05.000000 py-pilecore-0.4.0/src/py_pilecore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:16:05.942549 py-pilecore-0.4.0/src/pypilecore/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:16:05.942549 py-pilecore-0.4.0/src/pypilecore/input/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/input/grouper_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    19539 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/input/multi_cpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/input/pile_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/input/soil_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:16:05.946549 py-pilecore-0.4.0/src/pypilecore/results/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30903 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/grouper_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/load_settlement.py
--rw-r--r--   0 runner    (1001) docker     (127)    25398 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/multi_cpt_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    28592 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/pile_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/single_cpt_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    20722 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/results/soil_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/src/pypilecore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:16:05.946549 py-pilecore-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    24794 2024-03-12 20:16:02.000000 py-pilecore-0.4.0/tests/test_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.184058 py_pilecore-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-02 13:28:31.184058 py_pilecore-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:28:31.184058 py_pilecore-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.172057 py_pilecore-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.180057 py_pilecore-0.4.1/src/py_pilecore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 13:28:31.000000 py_pilecore-0.4.1/src/py_pilecore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.176057 py_pilecore-0.4.1/src/pypilecore/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.176057 py_pilecore-0.4.1/src/pypilecore/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/grouper_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/multi_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/pile_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/input/soil_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.180057 py_pilecore-0.4.1/src/pypilecore/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30927 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/grouper_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/load_settlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25398 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/multi_cpt_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28592 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/pile_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/single_cpt_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20722 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/results/soil_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/src/pypilecore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:28:31.180057 py_pilecore-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-05-02 13:28:27.000000 py_pilecore-0.4.1/tests/test_input.py
```

### Comparing `py-pilecore-0.4.0/LICENSE` & `py_pilecore-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/PKG-INFO` & `py_pilecore-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pilecore
-Version: 0.4.0
+Version: 0.4.1
 Summary: Public python SDK for the CEMS PileCore web-API.
 License: MIT License
         
         Copyright (c) 2023 CEMS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -33,14 +33,15 @@
 Requires-Dist: numpy<2,>1
 Requires-Dist: pandas<3,>2
 Requires-Dist: cems-nuclei[client]<1,>=0.5
 Requires-Dist: matplotlib<4,>=3.8
 Requires-Dist: tqdm[notebook]<5,>4
 Requires-Dist: natsort<9,>8
 Requires-Dist: shapely<3,>=2
+Requires-Dist: scipy<2,>=1
 Provides-Extra: test
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
 Requires-Dist: Sphinx==6.1.3; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.22; extra == "docs"
 Requires-Dist: ipython==8.11.0; extra == "docs"
```

### Comparing `py-pilecore-0.4.0/README.md` & `py_pilecore-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/pyproject.toml` & `py_pilecore-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-pilecore"
-version = "0.4.0"
+version = "0.4.1"
 description = "Public python SDK for the CEMS PileCore web-API."
 requires-python = ">=3.9"
 dependencies = [
     'pygef>0.8,<1',
     'numpy>1,<2',
     'pandas>2,<3',
     'cems-nuclei[client]>=0.5,<1',
     'matplotlib>=3.8,<4',
     "tqdm[notebook]>4,<5",
     "natsort>8,<9",
     "shapely>=2,<3",
+    "scipy>=1, <2",
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 keywords = ["API", "PileCore", "CEMS", "CRUX"]
 
 [project.urls]
 repository = "https://github.com/cemsbv/py-pilecore"
```

### Comparing `py-pilecore-0.4.0/src/py_pilecore.egg-info/PKG-INFO` & `py_pilecore-0.4.1/src/py_pilecore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pilecore
-Version: 0.4.0
+Version: 0.4.1
 Summary: Public python SDK for the CEMS PileCore web-API.
 License: MIT License
         
         Copyright (c) 2023 CEMS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -33,14 +33,15 @@
 Requires-Dist: numpy<2,>1
 Requires-Dist: pandas<3,>2
 Requires-Dist: cems-nuclei[client]<1,>=0.5
 Requires-Dist: matplotlib<4,>=3.8
 Requires-Dist: tqdm[notebook]<5,>4
 Requires-Dist: natsort<9,>8
 Requires-Dist: shapely<3,>=2
+Requires-Dist: scipy<2,>=1
 Provides-Extra: test
 Requires-Dist: coveralls; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
 Requires-Dist: Sphinx==6.1.3; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.22; extra == "docs"
 Requires-Dist: ipython==8.11.0; extra == "docs"
```

### Comparing `py-pilecore-0.4.0/src/py_pilecore.egg-info/SOURCES.txt` & `py_pilecore-0.4.1/src/py_pilecore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/py_pilecore.egg-info/requires.txt` & `py_pilecore-0.4.1/src/py_pilecore.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 numpy<2,>1
 pandas<3,>2
 cems-nuclei[client]<1,>=0.5
 matplotlib<4,>=3.8
 tqdm[notebook]<5,>4
 natsort<9,>8
 shapely<3,>=2
+scipy<2,>=1
 
 [docs]
 Sphinx==6.1.3
 sphinx-autodoc-typehints==1.22
 ipython==8.11.0
 asteroid-sphinx-theme==0.0.3
 sphinx_rtd_theme==1.2.0
```

### Comparing `py-pilecore-0.4.0/src/pypilecore/api.py` & `py_pilecore-0.4.1/src/pypilecore/api.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/input/__init__.py` & `py_pilecore-0.4.1/src/pypilecore/input/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/input/grouper_properties.py` & `py_pilecore-0.4.1/src/pypilecore/input/grouper_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,28 +39,27 @@
     skip_nan: bool = False,
 ) -> dict:
     """
     Creates a dictionary with the payload content for the PileCore endpoint
     "/grouper/group_cpts"
 
 
-    Notes
+    Note
     ------
     The grouper uses pile bearing capacity results calculated by PileCore or other software to
     form  subgroups of the total group of CPT’s belonging to this project.
     Valid subgroups have three characteristics:
 
         - a maximum variation coefficient of 12% at one or more pile-tip levels. (Variation check
           NEN9997-1 A.3.3.3)
         - a minimum design pile bearing capacity based on the given pile load ULS at one or more
           pile-tip levels. (Bearing check)
         - is spatially coherent, which means there are no other CPTs in between the members
           of the subgroup. (Spatial check)
 
-
     Additionally, centre to centre validation (include_centre_to_centre_check; NEN9997-1 3.2.3) can be
     added to the cluster method. This check adds restrictions to the maximum allowable R;c;cal outliers
     and makes sure that the suitable data density requirements for the subgroup are met, by checking the
     centre-to-centre (CTC) distance of the cpts in a regular square grid:
 
         - A maximum CTC distance of 25 m, if no R;c;cal outliers greater than 30% off the average;
         - A maximum CTC distance of 20 m, if no R;c;cal outliers greater than 40% off the average;
```

### Comparing `py-pilecore-0.4.0/src/pypilecore/input/multi_cpt.py` & `py_pilecore-0.4.1/src/pypilecore/input/multi_cpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
         pile_tip_levels_nap=list(pile_tip_levels_nap),
         list_soil_properties=soil_properties_list,
         pile_properties=pile_properties,
         friction_range_strategy=friction_range_strategy,
         pile_head_level_nap=pile_head_level_nap,
         stiff_construction=stiff_construction,
         rel_pile_load=relative_pile_load,
-        soil_load=soil_load_sls,
+        soil_load=soil_load_sls if soil_load_sls is not None else 0.0,
         excavation_param_t=excavation_param_t,
         use_almere_rules=use_almere_rules,
         gamma_f_nk=gamma_f_nk,
         gamma_r_b=gamma_r_b,
         gamma_r_s=gamma_r_s,
     )
```

### Comparing `py-pilecore-0.4.0/src/pypilecore/input/pile_properties.py` & `py_pilecore-0.4.1/src/pypilecore/input/pile_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,17 @@
     is_low_vibrating: float | None = None,
     negative_fr_delta_factor: float | None = None,
 ) -> dict:
     """
     Creates a dictionary with the `pile_properties` payload content for the PileCore
     endpoints.
 
-    Note that
-    the dictionary should be converted to a jsonifyable message before it can be passed
+    Note
+    ----
+    The dictionary should be converted to a jsonifyable message before it can be passed
     to a `requests` call directly, for instance with
     `nuclei.client.utils.python_types_to_message()`.
 
     Parameters
     ----------
     pile_type:
         The equaly named entry in the "pile_type_specification" settings.
```

### Comparing `py-pilecore-0.4.0/src/pypilecore/input/soil_properties.py` & `py_pilecore-0.4.1/src/pypilecore/input/soil_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     | None = None,
     individual_ocr: Mapping[Any, float] | None = None,
 ) -> Tuple[List[dict], Dict[str, dict]]:
     """
     Creates a dictionary with the `soil_properties` payload content for the PileCore
     endpoints.
 
-    Notes
+    Note
     ------
     the dictionary should be converted to a jsonifyable message before it can be passed
     to a `requests` call directly, for instance with
     `nuclei.client.utils.python_types_to_message()`.
 
     Parameters
     ----------
```

### Comparing `py-pilecore-0.4.0/src/pypilecore/plot_utils.py` & `py_pilecore-0.4.1/src/pypilecore/plot_utils.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/results/grouper_result.py` & `py_pilecore-0.4.1/src/pypilecore/results/grouper_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
     def plot_bearing_capacity(
         self, axes: plt.Axes | None = None, pile_load_uls: float = 0.0, **kwargs: Any
     ) -> None:
         """
         Plot the bearing capacity and variation coefficient in a subplot
 
-        Notes
+        Note
         ------
         For the `Net bearing capacity` subplot there are two colors plotted:
          - orange:  conservative bearing capacity
          - blue:    net bearing capacity
 
         Parameters
         ----------
@@ -247,15 +247,15 @@
 
     def plot_group_centre_to_centre_validation(
         self, axes: plt.Axes | None = None, **kwargs: Any
     ) -> None:
         """
         Plot the spacing checks in a subplot
 
-        Notes
+        Note
         ------
         For the `spacing` subplot there are two colors plotted:
          - red:     invalid spacing
          - green:   valid spacing
 
         Parameters
         ----------
@@ -304,15 +304,15 @@
         axes.set_xticks([0, 1, 2], ["25", "20", "15"])
         axes.set_xlabel("CPT ctc [m]")
 
     def plot_xi(self, axes: plt.Axes | None = None, **kwargs: Any) -> None:
         """
         Plot the xi factor in a subplot
 
-        Notes
+        Note
         ------
         For the `xi factor` subplot there are two colors plotted:
          - olive:   xi3
          - cyan:    xi4
 
         Parameters
         ----------
@@ -495,15 +495,15 @@
         """
         Plot contains the:
             - bearing capacity
             - variation coefficient
             - xi factor
             - centre to centre validation
 
-        Notes
+        Note
         ------
         For the `Net bearing capacity` subplot there are two colors plotted:
          - orange:  conservative bearing capacity
          - blue:    net bearing capacity
 
         For the `xi factor` subplot there are two colors plotted:
          - olive:   xi3
@@ -771,14 +771,17 @@
     def plot(
         self,
         figsize: Tuple[int, int] | None = None,
         **kwargs: Any,
     ) -> plt.Figure:
         """
         Plot a summary of the valid subgroups.
+
+        Note
+        -----
         Plot contains the:
 
             - cpts within a subgroup
                 - green:
                     There are no other CPTs in between the members of the subgroup. The
                     group is also compliant with the NEN9997-1 3.2.3 centre to centre
                     validation.
```

### Comparing `py-pilecore-0.4.0/src/pypilecore/results/load_settlement.py` & `py_pilecore-0.4.1/src/pypilecore/results/load_settlement.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/results/multi_cpt_results.py` & `py_pilecore-0.4.1/src/pypilecore/results/multi_cpt_results.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/results/pile_properties.py` & `py_pilecore-0.4.1/src/pypilecore/results/pile_properties.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/results/post_processing.py` & `py_pilecore-0.4.1/src/pypilecore/results/post_processing.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple
 
 import matplotlib.patches as patches
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
+from matplotlib.collections import PatchCollection
 from matplotlib.figure import Figure
 from numpy.typing import NDArray
+from scipy.spatial import Delaunay, Voronoi, voronoi_plot_2d
 
 from pypilecore.results.soil_properties import SoilProperties, get_soil_layer_handles
 
 
 class MaxBearingTable:
     """
     Object that contains the results belonging to the maximum net design bearing capacity (R_c_d_net) for a single CPT.
@@ -90,15 +92,15 @@
 
     Attributes
     ----------
     soil_properties
         The object with soil properties
     pile_head_level_nap
         The elevation of the pile-head, in [m] w.r.t. NAP.
-    results_table
+    table
         The object with CPT results.
     """
 
     soil_properties: SoilProperties
     pile_head_level_nap: float
     table: MaxBearingTable
 
@@ -367,14 +369,67 @@
         cpt_results_df = pd.concat(df_list)
         cpt_results_df = cpt_results_df.assign(
             pile_tip_level_nap=cpt_results_df.pile_tip_level_nap.round(1)
         )
 
         return cpt_results_df
 
+    @lru_cache()
+    def triangulation(self, pile_tip_level_nap: float) -> List[Dict[str, list]]:
+        """
+        Delaunay tessellation based on the CPT location
+
+        Returns
+        -------
+        collection: List
+            A list of dictionaries containing the tessellation
+            geometry and corresponding cpt names:
+
+                - geometry: List[Tuple[float, float]]
+                - test_id: List[str]
+
+        """
+        _lookup = {
+            (point.soil_properties.x, point.soil_properties.y): key
+            for key, point in self.cpt_results_dict.items()
+        }
+        # select point with valid bearing capacity at pile tip level
+        _points = (
+            self.to_pandas()
+            .loc[
+                (self.to_pandas()["pile_tip_level_nap"] == pile_tip_level_nap)
+                & (~pd.isna(self.to_pandas()["R_c_d_net"])),
+                ["x", "y"],
+            ]
+            .to_numpy()
+            .tolist()
+        )
+
+        # check if enough points Delaunay
+        if len(_points) < 4:
+            raise ValueError(
+                "Not enough points at this pile tip level to construct "
+                "the delaunay tessellation based on the CPT location."
+            )
+        tri = Delaunay(
+            _points,
+            incremental=False,
+            furthest_site=False,
+            qhull_options="Qbb",
+        )
+        geometries = np.array(_points)[tri.simplices]
+
+        return [
+            {
+                "geometry": geometry.tolist(),
+                "test_id": [_lookup[(xy[0], xy[1])] for xy in geometry],
+            }
+            for geometry in geometries
+        ]
+
     def plot(
         self,
         projection: Optional[Literal["3d"]] = "3d",
         hue: Literal["colormap", "category"] = "colormap",
         pile_load_uls: float = 100,
         figsize: Tuple[int, int] | None = None,
         **kwargs: Any,
@@ -409,28 +464,28 @@
             "figsize": figsize,
             "tight_layout": True,
         }
 
         kwargs_subplot.update(kwargs)
         fig = plt.figure(**kwargs_subplot)
         axes = fig.add_subplot(projection=projection)
+        df = self.to_pandas().dropna()
         # create color list based on hue option
         if hue == "category":
             colors = [
-                "red" if var < pile_load_uls else "green"
-                for var in self.to_pandas()["R_c_d_net"]
+                "red" if var < pile_load_uls else "green" for var in df["R_c_d_net"]
             ]
         else:
-            colors = self.to_pandas()["R_c_d_net"].tolist()
+            colors = df["R_c_d_net"].tolist()
         # create scatter plot
         if projection == "3d":
             cmap = axes.scatter(
-                self.to_pandas()["x"],
-                self.to_pandas()["y"],
-                self.to_pandas()["pile_tip_level_nap"],
+                df["x"],
+                df["y"],
+                df["pile_tip_level_nap"],
                 c=colors,
             )
             axes.set_xlabel("X")
             axes.set_ylabel("Y")
             axes.set_zlabel("Z [m w.r.t NAP]")
 
             # set cpt names
@@ -440,20 +495,21 @@
                     result.soil_properties.y,
                     result.table.pile_tip_level_nap.max(),
                     key,
                     "z",
                 )
         else:
             cmap = axes.scatter(
-                self.to_pandas()["test_id"],
-                self.to_pandas()["pile_tip_level_nap"],
+                df["test_id"],
+                df["pile_tip_level_nap"],
                 c=colors,
             )
             axes.set_ylabel("Z [m w.r.t NAP]")
             axes.tick_params(axis="x", labelrotation=90)
+            axes.grid()
 
         if hue == "category":
             fig.legend(
                 title="$R_{c;d;net}$ [kN]",
                 title_fontsize=18,
                 fontsize=15,
                 loc="lower right",
@@ -471,7 +527,153 @@
                     )
                 ],
             )
         else:
             fig.colorbar(cmap, orientation="vertical", label="$R_{c;d;net}$ [kN]")
 
         return fig
+
+    def map(
+        self,
+        pile_tip_level_nap: float,
+        pile_load_uls: float = 100,
+        show_delaunay_vertices: bool = True,
+        show_voronoi_vertices: bool = False,
+        figsize: Tuple[int, int] | None = None,
+        **kwargs: Any,
+    ) -> plt.Figure:
+        """
+        Plot a map of the valid ULS load for a given depth.
+
+        Note
+        ------
+        Based on the Delaunay methode a tessellation is created with
+        the location of the CPT's. Each triangle is then colored according to
+        the bearing capacity of the CPT its based on. If any of the CPT does
+        not meet the required capacity the triangle becomes also invalid.
+
+        Warnings
+        --------
+        Please note that this map indication of valid ULS zones is intended as a visual aid to help
+        the geotechnical engineer. It does not necessarily comply with the NEN 9997-1+C2:2017 since the NEN is open
+        to interpretation. It is therefore that the interpretation provided by this methode must be carefully
+        validated by a geotechnical engineer.
+
+        Parameters
+        ----------
+        pile_tip_level_nap:
+            Pile tip level to generate map.
+        pile_load_uls
+            default is 100 kN
+            ULS load in kN. Used to determine if a pile tip level configuration is valid.
+        show_delaunay_vertices
+            default is True
+            Add delaunay vertices to the figure
+        show_voronoi_vertices
+            default is False
+            Add voronoi vertices to the figure
+        figsize:
+            Size of the activate figure, as the `plt.figure()` argument.
+        **kwargs:
+            All additional keyword arguments are passed to the `pyplot.subplots()` call.
+
+        Returns
+        -------
+        figure:
+            The `Figure` object where the data was plotted on.
+        """
+        kwargs_subplot = {
+            "figsize": figsize,
+            "tight_layout": True,
+        }
+
+        kwargs_subplot.update(kwargs)
+        fig, axes = plt.subplots(**kwargs_subplot)
+
+        # filter data
+        df = (
+            self.to_pandas()
+            .loc[self.to_pandas()["pile_tip_level_nap"] == pile_tip_level_nap]
+            .dropna()
+        )
+
+        if df.empty:
+            raise ValueError(
+                "Pile tip level is not valid pile tip level. "
+                "Please select one of the following pile tip level: "
+                f"[{(self.to_pandas()['pile_tip_level_nap']).unique()}]"
+            )
+
+        df["valid"] = [
+            False if var < pile_load_uls else True for var in df["R_c_d_net"]
+        ]
+
+        # iterate over geometry
+        if show_delaunay_vertices:
+            _patches = []
+            for tri in self.triangulation(pile_tip_level_nap):
+                color = (
+                    "green"
+                    if all(
+                        df.where(df["test_id"].isin(tri["test_id"])).dropna()["valid"]
+                    )
+                    else "red"
+                )
+                _patches.append(
+                    patches.Polygon(
+                        np.array(tri["geometry"]), facecolor=color, edgecolor="grey"
+                    )
+                )
+
+            collection = PatchCollection(_patches, match_original=True)
+            axes.add_collection(collection)
+
+        if show_voronoi_vertices:
+            points = [
+                (point.soil_properties.x, point.soil_properties.y)
+                for point in self.cpt_results_dict.values()
+            ]
+            vor = Voronoi(points)
+            voronoi_plot_2d(
+                vor,
+                show_vertices=False,
+                show_points=False,
+                ax=axes,
+                line_colors="black",
+                line_alpha=0.7,
+                line_width=0.1,
+                point_size=0.0,
+            )
+
+        # add the cpt names
+        axes.scatter(
+            df["x"],
+            df["y"],
+            c=["green" if val else "red" for val in df["valid"]],
+        )
+        for label, x, y in zip(df["test_id"], df["x"], df["y"]):
+            axes.annotate(label, xy=(x, y), xytext=(3, 3), textcoords="offset points")
+        axes.set_xlabel("X")
+        axes.set_ylabel("Y")
+        axes.ticklabel_format(useOffset=False)
+        fig.legend(
+            title="$R_{c;d;net}$ [kN]",
+            title_fontsize=18,
+            fontsize=15,
+            loc="lower right",
+            handles=[
+                patches.Patch(
+                    facecolor=color,
+                    label=label,
+                    alpha=0.9,
+                    linewidth=2,
+                    edgecolor="black",
+                )
+                for label, color in zip(
+                    [f">= {pile_load_uls}", f"< {pile_load_uls}"],
+                    ["green", "red"],
+                )
+            ],
+        )
+        axes.set_title(f"Pile tip level at: {pile_tip_level_nap} [m w.r.t NAP]")
+
+        return fig
```

### Comparing `py-pilecore-0.4.0/src/pypilecore/results/single_cpt_results.py` & `py_pilecore-0.4.1/src/pypilecore/results/single_cpt_results.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/results/soil_properties.py` & `py_pilecore-0.4.1/src/pypilecore/results/soil_properties.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/src/pypilecore/utils.py` & `py_pilecore-0.4.1/src/pypilecore/utils.py`

 * *Files identical despite different names*

### Comparing `py-pilecore-0.4.0/tests/test_input.py` & `py_pilecore-0.4.1/tests/test_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -734,7 +734,30 @@
             classify_tables={cpt.alias: mock_classify_response},
             groundwater_level_nap=-2.5,
             pile_type="A",
             specification="concrete",
             installation="1",
             pile_shape="rect",
         )
+
+def test_soil_load_is_always_float(
+    cpt: CPTData, mock_classify_response: dict
+) -> None:
+    """
+    Check that a soil-load value `float(0)` is passed even when the soil_load_sls
+    argument is None.
+    """
+
+    payload, _ = create_multi_cpt_payload(
+        pile_tip_levels_nap=[0, 1],
+        cptdata_objects=[cpt],
+        classify_tables={cpt.alias: mock_classify_response},
+        groundwater_level_nap=-2.5,
+        pile_type="concrete",
+        specification="1",
+        installation="A",
+        pile_shape="round",
+        diameter_base=0.3,
+        soil_load_sls=None,
+    )
+
+    assert np.isclose(payload.pop("soil_load"), 0.0)
```

