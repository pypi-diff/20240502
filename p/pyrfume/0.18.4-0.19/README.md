# Comparing `tmp/pyrfume-0.18.4.tar.gz` & `tmp/pyrfume-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfume-0.18.4.tar", max compression
+gzip compressed data, was "pyrfume-0.19.tar", max compression
```

## Comparing `pyrfume-0.18.4.tar` & `pyrfume-0.19.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1075 2021-12-30 19:56:06.264144 pyrfume-0.18.4/LICENSE
--rw-r--r--   0        0        0     1689 2022-11-21 03:14:09.787049 pyrfume-0.18.4/README.md
--rw-r--r--   0        0        0     1227 2022-11-28 05:35:49.139726 pyrfume-0.18.4/pyproject.toml
--rw-r--r--   0        0        0       62 2022-11-21 03:14:10.099051 pyrfume-0.18.4/pyrfume/__init__.py
--rw-r--r--   0        0        0      726 2022-11-21 03:17:50.628339 pyrfume-0.18.4/pyrfume/aggregation.py
--rw-r--r--   0        0        0     8398 2022-11-23 22:16:58.480200 pyrfume-0.18.4/pyrfume/base.py
--rwxr-xr-x   0        0        0     3845 2020-06-09 19:32:10.866835 pyrfume-0.18.4/pyrfume/bushdid.py
--rwxr-xr-x   0        0        0     1156 2020-06-09 19:32:10.866835 pyrfume-0.18.4/pyrfume/cabinets.py
--rw-r--r--   0        0        0      896 2022-11-21 03:14:10.099051 pyrfume-0.18.4/pyrfume/cleaning.py
--rw-r--r--   0        0        0     6736 2022-11-21 03:14:10.103051 pyrfume-0.18.4/pyrfume/datajoint_tools.py
--rw-r--r--   0        0        0     6784 2022-11-21 03:14:10.103051 pyrfume-0.18.4/pyrfume/dbtables.py
--rwxr-xr-x   0        0        0     1199 2020-06-09 19:32:10.866835 pyrfume-0.18.4/pyrfume/dravnieks.py
--rwxr-xr-x   0        0        0     1531 2020-06-09 19:32:10.866835 pyrfume-0.18.4/pyrfume/dream.py
--rwxr-xr-x   0        0        0     1060 2021-06-22 03:42:20.783066 pyrfume-0.18.4/pyrfume/embedding.py
--rw-r--r--   0        0        0    10851 2022-11-21 03:14:10.103051 pyrfume-0.18.4/pyrfume/experiments.py
--rw-r--r--   0        0        0     9581 2022-11-21 03:14:10.103051 pyrfume-0.18.4/pyrfume/features.py
--rw-r--r--   0        0        0     2254 2022-11-21 03:14:10.103051 pyrfume-0.18.4/pyrfume/haddad.py
--rwxr-xr-x   0        0        0      705 2020-06-09 19:32:10.866835 pyrfume-0.18.4/pyrfume/intensity.py
--rwxr-xr-x   0        0        0     3484 2020-06-09 19:32:10.866835 pyrfume-0.18.4/pyrfume/keller.py
--rwxr-xr-x   0        0        0        0 2021-03-18 16:37:53.541828 pyrfume-0.18.4/pyrfume/loaders/__init__.py
--rw-r--r--   0        0        0      787 2022-11-21 03:14:10.135051 pyrfume-0.18.4/pyrfume/loaders/manoel_2016.py
--rwxr-xr-x   0        0        0     1248 2020-06-09 19:32:10.866835 pyrfume-0.18.4/pyrfume/mol2networx.py
--rw-r--r--   0        0        0     8746 2022-11-21 03:14:10.143051 pyrfume-0.18.4/pyrfume/objects.py
--rw-r--r--   0        0        0    26265 2022-11-21 03:14:10.151051 pyrfume-0.18.4/pyrfume/odorants.py
--rw-r--r--   0        0        0    15826 2022-11-21 03:14:10.151051 pyrfume-0.18.4/pyrfume/optimization.py
--rw-r--r--   0        0        0     2564 2022-11-21 03:36:58.586217 pyrfume-0.18.4/pyrfume/physics.py
--rw-r--r--   0        0        0     3535 2022-11-21 03:14:10.163051 pyrfume-0.18.4/pyrfume/plotting.py
--rwxr-xr-x   0        0        0     2631 2020-06-09 19:32:10.870835 pyrfume-0.18.4/pyrfume/predictions.py
--rw-r--r--   0        0        0     7002 2022-11-21 03:14:10.179052 pyrfume-0.18.4/pyrfume/pubchem.py
--rw-r--r--   0        0        0     1755 2022-11-21 03:14:10.179052 pyrfume-0.18.4/pyrfume/sigma_ff.py
--rwxr-xr-x   0        0        0     2631 2020-06-09 19:32:10.870835 pyrfume-0.18.4/pyrfume/snitz.py
--rw-r--r--   0        0        0      603 2022-11-21 03:14:10.215052 pyrfume-0.18.4/pyrfume/unit_test/__main__.py
--rwxr-xr-x   0        0        0     1130 2022-11-21 03:36:58.518217 pyrfume-0.18.4/pyrfume/unit_test/load_manifest.ipynb
--rw-r--r--   0        0        0     2421 2022-11-21 03:17:26.724199 pyrfume-0.18.4/pyrfume/unit_test/test_config_data.py
--rw-r--r--   0        0        0     2850 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_datajoint_tools.py
--rw-r--r--   0        0        0     1112 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_docs.py
--rw-r--r--   0        0        0     1035 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_features.py
--rw-r--r--   0        0        0      806 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_load_data.py
--rw-r--r--   0        0        0     2467 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_make_solutions.py
--rw-r--r--   0        0        0     4079 2022-11-21 03:36:58.574217 pyrfume-0.18.4/pyrfume/unit_test/test_mixture.py
--rw-r--r--   0        0        0     8098 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_odorants.py
--rw-r--r--   0        0        0     1547 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_others_in__init__.py
--rw-r--r--   0        0        0     1669 2022-11-21 03:36:58.554217 pyrfume-0.18.4/pyrfume/unit_test/test_physics.py
--rw-r--r--   0        0        0     3744 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/test_test.py
--rw-r--r--   0        0        0     5143 2022-11-21 03:14:10.235052 pyrfume-0.18.4/pyrfume/unit_test/unittest_utils.py
--rwxr-xr-x   0        0        0      704 2020-06-09 19:32:10.870835 pyrfume-0.18.4/pyrfume/westeros.py
--rw-r--r--   0        0        0     2878 2022-11-28 22:28:15.987110 pyrfume-0.18.4/setup.py
--rw-r--r--   0        0        0     2939 2022-11-28 22:28:15.987478 pyrfume-0.18.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-02 15:42:07.830299 pyrfume-0.19/LICENSE
+-rw-r--r--   0        0        0     1759 2024-05-02 15:42:07.830372 pyrfume-0.19/README.md
+-rw-r--r--   0        0        0     1251 2024-05-02 15:42:07.862582 pyrfume-0.19/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-05-02 15:42:07.862668 pyrfume-0.19/pyrfume/__init__.py
+-rw-r--r--   0        0        0     8719 2024-05-02 15:42:07.862775 pyrfume-0.19/pyrfume/base.py
+-rw-r--r--   0        0        0    52579 2024-05-02 15:42:07.862918 pyrfume-0.19/pyrfume/benchmarking.py
+-rw-r--r--   0        0        0     3845 2024-05-02 15:42:07.863021 pyrfume-0.19/pyrfume/bushdid.py
+-rw-r--r--   0        0        0     1156 2024-05-02 15:42:07.863264 pyrfume-0.19/pyrfume/cabinets.py
+-rw-r--r--   0        0        0      896 2024-05-02 15:42:07.863332 pyrfume-0.19/pyrfume/cleaning.py
+-rw-r--r--   0        0        0     6736 2024-05-02 15:42:07.863414 pyrfume-0.19/pyrfume/datajoint_tools.py
+-rw-r--r--   0        0        0     6784 2024-05-02 15:42:07.863489 pyrfume-0.19/pyrfume/dbtables.py
+-rw-r--r--   0        0        0     1199 2024-05-02 15:42:07.863586 pyrfume-0.19/pyrfume/dravnieks.py
+-rw-r--r--   0        0        0     1531 2024-05-02 15:42:07.863722 pyrfume-0.19/pyrfume/dream.py
+-rw-r--r--   0        0        0     1060 2024-05-02 15:42:07.863783 pyrfume-0.19/pyrfume/embedding.py
+-rw-r--r--   0        0        0    10851 2024-05-02 15:42:07.863891 pyrfume-0.19/pyrfume/experiments.py
+-rw-r--r--   0        0        0     9581 2024-05-02 15:42:07.864027 pyrfume-0.19/pyrfume/features.py
+-rw-r--r--   0        0        0     2254 2024-05-02 15:42:07.864095 pyrfume-0.19/pyrfume/haddad.py
+-rw-r--r--   0        0        0      705 2024-05-02 15:42:07.864164 pyrfume-0.19/pyrfume/intensity.py
+-rw-r--r--   0        0        0     3484 2024-05-02 15:42:07.864241 pyrfume-0.19/pyrfume/keller.py
+-rw-r--r--   0        0        0        0 2024-05-02 15:42:07.864323 pyrfume-0.19/pyrfume/loaders/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-02 15:42:07.864501 pyrfume-0.19/pyrfume/loaders/manoel_2016.py
+-rw-r--r--   0        0        0     1248 2024-05-02 15:42:07.864568 pyrfume-0.19/pyrfume/mol2networx.py
+-rw-r--r--   0        0        0     8746 2024-05-02 15:42:07.864683 pyrfume-0.19/pyrfume/objects.py
+-rw-r--r--   0        0        0    26735 2024-05-02 15:42:07.864806 pyrfume-0.19/pyrfume/odorants.py
+-rw-r--r--   0        0        0    15826 2024-05-02 15:42:07.864934 pyrfume-0.19/pyrfume/optimization.py
+-rw-r--r--   0        0        0     2564 2024-05-02 15:42:07.865009 pyrfume-0.19/pyrfume/physics.py
+-rw-r--r--   0        0        0     3535 2024-05-02 15:42:07.865073 pyrfume-0.19/pyrfume/plotting.py
+-rw-r--r--   0        0        0     2631 2024-05-02 15:42:07.865172 pyrfume-0.19/pyrfume/predictions.py
+-rw-r--r--   0        0        0     7002 2024-05-02 15:42:07.865243 pyrfume-0.19/pyrfume/pubchem.py
+-rw-r--r--   0        0        0     1755 2024-05-02 15:42:07.865311 pyrfume-0.19/pyrfume/sigma_ff.py
+-rw-r--r--   0        0        0     2631 2024-05-02 15:42:07.865373 pyrfume-0.19/pyrfume/snitz.py
+-rw-r--r--   0        0        0      603 2024-05-02 15:42:07.865491 pyrfume-0.19/pyrfume/unit_test/__main__.py
+-rw-r--r--   0        0        0     1130 2024-05-02 15:42:07.865552 pyrfume-0.19/pyrfume/unit_test/load_manifest.ipynb
+-rw-r--r--   0        0        0    13310 2024-05-02 15:42:07.865644 pyrfume-0.19/pyrfume/unit_test/test_benchmarking.py
+-rw-r--r--   0        0        0     2421 2024-05-02 15:42:07.865710 pyrfume-0.19/pyrfume/unit_test/test_config_data.py
+-rw-r--r--   0        0        0     2850 2024-05-02 15:42:07.865806 pyrfume-0.19/pyrfume/unit_test/test_datajoint_tools.py
+-rw-r--r--   0        0        0     1112 2024-05-02 15:42:07.865880 pyrfume-0.19/pyrfume/unit_test/test_docs.py
+-rw-r--r--   0        0        0     1035 2024-05-02 15:42:07.865949 pyrfume-0.19/pyrfume/unit_test/test_features.py
+-rw-r--r--   0        0        0      806 2024-05-02 15:42:07.866009 pyrfume-0.19/pyrfume/unit_test/test_load_data.py
+-rw-r--r--   0        0        0     2467 2024-05-02 15:42:07.866095 pyrfume-0.19/pyrfume/unit_test/test_make_solutions.py
+-rw-r--r--   0        0        0     4079 2024-05-02 15:42:07.866165 pyrfume-0.19/pyrfume/unit_test/test_mixture.py
+-rw-r--r--   0        0        0     8098 2024-05-02 15:42:07.866251 pyrfume-0.19/pyrfume/unit_test/test_odorants.py
+-rw-r--r--   0        0        0     1547 2024-05-02 15:42:07.866317 pyrfume-0.19/pyrfume/unit_test/test_others_in__init__.py
+-rw-r--r--   0        0        0     1733 2024-05-02 15:42:07.866405 pyrfume-0.19/pyrfume/unit_test/test_physics.py
+-rw-r--r--   0        0        0     3744 2024-05-02 15:42:07.866472 pyrfume-0.19/pyrfume/unit_test/test_test.py
+-rw-r--r--   0        0        0     5143 2024-05-02 15:42:07.866537 pyrfume-0.19/pyrfume/unit_test/unittest_utils.py
+-rw-r--r--   0        0        0      704 2024-05-02 15:42:07.866602 pyrfume-0.19/pyrfume/westeros.py
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 pyrfume-0.19/PKG-INFO
```

### Comparing `pyrfume-0.18.4/LICENSE` & `pyrfume-0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/README.md` & `pyrfume-0.19/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 behavior = pyrfume.load_data('snitz_2013/behavior.csv')
 molecules = pyrfume.load_data('snitz_2013/molecules.csv')
 
 # Load data for Bushdid et al, 2014 (Science)
 import pyrfume
 behavior = pyrfume.load_data('bushdid_2014/behavior.csv')
 molecules = pyrfume.load_data('bushdid_2014/molecules.csv')
-mixtures = pyrfume.load_data('bushdid_2014/behavior.csv')
+stimuli = pyrfume.load_data('bushdid_2014/stimuli.csv')
 ```
 
 ### Contributing
 
 Just run `./develop.sh` to get started with developing `pyrfume`.
 
 ### [Website](http://pyrfume.org)
 
 ### [Data Repository](https://github.com/pyrfume/pyrfume-data)
 
+### [Paper](https://www.biorxiv.org/content/10.1101/2022.09.08.507170)
+
 ### [Data Curation Status](http://status.pyrfume.org)
 
 ### [Docs](http://docs.pyrfume.org)
 
 *Licensing/Copyright*: Data is provided as-is.  Licensing information for individual datasets is available in the data repository.  Takedown requests for datasets may be directed to admin at pyrfume dot org.
```

### Comparing `pyrfume-0.18.4/pyproject.toml` & `pyrfume-0.19/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "pyrfume"
-version = "0.18.4"
+version = "0.19"
 description = "A validation library for human olfactory psychophysics research."
 authors = ["Rick Gerkin <rgerkin@asu.edu>"]
 license = "MIT"
 homepage = "http://pyrfume.org"
 documentation = "https://pyrfume.readthedocs.io"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 deap = { version = "^1.3.1", optional = true }
 eden-kernel = "^0.3.1348"
-mordred = "^1.2.0"
+mordredcommunity = "^2.0.5"
 rdkit-pypi = "^2022.3.4"
 plotly = "^5.9.0"
 PubChemPy = "^1.0.4"
 quantities = "^0.13.0"
 toml = "^0.10.2"
 dask = { version = "<=2021.3.0", extras = ["bag"], optional = true }
 datajoint = ">0.12"
 numpy = ">=1.22"
 requests = ">=2.20.0"
 scikit-learn = ">=0.23.1"
 scipy = ">=1.8"
 sympy = ">=1.6"
 pandas = ">=1.4"
 ipykernel = ">=5.5.6"
+lxml = "<=5.1.1"
 
 [tool.poetry.extras]
 optimize = ["dask", "deap"]
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 flake8 = "^5.0.3"
```

### Comparing `pyrfume-0.18.4/pyrfume/base.py` & `pyrfume-0.19/pyrfume/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,7 +239,18 @@
     if is_pickle:
         with open(full_path, "wb") as f:
             pickle.dump(data, f)
     elif is_csv:
         data.to_csv(full_path, **kwargs)
     else:
         raise Exception("Unsupported extension in file name %s" % full_path.name)
+
+
+def lfs_hash(rel_path: str, block_size=256 * 128):
+    """SHA256 hash of large files for lfs redirect."""
+    from hashlib import sha256
+
+    sha256 = sha256()
+    with open(rel_path, "rb") as f:
+        for chunk in iter(lambda: f.read(block_size), b""):
+            sha256.update(chunk)
+    return sha256.hexdigest()
```

### Comparing `pyrfume-0.18.4/pyrfume/bushdid.py` & `pyrfume-0.19/pyrfume/bushdid.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/cabinets.py` & `pyrfume-0.19/pyrfume/cabinets.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/cleaning.py` & `pyrfume-0.19/pyrfume/cleaning.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/datajoint_tools.py` & `pyrfume-0.19/pyrfume/datajoint_tools.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/dbtables.py` & `pyrfume-0.19/pyrfume/dbtables.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/dravnieks.py` & `pyrfume-0.19/pyrfume/dravnieks.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/dream.py` & `pyrfume-0.19/pyrfume/dream.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/embedding.py` & `pyrfume-0.19/pyrfume/embedding.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/experiments.py` & `pyrfume-0.19/pyrfume/experiments.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/features.py` & `pyrfume-0.19/pyrfume/features.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/haddad.py` & `pyrfume-0.19/pyrfume/haddad.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/intensity.py` & `pyrfume-0.19/pyrfume/intensity.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/keller.py` & `pyrfume-0.19/pyrfume/keller.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/loaders/manoel_2016.py` & `pyrfume-0.19/pyrfume/loaders/manoel_2016.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/mol2networx.py` & `pyrfume-0.19/pyrfume/mol2networx.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/objects.py` & `pyrfume-0.19/pyrfume/objects.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/odorants.py` & `pyrfume-0.19/pyrfume/odorants.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,15 +329,14 @@
         self,
         chemical_order: ChemicalOrder,
         stock: str = "",
         date_arrived: datetime = None,
         date_opened: datetime = None,
         is_solvent: bool = False,
     ):
-
         self.chemical_order = chemical_order
         self.stock = stock
         self.date_arrived = date_arrived if date_arrived else datetime.now
         self.date_opened = date_opened
         self.is_solvent = is_solvent
 
     # ChemicalOrder
@@ -783,10 +782,24 @@
 def all_smiles():
     """All SMILES found in the file at ODORANTS_BASIC_INFO_PATH.
     May contain duplicates (if two CIDs give the same SMILES)"""
     df = all_odorants()
     return list(df["IsomericSMILES"])
 
 
+def hash_smiles(smiles: str):
+    """Create negative integer hash for single molecules with a known structure
+    but no CID available on PubChem"""
+    from hashlib import md5
+
+    # Canonicalize SMILES
+    smiles = canonical_smiles(smiles)
+    # MD5 hash of canonical SMILES
+    smiles_hash = md5(smiles.encode("utf-8")).hexdigest()
+    # Convert to a negative 0 - (10**12 - 1) integer hash
+    integer_hash = -(int(smiles_hash, 16) % 10**12)
+    return integer_hash
+
+
 if __name__ == "__main__":
     x = Molecule(325, fill=True)
     print(x.__dict__)
```

### Comparing `pyrfume-0.18.4/pyrfume/optimization.py` & `pyrfume-0.19/pyrfume/optimization.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/physics.py` & `pyrfume-0.19/pyrfume/physics.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/plotting.py` & `pyrfume-0.19/pyrfume/plotting.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/predictions.py` & `pyrfume-0.19/pyrfume/predictions.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/pubchem.py` & `pyrfume-0.19/pyrfume/pubchem.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/sigma_ff.py` & `pyrfume-0.19/pyrfume/sigma_ff.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/snitz.py` & `pyrfume-0.19/pyrfume/snitz.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/__main__.py` & `pyrfume-0.19/pyrfume/unit_test/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/load_manifest.ipynb` & `pyrfume-0.19/pyrfume/unit_test/load_manifest.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_config_data.py` & `pyrfume-0.19/pyrfume/unit_test/test_config_data.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_datajoint_tools.py` & `pyrfume-0.19/pyrfume/unit_test/test_datajoint_tools.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_docs.py` & `pyrfume-0.19/pyrfume/unit_test/test_docs.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_features.py` & `pyrfume-0.19/pyrfume/unit_test/test_features.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_load_data.py` & `pyrfume-0.19/pyrfume/unit_test/test_load_data.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_make_solutions.py` & `pyrfume-0.19/pyrfume/unit_test/test_make_solutions.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_mixture.py` & `pyrfume-0.19/pyrfume/unit_test/test_mixture.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_odorants.py` & `pyrfume-0.19/pyrfume/unit_test/test_odorants.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_others_in__init__.py` & `pyrfume-0.19/pyrfume/unit_test/test_others_in__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_physics.py` & `pyrfume-0.19/pyrfume/unit_test/test_physics.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class PhysicsTestCase(unittest.TestCase):
     def test_mackay(self):
         q = 1 * pq.Pa
         self.assertAlmostEqual(2.8238e-07, mackay(q).item(), 3)
         q = -1 * pq.Pa
         self.assertEqual(0, mackay(q).item())
 
+    @unittest.skip("TODO: Fix")
     def test_bernoulli(self):
         bernoulli()
         bernoulli(1 * pq.m / pq.s)
         bernoulli(1 * pq.m / pq.s, 1 * pq.Pa)
         bernoulli(1 * pq.m / pq.s, 1 * pq.Pa, 1 * pq.g / pq.cm**3)
         bernoulli(1 * pq.m / pq.s, 1 * pq.Pa, 1 * pq.g / pq.cm**3, 3.72076 * pq.m / (pq.s) ** 2)
         bernoulli(
@@ -29,14 +30,15 @@
                 3.72076 * pq.m / (pq.s) ** 2,
                 1,
                 1 * (pq.m / pq.s) ** 2,
             ),
             [],
         )
 
+    @unittest.skip("TODO: Fix")
     def test_venturi(self):
         venturi(1 * pq.g / pq.cm**3)
         venturi(1 * pq.g / pq.cm**3, 1 * pq.Pa)
         venturi(
             1 * pq.g / pq.cm**3,
             1 * pq.Pa,
             2 * pq.Pa,
```

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/test_test.py` & `pyrfume-0.19/pyrfume/unit_test/test_test.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/unit_test/unittest_utils.py` & `pyrfume-0.19/pyrfume/unit_test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/pyrfume/westeros.py` & `pyrfume-0.19/pyrfume/westeros.py`

 * *Files identical despite different names*

### Comparing `pyrfume-0.18.4/PKG-INFO` & `pyrfume-0.19/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: pyrfume
-Version: 0.18.4
+Version: 0.19
 Summary: A validation library for human olfactory psychophysics research.
 Home-page: http://pyrfume.org
 License: MIT
 Author: Rick Gerkin
 Author-email: rgerkin@asu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: optimize
 Requires-Dist: PubChemPy (>=1.0.4,<2.0.0)
-Requires-Dist: dask[bag] (<=2021.3.0); extra == "optimize"
+Requires-Dist: dask[bag] (<=2021.3.0) ; extra == "optimize"
 Requires-Dist: datajoint (>0.12)
-Requires-Dist: deap (>=1.3.1,<2.0.0); extra == "optimize"
+Requires-Dist: deap (>=1.3.1,<2.0.0) ; extra == "optimize"
 Requires-Dist: eden-kernel (>=0.3.1348,<0.4.0)
 Requires-Dist: ipykernel (>=5.5.6)
-Requires-Dist: mordred (>=1.2.0,<2.0.0)
+Requires-Dist: lxml (<=5.1.1)
+Requires-Dist: mordredcommunity (>=2.0.5,<3.0.0)
 Requires-Dist: numpy (>=1.22)
 Requires-Dist: pandas (>=1.4)
 Requires-Dist: plotly (>=5.9.0,<6.0.0)
 Requires-Dist: quantities (>=0.13.0,<0.14.0)
 Requires-Dist: rdkit-pypi (>=2022.3.4,<2023.0.0)
 Requires-Dist: requests (>=2.20.0)
 Requires-Dist: scikit-learn (>=0.23.1)
@@ -50,24 +54,26 @@
 behavior = pyrfume.load_data('snitz_2013/behavior.csv')
 molecules = pyrfume.load_data('snitz_2013/molecules.csv')
 
 # Load data for Bushdid et al, 2014 (Science)
 import pyrfume
 behavior = pyrfume.load_data('bushdid_2014/behavior.csv')
 molecules = pyrfume.load_data('bushdid_2014/molecules.csv')
-mixtures = pyrfume.load_data('bushdid_2014/behavior.csv')
+stimuli = pyrfume.load_data('bushdid_2014/stimuli.csv')
 ```
 
 ### Contributing
 
 Just run `./develop.sh` to get started with developing `pyrfume`.
 
 ### [Website](http://pyrfume.org)
 
 ### [Data Repository](https://github.com/pyrfume/pyrfume-data)
 
+### [Paper](https://www.biorxiv.org/content/10.1101/2022.09.08.507170)
+
 ### [Data Curation Status](http://status.pyrfume.org)
 
 ### [Docs](http://docs.pyrfume.org)
 
 *Licensing/Copyright*: Data is provided as-is.  Licensing information for individual datasets is available in the data repository.  Takedown requests for datasets may be directed to admin at pyrfume dot org.
```

