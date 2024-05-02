# Comparing `tmp/maples_dr-0.1.0rc3.tar.gz` & `tmp/maples_dr-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maples_dr-0.1.0rc3.tar", last modified: Tue Apr 23 17:22:40 2024, max compression
+gzip compressed data, was "maples_dr-0.1.0rc4.tar", last modified: Thu May  2 17:26:30 2024, max compression
```

## Comparing `maples_dr-0.1.0rc3.tar` & `maples_dr-0.1.0rc4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 17:22:40.306679 maples_dr-0.1.0rc3/
--rw-r--r--   0 gaby      (1000) gaby      (1000)     7048 2023-12-21 00:27:55.000000 maples_dr-0.1.0rc3/LICENSE
--rw-r--r--   0 gaby      (1000) gaby      (1000)     4439 2024-04-23 17:22:40.306679 maples_dr-0.1.0rc3/PKG-INFO
--rw-r--r--   0 gaby      (1000) gaby      (1000)     3107 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/README.md
--rw-r--r--   0 gaby      (1000) gaby      (1000)     1561 2024-04-23 17:21:59.000000 maples_dr-0.1.0rc3/pyproject.toml
--rw-r--r--   0 gaby      (1000) gaby      (1000)       38 2024-04-23 17:22:40.306679 maples_dr-0.1.0rc3/setup.cfg
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 17:22:40.302679 maples_dr-0.1.0rc3/src/
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 17:22:40.303679 maples_dr-0.1.0rc3/src/maples_dr/
--rw-r--r--   0 gaby      (1000) gaby      (1000)      644 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/src/maples_dr/__init__.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     5829 2024-04-22 21:24:44.000000 maples_dr-0.1.0rc3/src/maples_dr/config.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)    37072 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/src/maples_dr/dataset.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)    26633 2024-04-23 14:57:47.000000 maples_dr-0.1.0rc3/src/maples_dr/loader.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     6605 2024-04-23 17:17:48.000000 maples_dr-0.1.0rc3/src/maples_dr/preprocessing.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     4018 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/src/maples_dr/quick_api.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)    16870 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/src/maples_dr/utilities.py
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 17:22:40.305679 maples_dr-0.1.0rc3/src/maples_dr.egg-info/
--rw-r--r--   0 gaby      (1000) gaby      (1000)     4439 2024-04-23 17:22:40.000000 maples_dr-0.1.0rc3/src/maples_dr.egg-info/PKG-INFO
--rw-r--r--   0 gaby      (1000) gaby      (1000)      590 2024-04-23 17:22:40.000000 maples_dr-0.1.0rc3/src/maples_dr.egg-info/SOURCES.txt
--rw-r--r--   0 gaby      (1000) gaby      (1000)        1 2024-04-23 17:22:40.000000 maples_dr-0.1.0rc3/src/maples_dr.egg-info/dependency_links.txt
--rw-r--r--   0 gaby      (1000) gaby      (1000)      219 2024-04-23 17:22:40.000000 maples_dr-0.1.0rc3/src/maples_dr.egg-info/requires.txt
--rw-r--r--   0 gaby      (1000) gaby      (1000)       10 2024-04-23 17:22:40.000000 maples_dr-0.1.0rc3/src/maples_dr.egg-info/top_level.txt
-drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-04-23 17:22:40.305679 maples_dr-0.1.0rc3/tests/
--rw-r--r--   0 gaby      (1000) gaby      (1000)    10142 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/tests/test_maples_dr_cache.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)      266 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/tests/test_maples_dr_config.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     5995 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/tests/test_maples_dr_dataset.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)     1207 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/tests/test_maples_dr_download.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)      757 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/tests/test_maples_dr_fundus.py
--rw-r--r--   0 gaby      (1000) gaby      (1000)      462 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc3/tests/test_maples_dr_quickapi.py
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-05-02 17:26:30.335414 maples_dr-0.1.0rc4/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     7048 2023-12-21 00:27:55.000000 maples_dr-0.1.0rc4/LICENSE
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     4580 2024-05-02 17:26:30.335414 maples_dr-0.1.0rc4/PKG-INFO
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     3216 2024-04-23 17:58:15.000000 maples_dr-0.1.0rc4/README.md
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     1593 2024-05-02 15:34:48.000000 maples_dr-0.1.0rc4/pyproject.toml
+-rw-r--r--   0 gaby      (1000) gaby      (1000)       38 2024-05-02 17:26:30.336414 maples_dr-0.1.0rc4/setup.cfg
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-05-02 17:26:30.328415 maples_dr-0.1.0rc4/src/
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-05-02 17:26:30.330414 maples_dr-0.1.0rc4/src/maples_dr/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      829 2024-05-02 15:34:24.000000 maples_dr-0.1.0rc4/src/maples_dr/__init__.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     5805 2024-04-29 16:33:19.000000 maples_dr-0.1.0rc4/src/maples_dr/config.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    41349 2024-05-02 16:09:22.000000 maples_dr-0.1.0rc4/src/maples_dr/dataset.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    26606 2024-04-29 16:33:19.000000 maples_dr-0.1.0rc4/src/maples_dr/loader.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     6605 2024-04-23 17:58:15.000000 maples_dr-0.1.0rc4/src/maples_dr/preprocessing.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     4713 2024-04-29 16:33:19.000000 maples_dr-0.1.0rc4/src/maples_dr/quick_api.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    16870 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc4/src/maples_dr/utilities.py
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-05-02 17:26:30.333414 maples_dr-0.1.0rc4/src/maples_dr.egg-info/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     4580 2024-05-02 17:26:30.000000 maples_dr-0.1.0rc4/src/maples_dr.egg-info/PKG-INFO
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      590 2024-05-02 17:26:30.000000 maples_dr-0.1.0rc4/src/maples_dr.egg-info/SOURCES.txt
+-rw-r--r--   0 gaby      (1000) gaby      (1000)        1 2024-05-02 17:26:30.000000 maples_dr-0.1.0rc4/src/maples_dr.egg-info/dependency_links.txt
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      219 2024-05-02 17:26:30.000000 maples_dr-0.1.0rc4/src/maples_dr.egg-info/requires.txt
+-rw-r--r--   0 gaby      (1000) gaby      (1000)       10 2024-05-02 17:26:30.000000 maples_dr-0.1.0rc4/src/maples_dr.egg-info/top_level.txt
+drwxr-xr-x   0 gaby      (1000) gaby      (1000)        0 2024-05-02 17:26:30.333414 maples_dr-0.1.0rc4/tests/
+-rw-r--r--   0 gaby      (1000) gaby      (1000)    10142 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc4/tests/test_maples_dr_cache.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      266 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc4/tests/test_maples_dr_config.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     7567 2024-04-29 16:33:19.000000 maples_dr-0.1.0rc4/tests/test_maples_dr_dataset.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)     1221 2024-04-29 16:33:19.000000 maples_dr-0.1.0rc4/tests/test_maples_dr_download.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      757 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc4/tests/test_maples_dr_fundus.py
+-rw-r--r--   0 gaby      (1000) gaby      (1000)      462 2024-04-22 20:38:53.000000 maples_dr-0.1.0rc4/tests/test_maples_dr_quickapi.py
```

### Comparing `maples_dr-0.1.0rc3/LICENSE` & `maples_dr-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc3/PKG-INFO` & `maples_dr-0.1.0rc4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: maples-dr
-Version: 0.1.0rc3
-Summary: Utilities python library for the public dataset: MAPLES-DR.
+Version: 0.1.0rc4
+Summary: Utilities python library for the public dataset of retinal structures: MAPLES-DR.
 Author-email: Gabriel Lepetit-Aimon <gabriel.lepetit-aimon@polymtl.ca>
-Project-URL: Homepage, https://liv4d.github.io/MAPLES-DR/en/welcome/maples_dr
-Project-URL: Documentation, https://liv4d.github.io/MAPLES-DR/en/
+Project-URL: Homepage, https://liv4d.github.io/MAPLES-DR/en/
+Project-URL: Documentation, https://liv4d.github.io/MAPLES-DR/en/welcome/python_library.html
 Project-URL: Source, https://github.com/LIV4D/MAPlES-DR
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: pandas
@@ -32,16 +32,18 @@
 Requires-Dist: sphinx-intl; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # MAPLES-DR
 
+[![Version](https://img.shields.io/pypi/v/maples_dr.svg?logo=pypi)](https://pypi.python.org/pypi/maples_dr)
 [![doc](https://github.com/LIV4D/MAPLES-DR/actions/workflows/documentation.yml/badge.svg?branch=dev)](https://liv4d.github.io/MAPLES-DR/en/)
 
+
 **MAPLES-DR _(MESSIDOR Anatomical and Pathological Labels for Explainable Screening of Diabetic Retinopathy)_** is a public dataset which provides diagnoses for DR and ME as well as pixel-wise segmentation maps for 10 retinal structures for 198 images of MESSIDOR. This repository provides a python library of utility codes to ease the use of the database.
 
 ## MAPLES-DR Dataset Content
 ![Overview of the content of the MAPLES-DR dataset.](docs/source/_static/MAPLES-DR_Overview.svg)
 
 MAPLES-DR dataset is available for download on [figshare](https://doi.org/10.6084/m9.figshare.24328660). The fundus images are not included in MAPLES-DR but one can download them from [MESSIDOR Consortium's website](https://www.adcis.net/fr/logiciels-tiers/messidor-fr/).
```

### Comparing `maples_dr-0.1.0rc3/README.md` & `maples_dr-0.1.0rc4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # MAPLES-DR
 
+[![Version](https://img.shields.io/pypi/v/maples_dr.svg?logo=pypi)](https://pypi.python.org/pypi/maples_dr)
 [![doc](https://github.com/LIV4D/MAPLES-DR/actions/workflows/documentation.yml/badge.svg?branch=dev)](https://liv4d.github.io/MAPLES-DR/en/)
 
+
 **MAPLES-DR _(MESSIDOR Anatomical and Pathological Labels for Explainable Screening of Diabetic Retinopathy)_** is a public dataset which provides diagnoses for DR and ME as well as pixel-wise segmentation maps for 10 retinal structures for 198 images of MESSIDOR. This repository provides a python library of utility codes to ease the use of the database.
 
 ## MAPLES-DR Dataset Content
 ![Overview of the content of the MAPLES-DR dataset.](docs/source/_static/MAPLES-DR_Overview.svg)
 
 MAPLES-DR dataset is available for download on [figshare](https://doi.org/10.6084/m9.figshare.24328660). The fundus images are not included in MAPLES-DR but one can download them from [MESSIDOR Consortium's website](https://www.adcis.net/fr/logiciels-tiers/messidor-fr/).
```

### Comparing `maples_dr-0.1.0rc3/pyproject.toml` & `maples_dr-0.1.0rc4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 
 name = "maples-dr"
-version = '0.1.0rc3'
+version = '0.1.0rc4'
 authors = [
     {name= 'Gabriel Lepetit-Aimon', email= 'gabriel.lepetit-aimon@polymtl.ca'},
 ]
-description = """Utilities python library for the public dataset: MAPLES-DR."""
+description = """Utilities python library for the public dataset of retinal structures: MAPLES-DR."""
 readme = 'README.md'
 
 requires-python = '>=3.10'
 dependencies = [
     'numpy',
     'Pillow',
     'pandas',
@@ -38,16 +38,16 @@
     'ipython',
 ]
 test = [
     'pytest',
 ]
 
 [project.urls]
-Homepage = 'https://liv4d.github.io/MAPLES-DR/en/welcome/maples_dr'
-Documentation = 'https://liv4d.github.io/MAPLES-DR/en/'
+Homepage = 'https://liv4d.github.io/MAPLES-DR/en/'
+Documentation = 'https://liv4d.github.io/MAPLES-DR/en/welcome/python_library.html'
 Source = 'https://github.com/LIV4D/MAPlES-DR'
 
 
 [build-system]
 requires = ["wheel", "setuptools", "numpy"]
 build-backend = "setuptools.build_meta"
```

### Comparing `maples_dr-0.1.0rc3/src/maples_dr/config.py` & `maples_dr-0.1.0rc4/src/maples_dr/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 
     #: Preprocessing based on median filtering.
     #:
     #: See :func:`maples_dr.preprocessing.median_preprocessing`.
     MEDIAN = "median"
 
 
-DOWNLOAD = "DOWNLOAD"
-
-
 @dataclass
 class DatasetConfig:
     """
     Dataclass storing the configuration of the dataset.
     """
 
     #: Size of the generated images.
```

### Comparing `maples_dr-0.1.0rc3/src/maples_dr/dataset.py` & `maples_dr-0.1.0rc4/src/maples_dr/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -242,20 +242,20 @@
 
     #: The Macular Edema.
     ME = "me"
 
 
 #: The name of a valid image field in MAPLES-DR.
 #:
-#: This type alias is a union of :class:`BiomarkerField` and :class:`FundusField`.
+#: This type alias is a union of :class:`BiomarkerField <maples_dr.dataset.BiomarkerField>` and :class:`FundusField <,maples_dr.dataset.FundusField>`.
 ImageField: TypeAlias = Union[FundusField, BiomarkerField]
 
 #: The name of a valid field in MAPLES-DR.
 #:
-#: This type alias is a union of :class:`DiagnosisField`, :class:`BiomarkerField`, and :class:`FundusField`.
+#: This type alias is a union of :class:`DiagnosisField <maples_dr.dataset.DiagnosisField>`, :class:`BiomarkerField <maples_dr.dataset.BiomarkerField>`, and :class:`FundusField <maples_dr.dataset.FundusField>`.
 Field: TypeAlias = Union[DiagnosisField, ImageField]
 
 
 def check_field(field: Field | str) -> Field:
     try:
         return DiagnosisField.parse(field)
     except ValueError:
@@ -279,15 +279,15 @@
 
 class Dataset(Sequence):
     """A set of samples from the MAPLES-DR dataset.
 
     Datasets are a utility class to access and export samples from the MAPLES-DR dataset.
 
     They are equivalent to a list of samples, each sample being stored as a dictionary­.
-    See :obj:`Field` for the list of available fields.
+    See :class:`Field <maples_dr.dataset.Field>` for the list of available fields.
     """
 
     def __init__(self, data: pd.DataFrame, cfg: DatasetConfig, messidor_rois: pd.DataFrame):
         """Create a new dataset. (Internal use only)
 
         :meta private:
 
@@ -328,31 +328,26 @@
             assert "W" in messidor_rois.columns, "Missing 'W' column in the MESSIDOR ROIs dataframe."
             assert "H" in messidor_rois.columns, "Missing 'H' column in the MESSIDOR ROIs dataframe."
         self._rois: pd.DataFrame = messidor_rois
 
     def __getitem__(self, idx: int | str | slice[int] | list[str]) -> DataSample:
         """Get a sample from the dataset.
 
-        This method is a shortcut for :meth:`read_sample`.
-        It returns the sample as a dictionary with the keys:
+        The sample is returned as a :class:`DataSample <maples_dr.dataset.DataSample>`.
 
-        - ``name`` containing the name of the image (e.g. "20051116_44816_0400_PP").
-        - every :class:`Field` except ``bright_lesions`` and ``red_lesions``.
-
-        The image are formatted following the default configuration (see :func:`maples_dr.configure`).
 
         Parameters
         ----------
         idx : int | str
             Index of the sample. Can be an integer or the name of the sample (e.g. "20051116_44816_0400_PP").
 
         Returns
         -------
-        dict
-            The sample as a dictionary.
+        DataSample
+            The sample.
         """
         if isinstance(idx, (str, int)):
             sample_infos = self.get_sample_infos(idx)
             rois = self._rois.loc[sample_infos.name]
             return DataSample(sample_infos, self._cfg, rois)
         elif isinstance(idx, slice):
             return self.subset(start=idx.start, end=idx.stop, step=idx.step)
@@ -372,18 +367,19 @@
         return len(self._data)
 
     @property
     def data(self) -> pd.DataFrame:
         """The data of the dataset.
 
         A dataframe containing the information of each sample. It has the following columns:
+
             - index: the name of the sample.
             - ``fundus``: the path to the fundus image.
-            - [:class:`BiomarkerField`] (accept aggregated): the path to the biomarkers masks.
-            - [:class:`BiomarkersAnnotationTasks` ``_`` :class:`BiomarkersAnnotationInfos`]: the additional annotations informations.
+            - :class:`BiomarkerField <maples_dr.dataset.BiomarkerField>` (accept aggregated): the path to the biomarkers masks.
+            - :class:`BiomarkersAnnotationTasks <maples_dr.dataset.BiomarkersAnnotationTasks>` _ :class:`BiomarkersAnnotationInfos <maples_dr.dataset.BiomarkersAnnotationInfos>`: the additional annotations informations.
             - ``dr``: the consensus DR grade.
             - ``me``: the consensus ME grade.
             - ``dr_{A|B|C}``: the DR grade given by one retinologist.
             - ``me_{A|B|C}``: the ME grade given by one retinologist.
             - ``dr_{A|B|C}_comment``: comments from the retinologist when grading the DR diagnosis.
         """
         return self._data
@@ -604,28 +600,26 @@
 
         for field in fields.values():
             field_folder = path / field
             field_folder.mkdir(parents=True, exist_ok=True)
 
         with RichProgress.iteration("Exporting Maples-DR...", len(self), "Maples-DR exported in {t} seconds.") as p:
             for i in range(len(self)):
-                sample = self.read_sample(i, list(fields.keys()), image_format="PIL")
+                sample = self[i]
 
-                for field, img in sample.items():
-                    if field not in fields:
-                        continue
-
-                    field_folder = path / fields[field]
+                for field, folder in fields.items():
+                    field_folder = path / folder
 
                     opt = {}
                     if field not in ("fundus", "raw_fundus"):
                         opt["bits "] = 1
                         opt["optimize"] = optimize
 
-                    img.save(field_folder / f"{sample['name']}.png", **opt)
+                    img = sample.read_field(field, image_format=ImageFormat.PIL)
+                    img.save(field_folder / f"{sample.name}.png", **opt)
                     p.update(1 / len(fields))
 
 
 class DataSample(Mapping):
     """A sample from the MAPLES-DR dataset.
 
     A sample is a dictionary containing the information of a single sample from the dataset.
@@ -644,25 +638,71 @@
         self._roi: Rect = Rect.from_points(int(roi["y0"]), int(roi["x0"]), int(roi["y1"]), int(roi["x1"]))
         self._messidor_shape: Point = Point(int(roi["H"]), int(roi["W"]))
 
     def __len__(self) -> int:
         return len(self._data)
 
     def __getitem__(self, key: Field | str) -> Union[Image.Image, np.ndarray, str]:
-        key = check_field(key)
-        if isinstance(key, BiomarkerField):
-            return self.read_biomarker(key)
-        elif isinstance(key, DiagnosisField):
-            return self._data[key.value]
-        elif key is FundusField.FUNDUS:
-            return self.read_fundus()
-        elif key is FundusField.RAW_FUNDUS:
-            return self.read_fundus(preprocess=False)
-        elif key is FundusField.MASK:
-            return self.read_roi_mask()
+        return self.read_field(field=key)
+
+    def read_field(
+        self,
+        field: Field | str,
+        image_format: Optional[ImageFormat] = None,
+        resize: Optional[int | bool] = None,
+        pre_annotation: bool = False,
+    ):
+        """Read one field of the sample.
+
+        This function is similar to __getitem__ but provides more options to format the result (resize, image format...).
+
+        Parameters
+        ----------
+        field : Field | str
+            Any field from:
+
+            - :class:`BiomarkerField <maples_dr.dataset.BiomarkerField>`: a biomarker name, possible values are: ``'opticCup'``, ``'opticDisc'``, ``'macula'``, ``'vessels'``, ``'brightLesions'``, ``'cottonWoolSpots'``, ``'drusens'``, ``'exudates'``, ``'brightUncertains'``, ``'redLesions'``, ``'hemorrhages'``, ``'microaneurysms'``, ``'neovascularization'``, ``'redUncertains'``.
+            - :class:`DiagnosisField <maples_dr.dataset.DiagnosisField>`: a diagnosis name, possible values are: ``'dr'``, ``'me'``.
+            - :class:`FundusField <maples_dr.dataset.FundusField>`: a fundus field, possible values are: ``'fundus'``, ``'rawFundus'``, ``'mask'``.
+
+        image_format :
+            Format of the image to return.
+
+            If ``None`` (by default), use the format defined in the configuration.
+
+        resize :
+            Resize the image to the given size.
+
+            - If ``resize`` is an int, crop the image to a square ROI and resize it to the shape ``(resize, resize)``;
+            - If ``True``, keep the original MAPLES-DR resolution of 1500x1500 px;
+            - If ``False``, use the original MESSIDOR resolution if MESSIDOR path is configured, otherwise fallback to MAPLES-DR original resolution.
+            - If ``None`` (by default), use the size defined in the configuration.
+
+        pre_annotation :
+            If set to ``True``, read the pre-annotation biomarkers instead of the final ones.
+
+            .. warning::
+                Only hemorrhages, microaneurysms, exudates and vessels have pre-annotations.
+
+        Returns
+        -------
+        Image.Image | np.ndarray | str
+            The field under the format specified.
+        """
+        field = check_field(field)
+        if isinstance(field, BiomarkerField):
+            return self.read_biomarker(field, image_format=image_format, resize=resize, pre_annotation=pre_annotation)
+        elif isinstance(field, DiagnosisField):
+            return self._data[field.value]
+        elif field is FundusField.FUNDUS:
+            return self.read_fundus(image_format=image_format, resize=resize)
+        elif field is FundusField.RAW_FUNDUS:
+            return self.read_fundus(image_format=image_format, resize=resize, preprocess=False)
+        elif field is FundusField.MASK:
+            return self.read_roi_mask(image_format=image_format, resize=resize)
 
     def __iter__(self) -> Generator[Field]:
         if FundusField.FUNDUS.value in self._data:
             if self._cfg.preprocessing != Preprocessing.NONE:
                 yield FundusField.RAW_FUNDUS
             yield [FundusField.FUNDUS]
 
@@ -686,20 +726,24 @@
         no_cache: bool = False,
     ) -> any:
         """Read a biomarker from the sample.
 
         Parameters
         ----------
         biomarkers :
-            Name of the biomarker(s) to read.
+            Name of the biomarker(s) to read. Possible values are: ``'opticCup'``, ``'opticDisc'``, ``'macula'``,
+            ``'vessels'``, ``'brightLesions'``, ``'cottonWoolSpots'``, ``'drusens'``, ``'exudates'``,
+            ``'brightUncertains'``, ``'redLesions'``, ``'hemorrhages'``, ``'microaneurysms'``,
+            ``'neovascularization'``, ``'redUncertains'`` (see :class:`BiomarkerField <maples_dr.dataset.BiomarkerField>` for more details).
 
             If multiple biomarkers are given, the corresponding masks will be merged.
 
         image_format :
-            Format of the image to return.
+            Format of the image to return. Possible values are: ``'PIL'``, ``'BGR'`` or ``'RGB'``
+            (see :class:`ImageFormat <maples_dr.config.ImageFormat>` for more details.).
 
             If ``None`` (by default), use the format defined in the configuration.
 
         resize :
             Resize the image to the given size.
 
             - If ``resize`` is an int, crop the image to a square ROI and resize it to the shape ``(resize, resize)``;
@@ -822,18 +866,22 @@
     ):
         """
         Read multiple biomarkers at once, assigning a class to a biomarker or a group of them.
 
         Parameters
         ----------
         biomarkers :
-            Name of the biomarker(s) to read.
+            Name of the biomarker(s) to read. Possible values are: ``'opticCup'``, ``'opticDisc'``, ``'macula'``,
+            ``'vessels'``, ``'brightLesions'``, ``'cottonWoolSpots'``, ``'drusens'``, ``'exudates'``,
+            ``'brightUncertains'``, ``'redLesions'``, ``'hemorrhages'``, ``'microaneurysms'``,
+            ``'neovascularization'``, ``'redUncertains'`` (see :class:`BiomarkerField <maples_dr.dataset.BiomarkerField>` for more details).
 
         image_format :
-            Format of the image to return.
+            Format of the image to return. Possible values are: ``'PIL'``, ``'BGR'`` or ``'RGB'``
+            (see :class:`ImageFormat <maples_dr.config.ImageFormat>` for more details.).
 
             If None (by default), use the format defined in the configuration.
 
         pre_annotation :
             If set to ``True``, read the pre-annotation biomarkers instead of the final ones.
 
             .. warning::
@@ -863,20 +911,21 @@
         """Read the fundus image of the sample.
 
         Parameters
         ----------
         preprocess :
             Preprocessing to apply to the image.
 
-            - If a :class:`maples_dr.config.Preprocessing` (or an equivalent string), the image is preprocessed with the given preprocessing;
+            - If a :class:`Preprocessing <maples_dr.config.Preprocessing>` (or an equivalent string), the image is preprocessed with the given preprocessing;
             - if ``False``, the image is not preprocessed.
             - if ``None`` (by default) or ``True``, use the preprocessing defined in the configuration.
 
         image_format :
-            Format of the image to return.
+            Format of the image to return. Possible values are: ``'PIL'``, ``'BGR'`` or ``'RGB'``
+            (see :class:`ImageFormat <maples_dr.config.ImageFormat>` for more details.).
 
             If ``None`` (by default), use the format defined in the configuration.
 
         resize :
             Resize the image to the given size.
 
             - If ``resize`` is an int, crop the image to a square ROI and resize it to the shape ``(resize, resize)``;
@@ -948,29 +997,42 @@
             fundus_format = ImageFormat.BGR
             self._fundus = fundus
 
             fundus = preprocess_fundus(fundus, preprocess)
 
         return self._apply_image_format(fundus, fundus_format, image_format)
 
-    def read_roi_mask(self, image_format: Optional[ImageFormat] = None) -> np.ndarray | Image.Image:
+    def read_roi_mask(
+        self, image_format: Optional[ImageFormat] = None, resize: Optional[int | bool] = None
+    ) -> np.ndarray | Image.Image:
         """Read the region of interest of the fundus image.
 
         Parameters
         ----------
 
         image_format :
-            Format of the image to return. If None, use the format defined in the configuration.
+            Format of the image to return. Possible values are: ``'PIL'``, ``'BGR'`` or ``'RGB'``
+            (see :class:`ImageFormat <maples_dr.config.ImageFormat>` for more details.).
+
+            If ``None`` (by default), use the format defined in the configuration.
+
+        resize :
+            Resize the image to the given size.
+
+            - If ``resize`` is an int, crop the image to a square ROI and resize it to the shape ``(resize, resize)``;
+            - If ``True``, use the original MAPLES-DR resolution of 1500x1500 px;
+            - If ``False``, keep the original MESSIDOR resolution.
+            - If ``None`` (by default), use the size defined in the configuration.
 
         Returns
         -------
         np.ndarray
             The region of interest of the fundus image.
         """
-        fundus = self.read_fundus(preprocess=False, image_format=ImageFormat.BGR)
+        fundus = self.read_fundus(preprocess=False, image_format=ImageFormat.BGR, resize=resize)
         mask = fundus_roi(fundus)
 
         return self._apply_image_format(mask, ImageFormat.BGR, image_format)
 
     def _apply_image_format(
         self, image: Image.Image | np.ndarray, input_format: ImageFormat, target_format: str | ImageFormat | None
     ) -> Image.Image | np.ndarray:
```

### Comparing `maples_dr-0.1.0rc3/src/maples_dr/loader.py` & `maples_dr-0.1.0rc4/src/maples_dr/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from urllib.request import urlopen
 from zipfile import ZipFile
 
 import pandas as pd
 import yaml
 
 from .config import (
-    DOWNLOAD,
     DatasetConfig,
     ImageFormat,
     InvalidConfigError,
     Preprocessing,
 )
 from .dataset import (
     BiomarkerField,
@@ -32,14 +31,17 @@
 #   === CONSTANTS ===
 # Figshare public urls of the MAPLES DR dataset
 MAPLES_DR_ADDITIONAL_URL = "https://figshare.com/ndownloader/files/45795384"
 
 #: Unset constant
 UNSET = "UNSET"
 
+#: Persistent cache constant
+DOWNLOAD_CACHE = xdg_data_home() / "maples_dr" / "AdditionalData"
+
 
 class DatasetSubset(str, Enum):
     """Enumeration of the possible subsets of the MAPLES-DR dataset."""
 
     #: The training set (138 images)
     TRAIN = "train"
 
@@ -57,17 +59,15 @@
 
 
 class NotConfiguredError(Exception):
     """
     Exception raised when the dataset loader is not configured.
     """
 
-    def __init__(
-        self, message: str = "MAPLES-DR dataset is not configured yet.", *args
-    ):
+    def __init__(self, message: str = "MAPLES-DR dataset is not configured yet.", *args):
         super().__init__(message, *args)
 
 
 class DatasetLoader:
     """
     Loader for MAPLES-DR dataset.
     """
@@ -78,15 +78,16 @@
             image_format="PIL",
             preprocessing="none",
         )
         self.dataset_record: Optional[dict] = None
         self._maples_dr_path: Optional[Path] = None
         self._diagnosis: Optional[pd.DataFrame] = None
         self._annotations_infos: Optional[Dict[str, pd.DataFrame]] = None
-        self._is_maples_dr_folder_temporary: bool = False
+        self._exclude_missing_macula = False
+        self._exclude_missing_cup = False
 
         self._messidor_paths: Optional[dict[str, str]] = None
         self._messidor_ROIs: Optional[pd.DataFrame] = None
 
     def __del__(self):
         if self._is_maples_dr_folder_temporary:
             rmtree(self._maples_dr_path, ignore_errors=True)
@@ -97,14 +98,16 @@
         maples_dr_path: Optional[str | Path] = UNSET,
         messidor_path: Optional[str | Path] = UNSET,
         *,
         cache: Optional[str | Path] = UNSET,
         resize: Optional[int] = None,
         image_format: Optional[ImageFormat] = None,
         preprocessing: Optional[Preprocessing] = None,
+        exclude_missing_macula: Optional[bool] = None,
+        exclude_missing_cup: Optional[bool] = None,
         disable_check: bool = False,
     ):
         """Configure the default behavior of the MAPLES-DR dataset.
 
         Any parameters left to None (or 'UNSET' for the first two paths) will leave the current configuration unaffected.
 
         Parameters
@@ -144,39 +147,50 @@
             Preprocessing algorithm applied on the fundus images.
 
             By default, no preprocessing is applied.
 
         disable_check : bool, optional
             If True, disable the integrity check of the dataset.
 
+        exclude_missing_macula : bool, optional
+            If True, exclude images with missing macula segmentation (one image of the train set).
+
+            By default: False.
+
+        exclude_missing_cup : bool, optional
+            If True, exclude images with missing optic cup segmentation (4 images of the train set, 2 of the test set).
+
+            By default: False.
+
         """
         # === Update the dataset configuration ===
         self._datasets_config.update(
             dict(
                 resize=resize,
                 image_format=image_format,
                 preprocessing=preprocessing,
             )
         )
+        if exclude_missing_macula is not None:
+            self._exclude_missing_macula = exclude_missing_macula
+        if exclude_missing_cup is not None:
+            self._exclude_missing_cup = exclude_missing_cup
 
         # === Set Maples-DR cache ===
         if cache is not UNSET and self.cfg._cache != cache:
             cache = self._change_cache_path(cache)
         else:
             cache = self.cfg.cache_path
 
         # === Prepare Maples-DR ===
-        # If configure is called the first time with no path, download the dataset or use the cache.
-        if maples_dr_path is UNSET and self._maples_dr_path is None:
-            if cache is None:
-                maples_dr_path = DOWNLOAD
-            else:
-                maples_dr_path = cache / "AdditionalData"
+        if (maples_dr_path is not UNSET and self._maples_dr_path != maples_dr_path) or self._maples_dr_path is None:
+            # If configure is called the first time with no path, download the dataset or use the cache.
+            if maples_dr_path is UNSET:
+                maples_dr_path = None
 
-        if maples_dr_path is not UNSET and self._maples_dr_path != maples_dr_path:
             # Set the path and download the dataset if needed.
             maples_dr_path = self._change_maples_dr_path(maples_dr_path)
 
             # Load the dataset infos.
             (
                 self.dataset_record,
                 self._messidor_ROIs,
@@ -189,25 +203,19 @@
             if not disable_check:
                 self.check_maples_dr_integrity(
                     path=maples_dr_path,
                     biomarkers=list(self.dataset_record["biomarkers"]),
                     images_names=self.image_names(DatasetSubset.ALL_WITH_DUPLICATES),
                 )
 
-            self._diagnosis = self.load_maples_dr_diagnosis(
-                maples_dr_path / "diagnosis_infos.xls"
-            )
+            self._diagnosis = self.load_maples_dr_diagnosis(maples_dr_path / "diagnosis_infos.xls")
 
         # === Prepare MESSIDOR ===
         if messidor_path is UNSET:
-            if (
-                self._messidor_paths is None
-                and cache is not None
-                and (cache / "MESSIDOR").is_dir()
-            ):
+            if self._messidor_paths is None and cache is not None and (cache / "MESSIDOR").is_dir():
                 messidor_path = cache / "MESSIDOR"
 
         if messidor_path is not UNSET:
             if messidor_path is None:
                 self._messidor_paths = None
             else:
                 self._messidor_paths = self.discover_messidor_images(
@@ -218,14 +226,21 @@
     def clear_cache(self):
         """
         Clear the cache.
         """
         if self.cfg.cache_path is not None:
             rmtree(self.cfg.cache_path, ignore_errors=True)
 
+    @staticmethod
+    def clear_download_cache():
+        """
+        Clear the cache where the MAPLES-DR archive is downloaded and extracted.
+        """
+        rmtree(DOWNLOAD_CACHE, ignore_errors=True)
+
     @property
     def cfg(self) -> DatasetConfig:
         """
         Return the default configuration of the loaded dataset.
         """
         return self._datasets_config
 
@@ -260,17 +275,15 @@
         previous_cache = self.cfg.cache_path
         if previous_cache is not None and path.absolute() == previous_cache.absolute():
             return path
 
         # If a cache already existed, copy the MAPLES-DR original dataset to the new cache path.
         if previous_cache is not None:
             if (previous_cache / "AdditionalData").is_dir():
-                shutil.copytree(
-                    previous_cache / "AdditionalData", path / "AdditionalData"
-                )
+                shutil.copytree(previous_cache / "AdditionalData", path / "AdditionalData")
             if (previous_cache / "MESSIDOR").is_dir():
                 shutil.copytree(previous_cache / "MESSIDOR", path / "MESSIDOR")
 
         self.cfg._cache = path
         return path
 
     # --- Maples-DR path configuration ---
@@ -283,89 +296,79 @@
             raise NotConfiguredError()
         return self._maples_dr_path
 
     def _change_maples_dr_path(self, path: Optional[str | Path] = None) -> Path:
         """
         Return the path to the MAPLES-DR dataset folder.
         """
-        # If Maples-DR was previously downloaded, delete the temporary folder.
-        if self._is_maples_dr_folder_temporary and self._maples_dr_path is not None:
-            rmtree(self._maples_dr_path, ignore_errors=True)
-            self._is_maples_dr_folder_temporary = False
-
         self._maples_dr_path = None
 
-        if path is None or path is DOWNLOAD:
-            # If no path is given, prepare the dataset download to...
-            path = mkdtemp()
-            self._is_maples_dr_folder_temporary = True
+        if path is None:
+            # If the cache is enabled, prepare the dataset download to the cache folder.
+            path = DOWNLOAD_CACHE
 
         path = Path(path)
 
-        if path.is_dir():
-            # === If the path is a directory ===
-            # Ensure it exists ...
-            if not path.exists():
-                path.mkdir(parents=True)
-            # and check if the folder contains the dataset record.
-            if not (path / "dataset_record.yaml").exists():
-                # If not, download the dataset.
-                zip_path = path / "maples_dr.zip"
-                download(MAPLES_DR_ADDITIONAL_URL, zip_path, "MAPLES-DR labels")
-                with ZipFile(path / "maples_dr.zip", "r") as zip_file:
-                    zip_file.extractall(path)
-                (path / "maples_dr.zip").unlink()
-
-        elif path.name.endswith(".zip"):
-            # === If the path is a zip file, unzip it to a temporary folder ===
+        if path.suffix == ".zip":
+            # === If the path is a zip file, unzip it to a cache folder ===
             zip_path = path
             if not zip_path.exists():
-                raise InvalidConfigError(
-                    f"Invalid Maples DR archive: {zip_path} doesn't exist."
-                )
+                raise InvalidConfigError(f"Invalid Maples DR archive: {zip_path} doesn't exist.")
 
-            # Create a temporary folder.
+            # Select the appropriate cache folder
             if self.cfg.cache_path is not None:
                 path = self.cfg.cache_path / "AdditionalData"
             else:
-                path = Path(mkdtemp())
+                path = DOWNLOAD_CACHE
+                path.mkdir(parents=True, exist_ok=True)
+
             # Unzip the dataset to the temporary folder.
             try:
                 with ZipFile(zip_path, "r") as zip_file:
                     zip_file.extractall(path)
             except Exception as e:
                 raise InvalidConfigError(
-                    f"Invalid Maples DR archive: {zip_path}:"
-                    "\n\t the provided archive is impossible to unzip."
+                    f"Invalid Maples DR archive: {zip_path}:" "\n\t the provided archive is impossible to unzip."
                 ) from e
-            else:
-                # Test if the zip file contains maples_dr folder.
-                if not (path / "dataset_record.yaml").exists():
-                    raise InvalidConfigError(
-                        f"Invalid Maples DR archive:  {path}:"
-                        '\n\t the provided archive doesn\'t contains the file "dataset_record.yaml".'
-                    )
-                if not (path / "MESSIDOR-ROIs.csv").exists():
-                    raise InvalidConfigError(
-                        f"Invalid Maples DR archive:  {path}:"
-                        '\n\t the provided archive doesn\'t contains the file "MESSIDOR-ROIs.csv".'
-                    )
-                if not (path / "diagnosis_infos.xls").exists():
-                    raise InvalidConfigError(
-                        f"Invalid Maples DR archive:  {path}:"
-                        '\n\t the provided archive doesn\'t contains the file "diagnosis_infos.xls".'
-                    )
-
-                if not (path / "biomarkers_annotation_infos.xls").exists():
-                    raise InvalidConfigError(
-                        f"Invalid Maples DR archive:  {path}:"
-                        '\n\t the provided archive doesn\'t contains the file "biomarkers_annotation_infos.xls".'
-                    )
-            if self.cfg.cache_path is not None:
-                self._is_maples_dr_folder_temporary = True
+
+        else:
+            # === If the path is a directory ===
+            # Ensure it exists ...
+            path.mkdir(parents=True, exist_ok=True)
+            # and check if the folder contains the dataset record.
+            if not (path / "dataset_record.yaml").exists():
+                # If not, download the dataset.
+                zip_path = path / "additional_data.zip"
+                download(MAPLES_DR_ADDITIONAL_URL, zip_path, "MAPLES-DR labels")
+                with ZipFile(path / "additional_data.zip", "r") as zip_file:
+                    zip_file.extractall(path)
+                (path / "additional_data.zip").unlink()
+
+        # Test if the final path contains maples_dr files.
+        if not (path / "dataset_record.yaml").exists():
+            raise InvalidConfigError(
+                f"Invalid Maples DR archive:  {path}:"
+                '\n\t the provided archive doesn\'t contains the file "dataset_record.yaml".'
+            )
+        if not (path / "MESSIDOR-ROIs.csv").exists():
+            raise InvalidConfigError(
+                f"Invalid Maples DR archive:  {path}:"
+                '\n\t the provided archive doesn\'t contains the file "MESSIDOR-ROIs.csv".'
+            )
+        if not (path / "diagnosis_infos.xls").exists():
+            raise InvalidConfigError(
+                f"Invalid Maples DR archive:  {path}:"
+                '\n\t the provided archive doesn\'t contains the file "diagnosis_infos.xls".'
+            )
+
+        if not (path / "biomarkers_annotation_infos.xls").exists():
+            raise InvalidConfigError(
+                f"Invalid Maples DR archive:  {path}:"
+                '\n\t the provided archive doesn\'t contains the file "biomarkers_annotation_infos.xls".'
+            )
 
         self._maples_dr_path = path
         return path
 
     @staticmethod
     def load_dataset_record_and_rois(path: str | Path) -> Tuple[Dict, Dict]:
         """
@@ -411,30 +414,26 @@
             infos = annotation_infos_data[sheet_name][biomarker_infos].copy()
             infos["Time"] = pd.to_timedelta(infos["Time"])
             infos = infos.rename(
                 columns={
                     "Retinologist": task + "_" + BiomarkersAnnotationInfos.RETINOLOGIST,
                     "Comment": task + "_" + BiomarkersAnnotationInfos.COMMENT,
                     "Time": task + "_" + BiomarkersAnnotationInfos.ANNOTATION_TIME,
-                    "Annotation #": task
-                    + "_"
-                    + BiomarkersAnnotationInfos.ANNOTATION_ID,
+                    "Annotation #": task + "_" + BiomarkersAnnotationInfos.ANNOTATION_ID,
                 },
             )
 
             if annotation_infos is None:
                 annotation_infos = infos
             else:
                 annotation_infos = annotation_infos.join(infos)
 
         return annotation_infos
 
-    def check_maples_dr_integrity(
-        self, path: Path, biomarkers: list[str], images_names: list[str]
-    ):
+    def check_maples_dr_integrity(self, path: Path, biomarkers: list[str], images_names: list[str]):
         """
         Check if the MAPLES-DR dataset contains all segmentation maps.
         """
         missing_images = 0
         for biomarker in biomarkers:
             for img in images_names:
                 if (
@@ -470,17 +469,15 @@
             .astype(str)
             .replace("nan", "")
         )
         return dr_diagnosis.join(me_diagnosis).join(dr_me_comments)
 
     # --- MESSIDOR path configuration ---
     @staticmethod
-    def discover_messidor_images(
-        images: list[str], path: Optional[str | Path] = None
-    ) -> Dict[str, Path]:
+    def discover_messidor_images(images: list[str], path: Optional[str | Path] = None) -> Dict[str, Path]:
         """
         Discover the MESSIDOR images corresponding to the given MAPLES-DR images.
 
         :param images: List of MAPLES-DR images names. The image name should not contain the extension.
         :param path: Path to the MESSIDOR dataset.
         """
         path = Path(path)
@@ -489,17 +486,15 @@
         if not path.is_dir():
             raise InvalidConfigError(f"Invalid MESSIDOR path: {path} is not a folder.")
 
         # Scan the MESSIDOR subfolders and list images.
 
         # Scan MESSIDOR subfolders to find each MAPLES-DR images.
         missing_images = set(images)
-        for img_path in chain.from_iterable(
-            path.glob(f"**/*.{ext}") for ext in ("tif", "jpg", "png")
-        ):
+        for img_path in chain.from_iterable(path.glob(f"**/*.{ext}") for ext in ("tif", "jpg", "png")):
             try:
                 missing_images.remove(img_path.stem)
             except KeyError:
                 pass
             else:
                 messidor_paths[img_path.stem] = img_path.absolute()
                 if len(missing_images) == 0:
@@ -525,57 +520,49 @@
                             try:
                                 missing_images.remove(img_stem)
                             except KeyError:
                                 continue
 
                             zip_info.filename = img_filename
                             zip_file.extract(zip_info, unzip_folder)
-                            messidor_paths[img_stem] = (
-                                unzip_folder / img_filename
-                            ).absolute()
+                            messidor_paths[img_stem] = (unzip_folder / img_filename).absolute()
 
                             progress.update(1)
                             if len(missing_images) == 0:
                                 return messidor_paths
 
         # If some images are still missing, raise an error.
         raise InvalidConfigError(
             f"The provided folder to the MESSIDOR dataset is incomplete: "
             f"{len(missing_images)} images included in MAPLES-DR are missing."
         )
 
     # === DATASETS FACTORIES ===
-    def load_dataset(
-        self, subset: DatasetSubset | str | list[str] = DatasetSubset.ALL
-    ) -> Dataset:
+    def load_dataset(self, subset: DatasetSubset | str | list[str] = DatasetSubset.ALL) -> Dataset:
         """
         Return the MAPLES-DR dataset.
 
         :param subset: Subset of the dataset to return. If None, return the whole dataset.
                        Must be either None, "train" or "test" or a list of valid image name.
         """
         if not self.is_configured():
             self.configure()
         if isinstance(subset, list):
             # Check that all images are valid.
             valid_images = set(self.image_names(DatasetSubset.ALL_WITH_DUPLICATES))
             for img in subset:
                 if img not in valid_images:
-                    raise ValueError(
-                        f"Invalid image name: {img} is not a valid image name."
-                    )
+                    raise ValueError(f"Invalid image name: {img} is unknown.")
             names = subset
         else:
             names = self.image_names(subset)
 
         paths = {}
         if self._messidor_paths is not None:
-            paths[FundusField.FUNDUS.value] = [
-                self._messidor_paths[name] for name in names
-            ]
+            paths[FundusField.FUNDUS.value] = [self._messidor_paths[name] for name in names]
 
         biomarkers_folder = {
             BiomarkerField.BRIGHT_UNCERTAINS.value: "BrightUncertains",
             BiomarkerField.COTTON_WOOL_SPOTS.value: "CottonWoolSpots",
             BiomarkerField.DRUSENS.value: "Drusens",
             BiomarkerField.EXUDATES.value: "Exudates",
             BiomarkerField.HEMORRHAGES.value: "Hemorrhages",
@@ -585,29 +572,25 @@
             BiomarkerField.OPTIC_CUP.value: "OpticCup",
             BiomarkerField.OPTIC_DISC.value: "OpticDisc",
             BiomarkerField.RED_UNCERTAINS.value: "RedUncertains",
             BiomarkerField.VESSELS.value: "Vessels",
         }
         for bio, bio_folder in biomarkers_folder.items():
             folder = self.maples_dr_folder / "annotations" / bio_folder
-            paths[bio] = [
-                folder / (n + ".png") if self.is_biomarker_segmented(bio, n) else None
-                for n in names
-            ]
+            paths[bio] = [folder / (n + ".png") if self.is_biomarker_segmented(bio, n) else None for n in names]
 
         preannotations_folder = {
             BiomarkerField.EXUDATES.value: "Exudates",
             BiomarkerField.HEMORRHAGES.value: "Hemorrhages",
             BiomarkerField.MICROANEURYSMS.value: "Microaneurysms",
             BiomarkerField.VESSELS.value: "Vessels",
         }
         for bio, bio_folder in preannotations_folder.items():
             paths[bio + "_pre"] = [
-                self.maples_dr_folder / "preannotations" / bio_folder / (name + ".png")
-                for name in names
+                self.maples_dr_folder / "preannotations" / bio_folder / (name + ".png") for name in names
             ]
 
         data = pd.DataFrame(paths, index=names)
 
         # Add the diagnosis and annotations infos.
         data = data.join(self._diagnosis).join(self._annotations_infos)
 
@@ -649,23 +632,27 @@
             DatasetSubset.TEST,
             DatasetSubset.ALL,
             DatasetSubset.ALL_WITH_DUPLICATES,
         ):
             names += self.dataset_record["test"]
         if subset in (DatasetSubset.DUPLICATES, DatasetSubset.ALL_WITH_DUPLICATES):
             names += list(self.dataset_record["duplicates"].values())
+
+        if self._exclude_missing_cup:
+            names = [name for name in names if name not in self.dataset_record["no_cup"]]
+        if self._exclude_missing_macula:
+            names = [name for name in names if name not in self.dataset_record["no_macula"]]
+
         if extension:
             if isinstance(extension, bool):
                 extension = "png"
             names = [name + "." + extension for name in names]
         return names
 
-    def is_biomarker_segmented(
-        self, biomarker: BiomarkerField | str, name: str
-    ) -> bool:
+    def is_biomarker_segmented(self, biomarker: BiomarkerField | str, name: str) -> bool:
         """
         Check if the given biomarker is segmented in the MAPLES-DR dataset.
 
         .. note::
 
             The macula segmentation is missing for one image centered on the optic disc.
 
@@ -683,35 +670,27 @@
         -------
         bool
             True if the biomarker is segmented, False otherwise.
         """
         if not self.is_configured():
             raise NotConfiguredError()
         biomarker = BiomarkerField.parse(biomarker)
-        if (
-            biomarker is BiomarkerField.MACULA
-            and name in self.dataset_record["no_macula"]
-        ):
+        if biomarker is BiomarkerField.MACULA and name in self.dataset_record["no_macula"]:
             return False
-        if (
-            biomarker is BiomarkerField.OPTIC_CUP
-            and name in self.dataset_record["no_cup"]
-        ):
+        if biomarker is BiomarkerField.OPTIC_CUP and name in self.dataset_record["no_cup"]:
             return False
         return True
 
 
 GLOBAL_LOADER = DatasetLoader()
 
 
 def download(url: str, path: str | Path, description: Optional[str] = None):
     """
     Download the file at the given url to the given path.
     """
     response = urlopen(url)
-    with RichProgress.download(
-        description, byte_size=int(response.info()["Content-length"])
-    ) as progress:
+    with RichProgress.download(description, byte_size=int(response.info()["Content-length"])) as progress:
         with open(path, "wb") as dest_file:
             for data in iter(partial(response.read, 32768), b""):
                 dest_file.write(data)
                 progress.update(len(data))
```

### Comparing `maples_dr-0.1.0rc3/src/maples_dr/preprocessing.py` & `maples_dr-0.1.0rc4/src/maples_dr/preprocessing.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc3/src/maples_dr/quick_api.py` & `maples_dr-0.1.0rc4/src/maples_dr/quick_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 __all__ = ["configure", "export_test_set", "export_train_set", "load_test_set", "load_train_set"]
 from pathlib import Path
 from typing import Dict, List, Optional
 
 from .dataset import Dataset, ImageField
-from .loader import DatasetLoader
+from .loader import DatasetLoader, DatasetSubset
 
 GLOBAL_LOADER = DatasetLoader()
 
 configure = GLOBAL_LOADER.configure
 
 
 def load_train_set() -> Dataset:
-    """Load the training set in memory.
+    """Load the training set.
 
     MAPLES-DR training set contains labels of pathological and anatomical structures for 138 fundus images.
     The dataset is return as a :class:`Dataset` object, which is equivalent to a list of samples.
     Each sample being stored as a dictionary with the following fields:
 
     - ``"fundus"``: The fundus image. (MESSIDOR path must have been configured!)
 
@@ -48,28 +48,46 @@
     >>> maples_dr.configure(messidor_path="path/to/messidor.zip")
     >>> train_set = maples_dr.load_train_set()
     >>> for sample in train_set:
     >>>     fundus = sample["fundus"]           # The fundus image
     >>>     vessels = sample["vessels"]         # The vessels mask
     >>>     dr = sample["dr"]                   # The Diabetic Retinopathy grade
     """
-    return GLOBAL_LOADER.load_dataset("train")
+    return GLOBAL_LOADER.load_dataset(DatasetSubset.TRAIN)
 
 
 def load_test_set() -> Dataset:
-    """Load the testing set in memory.
+    """Load the testing set.
 
     See :func:`load_train_set` for more details.
 
     Returns
     -------
     Dataset
         The testing set.
     """
-    return GLOBAL_LOADER.load_dataset("test")
+    return GLOBAL_LOADER.load_dataset(DatasetSubset.TEST)
+
+
+def load_dataset(subset: DatasetSubset | str | list[str] = DatasetSubset.ALL) -> Dataset:
+    """Load specific subset of the dataset (by default load the whole dataset without the duplicates).
+
+    Parameters
+    ----------
+    subset :
+        The subset to load (see :class:`DatasetSubset` for the available options), or a list of image names.
+
+
+
+    Returns
+    -------
+    Dataset
+        The corresponding subset of MAPLES-DR. See :func:`load_train_set` for more details on the data format.
+    """
+    return GLOBAL_LOADER.load_dataset(subset)
 
 
 def export_train_set(
     path: str | Path, fields: Optional[ImageField | List[ImageField] | Dict[ImageField, str]] = None
 ) -> None:
     """Save the training set to a folder.
 
@@ -117,7 +135,12 @@
     """
     return GLOBAL_LOADER.load_dataset("test").export(path, fields)
 
 
 def clear_cache():
     """Clear the cache directory."""
     return GLOBAL_LOADER.clear_cache()
+
+
+def clear_download_cache():
+    """Clear the download cache directory."""
+    return GLOBAL_LOADER.clear_download_cache()
```

### Comparing `maples_dr-0.1.0rc3/src/maples_dr/utilities.py` & `maples_dr-0.1.0rc4/src/maples_dr/utilities.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc3/src/maples_dr.egg-info/PKG-INFO` & `maples_dr-0.1.0rc4/src/maples_dr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: maples-dr
-Version: 0.1.0rc3
-Summary: Utilities python library for the public dataset: MAPLES-DR.
+Version: 0.1.0rc4
+Summary: Utilities python library for the public dataset of retinal structures: MAPLES-DR.
 Author-email: Gabriel Lepetit-Aimon <gabriel.lepetit-aimon@polymtl.ca>
-Project-URL: Homepage, https://liv4d.github.io/MAPLES-DR/en/welcome/maples_dr
-Project-URL: Documentation, https://liv4d.github.io/MAPLES-DR/en/
+Project-URL: Homepage, https://liv4d.github.io/MAPLES-DR/en/
+Project-URL: Documentation, https://liv4d.github.io/MAPLES-DR/en/welcome/python_library.html
 Project-URL: Source, https://github.com/LIV4D/MAPlES-DR
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: pandas
@@ -32,16 +32,18 @@
 Requires-Dist: sphinx-intl; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # MAPLES-DR
 
+[![Version](https://img.shields.io/pypi/v/maples_dr.svg?logo=pypi)](https://pypi.python.org/pypi/maples_dr)
 [![doc](https://github.com/LIV4D/MAPLES-DR/actions/workflows/documentation.yml/badge.svg?branch=dev)](https://liv4d.github.io/MAPLES-DR/en/)
 
+
 **MAPLES-DR _(MESSIDOR Anatomical and Pathological Labels for Explainable Screening of Diabetic Retinopathy)_** is a public dataset which provides diagnoses for DR and ME as well as pixel-wise segmentation maps for 10 retinal structures for 198 images of MESSIDOR. This repository provides a python library of utility codes to ease the use of the database.
 
 ## MAPLES-DR Dataset Content
 ![Overview of the content of the MAPLES-DR dataset.](docs/source/_static/MAPLES-DR_Overview.svg)
 
 MAPLES-DR dataset is available for download on [figshare](https://doi.org/10.6084/m9.figshare.24328660). The fundus images are not included in MAPLES-DR but one can download them from [MESSIDOR Consortium's website](https://www.adcis.net/fr/logiciels-tiers/messidor-fr/).
```

### Comparing `maples_dr-0.1.0rc3/src/maples_dr.egg-info/SOURCES.txt` & `maples_dr-0.1.0rc4/src/maples_dr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc3/tests/test_maples_dr_cache.py` & `maples_dr-0.1.0rc4/tests/test_maples_dr_cache.py`

 * *Files identical despite different names*

### Comparing `maples_dr-0.1.0rc3/tests/test_maples_dr_download.py` & `maples_dr-0.1.0rc4/tests/test_maples_dr_download.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     local_loader.configure(
         maples_dr_path="examples/PATH/TO/MAPLES-DR/AdditionalData.zip",
     )
     return local_loader.load_dataset("all_with_duplicates")
 
 
 def test_download(local_dataset):
-    downloaded_dataset = maples_dr.quick_api.GLOBAL_LOADER.load_dataset("all_with_duplicates")
+    maples_dr.clear_download_cache()
+
+    downloaded_dataset = maples_dr.load_dataset("all_with_duplicates")
 
     # === Check data content ===
     # Biomarkers
     for local_sample, downloaded_sample in zip(local_dataset, downloaded_dataset, strict=True):
         for biomarker in Bio:
             assert (
                 local_sample[biomarker] == downloaded_sample[biomarker]
```

### Comparing `maples_dr-0.1.0rc3/tests/test_maples_dr_fundus.py` & `maples_dr-0.1.0rc4/tests/test_maples_dr_fundus.py`

 * *Files identical despite different names*

