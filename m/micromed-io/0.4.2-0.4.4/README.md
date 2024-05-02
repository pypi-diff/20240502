# Comparing `tmp/micromed_io-0.4.2.tar.gz` & `tmp/micromed_io-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micromed_io-0.4.2.tar", max compression
+gzip compressed data, was "micromed_io-0.4.4.tar", max compression
```

## Comparing `micromed_io-0.4.2.tar` & `micromed_io-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1534 2024-02-08 14:48:10.197272 micromed_io-0.4.2/LICENSE
--rw-r--r--   0        0        0       50 2024-02-09 15:22:54.832636 micromed_io-0.4.2/micromed_io/__init__.py
--rw-r--r--   0        0        0     6333 2024-02-08 14:48:13.835447 micromed_io-0.4.2/micromed_io/buffer.py
--rw-r--r--   0        0        0     3846 2024-02-08 14:48:13.835447 micromed_io-0.4.2/micromed_io/header.py
--rw-r--r--   0        0        0    24452 2024-02-09 15:21:42.195872 micromed_io-0.4.2/micromed_io/in_out.py
--rw-r--r--   0        0        0     8164 2024-02-08 14:48:13.836441 micromed_io-0.4.2/micromed_io/scripts/emulate_online_trc.py
--rw-r--r--   0        0        0     1453 2024-02-08 14:48:13.836441 micromed_io-0.4.2/micromed_io/scripts/rename_trc.py
--rw-r--r--   0        0        0    12576 2024-02-08 14:48:13.836441 micromed_io-0.4.2/micromed_io/scripts/tcp_to_lsl.py
--rw-r--r--   0        0        0     3650 2024-02-08 14:48:13.836441 micromed_io-0.4.2/micromed_io/tcp.py
--rw-r--r--   0        0        0     4070 2024-02-08 14:48:13.836441 micromed_io-0.4.2/micromed_io/to_mne.py
--rw-r--r--   0        0        0     3267 2024-02-08 14:48:13.837441 micromed_io-0.4.2/micromed_io/trc.py
--rw-r--r--   0        0        0      864 2024-02-09 15:23:06.366665 micromed_io-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5298 2024-02-08 14:48:10.197272 micromed_io-0.4.2/README.rst
--rw-r--r--   0        0        0     5755 1970-01-01 00:00:00.000000 micromed_io-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1534 2024-02-08 14:48:10.197272 micromed_io-0.4.4/LICENSE
+-rw-r--r--   0        0        0       52 2024-05-02 07:42:39.386572 micromed_io-0.4.4/micromed_io/__init__.py
+-rw-r--r--   0        0        0     3846 2024-02-08 14:48:13.835447 micromed_io-0.4.4/micromed_io/header.py
+-rw-r--r--   0        0        0    24404 2024-05-02 07:31:49.684032 micromed_io-0.4.4/micromed_io/in_out.py
+-rw-r--r--   0        0        0     8164 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/scripts/emulate_online_trc.py
+-rw-r--r--   0        0        0     1453 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/scripts/rename_trc.py
+-rw-r--r--   0        0        0    12576 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/scripts/tcp_to_lsl.py
+-rw-r--r--   0        0        0     3650 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/tcp.py
+-rw-r--r--   0        0        0     4070 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/to_mne.py
+-rw-r--r--   0        0        0     3267 2024-02-08 14:48:13.837441 micromed_io-0.4.4/micromed_io/trc.py
+-rw-r--r--   0        0        0      864 2024-05-02 07:42:33.597836 micromed_io-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     4911 2024-04-10 10:45:33.365380 micromed_io-0.4.4/README.rst
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 micromed_io-0.4.4/PKG-INFO
```

### Comparing `micromed_io-0.4.2/LICENSE` & `micromed_io-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/micromed_io/header.py` & `micromed_io-0.4.4/micromed_io/header.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/micromed_io/in_out.py` & `micromed_io-0.4.4/micromed_io/in_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Micromed IO module"""
+
 #
 # the header parser has been updated to read almost all data thanks to wonambi library:
 # https://wonambi-python.github.io/api/wonambi.ioeeg.micromed.html
 #
 
 import logging
 from datetime import date, datetime
@@ -61,15 +62,14 @@
         self,
         picks: List[str] = None,
     ):
         self.micromed_header = MicromedHeader()
         self.current_data_eeg = None
         self.picks = picks
         self.picks_id = None
-        self.epoch_buffer = None
         self.mkr_index = None  # index of MKR+-MKR- channel in micromed_header.ch_names
         self.current_channels = None
         self.notes = {}
         self.note_start_offset = -1
         self.sfreq = None
 
     def decode_data_header_packet(self, packet: bytearray) -> None:
@@ -91,15 +91,15 @@
         self.micromed_header.nb_of_bytes = self._header["n_bytes"]
         self.micromed_header.header_type = self._header["header_type"]
         self.micromed_header.stored_channels = self._header["order"]
         self.micromed_header.ch_names = [
             f"{d['chan_name']}-{d['ground']}" for d in self._header["chans"]
         ]
 
-        # construct the indexes of channels to pick in epoch buffer
+        # construct the indexes of channels to pick
         if self.picks is None:
             self.picks_id = np.arange(len(self.micromed_header.stored_channels))
         else:
             # Check that all channels are pickable
             for ch in self.picks:
                 if ch not in self.micromed_header.ch_names:
                     raise ValueError(
@@ -228,15 +228,15 @@
                     logic_ground = self.micromed_header.elec_refs[i].logic_ground
 
                     if use_volt is True:
                         unit = self.micromed_header.elec_refs[i].units
                         ratio = 0
                         if unit == "nV":
                             ratio = 1e-9
-                        elif unit == "µV":
+                        elif unit == "μV":
                             ratio = 1e-6
                         elif unit == "mV":
                             ratio = 1e-3
                         elif unit == "V":
                             ratio = 1
                         else:
                             raise ValueError(
```

### Comparing `micromed_io-0.4.2/micromed_io/scripts/emulate_online_trc.py` & `micromed_io-0.4.4/micromed_io/scripts/emulate_online_trc.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/micromed_io/scripts/rename_trc.py` & `micromed_io-0.4.4/micromed_io/scripts/rename_trc.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/micromed_io/scripts/tcp_to_lsl.py` & `micromed_io-0.4.4/micromed_io/scripts/tcp_to_lsl.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/micromed_io/tcp.py` & `micromed_io-0.4.4/micromed_io/tcp.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/micromed_io/to_mne.py` & `micromed_io-0.4.4/micromed_io/to_mne.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/micromed_io/trc.py` & `micromed_io-0.4.4/micromed_io/trc.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.2/pyproject.toml` & `micromed_io-0.4.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micromed-io"
-version = "0.4.2"
+version = "0.4.4"
 description = "A library to read, emulate, and forward Micromed data in standard formats"
 authors = ["Etienne de MONTALIVET <etienne.demontalivet@protonmail.com>"]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 mne = "^1.0.0"
```

### Comparing `micromed_io-0.4.2/README.rst` & `micromed_io-0.4.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -131,39 +131,14 @@
 
 ..
 
    **Note**: Micromed TCP behaves as a client. If you want to try the
    emulate/read TCP script, launch the reader first that acts as server,
    then the emulator.
 
-Read online Micromed TCP in a sliding window buffer
----------------------------------------------------
-
-If you plan to use the Micromed data as input of a decoder, you probably
-want epochs of format ``(n_channels, n_samples)``. Then the
-``MicromedBuffer`` class is for you. The script ``tcp_to_epoch.py``
-shows you how to use it (see the ``PROCESS HERE`` comment). It uses a
-**buffer** that mimics the **sliding window** and triggers each time it
-is filled.
-
-.. code:: python
-
-   from micromed_io.buffer import MicromedBuffer
-   micromed_buffer = MicromedBuffer(epoch_duration=5, epoch_overlap=2.5)
-
-To run the example, you can download and run the ``tcp_to_epoch.py`` script in ``extern/`` 
-folder:
-
-.. code:: bash
-
-   $ python tcp_to_epoch.py --epoch-size=5 --overlap=2.5
-
-.. note::
-   
-   Try it with **emulated data** from a TRC file (cf `emulate TRC`_)
 
 Rename TRC files with recording datetime
 ----------------------------------------
 
 .. code:: bash
 
    $ mmio_rename_trc --dirpath=./ --format=%Y%m%d-%H%M%S
@@ -186,7 +161,24 @@
 
    $ conda env create -f environment.yml
    $ conda activate mmio
    $ poetry install
 
 
 Please feel free to reach me if you want to contribute.
+
+Sponsor
+-------
+
+This work has been supported by the Wyss Center.
+
+.. image:: https://raw.githubusercontent.com/etiennedemontalivet/micromed-io/master/docs/source/data/wyss-center-full.png
+  :alt: Wyss Center logo
+  :align: center
+  :class: only-light
+  :width: 50%
+
+.. image:: https://raw.githubusercontent.com/etiennedemontalivet/micromed-io/master/docs/source/data/wyss-center-full-inverse.png
+  :alt: Wyss Center inverse logo
+  :align: center
+  :class: only-dark
+  :width: 50%
```

### Comparing `micromed_io-0.4.2/PKG-INFO` & `micromed_io-0.4.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micromed-io
-Version: 0.4.2
+Version: 0.4.4
 Summary: A library to read, emulate, and forward Micromed data in standard formats
 Author: Etienne de MONTALIVET
 Author-email: etienne.demontalivet@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -148,39 +148,14 @@
 
 ..
 
    **Note**: Micromed TCP behaves as a client. If you want to try the
    emulate/read TCP script, launch the reader first that acts as server,
    then the emulator.
 
-Read online Micromed TCP in a sliding window buffer
----------------------------------------------------
-
-If you plan to use the Micromed data as input of a decoder, you probably
-want epochs of format ``(n_channels, n_samples)``. Then the
-``MicromedBuffer`` class is for you. The script ``tcp_to_epoch.py``
-shows you how to use it (see the ``PROCESS HERE`` comment). It uses a
-**buffer** that mimics the **sliding window** and triggers each time it
-is filled.
-
-.. code:: python
-
-   from micromed_io.buffer import MicromedBuffer
-   micromed_buffer = MicromedBuffer(epoch_duration=5, epoch_overlap=2.5)
-
-To run the example, you can download and run the ``tcp_to_epoch.py`` script in ``extern/`` 
-folder:
-
-.. code:: bash
-
-   $ python tcp_to_epoch.py --epoch-size=5 --overlap=2.5
-
-.. note::
-   
-   Try it with **emulated data** from a TRC file (cf `emulate TRC`_)
 
 Rename TRC files with recording datetime
 ----------------------------------------
 
 .. code:: bash
 
    $ mmio_rename_trc --dirpath=./ --format=%Y%m%d-%H%M%S
@@ -204,7 +179,23 @@
    $ conda env create -f environment.yml
    $ conda activate mmio
    $ poetry install
 
 
 Please feel free to reach me if you want to contribute.
 
+Sponsor
+-------
+
+This work has been supported by the Wyss Center.
+
+.. image:: https://raw.githubusercontent.com/etiennedemontalivet/micromed-io/master/docs/source/data/wyss-center-full.png
+  :alt: Wyss Center logo
+  :align: center
+  :class: only-light
+  :width: 50%
+
+.. image:: https://raw.githubusercontent.com/etiennedemontalivet/micromed-io/master/docs/source/data/wyss-center-full-inverse.png
+  :alt: Wyss Center inverse logo
+  :align: center
+  :class: only-dark
+  :width: 50%
```

