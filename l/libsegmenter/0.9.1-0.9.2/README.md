# Comparing `tmp/libsegmenter-0.9.1-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/libsegmenter-0.9.2-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 101925 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      708 b- defN 24-Apr-23 12:34 libsegmenter/Segmenter.py
--rw-rw-rw-  2.0 fat     9073 b- defN 24-Apr-23 12:34 libsegmenter/SegmenterTensorFlow.py
--rw-rw-rw-  2.0 fat     7599 b- defN 24-Apr-23 12:34 libsegmenter/SegmenterTorch.py
--rw-rw-rw-  2.0 fat      107 b- defN 24-Apr-23 12:34 libsegmenter/__init__.py
--rw-rw-rw-  2.0 fat   195072 b- defN 24-Apr-23 12:48 libsegmenter/bindings.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     4678 b- defN 24-Apr-23 12:34 libsegmenter/default_window_selector.py
--rw-rw-rw-  2.0 fat     2621 b- defN 24-Apr-23 12:34 libsegmenter/old.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 12:34 tests/__init__.py
--rw-rw-rw-  2.0 fat     2292 b- defN 24-Apr-23 12:34 tests/creational.py
--rw-rw-rw-  2.0 fat    12744 b- defN 24-Apr-23 12:34 tests/reconstruction.py
--rw-rw-rw-  2.0 fat      916 b- defN 24-Apr-23 12:34 tests/windows.py
--rw-rw-rw-  2.0 fat      279 b- defN 24-Apr-23 12:48 libsegmenter-0.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 24-Apr-23 12:48 libsegmenter-0.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-23 12:48 libsegmenter-0.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1236 b- defN 24-Apr-23 12:48 libsegmenter-0.9.1.dist-info/RECORD
-15 files, 237451 bytes uncompressed, 99879 bytes compressed:  57.9%
+Zip file size: 10704 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      708 b- defN 24-May-02 07:01 libsegmenter/Segmenter.py
+-rw-rw-rw-  2.0 fat     9073 b- defN 24-May-02 07:01 libsegmenter/SegmenterTensorFlow.py
+-rw-rw-rw-  2.0 fat     7539 b- defN 24-May-02 07:01 libsegmenter/SegmenterTorch.py
+-rw-rw-rw-  2.0 fat      107 b- defN 24-May-02 07:01 libsegmenter/__init__.py
+-rw-rw-rw-  2.0 fat     4680 b- defN 24-May-02 07:01 libsegmenter/default_window_selector.py
+-rw-rw-rw-  2.0 fat     2621 b- defN 24-May-02 07:01 libsegmenter/old.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-02 07:01 tests/__init__.py
+-rw-rw-rw-  2.0 fat     2292 b- defN 24-May-02 07:01 tests/creational.py
+-rw-rw-rw-  2.0 fat    12744 b- defN 24-May-02 07:01 tests/reconstruction.py
+-rw-rw-rw-  2.0 fat      916 b- defN 24-May-02 07:01 tests/windows.py
+-rw-rw-rw-  2.0 fat      279 b- defN 24-May-02 07:34 libsegmenter-0.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 24-May-02 07:34 libsegmenter-0.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 24-May-02 07:34 libsegmenter-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 24-May-02 07:34 libsegmenter-0.9.2.dist-info/RECORD
+14 files, 42215 bytes uncompressed, 8828 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -6,17 +6,14 @@
 
 Filename: libsegmenter/SegmenterTorch.py
 Comment: 
 
 Filename: libsegmenter/__init__.py
 Comment: 
 
-Filename: libsegmenter/bindings.pypy39-pp73-win_amd64.pyd
-Comment: 
-
 Filename: libsegmenter/default_window_selector.py
 Comment: 
 
 Filename: libsegmenter/old.py
 Comment: 
 
 Filename: tests/__init__.py
@@ -27,20 +24,20 @@
 
 Filename: tests/reconstruction.py
 Comment: 
 
 Filename: tests/windows.py
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/METADATA
+Filename: libsegmenter-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/WHEEL
+Filename: libsegmenter-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/top_level.txt
+Filename: libsegmenter-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/RECORD
+Filename: libsegmenter-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsegmenter/SegmenterTorch.py

```diff
@@ -106,15 +106,14 @@
             batched = False
             x = x.unsqueeze(0)
         else:
             raise ValueError(
                 f"only support for inputs with dimension 1 or 2, provided {x.dim()}"
             )
 
-
         number_of_segments = (
             (number_of_samples) // self.hop_size - self.frame_size // self.hop_size + 1
         )
 
         X = torch.zeros(
             (number_of_batch_elements, number_of_segments, self.frame_size),
             **self.factory_kwargs,
@@ -142,17 +141,15 @@
         else:
             for k in range(number_of_segments):
                 X[:, k, :] = x[
                     :, k * self.hop_size : k * self.hop_size + self.frame_size
                 ]
 
         if compute_spectrogram:
-            print(X[0,0,:])
             X = torch.fft.rfft(X)
-            print(X[0,0,:])
 
         if not batched:
             # convert back to not-batched
             X = X.squeeze(0)
 
         return X
```

## libsegmenter/default_window_selector.py

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from .bindings import *
 
+
 def kaiser(window_length: int, beta: float) -> np.array:
     """
     Note that the Kaiser window is not strictly speaking COLA compliant as it does not have harmonic nulls that can be tuned to the
     harmonics of the frame rate. As such it only offers approximate perfect reconstruction. However, by tuning the beta parameter,
     the reconstruction error can be controlled
     """
     M = np.float64(window_length + 1.0)
```

## Comparing `libsegmenter-0.9.1.dist-info/RECORD` & `libsegmenter-0.9.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 libsegmenter/Segmenter.py,sha256=x5oAD1C6jpBsuPNh_cFm5T_wpPT3j2-ecEl5k9B1Byc,708
 libsegmenter/SegmenterTensorFlow.py,sha256=X-sqvo3pURBUivUTjT24aGJsn8nrHHCTWfHV5R4aeiA,9073
-libsegmenter/SegmenterTorch.py,sha256=bp2lEmQIbfCLz34jillJHD9oB3xk7Z2c1-OH-DDsuAc,7599
+libsegmenter/SegmenterTorch.py,sha256=ghSxUn5gsQvypNlfGVyERRx5G9V4WxLE5gcMen3QC_U,7539
 libsegmenter/__init__.py,sha256=BhUJudEKMTAEnu1Kq-Ckbg6kTZp-g-6Zx2PvntlIeAQ,107
-libsegmenter/bindings.pypy39-pp73-win_amd64.pyd,sha256=AxEZRi7lGFPgKpsO1tIK9uBDKNw5pHw1r2GupHSBH80,195072
-libsegmenter/default_window_selector.py,sha256=q0dmDqPZMWc52ET0PwqpN17rRP53-BVody87akXBIXc,4678
+libsegmenter/default_window_selector.py,sha256=0e5aWMu6-4pQsuG4xFnmHceGDe_9-fo-3Ie8qJeONv8,4680
 libsegmenter/old.py,sha256=328FhSPvoTqEf-AUsq6WWkLY_fM_sHCqPPCTcRdfbog,2621
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/creational.py,sha256=QWS4mMHxRgeMcTV6f2i3DjuDF0e391w_ciIheb4krBI,2292
 tests/reconstruction.py,sha256=FsjjSivsY4s6LzY29KRMzNfrxtvw2HaYvdxn6YMfD74,12744
 tests/windows.py,sha256=fjwAUL-J9ZzwaXvSTZrgFO7D6RmfkGCmiYBkihEDI3E,916
-libsegmenter-0.9.1.dist-info/METADATA,sha256=CRaAoIttX_PObE4-ChG4SicV3eAlotjavRN0mrWjcFw,279
-libsegmenter-0.9.1.dist-info/WHEEL,sha256=0MDxp1g6SMi6x5fNLQYB_oq4z1ZIM2F5EzPGH_eSWIs,107
-libsegmenter-0.9.1.dist-info/top_level.txt,sha256=vM1fU6i2eEkdt_wR1Rvw_-LVSVSaa-Qr-O0y7KtZ500,19
-libsegmenter-0.9.1.dist-info/RECORD,,
+libsegmenter-0.9.2.dist-info/METADATA,sha256=TvgNaPSY7krhmC57uBNRoXY_mHTFh0Ii8rEWIM4EXdo,279
+libsegmenter-0.9.2.dist-info/WHEEL,sha256=0MDxp1g6SMi6x5fNLQYB_oq4z1ZIM2F5EzPGH_eSWIs,107
+libsegmenter-0.9.2.dist-info/top_level.txt,sha256=vM1fU6i2eEkdt_wR1Rvw_-LVSVSaa-Qr-O0y7KtZ500,19
+libsegmenter-0.9.2.dist-info/RECORD,,
```

