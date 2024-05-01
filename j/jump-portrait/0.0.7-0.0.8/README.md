# Comparing `tmp/jump_portrait-0.0.7.tar.gz` & `tmp/jump_portrait-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jump_portrait-0.0.7.tar", max compression
+gzip compressed data, was "jump_portrait-0.0.8.tar", max compression
```

## Comparing `jump_portrait-0.0.7.tar` & `jump_portrait-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4786 2024-01-11 16:45:58.000000 jump_portrait-0.0.7/README.md
--rw-r--r--   0        0        0      783 2024-01-12 22:50:07.000000 jump_portrait-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        1 2023-12-20 04:47:29.000000 jump_portrait-0.0.7/src/jump_portrait/__init__.py
--rw-r--r--   0        0        0     8540 2024-01-12 21:26:08.000000 jump_portrait-0.0.7/src/jump_portrait/fetch.py
--rw-r--r--   0        0        0     1708 2024-01-12 22:50:03.000000 jump_portrait-0.0.7/src/jump_portrait/s3.py
--rw-r--r--   0        0        0     1755 2023-12-20 04:47:29.000000 jump_portrait-0.0.7/src/jump_portrait/save.py
--rw-r--r--   0        0        0     2620 2023-12-20 04:47:29.000000 jump_portrait-0.0.7/src/jump_portrait/utils.py
--rw-r--r--   0        0        0      762 2024-01-04 20:15:55.000000 jump_portrait-0.0.7/src/jump_portrait/workflow.py
--rw-r--r--   0        0        0     5680 1970-01-01 00:00:00.000000 jump_portrait-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     4786 2024-01-11 16:45:58.000000 jump_portrait-0.0.8/README.md
+-rw-r--r--   0        0        0      731 2024-01-18 19:27:17.000000 jump_portrait-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-12-20 04:47:29.000000 jump_portrait-0.0.8/src/jump_portrait/__init__.py
+-rw-r--r--   0        0        0    11298 2024-01-18 19:17:32.000000 jump_portrait-0.0.8/src/jump_portrait/fetch.py
+-rw-r--r--   0        0        0     1708 2024-01-12 22:50:03.000000 jump_portrait-0.0.8/src/jump_portrait/s3.py
+-rw-r--r--   0        0        0     1755 2023-12-20 04:47:29.000000 jump_portrait-0.0.8/src/jump_portrait/save.py
+-rw-r--r--   0        0        0     2620 2023-12-20 04:47:29.000000 jump_portrait-0.0.8/src/jump_portrait/utils.py
+-rw-r--r--   0        0        0      762 2024-01-04 20:15:55.000000 jump_portrait-0.0.8/src/jump_portrait/workflow.py
+-rw-r--r--   0        0        0     5721 1970-01-01 00:00:00.000000 jump_portrait-0.0.8/PKG-INFO
```

### Comparing `jump_portrait-0.0.7/README.md` & `jump_portrait-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jump_portrait-0.0.7/pyproject.toml` & `jump_portrait-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 [tool.poetry]
 name = "jump-portrait"
-version = "0.0.7"
+version = "0.0.8"
 description = "Tools to fetch and visualize JUMP images"
 authors = ["Alan Munoz"]
 readme = "README.md"
 packages = [{include = "jump_portrait", from= "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pooch = "^1.7.0"
-tqdm = "^4.66.1"
+boto3 = ">=1.33.1"
+broad-babel = "^0.1.7"
+fsspec = "^2023.12.1"
+joblib = "^1.3.2"
 matplotlib = "^3.8.2"
+pillow = "^10.2.0"
+polars = "^0.19.19"
+pooch = "^1.7.0"
 pyarrow = "^14.0.1"
-fsspec = "^2023.12.1"
 s3fs = "^2023.12.1"
-boto3 = ">=1.33.1"
 s3path = "^0.5.0"
-broad-babel = "^0.1.7"
-polars = "^0.19.19"
-joblib = "^1.3.2"
+tqdm = "^4.66.1"
 
 [tool.poetry.group.dev.dependencies]
-jupytext = "^1.15.0"
-ipdb = "^0.13.13"
-isort = "^5.12.0"
-black = "^23.7.0"
 biopython = "^1.81"
+csvkit = "^1.1.1"
 jupyter = "^1.0.0"
-tqdm = "^4.66.1"
+jupytext = "^1.15.0"
 pytest = "^7.4.1"
-csvkit = "^1.1.1"
 ruff-lsp = "^0.0.48"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `jump_portrait-0.0.7/src/jump_portrait/fetch.py` & `jump_portrait-0.0.8/src/jump_portrait/fetch.py`

 * *Files 24% similar despite different names*

```diff
@@ -123,25 +123,28 @@
     first_row = unique_site.row(0, named=True)
     s3_image_path = build_s3_image_path(
         row=first_row, channel=channel, correction=correction
     )
     return get_image_from_s3path(s3_image_path)
 
 
-def get_item_location_metadata(item_name: str, controls: bool = True) -> pl.DataFrame:
+def get_item_location_metadata(
+    item_name: str, controls: bool = True, **kwargs
+) -> pl.DataFrame:
     """
     First search for datasets in which this item was present.
     Return tuple with its Metadata location in order source, batch, plate,
     well and site.
     """
+    input_column = kwargs.get("input_column") or "standard_key"
 
     # Get plates
     jcp_ids = query.run_query(
         query=item_name,
-        input_column="standard_key",
+        input_column=input_column,
         output_column="JCP2022,standard_key",
     )
     jcp_item = {x[0]: x[1] for x in jcp_ids}
     meta_wells = get_table("well")
     # found_rows = meta_wells[meta_wells["Metadata_JCP2022"].isin(jcp_item)].copy()
     found_rows = meta_wells.filter(pl.col("Metadata_JCP2022").is_in(jcp_item.keys()))
     found_rows = found_rows.with_columns(pl.lit(item_name).alias("standard_key"))
@@ -176,25 +179,32 @@
         on=("Metadata_Source", "Metadata_Plate"),
     )
     return well_level_metadata
 
 
 def load_filter_well_metadata(well_level_metadata: pl.DataFrame) -> pl.DataFrame:
     """
-    well_level_metadata: pl.DataFrame
+    Filters a dataframe with well info. Loading and filtering happens in a threaded manner. Note that it does not check for whole row duplication.
+
+    Parameters
+    ----------
+    well_level_metadata : pl.DataFrame
         Contains the data
 
     Load metadata from a dataframe containing these columns
     - Metadata_Source
     - Metadata_Batch
     - Metadata_Plate
     - Metadata_Well
 
-    Loading and filtering happens in a threaded manner. Note that it does not check for duplication.
-    Returns the wells and
+
+    Returns
+    -------
+    pl.DataFrame
+        DataFrame with location of item
     """
     core_cols = (
         "Metadata_Source",
         "Metadata_Batch",
         "Metadata_Plate",
         "Metadata_PlateType",
     )
@@ -216,19 +226,14 @@
             map(lambda x: x["Metadata_Well"], groups),
         )
     )
     well_images_uri = parallel(iterable, get_well_image_uris)
 
     selected_uris = pl.concat(well_images_uri)
 
-    # uris_with_jcp = selected_uris.join(
-    #     well_level_metadata, on=(*core_cols[:3], "Metadata_Well")
-    # )
-
-    # return uris_with_jcp
     return selected_uris
 
 
 @batch_processing
 def get_well_image_uris(s3_location_uri, wells: list[str]) -> pl.DataFrame:
     # Returns a dataframe indicating the image location of specific wells for a given parquet file.
     locations_df = pl.read_parquet(s3_location_uri, use_pyarrow=True)
@@ -255,14 +260,103 @@
         DataFrame with location of item
 
     Examples
     --------
     FIXME: Add docs.
 
     """
-    well_level_metadata = get_item_location_metadata(item_name, controls=controls)
+    input_column = kwargs.get("input_column") or "standard_key"
+
+    well_level_metadata = get_item_location_metadata(
+        item_name, controls=controls, input_column=input_column
+    )
     item_selected_meta = load_filter_well_metadata(well_level_metadata, **kwargs)
     joint = item_selected_meta.join(
         well_level_metadata.drop("Metadata_Well"),
         on=("Metadata_Source", "Metadata_Batch", "Metadata_Plate"),
     )
     return joint.unique()
+
+
+def get_collage(
+    gene: str, channel: str = "DNA", plate_type: str = "ORF", **kwargs
+) -> np.ndarray:
+    """Return a collage of images from a given gene. Returned matrices are arranged in two rows,
+    top row are the perturbations and bottom rows are their plate-per-plate controls.
+
+    Parameters
+    ----------
+    gene : str
+        input gene in standard format
+    channel : str
+        Channel to plot. Default is "DNA".
+    plate_type : str
+        plate type, can be "ORF", "CRISPR" or "Compound". Default is "ORF".
+    **kwargs :
+        Arguments to pass to get_item_location_info
+
+    Returns
+    -------
+    np.ndarray
+        Concatenated array of dimensions (2,N) where N is the number of plates
+        in which the gene is present.
+
+    Examples
+    --------
+    FIXME: Add docs.
+
+    """
+    # Convenience variables
+    transient_col = "fullpath"
+    input_column = kwargs.get("input_column", "standard_key")
+    group_by_fields = (
+        "Metadata_Source",
+        "Metadata_Batch",
+        "Metadata_Plate",
+        "Metadata_PlateType",
+    )
+
+    # Find location
+    all_locations = get_item_location_info(gene)
+    image_locations = {}
+    for v in ("control", gene):
+        subdf = all_locations.filter(pl.col(input_column) == v)
+        subdf = subdf.select(reversed(subdf.columns)).with_columns(
+            pl.concat_str(f"^.*Orig{channel}.*$").alias(transient_col)
+        )
+        image_locations[v] = subdf.group_by(group_by_fields).agg(pl.col(transient_col))
+
+    # Merge gene and control dataframes
+    combined = image_locations[gene].join(
+        image_locations["control"],
+        on=group_by_fields[:-2],
+        suffix="_control",
+    )
+
+    combined = combined.filter(pl.col("Metadata_PlateType") == plate_type)
+
+    # Sample items
+    regex = "^fullpath.*$"
+    samples = combined.with_columns(pl.all().map_elements(len)).select(
+        pl.col(regex).map_elements(lambda x: np.random.randint(x))
+    )
+
+    base = combined.select(pl.col(regex)).to_numpy()
+
+    # Fetch the sampled indices from our data frame
+    x, y = samples.shape
+    locations = [["" for _ in range(y)] for _ in range(x)]
+    for i, gene_ctrl in enumerate(samples.to_numpy()):
+        for j, x in enumerate(gene_ctrl):
+            locations[i][j] = base[i, j][x]
+
+    # Reformat and concatenate
+    imgs = []
+    for plate in locations:
+        pair = []
+        for fpath in plate:
+            pair.append(get_image_from_s3path(fpath))
+        imgs.append(pair)
+
+    concat = np.concatenate([np.concatenate(x, axis=0) for x in imgs], axis=1)
+
+    return concat
```

### Comparing `jump_portrait-0.0.7/src/jump_portrait/s3.py` & `jump_portrait-0.0.8/src/jump_portrait/s3.py`

 * *Files identical despite different names*

### Comparing `jump_portrait-0.0.7/src/jump_portrait/save.py` & `jump_portrait-0.0.8/src/jump_portrait/save.py`

 * *Files identical despite different names*

### Comparing `jump_portrait-0.0.7/src/jump_portrait/utils.py` & `jump_portrait-0.0.8/src/jump_portrait/utils.py`

 * *Files identical despite different names*

### Comparing `jump_portrait-0.0.7/src/jump_portrait/workflow.py` & `jump_portrait-0.0.8/src/jump_portrait/workflow.py`

 * *Files identical despite different names*

### Comparing `jump_portrait-0.0.7/PKG-INFO` & `jump_portrait-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: jump-portrait
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools to fetch and visualize JUMP images
 Author: Alan Munoz
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.33.1)
 Requires-Dist: broad-babel (>=0.1.7,<0.2.0)
 Requires-Dist: fsspec (>=2023.12.1,<2024.0.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
+Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: polars (>=0.19.19,<0.20.0)
 Requires-Dist: pooch (>=1.7.0,<2.0.0)
 Requires-Dist: pyarrow (>=14.0.1,<15.0.0)
 Requires-Dist: s3fs (>=2023.12.1,<2024.0.0)
 Requires-Dist: s3path (>=0.5.0,<0.6.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/markdown
```

