# Comparing `tmp/progres-0.2.2.tar.gz` & `tmp/progres-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progres-0.2.2.tar", last modified: Tue Apr 23 11:38:23 2024, max compression
+gzip compressed data, was "progres-0.2.3.tar", last modified: Thu May  2 11:39:10 2024, max compression
```

## Comparing `progres-0.2.2.tar` & `progres-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)     3635 2024-04-15 18:40:30.000000 progres-0.2.2/LICENSE
--rw-r--r--   0 jgreener  (1000) jgreener  (1000)    13001 2024-04-23 11:38:23.221322 progres-0.2.2/PKG-INFO
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    12350 2024-04-23 11:31:27.000000 progres-0.2.2/README.md
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/bin/
--rwxrwxr-x   0 jgreener  (1000) jgreener  (1000)     4009 2024-04-18 10:02:07.000000 progres-0.2.2/bin/progres
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/progres/
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       23 2022-11-16 16:19:38.000000 progres-0.2.2/progres/__init__.py
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    24079 2024-04-23 11:22:48.000000 progres-0.2.2/progres/progres.py
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-23 11:38:23.221322 progres-0.2.2/progres.egg-info/
--rw-r--r--   0 jgreener  (1000) jgreener  (1000)    13001 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/PKG-INFO
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      231 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/SOURCES.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        1 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/dependency_links.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       29 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/requires.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        8 2024-04-23 11:38:23.000000 progres-0.2.2/progres.egg-info/top_level.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       38 2024-04-23 11:38:23.221322 progres-0.2.2/setup.cfg
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      917 2024-04-23 11:31:43.000000 progres-0.2.2/setup.py
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-05-02 11:39:10.550449 progres-0.2.3/
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)     3635 2024-04-15 18:40:30.000000 progres-0.2.3/LICENSE
+-rw-r--r--   0 jgreener  (1000) jgreener  (1000)    13001 2024-05-02 11:39:10.550449 progres-0.2.3/PKG-INFO
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    12350 2024-05-02 11:37:59.000000 progres-0.2.3/README.md
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-05-02 11:39:10.550449 progres-0.2.3/bin/
+-rwxrwxr-x   0 jgreener  (1000) jgreener  (1000)     4009 2024-04-18 10:02:07.000000 progres-0.2.3/bin/progres
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-05-02 11:39:10.550449 progres-0.2.3/progres/
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       23 2022-11-16 16:19:38.000000 progres-0.2.3/progres/__init__.py
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    24667 2024-04-29 15:08:04.000000 progres-0.2.3/progres/progres.py
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-05-02 11:39:10.550449 progres-0.2.3/progres.egg-info/
+-rw-r--r--   0 jgreener  (1000) jgreener  (1000)    13001 2024-05-02 11:39:10.000000 progres-0.2.3/progres.egg-info/PKG-INFO
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      231 2024-05-02 11:39:10.000000 progres-0.2.3/progres.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        1 2024-05-02 11:39:10.000000 progres-0.2.3/progres.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       29 2024-05-02 11:39:10.000000 progres-0.2.3/progres.egg-info/requires.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        8 2024-05-02 11:39:10.000000 progres-0.2.3/progres.egg-info/top_level.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       38 2024-05-02 11:39:10.550449 progres-0.2.3/setup.cfg
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      917 2024-05-02 11:37:53.000000 progres-0.2.3/setup.py
```

### Comparing `progres-0.2.2/LICENSE` & `progres-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `progres-0.2.2/PKG-INFO` & `progres-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progres
-Version: 0.2.2
+Version: 0.2.3
 Summary: Fast protein structure searching using structure graph embeddings
 Home-page: https://github.com/greener-group/progres
 Author: Joe G Greener
 Author-email: jgreener@mrc-lmb.cam.ac.uk
 License: MIT
 Keywords: protein structure search graph embedding
 Classifier: Programming Language :: Python :: 3
@@ -62,15 +62,15 @@
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.2
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.3
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
```

### Comparing `progres-0.2.2/README.md` & `progres-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.2
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.3
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
```

### Comparing `progres-0.2.2/bin/progres` & `progres-0.2.3/bin/progres`

 * *Files identical despite different names*

### Comparing `progres-0.2.2/progres/progres.py` & `progres-0.2.3/progres/progres.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,33 +378,45 @@
 
     dirs_that_should_exist = [data_dir, trained_model_dir, database_dir]
     for dir in dirs_that_should_exist:
         os.makedirs(dir, exist_ok=True)    
 
     printed = False
     for fp, url in zip(fps, urls):
-        if not os.path.isfile(fp):
+        if not os.path.isfile(fp + ".okay") or not os.path.isfile(fp):
             if fp.endswith("afted.index"):
                 print("Downloading afted data as first time setup (~33 GB) to ", database_dir,
                       ", internet connection required, this may take a while",
                       sep="", file=sys.stderr)
                 printed = True
             if not printed:
                 print("Downloading data as first time setup (~220 MB) to ", data_dir,
                       ", internet connection required, this can take a few minutes",
                       sep="", file=sys.stderr)
                 printed = True
             try:
+                if os.path.isfile(fp):
+                    print("Removing ", fp,
+                          ", which may be an incomplete download, and downloading again",
+                          sep="", file=sys.stderr)
+                    os.remove(fp)
                 request.urlretrieve(url, fp)
-                if not fp.endswith("afted.index"):
+                # Check download seems okay and indicate this with a file
+                if fp.endswith("afted.index"):
+                    import faiss
+                    faiss.read_index(fp)
+                else:
                     d = torch.load(fp, map_location="cpu")
                     if fp == trained_model_fp:
                         assert "model" in d
                     else:
                         assert "notes" in d
+                        assert len(d["notes"]) > 10
+                with open(fp + ".okay", "w") as of:
+                    pass
             except:
                 if os.path.isfile(fp):
                     os.remove(fp)
                 print("Failed to download from", url, "and save to", fp, file=sys.stderr)
                 print("Exiting", file=sys.stderr)
                 sys.exit(1)
```

### Comparing `progres-0.2.2/progres.egg-info/PKG-INFO` & `progres-0.2.3/progres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progres
-Version: 0.2.2
+Version: 0.2.3
 Summary: Fast protein structure searching using structure graph embeddings
 Home-page: https://github.com/greener-group/progres
 Author: Joe G Greener
 Author-email: jgreener@mrc-lmb.cam.ac.uk
 License: MIT
 Keywords: protein structure search graph embedding
 Classifier: Programming Language :: Python :: 3
@@ -62,15 +62,15 @@
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.2
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.3
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
```

### Comparing `progres-0.2.2/setup.py` & `progres-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="progres",
-    version="0.2.2",
+    version="0.2.3",
     author="Joe G Greener",
     author_email="jgreener@mrc-lmb.cam.ac.uk",
     description="Fast protein structure searching using structure graph embeddings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/greener-group/progres",
     packages=setuptools.find_packages(),
```

