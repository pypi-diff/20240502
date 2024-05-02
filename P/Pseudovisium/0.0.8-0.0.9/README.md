# Comparing `tmp/Pseudovisium-0.0.8.tar.gz` & `tmp/Pseudovisium-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pseudovisium-0.0.8.tar", last modified: Mon Apr 29 19:56:51 2024, max compression
+gzip compressed data, was "Pseudovisium-0.0.9.tar", last modified: Thu May  2 07:18:41 2024, max compression
```

## Comparing `Pseudovisium-0.0.8.tar` & `Pseudovisium-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-29 19:56:51.592193 Pseudovisium-0.0.8/
--rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.8/LICENSE
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-29 19:56:51.591939 Pseudovisium-0.0.8/PKG-INFO
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-29 19:56:51.590159 Pseudovisium-0.0.8/Pseudovisium/
--rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.8/Pseudovisium/__init__.py
--rw-r--r--   0 k23030440   (504) staff       (20)    58663 2024-04-29 10:55:34.000000 Pseudovisium-0.0.8/Pseudovisium/pseudovisium_generate.py
--rw-r--r--   0 k23030440   (504) staff       (20)    14501 2024-04-23 21:00:08.000000 Pseudovisium-0.0.8/Pseudovisium/pseudovisium_merge.py
--rw-r--r--   0 k23030440   (504) staff       (20)    73864 2024-04-29 19:55:26.000000 Pseudovisium-0.0.8/Pseudovisium/pseudovisium_qc.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-29 19:56:51.591600 Pseudovisium-0.0.8/Pseudovisium.egg-info/
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-29 19:56:51.000000 Pseudovisium-0.0.8/Pseudovisium.egg-info/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-29 19:56:51.000000 Pseudovisium-0.0.8/Pseudovisium.egg-info/SOURCES.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-29 19:56:51.000000 Pseudovisium-0.0.8/Pseudovisium.egg-info/dependency_links.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-29 19:56:51.000000 Pseudovisium-0.0.8/Pseudovisium.egg-info/requires.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-29 19:56:51.000000 Pseudovisium-0.0.8/Pseudovisium.egg-info/top_level.txt
--rw-r--r--   0 k23030440   (504) staff       (20)     3637 2024-04-26 08:21:23.000000 Pseudovisium-0.0.8/README.md
--rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-29 19:56:51.592242 Pseudovisium-0.0.8/setup.cfg
--rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-29 19:56:25.000000 Pseudovisium-0.0.8/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-02 07:18:41.400373 Pseudovisium-0.0.9/
+-rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.9/LICENSE
+-rw-r--r--   0 k23030440   (504) staff       (20)      846 2024-05-02 07:18:41.400046 Pseudovisium-0.0.9/PKG-INFO
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-02 07:18:41.398154 Pseudovisium-0.0.9/Pseudovisium/
+-rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.9/Pseudovisium/__init__.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    62530 2024-05-01 16:32:22.000000 Pseudovisium-0.0.9/Pseudovisium/pseudovisium_generate.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    14501 2024-04-23 21:00:08.000000 Pseudovisium-0.0.9/Pseudovisium/pseudovisium_merge.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    83436 2024-05-01 16:41:51.000000 Pseudovisium-0.0.9/Pseudovisium/pseudovisium_qc.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-02 07:18:41.399724 Pseudovisium-0.0.9/Pseudovisium.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      846 2024-05-02 07:18:41.000000 Pseudovisium-0.0.9/Pseudovisium.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-05-02 07:18:41.000000 Pseudovisium-0.0.9/Pseudovisium.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-02 07:18:41.000000 Pseudovisium-0.0.9/Pseudovisium.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)      129 2024-05-02 07:18:41.000000 Pseudovisium-0.0.9/Pseudovisium.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-05-02 07:18:41.000000 Pseudovisium-0.0.9/Pseudovisium.egg-info/top_level.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)     7450 2024-05-01 18:25:36.000000 Pseudovisium-0.0.9/README.md
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-05-02 07:18:41.400437 Pseudovisium-0.0.9/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)     1110 2024-05-01 15:06:07.000000 Pseudovisium-0.0.9/setup.py
```

### Comparing `Pseudovisium-0.0.8/LICENSE` & `Pseudovisium-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.8/Pseudovisium/pseudovisium_generate.py` & `Pseudovisium-0.0.9/Pseudovisium/pseudovisium_generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 import time
 import scanpy as sc
 import scipy.io
 import h5py
 import scipy.sparse
 from pathlib import Path
 
-def closest_hex(x,y,hexagon_size):
+def closest_hex(x,y,hexagon_size,spot_diameter=None):
     """
-    closest_hex(x, y, hexagon_size)
     Calculates the closest hexagon centroid to the given (x, y) coordinates.
 
     Args:
-    x (float): The x-coordinate.
-    y (float): The y-coordinate.
-    hexagon_size (float): The size of the hexagon.
+        x (float): The x-coordinate.
+        y (float): The y-coordinate.
+        hexagon_size (float): The size of the hexagon.
+        spot_diameter (float, optional): The diameter of the spot. Defaults to None.
 
     Returns:
         tuple: The closest hexagon centroid coordinates (x, y) rounded to the nearest integer.
     """
+    spot = True if spot_diameter!=None else False
 
     x_ = x // (hexagon_size*2)
     y_= y // (hexagon_size*1.732050807)
 
 
     if y_ % 2 == 1:
 
@@ -67,34 +68,38 @@
         option_3_hexagon = ((x_+1)*2*hexagon_size,(y_+1)*1.732050807*hexagon_size)
 
         #calc distance from each option and return the closest
         distance_1 = math.sqrt((x - option_1_hexagon[0])**2 + (y - option_1_hexagon[1])**2)
         distance_2 = math.sqrt((x - option_2_hexagon[0])**2 + (y - option_2_hexagon[1])**2)
         distance_3 = math.sqrt((x - option_3_hexagon[0])**2 + (y - option_3_hexagon[1])**2)
         closest = [option_1_hexagon,option_2_hexagon,option_3_hexagon][np.argmin([distance_1,distance_2,distance_3])]
-
-    closest = (round(closest[0], 0), round(closest[1], 1))
-    return closest
+    
+        closest = (round(closest[0], 0), round(closest[1], 1))
+    if spot:
+        if math.sqrt((x-closest[0])**2 + (y-closest[1])**2) < spot_diameter/2:
+            return closest
+        else:
+            return -1
+    else:
+        return closest
 
 
 
 
 def preprocess_csv(csv_file, batch_size, fieldnames):
     """
-    preprocess_csv(csv_file, batch_size, fieldnames)
     Preprocesses a CSV file by splitting it into smaller batches.
 
     Args:
         csv_file (str): The path to the CSV file.
         batch_size (int): The number of rows per batch.
         fieldnames (list): The list of field names to include in the batch CSV files.
 
     Returns:
         tuple: A tuple containing the temporary directory path and the total number of batches created.
-
     """
 
 
     tmp_dir = tempfile.mkdtemp(prefix="tmp_hexa")
     print(f"Created temporary directory {tmp_dir}")
     #if csv_file is .gz, then open it with gzip
     if csv_file.endswith('.gz'):
@@ -142,37 +147,42 @@
                 print(f"Created batch {batch_num}")
 
     print(f"Finished preprocessing. Total batches created: {batch_num}")
     return tmp_dir, batch_num
 
 
 
-def process_batch(batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname=None, quality_filter=False, count_colname="NA",smoothing=False, quality_per_hexagon=False, quality_per_probe=False,move_x=0,move_y=0,coord_to_um_conversion=1):
+def process_batch(batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname=None, quality_filter=False, count_colname="NA",smoothing=False, quality_per_hexagon=False, quality_per_probe=False,move_x=0,move_y=0,coord_to_um_conversion=1,spot_diameter=None):
     """
-    process_batch(batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname=None, quality_filter=False, count_colname="NA", smoothing=False)
     Processes a batch CSV file to calculate hexagon counts and cell counts.
 
     Args:
-    batch_file (str): The path to the batch CSV file.
-    hexagon_size (float): The size of the hexagon.
-    feature_colname (str): The name of the feature column.
-    x_colname (str): The name of the x-coordinate column.
-    y_colname (str): The name of the y-coordinate column.
-    cell_id_colname (str): The name of the cell ID column.
-    quality_colname (str, optional): The name of the quality score column. Defaults to None.
-    quality_filter (bool, optional): Whether to filter rows based on quality score. Defaults to False.
-    count_colname (str, optional): The name of the count column. Defaults to "NA".
-    smoothing (bool, optional): Whether to apply smoothing to the counts. Defaults to False.
+        batch_file (str): The path to the batch CSV file.
+        hexagon_size (float): The size of the hexagon.
+        feature_colname (str): The name of the feature column.
+        x_colname (str): The name of the x-coordinate column.
+        y_colname (str): The name of the y-coordinate column.
+        cell_id_colname (str): The name of the cell ID column.
+        quality_colname (str, optional): The name of the quality score column. Defaults to None.
+        quality_filter (bool, optional): Whether to filter rows based on quality score. Defaults to False.
+        count_colname (str, optional): The name of the count column. Defaults to "NA".
+        smoothing (bool, optional): Whether to apply smoothing to the counts. Defaults to False.
+        quality_per_hexagon (bool, optional): Whether to calculate quality per hexagon. Defaults to False.
+        quality_per_probe (bool, optional): Whether to calculate quality per probe. Defaults to False.
+        move_x (float, optional): The amount to move the x-coordinate. Defaults to 0.
+        move_y (float, optional): The amount to move the y-coordinate. Defaults to 0.
+        coord_to_um_conversion (float, optional): The conversion factor from coordinates to micrometers. Defaults to 1.
+        spot_diameter (float, optional): The diameter of the spot. Defaults to None.
 
     Returns:
-        dict or tuple: If cell_id_colname is not "None", returns a tuple containing the hexagon counts and hexagon cell counts.
-                    Otherwise, returns the hexagon counts dictionary.
-
+        tuple: A tuple containing the hexagon counts, hexagon cell counts, hexagon quality, and probe quality dictionaries.
     """
-    
+    spot = True if spot_diameter!=None else False
+
+
     hexagon_counts = {}
     if cell_id_colname != "None":
         hexagon_cell_counts = {}
     if quality_per_hexagon==True:
         hexagon_quality = {}
     if quality_per_probe==True:
         probe_quality = {}
@@ -182,15 +192,20 @@
         ##########Xenium with quality filter scenario
         with open(batch_file, 'r') as file:
             reader = csv.DictReader(file)
             for row in reader:
                 try:
                     x = (float(row[x_colname]) + move_x)*coord_to_um_conversion
                     y = (float(row[y_colname]) + move_y)*coord_to_um_conversion
-                    closest_hexagon = closest_hex(x, y, hexagon_size)
+                    if spot:
+                        closest_hexagon = closest_hex(x, y, hexagon_size, spot_diameter)
+                        if closest_hexagon == -1:
+                            continue
+                    else:
+                        closest_hexagon = closest_hex(x, y, hexagon_size)
                     if quality_per_hexagon==True:
                         if closest_hexagon not in hexagon_quality:
                             hexagon_quality[closest_hexagon] = {"mean":float(row[quality_colname]),"count":1}
                         else:
                             hexagon_quality[closest_hexagon]["mean"] = (hexagon_quality[closest_hexagon]["mean"]*hexagon_quality[closest_hexagon]["count"]+float(row[quality_colname]))/(hexagon_quality[closest_hexagon]["count"]+1)
                             hexagon_quality[closest_hexagon]["count"]+=1
                     if quality_per_probe==True:
@@ -226,15 +241,20 @@
                 ##########Visium HD with smoothing scenario
                 reader = csv.DictReader(file)
                 for row in reader:
                     try:
                         x = float(row[x_colname])+move_x
                         y = float(row[y_colname])+move_y
                         for x_new,y_new in [(x+smoothing,y+smoothing),(x-smoothing,y-smoothing),(x-smoothing,y+smoothing),(x+smoothing,y-smoothing)]:
-                            closest_hexagon = closest_hex(x_new, y_new, hexagon_size)
+                            if spot:
+                                closest_hexagon = closest_hex(x_new, y_new, hexagon_size, spot_diameter)
+                                if closest_hexagon == -1:
+                                    continue
+                            else:
+                                closest_hexagon = closest_hex(x_new, y_new, hexagon_size)
                             if closest_hexagon not in hexagon_counts:
                                 hexagon_counts[closest_hexagon] = {}
                             if row[feature_colname] not in hexagon_counts[closest_hexagon]:
                                 hexagon_counts[closest_hexagon][row[feature_colname]] = 0
                             hexagon_counts[closest_hexagon][row[feature_colname]] += float(row[count_colname])/4
                             if cell_id_colname != "None":
                                 if closest_hexagon not in hexagon_cell_counts:
@@ -250,15 +270,20 @@
                 ##########Visium HD scenario without smoothing
                 
                 reader = csv.DictReader(file)
                 for row in reader:
                     try:
                         x = float(row[x_colname])+move_x
                         y = float(row[y_colname])+move_y
-                        closest_hexagon = closest_hex(x, y, hexagon_size)
+                        if spot:
+                            closest_hexagon = closest_hex(x,y, hexagon_size, spot_diameter)
+                            if closest_hexagon == -1:
+                                continue
+                            else:
+                                closest_hexagon = closest_hex(x,y, hexagon_size)
                         if closest_hexagon not in hexagon_counts:
                             hexagon_counts[closest_hexagon] = {}
                         if row[feature_colname] not in hexagon_counts[closest_hexagon]:
                             hexagon_counts[closest_hexagon][row[feature_colname]] = 0
                         hexagon_counts[closest_hexagon][row[feature_colname]] += float(row[count_colname])
                         if cell_id_colname != "None":
                             if closest_hexagon not in hexagon_cell_counts:
@@ -279,31 +304,23 @@
         returning_items.append(probe_quality)
     return tuple(returning_items)
 
 
 
 
 def write_10X_h5(adata, file):
-    """Writes adata to a 10X-formatted h5 file.
-    
-    Note that this function is not fully tested and may not work for all cases.
-    It will not write the following keys to the h5 file compared to 10X:
-    '_all_tag_keys', 'pattern', 'read', 'sequence'
+    """
+    Writes adata to a 10X-formatted h5 file.
 
     Args:
         adata (AnnData object): AnnData object to be written.
-        file (str): File name to be written to. If no extension is given, '.h5' is appended.
-
-    Raises:
-        FileExistsError: If file already exists.
-
+        file (str): File name to be written to. If no extension is gi
     Returns:
         None
     """
-    #remove file
     
     if '.h5' not in file: file = f'{file}.h5'
     if Path(file).exists():
         print(f"File `{file}` already exists. Removing it.")
         os.remove(file)
     def int_max(x):
         return int(max(np.floor(len(str(int(max(x)))) / 4), 1) * 4)
@@ -330,46 +347,53 @@
         ftrs.create_dataset("genome", data=adata.var.genome.values.astype('|S'))
     if 'gene_ids' in adata.var:
         ftrs.create_dataset("id", data=adata.var.gene_ids.values.astype('|S'))
     ftrs.create_dataset("name", data=adata.var.index.values.astype('|S'))
     
     w.close()
 
-    
-
 
 def process_csv_file(csv_file, hexagon_size, batch_size=1000000, technology="Xenium", feature_colname="feature_name", x_colname="x_location", y_colname="y_location", cell_id_colname="None", quality_colname="qv", max_workers=min(2, multiprocessing.cpu_count()),
-                     quality_filter=False, count_colname="NA",smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname="x",h5_y_colname="y",move_x=0,move_y=0,coord_to_um_conversion=1):
+                     quality_filter=False, count_colname="NA",smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname="x",h5_y_colname="y",move_x=0,move_y=0,coord_to_um_conversion=1,spot_diameter=None):
     """
-    process_csv_file(csv_file, hexagon_size, field_size, batch_size=1000000, technology="Xenium", feature_colname="feature_name", x_colname="x_location", y_colname="y_location", cell_id_colname="None", quality_colname="qv", max_workers=min(2, multiprocessing.cpu_count()), quality_filter=False, count_colname="NA", smoothing=False)
     Processes a CSV file to calculate hexagon counts and cell counts using parallel processing.
 
     Args:
-    csv_file (str): The path to the CSV file.
-    hexagon_size (float): The size of the hexagon.
-    field_size (tuple): The size of the field as (field_size_x, field_size_y).
-    batch_size (int, optional): The number of rows per batch. Defaults to 1000000.
-    technology (str, optional): The technology used. Defaults to "Xenium".
-    feature_colname (str, optional): The name of the feature column. Defaults to "feature_name".
-    x_colname (str, optional): The name of the x-coordinate column. Defaults to "x_location".
-    y_colname (str, optional): The name of the y-coordinate column. Defaults to "y_location".
-    cell_id_colname (str, optional): The name of the cell ID column. Defaults to "None".
-    quality_colname (str, optional): The name of the quality score column. Defaults to "qv".
-    max_workers (int, optional): The maximum number of worker processes to use. Defaults to min(2, multiprocessing.cpu_count()).
-    quality_filter (bool, optional): Whether to filter rows based on quality score. Defaults to False.
-    count_colname (str, optional): The name of the count column. Defaults to "NA".
-    smoothing (bool, optional): Whether to apply smoothing to the counts. Defaults to False.
+        csv_file (str): The path to the CSV file.
+        hexagon_size (float): The size of the hexagon.
+        batch_size (int, optional): The number of rows per batch. Defaults to 1000000.
+        technology (str, optional): The technology used. Defaults to "Xenium".
+        feature_colname (str, optional): The name of the feature column. Defaults to "feature_name".
+        x_colname (str, optional): The name of the x-coordinate column. Defaults to "x_location".
+        y_colname (str, optional): The name of the y-coordinate column. Defaults to "y_location".
+        cell_id_colname (str, optional): The name of the cell ID column. Defaults to "None".
+        quality_colname (str, optional): The name of the quality score column. Defaults to "qv".
+        max_workers (int, optional): The maximum number of worker processes to use. Defaults to min(2, multiprocessing.cpu_count()).
+        quality_filter (bool, optional): Whether to filter rows based on quality score. Defaults to False.
+        count_colname (str, optional): The name of the count column. Defaults to "NA".
+        smoothing (bool, optional): Whether to apply smoothing to the counts. Defaults to False.
+        quality_per_hexagon (bool, optional): Whether to calculate quality per hexagon. Defaults to False.
+        quality_per_probe (bool, optional): Whether to calculate quality per probe. Defaults to False.
+        h5_x_colname (str, optional): The name of the x-coordinate column in the h5 file. Defaults to "x".
+        h5_y_colname (str, optional): The name of the y-coordinate column in the h5 file. Defaults to "y".
+        move_x (float, optional): The amount to move the x-coordinate. Defaults to 0.
+        move_y (float, optional): The amount to move the y-coordinate. Defaults to 0.
+        coord_to_um_conversion (float, optional): The conversion factor from coordinates to micrometers. Defaults to 1.
+        spot_diameter (float, optional): The diameter of the spot. Defaults to None.
 
     Returns:
-        tuple: A tuple containing the hexagon counts, hexagons dictionary, and hexagon cell counts.
+        tuple: A tuple containing the hexagon counts, hexagon cell counts, hexagon quality, and probe quality dictionaries.
     """
 
     print(f"Quality filter is set to {quality_filter}")
     print(f"Quality counting per hexagon is set to {quality_per_hexagon}")
     print(f"Quality counting per probe is set to {quality_per_probe}")
+    spot = True if spot_diameter!=None else False
+    if spot:
+        print("Visium-like spots are going to be used rather than hexagonal tesselation!!!")
 
     hexagon_counts = {}
     hexagon_cell_counts = {}
     hexagon_quality = {}
     probe_quality = {}
     #create a nested dict called hexagon quality, with two keys for each hexagon, one for the quality score and one for the count
     
@@ -398,14 +422,16 @@
         y_colname = "y_global_px"
         feature_colname = "target"
         cell_id_colname = "cell"
         count_colname= "NA"
         coord_to_um_conversion = 0.12028
         #see ref https://smi-public.objects.liquidweb.services/cosmx-wtx/Pancreas-CosMx-ReadMe.html
         #https://nanostring.com/wp-content/uploads/2023/09/SMI-ReadMe-BETA_humanBrainRelease.html
+        #Whereas old smi output seems to be 0.18 
+        # https://nanostring-public-share.s3.us-west-2.amazonaws.com/SMI-Compressed/SMI-ReadMe.html
 
 
     elif technology == "Visium_HD":
         print("Technology is Visium_HD. Going forward with pseudovisium processed colnames.")
         x_colname = "x"
         y_colname = "y"
         feature_colname = "gene"
@@ -446,15 +472,15 @@
 
 
     tmp_dir, num_batches = preprocess_csv(csv_file, batch_size, fieldnames)
     batch_files = [os.path.join(tmp_dir, f"batch_{i}.csv") for i in range(num_batches)]
     n_process = min(max_workers, multiprocessing.cpu_count())
     print(f"Processing batches using {n_process} processes")
     with concurrent.futures.ProcessPoolExecutor(max_workers=n_process) as executor:
-        futures = [executor.submit(process_batch, batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname, quality_filter, count_colname,smoothing,quality_per_hexagon,quality_per_probe, move_x,move_y,coord_to_um_conversion) for batch_file in batch_files]
+        futures = [executor.submit(process_batch, batch_file, hexagon_size, feature_colname, x_colname, y_colname, cell_id_colname, quality_colname, quality_filter, count_colname,smoothing,quality_per_hexagon,quality_per_probe, move_x,move_y,coord_to_um_conversion,spot_diameter) for batch_file in batch_files]
         
         with tqdm(total=len(batch_files), desc="Processing batches", unit="batch") as progress_bar:
             for future in concurrent.futures.as_completed(futures):
                 all_res = future.result()
                 batch_hexagon_counts = all_res[0]
                 for hexagon_counts_hex, counts in batch_hexagon_counts.items():
                     for feature_name, count in counts.items():
@@ -521,50 +547,66 @@
 
     shutil.rmtree(tmp_dir)  # Remove temporary directory and files
 
     return hexagon_counts, hexagon_cell_counts, hexagon_quality, probe_quality
 
 
 
-def process_hexagon(hexagon, hexagon_index, features, hexagon_counts):
-        return [[features.index(feature) + 1, hexagon_index + 1, count]
-                for feature, count in hexagon_counts[hexagon].items()]
-
 def hex_to_rows(hexagon_batch, start_index, features, hexagon_counts,hexagon_names):
+    """
+    Converts a batch of hexagons to rows for the matrix.
+
+    Args:
+        hexagon_batch (list): A list of hexagons to process.
+        start_index (int): The starting index for the hexagons.
+        features (list): A list of features.
+        hexagon_counts (dict): A dictionary of hexagon counts.
+        hexagon_names (list): A list of hexagon names.
+
+    Returns:
+        list: A list of matrix rows.
+    """
+
     matrix_data = []
     for hexagon in hexagon_batch: ###Here is the error!!! HExagon indices are scrambled!!!!!
         count_dict = hexagon_counts.get(hexagon, {})
         for feature, count in count_dict.items():
             feature_index = features.index(feature)
             hexagon_index = hexagon_names.index(hexagon)
             matrix_data.append([feature_index + 1, hexagon_index + 1, count])
     print(f"Batch total count: {sum(row[2] for row in matrix_data)}")
     return matrix_data
 
 def create_pseudovisium(path,hexagon_counts,hexagon_cell_counts,hexagon_quality, probe_quality,
                         img_file_path=None,  project_name="project",
                          alignment_matrix_file=None,image_pixels_per_um=1/0.2125,hexagon_size=100,tissue_hires_scalef=0.2,
-                         pixel_to_micron=False,max_workers=min(2, multiprocessing.cpu_count())):
+                         pixel_to_micron=False,max_workers=min(2, multiprocessing.cpu_count()),spot_diameter=None):
     """
-    create_pseudovisium(path, hexagon_counts, hexagon_cell_counts, img_file_path=None, project_name="project", alignment_matrix_file=None, image_pixels_per_um=1/0.2125, hexagon_size=100, tissue_hires_scalef=0.2, pixel_to_micron=False, max_workers=min(2, multiprocessing.cpu_count()))
     Creates a Pseudovisium output directory structure and files.
-    
+
     Args:
-    path (str): The path to create the Pseudovisium output directory.
-    hexagon_counts (dict): A dictionary of hexagon counts.
-    hexagon_cell_counts (dict): A dictionary of hexagon cell counts.
-    img_file_path (str, optional): The path to the image file. Defaults to None.
-    project_name (str, optional): The name of the project. Defaults to "project".
-    alignment_matrix_file (str, optional): The path to the alignment matrix file. Defaults to None.
-    image_pixels_per_um (float, optional): The number of image pixels per micrometer. Defaults to 1/0.2125.
-    hexagon_size (int, optional): The size of the hexagon. Defaults to 100.
-    tissue_hires_scalef (float, optional): The scaling factor for the high-resolution tissue image. Defaults to 0.2.
-    pixel_to_micron (bool, optional): Whether to convert pixel coordinates to micron coordinates. Defaults to False.
-    max_workers (int, optional): The maximum number of worker processes to use. Defaults to min(2, multiprocessing.cpu_count()).
-    """
+        path (str): The path to create the Pseudovisium output directory.
+        hexagon_counts (dict): A dictionary of hexagon counts.
+        hexagon_cell_counts (dict): A dictionary of hexagon cell counts.
+        hexagon_quality (dict): A dictionary of hexagon quality scores.
+        probe_quality (dict): A dictionary of probe quality scores.
+        img_file_path (str, optional): The path to the image file. Defaults to None.
+        project_name (str, optional): The name of the project. Defaults to "project".
+        alignment_matrix_file (str, optional): The path to the alignment matrix file. Defaults to None.
+        image_pixels_per_um (float, optional): The number of image pixels per micrometer. Defaults to 1/0.2125.
+        hexagon_size (int, optional): The size of the hexagon. Defaults to 100.
+        tissue_hires_scalef (float, optional): The scaling factor for the high-resolution tissue image. Defaults to 0.2.
+        pixel_to_micron (bool, optional): Whether to convert pixel coordinates to micron coordinates. Defaults to False.
+        max_workers (int, optional): The maximum number of worker processes to use. Defaults to min(2, multiprocessing.cpu_count()).
+        spot_diameter (float, optional): The diameter of the spot. Defaults to None.
+    """
+    spot = True if spot_diameter!=None else False
+    if spot:
+        print("Visium-like array structure is being built rather than hexagonal tesselation!!!")
+
 
     #to path, create a folder called pseudovisium
     folderpath = path+ '/pseudovisium/' + project_name
     #if folderpath exists, delete it
     if os.path.exists(folderpath):
         shutil.rmtree(folderpath)
     try:
@@ -578,24 +620,29 @@
         os.mkdir(folderpath + '/spatial')
     except:
         pass
     
  ############################################## ##############################################
     # see https://kb.10xgenomics.com/hc/en-us/articles/11636252598925-What-are-the-Xenium-image-scale-factors
     #https://www.10xgenomics.com/support/software/space-ranger/latest/analysis/outputs/spatial-outputs
+    
     scalefactors = {"tissue_hires_scalef":tissue_hires_scalef,
                      "tissue_lowres_scalef": tissue_hires_scalef/10,
-                       "fiducial_diameter_fullres": 0,
-                         "spot_diameter_fullres": 2*hexagon_size*(image_pixels_per_um)}
+                       "fiducial_diameter_fullres": 0}
+
+    if spot:
+        scalefactors["spot_diameter_fullres"] = spot_diameter*image_pixels_per_um
+    else:
+        scalefactors["spot_diameter_fullres"] = 2*hexagon_size*image_pixels_per_um
     
     print("Creating scalefactors_json.json file in spatial folder.")
     with open(folderpath +'/spatial/scalefactors_json.json', 'w') as f:
         json.dump(scalefactors, f)
  ############################################## ##############################################
-
+    
     x, y, x_, y_, contain, hexagon_names = [], [], [], [], [], []
     for hexagon in hexagon_counts:
         x_.append((hexagon[0] + hexagon_size) // (2 * hexagon_size))
         y_.append(hexagon[1] // (1.73205 * hexagon_size))
         x.append(hexagon[0])
         y.append(hexagon[1])
         contain.append(1 if sum(hexagon_counts[hexagon].values()) > hexagon_size else 0)
@@ -832,23 +879,26 @@
 
 
 #####################
 ###############  Visium HD/Slide-seq helper functions 
 ###################################################################################################################################################
 def read_files(folder,technology):
     """
-    read_files(folder)
-    Reads the necessary files from a Visium HD folder.
+    Reads the necessary files from a Visium HD or Curio folder.
 
     Args:
-    folder (str): The path to the Visium HD folder.
+        folder (str): The path to the Visium HD or Curio folder.
+        technology (str): The technology used, either "Visium_HD" or "Curio".
 
     Returns:
-        tuple: A tuple containing the scale factors, tissue positions, and filtered feature-barcode matrix.
+        tuple or AnnData: A tuple containing the scale factors, tissue positions, and filtered feature-barcode matrix (for Visium HD),
+                          or an AnnData object (for Curio).
     """
+
+    
     if technology == "Visium_HD":
         scalefactors = json.load(open(folder+"/spatial/scalefactors_json.json"))
         tissue_pos = pd.read_parquet(folder+"/spatial/tissue_positions.parquet")
         fb_matrix = sc.read_10x_h5(folder+"/filtered_feature_bc_matrix.h5")
         return scalefactors,tissue_pos,fb_matrix
     elif technology == "Curio":
         #find file ending with .h5ad in folder
@@ -856,24 +906,28 @@
         h5ad_file = [file for file in folder_files if file.endswith(".h5ad")][0]
         adata = sc.read(folder+h5ad_file)
         return adata
     
 
 def anndata_to_df(adata, technology,tissue_pos=None,scalefactors=None,x_col=None,y_col=None):
     """
-    anndata_to_df(adata, tissue_pos, scalefactors)
     Converts an AnnData object to a DataFrame.
+
     Args:
-    adata (AnnData): The AnnData object containing the counts matrix.
-    tissue_pos (DataFrame): The tissue positions DataFrame.
-    scalefactors (dict): The scale factors dictionary.
+        adata (AnnData): The AnnData object containing the counts matrix.
+        technology (str): The technology used, either "Visium_HD" or "Curio".
+        tissue_pos (DataFrame, optional): The tissue positions DataFrame (for Visium HD). Defaults to None.
+        scalefactors (dict, optional): The scale factors dictionary (for Visium HD). Defaults to None.
+        x_col (str, optional): The name of the x-coordinate column (for Curio). Defaults to None.
+        y_col (str, optional): The name of the y-coordinate column (for Curio). Defaults to None.
 
     Returns:
-        tuple: A tuple containing the converted DataFrame and the image resolution.
+        tuple: A tuple containing the converted DataFrame and the image resolution or scale.
     """
+
     if technology == "Visium_HD":
         #get image resolution of the hires image
         image_resolution = scalefactors["microns_per_pixel"]/scalefactors["tissue_hires_scalef"]
         #change to pixel per micron
         image_resolution = 1/image_resolution
         #tissue_pos keep barcode, pxl_row_in_fullres, pxl_col_in_fullres
         tissue_pos = tissue_pos[["barcode","pxl_row_in_fullres","pxl_col_in_fullres"]]
@@ -928,22 +982,25 @@
         #join with tissue_pos
         df = pd.merge(df,obs,on="barcode")
         return df,scale
 
 
 def visium_hd_curio_to_transcripts(folder,output,technology,x_col=None,y_col=None):
     """
-    visium_hd_to_transcripts(folder, output)
-    Converts Visium HD files to a transcripts CSV file.
+    Converts Visium HD or Curio files to a transcripts CSV file.
+
     Args:
-    folder (str): The path to the Visium HD folder.
-    output (str): The path to save the transcripts CSV file.
+        folder (str): The path to the Visium HD or Curio folder.
+        output (str): The path to save the transcripts CSV file.
+        technology (str): The technology used, either "Visium_HD" or "Curio".
+        x_col (str, optional): The name of the x-coordinate column (for Curio). Defaults to None.
+        y_col (str, optional): The name of the y-coordinate column (for Curio). Defaults to None.
 
     Returns:
-        float: The image resolution (pixels per micrometer).
+        float: The image resolution (pixels per micrometer) for Visium HD, or the scale for Curio.
     """
 
     if technology == "Visium_HD":
         scalefactors,tissue_pos,fb_matrix = read_files(folder,technology)
         df,image_resolution  = anndata_to_df(adata=fb_matrix,technology=technology,tissue_pos=tissue_pos,scalefactors=scalefactors)
         df.to_csv(output,index=False)
         return image_resolution 
@@ -956,53 +1013,52 @@
 
 
 
 
 ######### Main function to generate pseudovisium output ############################################################################################################
     
 def generate_pv(csv_file,img_file_path=None, hexagon_size=100,  output_path=None, batch_size=1000000, alignment_matrix_file=None, project_name='project',
-                image_pixels_per_um=1/0.85, tissue_hires_scalef=0.2,technology="Xenium", 
+                image_pixels_per_um=1, tissue_hires_scalef=0.2,technology="Xenium", 
                 feature_colname="feature_name", x_colname="x_location", y_colname="y_location",
                 cell_id_colname="None", quality_colname="qv",
                 pixel_to_micron=False, max_workers=min(2, multiprocessing.cpu_count()), quality_filter=False, count_colname="NA",visium_hd_folder=None,
-                smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname = "x", h5_y_colname = "y",move_x=0,move_y=0,coord_to_um_conversion=1):
+                smoothing=False,quality_per_hexagon=False,quality_per_probe=False,h5_x_colname = "x", h5_y_colname = "y",move_x=0,move_y=0,coord_to_um_conversion=1,spot_diameter=None):
     """
-    generate_pv(csv_file, img_file_path=None, hexagon_size=100, field_size_x=1000, field_size_y=1000, output_path=None, 
-    batch_size=1000000, alignment_matrix_file=None, project_name='project', image_pixels_per_um=1/0.85, tissue_hires_scalef=0.2, 
-    technology="Xenium", feature_colname="feature_name", x_colname="x_location", y_colname="y_location", cell_id_colname="None", 
-    quality_colname="qv", pixel_to_micron=False, max_workers=min(2, multiprocessing.cpu_count()), quality_filter=False, 
-    count_colname="NA", visium_hd_folder=None, smoothing=False)
-
-    
-    Generates a Pseudovisium output from a CSV file.
+    Generates a Pseudovisium output from a CSV file or Visium HD/Curio folder.
 
     Args:
-    csv_file (str): The path to the CSV file.
-    img_file_path (str, optional): The path to the image file. Defaults to None.
-    hexagon_size (int, optional): The size of the hexagon. Defaults to 100.
-    field_size_x (int, optional): The size of the field in the x-dimension. Defaults to 1000.
-    field_size_y (int, optional): The size of the field in the y-dimension. Defaults to 1000.
-    output_path (str, optional): The path to save the Pseudovisium output. Defaults to None.
-    batch_size (int, optional): The number of rows per batch. Defaults to 1000000.
-    alignment_matrix_file (str, optional): The path to the alignment matrix file. Defaults to None.
-    project_name (str, optional): The name of the project. Defaults to 'project'.
-    image_pixels_per_um (float, optional): The number of image pixels per micrometer. Defaults to 1/0.85.
-    tissue_hires_scalef (float, optional): The scaling factor for the high-resolution tissue image. Defaults to 0.2.
-    technology (str, optional): The technology used. Defaults to "Xenium".
-    feature_colname (str, optional): The name of the feature column. Defaults to "feature_name".
-    x_colname (str, optional): The name of the x-coordinate column. Defaults to "x_location".
-    y_colname (str, optional): The name of the y-coordinate column. Defaults to "y_location".
-    cell_id_colname (str, optional): The name of the cell ID column. Defaults to "None".
-    quality_colname (str, optional): The name of the quality score column. Defaults to "qv".
-    pixel_to_micron (bool, optional): Whether to convert pixel coordinates to micron coordinates. Defaults to False.
-    max_workers (int, optional): The maximum number of worker processes to use. Defaults to min(2, multiprocessing.cpu_count()).
-    quality_filter (bool, optional): Whether to filter rows based on quality score. Defaults to False.
-    count_colname (str, optional): The name of the count column. Defaults to "NA".
-    visium_hd_folder (str, optional): The path to the Visium HD folder. Defaults to None.
-    smoothing (float, optional): The smoothing factor. Defaults to False.
+        csv_file (str): The path to the CSV file.
+        img_file_path (str, optional): The path to the image file. Defaults to None.
+        hexagon_size (int, optional): The size of the hexagon. Defaults to 100.
+        output_path (str, optional): The path to save the Pseudovisium output. Defaults to None.
+        batch_size (int, optional): The number of rows per batch. Defaults to 1000000.
+        alignment_matrix_file (str, optional): The path to the alignment matrix file. Defaults to None.
+        project_name (str, optional): The name of the project. Defaults to 'project'.
+        image_pixels_per_um (float, optional): The number of image pixels per micrometer. Defaults to 1.
+        tissue_hires_scalef (float, optional): The scaling factor for the high-resolution tissue image. Defaults to 0.2.
+        technology (str, optional): The technology used. Defaults to "Xenium".
+        feature_colname (str, optional): The name of the feature column. Defaults to "feature_name".
+        x_colname (str, optional): The name of the x-coordinate column. Defaults to "x_location".
+        y_colname (str, optional): The name of the y-coordinate column. Defaults to "y_location".
+        cell_id_colname (str, optional): The name of the cell ID column. Defaults to "None".
+        quality_colname (str, optional): The name of the quality score column. Defaults to "qv".
+        pixel_to_micron (bool, optional): Whether to convert pixel coordinates to micron coordinates. Defaults to False.
+        max_workers (int, optional): The maximum number of worker processes to use. Defaults to min(2, multiprocessing.cpu_count()).
+        quality_filter (bool, optional): Whether to filter rows based on quality score. Defaults to False.
+        count_colname (str, optional): The name of the count column. Defaults to "NA".
+        visium_hd_folder (str, optional): The path to the Visium HD folder. Defaults to None.
+        smoothing (float, optional): The smoothing factor. Defaults to False.
+        quality_per_hexagon (bool, optional): Whether to calculate quality per hexagon. Defaults to False.
+        quality_per_probe (bool, optional): Whether to calculate quality per probe. Defaults to False.
+        h5_x_colname (str, optional): The name of the x-coordinate column in the h5 file. Defaults to "x".
+        h5_y_colname (str, optional): The name of the y-coordinate column in the h5 file. Defaults to "y".
+        move_x (float, optional): The amount to move the x-coordinate. Defaults to 0.
+        move_y (float, optional): The amount to move the y-coordinate. Defaults to 0.
+        coord_to_um_conversion (float, optional): The conversion factor from coordinates to micrometers. Defaults to 1.
+        spot_diameter (float, optional): The diameter of the spot. Defaults to None.
     """
 
 
     start = time.time()
 
     if technology == "Visium_HD":
         print("Technology is Visium_HD. Generating transcripts.csv file from Visium HD files.")
@@ -1017,54 +1073,57 @@
         smoothing = smoothing_scale/4
         
         # Process CSV file to generate hexagon counts and hexagon information
     
     hexagon_counts, hexagon_cell_counts, hexagon_quality, probe_quality= process_csv_file(csv_file, hexagon_size,  batch_size, 
              technology, feature_colname, x_colname, y_colname,cell_id_colname, quality_colname=quality_colname,
                max_workers=max_workers, quality_filter=quality_filter, count_colname=count_colname,smoothing=smoothing,
-               quality_per_hexagon=quality_per_hexagon,quality_per_probe=quality_per_probe,h5_x_colname=h5_x_colname,h5_y_colname=h5_y_colname,move_x=move_x,move_y=move_y,coord_to_um_conversion=coord_to_um_conversion)
+               quality_per_hexagon=quality_per_hexagon,quality_per_probe=quality_per_probe,h5_x_colname=h5_x_colname,
+               h5_y_colname=h5_y_colname,move_x=move_x,move_y=move_y,coord_to_um_conversion=coord_to_um_conversion,
+                spot_diameter=spot_diameter)
         
     # Create Pseudovisium output
     create_pseudovisium(path=output_path,hexagon_counts=hexagon_counts, hexagon_cell_counts=hexagon_cell_counts, probe_quality=probe_quality,
                         img_file_path=img_file_path, hexagon_quality =hexagon_quality,
                           project_name=project_name, alignment_matrix_file=alignment_matrix_file,
                           image_pixels_per_um=image_pixels_per_um,hexagon_size=hexagon_size,
-                          tissue_hires_scalef=tissue_hires_scalef,pixel_to_micron=pixel_to_micron,max_workers=max_workers)
+                          tissue_hires_scalef=tissue_hires_scalef,pixel_to_micron=pixel_to_micron,max_workers=max_workers,
+                            spot_diameter=spot_diameter)
 
     #save all arguments in a json file called arguments.json
     print("Creating arguments.json file in output path.")
     arguments = {"csv_file":csv_file,"img_file_path":img_file_path,"hexagon_size":hexagon_size,
                     "output_path":output_path,
                     "batch_size":batch_size,"alignment_matrix_file":alignment_matrix_file,"project_name":project_name,
                     "image_pixels_per_um":image_pixels_per_um,"tissue_hires_scalef":tissue_hires_scalef,
                     "technology":technology,"feature_colname":feature_colname,"x_colname":x_colname,
                     "y_colname":y_colname,"cell_id_colname":cell_id_colname,"pixel_to_micron":pixel_to_micron,
                     "quality_colname":quality_colname,"quality_filter":quality_filter,"count_colname":count_colname,
                     "smoothing":smoothing,"quality_per_hexagon":quality_per_hexagon,"quality_per_probe":quality_per_probe,
                     "max_workers":max_workers,"visium_hd_folder":visium_hd_folder,"h5_x_colname":h5_x_colname,"h5_y_colname":h5_y_colname,
-                    "move_x":move_x,"move_y":move_y,"coord_to_um_conversion":coord_to_um_conversion}
+                    "move_x":move_x,"move_y":move_y,"coord_to_um_conversion":coord_to_um_conversion,
+                    "spot_diameter":spot_diameter}
 
     with open(output_path + '/pseudovisium/' + project_name + '/arguments.json', 'w') as f:
         json.dump(arguments, f)
 
     end = time.time()
     print(f"Time taken: {end - start} seconds")
 
 
 
 
 def main():
     """
-    main()
     The main function that parses command-line arguments and calls the generate_pv function.
     """
     parser = argparse.ArgumentParser(description="Process parameters.")
     parser.add_argument("--csv_file", "-c", type=str, help="CSV file path", default=None)
     parser.add_argument("--output_path", "-o", type=str, help="Output path", default='.')
-    parser.add_argument("--hexagon_size", "-hs", type=int, help="Hexagon size", default=100)
+    parser.add_argument("--hexagon_size", "-hs", type=float, help="Hexagon size", default=100.0)
     parser.add_argument("--img_file_path", "-i", type=str, help="Image file path", default=None)
     parser.add_argument("--alignment_matrix_file", "-am", type=str, help="Alignment matrix file path", default=None)
     parser.add_argument("--batch_size", "-b", type=int, help="Batch size", default=1000000)
     parser.add_argument("--project_name", "-p", type=str, help="Project name", default='project')
     parser.add_argument("--image_pixels_per_um", "-ppu", type=float, help="Image pixels per um", default=1)#changed from 1/0.2125 that was set for Xenium
     parser.add_argument("--tissue_hires_scalef", "-ths", type=float, help="Tissue hires scale factor", default=0.2)
     parser.add_argument("--technology", "-t", type=str, help="Technology", default="Xenium")
@@ -1079,48 +1138,59 @@
     parser.add_argument("--visium_hd_folder", "-vhf", type=str, help="Visium HD folder", default=None)
     parser.add_argument("--mw", "--max_workers", type=int, help="Max workers", default=min(2, multiprocessing.cpu_count()))
     parser.add_argument("--quality_filter", "-qf", action="store_true", help="Filter out rows with quality score less than 20")
     parser.add_argument("--quality_per_hexagon", "-qph", action="store_true", help="Calculate quality per hexagon")
     parser.add_argument("--quality_per_probe", "-qpp", action="store_true", help="Calculate quality per probe")
     parser.add_argument("--h5_x_colname", "-h5x", type=str, help="X column name in h5ad file", default="x")
     parser.add_argument("--h5_y_colname", "-h5y", type=str, help="Y column name in h5ad file", default="y")
-    parser.add_argument("--move_x","-mx", type=int, help="Move x", default=0)
-    parser.add_argument("--move_y","-my", type=int, help="Move y", default=0)
+    parser.add_argument("--move_x","-mx", type=float, help="Move x", default=0.0)
+    parser.add_argument("--move_y","-my", type=float, help="Move y", default=0.0)
     parser.add_argument("--coord_to_um_conversion","-ctu", type=float, help="Conversion factor from coordinates to microns", default=1.0)
+    parser.add_argument("--spot_diameter","-sd", type=float, help="Spot diameter", default=None)
     parser.add_argument("-v", "--verbose", action="store_true", help="Print out script purpose and parameters")
     
     
     #make sure to add verbose as well
     parser.add_argument("-help", action="store_true", help="Print out script purpose and parameters")
     args = parser.parse_args()
 
     if args.help:
         print("This is Pseudovisium, a software that compresses imaging-based spatial transcriptomics files using hexagonal binning of the data.")
         parser.print_help()
         sys.exit(0)
     
 
-    generate_pv(csv_file=args.csv_file,img_file_path=args.img_file_path,
-                hexagon_size=args.hexagon_size, output_path=args.output_path, 
+    generate_pv(csv_file=args.csv_file,
+                img_file_path=args.img_file_path,
+                hexagon_size=args.hexagon_size,
+                output_path=args.output_path, 
                 batch_size=args.batch_size,
                 alignment_matrix_file=args.alignment_matrix_file, 
-                project_name=args.project_name,image_pixels_per_um=args.image_pixels_per_um, 
-                tissue_hires_scalef=args.tissue_hires_scalef,technology=args.technology, 
-                feature_colname=args.feature_colname, x_colname=args.x_colname, 
-                y_colname=args.y_colname,cell_id_colname=args.cell_id_colname,
-                pixel_to_micron=args.pixel_to_micron,max_workers=args.mw,
-                quality_colname=args.quality_colname,quality_filter=args.quality_filter,
+                project_name=args.project_name,
+                image_pixels_per_um=args.image_pixels_per_um, 
+                tissue_hires_scalef=args.tissue_hires_scalef,
+                technology=args.technology, 
+                feature_colname=args.feature_colname,
+                x_colname=args.x_colname, 
+                y_colname=args.y_colname,
+                cell_id_colname=args.cell_id_colname,
+                pixel_to_micron=args.pixel_to_micron,
+                max_workers=args.mw,
+                quality_colname=args.quality_colname,
+                quality_filter=args.quality_filter,
                 count_colname=args.count_colname,
                 smoothing=args.smoothing,
                 quality_per_hexagon=args.quality_per_hexagon,
                 quality_per_probe=args.quality_per_probe,
-                h5_x_colname=args.h5_x_colname,h5_y_colname=args.h5_y_colname,
+                h5_x_colname=args.h5_x_colname,
+                h5_y_colname=args.h5_y_colname,
                 move_x=args.move_x,move_y=args.move_y,
                 coord_to_um_conversion=args.coord_to_um_conversion,
-                visium_hd_folder=args.visium_hd_folder)
+                visium_hd_folder=args.visium_hd_folder,
+                spot_diameter=args.spot_diameter)
                 
     print("Pseudovisium output generated successfully.")
```

### Comparing `Pseudovisium-0.0.8/Pseudovisium/pseudovisium_merge.py` & `Pseudovisium-0.0.9/Pseudovisium/pseudovisium_merge.py`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.8/Pseudovisium/pseudovisium_qc.py` & `Pseudovisium-0.0.9/Pseudovisium/pseudovisium_qc.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,26 @@
 import warnings
 
 #throughout remove Warnings
 warnings.filterwarnings("ignore",category=FutureWarning)
 
 
 def generate_qc_report(folders, output_folder=os.getcwd(), gene_names=["RYR3", "AQP4", "THBS1"], include_morans_i=False,max_workers=4,normalisation=False,save_plots=False):
+    """
+    Generate a QC report for Pseudovisium output.
+
+    Args:
+        folders (list): List of folders containing Pseudovisium output.
+        output_folder (str, optional): Output folder path. Defaults to current working directory.
+        gene_names (list, optional): List of gene names to plot. Defaults to ["RYR3", "AQP4", "THBS1"].
+        include_morans_i (bool, optional): Include Moran's I features tab. Defaults to False.
+        max_workers (int, optional): Number of workers to use for parallel processing. Defaults to 4.
+        normalisation (bool, optional): Normalise the counts by the total counts per cell. Defaults to False.
+        save_plots (bool, optional): Save generated plots as publication ready figures. Defaults to False.
+    """
 
     if save_plots:
         print("Plots will be saved")
     #if any entry in folders lacks final /, then add
     folders = [folder if folder[-1]=="/" else folder + "/" for folder in folders]
     #same with output_folder
     output_folder = output_folder if output_folder[-1]=="/" else output_folder + "/"
@@ -70,15 +82,15 @@
             
 
         if quality_per_probe:
             probe_quality = pd.read_csv(folder + "spatial/quality_per_probe.csv", header=None)
             #name cols as barcode, quality, count
             probe_quality.columns = ["Probe_ID", "Quality", "Count"]
             probe_quality["Dataset"] = dataset_name
-            non_ctrl_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
+            non_ctrl_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")]
             non_ctrl_probes_q_below_20 = non_ctrl_probes[non_ctrl_probes["Quality"]<20]
             pct_non_ctrl_probes_q_below_20 = len(non_ctrl_probes_q_below_20)/len(non_ctrl_probes)
             
         
         if cell_info:
             pv_cell_hex = pd.read_csv(folder + "spatial/pv_cell_hex.csv", header=None)
             pv_cell_hex.columns = ["Cell_ID", "Hexagon_ID", "Count"]
@@ -119,15 +131,15 @@
         cv_counts = np.std(grouped_matrix) / np.mean(grouped_matrix)
 
         grouped_matrix = matrix_joined.groupby("Barcode_ID")["Gene_ID_y"].count()
         median_features = np.median(grouped_matrix)
         cv_features = np.std(grouped_matrix) / np.mean(grouped_matrix)
 
         number_of_probes = len(features)
-        number_of_genes = len(features[~features["Gene_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")])
+        number_of_genes = len(features[~features["Gene_ID"].str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")])
         
 
         neg_control_probes = features[features["Gene_ID"].str.contains("Probe")].index + 1
         neg_control_counts = np.sum(matrix[matrix["Gene_ID"].isin(neg_control_probes)]["Counts"])
         total_counts = np.sum(matrix["Counts"])
         prop_neg_control = neg_control_counts / total_counts
         if cell_info:
@@ -299,15 +311,32 @@
     quality_per_hexagon=quality_per_hexagon,quality_per_probe=quality_per_probe,cell_info=cell_info,normalisation=normalisation,save_plots=save_plots,output_folder=data_output_folder + "/plots")
 
     with open(output, "w", encoding="utf-8") as html_file:
         html_file.write(html_code)
         print("HTML file generated successfully!")
 
 def generate_dashboard_html(replicates_data, gene_names, include_morans_i,quality_per_hexagon,quality_per_probe,cell_info,normalisation=False,save_plots=False,output_folder=os.getcwd()):
-    #AS A START PRINT VALUES OF include_morans_i, quality_per_hexagon etc.
+    """
+    Generate the HTML code for the QC report dashboard.
+
+    Args:
+        replicates_data (list): List of dictionaries containing data for each replicate.
+        gene_names (list): List of gene names to plot.
+        include_morans_i (bool): Include Moran's I features tab.
+        quality_per_hexagon (bool): Include quality per hexagon plots.
+        quality_per_probe (bool): Include quality per probe plots.
+        cell_info (bool): Include cell information plots.
+        normalisation (bool, optional): Normalise the counts by the total counts per cell. Defaults to False.
+        save_plots (bool, optional): Save generated plots as publication ready figures. Defaults to False.
+        output_folder (str, optional): Output folder path. Defaults to current working directory.
+
+    Returns:
+        str: Generated HTML code for the QC report dashboard.
+    """
+
     print("include_morans_i: ",include_morans_i)
     print("quality_per_hexagon: ",quality_per_hexagon)
     print("quality_per_probe: ",quality_per_probe)
     print("cell_info: ",cell_info)
 
 
     metrics_html = """
@@ -1014,18 +1043,28 @@
     </body>
     </html>
     """
     return html_code
 
 
 def not_working_probe_based_on_sum(matrix_joined,sample_id="Sample1"):
+    """
+    Identify probes that are not working based on their sum counts.
+
+    Args:
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+        sample_id (str, optional): Sample ID. Defaults to "Sample1".
+
+    Returns:
+        pandas.DataFrame: DataFrame with probe categories (Good, Bad, Neg_control) based on sum counts.
+    """
     grouped_matrix = matrix_joined.groupby("Gene_ID_y")["Counts"].sum()
     #where index has control|blank|Control|Blank|BLANK in it
-    grouped_matrix_neg_probes = grouped_matrix[grouped_matrix.index.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
-    grouped_matrix_true_probes = grouped_matrix[~grouped_matrix.index.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]     
+    grouped_matrix_neg_probes = grouped_matrix[grouped_matrix.index.str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")]
+    grouped_matrix_true_probes = grouped_matrix[~grouped_matrix.index.str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")]     
 
     #create a plot_df that is grouped_matrix and a column specifying whether the gene is a neg control or not
     plot_df = pd.DataFrame(grouped_matrix)
     plot_df["Probe category"] = [1 if gene in grouped_matrix_neg_probes.index.values else 0 for gene in plot_df.index.values]
     plot_df["gene"] = plot_df.index.values
     plot_df["log_counts"] = np.log10(plot_df["Counts"])
 
@@ -1049,14 +1088,29 @@
 
 
 
 
 
 
 def probe_stripplot(plot_df, col_to_plot="log_counts", sample_id="Sample 1", legend=False,save_plot=False,output_folder=None):
+    """
+    Generate a stripplot of probe counts or quality scores.
+
+    Args:
+        plot_df (pandas.DataFrame): DataFrame containing probe information.
+        col_to_plot (str, optional): Column to plot. Defaults to "log_counts".
+        sample_id (str, optional): Sample ID. Defaults to "Sample 1".
+        legend (bool, optional): Whether to include a legend. Defaults to False.
+        save_plot (bool, optional): Whether to save the plot. Defaults to False.
+        output_folder (str, optional): Output folder for saving the plot. Defaults to None.
+
+    Returns:
+        str: HTML code for the generated stripplot.
+    """
+    
     fig, ax = plt.subplots(figsize=(2, 2.5))
     # Define jitter amount
     jitter = 0.1
 
     # Create a dictionary to store x and y values for each point
     points = {"x": [], "y": [], "cat": [], "index": []}
 
@@ -1115,16 +1169,27 @@
         plt.savefig(f"{output_folder}/{sample_id}_probe_stripplot.png", dpi=400)
         plt.savefig(f"{output_folder}/{sample_id}_probe_stripplot.svg", dpi=400)
     plt.close(fig)
         
     return html_fig
 
 def not_working_probe_based_on_quality(probe_quality, sample_id="Sample1"):
-    probe_quality_neg_probes = probe_quality[probe_quality["Probe_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
-    probe_quality_true_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
+    """
+    Identify probes that are not working based on their quality scores.
+
+    Args:
+        probe_quality (pandas.DataFrame): DataFrame containing probe quality information.
+        sample_id (str, optional): Sample ID. Defaults to "Sample1".
+
+    Returns:
+        pandas.DataFrame: DataFrame with probe categories (Good, Bad, Neg_control) based on quality scores.
+    """
+    
+    probe_quality_neg_probes = probe_quality[probe_quality["Probe_ID"].str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")]
+    probe_quality_true_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")]
     plot_df = probe_quality.reset_index(drop=True)
     plot_df["Probe category"] = [1 if gene in probe_quality_neg_probes.Probe_ID.values else 0 for gene in plot_df.Probe_ID.values]
 
     #iterate through the true probes and see whether they are significantly outside of the distribution of the neg probes
     for gene in probe_quality_true_probes.Probe_ID.values:
         plot_df_gene_index = plot_df[plot_df["Probe_ID"]==gene].index[0]
         quality = plot_df[plot_df["Probe_ID"]==gene]["Quality"]
@@ -1141,17 +1206,26 @@
     plot_df = plot_df.sort_values("Probe category")
     return plot_df
 
 
 
 
 def not_working_probe_based_on_morans_i(morans_table, sample_id="Sample1"):
-    
-    morans_table_neg_probes = morans_table[morans_table.gene.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
-    morans_table_true_probes = morans_table[~morans_table.gene.str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]     
+    """
+    Identify probes that are not working based on their Moran's I values.
+
+    Args:
+        morans_table (pandas.DataFrame): DataFrame containing Moran's I values for each probe.
+        sample_id (str, optional): Sample ID. Defaults to "Sample1".
+
+    Returns:
+        pandas.DataFrame: DataFrame with probe categories (Good, Bad, Neg_control) based on Moran's I values.
+    """
+    morans_table_neg_probes = morans_table[morans_table.gene.str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")]
+    morans_table_true_probes = morans_table[~morans_table.gene.str.contains("control|ctrl|pos|NegPrb|neg|Ctrl|blank|Control|Blank|BLANK")]     
 
     #create a plot_df that is grouped_matrix and a column specifying whether the gene is a neg control or not
     plot_df = morans_table.reset_index(drop=True)
     plot_df["Probe category"] = [1 if gene in morans_table_neg_probes.gene.values else 0 for gene in plot_df.gene.values]
 
     neg_probes_morans_i_s = plot_df[plot_df["Probe category"]==1]["Morans_I"]
     mean = np.mean(neg_probes_morans_i_s)
@@ -1171,34 +1245,74 @@
     plot_df["Sample"] = sample_id
     plot_df = plot_df.sort_values("Probe category")
     return plot_df
 
 
 
 def get_unique_features_per_hexagon(matrix_joined):
+    """
+    Calculate the number of unique features per hexagon.
+
+    Args:
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+
+    Returns:
+        pandas.DataFrame: DataFrame with the number of unique features per hexagon.
+    """
     unique_features_per_hexagon = matrix_joined.groupby(['x', 'y'])['Gene_ID_y'].nunique().reset_index()
     unique_features_per_hexagon = unique_features_per_hexagon.rename(columns={"Gene_ID_y": "counts"})
     return unique_features_per_hexagon
 
 
 def get_total_counts_per_hexagon(matrix_joined):
+    
+    """
+    Calculate the total counts per hexagon.
+
+    Args:
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+
+    Returns:
+        pandas.DataFrame: DataFrame with the total counts per hexagon.
+    """
     total_counts_per_hexagon = matrix_joined.groupby(['x', 'y'])['Counts'].sum().reset_index()
     total_counts_per_hexagon = total_counts_per_hexagon.rename(columns={"Counts": "counts"})
     return total_counts_per_hexagon
 
 def get_quality_per_hexagon(matrix_joined):
+    """
+    Calculate the quality score per hexagon.
+
+    Args:
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+
+    Returns:
+        pandas.DataFrame: DataFrame with the quality score per hexagon.
+    """
     hexagon_quality = matrix_joined.groupby("Barcode_ID").agg({"Quality":"first","x":"first","y":"first"})
     hexagon_quality = hexagon_quality.reset_index()
     #rename Quality to counts
     hexagon_quality = hexagon_quality.rename(columns={"Quality": "counts"})
     return hexagon_quality
 
 
 # Functions used in generate_qc_report
 def get_df_for_gene(matrix_joined, tissue_positions_list, gene_name, normalised=False):
+    """
+    Get a DataFrame for a specific gene.
+
+    Args:
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+        tissue_positions_list (pandas.DataFrame): DataFrame containing tissue positions.
+        gene_name (str): Name of the gene to retrieve.
+        normalised (bool, optional): Whether to normalize the counts. Defaults to False.
+
+    Returns:
+        pandas.DataFrame: DataFrame containing information for the specified gene.
+    """
     matrix_subset = matrix_joined[matrix_joined["Gene_ID_y"] == gene_name]
     matrix_subset.reset_index(drop=True, inplace=True)
     x = tissue_positions_list["x"]
     y = tissue_positions_list["y"]
     counts = np.zeros(len(tissue_positions_list))
     for i in range(len(matrix_subset)):
         count = matrix_subset["Counts"][i]
@@ -1213,14 +1327,31 @@
         counts = np.append(counts, count)
     df = pd.DataFrame({"x": x, "y": y, "counts": counts})
     return df.sort_values("counts", ascending=False).drop_duplicates(subset=["x", "y"])
 
 
 
 def hexagon_plot_to_html(hexagon_df, hexagon_size, image_pixels_per_um, gene_name, dataset_name,morans_i=None,save_plot=False,output_folder=None):
+    """
+    Generate an HTML hexagon plot for a specific gene.
+
+    Args:
+        hexagon_df (pandas.DataFrame): DataFrame containing hexagon information.
+        hexagon_size (float): Size of the hexagons.
+        image_pixels_per_um (float): Number of image pixels per micrometer.
+        gene_name (str): Name of the gene being plotted.
+        dataset_name (str): Name of the dataset.
+        morans_i (float, optional): Moran's I value for the gene. Defaults to None.
+        save_plot (bool, optional): Whether to save the plot. Defaults to False.
+        output_folder (str, optional): Output folder for saving the plot. Defaults to None.
+
+    Returns:
+        str: HTML code for the generated hexagon plot.
+    """
+    
     fig, ax = plt.subplots(figsize=(3, 2.5))
     sc = ax.scatter(hexagon_df["x"], hexagon_df["y"], c=hexagon_df["counts"], cmap="viridis", s=2, alpha=0.6)
     for hx, hy in zip(hexagon_df["x"], hexagon_df["y"]):
         #Double check this and why there is the 0.865 division
         hexagon = RegularPolygon((hx, hy), numVertices=6, radius=hexagon_size * image_pixels_per_um / 0.865, alpha=0.2, edgecolor='k', orientation=np.pi / 2)
         ax.add_patch(hexagon)
     ax.set_xlim(0, max(hexagon_df["x"]))
@@ -1252,22 +1383,45 @@
     plt.close(fig)  # Close the plot to free memory
 
     return html_fig
 
 
 
 def get_probe_sums(matrix_joined):
+    """
+    Calculate the sum of counts for each probe.
+
+    Args:
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+
+    Returns:
+        pandas.DataFrame: DataFrame with the sum of counts for each probe.
+    """
     sums = matrix_joined.groupby("Gene_ID_y").sum()
     sums["Counts"] = np.log10(sums["Counts"])
     sums = sums[["Counts"]]
     sums.reset_index(inplace=True)
     return sums
 
 
 def plot_sums_to_html(sums1, sums2, dataset1_name, dataset2_name,save_plot=False,output_folder=None):
+    """
+    Generate an HTML plot comparing probe sums between two datasets.
+
+    Args:
+        sums1 (pandas.DataFrame): DataFrame containing probe sums for the first dataset.
+        sums2 (pandas.DataFrame): DataFrame containing probe sums for the second dataset.
+        dataset1_name (str): Name of the first dataset.
+        dataset2_name (str): Name of the second dataset.
+        save_plot (bool, optional): Whether to save the plot. Defaults to False.
+        output_folder (str, optional): Output folder for saving the plot. Defaults to None.
+
+    Returns:
+        str: HTML code for the generated plot comparing probe sums.
+    """
     common_probes = list(set(sums1["Gene_ID_y"]) & set(sums2["Gene_ID_y"]))
 
     if len(common_probes) < 20:
         fig, ax = plt.subplots(figsize=(4, 4))
         ax.text(0.5, 0.5, "Not enough overlapping probes", fontsize=12, ha='center')
         ax.axis('off')
 
@@ -1324,14 +1478,25 @@
         plt.close(fig)  # Close the plot to free memory
 
         return html_fig
 
 
 
 def plot_abundance_correlation_heatmap(replicates_data,save_plot=False,output_folder=None):
+    """
+    Generate an HTML heatmap plot showing the correlation of probe abundances between datasets.
+
+    Args:
+        replicates_data (list): List of dictionaries containing data for each replicate.
+        save_plot (bool, optional): Whether to save the plot. Defaults to False.
+        output_folder (str, optional): Output folder for saving the plot. Defaults to None.
+
+    Returns:
+        str: HTML code for the generated abundance correlation heatmap.
+    """
     # Calculate the sums of features for each replicate
     sums_data = []
     replicate_names = []
     for replicate_data in replicates_data:
         sums = get_probe_sums(replicate_data['matrix_joined'])
         sums_data.append(sums)
         replicate_names.append(replicate_data['dataset_name'])
@@ -1373,14 +1538,26 @@
         clustermap.savefig(f"{output_folder}/abundance_correlation_heatmap.svg", dpi=400)
 
     plt.close(clustermap.figure)
     return html_fig
 
 
 def get_df_for_gene(matrix_joined, tissue_positions_list, gene_name, normalised=False):
+    """
+    Get a DataFrame for a specific gene.
+
+    Args:
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+        tissue_positions_list (pandas.DataFrame): DataFrame containing tissue positions.
+        gene_name (str): Name of the gene to retrieve.
+        normalised (bool, optional): Whether to normalize the counts. Defaults to False.
+
+    Returns:
+        pandas.DataFrame: DataFrame containing information for the specified gene.
+    """
     matrix_subset = matrix_joined[matrix_joined["Gene_ID_y"] == gene_name]
     matrix_subset.reset_index(drop=True, inplace=True)
     x = tissue_positions_list["x"]
     y = tissue_positions_list["y"]
     counts = np.zeros(len(tissue_positions_list))
     for i in range(len(matrix_subset)):
         count = matrix_subset["Counts"][i]
@@ -1394,23 +1571,47 @@
 
         counts = np.append(counts, count)
     df = pd.DataFrame({"x": x, "y": y, "counts": counts})
     return df.sort_values("counts", ascending=False).drop_duplicates(subset=["x", "y"])
 
 
 def process_gene(gene, matrix_joined, tissue_positions_list):
+    """
+    Process a gene to calculate its Moran's I value.
+
+    Args:
+        gene (str): Name of the gene to process.
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+        tissue_positions_list (pandas.DataFrame): DataFrame containing tissue positions.
+
+    Returns:
+        dict: Dictionary containing the gene name and its Moran's I value.
+    """
     gene_df = get_df_for_gene(matrix_joined, tissue_positions_list, gene, normalised=True)
     points = [Point(xy) for xy in zip(gene_df['x'], gene_df['y'])]
     gene_gdf = gpd.GeoDataFrame(gene_df, geometry=points)
     w = weights.KNN.from_dataframe(gene_gdf, k=18)
     w.transform = 'R'
     mi = Moran(gene_df["counts"], w, permutations=0)
     return {"gene": gene, "Morans_I": mi.I}
 
 def get_morans_i(gene_name, matrix_joined, tissue_positions_list, max_workers=4):
+    """
+    Calculate Moran's I values for a specific gene or for all genes.
+
+    Args:
+        gene_name (str): Name of the gene to calculate Moran's I for. Use "all" to calculate for all genes.
+        matrix_joined (pandas.DataFrame): Joined matrix containing probe information.
+        tissue_positions_list (pandas.DataFrame): DataFrame containing tissue positions.
+        max_workers (int, optional): Number of workers to use for parallel processing. Defaults to 4.
+
+    Returns:
+        pandas.DataFrame or float: If gene_name is "all", returns a DataFrame with Moran's I values for all genes.
+                                   If gene_name is a specific gene, returns the Moran's I value for that gene.
+    """
 
     if gene_name == "all":
         unique_genes = matrix_joined["Gene_ID_y"].unique()
         #remove those unique genes which have less than total 100 counts
         #lowly_expressed_genes = matrix_joined.groupby("Gene_ID_y")["Counts"].sum()
         #lowly_expressed_genes = lowly_expressed_genes[lowly_expressed_genes<100].index.values
         unique_genes = [gene for gene in unique_genes] #if gene not in lowly_expressed_genes]
@@ -1477,14 +1678,28 @@
         w.transform = 'R'
         mi = esda.Moran(gene_df["counts"], w, permutations=0)
         return mi.I
 
 
 
 def plot_morans_i_to_html(morans_i1, morans_i2, dataset1_name, dataset2_name,save_plot=False,output_folder=None):
+    """
+    Generate an HTML plot comparing Moran's I values between two datasets.
+
+    Args:
+        morans_i1 (pandas.DataFrame): DataFrame containing Moran's I values for the first dataset.
+        morans_i2 (pandas.DataFrame): DataFrame containing Moran's I values for the second dataset.
+        dataset1_name (str): Name of the first dataset.
+        dataset2_name (str): Name of the second dataset.
+        save_plot (bool, optional): Whether to save the plot. Defaults to False.
+        output_folder (str, optional): Output folder for saving the plot. Defaults to None.
+
+    Returns:
+        str: HTML code for the generated plot comparing Moran's I values.
+    """
     common_probes = list(set(morans_i1["gene"]) & set(morans_i2["gene"]))
     if len(common_probes) < 20:
         fig, ax = plt.subplots(figsize=(4, 4))
         ax.text(0.5, 0.5, "Not enough overlapping probes", fontsize=12, ha='center')
         ax.axis('off')
 
         # Convert the plot to HTML
@@ -1534,14 +1749,25 @@
 
         plt.close(fig)  # Close the plot to free memory
 
         return html_fig
 
 
 def plot_morans_i_correlation_heatmap(replicates_data, save_plot=False,output_folder=None):
+    """
+    Generate an HTML heatmap plot showing the correlation of Moran's I values between datasets.
+
+    Args:
+        replicates_data (list): List of dictionaries containing data for each replicate.
+        save_plot (bool, optional): Whether to save the plot. Defaults to False.
+        output_folder (str, optional): Output folder for saving the plot. Defaults to None.
+
+    Returns:
+        str: HTML code for the generated Moran's I correlation heatmap.
+    """
     #get the morans i for each dataset
     morans_i_data = []
     replicate_names = []
     for replicate_data in replicates_data:
         morans_i = replicate_data["morans_i"]
         morans_i_data.append(morans_i)
         replicate_names.append(replicate_data['dataset_name'])
@@ -1581,14 +1807,17 @@
 
     plt.close(clustermap.figure)
     return html_fig
 
 
 
 def main():
+    """
+    Main function to parse command-line arguments and generate the QC report.
+    """
     parser = argparse.ArgumentParser(description="Generate QC report for Pseudovisium output.")
     parser.add_argument("--folders", "-f", nargs="+", help="List of folders containing Pseudovisium output", required=True)
     parser.add_argument("--output_folder", "-o", default="/Users/k23030440/", help="Output folder path")
     parser.add_argument("--gene_names", "-g", nargs="+", default=["RYR3", "AQP4", "THBS1"], help="List of gene names to plot")
     parser.add_argument("--include_morans_i", "-m", action="store_true", help="Include Moran's I features tab")
     parser.add_argument("-max_workers", "--mw", type=int, default=4, help="Number of workers to use for parallel processing")
     parser.add_argument("-normalisation","--n",action="store_true",help="Normalise the counts by the total counts per cell")
```

### Comparing `Pseudovisium-0.0.8/setup.py` & `Pseudovisium-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data'
 LONG_DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data, for more information see https://github.com/BKover99/pseudovisium'
 
 
 setup(
     name="Pseudovisium",
     version=VERSION,
     author="Bence Kover",
     author_email="<kover.bence@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['numpy','pandas', 'scanpy', 'squidpy', 'matplotlib'],
+    install_requires=[
+    'numpy',
+    'pandas',
+    'scipy',
+    'scanpy',
+    'squidpy',
+    'matplotlib',
+    'opencv-python',
+    'h5py',
+    'anndata',
+    'tifffile',
+    'tqdm',
+    'pysal',
+    'geopandas',
+    'seaborn',
+    'adjustText',
+    'shapely'
+        ],
+
     keywords=['spatial', 'transcriptomics', 'visium', 'xenium', 'cosmx'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X"
     ]
```

