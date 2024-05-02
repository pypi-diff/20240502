# Comparing `tmp/pyvalem-2.6.tar.gz` & `tmp/pyvalem-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvalem-2.6.tar", last modified: Tue Apr 30 13:26:26 2024, max compression
+gzip compressed data, was "pyvalem-2.6.1.tar", last modified: Thu May  2 07:59:43 2024, max compression
```

## Comparing `pyvalem-2.6.tar` & `pyvalem-2.6.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.362577 pyvalem-2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-30 13:26:15.000000 pyvalem-2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-30 13:26:26.362577 pyvalem-2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-30 13:26:15.000000 pyvalem-2.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 13:26:15.000000 pyvalem-2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 13:26:26.362577 pyvalem-2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-30 13:26:15.000000 pyvalem-2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.354577 pyvalem-2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.354577 pyvalem-2.6/src/pyvalem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_data_atomic_weights.txt
--rw-r--r--   0 runner    (1001) docker     (127)   158055 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_data_isotope_masses.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_special_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/atom_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    23660 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/formula.py
--rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/stateful_species.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.358577 pyvalem-2.6/src/pyvalem/states/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/_base_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/_state_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/atomic_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/atomic_term_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/compound_LS_coupling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/diatomic_molecular_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/generic_excited_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/key_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/molecular_term_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/racah_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/rotational_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-30 13:26:15.000000 pyvalem-2.6/src/pyvalem/states/vibrational_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.362577 pyvalem-2.6/src/pyvalem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 13:26:26.000000 pyvalem-2.6/src/pyvalem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:26:26.362577 pyvalem-2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_atomic_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_atomic_term_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_atoms_isotopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_compound_LS_coupling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_diatomic_molecular_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_generic_excited_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_key_value_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_molecular_term_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_racah_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_rotational_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_stateful_species.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-30 13:26:15.000000 pyvalem-2.6/tests/test_vibrational_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:59:43.563296 pyvalem-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 07:59:31.000000 pyvalem-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-05-02 07:59:43.563296 pyvalem-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-02 07:59:31.000000 pyvalem-2.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 07:59:31.000000 pyvalem-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 07:59:43.563296 pyvalem-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-02 07:59:31.000000 pyvalem-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:59:43.551296 pyvalem-2.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:59:43.555296 pyvalem-2.6.1/src/pyvalem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/_data_atomic_weights.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   158055 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/_data_isotope_masses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/_special_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/atom_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23660 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/stateful_species.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:59:43.559296 pyvalem-2.6.1/src/pyvalem/states/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/_base_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/_state_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/atomic_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/atomic_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/compound_LS_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/diatomic_molecular_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/generic_excited_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/key_value_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/molecular_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/racah_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/rotational_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-02 07:59:31.000000 pyvalem-2.6.1/src/pyvalem/states/vibrational_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:59:43.563296 pyvalem-2.6.1/src/pyvalem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-05-02 07:59:43.000000 pyvalem-2.6.1/src/pyvalem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 07:59:43.000000 pyvalem-2.6.1/src/pyvalem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:59:43.000000 pyvalem-2.6.1/src/pyvalem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 07:59:43.000000 pyvalem-2.6.1/src/pyvalem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 07:59:43.000000 pyvalem-2.6.1/src/pyvalem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:59:43.563296 pyvalem-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_atomic_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_atomic_term_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_atoms_isotopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_compound_LS_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_diatomic_molecular_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_generic_excited_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_key_value_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_molecular_term_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_racah_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_rotational_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_stateful_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-02 07:59:31.000000 pyvalem-2.6.1/tests/test_vibrational_state.py
```

### Comparing `pyvalem-2.6/LICENSE` & `pyvalem-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/PKG-INFO` & `pyvalem-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalem
-Version: 2.6
+Version: 2.6.1
 Summary: A package for managing simple chemical species and states
 Home-page: https://github.com/xnx/pyvalem
 Author: Christian Hill
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/pyvalem/issues
 Keywords: chemistry,formula,species,state,reaction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvalem-2.6/README.rst` & `pyvalem-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/pyproject.toml` & `pyvalem-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/setup.py` & `pyvalem-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 root = Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (root / "README.rst").read_text(encoding="utf-8")
 
 setup(
     name="pyvalem",
-    version="2.6",
+    version="2.6.1",
     description="A package for managing simple chemical species and states",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/xnx/pyvalem",
     author="Christian Hill",
     author_email="ch.hill@iaea.org",
     classifiers=[
```

### Comparing `pyvalem-2.6/src/pyvalem/_data_atomic_weights.txt` & `pyvalem-2.6.1/src/pyvalem/_data_atomic_weights.txt`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/_data_isotope_masses.txt` & `pyvalem-2.6.1/src/pyvalem/_data_isotope_masses.txt`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/_special_cases.py` & `pyvalem-2.6.1/src/pyvalem/_special_cases.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/_utils.py` & `pyvalem-2.6.1/src/pyvalem/_utils.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/atom_data.py` & `pyvalem-2.6.1/src/pyvalem/atom_data.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/formula.py` & `pyvalem-2.6.1/src/pyvalem/formula.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/reaction.py` & `pyvalem-2.6.1/src/pyvalem/reaction.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/stateful_species.py` & `pyvalem-2.6.1/src/pyvalem/stateful_species.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/_base_state.py` & `pyvalem-2.6.1/src/pyvalem/states/_base_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/_state_parser.py` & `pyvalem-2.6.1/src/pyvalem/states/_state_parser.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/atomic_configuration.py` & `pyvalem-2.6.1/src/pyvalem/states/atomic_configuration.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/atomic_term_symbol.py` & `pyvalem-2.6.1/src/pyvalem/states/atomic_term_symbol.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/compound_LS_coupling.py` & `pyvalem-2.6.1/src/pyvalem/states/compound_LS_coupling.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/diatomic_molecular_configuration.py` & `pyvalem-2.6.1/src/pyvalem/states/diatomic_molecular_configuration.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/generic_excited_state.py` & `pyvalem-2.6.1/src/pyvalem/states/generic_excited_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/key_value_pair.py` & `pyvalem-2.6.1/src/pyvalem/states/key_value_pair.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/molecular_term_symbol.py` & `pyvalem-2.6.1/src/pyvalem/states/molecular_term_symbol.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/racah_symbol.py` & `pyvalem-2.6.1/src/pyvalem/states/racah_symbol.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/rotational_state.py` & `pyvalem-2.6.1/src/pyvalem/states/rotational_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem/states/vibrational_state.py` & `pyvalem-2.6.1/src/pyvalem/states/vibrational_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/src/pyvalem.egg-info/PKG-INFO` & `pyvalem-2.6.1/src/pyvalem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalem
-Version: 2.6
+Version: 2.6.1
 Summary: A package for managing simple chemical species and states
 Home-page: https://github.com/xnx/pyvalem
 Author: Christian Hill
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/pyvalem/issues
 Keywords: chemistry,formula,species,state,reaction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvalem-2.6/src/pyvalem.egg-info/SOURCES.txt` & `pyvalem-2.6.1/src/pyvalem.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 tests/test_atomic_configurations.py
 tests/test_atomic_term_symbols.py
 tests/test_atoms_isotopes.py
 tests/test_compound_LS_coupling.py
 tests/test_diatomic_molecular_configurations.py
 tests/test_formula.py
 tests/test_generic_excited_state.py
+tests/test_imports.py
 tests/test_key_value_pairs.py
 tests/test_molecular_term_symbol.py
 tests/test_racah_symbols.py
 tests/test_reaction.py
 tests/test_rotational_state.py
 tests/test_stateful_species.py
 tests/test_vibrational_state.py
```

### Comparing `pyvalem-2.6/tests/test_aliases.py` & `pyvalem-2.6.1/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_atomic_configurations.py` & `pyvalem-2.6.1/tests/test_atomic_configurations.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_atomic_term_symbols.py` & `pyvalem-2.6.1/tests/test_atomic_term_symbols.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_atoms_isotopes.py` & `pyvalem-2.6.1/tests/test_atoms_isotopes.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_compound_LS_coupling.py` & `pyvalem-2.6.1/tests/test_compound_LS_coupling.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_diatomic_molecular_configurations.py` & `pyvalem-2.6.1/tests/test_diatomic_molecular_configurations.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_formula.py` & `pyvalem-2.6.1/tests/test_formula.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_generic_excited_state.py` & `pyvalem-2.6.1/tests/test_generic_excited_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_key_value_pairs.py` & `pyvalem-2.6.1/tests/test_key_value_pairs.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_molecular_term_symbol.py` & `pyvalem-2.6.1/tests/test_molecular_term_symbol.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_racah_symbols.py` & `pyvalem-2.6.1/tests/test_racah_symbols.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_reaction.py` & `pyvalem-2.6.1/tests/test_reaction.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_rotational_state.py` & `pyvalem-2.6.1/tests/test_rotational_state.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_stateful_species.py` & `pyvalem-2.6.1/tests/test_stateful_species.py`

 * *Files identical despite different names*

### Comparing `pyvalem-2.6/tests/test_vibrational_state.py` & `pyvalem-2.6.1/tests/test_vibrational_state.py`

 * *Files identical despite different names*

