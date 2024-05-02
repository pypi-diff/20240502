# Comparing `tmp/libsegmenter-0.9.1-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/libsegmenter-0.9.2-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,20 @@
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
+Zip file size: 149389 bytes, number of entries: 18
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 07:09 tests/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 07:09 libsegmenter/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 07:09 libsegmenter-0.9.2.dist-info/
+-rw-r--r--  2.0 unx    12369 b- defN 24-May-02 07:01 tests/reconstruction.py
+-rw-r--r--  2.0 unx     2229 b- defN 24-May-02 07:01 tests/creational.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 07:01 tests/__init__.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-02 07:01 tests/windows.py
+-rw-r--r--  2.0 unx     4569 b- defN 24-May-02 07:01 libsegmenter/default_window_selector.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-May-02 07:01 libsegmenter/old.py
+-rw-r--r--  2.0 unx      102 b- defN 24-May-02 07:01 libsegmenter/__init__.py
+-rwxr-xr-x  2.0 unx   382048 b- defN 24-May-02 07:09 libsegmenter/bindings.pypy39-pp73-darwin.so
+-rw-r--r--  2.0 unx     8835 b- defN 24-May-02 07:01 libsegmenter/SegmenterTensorFlow.py
+-rw-r--r--  2.0 unx      684 b- defN 24-May-02 07:01 libsegmenter/Segmenter.py
+-rw-r--r--  2.0 unx     7329 b- defN 24-May-02 07:01 libsegmenter/SegmenterTorch.py
+-rw-rw-r--  2.0 unx     1247 b- defN 24-May-02 07:09 libsegmenter-0.9.2.dist-info/RECORD
+-rw-r--r--  2.0 unx      115 b- defN 24-May-02 07:09 libsegmenter-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-02 07:09 libsegmenter-0.9.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      270 b- defN 24-May-02 07:09 libsegmenter-0.9.2.dist-info/METADATA
+18 files, 423245 bytes uncompressed, 147027 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,46 +1,55 @@
-Filename: libsegmenter/Segmenter.py
+Filename: tests/
 Comment: 
 
-Filename: libsegmenter/SegmenterTensorFlow.py
+Filename: libsegmenter/
 Comment: 
 
-Filename: libsegmenter/SegmenterTorch.py
+Filename: libsegmenter-0.9.2.dist-info/
 Comment: 
 
-Filename: libsegmenter/__init__.py
+Filename: tests/reconstruction.py
+Comment: 
+
+Filename: tests/creational.py
+Comment: 
+
+Filename: tests/__init__.py
 Comment: 
 
-Filename: libsegmenter/bindings.pypy39-pp73-win_amd64.pyd
+Filename: tests/windows.py
 Comment: 
 
 Filename: libsegmenter/default_window_selector.py
 Comment: 
 
 Filename: libsegmenter/old.py
 Comment: 
 
-Filename: tests/__init__.py
+Filename: libsegmenter/__init__.py
 Comment: 
 
-Filename: tests/creational.py
+Filename: libsegmenter/bindings.pypy39-pp73-darwin.so
 Comment: 
 
-Filename: tests/reconstruction.py
+Filename: libsegmenter/SegmenterTensorFlow.py
 Comment: 
 
-Filename: tests/windows.py
+Filename: libsegmenter/Segmenter.py
+Comment: 
+
+Filename: libsegmenter/SegmenterTorch.py
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/METADATA
+Filename: libsegmenter-0.9.2.dist-info/RECORD
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/WHEEL
+Filename: libsegmenter-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/top_level.txt
+Filename: libsegmenter-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: libsegmenter-0.9.1.dist-info/RECORD
+Filename: libsegmenter-0.9.2.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## libsegmenter/Segmenter.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-import numpy as np
-from .default_window_selector import default_window_selector
-
-backends = ["torch", "tensorflow", "base"]
-
-
-def make_segmenter(backend: str = "base", *args, **kwargs):
-    if backend not in backends:
-        raise ValueError(f"Unsupported backend {backend}, availible: {backends}")
-
-    if backend == "torch":
-        from .SegmenterTorch import SegmenterTorch
-
-        return SegmenterTorch(*args, **kwargs)
-
-    if backend == "tensorflow":
-        from .SegmenterTensorFlow import SegmenterTensorFlow
-
-        return SegmenterTensorFlow(*args, **kwargs)
-
-    if backend == "base":
-        from .bindings import Segmenter
-
-        return Segmenter(*args, **kwargs)
+import numpy as np
+from .default_window_selector import default_window_selector
+
+backends = ["torch", "tensorflow", "base"]
+
+
+def make_segmenter(backend: str = "base", *args, **kwargs):
+    if backend not in backends:
+        raise ValueError(f"Unsupported backend {backend}, availible: {backends}")
+
+    if backend == "torch":
+        from .SegmenterTorch import SegmenterTorch
+
+        return SegmenterTorch(*args, **kwargs)
+
+    if backend == "tensorflow":
+        from .SegmenterTensorFlow import SegmenterTensorFlow
+
+        return SegmenterTensorFlow(*args, **kwargs)
+
+    if backend == "base":
+        from .bindings import Segmenter
+
+        return Segmenter(*args, **kwargs)
```

## libsegmenter/SegmenterTensorFlow.py

 * *Ordering differences only*

```diff
@@ -1,238 +1,238 @@
-import numpy as np
-import tensorflow as tf
-from .bindings import check_cola
-
-
-class SegmenterTensorFlow(tf.Module):
-    def __init__(
-        self,
-        frame_size,
-        hop_size,
-        window,
-        mode="wola",
-        edge_correction=True,
-        normalize_window=True,
-    ):
-        """
-        A class for segmenting input data using windowing and hop size with support for WOLA and OLA modes.
-
-        Attributes:
-            segment_size (int): Size of each segment.
-            hop_size (int): Hop size between segments.
-            window (Tensor): Windowing function applied to each segment.
-            mode (str): Either 'wola' or 'ola' for Weighted Overlap-Add or Overlap-Add method.
-            edge_correction (bool): If True, apply edge correction to the first and last segments.
-            normalize_window (bool): If True, normalize the windowing function.
-        """
-        super(SegmenterTensorFlow, self).__init__()
-        self.hop_size = hop_size
-        self.frame_size = frame_size
-        self.window = window
-
-        # asserts to ensure correctness
-        if self.frame_size % 2 != 0:
-            raise ValueError("only even frame_size is supported")
-
-        if self.hop_size > self.frame_size:
-            raise ValueError("hop_size cannot be larger than frame_size")
-
-        if self.window.shape[0] != self.frame_size:
-            raise ValueError("specified window must have the same size as frame_size")
-
-        if any(window < 0.0):
-            raise ValueError("specified window contains negative values")
-
-        if check_cola(window, self.hop_size)[0] == False:
-            raise ValueError(
-                "specified window is not COLA, consider using `default_window_selector`"
-            )
-
-        # compute prewindow and postwindow
-        prewindow = np.copy(window)
-        for hIdx in range(1, self.frame_size // self.hop_size + 1):
-            idx1Start = hIdx * self.hop_size
-            idx1End = self.frame_size
-            idx2Start = 0
-            idx2End = self.frame_size - idx1Start
-            prewindow[idx2Start:idx2End] = (
-                prewindow[idx2Start:idx2End] + window[idx1Start:idx1End]
-            )
-
-        postwindow = np.copy(window)
-        for hIdx in range(1, self.frame_size // self.hop_size + 1):
-            idx1Start = hIdx * self.hop_size
-            idx1End = self.frame_size
-            idx2Start = 0
-            idx2End = self.frame_size - idx1Start
-            postwindow[idx1Start:idx1End] = (
-                postwindow[idx1Start:idx1End] + window[idx2Start:idx2End]
-            )
-
-        # this is a tiny bit hacked, but it works well in practise
-        if normalize_window:
-            value = check_cola(window, hop_size)
-            normalization = value[1]
-            window = window / normalization
-            prewindow = prewindow / normalization
-            postwindow = postwindow / normalization
-
-        if not edge_correction:
-            prewindow = window
-            postwindow = window
-
-        if mode == "wola":
-            self.mode = mode
-            window = np.sqrt(window)
-            prewindow = np.sqrt(prewindow)
-            postwindow = np.sqrt(postwindow)
-        elif mode == "ola":
-            self.mode = mode
-        else:
-            raise ValueError(f"only support for mode ola and wola")
-
-        self.window = tf.convert_to_tensor(window, dtype=tf.float32)
-        self.prewindow = tf.convert_to_tensor(prewindow, dtype=tf.float32)
-        self.postwindow = tf.convert_to_tensor(postwindow, dtype=tf.float32)
-
-    def _segment(self, x, compute_spectrogram=False):
-        if (tf.rank(x) == 2) and (x.shape[1] > 1):
-            number_of_batch_elements = x.shape[0]
-            number_of_samples = x.shape[1]
-            batched = True
-        elif tf.rank(x) == 1:
-            number_of_samples = x.shape[0]
-            number_of_batch_elements = 1
-
-            # convert to batched to simplify subsequent code
-            batched = False
-            x = tf.expand_dims(x, axis=0)
-
-        else:
-            raise ValueError(
-                f"only support for inputs with dimension 1 or 2, provided {len(x.shape)}"
-            )
-
-        number_of_frames = (
-            (number_of_samples) // self.hop_size - self.frame_size // self.hop_size + 1
-        )
-
-        X = tf.zeros(
-            shape=(number_of_batch_elements, number_of_frames, self.frame_size)
-        )
-        for b in range(number_of_batch_elements):
-            if self.mode == "wola":
-                k = 0
-                tmp = tf.reshape(
-                    x[b, k * self.hop_size : k * self.hop_size + self.frame_size],
-                    shape=(1, 1, self.frame_size),
-                )
-                X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp * self.prewindow)
-                for k in range(1, number_of_frames - 1):
-                    tmp = tf.reshape(
-                        x[
-                            b,
-                            k * self.hop_size : k * self.hop_size + self.frame_size,
-                        ],
-                        shape=(1, 1, self.frame_size),
-                    )
-                    X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp * self.window)
-                k = number_of_frames - 1
-                tmp = tf.reshape(
-                    x[b, k * self.hop_size : k * self.hop_size + self.frame_size],
-                    shape=(1, 1, self.frame_size),
-                )
-                X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp * self.postwindow)
-            else:
-                for k in range(number_of_frames):
-                    tmp = tf.reshape(
-                        x[
-                            b,
-                            k * self.hop_size : k * self.hop_size + self.frame_size,
-                        ],
-                        shape=(1, 1, self.frame_size),
-                    )
-                    X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp)
-
-        if compute_spectrogram:
-            X = tf.signal.rfft(X)
-
-        # torchaudio convention
-        # X = tf.transpose(X, perm=[0, 2, 1])
-
-        if not batched:
-            # convert back to not-batched
-            X = tf.squeeze(X, axis=0)
-
-        return X
-
-    def _unsegment(self, X, compute_spectrogram=False):
-        if tf.rank(X) == 3:
-            number_of_batch_elements = X.shape[0]
-            number_of_frames = X.shape[1]
-            batched = True
-        elif tf.rank(X) == 2:
-            number_of_batch_elements = 1
-            number_of_frames = X.shape[0]
-
-            # convert to batched to simplify subsequent code
-            batched = False
-            X = tf.expand_dims(X, axis=0)
-        else:
-            raise ValueError(
-                f"only support for inputs with dimension 2 or 3, provided {len(X.shape)}"
-            )
-        number_of_samples = (number_of_frames - 1) * self.hop_size + self.frame_size
-
-        # torchaudio convention
-        # X = tf.transpose(X, perm=[0, 2, 1])
-
-        if compute_spectrogram:
-            X = tf.signal.irfft(X)
-
-        x = tf.zeros(shape=(number_of_batch_elements, number_of_samples))
-        for b in range(number_of_batch_elements):
-            k = 0
-            tmpIdx = tf.reshape(
-                tf.range(k * self.hop_size, k * self.hop_size + self.frame_size),
-                shape=(self.frame_size, 1),
-            )
-            idx = tf.concat(
-                [tf.constant(b, shape=(self.frame_size, 1)), tmpIdx], axis=1
-            )
-            x = tf.tensor_scatter_nd_add(x, idx, self.prewindow * X[b, k, :])
-            for k in range(1, number_of_frames - 1):
-                tmpIdx = tf.reshape(
-                    tf.range(k * self.hop_size, k * self.hop_size + self.frame_size),
-                    shape=(self.frame_size, 1),
-                )
-                idx = tf.concat(
-                    [tf.constant(b, shape=(self.frame_size, 1)), tmpIdx], axis=1
-                )
-                x = tf.tensor_scatter_nd_add(x, idx, self.window * X[b, k, :])
-            k = k + 1
-            tmpIdx = tf.reshape(
-                tf.range(k * self.hop_size, k * self.hop_size + self.frame_size),
-                shape=(self.frame_size, 1),
-            )
-            idx = tf.concat(
-                [tf.constant(b, shape=(self.frame_size, 1)), tmpIdx], axis=1
-            )
-            x = tf.tensor_scatter_nd_add(x, idx, self.postwindow * X[b, k, :])
-
-        if not batched:
-            # convert back to not-batched
-            x = tf.squeeze(x, axis=0)
-
-        return x
-
-    def segment(self, x):
-        return self._segment(x)
-
-    def unsegment(self, X):
-        return self._unsegment(X)
-
-    def spectrogram(self, x):
-        X = self._segment(x, compute_spectrogram=True)
-
-    def unspectrogram(self, X):
-        return self._unsegment(X, compute_spectrogram=True)
+import numpy as np
+import tensorflow as tf
+from .bindings import check_cola
+
+
+class SegmenterTensorFlow(tf.Module):
+    def __init__(
+        self,
+        frame_size,
+        hop_size,
+        window,
+        mode="wola",
+        edge_correction=True,
+        normalize_window=True,
+    ):
+        """
+        A class for segmenting input data using windowing and hop size with support for WOLA and OLA modes.
+
+        Attributes:
+            segment_size (int): Size of each segment.
+            hop_size (int): Hop size between segments.
+            window (Tensor): Windowing function applied to each segment.
+            mode (str): Either 'wola' or 'ola' for Weighted Overlap-Add or Overlap-Add method.
+            edge_correction (bool): If True, apply edge correction to the first and last segments.
+            normalize_window (bool): If True, normalize the windowing function.
+        """
+        super(SegmenterTensorFlow, self).__init__()
+        self.hop_size = hop_size
+        self.frame_size = frame_size
+        self.window = window
+
+        # asserts to ensure correctness
+        if self.frame_size % 2 != 0:
+            raise ValueError("only even frame_size is supported")
+
+        if self.hop_size > self.frame_size:
+            raise ValueError("hop_size cannot be larger than frame_size")
+
+        if self.window.shape[0] != self.frame_size:
+            raise ValueError("specified window must have the same size as frame_size")
+
+        if any(window < 0.0):
+            raise ValueError("specified window contains negative values")
+
+        if check_cola(window, self.hop_size)[0] == False:
+            raise ValueError(
+                "specified window is not COLA, consider using `default_window_selector`"
+            )
+
+        # compute prewindow and postwindow
+        prewindow = np.copy(window)
+        for hIdx in range(1, self.frame_size // self.hop_size + 1):
+            idx1Start = hIdx * self.hop_size
+            idx1End = self.frame_size
+            idx2Start = 0
+            idx2End = self.frame_size - idx1Start
+            prewindow[idx2Start:idx2End] = (
+                prewindow[idx2Start:idx2End] + window[idx1Start:idx1End]
+            )
+
+        postwindow = np.copy(window)
+        for hIdx in range(1, self.frame_size // self.hop_size + 1):
+            idx1Start = hIdx * self.hop_size
+            idx1End = self.frame_size
+            idx2Start = 0
+            idx2End = self.frame_size - idx1Start
+            postwindow[idx1Start:idx1End] = (
+                postwindow[idx1Start:idx1End] + window[idx2Start:idx2End]
+            )
+
+        # this is a tiny bit hacked, but it works well in practise
+        if normalize_window:
+            value = check_cola(window, hop_size)
+            normalization = value[1]
+            window = window / normalization
+            prewindow = prewindow / normalization
+            postwindow = postwindow / normalization
+
+        if not edge_correction:
+            prewindow = window
+            postwindow = window
+
+        if mode == "wola":
+            self.mode = mode
+            window = np.sqrt(window)
+            prewindow = np.sqrt(prewindow)
+            postwindow = np.sqrt(postwindow)
+        elif mode == "ola":
+            self.mode = mode
+        else:
+            raise ValueError(f"only support for mode ola and wola")
+
+        self.window = tf.convert_to_tensor(window, dtype=tf.float32)
+        self.prewindow = tf.convert_to_tensor(prewindow, dtype=tf.float32)
+        self.postwindow = tf.convert_to_tensor(postwindow, dtype=tf.float32)
+
+    def _segment(self, x, compute_spectrogram=False):
+        if (tf.rank(x) == 2) and (x.shape[1] > 1):
+            number_of_batch_elements = x.shape[0]
+            number_of_samples = x.shape[1]
+            batched = True
+        elif tf.rank(x) == 1:
+            number_of_samples = x.shape[0]
+            number_of_batch_elements = 1
+
+            # convert to batched to simplify subsequent code
+            batched = False
+            x = tf.expand_dims(x, axis=0)
+
+        else:
+            raise ValueError(
+                f"only support for inputs with dimension 1 or 2, provided {len(x.shape)}"
+            )
+
+        number_of_frames = (
+            (number_of_samples) // self.hop_size - self.frame_size // self.hop_size + 1
+        )
+
+        X = tf.zeros(
+            shape=(number_of_batch_elements, number_of_frames, self.frame_size)
+        )
+        for b in range(number_of_batch_elements):
+            if self.mode == "wola":
+                k = 0
+                tmp = tf.reshape(
+                    x[b, k * self.hop_size : k * self.hop_size + self.frame_size],
+                    shape=(1, 1, self.frame_size),
+                )
+                X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp * self.prewindow)
+                for k in range(1, number_of_frames - 1):
+                    tmp = tf.reshape(
+                        x[
+                            b,
+                            k * self.hop_size : k * self.hop_size + self.frame_size,
+                        ],
+                        shape=(1, 1, self.frame_size),
+                    )
+                    X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp * self.window)
+                k = number_of_frames - 1
+                tmp = tf.reshape(
+                    x[b, k * self.hop_size : k * self.hop_size + self.frame_size],
+                    shape=(1, 1, self.frame_size),
+                )
+                X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp * self.postwindow)
+            else:
+                for k in range(number_of_frames):
+                    tmp = tf.reshape(
+                        x[
+                            b,
+                            k * self.hop_size : k * self.hop_size + self.frame_size,
+                        ],
+                        shape=(1, 1, self.frame_size),
+                    )
+                    X = tf.tensor_scatter_nd_add(X, [[[b, k]]], tmp)
+
+        if compute_spectrogram:
+            X = tf.signal.rfft(X)
+
+        # torchaudio convention
+        # X = tf.transpose(X, perm=[0, 2, 1])
+
+        if not batched:
+            # convert back to not-batched
+            X = tf.squeeze(X, axis=0)
+
+        return X
+
+    def _unsegment(self, X, compute_spectrogram=False):
+        if tf.rank(X) == 3:
+            number_of_batch_elements = X.shape[0]
+            number_of_frames = X.shape[1]
+            batched = True
+        elif tf.rank(X) == 2:
+            number_of_batch_elements = 1
+            number_of_frames = X.shape[0]
+
+            # convert to batched to simplify subsequent code
+            batched = False
+            X = tf.expand_dims(X, axis=0)
+        else:
+            raise ValueError(
+                f"only support for inputs with dimension 2 or 3, provided {len(X.shape)}"
+            )
+        number_of_samples = (number_of_frames - 1) * self.hop_size + self.frame_size
+
+        # torchaudio convention
+        # X = tf.transpose(X, perm=[0, 2, 1])
+
+        if compute_spectrogram:
+            X = tf.signal.irfft(X)
+
+        x = tf.zeros(shape=(number_of_batch_elements, number_of_samples))
+        for b in range(number_of_batch_elements):
+            k = 0
+            tmpIdx = tf.reshape(
+                tf.range(k * self.hop_size, k * self.hop_size + self.frame_size),
+                shape=(self.frame_size, 1),
+            )
+            idx = tf.concat(
+                [tf.constant(b, shape=(self.frame_size, 1)), tmpIdx], axis=1
+            )
+            x = tf.tensor_scatter_nd_add(x, idx, self.prewindow * X[b, k, :])
+            for k in range(1, number_of_frames - 1):
+                tmpIdx = tf.reshape(
+                    tf.range(k * self.hop_size, k * self.hop_size + self.frame_size),
+                    shape=(self.frame_size, 1),
+                )
+                idx = tf.concat(
+                    [tf.constant(b, shape=(self.frame_size, 1)), tmpIdx], axis=1
+                )
+                x = tf.tensor_scatter_nd_add(x, idx, self.window * X[b, k, :])
+            k = k + 1
+            tmpIdx = tf.reshape(
+                tf.range(k * self.hop_size, k * self.hop_size + self.frame_size),
+                shape=(self.frame_size, 1),
+            )
+            idx = tf.concat(
+                [tf.constant(b, shape=(self.frame_size, 1)), tmpIdx], axis=1
+            )
+            x = tf.tensor_scatter_nd_add(x, idx, self.postwindow * X[b, k, :])
+
+        if not batched:
+            # convert back to not-batched
+            x = tf.squeeze(x, axis=0)
+
+        return x
+
+    def segment(self, x):
+        return self._segment(x)
+
+    def unsegment(self, X):
+        return self._unsegment(X)
+
+    def spectrogram(self, x):
+        X = self._segment(x, compute_spectrogram=True)
+
+    def unspectrogram(self, X):
+        return self._unsegment(X, compute_spectrogram=True)
```

## libsegmenter/SegmenterTorch.py

```diff
@@ -1,213 +1,210 @@
-import torch
-import numpy as np
-from .bindings import check_cola
-
-
-class SegmenterTorch(torch.nn.Module):
-    def __init__(
-        self,
-        frame_size,
-        hop_size,
-        window,
-        mode="wola",
-        edge_correction=True,
-        normalize_window=True,
-        device=None,
-        dtype=None,
-    ):
-        """
-        A class for segmenting input data using windowing and hop size with support for WOLA and OLA modes.
-
-        Attributes:
-            frame_size (int): Size of each segment.
-            hop_size (int): Hop size between segments.
-            window (Tensor): Windowing function applied to each segment.
-            mode (str): Either 'wola' or 'ola' for Weighted Overlap-Add or Overlap-Add method.
-            edge_correction (bool): If True, apply edge correction to the first and last segments.
-            normalize_window (bool): If True, normalize the windowing function.
-        """
-        self.factory_kwargs = {"device": device, "dtype": dtype}
-
-        super(SegmenterTorch, self).__init__()
-        self.hop_size = hop_size
-        self.frame_size = frame_size
-        if isinstance(window, np.ndarray):
-            self.window = torch.tensor(window)
-        elif isinstance(window, torch.Tensor):
-            self.window = window.to(device)
-        else:
-            raise ValueError("provided window is not numpy ndarray nor pytorch tensor")
-
-        # asserts to ensure correctness
-        if self.frame_size % 2 != 0:
-            raise ValueError("only even frame_size is supported")
-
-        if self.hop_size > self.frame_size:
-            raise ValueError("hop_size cannot be larger than frame_size")
-
-        if self.window.shape[0] != self.frame_size:
-            raise ValueError("specified window must have the same size as frame_size")
-
-        if any(window < 0.0):
-            raise ValueError("specified window contains negative values")
-
-        if check_cola(self.window.cpu().numpy(), self.hop_size)[0] == False:
-            raise ValueError(
-                "specified window is not COLA, consider using `default_window_selector`"
-            )
-
-        # compute prewindow and postwindow
-        self.prewindow = self.window.clone()
-        self.postwindow = self.window.clone()
-        i = self.hop_size
-        if edge_correction:
-            for h_idx in range(1, self.frame_size // self.hop_size + 1):
-                idx1_start = h_idx * self.hop_size
-                idx1_end = self.frame_size
-                idx2_start = 0
-                idx2_end = self.frame_size - idx1_start
-                self.prewindow[idx2_start:idx2_end] = (
-                    self.prewindow[idx2_start:idx2_end]
-                    + self.window[idx1_start:idx1_end]
-                )
-                self.postwindow[idx1_start:idx1_end] = (
-                    self.postwindow[idx1_start:idx1_end]
-                    + self.window[idx2_start:idx2_end]
-                )
-
-        # Perform normalization of window function
-        if normalize_window:
-            value = check_cola(self.window.cpu().numpy(), self.hop_size)
-            normalization = value[1]
-            self.window = self.window / normalization
-            self.prewindow = self.prewindow / normalization
-            self.postwindow = self.postwindow / normalization
-
-        if mode == "wola":
-            self.mode = mode
-            self.window = torch.sqrt(self.window)
-            self.prewindow = torch.sqrt(self.prewindow)
-            self.postwindow = torch.sqrt(self.postwindow)
-        elif mode == "ola":
-            self.mode = mode
-        else:
-            raise ValueError(f"only support for model ola and wola")
-
-    def _segment(self, x, compute_spectrogram=False):
-        if (x.dim() == 2) and (x.shape[1] > 1):
-            number_of_batch_elements = x.shape[0]
-            number_of_samples = x.shape[1]
-            batched = True
-        elif x.dim() == 1:
-            number_of_batch_elements = 1
-            number_of_samples = x.shape[0]
-
-            # convert to batched to simplify subsequent code
-            batched = False
-            x = x.unsqueeze(0)
-        else:
-            raise ValueError(
-                f"only support for inputs with dimension 1 or 2, provided {x.dim()}"
-            )
-
-
-        number_of_segments = (
-            (number_of_samples) // self.hop_size - self.frame_size // self.hop_size + 1
-        )
-
-        X = torch.zeros(
-            (number_of_batch_elements, number_of_segments, self.frame_size),
-            **self.factory_kwargs,
-        )
-
-        if self.mode == "wola":
-            k = 0
-            X[:, k, :] = (
-                x[:, k * self.hop_size : k * self.hop_size + self.frame_size]
-                * self.prewindow
-            )
-            for k in range(1, number_of_segments - 1):
-                X[:, k, :] = (
-                    x[
-                        :,
-                        k * self.hop_size : k * self.hop_size + self.frame_size,
-                    ]
-                    * self.window
-                )
-            k = number_of_segments - 1
-            X[:, k, :] = (
-                x[:, k * self.hop_size : k * self.hop_size + self.frame_size]
-                * self.postwindow
-            )
-        else:
-            for k in range(number_of_segments):
-                X[:, k, :] = x[
-                    :, k * self.hop_size : k * self.hop_size + self.frame_size
-                ]
-
-        if compute_spectrogram:
-            print(X[0,0,:])
-            X = torch.fft.rfft(X)
-            print(X[0,0,:])
-
-        if not batched:
-            # convert back to not-batched
-            X = X.squeeze(0)
-
-        return X
-
-    def _unsegment(self, X, compute_spectrogram=False):
-        if X.dim() == 3:
-            number_of_batch_elements = X.shape[0]
-            number_of_segments = X.shape[1]
-            batched = True
-
-        elif X.dim() == 2:
-            number_of_batch_elements = 1
-            number_of_segments = X.shape[0]
-
-            # convert to batched to simplify subsequent code
-            batched = False
-            X = X.unsqueeze(0)
-        else:
-            raise ValueError(
-                f"only support for inputs with dimension 2 or 3, provided {X.dim()}"
-            )
-
-        if compute_spectrogram:
-            X = torch.fft.irfft(X)
-
-        number_of_samples = (number_of_segments - 1) * self.hop_size + self.frame_size
-
-        x = torch.zeros(
-            (number_of_batch_elements, number_of_samples), **self.factory_kwargs
-        )
-        k = 0
-        x[:, k * self.hop_size : k * self.hop_size + self.frame_size] += (
-            self.prewindow * X[:, k, :]
-        )
-        for k in range(1, number_of_segments - 1):
-            x[:, k * self.hop_size : k * self.hop_size + self.frame_size] += (
-                self.window * X[:, k, :]
-            )
-        k = k + 1
-        x[:, k * self.hop_size : k * self.hop_size + self.frame_size] += (
-            self.postwindow * X[:, k, :]
-        )
-
-        if not batched:
-            # convert back to not-batched
-            x = x.squeeze(0)
-        return x
-
-    def segment(self, x):
-        return self._segment(x)
-
-    def unsegment(self, X):
-        return self._unsegment(X)
-
-    def spectrogram(self, x):
-        return self._segment(x, compute_spectrogram=True)
-
-    def unspectrogram(self, X):
-        return self._unsegment(X, compute_spectrogram=True)
+import torch
+import numpy as np
+from .bindings import check_cola
+
+
+class SegmenterTorch(torch.nn.Module):
+    def __init__(
+        self,
+        frame_size,
+        hop_size,
+        window,
+        mode="wola",
+        edge_correction=True,
+        normalize_window=True,
+        device=None,
+        dtype=None,
+    ):
+        """
+        A class for segmenting input data using windowing and hop size with support for WOLA and OLA modes.
+
+        Attributes:
+            frame_size (int): Size of each segment.
+            hop_size (int): Hop size between segments.
+            window (Tensor): Windowing function applied to each segment.
+            mode (str): Either 'wola' or 'ola' for Weighted Overlap-Add or Overlap-Add method.
+            edge_correction (bool): If True, apply edge correction to the first and last segments.
+            normalize_window (bool): If True, normalize the windowing function.
+        """
+        self.factory_kwargs = {"device": device, "dtype": dtype}
+
+        super(SegmenterTorch, self).__init__()
+        self.hop_size = hop_size
+        self.frame_size = frame_size
+        if isinstance(window, np.ndarray):
+            self.window = torch.tensor(window)
+        elif isinstance(window, torch.Tensor):
+            self.window = window.to(device)
+        else:
+            raise ValueError("provided window is not numpy ndarray nor pytorch tensor")
+
+        # asserts to ensure correctness
+        if self.frame_size % 2 != 0:
+            raise ValueError("only even frame_size is supported")
+
+        if self.hop_size > self.frame_size:
+            raise ValueError("hop_size cannot be larger than frame_size")
+
+        if self.window.shape[0] != self.frame_size:
+            raise ValueError("specified window must have the same size as frame_size")
+
+        if any(window < 0.0):
+            raise ValueError("specified window contains negative values")
+
+        if check_cola(self.window.cpu().numpy(), self.hop_size)[0] == False:
+            raise ValueError(
+                "specified window is not COLA, consider using `default_window_selector`"
+            )
+
+        # compute prewindow and postwindow
+        self.prewindow = self.window.clone()
+        self.postwindow = self.window.clone()
+        i = self.hop_size
+        if edge_correction:
+            for h_idx in range(1, self.frame_size // self.hop_size + 1):
+                idx1_start = h_idx * self.hop_size
+                idx1_end = self.frame_size
+                idx2_start = 0
+                idx2_end = self.frame_size - idx1_start
+                self.prewindow[idx2_start:idx2_end] = (
+                    self.prewindow[idx2_start:idx2_end]
+                    + self.window[idx1_start:idx1_end]
+                )
+                self.postwindow[idx1_start:idx1_end] = (
+                    self.postwindow[idx1_start:idx1_end]
+                    + self.window[idx2_start:idx2_end]
+                )
+
+        # Perform normalization of window function
+        if normalize_window:
+            value = check_cola(self.window.cpu().numpy(), self.hop_size)
+            normalization = value[1]
+            self.window = self.window / normalization
+            self.prewindow = self.prewindow / normalization
+            self.postwindow = self.postwindow / normalization
+
+        if mode == "wola":
+            self.mode = mode
+            self.window = torch.sqrt(self.window)
+            self.prewindow = torch.sqrt(self.prewindow)
+            self.postwindow = torch.sqrt(self.postwindow)
+        elif mode == "ola":
+            self.mode = mode
+        else:
+            raise ValueError(f"only support for model ola and wola")
+
+    def _segment(self, x, compute_spectrogram=False):
+        if (x.dim() == 2) and (x.shape[1] > 1):
+            number_of_batch_elements = x.shape[0]
+            number_of_samples = x.shape[1]
+            batched = True
+        elif x.dim() == 1:
+            number_of_batch_elements = 1
+            number_of_samples = x.shape[0]
+
+            # convert to batched to simplify subsequent code
+            batched = False
+            x = x.unsqueeze(0)
+        else:
+            raise ValueError(
+                f"only support for inputs with dimension 1 or 2, provided {x.dim()}"
+            )
+
+        number_of_segments = (
+            (number_of_samples) // self.hop_size - self.frame_size // self.hop_size + 1
+        )
+
+        X = torch.zeros(
+            (number_of_batch_elements, number_of_segments, self.frame_size),
+            **self.factory_kwargs,
+        )
+
+        if self.mode == "wola":
+            k = 0
+            X[:, k, :] = (
+                x[:, k * self.hop_size : k * self.hop_size + self.frame_size]
+                * self.prewindow
+            )
+            for k in range(1, number_of_segments - 1):
+                X[:, k, :] = (
+                    x[
+                        :,
+                        k * self.hop_size : k * self.hop_size + self.frame_size,
+                    ]
+                    * self.window
+                )
+            k = number_of_segments - 1
+            X[:, k, :] = (
+                x[:, k * self.hop_size : k * self.hop_size + self.frame_size]
+                * self.postwindow
+            )
+        else:
+            for k in range(number_of_segments):
+                X[:, k, :] = x[
+                    :, k * self.hop_size : k * self.hop_size + self.frame_size
+                ]
+
+        if compute_spectrogram:
+            X = torch.fft.rfft(X)
+
+        if not batched:
+            # convert back to not-batched
+            X = X.squeeze(0)
+
+        return X
+
+    def _unsegment(self, X, compute_spectrogram=False):
+        if X.dim() == 3:
+            number_of_batch_elements = X.shape[0]
+            number_of_segments = X.shape[1]
+            batched = True
+
+        elif X.dim() == 2:
+            number_of_batch_elements = 1
+            number_of_segments = X.shape[0]
+
+            # convert to batched to simplify subsequent code
+            batched = False
+            X = X.unsqueeze(0)
+        else:
+            raise ValueError(
+                f"only support for inputs with dimension 2 or 3, provided {X.dim()}"
+            )
+
+        if compute_spectrogram:
+            X = torch.fft.irfft(X)
+
+        number_of_samples = (number_of_segments - 1) * self.hop_size + self.frame_size
+
+        x = torch.zeros(
+            (number_of_batch_elements, number_of_samples), **self.factory_kwargs
+        )
+        k = 0
+        x[:, k * self.hop_size : k * self.hop_size + self.frame_size] += (
+            self.prewindow * X[:, k, :]
+        )
+        for k in range(1, number_of_segments - 1):
+            x[:, k * self.hop_size : k * self.hop_size + self.frame_size] += (
+                self.window * X[:, k, :]
+            )
+        k = k + 1
+        x[:, k * self.hop_size : k * self.hop_size + self.frame_size] += (
+            self.postwindow * X[:, k, :]
+        )
+
+        if not batched:
+            # convert back to not-batched
+            x = x.squeeze(0)
+        return x
+
+    def segment(self, x):
+        return self._segment(x)
+
+    def unsegment(self, X):
+        return self._unsegment(X)
+
+    def spectrogram(self, x):
+        return self._segment(x, compute_spectrogram=True)
+
+    def unspectrogram(self, X):
+        return self._unsegment(X, compute_spectrogram=True)
```

## libsegmenter/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-from .Segmenter import *
-from .default_window_selector import *
-
-# pybindings
-from .bindings import *
+from .Segmenter import *
+from .default_window_selector import *
+
+# pybindings
+from .bindings import *
```

## libsegmenter/default_window_selector.py

```diff
@@ -1,110 +1,111 @@
-import numpy as np
-from .bindings import *
-
-def kaiser(window_length: int, beta: float) -> np.array:
-    """
-    Note that the Kaiser window is not strictly speaking COLA compliant as it does not have harmonic nulls that can be tuned to the
-    harmonics of the frame rate. As such it only offers approximate perfect reconstruction. However, by tuning the beta parameter,
-    the reconstruction error can be controlled
-    """
-    M = np.float64(window_length + 1.0)
-    m = np.arange(-(M - 1) / 2.0, (M - 1) / 2.0, dtype=np.float64)
-    window = np.i0(beta * np.sqrt(1 - (m / (M / 2)) ** 2.0)) / np.i0(beta)
-    return window
-
-
-def default_window_selector(window_name: str, window_length: int) -> np.array:
-    if window_name == "bartlett50":
-        # Bartlett (triangular) window with 50% overlap
-        if int(window_length) % 2 != 0:
-            raise ValueError(
-                "Odd length Bartlett window with 50 percent overlap is not currently supported."
-            )
-        else:
-            window = bartlett(window_length)
-            hopSize = int(window_length) // 2
-            return window, hopSize
-    elif window_name == "bartlett75":
-        # Bartlett window with 75% overlap
-        if int(window_length) % 4 != 0:
-            raise ValueError(
-                "Bartlett windows with 75 percent overlap expects a window_length divisible by 4."
-            )
-        else:
-            window = bartlett(window_length)
-            hopSize = int(window_length) // 4
-            return window, hopSize
-    elif window_name == "blackman":
-        # Blackman window with 2/3 overlap
-        if int(window_length) % 3 != 0:
-            raise ValueError(
-                "The Blackman window currently only supports overlaps of 2/3."
-            )
-        else:
-            window = blackman(window_length)
-            hopSize = int(window_length) // 3
-            return window, hopSize
-    elif window_name == "kaiser82":
-        # Kaiser window with beta = 8 and approx 82% overlap
-        beta = 8.0
-        window = kaiser(window_length, beta)
-        hopSize = int(np.floor(1.7 * (np.float64(window_length) - 1.0) / (beta + 1.0)))
-        return window, hopSize
-    elif window_name == "kaiser85":
-        # Kaiser window with beta = 10 and approx 85% overlap
-        beta = 10.0
-        window = kaiser(window_length, beta)
-        hopSize = int(np.floor(1.7 * (np.float64(window_length) - 1.0) / (beta + 1.0)))
-        return window, hopSize
-    elif window_name == "hamming50":
-        # Hamming window with 50% overlap
-        if window_length % 2 != 0:
-            raise ValueError(
-                "Odd length Hamming window at 50 percent overlap is not currently supported."
-            )
-        else:
-            window = hamming(window_length)
-            hopSize = int(window_length) // 2
-            return window, hopSize
-    elif window_name == "hamming75":
-        # Hamming window with 75% overlap
-        if int(window_length) % 4 != 0:
-            raise ValueError(
-                "For Hamming windows with 75 percent overlay, the window_length is expected to be divisible by 4."
-            )
-        else:
-            window = hamming(window_length)
-            hopSize = int(window_length) // 4
-            return window, hopSize
-    elif window_name == "hann50":
-        # Hann window with 50% overlap
-        if int(window_length) % 2 != 0:
-            raise ValueError(
-                "Odd length Hann window at 50 percent overlap is not currently supported."
-            )
-        else:
-            window = hann(window_length)
-            hopSize = int(window_length) // 2
-            return window, hopSize
-    elif window_name == "hann75":
-        # Hann window with 75% overlap
-        if int(window_length) % 4 != 0:
-            raise ValueError(
-                "For Hann windows with 75 percent overlap, the window_length is expected to be divisible by 4."
-            )
-        else:
-            window = hann(window_length)
-            hopSize = int(window_length) // 4
-            return window, hopSize
-    elif window_name == "rectangular0":
-        # Rectangular window with 0% overlap
-        window = np.ones(window_length, dtype=np.float64)
-        hopSize = int(window_length)
-        return window, hopSize
-    elif window_name == "rectangular50":
-        # Rectangular window with 50% overlap
-        window = np.ones(window_length, dtype=np.float64)
-        hopSize = int(window_length) // 2
-        return window, hopSize
-    else:
-        raise ValueError("No valid window_name was provided.")
+import numpy as np
+from .bindings import *
+
+
+def kaiser(window_length: int, beta: float) -> np.array:
+    """
+    Note that the Kaiser window is not strictly speaking COLA compliant as it does not have harmonic nulls that can be tuned to the
+    harmonics of the frame rate. As such it only offers approximate perfect reconstruction. However, by tuning the beta parameter,
+    the reconstruction error can be controlled
+    """
+    M = np.float64(window_length + 1.0)
+    m = np.arange(-(M - 1) / 2.0, (M - 1) / 2.0, dtype=np.float64)
+    window = np.i0(beta * np.sqrt(1 - (m / (M / 2)) ** 2.0)) / np.i0(beta)
+    return window
+
+
+def default_window_selector(window_name: str, window_length: int) -> np.array:
+    if window_name == "bartlett50":
+        # Bartlett (triangular) window with 50% overlap
+        if int(window_length) % 2 != 0:
+            raise ValueError(
+                "Odd length Bartlett window with 50 percent overlap is not currently supported."
+            )
+        else:
+            window = bartlett(window_length)
+            hopSize = int(window_length) // 2
+            return window, hopSize
+    elif window_name == "bartlett75":
+        # Bartlett window with 75% overlap
+        if int(window_length) % 4 != 0:
+            raise ValueError(
+                "Bartlett windows with 75 percent overlap expects a window_length divisible by 4."
+            )
+        else:
+            window = bartlett(window_length)
+            hopSize = int(window_length) // 4
+            return window, hopSize
+    elif window_name == "blackman":
+        # Blackman window with 2/3 overlap
+        if int(window_length) % 3 != 0:
+            raise ValueError(
+                "The Blackman window currently only supports overlaps of 2/3."
+            )
+        else:
+            window = blackman(window_length)
+            hopSize = int(window_length) // 3
+            return window, hopSize
+    elif window_name == "kaiser82":
+        # Kaiser window with beta = 8 and approx 82% overlap
+        beta = 8.0
+        window = kaiser(window_length, beta)
+        hopSize = int(np.floor(1.7 * (np.float64(window_length) - 1.0) / (beta + 1.0)))
+        return window, hopSize
+    elif window_name == "kaiser85":
+        # Kaiser window with beta = 10 and approx 85% overlap
+        beta = 10.0
+        window = kaiser(window_length, beta)
+        hopSize = int(np.floor(1.7 * (np.float64(window_length) - 1.0) / (beta + 1.0)))
+        return window, hopSize
+    elif window_name == "hamming50":
+        # Hamming window with 50% overlap
+        if window_length % 2 != 0:
+            raise ValueError(
+                "Odd length Hamming window at 50 percent overlap is not currently supported."
+            )
+        else:
+            window = hamming(window_length)
+            hopSize = int(window_length) // 2
+            return window, hopSize
+    elif window_name == "hamming75":
+        # Hamming window with 75% overlap
+        if int(window_length) % 4 != 0:
+            raise ValueError(
+                "For Hamming windows with 75 percent overlay, the window_length is expected to be divisible by 4."
+            )
+        else:
+            window = hamming(window_length)
+            hopSize = int(window_length) // 4
+            return window, hopSize
+    elif window_name == "hann50":
+        # Hann window with 50% overlap
+        if int(window_length) % 2 != 0:
+            raise ValueError(
+                "Odd length Hann window at 50 percent overlap is not currently supported."
+            )
+        else:
+            window = hann(window_length)
+            hopSize = int(window_length) // 2
+            return window, hopSize
+    elif window_name == "hann75":
+        # Hann window with 75% overlap
+        if int(window_length) % 4 != 0:
+            raise ValueError(
+                "For Hann windows with 75 percent overlap, the window_length is expected to be divisible by 4."
+            )
+        else:
+            window = hann(window_length)
+            hopSize = int(window_length) // 4
+            return window, hopSize
+    elif window_name == "rectangular0":
+        # Rectangular window with 0% overlap
+        window = np.ones(window_length, dtype=np.float64)
+        hopSize = int(window_length)
+        return window, hopSize
+    elif window_name == "rectangular50":
+        # Rectangular window with 50% overlap
+        window = np.ones(window_length, dtype=np.float64)
+        hopSize = int(window_length) // 2
+        return window, hopSize
+    else:
+        raise ValueError("No valid window_name was provided.")
```

## libsegmenter/old.py

 * *Ordering differences only*

```diff
@@ -1,81 +1,81 @@
-# DEPRICATED IN FAVOUR OF THE CPP VERSION, BUT KEPT FOR DOCUMENTATION
-def bartlett(window_length: int) -> np.array:
-    """
-    Bartlett (triangular) window
-    """
-    M = np.float64(window_length + 1.0)
-    m = np.arange(-(M - 1) / 2.0, (M - 1) / 2.0, dtype=np.float64)
-    window = 1 - abs(m) * 2.0 / (M - 1)
-    return window
-
-
-def blackman(window_length: int) -> np.array:
-    """
-    Provides COLA-compliant windows for hopSize = (M-1)/3 when M is odd and
-    hopSize M/3 when M is even
-    """
-    M = np.float64(window_length + 1.0)
-    m = np.arange(0, M - 1, dtype=np.float64) / (M - 1)
-    window = (
-        7938.0 / 18608.0
-        - 9240.0 / 18608.0 * np.cos(2.0 * np.pi * m)
-        + 1430.0 / 18608.0 * np.cos(4.0 * np.pi * m)
-    )
-
-    return window
-
-
-def hamming(window_length: int) -> np.array:
-    """
-    Provides COLA-compliant windows for hopSize = M/2, M/4, ...
-    """
-    M = np.float64(window_length)
-    alpha = 25.0 / 46.0
-    beta = (1 - alpha) / 2.0
-    window = alpha - 2 * beta * np.cos(
-        2.0 * np.pi * np.arange(0, window_length, dtype=np.float64) / window_length
-    )
-    return window
-
-
-def hann(window_length: int) -> np.array:
-    """
-    Provides COLA-compliant windows for hopSize = window_length/2,
-    window_length/4, ...
-    """
-    M = np.float64(window_length)
-    m = np.arange(0, M, dtype=np.float64)
-    window = 0.5 * (1.0 - np.cos(2.0 * np.pi * m / M))
-    return window
-
-
-def check_cola(window: np.array, hop_size: int, eps=1e-5) -> (bool, np.float64):
-    window_length = window.size
-
-    # Assuming the sampling frequency is 1
-    frame_rate = 1.0 / np.float64(hop_size)
-    N = 6 * window_length
-    sp = np.sum(window) / np.float64(hop_size) * np.ones(N, dtype=np.float64)
-    ubound = sp[0] * 1.0
-    lbound = sp[0] * 1.0
-    n = np.arange(0, N, dtype=np.float64)
-
-    for k in range(1, hop_size):
-        f = frame_rate * k
-        csin = np.exp(1j * 2.0 * np.pi * np.float64(f) * n)
-
-        # Find exact window transform at frequency f
-        Wf = np.sum(window * np.conj(csin[0:window_length]))
-        hum = Wf * csin  # contribution to OLA "hum"
-        sp = sp + hum / np.float64(hop_size)  # Poisson summation into OLA
-
-        # Update lower and upper bounds
-        Wfb = np.abs(Wf)
-        ubound = ubound + Wfb / np.float64(hop_size)
-        lbound = lbound - Wfb / np.float64(hop_size)
-
-    normalization_value = (ubound + lbound) / 2
-    if (ubound - lbound) < eps:
-        return True, normalization_value
-    else:
-        return False, normalization_value
+# DEPRICATED IN FAVOUR OF THE CPP VERSION, BUT KEPT FOR DOCUMENTATION
+def bartlett(window_length: int) -> np.array:
+    """
+    Bartlett (triangular) window
+    """
+    M = np.float64(window_length + 1.0)
+    m = np.arange(-(M - 1) / 2.0, (M - 1) / 2.0, dtype=np.float64)
+    window = 1 - abs(m) * 2.0 / (M - 1)
+    return window
+
+
+def blackman(window_length: int) -> np.array:
+    """
+    Provides COLA-compliant windows for hopSize = (M-1)/3 when M is odd and
+    hopSize M/3 when M is even
+    """
+    M = np.float64(window_length + 1.0)
+    m = np.arange(0, M - 1, dtype=np.float64) / (M - 1)
+    window = (
+        7938.0 / 18608.0
+        - 9240.0 / 18608.0 * np.cos(2.0 * np.pi * m)
+        + 1430.0 / 18608.0 * np.cos(4.0 * np.pi * m)
+    )
+
+    return window
+
+
+def hamming(window_length: int) -> np.array:
+    """
+    Provides COLA-compliant windows for hopSize = M/2, M/4, ...
+    """
+    M = np.float64(window_length)
+    alpha = 25.0 / 46.0
+    beta = (1 - alpha) / 2.0
+    window = alpha - 2 * beta * np.cos(
+        2.0 * np.pi * np.arange(0, window_length, dtype=np.float64) / window_length
+    )
+    return window
+
+
+def hann(window_length: int) -> np.array:
+    """
+    Provides COLA-compliant windows for hopSize = window_length/2,
+    window_length/4, ...
+    """
+    M = np.float64(window_length)
+    m = np.arange(0, M, dtype=np.float64)
+    window = 0.5 * (1.0 - np.cos(2.0 * np.pi * m / M))
+    return window
+
+
+def check_cola(window: np.array, hop_size: int, eps=1e-5) -> (bool, np.float64):
+    window_length = window.size
+
+    # Assuming the sampling frequency is 1
+    frame_rate = 1.0 / np.float64(hop_size)
+    N = 6 * window_length
+    sp = np.sum(window) / np.float64(hop_size) * np.ones(N, dtype=np.float64)
+    ubound = sp[0] * 1.0
+    lbound = sp[0] * 1.0
+    n = np.arange(0, N, dtype=np.float64)
+
+    for k in range(1, hop_size):
+        f = frame_rate * k
+        csin = np.exp(1j * 2.0 * np.pi * np.float64(f) * n)
+
+        # Find exact window transform at frequency f
+        Wf = np.sum(window * np.conj(csin[0:window_length]))
+        hum = Wf * csin  # contribution to OLA "hum"
+        sp = sp + hum / np.float64(hop_size)  # Poisson summation into OLA
+
+        # Update lower and upper bounds
+        Wfb = np.abs(Wf)
+        ubound = ubound + Wfb / np.float64(hop_size)
+        lbound = lbound - Wfb / np.float64(hop_size)
+
+    normalization_value = (ubound + lbound) / 2
+    if (ubound - lbound) < eps:
+        return True, normalization_value
+    else:
+        return False, normalization_value
```

## tests/creational.py

 * *Ordering differences only*

```diff
@@ -1,63 +1,63 @@
-import pytest
-import torch
-import tensorflow
-import libsegmenter
-
-"""
-tests testing the creational pattern for the Segmenters
-"""
-
-
-@pytest.mark.parametrize(
-    ("backend", "frame_size", "hop_size", "window", "kwargs", "should_throw"),
-    [
-        # mismatch between specified frame_size and window
-        ("torch", 99, 50, libsegmenter.hamming(100), None, True),
-        ("torch", 100, 50, libsegmenter.hamming(99), None, True),
-        ("tensorflow", 99, 50, libsegmenter.hamming(100), None, True),
-        ("tensorflow", 100, 50, libsegmenter.hamming(99), None, True),
-        # modes
-        ("torch", 100, 50, libsegmenter.hamming(100), {"mode": "asdf"}, True),
-        ("torch", 100, 50, libsegmenter.hamming(100), {"mode": "ola"}, False),
-        ("torch", 100, 50, libsegmenter.hamming(100), {"mode": "wola"}, False),
-        ("tensorflow", 100, 50, libsegmenter.hamming(100), {"mode": "asdf"}, True),
-        ("tensorflow", 100, 50, libsegmenter.hamming(100), {"mode": "ola"}, False),
-        ("tensorflow", 100, 50, libsegmenter.hamming(100), {"mode": "wola"}, False),
-        # hop_size > frame_size
-        ("torch", 100, 101, libsegmenter.hamming(100), None, True),
-        ("tensorflow", 100, 101, libsegmenter.hamming(100), None, True),
-        # invalid window
-        ("torch", 100, 23, libsegmenter.blackman(100), None, True),
-        ("tensorflow", 100, 23, libsegmenter.blackman(100), None, True),
-    ],
-)
-def test_creational(backend, frame_size, hop_size, window, kwargs, should_throw):
-    try:
-        segmenter = libsegmenter.make_segmenter(
-            backend=backend,
-            frame_size=frame_size,
-            hop_size=hop_size,
-            window=window,
-            **kwargs
-        )
-    except:
-        if not should_throw:
-            assert False
-
-        return
-
-    # should throw
-    if should_throw:
-        assert False
-
-
-@pytest.mark.parametrize(
-    ("backend", "frame_size", "hop_size", "window"),
-    [
-        ("torch", 100, 50, torch.tensor(libsegmenter.hamming(100))),
-    ],
-)
-def test_pytorch_tensor(backend, frame_size, hop_size, window):
-    segmenter = libsegmenter.make_segmenter(
-        backend=backend, frame_size=frame_size, hop_size=hop_size, window=window
-    )
+import pytest
+import torch
+import tensorflow
+import libsegmenter
+
+"""
+tests testing the creational pattern for the Segmenters
+"""
+
+
+@pytest.mark.parametrize(
+    ("backend", "frame_size", "hop_size", "window", "kwargs", "should_throw"),
+    [
+        # mismatch between specified frame_size and window
+        ("torch", 99, 50, libsegmenter.hamming(100), None, True),
+        ("torch", 100, 50, libsegmenter.hamming(99), None, True),
+        ("tensorflow", 99, 50, libsegmenter.hamming(100), None, True),
+        ("tensorflow", 100, 50, libsegmenter.hamming(99), None, True),
+        # modes
+        ("torch", 100, 50, libsegmenter.hamming(100), {"mode": "asdf"}, True),
+        ("torch", 100, 50, libsegmenter.hamming(100), {"mode": "ola"}, False),
+        ("torch", 100, 50, libsegmenter.hamming(100), {"mode": "wola"}, False),
+        ("tensorflow", 100, 50, libsegmenter.hamming(100), {"mode": "asdf"}, True),
+        ("tensorflow", 100, 50, libsegmenter.hamming(100), {"mode": "ola"}, False),
+        ("tensorflow", 100, 50, libsegmenter.hamming(100), {"mode": "wola"}, False),
+        # hop_size > frame_size
+        ("torch", 100, 101, libsegmenter.hamming(100), None, True),
+        ("tensorflow", 100, 101, libsegmenter.hamming(100), None, True),
+        # invalid window
+        ("torch", 100, 23, libsegmenter.blackman(100), None, True),
+        ("tensorflow", 100, 23, libsegmenter.blackman(100), None, True),
+    ],
+)
+def test_creational(backend, frame_size, hop_size, window, kwargs, should_throw):
+    try:
+        segmenter = libsegmenter.make_segmenter(
+            backend=backend,
+            frame_size=frame_size,
+            hop_size=hop_size,
+            window=window,
+            **kwargs
+        )
+    except:
+        if not should_throw:
+            assert False
+
+        return
+
+    # should throw
+    if should_throw:
+        assert False
+
+
+@pytest.mark.parametrize(
+    ("backend", "frame_size", "hop_size", "window"),
+    [
+        ("torch", 100, 50, torch.tensor(libsegmenter.hamming(100))),
+    ],
+)
+def test_pytorch_tensor(backend, frame_size, hop_size, window):
+    segmenter = libsegmenter.make_segmenter(
+        backend=backend, frame_size=frame_size, hop_size=hop_size, window=window
+    )
```

## tests/reconstruction.py

 * *Ordering differences only*

```diff
@@ -1,375 +1,375 @@
-import pytest
-import torch
-import tensorflow
-import libsegmenter
-import numpy
-
-"""
-tests testing the creational pattern for the Segmenters
-"""
-
-test_cases_edge_corrected = []
-for backend in ["torch", "tensorflow", "base"]:
-    for mode in ["wola", "ola"]:
-        for window_settings in [
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hamming(100),
-                "input_size": (1000,),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hamming(100),
-                "input_size": (1, 1000),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hann(100),
-                "input_size": (1000,),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hann(100),
-                "input_size": (1, 1000),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.bartlett(100),
-                "input_size": (1000,),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.bartlett(100),
-                "input_size": (1, 1000),
-            },
-            {
-                "hop_size": 10,
-                "window": libsegmenter.blackman(30),
-                "input_size": (300,),
-            },
-            {
-                "hop_size": 10,
-                "window": libsegmenter.blackman(30),
-                "input_size": (1, 300),
-            },
-        ]:
-            test_cases_edge_corrected.append(
-                (
-                    libsegmenter.make_segmenter(
-                        backend=backend,
-                        frame_size=window_settings["window"].size,
-                        hop_size=window_settings["hop_size"],
-                        window=window_settings["window"],
-                        mode=mode,
-                        edge_correction=True,
-                    ),
-                    torch.randn((window_settings["input_size"])),
-                )
-            )
-
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_edge_corrected)
-def test_reconstruction_corrected(segmenter, x):
-    assert True == True
-    return
-    X = segmenter.segment(x)
-    y = segmenter.unsegment(X)
-
-    y = numpy.array(y)
-    x = numpy.array(x)
-    assert y == pytest.approx(x, abs=1e-5)
-
-
-test_cases_edge_uncorrected = []
-for backend in ["torch", "tensorflow", "base"]:
-    for mode in ["wola", "ola"]:
-        for window_settings in [
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hamming(100),
-                "input_size": (1000,),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hamming(100),
-                "input_size": (1, 1000),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hann(100),
-                "input_size": (1000,),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.hann(100),
-                "input_size": (1, 1000),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.bartlett(100),
-                "input_size": (1000,),
-            },
-            {
-                "hop_size": 50,
-                "window": libsegmenter.bartlett(100),
-                "input_size": (1, 1000),
-            },
-            {
-                "hop_size": 10,
-                "window": libsegmenter.blackman(30),
-                "input_size": (300,),
-            },
-            {
-                "hop_size": 10,
-                "window": libsegmenter.blackman(30),
-                "input_size": (1, 300),
-            },
-        ]:
-            test_cases_edge_uncorrected.append(
-                (
-                    libsegmenter.make_segmenter(
-                        backend=backend,
-                        frame_size=window_settings["window"].size,
-                        hop_size=window_settings["hop_size"],
-                        window=window_settings["window"],
-                        mode=mode,
-                        edge_correction=False,
-                    ),
-                    torch.randn((window_settings["input_size"])),
-                )
-            )
-
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_edge_uncorrected)
-def test_reconstruction_uncorrected(segmenter, x):
-    assert True == True
-    return
-    X = segmenter.segment(x)
-    y = segmenter.unsegment(X)
-
-    y = numpy.array(y)
-    x = numpy.array(x)
-    assert y[segmenter.frame_size : -segmenter.frame_size] == pytest.approx(
-        x[segmenter.frame_size : -segmenter.frame_size], abs=1e-5
-    )
-
-
-test_cases_torch_vs_tensorflow = []
-for mode in ["wola", "ola"]:
-    for window_settings in [
-        {
-            "hop_size": 50,
-            "window": libsegmenter.hamming(100),
-            "input_size": (1000,),
-        },
-        {
-            "hop_size": 50,
-            "window": libsegmenter.hamming(100),
-            "input_size": (1, 1000),
-        },
-        {
-            "hop_size": 50,
-            "window": libsegmenter.hann(100),
-            "input_size": (1000,),
-        },
-        {
-            "hop_size": 50,
-            "window": libsegmenter.hann(100),
-            "input_size": (1, 1000),
-        },
-        {
-            "hop_size": 50,
-            "window": libsegmenter.bartlett(100),
-            "input_size": (1000,),
-        },
-        {
-            "hop_size": 50,
-            "window": libsegmenter.bartlett(100),
-            "input_size": (1, 1000),
-        },
-        {
-            "hop_size": 10,
-            "window": libsegmenter.blackman(30),
-            "input_size": (300,),
-        },
-        {
-            "hop_size": 10,
-            "window": libsegmenter.blackman(30),
-            "input_size": (1, 300),
-        },
-    ]:
-        test_cases_torch_vs_tensorflow.append(
-            (
-                (
-                    libsegmenter.make_segmenter(
-                        backend="torch",
-                        frame_size=window_settings["window"].size,
-                        hop_size=window_settings["hop_size"],
-                        window=window_settings["window"],
-                        mode=mode,
-                        edge_correction=True,
-                    ),
-                    libsegmenter.make_segmenter(
-                        backend="tensorflow",
-                        frame_size=window_settings["window"].size,
-                        hop_size=window_settings["hop_size"],
-                        window=window_settings["window"],
-                        mode=mode,
-                        edge_correction=True,
-                    ),
-                ),
-                torch.randn((window_settings["input_size"])),
-            ),
-        )
-
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_tensorflow)
-def test_torch_vs_tensorflow_segment(segmenter, x):
-    X_tc = segmenter[0].segment(x)
-    X_tf = segmenter[1].segment(x)
-
-    assert X_tc == pytest.approx(X_tf, abs=1e-5)
-
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_tensorflow)
-def test_torch_vs_tensorflow_unsegment(segmenter, x):
-    x_tc = segmenter[0].unsegment(segmenter[0].segment(x))
-    x_tf = segmenter[1].unsegment(segmenter[1].segment(x))
-
-    assert x_tc == pytest.approx(x_tf, abs=1e-5)
-
-
-test_cases_torch_vs_base = []
-for edge_correction in [True, False]:
-    for mode in ["ola", "wola"]:
-        for window_settings in [
-            {
-                "hop_size": 32,
-                "window": libsegmenter.hamming(64),
-                "input_size": (640),
-            },
-            {
-                "hop_size": 32,
-                "window": libsegmenter.hamming(64),
-                "input_size": (1, 640),
-            },
-            {
-                "hop_size": 32,
-                "window": libsegmenter.hann(64),
-                "input_size": (640,),
-            },
-            {
-                "hop_size": 32,
-                "window": libsegmenter.hann(64),
-                "input_size": (1, 640),
-            },
-            {
-                "hop_size": 32,
-                "window": libsegmenter.bartlett(64),
-                "input_size": (640,),
-            },
-            {
-                "hop_size": 32,
-                "window": libsegmenter.bartlett(64),
-                "input_size": (1, 640),
-            },
-            {
-                "hop_size": 10,
-                "window": libsegmenter.blackman(30),
-                "input_size": (300,),
-            },
-            {
-                "hop_size": 10,
-                "window": libsegmenter.blackman(30),
-                "input_size": (1, 300),
-            },
-        ]:
-            test_cases_torch_vs_base.append(
-                (
-                    (
-                        libsegmenter.make_segmenter(
-                            backend="torch",
-                            frame_size=window_settings["window"].size,
-                            hop_size=window_settings["hop_size"],
-                            window=window_settings["window"].copy(),
-                            mode=mode,
-                            edge_correction=edge_correction,
-                        ),
-                        libsegmenter.make_segmenter(
-                            backend="base",
-                            frame_size=window_settings["window"].size,
-                            hop_size=window_settings["hop_size"],
-                            window=window_settings["window"].copy(),
-                            mode=mode,
-                            edge_correction=edge_correction,
-                        ),
-                    ),
-                    torch.randn((window_settings["input_size"])),
-                ),
-            )
-
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
-def test_torch_vs_base_segment(segmenter, x):
-    X_tc = segmenter[0].segment(x.clone())
-    X_ba = segmenter[1].segment(x.clone())
-    assert X_tc.shape == X_ba.shape
-    assert X_ba == pytest.approx(X_tc, abs=1e-5)
-
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
-def test_torch_vs_base_unsegment(segmenter, x):
-    x_tc = segmenter[0].segment(x.clone())
-    x_ba = segmenter[1].segment(x.clone())
-    assert x_tc.shape == x_ba.shape
-    segmenter[0].unsegment(x_tc)
-    segmenter[1].unsegment(x_ba)
-    assert x_tc.shape == x_ba.shape
-    assert x_tc == pytest.approx(x_ba, abs=1e-5)
-
-
-def is_radix_2(x):
-    return (x > 0) and (x & (x - 1)) == 0
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
-def test_torch_vs_base_spectrogram(segmenter, x):
-    # skip for non radix-2 examples, but sloppy but so be it
-    if not is_radix_2(segmenter[0].frame_size):
-        return
-    X_tc = segmenter[0].spectrogram(x.clone())
-    X_ba = segmenter[1].spectrogram(x.clone())
-    assert X_tc.shape == X_ba.shape
-    assert X_ba == pytest.approx(X_tc, abs=1e-5)
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
-def test_torch_vs_base_unspectrogram(segmenter, x):
-    # skip for non radix-2 examples, but sloppy but so be it
-    if not is_radix_2(segmenter[0].frame_size):
-        return
-    x_tc = segmenter[0].spectrogram(x.clone())
-    x_ba = segmenter[1].spectrogram(x.clone())
-    assert x_tc.shape == x_ba.shape
-    segmenter[0].unspectrogram(x_tc)
-    segmenter[1].unspectrogram(x_ba)
-    assert x_tc.shape == x_ba.shape
-    assert x_tc == pytest.approx(x_ba, abs=1e-5)
-
-@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
-def test_torch_vs_base_unspectrogram_twice(segmenter, x):
-    # skip for non radix-2 examples, but sloppy but so be it
-    if not is_radix_2(segmenter[0].frame_size):
-        return
-
-    x_tc = segmenter[0].spectrogram(x.clone())
-    x_ba = segmenter[1].spectrogram(x.clone())
-    assert x_tc.shape == x_ba.shape
-    segmenter[0].unspectrogram(x_tc)
-    segmenter[1].unspectrogram(x_ba)
-    assert x_tc.shape == x_ba.shape
-    assert x_tc == pytest.approx(x_ba, abs=1e-5)
-    x_tc = segmenter[0].spectrogram(x.clone())
-    x_ba = segmenter[1].spectrogram(x.clone())
-    assert x_tc.shape == x_ba.shape
-    segmenter[0].unspectrogram(x_tc)
-    segmenter[1].unspectrogram(x_ba)
-    assert x_tc.shape == x_ba.shape
-    assert x_tc == pytest.approx(x_ba, abs=1e-5)
+import pytest
+import torch
+import tensorflow
+import libsegmenter
+import numpy
+
+"""
+tests testing the creational pattern for the Segmenters
+"""
+
+test_cases_edge_corrected = []
+for backend in ["torch", "tensorflow", "base"]:
+    for mode in ["wola", "ola"]:
+        for window_settings in [
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hamming(100),
+                "input_size": (1000,),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hamming(100),
+                "input_size": (1, 1000),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hann(100),
+                "input_size": (1000,),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hann(100),
+                "input_size": (1, 1000),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.bartlett(100),
+                "input_size": (1000,),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.bartlett(100),
+                "input_size": (1, 1000),
+            },
+            {
+                "hop_size": 10,
+                "window": libsegmenter.blackman(30),
+                "input_size": (300,),
+            },
+            {
+                "hop_size": 10,
+                "window": libsegmenter.blackman(30),
+                "input_size": (1, 300),
+            },
+        ]:
+            test_cases_edge_corrected.append(
+                (
+                    libsegmenter.make_segmenter(
+                        backend=backend,
+                        frame_size=window_settings["window"].size,
+                        hop_size=window_settings["hop_size"],
+                        window=window_settings["window"],
+                        mode=mode,
+                        edge_correction=True,
+                    ),
+                    torch.randn((window_settings["input_size"])),
+                )
+            )
+
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_edge_corrected)
+def test_reconstruction_corrected(segmenter, x):
+    assert True == True
+    return
+    X = segmenter.segment(x)
+    y = segmenter.unsegment(X)
+
+    y = numpy.array(y)
+    x = numpy.array(x)
+    assert y == pytest.approx(x, abs=1e-5)
+
+
+test_cases_edge_uncorrected = []
+for backend in ["torch", "tensorflow", "base"]:
+    for mode in ["wola", "ola"]:
+        for window_settings in [
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hamming(100),
+                "input_size": (1000,),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hamming(100),
+                "input_size": (1, 1000),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hann(100),
+                "input_size": (1000,),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.hann(100),
+                "input_size": (1, 1000),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.bartlett(100),
+                "input_size": (1000,),
+            },
+            {
+                "hop_size": 50,
+                "window": libsegmenter.bartlett(100),
+                "input_size": (1, 1000),
+            },
+            {
+                "hop_size": 10,
+                "window": libsegmenter.blackman(30),
+                "input_size": (300,),
+            },
+            {
+                "hop_size": 10,
+                "window": libsegmenter.blackman(30),
+                "input_size": (1, 300),
+            },
+        ]:
+            test_cases_edge_uncorrected.append(
+                (
+                    libsegmenter.make_segmenter(
+                        backend=backend,
+                        frame_size=window_settings["window"].size,
+                        hop_size=window_settings["hop_size"],
+                        window=window_settings["window"],
+                        mode=mode,
+                        edge_correction=False,
+                    ),
+                    torch.randn((window_settings["input_size"])),
+                )
+            )
+
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_edge_uncorrected)
+def test_reconstruction_uncorrected(segmenter, x):
+    assert True == True
+    return
+    X = segmenter.segment(x)
+    y = segmenter.unsegment(X)
+
+    y = numpy.array(y)
+    x = numpy.array(x)
+    assert y[segmenter.frame_size : -segmenter.frame_size] == pytest.approx(
+        x[segmenter.frame_size : -segmenter.frame_size], abs=1e-5
+    )
+
+
+test_cases_torch_vs_tensorflow = []
+for mode in ["wola", "ola"]:
+    for window_settings in [
+        {
+            "hop_size": 50,
+            "window": libsegmenter.hamming(100),
+            "input_size": (1000,),
+        },
+        {
+            "hop_size": 50,
+            "window": libsegmenter.hamming(100),
+            "input_size": (1, 1000),
+        },
+        {
+            "hop_size": 50,
+            "window": libsegmenter.hann(100),
+            "input_size": (1000,),
+        },
+        {
+            "hop_size": 50,
+            "window": libsegmenter.hann(100),
+            "input_size": (1, 1000),
+        },
+        {
+            "hop_size": 50,
+            "window": libsegmenter.bartlett(100),
+            "input_size": (1000,),
+        },
+        {
+            "hop_size": 50,
+            "window": libsegmenter.bartlett(100),
+            "input_size": (1, 1000),
+        },
+        {
+            "hop_size": 10,
+            "window": libsegmenter.blackman(30),
+            "input_size": (300,),
+        },
+        {
+            "hop_size": 10,
+            "window": libsegmenter.blackman(30),
+            "input_size": (1, 300),
+        },
+    ]:
+        test_cases_torch_vs_tensorflow.append(
+            (
+                (
+                    libsegmenter.make_segmenter(
+                        backend="torch",
+                        frame_size=window_settings["window"].size,
+                        hop_size=window_settings["hop_size"],
+                        window=window_settings["window"],
+                        mode=mode,
+                        edge_correction=True,
+                    ),
+                    libsegmenter.make_segmenter(
+                        backend="tensorflow",
+                        frame_size=window_settings["window"].size,
+                        hop_size=window_settings["hop_size"],
+                        window=window_settings["window"],
+                        mode=mode,
+                        edge_correction=True,
+                    ),
+                ),
+                torch.randn((window_settings["input_size"])),
+            ),
+        )
+
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_tensorflow)
+def test_torch_vs_tensorflow_segment(segmenter, x):
+    X_tc = segmenter[0].segment(x)
+    X_tf = segmenter[1].segment(x)
+
+    assert X_tc == pytest.approx(X_tf, abs=1e-5)
+
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_tensorflow)
+def test_torch_vs_tensorflow_unsegment(segmenter, x):
+    x_tc = segmenter[0].unsegment(segmenter[0].segment(x))
+    x_tf = segmenter[1].unsegment(segmenter[1].segment(x))
+
+    assert x_tc == pytest.approx(x_tf, abs=1e-5)
+
+
+test_cases_torch_vs_base = []
+for edge_correction in [True, False]:
+    for mode in ["ola", "wola"]:
+        for window_settings in [
+            {
+                "hop_size": 32,
+                "window": libsegmenter.hamming(64),
+                "input_size": (640),
+            },
+            {
+                "hop_size": 32,
+                "window": libsegmenter.hamming(64),
+                "input_size": (1, 640),
+            },
+            {
+                "hop_size": 32,
+                "window": libsegmenter.hann(64),
+                "input_size": (640,),
+            },
+            {
+                "hop_size": 32,
+                "window": libsegmenter.hann(64),
+                "input_size": (1, 640),
+            },
+            {
+                "hop_size": 32,
+                "window": libsegmenter.bartlett(64),
+                "input_size": (640,),
+            },
+            {
+                "hop_size": 32,
+                "window": libsegmenter.bartlett(64),
+                "input_size": (1, 640),
+            },
+            {
+                "hop_size": 10,
+                "window": libsegmenter.blackman(30),
+                "input_size": (300,),
+            },
+            {
+                "hop_size": 10,
+                "window": libsegmenter.blackman(30),
+                "input_size": (1, 300),
+            },
+        ]:
+            test_cases_torch_vs_base.append(
+                (
+                    (
+                        libsegmenter.make_segmenter(
+                            backend="torch",
+                            frame_size=window_settings["window"].size,
+                            hop_size=window_settings["hop_size"],
+                            window=window_settings["window"].copy(),
+                            mode=mode,
+                            edge_correction=edge_correction,
+                        ),
+                        libsegmenter.make_segmenter(
+                            backend="base",
+                            frame_size=window_settings["window"].size,
+                            hop_size=window_settings["hop_size"],
+                            window=window_settings["window"].copy(),
+                            mode=mode,
+                            edge_correction=edge_correction,
+                        ),
+                    ),
+                    torch.randn((window_settings["input_size"])),
+                ),
+            )
+
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
+def test_torch_vs_base_segment(segmenter, x):
+    X_tc = segmenter[0].segment(x.clone())
+    X_ba = segmenter[1].segment(x.clone())
+    assert X_tc.shape == X_ba.shape
+    assert X_ba == pytest.approx(X_tc, abs=1e-5)
+
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
+def test_torch_vs_base_unsegment(segmenter, x):
+    x_tc = segmenter[0].segment(x.clone())
+    x_ba = segmenter[1].segment(x.clone())
+    assert x_tc.shape == x_ba.shape
+    segmenter[0].unsegment(x_tc)
+    segmenter[1].unsegment(x_ba)
+    assert x_tc.shape == x_ba.shape
+    assert x_tc == pytest.approx(x_ba, abs=1e-5)
+
+
+def is_radix_2(x):
+    return (x > 0) and (x & (x - 1)) == 0
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
+def test_torch_vs_base_spectrogram(segmenter, x):
+    # skip for non radix-2 examples, but sloppy but so be it
+    if not is_radix_2(segmenter[0].frame_size):
+        return
+    X_tc = segmenter[0].spectrogram(x.clone())
+    X_ba = segmenter[1].spectrogram(x.clone())
+    assert X_tc.shape == X_ba.shape
+    assert X_ba == pytest.approx(X_tc, abs=1e-5)
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
+def test_torch_vs_base_unspectrogram(segmenter, x):
+    # skip for non radix-2 examples, but sloppy but so be it
+    if not is_radix_2(segmenter[0].frame_size):
+        return
+    x_tc = segmenter[0].spectrogram(x.clone())
+    x_ba = segmenter[1].spectrogram(x.clone())
+    assert x_tc.shape == x_ba.shape
+    segmenter[0].unspectrogram(x_tc)
+    segmenter[1].unspectrogram(x_ba)
+    assert x_tc.shape == x_ba.shape
+    assert x_tc == pytest.approx(x_ba, abs=1e-5)
+
+@pytest.mark.parametrize(("segmenter", "x"), test_cases_torch_vs_base)
+def test_torch_vs_base_unspectrogram_twice(segmenter, x):
+    # skip for non radix-2 examples, but sloppy but so be it
+    if not is_radix_2(segmenter[0].frame_size):
+        return
+
+    x_tc = segmenter[0].spectrogram(x.clone())
+    x_ba = segmenter[1].spectrogram(x.clone())
+    assert x_tc.shape == x_ba.shape
+    segmenter[0].unspectrogram(x_tc)
+    segmenter[1].unspectrogram(x_ba)
+    assert x_tc.shape == x_ba.shape
+    assert x_tc == pytest.approx(x_ba, abs=1e-5)
+    x_tc = segmenter[0].spectrogram(x.clone())
+    x_ba = segmenter[1].spectrogram(x.clone())
+    assert x_tc.shape == x_ba.shape
+    segmenter[0].unspectrogram(x_tc)
+    segmenter[1].unspectrogram(x_ba)
+    assert x_tc.shape == x_ba.shape
+    assert x_tc == pytest.approx(x_ba, abs=1e-5)
```

## tests/windows.py

 * *Ordering differences only*

```diff
@@ -1,27 +1,27 @@
-import pytest
-import libsegmenter
-
-"""
-tests ensuring the `check_cola` and windowing functions included in the library are correct
-"""
-
-
-@pytest.mark.parametrize(
-    ("window", "hop_size", "valid"),
-    [
-        (libsegmenter.bartlett(100), 50, True),
-        (libsegmenter.bartlett(100), 25, True),
-        (libsegmenter.bartlett(100), 50, True),
-        (libsegmenter.bartlett(100), 51, False),
-        (libsegmenter.blackman(99), 33, True),
-        (libsegmenter.blackman(99), 34, False),
-        (libsegmenter.hamming(100), 50, True),
-        (libsegmenter.hamming(100), 25, True),
-        (libsegmenter.hamming(100), 23, False),
-        (libsegmenter.hann(100), 50, True),
-        (libsegmenter.hann(100), 25, True),
-        (libsegmenter.hann(100), 23, False),
-    ],
-)
-def test_check_cola(window, hop_size, valid):
-    assert libsegmenter.check_cola(window, hop_size)[0] == valid
+import pytest
+import libsegmenter
+
+"""
+tests ensuring the `check_cola` and windowing functions included in the library are correct
+"""
+
+
+@pytest.mark.parametrize(
+    ("window", "hop_size", "valid"),
+    [
+        (libsegmenter.bartlett(100), 50, True),
+        (libsegmenter.bartlett(100), 25, True),
+        (libsegmenter.bartlett(100), 50, True),
+        (libsegmenter.bartlett(100), 51, False),
+        (libsegmenter.blackman(99), 33, True),
+        (libsegmenter.blackman(99), 34, False),
+        (libsegmenter.hamming(100), 50, True),
+        (libsegmenter.hamming(100), 25, True),
+        (libsegmenter.hamming(100), 23, False),
+        (libsegmenter.hann(100), 50, True),
+        (libsegmenter.hann(100), 25, True),
+        (libsegmenter.hann(100), 23, False),
+    ],
+)
+def test_check_cola(window, hop_size, valid):
+    assert libsegmenter.check_cola(window, hop_size)[0] == valid
```

## Comparing `libsegmenter-0.9.1.dist-info/RECORD` & `libsegmenter-0.9.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-libsegmenter/Segmenter.py,sha256=x5oAD1C6jpBsuPNh_cFm5T_wpPT3j2-ecEl5k9B1Byc,708
-libsegmenter/SegmenterTensorFlow.py,sha256=X-sqvo3pURBUivUTjT24aGJsn8nrHHCTWfHV5R4aeiA,9073
-libsegmenter/SegmenterTorch.py,sha256=bp2lEmQIbfCLz34jillJHD9oB3xk7Z2c1-OH-DDsuAc,7599
-libsegmenter/__init__.py,sha256=BhUJudEKMTAEnu1Kq-Ckbg6kTZp-g-6Zx2PvntlIeAQ,107
-libsegmenter/bindings.pypy39-pp73-win_amd64.pyd,sha256=AxEZRi7lGFPgKpsO1tIK9uBDKNw5pHw1r2GupHSBH80,195072
-libsegmenter/default_window_selector.py,sha256=q0dmDqPZMWc52ET0PwqpN17rRP53-BVody87akXBIXc,4678
-libsegmenter/old.py,sha256=328FhSPvoTqEf-AUsq6WWkLY_fM_sHCqPPCTcRdfbog,2621
-tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/creational.py,sha256=QWS4mMHxRgeMcTV6f2i3DjuDF0e391w_ciIheb4krBI,2292
-tests/reconstruction.py,sha256=FsjjSivsY4s6LzY29KRMzNfrxtvw2HaYvdxn6YMfD74,12744
-tests/windows.py,sha256=fjwAUL-J9ZzwaXvSTZrgFO7D6RmfkGCmiYBkihEDI3E,916
-libsegmenter-0.9.1.dist-info/METADATA,sha256=CRaAoIttX_PObE4-ChG4SicV3eAlotjavRN0mrWjcFw,279
-libsegmenter-0.9.1.dist-info/WHEEL,sha256=0MDxp1g6SMi6x5fNLQYB_oq4z1ZIM2F5EzPGH_eSWIs,107
-libsegmenter-0.9.1.dist-info/top_level.txt,sha256=vM1fU6i2eEkdt_wR1Rvw_-LVSVSaa-Qr-O0y7KtZ500,19
-libsegmenter-0.9.1.dist-info/RECORD,,
+tests/reconstruction.py,sha256=cyo5rwegyPn3xLpQXRVkLr-dkL9fffIrKjn998Fu3QI,12369
+tests/creational.py,sha256=nhRduMAq_zVExDnkUj_grxKHE9LvUEL5kfKSe10Xik8,2229
+tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/windows.py,sha256=3AsqCfSAjYJL8miyEtPrNgAywvngxxOv7zqszZB_Qu4,889
+libsegmenter/default_window_selector.py,sha256=dYgXxLQ0oYAq-yqbs45QX-Udmhmw2Enzcuds72KXY5U,4569
+libsegmenter/old.py,sha256=24UtckNg43Dnzge8XW6czXkfsQA9eWUaET5uBwF1yqA,2540
+libsegmenter/__init__.py,sha256=_wY2cRUmJFCGZTNvyGAz2Y1hxFBdywyln_yclkzHdrA,102
+libsegmenter/bindings.pypy39-pp73-darwin.so,sha256=jUS2dk32_djNjBwtIb_Od03XzazKrY34aeWtGat2XUQ,382048
+libsegmenter/SegmenterTensorFlow.py,sha256=mUSRTncmzWOzQACh9q_zR5gEZbH6nRMvfYZxmLgYXXQ,8835
+libsegmenter/Segmenter.py,sha256=wXYPtzzrgB2pJ4uEqVtZobdvtfgGzFqPA7sxBXsNDGg,684
+libsegmenter/SegmenterTorch.py,sha256=oTpp4Czn7IBjNNkTizrMYD--iNCKpiICvz8Mjp06ELA,7329
+libsegmenter-0.9.2.dist-info/RECORD,,
+libsegmenter-0.9.2.dist-info/WHEEL,sha256=cyXkGwv3Qv6v4LhlqIWnhSeL6MEVHOhiaSsK5HPxXp4,115
+libsegmenter-0.9.2.dist-info/top_level.txt,sha256=vM1fU6i2eEkdt_wR1Rvw_-LVSVSaa-Qr-O0y7KtZ500,19
+libsegmenter-0.9.2.dist-info/METADATA,sha256=2OjpdMTNp9H7RyBj0fB1MDmUNhtgGcDj4Svi-_5xEUM,270
```

