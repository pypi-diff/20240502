# Comparing `tmp/blending_toolkit-1.0.0b7.tar.gz` & `tmp/blending_toolkit-1.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blending_toolkit-1.0.0b7.tar", max compression
+gzip compressed data, was "blending_toolkit-1.0.0b8.tar", max compression
```

## Comparing `blending_toolkit-1.0.0b7.tar` & `blending_toolkit-1.0.0b8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1178 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/LICENSE
--rw-r--r--   0        0        0     4721 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/README.md
--rw-r--r--   0        0        0      601 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/__init__.py
--rw-r--r--   0        0        0    17521 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/blend_batch.py
--rw-r--r--   0        0        0     2480 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/blend_generator.py
--rw-r--r--   0        0        0     5623 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/catalog.py
--rw-r--r--   0        0        0    26203 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/deblend.py
--rw-r--r--   0        0        0    25983 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/draw_blends.py
--rw-r--r--   0        0        0    13914 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/match.py
--rw-r--r--   0        0        0     5398 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/measure.py
--rw-r--r--   0        0        0      139 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/__init__.py
--rw-r--r--   0        0        0     1449 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/base.py
--rw-r--r--   0        0        0     2171 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/detection.py
--rw-r--r--   0        0        0     2417 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/reconstruction.py
--rw-r--r--   0        0        0     1314 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/segmentation.py
--rw-r--r--   0        0        0     4704 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/utils.py
--rw-r--r--   0        0        0     2588 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/multiprocess.py
--rw-r--r--   0        0        0     1191 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/plotting.py
--rw-r--r--   0        0        0    24700 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/sampling_functions.py
--rw-r--r--   0        0        0     9325 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/survey.py
--rw-r--r--   0        0        0      889 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/utils.py
--rw-r--r--   0        0        0     4193 2024-04-16 16:10:29.041516 blending_toolkit-1.0.0b7/pyproject.toml
--rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 blending_toolkit-1.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1178 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/LICENSE
+-rw-r--r--   0        0        0     4718 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/README.md
+-rw-r--r--   0        0        0      601 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/__init__.py
+-rw-r--r--   0        0        0    17521 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/blend_batch.py
+-rw-r--r--   0        0        0     2480 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/blend_generator.py
+-rw-r--r--   0        0        0     5623 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/catalog.py
+-rw-r--r--   0        0        0    27255 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/deblend.py
+-rw-r--r--   0        0        0    26010 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/draw_blends.py
+-rw-r--r--   0        0        0    15597 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/match.py
+-rw-r--r--   0        0        0     6360 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/measure.py
+-rw-r--r--   0        0        0      139 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/metrics/__init__.py
+-rw-r--r--   0        0        0     1449 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/metrics/base.py
+-rw-r--r--   0        0        0     2171 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/metrics/detection.py
+-rw-r--r--   0        0        0     2417 2024-05-02 14:52:05.471352 blending_toolkit-1.0.0b8/btk/metrics/reconstruction.py
+-rw-r--r--   0        0        0     1428 2024-05-02 14:52:05.475352 blending_toolkit-1.0.0b8/btk/metrics/segmentation.py
+-rw-r--r--   0        0        0     4704 2024-05-02 14:52:05.475352 blending_toolkit-1.0.0b8/btk/metrics/utils.py
+-rw-r--r--   0        0        0     2588 2024-05-02 14:52:05.475352 blending_toolkit-1.0.0b8/btk/multiprocess.py
+-rw-r--r--   0        0        0     1348 2024-05-02 14:52:05.475352 blending_toolkit-1.0.0b8/btk/plotting.py
+-rw-r--r--   0        0        0    24700 2024-05-02 14:52:05.475352 blending_toolkit-1.0.0b8/btk/sampling_functions.py
+-rw-r--r--   0        0        0     9294 2024-05-02 14:52:05.475352 blending_toolkit-1.0.0b8/btk/survey.py
+-rw-r--r--   0        0        0      889 2024-05-02 14:52:05.475352 blending_toolkit-1.0.0b8/btk/utils.py
+-rw-r--r--   0        0        0     4215 2024-05-02 14:52:32.275537 blending_toolkit-1.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0     5934 1970-01-01 00:00:00.000000 blending_toolkit-1.0.0b8/PKG-INFO
```

### Comparing `blending_toolkit-1.0.0b7/LICENSE` & `blending_toolkit-1.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/README.md` & `blending_toolkit-1.0.0b8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 ```
 
 ## Installation
 
 BTK is pip installable, with the following command:
 
 ```bash
-pip install blending-toolkit==1.0.0b7
+pip install --pre blending-toolkit
 ```
 
 In case of any issues and for details of required packages, please see the more detailed installation instructions [here](https://lsstdesc.org/BlendingToolKit/install.html).
 
 ## Contributing
 
 Everyone can contribute to this project, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) document for details.
```

### Comparing `blending_toolkit-1.0.0b7/btk/__init__.py` & `blending_toolkit-1.0.0b8/btk/__init__.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/blend_batch.py` & `blending_toolkit-1.0.0b8/btk/blend_batch.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/blend_generator.py` & `blending_toolkit-1.0.0b8/btk/blend_generator.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/catalog.py` & `blending_toolkit-1.0.0b8/btk/catalog.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/deblend.py` & `blending_toolkit-1.0.0b8/btk/deblend.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     MultiResolutionBlendBatch,
 )
 from btk.draw_blends import DrawBlendsGenerator
 from btk.multiprocess import multiprocess
 
 
 class Deblender(ABC):
-    """Abstract base class containing the measure class for BTK.
+    """Abstract base class containing the deblender class for BTK.
 
-    Each new measure class should be a subclass of Measure.
+    Each new deblender class should be a subclass of Deblender.
     """
 
     def __init__(self, max_n_sources: int) -> None:
         """Initialize the Deblender class.
 
         Args:
             max_n_sources: Maximum number of sources returned by the deblender.
@@ -67,15 +67,15 @@
             blend_batch: Instance of `BlendBatch` class
 
         Returns:
             Instance of `DeblendedExample` class
         """
 
     def batch_call(self, blend_batch: BlendBatch, njobs: int = 1, **kwargs) -> DeblendBatch:
-        """Implements the call of a measure function on the entire batch.
+        """Implements the call of the deblender on the entire batch.
 
         Overwrite this function if you perform measurments on the batch.
         The default fucntionality is to use multiprocessing to speed up
         the iteration over all examples in the batch.
 
         Args:
             blend_batch: Instance of `BlendBatch` class
@@ -156,15 +156,15 @@
             mr_batch: Instance of `MultiResolutionBlendBatch` class
 
         Returns:
             Instance of `DeblendedExample` class
         """
 
     def batch_call(self, mr_batch: MultiResolutionBlendBatch, njobs: int = 1) -> DeblendBatch:
-        """Implements the call of a measure function on the entire batch.
+        """Implements the call of the deblender on the entire batch.
 
         Overwrite this function if you perform measurments on a batch.
         The default fucntionality is to use multiprocessing to speed up
         the iteration over all examples in the batch.
 
         Args:
             mr_batch: Instance of `MultiResolutionBlendBatch` class
@@ -188,49 +188,57 @@
     band index. If use_mean feature is used, then the Deblender will use
     the average of all the bands.
     """
 
     def __init__(
         self,
         max_n_sources: int,
+        sky_level: float,
         threshold_scale: int = 5,
         min_distance: int = 2,
         use_mean: bool = False,
         use_band: Optional[int] = None,
     ) -> None:
         """Initializes Deblender class. Exactly one of 'use_mean' or 'use_band' must be specified.
 
         Args:
             max_n_sources: See parent class.
-            threshold_scale: Minimum intensity of peaks.
+            sky_level: Background intensity in images to be detected (assumed constant).
+            threshold_scale: Minimum number of sigmas above noise level for detections.
             min_distance: Minimum distance in pixels between two peaks.
             use_mean: Flag to use the band average for deblending.
             use_band: Integer index of the band to use for deblending
         """
         super().__init__(max_n_sources)
         self.min_distance = min_distance
         self.threshold_scale = threshold_scale
+        self.sky_level = sky_level
 
         if use_band is None and not use_mean:
             raise ValueError("Either set 'use_mean=True' OR indicate a 'use_band' index")
         if use_band is not None and use_mean:
             raise ValueError("Only one of the parameters 'use_band' and 'use_mean' has to be set")
         self.use_mean = use_mean
         self.use_band = use_band
 
     def deblend(self, ii: int, blend_batch: BlendBatch) -> DeblendExample:
         """Performs deblending on the ii-th example from the batch."""
         blend_image = blend_batch.blend_images[ii]
         image = np.mean(blend_image, axis=0) if self.use_mean else blend_image[self.use_band]
 
         # compute threshold value
-        threshold = self.threshold_scale * np.std(image)
+        threshold = self.threshold_scale * np.sqrt(self.sky_level)
 
         # calculate coordinates
-        coordinates = peak_local_max(image, min_distance=self.min_distance, threshold_abs=threshold)
+        coordinates = peak_local_max(
+            image,
+            min_distance=self.min_distance,
+            threshold_abs=threshold,
+            num_peaks=self.max_n_sources,
+        )
         x, y = coordinates[:, 1], coordinates[:, 0]
 
         # convert coordinates to ra, dec
         wcs = blend_batch.wcs
         ra, dec = wcs.pixel_to_world_values(x, y)
         ra *= 3600
         dec *= 3600
@@ -336,26 +344,26 @@
             1,  # single band is returned
             blend_batch.image_size,
             segmentation_exp,
             deblended_images[:, None].clip(0),  # add a channel dimension
         )
 
 
-class SepMultiband(Deblender):
+class SepMultiBand(Deblender):
     """This class returns centers detected with SEP by combining predictions in different bands.
 
     For each band in the input image we run `sep` for detection and append new detections
     to a running list of detected coordinates. In order to avoid repeating detections,
     we run a KD-Tree algorithm to calculate the angular distance between each new
     coordinate and its closest neighbour. Then we discard those new coordinates that
     were closer than `matching_threshold` to any one of already detected coordinates.
     """
 
     def __init__(self, max_n_sources: int, matching_threshold: float = 1.0, thresh: float = 1.5):
-        """Initialize the SepMultiband Deblender.
+        """Initialize the SepMultiBand Deblender.
 
         Args:
             max_n_sources: See parent class.
             matching_threshold: Threshold value for match detections that are close (arcsecs).
             thresh: See `SepSingleBand` class.
         """
         super().__init__(max_n_sources)
@@ -384,14 +392,20 @@
             # run source extractor
             band_image = image[band]
             bkg = sep.Background(band_image)
             catalog = sep.extract(
                 band_image, self.thresh, err=bkg.globalrms, segmentation_map=False
             )
 
+            if len(catalog) > self.max_n_sources:
+                raise ValueError(
+                    "SEP predicted more sources than `max_n_sources`. Consider increasing `thresh`"
+                    " or `max_n_sources`."
+                )
+
             # convert predictions to arcseconds
             ra_detections, dec_detections = wcs.pixel_to_world_values(catalog["x"], catalog["y"])
             ra_detections *= 3600
             dec_detections *= 3600
 
             # convert to sky coordinates
             c1 = SkyCoord(ra=ra_detections * units.arcsec, dec=dec_detections * units.arcsec)
@@ -443,14 +457,21 @@
 
         This class uses the scarlet deblender to deblend the images. We follow the basic
         implementation that is layed out in the Scarlet documentation:
         https://pmelchior.github.io/scarlet/0-quickstart.html. For more details on each
         of the argument also see the Scarlet API at:
         https://pmelchior.github.io/scarlet/api/scarlet.initialization.html.
 
+        Note that as of commit 45187fd, Scarlet raises a `LinAlg` error if two sources are on
+        the same pixel, which is allowed by the majority of currently implemented sampling
+        functions in BTK. To get around this, our Deblender implementation automatically
+        catches this exception and outputs an array of zeroes for the deblended images of the
+        particular blend that caused this exception. See this issue for details:
+        https://github.com/pmelchior/scarlet/issues/282#issuecomment-2074886534
+
         Args:
             max_n_sources: See parent class.
             thresh: Multiple of the backround RMS used as a flux cutoff for morphology
                 initialization for `scarlet.source.ExtendedSource` class. (Default: 1.0)
             e_rel: Relative error for convergence of the loss function
                 See `scarlet.blend.Blend.fit` method for details. (Default: 1e-5)
             max_iter: Maximum number of iterations for the optimization (Default: 200)
@@ -647,10 +668,10 @@
         }
         return blend_batch, deblended_output
 
 
 available_deblenders = {
     "PeakLocalMax": PeakLocalMax,
     "SepSingleBand": SepSingleBand,
-    "SepMultiBand": SepMultiband,
+    "SepMultiBand": SepMultiBand,
     "Scarlet": Scarlet,
 }
```

### Comparing `blending_toolkit-1.0.0b7/btk/draw_blends.py` & `blending_toolkit-1.0.0b8/btk/draw_blends.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,16 @@
 
     def _get_psf_from_survey(self, survey: Survey) -> List[galsim.GSObject]:
         # make PSF and WCS
         psf = []
         for band in survey.available_filters:
             filt = survey.get_filter(band)
             if callable(filt.psf):
-                generated_psf = filt.psf()  # generate the PSF with the provided function
+                # generate the PSF with the provided function
+                generated_psf = filt.psf(survey, filt)
                 if isinstance(generated_psf, galsim.GSObject):
                     psf.append(generated_psf)
                 else:
                     raise TypeError(
                         f"The generated PSF with the provided function"
                         f"for filter '{filt.name}' is not a galsim object"
                     )
```

### Comparing `blending_toolkit-1.0.0b7/btk/match.py` & `blending_toolkit-1.0.0b8/btk/match.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,21 +20,20 @@
         pred_matches: List[np.ndarray],
         n_true: np.ndarray,
         n_pred: np.ndarray,
     ) -> None:
         """Initialize MatchInfo.
 
         Args:
-            true_matches: a list of 1D array, each entry corresponds to a numpy array
-                containing the index of detected object in the truth catalog that
-                got matched with the i-th truth object in the blend.
-            pred_matches: a list of 1D array, where the j-th entry of i-th array
-                corresponds to the index of truth object in the i-th blend
-                that got matched with the j-th detected object in that blend.
-                If no match, value is -1.
+            true_matches: a list of 1D arrays, each array containing the matching indices of
+                truth catalog rows for a given element of a batch. These indices are in 1-1
+                correspondence to the `pred_matches` indices.
+            pred_matches: a list of 1D arrays, each array containing the matching indices of
+                predicted catalog rows for a given element of a batch. These indices are in 1-1
+                correspondence to the `true_matches` indices.
             n_true: a 1D array of length N, where each entry is the number of truth objects.
             n_pred: a 1D array of length N, where each entry is the number of detected objects.
         """
         self.true_matches = true_matches
         self.pred_matches = pred_matches
         self.n_true = n_true
         self.n_pred = n_pred
@@ -62,20 +61,19 @@
             matches = self.pred_matches
         else:
             raise ValueError("true_or_pred must be 'true' or 'pred'")
 
         new_arrs = []
         for arr in arrs:
             assert len(arr) == self.batch_size
-            new_arr = np.zeros_like(arr)
+            new_arr = np.zeros((self.batch_size, self.max_n_sources, *arr.shape[2:]))
             for ii in range(self.batch_size):
-                n_sources = len(matches[ii])
-                assert n_sources <= self.max_n_sources
-                new_arr[ii, :n_sources] = arr[ii][matches[ii]]
-            new_arrs.append(new_arr[:, : self.max_n_sources])
+                for jj, m in enumerate(matches[ii]):
+                    new_arr[ii, jj] = arr[ii, m]
+            new_arrs.append(new_arr)
         return tuple(new_arrs) if len(new_arrs) > 1 else new_arrs[0]
 
     def match_true_catalogs(self, catalog_list: Table) -> List[Table]:
         """Returns a list of matched truth catalogs."""
         return self._match_catalogs(catalog_list, true_or_pred="true")
 
     def match_true_arrays(self, *arrs: np.ndarray) -> tuple:
@@ -111,14 +109,39 @@
             new_n_true.append(np.sum(mask[ii]))
             new_n_pred.append(self.n_pred[ii])
 
         return Matching(
             new_true_matches, new_pred_matches, np.array(new_n_true), np.array(new_n_pred)
         )
 
+    def filter_by_pred(self, mask: List[np.ndarray]) -> "Matching":
+        """Returns a new Matching object with detected objects that pass the mask."""
+        new_true_matches = []
+        new_pred_matches = []
+        new_n_true = []
+        new_n_pred = []
+        for ii in range(self.batch_size):
+            true_match = self.true_matches[ii]
+            pred_match = self.pred_matches[ii]
+
+            # get indices in pred_matches of pred objects that do not pass mask
+            isin_pred = np.isin(pred_match, np.where(~mask[ii])[0])
+            index_of_interest = np.argwhere(isin_pred).ravel()
+
+            # remove those indices from true_matches and pred_matches
+            new_true_matches.append(np.delete(true_match, index_of_interest, axis=0))
+            new_pred_matches.append(np.delete(pred_match, index_of_interest, axis=0))
+
+            new_n_true.append(self.n_true[ii])
+            new_n_pred.append(np.sum(mask[ii]))
+
+        return Matching(
+            new_true_matches, new_pred_matches, np.array(new_n_true), np.array(new_n_pred)
+        )
+
     @property
     def tp(self) -> np.ndarray:
         """Returns true positive array."""
         return np.array([len(d) for d in self.true_matches])
 
     @property
     def fp(self) -> np.ndarray:
@@ -150,14 +173,18 @@
         n_true = []
         n_pred = []
         for true_catalog, pred_catalog in zip(true_catalog_list, pred_catalog_list):
             if len(true_catalog) == 0 or len(pred_catalog) == 0:
                 true_match, pred_match = np.array([]).astype(int), np.array([]).astype(int)
             else:
                 true_match, pred_match = self.match_catalogs(true_catalog, pred_catalog)
+
+            if -1 in true_match or -1 in pred_match:
+                raise ValueError("Matcher should return only matching indices, not dummy -1 index.")
+
             match_true.append(true_match)
             match_pred.append(pred_match)
             n_true.append(len(true_catalog))
             n_pred.append(len(pred_catalog))
         return Matching(match_true, match_pred, np.array(n_true), np.array(n_pred))
 
     def compute_distance_matrix(self, truth_catalog: Table, predicted_catalog: Table) -> np.ndarray:
@@ -178,14 +205,19 @@
 
 
 class IdentityMatcher(Matcher):
     """Assumes catalogs are already matched one-to-one, returns trivial identity matching."""
 
     def match_catalogs(self, truth_catalog, predicted_catalog) -> np.ndarray:
         """Returns trivial identity matching."""
+        if not len(truth_catalog) == len(predicted_catalog):
+            raise ValueError(
+                "IdenityMatcher can be used because the given pair of truth "
+                "and predicated catalogs do not have the same size."
+            )
         true_indx = np.array(range(len(truth_catalog)))
         pred_indx = np.array(range(len(predicted_catalog)))
         return true_indx, pred_indx
 
 
 class PixelHungarianMatcher(Matcher):
     """Match based on pixel coordinates using Hungarian matching algorithm."""
@@ -204,33 +236,36 @@
     def match_catalogs(self, truth_catalog: Table, predicted_catalog: Table) -> np.ndarray:
         """Performs Hungarian matching algorithm on pixel coordinates from catalogs.
 
         Based on this implementation in scipy:
         https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.linear_sum_assignment.html
 
         Args:
-            truth_catalog: truth catalog containing relevant detecion information
-            predicted_catalog: predicted catalog to compare with the ground truth
+            truth_catalog: truth catalog containing true source centroid information.
+            predicted_catalog: predicted catalog containing detection information.
+
         Returns:
-            matched_indx: a 1D array where j-th entry is the index of the target row
-                that matched with the j-th detected row. If no match, value is -1.
+            A tuple of two arrays, each has length equal to the total number of matches. The i-th
+            index in the first array is the row of the truth catalog that was matched with the row
+            of the predicted catalog corresponding to the i-th index of the second array. The index
+            in each array.
         """
         dist = self.compute_distance_matrix(truth_catalog, predicted_catalog)
         # solve optimization problem using Hungarian matching algorithm
         # truth_catalog[true_indx[i]] is matched with predicted_catalog[matched_indx[i]]
-        # len(true_indx) = len(detect_indx) = min(len(true_table), len(detected_table))
+        # len(true_indx) = len(pred_indx) = min(len(true_table), len(pred_table))
         true_indx, pred_indx = linear_sum_assignment(dist)
 
-        # if the distance is greater than max_sep then mark detection as -1
-        true_mask = dist.T[pred_indx, true_indx] > self.max_sep
-        true_indx[true_mask] = -1
-        pred_mask = dist[true_indx, pred_indx] > self.max_sep
-        pred_indx[pred_mask] = -1
+        # if the distance is greater than `max_sep` then remove the matching.
+        true_mask = dist.T[pred_indx, true_indx] < self.max_sep
+        true_match = true_indx[true_mask]
+        pred_mask = dist[true_indx, pred_indx] < self.max_sep
+        pred_match = pred_indx[pred_mask]
 
-        return true_indx, pred_indx
+        return true_match, pred_match
 
 
 class SkyClosestNeighbourMatcher(Matcher):
     """Match based on closest neighbour in the sky."""
 
     def __init__(self, arcsec_max_sep=2.0, **kwargs) -> None:
         """Initialize matching class.
@@ -280,28 +315,30 @@
         for target_idx in set(idx):
             masked_d2d = d2d.arcsec.copy()
             masked_d2d[idx != target_idx] = np.inf
             match_id = np.argmin(masked_d2d)
             pred_indx[match_id] = target_idx
 
         # if the matched distance exceeds max_sep, we discard that detection
-        pred_indx[d2d.to(units.arcsec) > self.max_sep * units.arcsec] = -1
+        pred_mask = d2d.to(units.arcsec) < self.max_sep * units.arcsec
+        pred_match = pred_indx[pred_mask]
 
         # now for ture indices
         idx, d2d, _ = true_coordinates.match_to_catalog_sky(pred_coordinates)
         true_indx = np.array([-1] * len(idx))
         for target_idx in set(idx):
             masked_d2d = d2d.arcsec.copy()
             masked_d2d[idx != target_idx] = np.inf
             match_id = np.argmin(masked_d2d)
             true_indx[match_id] = target_idx
 
-        true_indx[d2d.to(units.arcsec) > self.max_sep * units.arcsec] = -1
+        true_mask = d2d.to(units.arcsec) < self.max_sep * units.arcsec
+        true_match = true_indx[true_mask]
 
-        return true_indx, pred_indx
+        return true_match, pred_match
 
 
 def pixel_l2_distance_matrix(
     x1: np.ndarray, y1: np.ndarray, x2: np.ndarray, y2: np.ndarray
 ) -> np.ndarray:
     """Computes the pixel L2 (Ecludian) distance matrix between targets and detections.
```

### Comparing `blending_toolkit-1.0.0b7/btk/measure.py` & `blending_toolkit-1.0.0b8/btk/measure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module for measuring galaxy properties."""
+"""Module for measuring galaxy properties from images."""
 
 from typing import Tuple
 
 import galsim
 import numpy as np
 import sep
 from galsim import GSObject
@@ -52,78 +52,98 @@
                     images[ii, jj], psf, pixel_scale, verbose=verbose
                 )
             else:
                 ellipticities[ii, jj] = (np.nan, np.nan)
     return ellipticities
 
 
-def get_blendedness(iso_image: np.ndarray):
+def get_blendedness(iso_image: np.ndarray) -> np.ndarray:
     """Calculate blendedness given isolated images of each galaxy in a blend.
 
     Args:
-        iso_image: Array of shape = (..., N, H, W) corresponding to images of the isolated
-            galaxy you are calculating blendedness for.
+        iso_image: Array of shape = (..., N, H, W) corresponding to images of isolated
+            galaxies you are calculating blendedness for.
+
+    Returns:
+        Array of size (..., N) corresponding to blendedness values for each individual galaxy.
     """
     assert iso_image.ndim >= 3
     num = np.sum(iso_image * iso_image, axis=(-1, -2))
     blend = np.sum(iso_image, axis=-3)[..., None, :, :]
     denom = np.sum(blend * iso_image, axis=(-1, -2))
-    return 1 - num / denom
+    return 1 - np.divide(num, denom, out=np.ones_like(num), where=(num != 0))
 
 
-def get_snr(iso_image: np.ndarray, sky_level: float) -> float:
+def get_snr(iso_image: np.ndarray, sky_level: float) -> np.ndarray:
     """Calculate SNR of a set of isolated galaxies with same sky level.
 
     Args:
         iso_image: Array of shape = (..., H, W) corresponding to image of the isolated
             galaxy you are calculating SNR for.
         sky_level: Background level of all images. Images are assume to be
             background-substracted.
+
+    Returns:
+        Array of size (...) corresponding to SNR values for each individual galaxy.
     """
     images = iso_image + sky_level
     return np.sqrt(np.sum(iso_image * iso_image / images, axis=(-1, -2)))
 
 
 def _get_single_aperture_flux(
     image: np.ndarray, x: np.ndarray, y: np.ndarray, radius: float, sky_level: float
-) -> np.ndarray:
+) -> Tuple[np.ndarray, np.ndarray]:
     """Utility function to measure flux using fixed circular aperture with sep.
 
     Args:
         image (np.array): Single iamge to measure flux on, with shape (H, W).
         x (np.array): x coordinates of the center of the aperture (in pixels).
         y (np.array): y coordinates of the center of the aperture (in pixels).
         sky_level (float): Background level of all images.
             Images are assume to be background substracted.
         radius (float): Radius of the aperture in pixels.
+
+    Returns:
+        Tuple of flux and fluxerr.
     """
     assert image.ndim == 2
-    flux, _, _ = sep.sum_circle(image, x, y, radius, err=sky_level)
-    return flux[0]
+    assert x.ndim == 1 and y.ndim == 1
+    flux, fluxerr, _ = sep.sum_circle(image, x, y, radius, var=sky_level)
+    return flux, fluxerr
 
 
 def get_aperture_fluxes(
     images: np.ndarray, xs: np.ndarray, ys: np.ndarray, radius: float, sky_level: float
-) -> np.ndarray:
+) -> Tuple[np.ndarray, np.ndarray]:
     """Utility function to measure flux using fixed circular aperture with sep.
 
     Args:
         images (np.array): Images to measure flux on, with shape (B, H, W).
         xs (np.array): x coordinates of the center of the aperture (in pixels).
         ys (np.array): y coordinates of the center of the aperture (in pixels).
         sky_level (float): Background level of all images.
             Images are assume to be background substracted.
         radius (float): Radius of the aperture in pixels.
+
+    Returns:
+        fluxes (np.array): Array of shape (B, N) corresponding to the measured aperture fluxes
+            in each given position for each of the B batches.
+        fluxerr (np.array): Array of same shape with corresponding flux errors.
     """
     assert images.ndim == 3
-    batch_size = images.shape[0]
-    fluxes = np.zeros((batch_size, len(xs)))
+    assert xs.ndim == 2 and ys.ndim == 2
+    batch_size, max_n_sources = xs.shape
+    fluxes = np.zeros((batch_size, max_n_sources))
+    fluxerrs = np.zeros((batch_size, max_n_sources))
     for ii in range(batch_size):
-        fluxes[ii] = _get_single_aperture_flux(images[ii], xs[ii], ys[ii], radius, sky_level)
-    return fluxes
+        n_sources = np.sum((xs[ii] > 0) & (ys[ii] > 0)).astype(int)
+        flux, err = _get_single_aperture_flux(images[ii], xs[ii], ys[ii], radius, sky_level)
+        fluxes[ii, :n_sources] = flux[:n_sources]
+        fluxerrs[ii, :n_sources] = err[:n_sources]
+    return fluxes, fluxerrs
 
 
 def get_residual_images(iso_images: np.ndarray, blend_images: np.ndarray) -> np.ndarray:
     """Calculate residual images given isolated images of each galaxy in a blend.
 
     Args:
         iso_images: Array of shape = (B, N, H, W) corresponding to images of the isolated
```

### Comparing `blending_toolkit-1.0.0b7/btk/metrics/base.py` & `blending_toolkit-1.0.0b8/btk/metrics/base.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/metrics/detection.py` & `blending_toolkit-1.0.0b8/btk/metrics/detection.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/metrics/reconstruction.py` & `blending_toolkit-1.0.0b8/btk/metrics/reconstruction.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/metrics/segmentation.py` & `blending_toolkit-1.0.0b8/btk/metrics/segmentation.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     def _get_data(
         self,
         seg1: np.ndarray,
         seg2: np.ndarray,
     ) -> Dict[str, np.ndarray]:
         assert seg1.shape == seg2.shape
         assert seg1.ndim == 4  # batch, max_n_sources, x, y
-        ious = np.zeros(self.batch_size)
+        ious = np.full((self.batch_size, seg1.shape[1]), fill_value=np.nan)
         for ii in range(self.batch_size):
-            n_sources = np.sum(~np.isnan(seg1[ii].sum(axis=(-1, -2))))
+            n_sources1 = np.sum(np.sum(seg1[ii], axis=(-1, -2)) > 0)
+            n_sources2 = np.sum(np.sum(seg2[ii], axis=(-1, -2)) > 0)
+            n_sources = min(n_sources1, n_sources2)
             if n_sources > 0:
                 seg1_ii = seg1[ii, :n_sources]
                 seg2_ii = seg2[ii, :n_sources]
-                ious[ii] = iou(seg1_ii, seg2_ii)
-            else:
-                ious[ii] = np.nan
+                ious[ii, :n_sources] = iou(seg1_ii, seg2_ii)
 
         return {"iou": ious}
 
     def _compute(self, data: dict) -> float:
         return np.nanmean(data["iou"])
```

### Comparing `blending_toolkit-1.0.0b7/btk/metrics/utils.py` & `blending_toolkit-1.0.0b8/btk/metrics/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     Returns:
         Returns `iou` between each corresponding segmentation map as an array of shape `N`
 
     """
     assert not np.any(np.isnan(seg1)) and not np.any(np.isnan(seg2))
     seg1 = seg1.astype(bool)
-    seg2 = seg1.astype(bool)
+    seg2 = seg2.astype(bool)
     i = np.logical_and(seg1, seg2).sum(axis=(-1, -2))
     u = np.logical_or(seg1, seg2).sum(axis=(-1, -2))
     return i / u
 
 
 def psnr(images1: np.ndarray, images2: np.ndarray) -> np.ndarray:
     """Compute peak-signal-to-noise-ratio from skimage.
```

### Comparing `blending_toolkit-1.0.0b7/btk/multiprocess.py` & `blending_toolkit-1.0.0b8/btk/multiprocess.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/btk/plotting.py` & `blending_toolkit-1.0.0b8/btk/plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 """Utility functions for plotting images."""
 
 from typing import Optional
 
 import numpy as np
 
+CB_color_cycle = [
+    "#377eb8",
+    "#ff7f00",
+    "#4daf4a",
+    "#f781bf",
+    "#a65628",
+    "#984ea3",
+    "#999999",
+    "#e41a1c",
+    "#dede00",
+]
+
 
 def get_rgb(image: np.ndarray, min_val: Optional[float] = None, max_val: Optional[float] = None):
     """Function to normalize 3 band input image to RGB 0-255 image.
 
     Args:
         image: Image array to convert to RGB image with dtype
                 uint8 [bands, height, width].
```

### Comparing `blending_toolkit-1.0.0b7/btk/sampling_functions.py` & `blending_toolkit-1.0.0b8/btk/sampling_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
     can be customized by the user at initialization.
 
     """
 
     def __init__(
         self,
         stamp_size: float = 24.0,
-        max_shift: float = Optional[None],
+        max_shift: Optional[float] = None,
         mag_name: str = "i_ab",
         seed: int = DEFAULT_SEED,
         bright_cut: float = 25.3,
         dim_cut: float = 28.0,
     ):
         """Initializes the PairSampling function.
```

### Comparing `blending_toolkit-1.0.0b7/btk/survey.py` & `blending_toolkit-1.0.0b8/btk/survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,17 @@
     # add PSF to filters
     surveys = []
     for survey_name in names:
         survey = Survey.from_galcheat_survey(survey_name)
         for band in survey.available_filters:
             filtr = survey.get_filter(band)
             if psf_func is None:
-                psf = _get_default_psf_with_galcheat_info(survey, filtr)
+                filtr.psf = _get_default_psf_with_galcheat_info(survey, filtr)
             else:
-                psf = psf_func(survey, filtr)
-            filtr.psf = psf
+                filtr.psf = psf_func
         surveys.append(survey)
 
     if len(surveys) == 1:
         surveys = surveys[0]
     return surveys
```

### Comparing `blending_toolkit-1.0.0b7/btk/utils.py` & `blending_toolkit-1.0.0b8/btk/utils.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b7/pyproject.toml` & `blending_toolkit-1.0.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Blending ToolKit"
 keywords = ["cosmology", "galaxies", "blending", "lsst", "simulation"]
 license = "MIT"
 name = "blending_toolkit"
 readme = "README.md"
-version = "1.0.0b7"
+version = "1.0.0b8"
 packages = [{ include = "btk" }]
 repository = "https://github.com/LSSTDESC/BlendingToolKit"
 homepage = "https://lsstdesc.org/BlendingToolKit/index.html"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/LSSTDESC/BlendingToolKit/issues"
 
@@ -40,15 +40,14 @@
 scipy = ">=1.9.1"
 tqdm = ">=4.65.0"
 sep = ">=1.2.1"
 galsim = ">=2.4.9"
 python = "^3.8.1,<3.12"
 h5py = "^3.9.0"
 fast3tree = "^0.4.1"
-ruff = "^0.3.2"
 
 [tool.poetry.group.scarlet]
 optional = true
 
 [tool.poetry.group.scarlet.dependencies]
 peigen = "^0.0.9"
 autograd = "^1.5"
@@ -61,14 +60,16 @@
 jupyter = ">=1.0.0"
 jupyter-sphinx = ">=0.4.0"
 nbmake = ">=1.4.1"
 nbstripout = ">=0.6.1"
 pytest = ">=7.3.1"
 sphinx = ">=4.2.0"
 sphinx-rtd-theme = ">=1.2.1"
+ruff = "^0.3.2"
+
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core>=1.0.0",
   "setuptools",
   "numpy",
@@ -167,14 +168,15 @@
 # enabled.
 docstring-code-line-length = "dynamic"
 
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["E402", "I", "F"]
 "**/{tests,docs,tools}/*" = ["E402", "D", "PLR0915"]
+"**/*.ipynb" = ["I"]
 
 [tool.ruff.lint.pydocstyle]
 convention="google"
 
 [tool.pytest.ini_options]
 addopts = "-ra"
 minversion = "6.0"
```

### Comparing `blending_toolkit-1.0.0b7/PKG-INFO` & `blending_toolkit-1.0.0b8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blending_toolkit
-Version: 1.0.0b7
+Version: 1.0.0b8
 Summary: Blending ToolKit
 Home-page: https://lsstdesc.org/BlendingToolKit/index.html
 License: MIT
 Keywords: cosmology,galaxies,blending,lsst,simulation
 Author: Ismael Mendoza
 Author-email: imendoza@umich.edu
 Requires-Python: >=3.8.1,<3.12
@@ -18,15 +18,14 @@
 Requires-Dist: astropy (>=5.1)
 Requires-Dist: fast3tree (>=0.4.1,<0.5.0)
 Requires-Dist: galcheat (>=1.0.0,<2.0.0)
 Requires-Dist: galsim (>=2.4.9)
 Requires-Dist: h5py (>=3.9.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: numpy (>=1.22)
-Requires-Dist: ruff (>=0.3.2,<0.4.0)
 Requires-Dist: scikit-image (>=0.20.0)
 Requires-Dist: scipy (>=1.9.1)
 Requires-Dist: sep (>=1.2.1)
 Requires-Dist: tqdm (>=4.65.0)
 Project-URL: Bug Tracker, https://github.com/LSSTDESC/BlendingToolKit/issues
 Project-URL: Repository, https://github.com/LSSTDESC/BlendingToolKit
 Description-Content-Type: text/markdown
@@ -115,15 +114,15 @@
 ```
 
 ## Installation
 
 BTK is pip installable, with the following command:
 
 ```bash
-pip install blending-toolkit==1.0.0b7
+pip install --pre blending-toolkit
 ```
 
 In case of any issues and for details of required packages, please see the more detailed installation instructions [here](https://lsstdesc.org/BlendingToolKit/install.html).
 
 ## Contributing
 
 Everyone can contribute to this project, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) document for details.
```

