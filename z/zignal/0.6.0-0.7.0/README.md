# Comparing `tmp/zignal-0.6.0.tar.gz` & `tmp/zignal-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zignal-0.6.0.tar", last modified: Sun Feb 23 18:47:44 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `zignal-0.6.0.tar` & `zignal-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2020-02-23 18:47:44.000000 zignal-0.6.0/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       38 2020-02-23 18:47:44.000000 zignal-0.6.0/setup.cfg
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     5120 2019-09-23 21:51:38.000000 zignal-0.6.0/setup.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     6915 2020-02-23 18:47:44.000000 zignal-0.6.0/PKG-INFO
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       63 2019-08-06 22:26:46.000000 zignal-0.6.0/MANIFEST.in
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal.egg-info/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     6915 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal.egg-info/PKG-INFO
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      504 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal.egg-info/SOURCES.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       69 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal.egg-info/entry_points.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)        7 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal.egg-info/top_level.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)       69 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal.egg-info/requires.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)        1 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal.egg-info/dependency_links.txt
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     1082 2017-12-05 23:44:33.000000 zignal-0.6.0/LICENSE.txt
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal/
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal/measure/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      190 2019-08-06 22:26:46.000000 zignal-0.6.0/zignal/measure/__init__.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)    32425 2017-12-05 23:44:33.000000 zignal-0.6.0/zignal/measure/mlstaps.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)    19183 2020-02-23 18:44:20.000000 zignal-0.6.0/zignal/measure/mls.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)    42529 2020-02-23 18:44:20.000000 zignal-0.6.0/zignal/audio.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)    22469 2019-08-06 22:26:46.000000 zignal-0.6.0/zignal/sndcard.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      432 2020-02-23 18:44:20.000000 zignal-0.6.0/zignal/__init__.py
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal/music/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     2869 2019-08-06 22:26:46.000000 zignal-0.6.0/zignal/music/spn.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      225 2019-08-06 22:26:46.000000 zignal-0.6.0/zignal/music/__init__.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     2907 2019-08-06 22:26:46.000000 zignal-0.6.0/zignal/music/scales.py
-drwxrwxr-x   0 ronny     (1000) ronny     (1000)        0 2020-02-23 18:47:44.000000 zignal-0.6.0/zignal/filters/
--rw-rw-r--   0 ronny     (1000) ronny     (1000)    11184 2019-08-06 22:26:46.000000 zignal-0.6.0/zignal/filters/linearfilter.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)      247 2019-08-06 22:26:46.000000 zignal-0.6.0/zignal/filters/__init__.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)    13783 2020-02-23 18:44:20.000000 zignal-0.6.0/zignal/filters/biquads.py
--rw-rw-r--   0 ronny     (1000) ronny     (1000)     3269 2019-08-06 22:26:46.000000 zignal-0.6.0/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 zignal-0.7.0/Makefile
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 zignal-0.7.0/setup.cfg
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_FFT.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_append.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_chunks.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_comment.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_decimate.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_filter_biquad.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_filter_cic.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_fourier.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_mls.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_noise.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_peak_rms_crestfactor.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_sine.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 zignal-0.7.0/examples/ex_sndcard.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/__init__.py
+-rw-r--r--   0        0        0    45911 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/audio.py
+-rw-r--r--   0        0        0    22031 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/sndcard.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/filters/__init__.py
+-rw-r--r--   0        0        0    13964 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/filters/biquads.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/filters/cic.py
+-rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/filters/linearfilter.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/measure/__init__.py
+-rw-r--r--   0        0        0    19450 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/measure/mls.py
+-rw-r--r--   0        0        0    27091 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/measure/mlstaps.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/music/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/music/scales.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/music/spn.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_audio_constructor.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_audio_datatype_conversion.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_audio_peak.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_db_conversions.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_linearfilter.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_music_scales.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_music_spn.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 zignal-0.7.0/zignal/tests/test_sine.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 zignal-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 zignal-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 zignal-0.7.0/README.md
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 zignal-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 zignal-0.7.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zignal-0.6.0/PKG-INFO` & `zignal-0.7.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,145 +1,152 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: zignal
-Version: 0.6.0
+Version: 0.7.0
 Summary: Audio signal processing library
-Home-page: https://github.com/ronnyandersson/zignal
-Author: Ronny Andersson
-Author-email: ronny@andersson.tk
-License: The MIT License (MIT)
-
-Copyright (c) 2013 Ronny Andersson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-Download-URL: https://pypi.python.org/pypi/zignal
-Description: # zignal
-        
-        This is a python audio signal processing library.
-        
-        Python 2 is no longer supported, the last version to support python 2 is 0.2.0
-        
-        ## Example usage
-        
-            >>> import zignal
-            >>>
-            >>> x = zignal.Sinetone(fs=44100, f0=997, duration=0.1, gaindb=-20)
-            >>> print(x)
-            =======================================
-            classname        : Sinetone
-            sample rate      : 44100.0 [Hz]
-            channels         : 1
-            duration         : 0.100 [s]
-            datatype         : float64
-            samples per ch   : 4410
-            data size        : 0.034 [Mb]
-            has comment      : no
-            peak             : [ 0.1]
-            RMS              : [ 0.0707]
-            crestfactor      : [ 1.4147]
-            -----------------:---------------------
-            frequency        : 997.0 [Hz]
-            phase            : 0.0 [deg]
-            -----------------:---------------------
-        
-            >>> x.fade_out(millisec=10)
-            >>> x.convert_to_float(targetbits=32)
-            >>> x.write_wav_file("sinetone.wav")
-            >>> x.plot()
-            >>> x.plot_fft()
-            >>>
-            >>> f = zignal.filters.biquads.RBJ(filtertype="peak", gaindb=-6, f0=997, Q=0.707, fs=96000)
-            >>> print(f)
-            =======================================
-            classname        : RBJ
-            sample rate      : 96000.0 [Hz]
-            feedforward  (B) : [ 0.96949457 -1.87369167  0.90819329]
-            feedback     (A) : [ 1.         -1.87369167  0.87768787]
-            number of zeros  : 2
-            number of poles  : 2
-            minimum phase?   : Yes
-            -----------------:---------------------
-            stable?          : Yes
-            type             : peak
-            gain             : -6.00 [dB]
-            f0               : 997.0 [Hz]
-            Q                : 0.7070
-        
-            >>> f.plot_mag_phase()
-            >>> f.plot_pole_zero()
-            >>>
-        
-        See the examples folder for more examples.
-        
-        ## Requirements
-        
-        This library relies on numpy, scipy, matplotlib and optionally pyaudio (and nose for unit testing). It is recommended to create a virtual environment and let pip install the dependencies automatically.
-        
-            python3 -m venv <name-of-virtualenv>
-            . <name-of-virtualenv>/bin/activate
-            pip install zignal
-        
-        Optionally, to be able to use a soundcard, first install the python development headers and the portaudio development files. On debian/ubuntu,
-        
-            sudo apt install python3-dev portaudio19-dev
-        
-        then run
-        
-            pip install zignal[sndcard]
-        
-        which will automatically build the portaudio library and then pyaudio.
-        
-        ## Local development
-        
-        Create a python3 virtualenv and install from the requirements.txt file to make the zignal library editable. Note that the python development headers (python3-dev) and portaudio19-dev must be installed first.
-        
-            python3 -m venv zignaldev
-            . zignaldev/bin/activate
-            pip install -r requirements.txt
-        
-        ## Design goals
-        
-        1.  Readability over efficiency. This is a python library for development and understanding of audio signal processing.
-        2.  The initial goal is to write the functionality in pure python, with the use of numpy, scipy and matplotlib. See rule 1. If efficiency becomes an issue a c/c++ library might be implemented but the pure python code must remain the default choice.
-        3.  Design for non real-time processing. Functionality to do real-time processing can be added if it does not break rule 1.
-        4.  Self documentation. The code should aim to be well documented, in the source code itself.
-        
-Keywords: audio,sound,card,soundcard,pyaudio,portaudio,playback,recording,digital,signal,processing,DSP,signalprocessing,fourier,FFT,filter,filtering,parametric,eq,equaliser,equalizer,biquad,cookbook,sine,generator,mls,mlssa,maximum,length,sequence,maximumlengthsequence,pseudo,random,pseudorandom,measure,measurement,impulse,response,impulseresponse,frequency,frequencyresponse,magnitude,magnituderesponse,piano,midi,tuning,scale,pitch,notation,equal,temperament,12TET,spn
-Platform: any
+Project-URL: Homepage, https://github.com/ronnyandersson/zignal
+Project-URL: Issues, https://github.com/ronnyandersson/zignal/issues
+Project-URL: Download, https://pypi.python.org/pypi/zignal
+Author-email: Ronny Andersson <ronny@andersson.tk>
+License: MIT License
+License-File: LICENSE.txt
+Keywords: 12TET,CIC,DSP,FFT,FIR,IIR,audio,biquad,card,cascaded,comb,cookbook,decimation,decimator,digital,eq,equal,equaliser,equalizer,filter,filtering,finite,fourier,frequency,frequencyresponse,generator,impulse,impulseresponse,infinite,integrator,length,magnitude,magnituderesponse,maximum,maximumlengthsequence,measure,measurement,midi,mls,mlssa,notation,parametric,piano,pitch,playback,portaudio,processing,pseudo,pseudorandom,pyaudio,random,recording,response,scale,sequence,signal,signalprocessing,sine,sound,soundcard,spn,temperament,tuning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
 Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Multimedia :: Sound/Audio :: Mixers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Provides-Extra: dev
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: pyaudio; extra == 'dev'
 Provides-Extra: sndcard
-Provides-Extra: testing
+Requires-Dist: pyaudio; extra == 'sndcard'
+Description-Content-Type: text/markdown
+
+# zignal
+
+This is a python audio signal processing library.
+
+## Example usage
+
+    >>> import zignal
+    >>>
+    >>> x = zignal.Sinetone(fs=44100, f0=997, duration=0.1, gaindb=-20)
+    >>> print(x)
+    =======================================
+    classname        : Sinetone
+    sample rate      : 44100.0 [Hz]
+    channels         : 1
+    duration         : 0.100 [s]
+    datatype         : float64
+    samples per ch   : 4410
+    data size        : 0.034 [Mb]
+    has comment      : no
+    peak             : [ 0.1]
+    RMS              : [ 0.0707]
+    crestfactor      : [ 1.4147]
+    -----------------:---------------------
+    frequency        : 997.0 [Hz]
+    phase            : 0.0 [deg]
+    -----------------:---------------------
+
+    >>> x.fade_out(millisec=10)
+    >>> x.convert_to_float(targetbits=32)
+    >>> x.write_wav_file("sinetone.wav")
+    >>> x.plot()
+    >>> x.plot_fft()
+    >>>
+    >>> f = zignal.filters.biquads.RBJ(filtertype="peak", gaindb=-6, f0=997, Q=0.707, fs=96000)
+    >>> print(f)
+    =======================================
+    classname        : RBJ
+    sample rate      : 96000.0 [Hz]
+    feedforward  (B) : [ 0.96949457 -1.87369167  0.90819329]
+    feedback     (A) : [ 1.         -1.87369167  0.87768787]
+    number of zeros  : 2
+    number of poles  : 2
+    minimum phase?   : Yes
+    -----------------:---------------------
+    stable?          : Yes
+    type             : peak
+    gain             : -6.00 [dB]
+    f0               : 997.0 [Hz]
+    Q                : 0.7070
+
+    >>> f.plot_mag_phase()
+    >>> f.plot_pole_zero()
+    >>>
+
+See the examples folder for more examples.
+
+## Requirements
+
+This library relies on numpy, scipy, matplotlib and optionally pyaudio. It is
+recommended to create a virtual environment and let pip install the
+dependencies automatically.
+
+    python3 -m venv <name-of-virtualenv>
+    . <name-of-virtualenv>/bin/activate
+    pip install zignal
+
+Optionally, to be able to use a soundcard, first install the python development
+headers and the portaudio development files. On debian/ubuntu,
+
+    sudo apt install python3-dev portaudio19-dev
+
+then run
+
+    pip install zignal[sndcard]
+
+which will automatically build the portaudio library and then pyaudio.
+
+## Local development
+
+Create a python3 virtualenv and install from the local source code to make the
+zignal library editable. Note that the python development headers (python3-dev)
+and portaudio19-dev must be installed first.
+
+    python3 -m venv venv_dev
+    . venv_dev/bin/activate
+    pip install --editable .[dev]
+
+By running `make` it is now possible to run isort, flake8 and also all the unit
+tests. They can also be executed directly from the command line, see the
+Makefile for the full commands to run.
+
+## Build a release
+
+    python3 -m venv venv_build
+    . ./venv_build/bin/activate
+    pip install --upgrade pip build
+    python3 -m build
+
+## Design goals
+
+1.  Readability over efficiency. This is a python library for development and
+    understanding of audio signal processing.
+2.  The initial goal is to write the functionality in pure python, with the use
+    of numpy, scipy and matplotlib. See rule 1. If efficiency becomes an issue
+    a c/c++ library might be implemented but the pure python code must remain
+    the default choice.
+3.  Design for non real-time processing. Functionality to do real-time
+    processing can be added if it does not break rule 1.
+4.  Self documentation. The code should aim to be well documented, in the
+    source code itself.
```

### Comparing `zignal-0.6.0/LICENSE.txt` & `zignal-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zignal-0.6.0/zignal/measure/mlstaps.py` & `zignal-0.7.0/zignal/measure/mlstaps.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,1093 +2,1095 @@
 Created on 22 Mar 2014
 
 @author: Ronny Andersson (ronny@andersson.tk)
 @copyright: (c) 2014 Ronny Andersson
 @license: MIT
 """
 
-__all__ = ['TAPS',]
+__all__ = [
+    'TAPS',
+    ]
 
 # All taps are found on this website:
 # www.newwaveinstruments.com/resources/articles/m_sequence_linear_feedback_shift_register_lfsr.htm
 #
 # Taps are always 1-indexed, i.e. they start at 1 (one). So index 1 means
 # first (rightmost) tap.
 TAPS = {
-        3 : (
-             (3, 2),
-             ),
-        4 : (
-             (4, 3),
-             ),
-        5 : (
-             (5, 3),
-             (5, 4, 3, 2),
-             (5, 4, 3, 1),
-             ),
-        6 : (
-             (6, 5),
-             (6, 5, 4, 1),
-             (6, 5, 3, 2),
-             ),
-        7 : (
-             (7, 6),
-             (7, 4),
-             (7, 6, 5, 4),
-             (7, 6, 5, 2),
-             (7, 6, 4, 2),
-             (7, 6, 4, 1),
-             (7, 5, 4, 3),
-             (7, 6, 5, 4, 3, 2),
-             (7, 6, 5, 4, 2, 1),
-             ),
-        8 : (
-             (8, 7, 6, 1),
-             (8, 7, 5, 3),
-             (8, 7, 3, 2),
-             (8, 6, 5, 4),
-             (8, 6, 5, 3),
-             (8, 6, 5, 2),
-             (8, 7, 6, 5, 4, 2),
-             (8, 7, 6, 5, 2, 1),
-             ),
-        9 : (
-             (9, 5),
-             (9, 8, 7, 2),
-             (9, 8, 6, 5),
-             (9, 8, 5, 4),
-             (9, 8, 5, 1),
-             (9, 8, 4, 2),
-             (9, 7, 6, 4),
-             (9, 7, 5, 2),
-             (9, 6, 5, 3),
-             (9, 8, 7, 6, 5, 3),
-             (9, 8, 7, 6, 5, 1),
-             (9, 8, 7, 6, 4, 3),
-             (9, 8, 7, 6, 4, 2),
-             (9, 8, 7, 6, 3, 2),
-             (9, 8, 7, 6, 3, 1),
-             (9, 8, 7, 6, 2, 1),
-             (9, 8, 7, 5, 4, 3),
-             (9, 8, 7, 5, 4, 2),
-             (9, 8, 6, 5, 4, 1),
-             (9, 8, 6, 5, 3, 2),
-             (9, 8, 6, 5, 3, 1),
-             (9, 7, 6, 5, 4, 3),
-             (9, 7, 6, 5, 4, 2),
-             (9, 8, 7, 6, 5, 4, 3, 1),
-             ),
-        10: (
-             (10, 7),
-             (10, 9, 8, 5),
-             (10, 9, 7, 6),
-             (10, 9, 7, 3),
-             (10, 9, 6, 1),
-             (10, 9, 5, 2),
-             (10, 9, 4, 2),
-             (10, 8, 7, 5),
-             (10, 8, 7, 2),
-             (10, 8, 5, 4),
-             (10, 8, 4, 3),
-             (10, 9, 8, 7, 5, 4),
-             (10, 9, 8, 7, 4, 1),
-             (10, 9, 8, 7, 3, 2),
-             (10, 9, 8, 6, 5, 1),
-             (10, 9, 8, 6, 4, 3),
-             (10, 9, 8, 6, 4, 2),
-             (10, 9, 8, 6, 3, 2),
-             (10, 9, 8, 6, 2, 1),
-             (10, 9, 8, 5, 4, 3),
-             (10, 9, 8, 4, 3, 2),
-             (10, 9, 7, 6, 4, 1),
-             (10, 9, 7, 5, 4, 2),
-             (10, 9, 6, 5, 4, 3),
-             (10, 8, 7, 6, 5, 2),
-             (10, 9, 8, 7, 6, 5, 4, 3),
-             (10, 9, 8, 7, 6, 5, 4, 1),
-             (10, 9, 8, 7, 6, 4, 3, 1),
-             (10, 9, 8, 6, 5, 4, 3, 2),
-             (10, 9, 7, 6, 5, 4, 3, 2),
-             ),
-        11: (
-             (11, 9),
-             (11, 10, 9, 7),
-             (11, 10, 9, 5),
-             (11, 10, 9, 2),
-             (11, 10, 8, 6),
-             (11, 10, 8, 1),
-             (11, 10, 7, 3),
-             (11, 10, 7, 2),
-             (11, 10, 6, 5),
-             (11, 10, 4, 3),
-             (11, 10, 3, 2),
-             (11, 9, 8, 6),
-             (11, 9, 8, 4),
-             (11, 9, 8, 3),
-             (11, 9, 7, 4),
-             (11, 9, 7, 2),
-             (11, 9, 6, 5),
-             (11, 9, 6, 3),
-             (11, 9, 5, 3),
-             (11, 8, 6, 4),
-             (11, 8, 6, 3),
-             (11, 7, 6, 5),
-             (11, 7, 6, 4),
-             (11, 10, 9, 8, 7, 4),
-             (11, 10, 9, 8, 7, 1),
-             (11, 10, 9, 8, 5, 4),
-             (11, 10, 9, 8, 4, 3),
-             (11, 10, 9, 8, 3, 1),
-             (11, 10, 9, 7, 5, 1),
-             (11, 10, 9, 7, 4, 1),
-             (11, 10, 9, 6, 5, 4),
-             (11, 10, 9, 6, 4, 2),
-             (11, 10, 9, 6, 3, 1),
-             (11, 10, 9, 6, 2, 1),
-             (11, 10, 9, 5, 4, 3),
-             (11, 10, 9, 5, 4, 1),
-             (11, 10, 9, 5, 3, 1),
-             (11, 10, 9, 4, 3, 2),
-             (11, 10, 8, 7, 6, 5),
-             (11, 10, 8, 7, 6, 3),
-             (11, 10, 8, 7, 5, 3),
-             (11, 10, 8, 7, 4, 1),
-             (11, 10, 8, 6, 5, 4),
-             (11, 10, 8, 6, 5, 1),
-             (11, 10, 8, 6, 4, 3),
-             (11, 10, 8, 6, 4, 2),
-             (11, 10, 8, 5, 3, 2),
-             (11, 10, 8, 4, 3, 2),
-             (11, 10, 7, 6, 5, 3),
-             (11, 10, 7, 6, 5, 1),
-             (11, 10, 7, 6, 4, 2),
-             (11, 10, 7, 6, 4, 1),
-             (11, 10, 7, 6, 3, 2),
-             (11, 10, 7, 4, 3, 2),
-             (11, 9, 8, 7, 6, 3),
-             (11, 9, 8, 7, 4, 2),
-             (11, 9, 8, 6, 5, 2),
-             (11, 9, 8, 6, 4, 3),
-             (11, 9, 7, 6, 5, 4),
-             (11, 9, 7, 6, 5, 3),
-             (11, 9, 7, 6, 4, 2),
-             (11, 9, 6, 5, 4, 3),
-             (11, 8, 7, 6, 4, 3),
-             ),
-        12: (
-             (12, 11, 10, 4),
-             (12, 11, 10, 2),
-             (12, 11, 8, 6),
-             (12, 11, 7, 4),
-             (12, 10, 9, 3),
-             (12, 10, 5, 4),
-             (12, 9, 8, 5),
-             (12, 9, 7, 6),
-             (12, 8, 6, 5),
-             (12, 11, 10, 9, 8, 4),
-             (12, 11, 10, 9, 6, 4),
-             (12, 11, 10, 9, 6, 2),
-             (12, 11, 10, 9, 4, 3),
-             (12, 11, 10, 9, 4, 2),
-             (12, 11, 10, 8, 7, 3),
-             (12, 11, 10, 8, 7, 2),
-             (12, 11, 10, 8, 6, 4),
-             (12, 11, 10, 8, 6, 1),
-             (12, 11, 10, 8, 5, 1),
-             (12, 11, 10, 8, 2, 1),
-             (12, 11, 10, 7, 6, 3),
-             (12, 11, 10, 7, 6, 2),
-             (12, 11, 10, 7, 5, 2),
-             (12, 11, 10, 7, 2, 1),
-             (12, 11, 10, 6, 3, 2),
-             (12, 11, 9, 8, 7, 6),
-             (12, 11, 9, 8, 7, 4),
-             (12, 11, 9, 8, 4, 1),
-             (12, 11, 9, 8, 3, 1),
-             (12, 11, 9, 7, 6, 5),
-             (12, 11, 9, 7, 6, 4),
-             (12, 11, 9, 7, 3, 1),
-             (12, 11, 9, 6, 5, 3),
-             (12, 11, 9, 5, 4, 1),
-             (12, 11, 8, 7, 6, 3),
-             (12, 11, 8, 7, 5, 4),
-             (12, 11, 8, 6, 5, 2),
-             (12, 11, 8, 5, 4, 2),
-             (12, 11, 7, 5, 4, 3),
-             (12, 11, 6, 4, 3, 2),
-             (12, 10, 9, 8, 7, 6),
-             (12, 10, 9, 8, 7, 3),
-             (12, 10, 9, 8, 6, 2),
-             (12, 10, 9, 8, 4, 3),
-             (12, 10, 9, 8, 4, 2),
-             (12, 10, 9, 7, 5, 2),
-             (12, 10, 9, 6, 4, 3),
-             (12, 10, 9, 6, 4, 2),
-             (12, 10, 8, 7, 6, 2),
-             (12, 9, 8, 7, 5, 3),
-             (12, 9, 8, 7, 4, 3),
-             (12, 9, 8, 6, 5, 4),
-             ),
-        13: (
-             (13, 12, 11, 8),
-             (13, 12, 11, 2),
-             (13, 12, 11, 1),
-             (13, 12, 10, 9),
-             (13, 12, 10, 6),
-             (13, 12, 10, 3),
-             (13, 12, 9, 7),
-             (13, 12, 9, 3),
-             (13, 12, 8, 2),
-             (13, 12, 7, 6),
-             (13, 12, 7, 5),
-             (13, 12, 7, 4),
-             (13, 12, 6, 3),
-             (13, 12, 4, 3),
-             (13, 12, 4, 2),
-             (13, 11, 10, 6),
-             (13, 11, 10, 5),
-             (13, 11, 9, 8),
-             (13, 11, 9, 5),
-             (13, 11, 8, 7),
-             (13, 11, 8, 6),
-             (13, 11, 8, 4),
-             (13, 11, 8, 3),
-             (13, 11, 7, 2),
-             (13, 11, 5, 4),
-             (13, 11, 4, 3),
-             (13, 10, 9, 4),
-             (13, 10, 8, 5),
-             (13, 10, 8, 3),
-             (13, 10, 7, 6),
-             (13, 10, 6, 5),
-             (13, 10, 6, 4),
-             (13, 8, 7, 6),
-             (13, 12, 11, 10, 9, 6),
-             (13, 12, 11, 10, 9, 3),
-             (13, 12, 11, 10, 9, 2),
-             (13, 12, 11, 10, 8, 7),
-             (13, 12, 11, 10, 8, 6),
-             (13, 12, 11, 10, 8, 5),
-             (13, 12, 11, 10, 8, 1),
-             (13, 12, 11, 10, 7, 1),
-             ),
-        14: (
-             (14, 13, 12, 2),
-             (14, 13, 11, 9),
-             (14, 13, 11, 4),
-             (14, 13, 10, 8),
-             (14, 13, 10, 6),
-             (14, 13, 10, 3),
-             (14, 13, 8, 6),
-             (14, 13, 8, 4),
-             (14, 13, 8, 3),
-             (14, 13, 7, 3),
-             (14, 13, 4, 2),
-             (14, 13, 3, 2),
-             (14, 12, 11, 6),
-             (14, 12, 11, 5),
-             (14, 12, 9, 2),
-             (14, 12, 7, 5),
-             (14, 11, 10, 9),
-             (14, 11, 10, 3),
-             (14, 11, 9, 7),
-             (14, 11, 6, 5),
-             (14, 9, 8, 5),
-             (14, 13, 12, 11, 10, 8),
-             (14, 13, 12, 11, 10, 2),
-             (14, 13, 12, 11, 9, 7),
-             (14, 13, 12, 11, 9, 1),
-             (14, 13, 12, 11, 8, 7),
-             (14, 13, 12, 11, 5, 4),
-             (14, 13, 12, 11, 5, 2),
-             (14, 13, 12, 11, 4, 2),
-             (14, 13, 12, 10, 8, 5),
-             (14, 13, 12, 10, 4, 2),
-             (14, 13, 12, 10, 4, 1),
-             (14, 13, 12, 9, 8, 3),
-             (14, 13, 12, 9, 8, 1),
-             (14, 13, 12, 9, 7, 6),
-             (14, 13, 12, 9, 5, 4),
-             (14, 13, 12, 8, 7, 5),
-             (14, 13, 12, 8, 5, 4),
-             (14, 13, 12, 8, 4, 3),
-             (14, 13, 12, 8, 4, 2),
-             (14, 13, 12, 8, 4, 1),
-             ),
-        15: (
-             (15, 14),
-             (15, 11),
-             (15, 8),
-             (15, 14, 13, 11),
-             (15, 14, 13, 8),
-             (15, 14, 13, 1),
-             (15, 14, 12, 3),
-             (15, 14, 12, 2),
-             (15, 14, 11, 8),
-             (15, 14, 11, 6),
-             (15, 14, 11, 1),
-             (15, 14, 10, 5),
-             (15, 14, 10, 2),
-             (15, 14, 9, 8),
-             (15, 14, 9, 3),
-             (15, 14, 9, 2),
-             (15, 14, 8, 5),
-             (15, 14, 8, 4),
-             (15, 14, 7, 2),
-             (15, 14, 6, 3),
-             (15, 14, 5, 2),
-             (15, 13, 12, 10),
-             (15, 13, 11, 10),
-             (15, 13, 11, 7),
-             (15, 13, 10, 8),
-             (15, 13, 10, 7),
-             (15, 13, 10, 3),
-             (15, 13, 10, 2),
-             (15, 13, 9, 6),
-             (15, 13, 8, 7),
-             (15, 13, 7, 4),
-             (15, 13, 7, 3),
-             (15, 12, 11, 5),
-             (15, 12, 11, 3),
-             (15, 12, 9, 4),
-             (15, 12, 8, 6),
-             (15, 12, 8, 3),
-             (15, 12, 7, 4),
-             (15, 12, 6, 5),
-             (15, 11, 10, 5),
-             (15, 11, 6, 5),
-             ),
-        16: (
-             (16, 15, 13, 4),
-             (16, 15, 12, 10),
-             (16, 15, 12, 1),
-             (16, 15, 10, 4),
-             (16, 15, 9, 6),
-             (16, 15, 9, 4),
-             (16, 15, 7, 2),
-             (16, 15, 4, 2),
-             (16, 14, 13, 11),
-             (16, 14, 13, 5),
-             (16, 14, 12, 7),
-             (16, 14, 11, 7),
-             (16, 14, 9, 7),
-             (16, 14, 9, 4),
-             (16, 14, 8, 3),
-             (16, 13, 12, 11),
-             (16, 13, 12, 7),
-             (16, 13, 11, 6),
-             (16, 13, 9, 6),
-             (16, 13, 6, 4),
-             (16, 12, 9, 7),
-             (16, 12, 9, 6),
-             (16, 11, 10, 5),
-             (16, 11, 9, 8),
-             (16, 11, 9, 7),
-             (16, 10, 9, 6),
-             (16, 15, 14, 13, 12, 11),
-             (16, 15, 14, 13, 11, 8),
-             (16, 15, 14, 13, 11, 7),
-             (16, 15, 14, 13, 10, 8),
-             (16, 15, 14, 13, 10, 4),
-             (16, 15, 14, 13, 9, 3),
-             (16, 15, 14, 13, 6, 5),
-             (16, 15, 14, 13, 6, 3),
-             (16, 15, 14, 13, 6, 2),
-             (16, 15, 14, 13, 4, 2),
-             (16, 15, 14, 13, 4, 1),
-             (16, 15, 14, 12, 10, 9),
-             (16, 15, 14, 12, 10, 6),
-             (16, 15, 14, 12, 9, 8),
-             (16, 15, 14, 12, 9, 4),
-             ),
-        17: (
-             (17, 14),
-             (17, 12),
-             (17, 11),
-             (17, 16, 15, 14),
-             (17, 16, 15, 7),
-             (17, 16, 14, 9),
-             (17, 16, 14, 6),
-             (17, 16, 14, 4),
-             (17, 16, 14, 1),
-             (17, 16, 13, 12),
-             (17, 16, 13, 5),
-             (17, 16, 13, 2),
-             (17, 16, 12, 10),
-             (17, 16, 12, 8),
-             (17, 16, 12, 4),
-             (17, 16, 12, 1),
-             (17, 16, 11, 7),
-             (17, 16, 11, 1),
-             (17, 16, 10, 9),
-             (17, 16, 10, 8),
-             (17, 16, 10, 5),
-             (17, 16, 9, 5),
-             (17, 16, 9, 4),
-             (17, 16, 8, 6),
-             (17, 16, 8, 3),
-             (17, 16, 5, 4),
-             (17, 16, 5, 3),
-             (17, 16, 3, 2),
-             (17, 15, 14, 12),
-             (17, 15, 14, 10),
-             (17, 15, 14, 9),
-             (17, 15, 14, 8),
-             (17, 15, 14, 6),
-             (17, 15, 14, 5),
-             (17, 15, 13, 11),
-             (17, 15, 13, 7),
-             (17, 15, 13, 5),
-             (17, 15, 12, 9),
-             (17, 15, 12, 2),
-             (17, 15, 11, 10),
-             (17, 15, 11, 8),
-             ),
-        18: (
-             (18, 11),
-             (18, 17, 16, 13),
-             (18, 17, 16, 10),
-             (18, 17, 16, 5),
-             (18, 17, 15, 9),
-             (18, 17, 14, 9),
-             (18, 17, 13, 4),
-             (18, 17, 13, 1),
-             (18, 17, 10, 2),
-             (18, 17, 8, 6),
-             (18, 16, 15, 12),
-             (18, 16, 13, 6),
-             (18, 16, 13, 3),
-             (18, 16, 11, 7),
-             (18, 16, 11, 4),
-             (18, 16, 10, 7),
-             (18, 16, 9, 3),
-             (18, 16, 8, 5),
-             (18, 16, 7, 3),
-             (18, 16, 5, 4),
-             (18, 15, 14, 8),
-             (18, 15, 13, 6),
-             (18, 15, 13, 4),
-             (18, 15, 11, 8),
-             (18, 15, 11, 6),
-             (18, 15, 9, 8),
-             (18, 15, 9, 5),
-             (18, 15, 9, 4),
-             (18, 14, 13, 8),
-             (18, 14, 13, 5),
-             (18, 14, 12, 5),
-             (18, 14, 11, 10),
-             (18, 13, 12, 9),
-             (18, 13, 11, 8),
-             (18, 13, 11, 5),
-             (18, 13, 10, 8),
-             (18, 13, 9, 6),
-             (18, 17, 16, 15, 14, 13),
-             (18, 17, 16, 15, 13, 2),
-             (18, 17, 16, 15, 12, 10),
-             (18, 17, 16, 15, 12, 4),
-             ),
-        19: (
-             (19, 18, 17, 14),
-             (19, 18, 17, 13),
-             (19, 18, 17, 5),
-             (19, 18, 16, 10),
-             (19, 18, 16, 5),
-             (19, 18, 15, 13),
-             (19, 18, 15, 12),
-             (19, 18, 15, 10),
-             (19, 18, 15, 3),
-             (19, 18, 14, 13),
-             (19, 18, 14, 1),
-             (19, 18, 13, 11),
-             (19, 18, 13, 8),
-             (19, 18, 13, 3),
-             (19, 18, 13, 1),
-             (19, 18, 12, 10),
-             (19, 18, 12, 3),
-             (19, 18, 10, 6),
-             (19, 18, 10, 2),
-             (19, 18, 9, 6),
-             (19, 18, 9, 4),
-             (19, 18, 8, 7),
-             (19, 18, 8, 2),
-             (19, 18, 7, 5),
-             (19, 18, 7, 3),
-             (19, 18, 5, 2),
-             (19, 17, 16, 6),
-             (19, 17, 15, 8),
-             (19, 17, 14, 10),
-             (19, 17, 14, 3),
-             (19, 17, 13, 8),
-             (19, 17, 13, 5),
-             (19, 17, 12, 11),
-             (19, 17, 12, 10),
-             (19, 17, 12, 4),
-             (19, 17, 11, 6),
-             (19, 17, 10, 6),
-             (19, 17, 10, 3),
-             (19, 17, 7, 3),
-             (19, 17, 6, 5),
-             (19, 17, 5, 4),
-             ),
-        20: (
-             (20, 17),
-             (20, 19, 16, 14),
-             (20, 19, 16, 2),
-             (20, 19, 15, 11),
-             (20, 19, 15, 10),
-             (20, 19, 15, 4),
-             (20, 19, 14, 9),
-             (20, 19, 14, 4),
-             (20, 19, 12, 8),
-             (20, 19, 11, 7),
-             (20, 19, 9, 8),
-             (20, 19, 9, 2),
-             (20, 19, 8, 4),
-             (20, 19, 7, 6),
-             (20, 19, 4, 3),
-             (20, 18, 15, 14),
-             (20, 18, 13, 10),
-             (20, 18, 13, 7),
-             (20, 18, 11, 10),
-             (20, 18, 11, 8),
-             (20, 18, 11, 5),
-             (20, 18, 9, 3),
-             (20, 17, 16, 9),
-             (20, 17, 15, 14),
-             (20, 17, 15, 11),
-             (20, 17, 15, 9),
-             (20, 17, 14, 8),
-             (20, 17, 14, 3),
-             (20, 17, 13, 4),
-             (20, 17, 12, 10),
-             (20, 17, 11, 9),
-             (20, 17, 9, 8),
-             (20, 17, 9, 7),
-             (20, 17, 9, 4),
-             (20, 17, 6, 4),
-             (20, 16, 15, 11),
-             (20, 16, 15, 5),
-             (20, 16, 13, 9),
-             (20, 16, 13, 5),
-             (20, 16, 12, 7),
-             (20, 16, 10, 9),
-             ),
-        21: (
-             (21, 19),
-             (21, 20, 19, 16),
-             (21, 20, 19, 13),
-             (21, 20, 19, 7),
-             (21, 20, 19, 5),
-             (21, 20, 19, 4),
-             (21, 20, 19, 2),
-             (21, 20, 18, 6),
-             (21, 20, 17, 14),
-             (21, 20, 17, 10),
-             (21, 20, 17, 7),
-             (21, 20, 17, 3),
-             (21, 20, 17, 2),
-             (21, 20, 16, 11),
-             (21, 20, 16, 2),
-             (21, 20, 14, 10),
-             (21, 20, 14, 8),
-             (21, 20, 13, 7),
-             (21, 20, 11, 9),
-             (21, 20, 9, 3),
-             (21, 20, 8, 3),
-             (21, 20, 7, 5),
-             (21, 20, 6, 5),
-             (21, 20, 5, 2),
-             (21, 19, 18, 10),
-             (21, 19, 17, 11),
-             (21, 19, 17, 10),
-             (21, 19, 17, 4),
-             (21, 19, 16, 15),
-             (21, 19, 16, 12),
-             (21, 19, 16, 8),
-             (21, 19, 16, 5),
-             (21, 19, 15, 9),
-             (21, 19, 15, 4),
-             (21, 19, 14, 13),
-             (21, 19, 14, 7),
-             (21, 19, 13, 6),
-             (21, 19, 12, 6),
-             (21, 19, 11, 8),
-             (21, 19, 11, 4),
-             (21, 19, 10, 5),
-             ),
-        22: (
-             (22, 21),
-             (22, 21, 20, 11),
-             (22, 21, 20, 7),
-             (22, 21, 19, 10),
-             (22, 21, 19, 2),
-             (22, 21, 18, 12),
-             (22, 21, 17, 13),
-             (22, 21, 17, 8),
-             (22, 21, 16, 15),
-             (22, 21, 15, 6),
-             (22, 21, 14, 11),
-             (22, 21, 13, 1),
-             (22, 21, 12, 9),
-             (22, 21, 10, 9),
-             (22, 21, 10, 6),
-             (22, 21, 10, 5),
-             (22, 21, 7, 2),
-             (22, 21, 5, 4),
-             (22, 20, 19, 8),
-             (22, 20, 19, 3),
-             (22, 20, 16, 3),
-             (22, 20, 14, 13),
-             (22, 20, 13, 9),
-             (22, 20, 13, 8),
-             (22, 20, 13, 6),
-             (22, 20, 11, 10),
-             (22, 20, 11, 9),
-             (22, 20, 11, 4),
-             (22, 20, 11, 3),
-             (22, 19, 18, 17),
-             (22, 19, 17, 14),
-             (22, 19, 17, 11),
-             (22, 19, 17, 9),
-             (22, 19, 16, 6),
-             (22, 19, 16, 4),
-             (22, 19, 15, 12),
-             (22, 19, 15, 10),
-             (22, 19, 15, 5),
-             (22, 19, 14, 5),
-             (22, 19, 12, 9),
-             (22, 19, 6, 5),
-             ),
-        23: (
-             (23, 18),
-             (23, 14),
-             (23, 22, 21, 16),
-             (23, 22, 21, 8),
-             (23, 22, 21, 2),
-             (23, 22, 21, 1),
-             (23, 22, 20, 18),
-             (23, 22, 20, 16),
-             (23, 22, 20, 4),
-             (23, 22, 20, 3),
-             (23, 22, 19, 18),
-             (23, 22, 19, 8),
-             (23, 22, 19, 3),
-             (23, 22, 18, 16),
-             (23, 22, 18, 11),
-             (23, 22, 18, 8),
-             (23, 22, 18, 5),
-             (23, 22, 18, 4),
-             (23, 22, 17, 10),
-             (23, 22, 17, 6),
-             (23, 22, 16, 15),
-             (23, 22, 16, 8),
-             (23, 22, 16, 6),
-             (23, 22, 15, 14),
-             (23, 22, 15, 1),
-             (23, 22, 14, 12),
-             (23, 22, 14, 10),
-             (23, 22, 14, 7),
-             (23, 22, 13, 6),
-             (23, 22, 12, 10),
-             (23, 22, 12, 8),
-             (23, 22, 12, 4),
-             (23, 22, 11, 10),
-             (23, 22, 10, 5),
-             (23, 22, 8, 7),
-             (23, 22, 8, 4),
-             (23, 22, 6, 5),
-             (23, 22, 5, 4),
-             (23, 22, 4, 2),
-             (23, 21, 20, 18),
-             (23, 21, 20, 17),
-             ),
-        24: (
-             (24, 23, 22, 17),
-             (24, 23, 22, 7),
-             (24, 23, 21, 20),
-             (24, 23, 21, 11),
-             (24, 23, 21, 8),
-             (24, 23, 19, 2),
-             (24, 23, 18, 14),
-             (24, 23, 16, 13),
-             (24, 23, 14, 1),
-             (24, 23, 10, 8),
-             (24, 23, 9, 3),
-             (24, 23, 5, 4),
-             (24, 22, 21, 12),
-             (24, 22, 21, 9),
-             (24, 22, 20, 7),
-             (24, 22, 19, 16),
-             (24, 22, 19, 15),
-             (24, 22, 19, 13),
-             (24, 22, 19, 8),
-             (24, 22, 19, 6),
-             (24, 22, 18, 13),
-             (24, 22, 17, 8),
-             (24, 22, 16, 7),
-             (24, 22, 15, 4),
-             (24, 22, 15, 3),
-             (24, 22, 14, 13),
-             (24, 22, 9, 3),
-             (24, 22, 8, 7),
-             (24, 22, 7, 6),
-             (24, 21, 20, 14),
-             (24, 21, 18, 14),
-             (24, 21, 18, 5),
-             (24, 21, 11, 5),
-             (24, 20, 19, 17),
-             (24, 20, 19, 5),
-             (24, 20, 18, 15),
-             (24, 20, 11, 9),
-             (24, 20, 11, 5),
-             (24, 19, 14, 11),
-             (24, 19, 13, 11),
-             (24, 19, 9, 6),
-             ),
-        25: (
-             (25, 22),
-             (25, 18),
-             (25, 24, 23, 22),
-             (25, 24, 23, 2),
-             (25, 24, 22, 15),
-             (25, 24, 22, 13),
-             (25, 24, 22, 8),
-             (25, 24, 22, 5),
-             (25, 24, 22, 3),
-             (25, 24, 21, 18),
-             (25, 24, 21, 9),
-             (25, 24, 20, 16),
-             (25, 24, 20, 13),
-             (25, 24, 20, 11),
-             (25, 24, 20, 8),
-             (25, 24, 20, 4),
-             (25, 24, 19, 11),
-             (25, 24, 19, 8),
-             (25, 24, 19, 1),
-             (25, 24, 18, 4),
-             (25, 24, 18, 3),
-             (25, 24, 17, 8),
-             (25, 24, 17, 4),
-             (25, 24, 17, 2),
-             (25, 24, 17, 1),
-             (25, 24, 16, 13),
-             (25, 24, 16, 9),
-             (25, 24, 16, 7),
-             (25, 24, 16, 1),
-             (25, 24, 15, 12),
-             (25, 24, 15, 3),
-             (25, 24, 13, 12),
-             (25, 24, 13, 11),
-             (25, 24, 13, 6),
-             (25, 24, 13, 5),
-             (25, 24, 13, 4),
-             (25, 24, 13, 1),
-             (25, 24, 12, 9),
-             (25, 24, 11, 10),
-             (25, 24, 11, 7),
-             (25, 24, 11, 5),
-             ),
-        26: (
-             (26, 25, 24, 20),
-             (26, 25, 24, 8),
-             (26, 25, 24, 7),
-             (26, 25, 22, 17),
-             (26, 25, 22, 14),
-             (26, 25, 22, 3),
-             (26, 25, 22, 2),
-             (26, 25, 21, 1),
-             (26, 25, 20, 15),
-             (26, 25, 19, 18),
-             (26, 25, 19, 3),
-             (26, 25, 18, 13),
-             (26, 25, 18, 2),
-             (26, 25, 17, 9),
-             (26, 25, 17, 7),
-             (26, 25, 16, 5),
-             (26, 25, 15, 13),
-             (26, 25, 14, 3),
-             (26, 25, 13, 3),
-             (26, 25, 13, 2),
-             (26, 25, 12, 11),
-             (26, 25, 12, 7),
-             (26, 25, 11, 9),
-             (26, 25, 11, 7),
-             (26, 25, 10, 8),
-             (26, 25, 10, 6),
-             (26, 25, 9, 4),
-             (26, 25, 8, 6),
-             (26, 25, 7, 3),
-             (26, 24, 23, 20),
-             (26, 24, 23, 10),
-             (26, 24, 22, 7),
-             (26, 24, 21, 5),
-             (26, 24, 20, 17),
-             (26, 24, 20, 9),
-             (26, 24, 19, 17),
-             (26, 24, 18, 5),
-             (26, 24, 17, 9),
-             (26, 24, 17, 7),
-             (26, 24, 17, 5),
-             (26, 24, 16, 13),
-             ),
-        27: (
-             (27, 26, 25, 22),
-             (27, 26, 25, 17),
-             (27, 26, 25, 11),
-             (27, 26, 24, 11),
-             (27, 26, 23, 7),
-             (27, 26, 22, 10),
-             (27, 26, 22, 2),
-             (27, 26, 22, 1),
-             (27, 26, 21, 11),
-             (27, 26, 20, 19),
-             (27, 26, 20, 9),
-             (27, 26, 18, 11),
-             (27, 26, 17, 9),
-             (27, 26, 17, 1),
-             (27, 26, 16, 14),
-             (27, 26, 16, 7),
-             (27, 26, 16, 2),
-             (27, 26, 15, 2),
-             (27, 26, 14, 9),
-             (27, 26, 14, 7),
-             (27, 26, 13, 2),
-             (27, 26, 12, 6),
-             (27, 26, 10, 5),
-             (27, 26, 6, 3),
-             (27, 26, 3, 2),
-             (27, 25, 24, 15),
-             (27, 25, 23, 10),
-             (27, 25, 23, 7),
-             (27, 25, 22, 18),
-             (27, 25, 22, 14),
-             (27, 25, 22, 3),
-             (27, 25, 21, 15),
-             (27, 25, 21, 9),
-             (27, 25, 21, 4),
-             (27, 25, 20, 17),
-             (27, 25, 20, 11),
-             (27, 25, 20, 8),
-             (27, 25, 20, 4),
-             (27, 25, 19, 18),
-             (27, 25, 19, 8),
-             (27, 25, 19, 3),
-             ),
-        28: (
-             (28, 25),
-             (28, 19),
-             (28, 15),
-             (28, 27, 26, 16),
-             (28, 27, 26, 11),
-             (28, 27, 25, 18),
-             (28, 27, 25, 6),
-             (28, 27, 24, 22),
-             (28, 27, 24, 7),
-             (28, 27, 23, 19),
-             (28, 27, 23, 4),
-             (28, 27, 21, 13),
-             (28, 27, 21, 7),
-             (28, 27, 20, 14),
-             (28, 27, 20, 11),
-             (28, 27, 17, 1),
-             (28, 27, 16, 5),
-             (28, 27, 16, 3),
-             (28, 27, 15, 7),
-             (28, 27, 15, 3),
-             (28, 27, 14, 5),
-             (28, 27, 13, 8),
-             (28, 27, 13, 4),
-             (28, 27, 8, 7),
-             (28, 27, 5, 4),
-             (28, 26, 23, 15),
-             (28, 26, 23, 13),
-             (28, 26, 23, 9),
-             (28, 26, 21, 14),
-             (28, 26, 21, 5),
-             (28, 26, 20, 13),
-             (28, 26, 20, 7),
-             (28, 26, 19, 6),
-             (28, 26, 15, 11),
-             (28, 26, 10, 5),
-             (28, 26, 10, 3),
-             (28, 26, 6, 5),
-             (28, 25, 24, 11),
-             (28, 25, 24, 9),
-             (28, 25, 23, 18),
-             (28, 25, 22, 12),
-             ),
-        29: (
-             (29, 27),
-             (29, 28, 27, 25),
-             (29, 28, 27, 20),
-             (29, 28, 27, 8),
-             (29, 28, 27, 4),
-             (29, 28, 26, 10),
-             (29, 28, 25, 6),
-             (29, 28, 24, 19),
-             (29, 28, 24, 2),
-             (29, 28, 23, 22),
-             (29, 28, 23, 19),
-             (29, 28, 23, 15),
-             (29, 28, 21, 11),
-             (29, 28, 20, 10),
-             (29, 28, 20, 7),
-             (29, 28, 19, 15),
-             (29, 28, 17, 10),
-             (29, 28, 17, 3),
-             (29, 28, 15, 8),
-             (29, 28, 15, 5),
-             (29, 28, 14, 4),
-             (29, 28, 13, 6),
-             (29, 28, 12, 10),
-             (29, 28, 11, 4),
-             (29, 28, 10, 2),
-             (29, 28, 8, 6),
-             (29, 27, 26, 25),
-             (29, 27, 26, 22),
-             (29, 27, 26, 19),
-             (29, 27, 26, 17),
-             (29, 27, 26, 15),
-             (29, 27, 26, 11),
-             (29, 27, 25, 20),
-             (29, 27, 25, 14),
-             (29, 27, 25, 13),
-             (29, 27, 25, 7),
-             (29, 27, 24, 15),
-             (29, 27, 24, 11),
-             (29, 27, 24, 9),
-             (29, 27, 24, 8),
-             (29, 27, 24, 3),
-             ),
-        30: (
-             (30, 29, 28, 7),
-             (30, 29, 26, 24),
-             (30, 29, 26, 22),
-             (30, 29, 26, 4),
-             (30, 29, 24, 17),
-             (30, 29, 24, 12),
-             (30, 29, 23, 20),
-             (30, 29, 23, 18),
-             (30, 29, 23, 13),
-             (30, 29, 23, 8),
-             (30, 29, 22, 7),
-             (30, 29, 19, 17),
-             (30, 29, 19, 10),
-             (30, 29, 19, 8),
-             (30, 29, 18, 9),
-             (30, 29, 18, 3),
-             (30, 29, 17, 7),
-             (30, 29, 17, 5),
-             (30, 29, 16, 4),
-             (30, 29, 15, 14),
-             (30, 29, 14, 2),
-             (30, 29, 12, 3),
-             (30, 29, 10, 4),
-             (30, 29, 9, 6),
-             (30, 29, 8, 5),
-             (30, 28, 27, 6),
-             (30, 28, 26, 7),
-             (30, 28, 23, 17),
-             (30, 28, 23, 11),
-             (30, 28, 23, 10),
-             (30, 28, 23, 4),
-             (30, 28, 22, 17),
-             (30, 28, 21, 12),
-             (30, 28, 21, 7),
-             (30, 28, 20, 19),
-             (30, 28, 20, 17),
-             (30, 28, 19, 7),
-             (30, 28, 18, 7),
-             (30, 28, 16, 9),
-             (30, 28, 15, 12),
-             (30, 28, 14, 5),
-             ),
-        31: (
-             (31, 28),
-             (31, 25),
-             (31, 24),
-             (31, 18),
-             (31, 30, 29, 28),
-             (31, 30, 29, 25),
-             (31, 30, 29, 20),
-             (31, 30, 29, 19),
-             (31, 30, 29, 5),
-             (31, 30, 28, 24),
-             (31, 30, 28, 22),
-             (31, 30, 28, 18),
-             (31, 30, 28, 16),
-             (31, 30, 28, 13),
-             (31, 30, 28, 10),
-             (31, 30, 28, 8),
-             (31, 30, 28, 3),
-             (31, 30, 27, 16),
-             (31, 30, 26, 22),
-             (31, 30, 26, 8),
-             (31, 30, 25, 16),
-             (31, 30, 25, 9),
-             (31, 30, 25, 7),
-             (31, 30, 25, 5),
-             (31, 30, 24, 19),
-             (31, 30, 24, 16),
-             (31, 30, 24, 12),
-             (31, 30, 23, 20),
-             (31, 30, 23, 19),
-             (31, 30, 23, 5),
-             (31, 30, 22, 21),
-             (31, 30, 22, 20),
-             (31, 30, 22, 12),
-             (31, 30, 22, 4),
-             (31, 30, 21, 18),
-             (31, 30, 21, 10),
-             (31, 30, 20, 11),
-             (31, 30, 20, 8),
-             (31, 30, 20, 7),
-             (31, 30, 20, 1),
-             (31, 30, 19, 17),
-             ),
-        32: (
-             (32, 31, 30, 10),
-             (32, 31, 29, 1),
-             (32, 31, 26, 18),
-             (32, 31, 26, 9),
-             (32, 31, 26, 7),
-             (32, 31, 23, 10),
-             (32, 31, 22, 17),
-             (32, 31, 21, 16),
-             (32, 31, 21, 5),
-             (32, 31, 18, 10),
-             (32, 31, 16, 2),
-             (32, 31, 15, 10),
-             (32, 31, 14, 4),
-             (32, 31, 13, 8),
-             (32, 31, 9, 7),
-             (32, 31, 5, 4),
-             (32, 30, 29, 23),
-             (32, 30, 29, 20),
-             (32, 30, 29, 16),
-             (32, 30, 29, 15),
-             (32, 30, 27, 24),
-             (32, 30, 27, 21),
-             (32, 30, 27, 12),
-             (32, 30, 27, 8),
-             (32, 30, 26, 25),
-             (32, 30, 26, 13),
-             (32, 30, 25, 16),
-             (32, 30, 23, 16),
-             (32, 30, 23, 14),
-             (32, 30, 23, 4),
-             (32, 30, 21, 14),
-             (32, 30, 19, 8),
-             (32, 30, 19, 4),
-             (32, 30, 17, 3),
-             (32, 30, 15, 6),
-             (32, 30, 11, 8),
-             (32, 30, 11, 5),
-             (32, 30, 8, 3),
-             (32, 30, 7, 4),
-             (32, 29, 28, 19),
-             (32, 29, 27, 23),
-             ),
-        }
+    3 : (
+        (3, 2),
+        ),
+    4 : (
+        (4, 3),
+        ),
+    5 : (
+        (5, 3),
+        (5, 4, 3, 2),
+        (5, 4, 3, 1),
+        ),
+    6 : (
+        (6, 5),
+        (6, 5, 4, 1),
+        (6, 5, 3, 2),
+        ),
+    7 : (
+        (7, 6),
+        (7, 4),
+        (7, 6, 5, 4),
+        (7, 6, 5, 2),
+        (7, 6, 4, 2),
+        (7, 6, 4, 1),
+        (7, 5, 4, 3),
+        (7, 6, 5, 4, 3, 2),
+        (7, 6, 5, 4, 2, 1),
+        ),
+    8 : (
+        (8, 7, 6, 1),
+        (8, 7, 5, 3),
+        (8, 7, 3, 2),
+        (8, 6, 5, 4),
+        (8, 6, 5, 3),
+        (8, 6, 5, 2),
+        (8, 7, 6, 5, 4, 2),
+        (8, 7, 6, 5, 2, 1),
+        ),
+    9 : (
+        (9, 5),
+        (9, 8, 7, 2),
+        (9, 8, 6, 5),
+        (9, 8, 5, 4),
+        (9, 8, 5, 1),
+        (9, 8, 4, 2),
+        (9, 7, 6, 4),
+        (9, 7, 5, 2),
+        (9, 6, 5, 3),
+        (9, 8, 7, 6, 5, 3),
+        (9, 8, 7, 6, 5, 1),
+        (9, 8, 7, 6, 4, 3),
+        (9, 8, 7, 6, 4, 2),
+        (9, 8, 7, 6, 3, 2),
+        (9, 8, 7, 6, 3, 1),
+        (9, 8, 7, 6, 2, 1),
+        (9, 8, 7, 5, 4, 3),
+        (9, 8, 7, 5, 4, 2),
+        (9, 8, 6, 5, 4, 1),
+        (9, 8, 6, 5, 3, 2),
+        (9, 8, 6, 5, 3, 1),
+        (9, 7, 6, 5, 4, 3),
+        (9, 7, 6, 5, 4, 2),
+        (9, 8, 7, 6, 5, 4, 3, 1),
+        ),
+    10: (
+        (10, 7),
+        (10, 9, 8, 5),
+        (10, 9, 7, 6),
+        (10, 9, 7, 3),
+        (10, 9, 6, 1),
+        (10, 9, 5, 2),
+        (10, 9, 4, 2),
+        (10, 8, 7, 5),
+        (10, 8, 7, 2),
+        (10, 8, 5, 4),
+        (10, 8, 4, 3),
+        (10, 9, 8, 7, 5, 4),
+        (10, 9, 8, 7, 4, 1),
+        (10, 9, 8, 7, 3, 2),
+        (10, 9, 8, 6, 5, 1),
+        (10, 9, 8, 6, 4, 3),
+        (10, 9, 8, 6, 4, 2),
+        (10, 9, 8, 6, 3, 2),
+        (10, 9, 8, 6, 2, 1),
+        (10, 9, 8, 5, 4, 3),
+        (10, 9, 8, 4, 3, 2),
+        (10, 9, 7, 6, 4, 1),
+        (10, 9, 7, 5, 4, 2),
+        (10, 9, 6, 5, 4, 3),
+        (10, 8, 7, 6, 5, 2),
+        (10, 9, 8, 7, 6, 5, 4, 3),
+        (10, 9, 8, 7, 6, 5, 4, 1),
+        (10, 9, 8, 7, 6, 4, 3, 1),
+        (10, 9, 8, 6, 5, 4, 3, 2),
+        (10, 9, 7, 6, 5, 4, 3, 2),
+        ),
+    11: (
+        (11, 9),
+        (11, 10, 9, 7),
+        (11, 10, 9, 5),
+        (11, 10, 9, 2),
+        (11, 10, 8, 6),
+        (11, 10, 8, 1),
+        (11, 10, 7, 3),
+        (11, 10, 7, 2),
+        (11, 10, 6, 5),
+        (11, 10, 4, 3),
+        (11, 10, 3, 2),
+        (11, 9, 8, 6),
+        (11, 9, 8, 4),
+        (11, 9, 8, 3),
+        (11, 9, 7, 4),
+        (11, 9, 7, 2),
+        (11, 9, 6, 5),
+        (11, 9, 6, 3),
+        (11, 9, 5, 3),
+        (11, 8, 6, 4),
+        (11, 8, 6, 3),
+        (11, 7, 6, 5),
+        (11, 7, 6, 4),
+        (11, 10, 9, 8, 7, 4),
+        (11, 10, 9, 8, 7, 1),
+        (11, 10, 9, 8, 5, 4),
+        (11, 10, 9, 8, 4, 3),
+        (11, 10, 9, 8, 3, 1),
+        (11, 10, 9, 7, 5, 1),
+        (11, 10, 9, 7, 4, 1),
+        (11, 10, 9, 6, 5, 4),
+        (11, 10, 9, 6, 4, 2),
+        (11, 10, 9, 6, 3, 1),
+        (11, 10, 9, 6, 2, 1),
+        (11, 10, 9, 5, 4, 3),
+        (11, 10, 9, 5, 4, 1),
+        (11, 10, 9, 5, 3, 1),
+        (11, 10, 9, 4, 3, 2),
+        (11, 10, 8, 7, 6, 5),
+        (11, 10, 8, 7, 6, 3),
+        (11, 10, 8, 7, 5, 3),
+        (11, 10, 8, 7, 4, 1),
+        (11, 10, 8, 6, 5, 4),
+        (11, 10, 8, 6, 5, 1),
+        (11, 10, 8, 6, 4, 3),
+        (11, 10, 8, 6, 4, 2),
+        (11, 10, 8, 5, 3, 2),
+        (11, 10, 8, 4, 3, 2),
+        (11, 10, 7, 6, 5, 3),
+        (11, 10, 7, 6, 5, 1),
+        (11, 10, 7, 6, 4, 2),
+        (11, 10, 7, 6, 4, 1),
+        (11, 10, 7, 6, 3, 2),
+        (11, 10, 7, 4, 3, 2),
+        (11, 9, 8, 7, 6, 3),
+        (11, 9, 8, 7, 4, 2),
+        (11, 9, 8, 6, 5, 2),
+        (11, 9, 8, 6, 4, 3),
+        (11, 9, 7, 6, 5, 4),
+        (11, 9, 7, 6, 5, 3),
+        (11, 9, 7, 6, 4, 2),
+        (11, 9, 6, 5, 4, 3),
+        (11, 8, 7, 6, 4, 3),
+        ),
+    12: (
+        (12, 11, 10, 4),
+        (12, 11, 10, 2),
+        (12, 11, 8, 6),
+        (12, 11, 7, 4),
+        (12, 10, 9, 3),
+        (12, 10, 5, 4),
+        (12, 9, 8, 5),
+        (12, 9, 7, 6),
+        (12, 8, 6, 5),
+        (12, 11, 10, 9, 8, 4),
+        (12, 11, 10, 9, 6, 4),
+        (12, 11, 10, 9, 6, 2),
+        (12, 11, 10, 9, 4, 3),
+        (12, 11, 10, 9, 4, 2),
+        (12, 11, 10, 8, 7, 3),
+        (12, 11, 10, 8, 7, 2),
+        (12, 11, 10, 8, 6, 4),
+        (12, 11, 10, 8, 6, 1),
+        (12, 11, 10, 8, 5, 1),
+        (12, 11, 10, 8, 2, 1),
+        (12, 11, 10, 7, 6, 3),
+        (12, 11, 10, 7, 6, 2),
+        (12, 11, 10, 7, 5, 2),
+        (12, 11, 10, 7, 2, 1),
+        (12, 11, 10, 6, 3, 2),
+        (12, 11, 9, 8, 7, 6),
+        (12, 11, 9, 8, 7, 4),
+        (12, 11, 9, 8, 4, 1),
+        (12, 11, 9, 8, 3, 1),
+        (12, 11, 9, 7, 6, 5),
+        (12, 11, 9, 7, 6, 4),
+        (12, 11, 9, 7, 3, 1),
+        (12, 11, 9, 6, 5, 3),
+        (12, 11, 9, 5, 4, 1),
+        (12, 11, 8, 7, 6, 3),
+        (12, 11, 8, 7, 5, 4),
+        (12, 11, 8, 6, 5, 2),
+        (12, 11, 8, 5, 4, 2),
+        (12, 11, 7, 5, 4, 3),
+        (12, 11, 6, 4, 3, 2),
+        (12, 10, 9, 8, 7, 6),
+        (12, 10, 9, 8, 7, 3),
+        (12, 10, 9, 8, 6, 2),
+        (12, 10, 9, 8, 4, 3),
+        (12, 10, 9, 8, 4, 2),
+        (12, 10, 9, 7, 5, 2),
+        (12, 10, 9, 6, 4, 3),
+        (12, 10, 9, 6, 4, 2),
+        (12, 10, 8, 7, 6, 2),
+        (12, 9, 8, 7, 5, 3),
+        (12, 9, 8, 7, 4, 3),
+        (12, 9, 8, 6, 5, 4),
+        ),
+    13: (
+        (13, 12, 11, 8),
+        (13, 12, 11, 2),
+        (13, 12, 11, 1),
+        (13, 12, 10, 9),
+        (13, 12, 10, 6),
+        (13, 12, 10, 3),
+        (13, 12, 9, 7),
+        (13, 12, 9, 3),
+        (13, 12, 8, 2),
+        (13, 12, 7, 6),
+        (13, 12, 7, 5),
+        (13, 12, 7, 4),
+        (13, 12, 6, 3),
+        (13, 12, 4, 3),
+        (13, 12, 4, 2),
+        (13, 11, 10, 6),
+        (13, 11, 10, 5),
+        (13, 11, 9, 8),
+        (13, 11, 9, 5),
+        (13, 11, 8, 7),
+        (13, 11, 8, 6),
+        (13, 11, 8, 4),
+        (13, 11, 8, 3),
+        (13, 11, 7, 2),
+        (13, 11, 5, 4),
+        (13, 11, 4, 3),
+        (13, 10, 9, 4),
+        (13, 10, 8, 5),
+        (13, 10, 8, 3),
+        (13, 10, 7, 6),
+        (13, 10, 6, 5),
+        (13, 10, 6, 4),
+        (13, 8, 7, 6),
+        (13, 12, 11, 10, 9, 6),
+        (13, 12, 11, 10, 9, 3),
+        (13, 12, 11, 10, 9, 2),
+        (13, 12, 11, 10, 8, 7),
+        (13, 12, 11, 10, 8, 6),
+        (13, 12, 11, 10, 8, 5),
+        (13, 12, 11, 10, 8, 1),
+        (13, 12, 11, 10, 7, 1),
+        ),
+    14: (
+        (14, 13, 12, 2),
+        (14, 13, 11, 9),
+        (14, 13, 11, 4),
+        (14, 13, 10, 8),
+        (14, 13, 10, 6),
+        (14, 13, 10, 3),
+        (14, 13, 8, 6),
+        (14, 13, 8, 4),
+        (14, 13, 8, 3),
+        (14, 13, 7, 3),
+        (14, 13, 4, 2),
+        (14, 13, 3, 2),
+        (14, 12, 11, 6),
+        (14, 12, 11, 5),
+        (14, 12, 9, 2),
+        (14, 12, 7, 5),
+        (14, 11, 10, 9),
+        (14, 11, 10, 3),
+        (14, 11, 9, 7),
+        (14, 11, 6, 5),
+        (14, 9, 8, 5),
+        (14, 13, 12, 11, 10, 8),
+        (14, 13, 12, 11, 10, 2),
+        (14, 13, 12, 11, 9, 7),
+        (14, 13, 12, 11, 9, 1),
+        (14, 13, 12, 11, 8, 7),
+        (14, 13, 12, 11, 5, 4),
+        (14, 13, 12, 11, 5, 2),
+        (14, 13, 12, 11, 4, 2),
+        (14, 13, 12, 10, 8, 5),
+        (14, 13, 12, 10, 4, 2),
+        (14, 13, 12, 10, 4, 1),
+        (14, 13, 12, 9, 8, 3),
+        (14, 13, 12, 9, 8, 1),
+        (14, 13, 12, 9, 7, 6),
+        (14, 13, 12, 9, 5, 4),
+        (14, 13, 12, 8, 7, 5),
+        (14, 13, 12, 8, 5, 4),
+        (14, 13, 12, 8, 4, 3),
+        (14, 13, 12, 8, 4, 2),
+        (14, 13, 12, 8, 4, 1),
+        ),
+    15: (
+        (15, 14),
+        (15, 11),
+        (15, 8),
+        (15, 14, 13, 11),
+        (15, 14, 13, 8),
+        (15, 14, 13, 1),
+        (15, 14, 12, 3),
+        (15, 14, 12, 2),
+        (15, 14, 11, 8),
+        (15, 14, 11, 6),
+        (15, 14, 11, 1),
+        (15, 14, 10, 5),
+        (15, 14, 10, 2),
+        (15, 14, 9, 8),
+        (15, 14, 9, 3),
+        (15, 14, 9, 2),
+        (15, 14, 8, 5),
+        (15, 14, 8, 4),
+        (15, 14, 7, 2),
+        (15, 14, 6, 3),
+        (15, 14, 5, 2),
+        (15, 13, 12, 10),
+        (15, 13, 11, 10),
+        (15, 13, 11, 7),
+        (15, 13, 10, 8),
+        (15, 13, 10, 7),
+        (15, 13, 10, 3),
+        (15, 13, 10, 2),
+        (15, 13, 9, 6),
+        (15, 13, 8, 7),
+        (15, 13, 7, 4),
+        (15, 13, 7, 3),
+        (15, 12, 11, 5),
+        (15, 12, 11, 3),
+        (15, 12, 9, 4),
+        (15, 12, 8, 6),
+        (15, 12, 8, 3),
+        (15, 12, 7, 4),
+        (15, 12, 6, 5),
+        (15, 11, 10, 5),
+        (15, 11, 6, 5),
+        ),
+    16: (
+        (16, 15, 13, 4),
+        (16, 15, 12, 10),
+        (16, 15, 12, 1),
+        (16, 15, 10, 4),
+        (16, 15, 9, 6),
+        (16, 15, 9, 4),
+        (16, 15, 7, 2),
+        (16, 15, 4, 2),
+        (16, 14, 13, 11),
+        (16, 14, 13, 5),
+        (16, 14, 12, 7),
+        (16, 14, 11, 7),
+        (16, 14, 9, 7),
+        (16, 14, 9, 4),
+        (16, 14, 8, 3),
+        (16, 13, 12, 11),
+        (16, 13, 12, 7),
+        (16, 13, 11, 6),
+        (16, 13, 9, 6),
+        (16, 13, 6, 4),
+        (16, 12, 9, 7),
+        (16, 12, 9, 6),
+        (16, 11, 10, 5),
+        (16, 11, 9, 8),
+        (16, 11, 9, 7),
+        (16, 10, 9, 6),
+        (16, 15, 14, 13, 12, 11),
+        (16, 15, 14, 13, 11, 8),
+        (16, 15, 14, 13, 11, 7),
+        (16, 15, 14, 13, 10, 8),
+        (16, 15, 14, 13, 10, 4),
+        (16, 15, 14, 13, 9, 3),
+        (16, 15, 14, 13, 6, 5),
+        (16, 15, 14, 13, 6, 3),
+        (16, 15, 14, 13, 6, 2),
+        (16, 15, 14, 13, 4, 2),
+        (16, 15, 14, 13, 4, 1),
+        (16, 15, 14, 12, 10, 9),
+        (16, 15, 14, 12, 10, 6),
+        (16, 15, 14, 12, 9, 8),
+        (16, 15, 14, 12, 9, 4),
+        ),
+    17: (
+        (17, 14),
+        (17, 12),
+        (17, 11),
+        (17, 16, 15, 14),
+        (17, 16, 15, 7),
+        (17, 16, 14, 9),
+        (17, 16, 14, 6),
+        (17, 16, 14, 4),
+        (17, 16, 14, 1),
+        (17, 16, 13, 12),
+        (17, 16, 13, 5),
+        (17, 16, 13, 2),
+        (17, 16, 12, 10),
+        (17, 16, 12, 8),
+        (17, 16, 12, 4),
+        (17, 16, 12, 1),
+        (17, 16, 11, 7),
+        (17, 16, 11, 1),
+        (17, 16, 10, 9),
+        (17, 16, 10, 8),
+        (17, 16, 10, 5),
+        (17, 16, 9, 5),
+        (17, 16, 9, 4),
+        (17, 16, 8, 6),
+        (17, 16, 8, 3),
+        (17, 16, 5, 4),
+        (17, 16, 5, 3),
+        (17, 16, 3, 2),
+        (17, 15, 14, 12),
+        (17, 15, 14, 10),
+        (17, 15, 14, 9),
+        (17, 15, 14, 8),
+        (17, 15, 14, 6),
+        (17, 15, 14, 5),
+        (17, 15, 13, 11),
+        (17, 15, 13, 7),
+        (17, 15, 13, 5),
+        (17, 15, 12, 9),
+        (17, 15, 12, 2),
+        (17, 15, 11, 10),
+        (17, 15, 11, 8),
+        ),
+    18: (
+        (18, 11),
+        (18, 17, 16, 13),
+        (18, 17, 16, 10),
+        (18, 17, 16, 5),
+        (18, 17, 15, 9),
+        (18, 17, 14, 9),
+        (18, 17, 13, 4),
+        (18, 17, 13, 1),
+        (18, 17, 10, 2),
+        (18, 17, 8, 6),
+        (18, 16, 15, 12),
+        (18, 16, 13, 6),
+        (18, 16, 13, 3),
+        (18, 16, 11, 7),
+        (18, 16, 11, 4),
+        (18, 16, 10, 7),
+        (18, 16, 9, 3),
+        (18, 16, 8, 5),
+        (18, 16, 7, 3),
+        (18, 16, 5, 4),
+        (18, 15, 14, 8),
+        (18, 15, 13, 6),
+        (18, 15, 13, 4),
+        (18, 15, 11, 8),
+        (18, 15, 11, 6),
+        (18, 15, 9, 8),
+        (18, 15, 9, 5),
+        (18, 15, 9, 4),
+        (18, 14, 13, 8),
+        (18, 14, 13, 5),
+        (18, 14, 12, 5),
+        (18, 14, 11, 10),
+        (18, 13, 12, 9),
+        (18, 13, 11, 8),
+        (18, 13, 11, 5),
+        (18, 13, 10, 8),
+        (18, 13, 9, 6),
+        (18, 17, 16, 15, 14, 13),
+        (18, 17, 16, 15, 13, 2),
+        (18, 17, 16, 15, 12, 10),
+        (18, 17, 16, 15, 12, 4),
+        ),
+    19: (
+        (19, 18, 17, 14),
+        (19, 18, 17, 13),
+        (19, 18, 17, 5),
+        (19, 18, 16, 10),
+        (19, 18, 16, 5),
+        (19, 18, 15, 13),
+        (19, 18, 15, 12),
+        (19, 18, 15, 10),
+        (19, 18, 15, 3),
+        (19, 18, 14, 13),
+        (19, 18, 14, 1),
+        (19, 18, 13, 11),
+        (19, 18, 13, 8),
+        (19, 18, 13, 3),
+        (19, 18, 13, 1),
+        (19, 18, 12, 10),
+        (19, 18, 12, 3),
+        (19, 18, 10, 6),
+        (19, 18, 10, 2),
+        (19, 18, 9, 6),
+        (19, 18, 9, 4),
+        (19, 18, 8, 7),
+        (19, 18, 8, 2),
+        (19, 18, 7, 5),
+        (19, 18, 7, 3),
+        (19, 18, 5, 2),
+        (19, 17, 16, 6),
+        (19, 17, 15, 8),
+        (19, 17, 14, 10),
+        (19, 17, 14, 3),
+        (19, 17, 13, 8),
+        (19, 17, 13, 5),
+        (19, 17, 12, 11),
+        (19, 17, 12, 10),
+        (19, 17, 12, 4),
+        (19, 17, 11, 6),
+        (19, 17, 10, 6),
+        (19, 17, 10, 3),
+        (19, 17, 7, 3),
+        (19, 17, 6, 5),
+        (19, 17, 5, 4),
+        ),
+    20: (
+        (20, 17),
+        (20, 19, 16, 14),
+        (20, 19, 16, 2),
+        (20, 19, 15, 11),
+        (20, 19, 15, 10),
+        (20, 19, 15, 4),
+        (20, 19, 14, 9),
+        (20, 19, 14, 4),
+        (20, 19, 12, 8),
+        (20, 19, 11, 7),
+        (20, 19, 9, 8),
+        (20, 19, 9, 2),
+        (20, 19, 8, 4),
+        (20, 19, 7, 6),
+        (20, 19, 4, 3),
+        (20, 18, 15, 14),
+        (20, 18, 13, 10),
+        (20, 18, 13, 7),
+        (20, 18, 11, 10),
+        (20, 18, 11, 8),
+        (20, 18, 11, 5),
+        (20, 18, 9, 3),
+        (20, 17, 16, 9),
+        (20, 17, 15, 14),
+        (20, 17, 15, 11),
+        (20, 17, 15, 9),
+        (20, 17, 14, 8),
+        (20, 17, 14, 3),
+        (20, 17, 13, 4),
+        (20, 17, 12, 10),
+        (20, 17, 11, 9),
+        (20, 17, 9, 8),
+        (20, 17, 9, 7),
+        (20, 17, 9, 4),
+        (20, 17, 6, 4),
+        (20, 16, 15, 11),
+        (20, 16, 15, 5),
+        (20, 16, 13, 9),
+        (20, 16, 13, 5),
+        (20, 16, 12, 7),
+        (20, 16, 10, 9),
+        ),
+    21: (
+        (21, 19),
+        (21, 20, 19, 16),
+        (21, 20, 19, 13),
+        (21, 20, 19, 7),
+        (21, 20, 19, 5),
+        (21, 20, 19, 4),
+        (21, 20, 19, 2),
+        (21, 20, 18, 6),
+        (21, 20, 17, 14),
+        (21, 20, 17, 10),
+        (21, 20, 17, 7),
+        (21, 20, 17, 3),
+        (21, 20, 17, 2),
+        (21, 20, 16, 11),
+        (21, 20, 16, 2),
+        (21, 20, 14, 10),
+        (21, 20, 14, 8),
+        (21, 20, 13, 7),
+        (21, 20, 11, 9),
+        (21, 20, 9, 3),
+        (21, 20, 8, 3),
+        (21, 20, 7, 5),
+        (21, 20, 6, 5),
+        (21, 20, 5, 2),
+        (21, 19, 18, 10),
+        (21, 19, 17, 11),
+        (21, 19, 17, 10),
+        (21, 19, 17, 4),
+        (21, 19, 16, 15),
+        (21, 19, 16, 12),
+        (21, 19, 16, 8),
+        (21, 19, 16, 5),
+        (21, 19, 15, 9),
+        (21, 19, 15, 4),
+        (21, 19, 14, 13),
+        (21, 19, 14, 7),
+        (21, 19, 13, 6),
+        (21, 19, 12, 6),
+        (21, 19, 11, 8),
+        (21, 19, 11, 4),
+        (21, 19, 10, 5),
+        ),
+    22: (
+        (22, 21),
+        (22, 21, 20, 11),
+        (22, 21, 20, 7),
+        (22, 21, 19, 10),
+        (22, 21, 19, 2),
+        (22, 21, 18, 12),
+        (22, 21, 17, 13),
+        (22, 21, 17, 8),
+        (22, 21, 16, 15),
+        (22, 21, 15, 6),
+        (22, 21, 14, 11),
+        (22, 21, 13, 1),
+        (22, 21, 12, 9),
+        (22, 21, 10, 9),
+        (22, 21, 10, 6),
+        (22, 21, 10, 5),
+        (22, 21, 7, 2),
+        (22, 21, 5, 4),
+        (22, 20, 19, 8),
+        (22, 20, 19, 3),
+        (22, 20, 16, 3),
+        (22, 20, 14, 13),
+        (22, 20, 13, 9),
+        (22, 20, 13, 8),
+        (22, 20, 13, 6),
+        (22, 20, 11, 10),
+        (22, 20, 11, 9),
+        (22, 20, 11, 4),
+        (22, 20, 11, 3),
+        (22, 19, 18, 17),
+        (22, 19, 17, 14),
+        (22, 19, 17, 11),
+        (22, 19, 17, 9),
+        (22, 19, 16, 6),
+        (22, 19, 16, 4),
+        (22, 19, 15, 12),
+        (22, 19, 15, 10),
+        (22, 19, 15, 5),
+        (22, 19, 14, 5),
+        (22, 19, 12, 9),
+        (22, 19, 6, 5),
+        ),
+    23: (
+        (23, 18),
+        (23, 14),
+        (23, 22, 21, 16),
+        (23, 22, 21, 8),
+        (23, 22, 21, 2),
+        (23, 22, 21, 1),
+        (23, 22, 20, 18),
+        (23, 22, 20, 16),
+        (23, 22, 20, 4),
+        (23, 22, 20, 3),
+        (23, 22, 19, 18),
+        (23, 22, 19, 8),
+        (23, 22, 19, 3),
+        (23, 22, 18, 16),
+        (23, 22, 18, 11),
+        (23, 22, 18, 8),
+        (23, 22, 18, 5),
+        (23, 22, 18, 4),
+        (23, 22, 17, 10),
+        (23, 22, 17, 6),
+        (23, 22, 16, 15),
+        (23, 22, 16, 8),
+        (23, 22, 16, 6),
+        (23, 22, 15, 14),
+        (23, 22, 15, 1),
+        (23, 22, 14, 12),
+        (23, 22, 14, 10),
+        (23, 22, 14, 7),
+        (23, 22, 13, 6),
+        (23, 22, 12, 10),
+        (23, 22, 12, 8),
+        (23, 22, 12, 4),
+        (23, 22, 11, 10),
+        (23, 22, 10, 5),
+        (23, 22, 8, 7),
+        (23, 22, 8, 4),
+        (23, 22, 6, 5),
+        (23, 22, 5, 4),
+        (23, 22, 4, 2),
+        (23, 21, 20, 18),
+        (23, 21, 20, 17),
+        ),
+    24: (
+        (24, 23, 22, 17),
+        (24, 23, 22, 7),
+        (24, 23, 21, 20),
+        (24, 23, 21, 11),
+        (24, 23, 21, 8),
+        (24, 23, 19, 2),
+        (24, 23, 18, 14),
+        (24, 23, 16, 13),
+        (24, 23, 14, 1),
+        (24, 23, 10, 8),
+        (24, 23, 9, 3),
+        (24, 23, 5, 4),
+        (24, 22, 21, 12),
+        (24, 22, 21, 9),
+        (24, 22, 20, 7),
+        (24, 22, 19, 16),
+        (24, 22, 19, 15),
+        (24, 22, 19, 13),
+        (24, 22, 19, 8),
+        (24, 22, 19, 6),
+        (24, 22, 18, 13),
+        (24, 22, 17, 8),
+        (24, 22, 16, 7),
+        (24, 22, 15, 4),
+        (24, 22, 15, 3),
+        (24, 22, 14, 13),
+        (24, 22, 9, 3),
+        (24, 22, 8, 7),
+        (24, 22, 7, 6),
+        (24, 21, 20, 14),
+        (24, 21, 18, 14),
+        (24, 21, 18, 5),
+        (24, 21, 11, 5),
+        (24, 20, 19, 17),
+        (24, 20, 19, 5),
+        (24, 20, 18, 15),
+        (24, 20, 11, 9),
+        (24, 20, 11, 5),
+        (24, 19, 14, 11),
+        (24, 19, 13, 11),
+        (24, 19, 9, 6),
+        ),
+    25: (
+        (25, 22),
+        (25, 18),
+        (25, 24, 23, 22),
+        (25, 24, 23, 2),
+        (25, 24, 22, 15),
+        (25, 24, 22, 13),
+        (25, 24, 22, 8),
+        (25, 24, 22, 5),
+        (25, 24, 22, 3),
+        (25, 24, 21, 18),
+        (25, 24, 21, 9),
+        (25, 24, 20, 16),
+        (25, 24, 20, 13),
+        (25, 24, 20, 11),
+        (25, 24, 20, 8),
+        (25, 24, 20, 4),
+        (25, 24, 19, 11),
+        (25, 24, 19, 8),
+        (25, 24, 19, 1),
+        (25, 24, 18, 4),
+        (25, 24, 18, 3),
+        (25, 24, 17, 8),
+        (25, 24, 17, 4),
+        (25, 24, 17, 2),
+        (25, 24, 17, 1),
+        (25, 24, 16, 13),
+        (25, 24, 16, 9),
+        (25, 24, 16, 7),
+        (25, 24, 16, 1),
+        (25, 24, 15, 12),
+        (25, 24, 15, 3),
+        (25, 24, 13, 12),
+        (25, 24, 13, 11),
+        (25, 24, 13, 6),
+        (25, 24, 13, 5),
+        (25, 24, 13, 4),
+        (25, 24, 13, 1),
+        (25, 24, 12, 9),
+        (25, 24, 11, 10),
+        (25, 24, 11, 7),
+        (25, 24, 11, 5),
+        ),
+    26: (
+        (26, 25, 24, 20),
+        (26, 25, 24, 8),
+        (26, 25, 24, 7),
+        (26, 25, 22, 17),
+        (26, 25, 22, 14),
+        (26, 25, 22, 3),
+        (26, 25, 22, 2),
+        (26, 25, 21, 1),
+        (26, 25, 20, 15),
+        (26, 25, 19, 18),
+        (26, 25, 19, 3),
+        (26, 25, 18, 13),
+        (26, 25, 18, 2),
+        (26, 25, 17, 9),
+        (26, 25, 17, 7),
+        (26, 25, 16, 5),
+        (26, 25, 15, 13),
+        (26, 25, 14, 3),
+        (26, 25, 13, 3),
+        (26, 25, 13, 2),
+        (26, 25, 12, 11),
+        (26, 25, 12, 7),
+        (26, 25, 11, 9),
+        (26, 25, 11, 7),
+        (26, 25, 10, 8),
+        (26, 25, 10, 6),
+        (26, 25, 9, 4),
+        (26, 25, 8, 6),
+        (26, 25, 7, 3),
+        (26, 24, 23, 20),
+        (26, 24, 23, 10),
+        (26, 24, 22, 7),
+        (26, 24, 21, 5),
+        (26, 24, 20, 17),
+        (26, 24, 20, 9),
+        (26, 24, 19, 17),
+        (26, 24, 18, 5),
+        (26, 24, 17, 9),
+        (26, 24, 17, 7),
+        (26, 24, 17, 5),
+        (26, 24, 16, 13),
+        ),
+    27: (
+        (27, 26, 25, 22),
+        (27, 26, 25, 17),
+        (27, 26, 25, 11),
+        (27, 26, 24, 11),
+        (27, 26, 23, 7),
+        (27, 26, 22, 10),
+        (27, 26, 22, 2),
+        (27, 26, 22, 1),
+        (27, 26, 21, 11),
+        (27, 26, 20, 19),
+        (27, 26, 20, 9),
+        (27, 26, 18, 11),
+        (27, 26, 17, 9),
+        (27, 26, 17, 1),
+        (27, 26, 16, 14),
+        (27, 26, 16, 7),
+        (27, 26, 16, 2),
+        (27, 26, 15, 2),
+        (27, 26, 14, 9),
+        (27, 26, 14, 7),
+        (27, 26, 13, 2),
+        (27, 26, 12, 6),
+        (27, 26, 10, 5),
+        (27, 26, 6, 3),
+        (27, 26, 3, 2),
+        (27, 25, 24, 15),
+        (27, 25, 23, 10),
+        (27, 25, 23, 7),
+        (27, 25, 22, 18),
+        (27, 25, 22, 14),
+        (27, 25, 22, 3),
+        (27, 25, 21, 15),
+        (27, 25, 21, 9),
+        (27, 25, 21, 4),
+        (27, 25, 20, 17),
+        (27, 25, 20, 11),
+        (27, 25, 20, 8),
+        (27, 25, 20, 4),
+        (27, 25, 19, 18),
+        (27, 25, 19, 8),
+        (27, 25, 19, 3),
+        ),
+    28: (
+        (28, 25),
+        (28, 19),
+        (28, 15),
+        (28, 27, 26, 16),
+        (28, 27, 26, 11),
+        (28, 27, 25, 18),
+        (28, 27, 25, 6),
+        (28, 27, 24, 22),
+        (28, 27, 24, 7),
+        (28, 27, 23, 19),
+        (28, 27, 23, 4),
+        (28, 27, 21, 13),
+        (28, 27, 21, 7),
+        (28, 27, 20, 14),
+        (28, 27, 20, 11),
+        (28, 27, 17, 1),
+        (28, 27, 16, 5),
+        (28, 27, 16, 3),
+        (28, 27, 15, 7),
+        (28, 27, 15, 3),
+        (28, 27, 14, 5),
+        (28, 27, 13, 8),
+        (28, 27, 13, 4),
+        (28, 27, 8, 7),
+        (28, 27, 5, 4),
+        (28, 26, 23, 15),
+        (28, 26, 23, 13),
+        (28, 26, 23, 9),
+        (28, 26, 21, 14),
+        (28, 26, 21, 5),
+        (28, 26, 20, 13),
+        (28, 26, 20, 7),
+        (28, 26, 19, 6),
+        (28, 26, 15, 11),
+        (28, 26, 10, 5),
+        (28, 26, 10, 3),
+        (28, 26, 6, 5),
+        (28, 25, 24, 11),
+        (28, 25, 24, 9),
+        (28, 25, 23, 18),
+        (28, 25, 22, 12),
+        ),
+    29: (
+        (29, 27),
+        (29, 28, 27, 25),
+        (29, 28, 27, 20),
+        (29, 28, 27, 8),
+        (29, 28, 27, 4),
+        (29, 28, 26, 10),
+        (29, 28, 25, 6),
+        (29, 28, 24, 19),
+        (29, 28, 24, 2),
+        (29, 28, 23, 22),
+        (29, 28, 23, 19),
+        (29, 28, 23, 15),
+        (29, 28, 21, 11),
+        (29, 28, 20, 10),
+        (29, 28, 20, 7),
+        (29, 28, 19, 15),
+        (29, 28, 17, 10),
+        (29, 28, 17, 3),
+        (29, 28, 15, 8),
+        (29, 28, 15, 5),
+        (29, 28, 14, 4),
+        (29, 28, 13, 6),
+        (29, 28, 12, 10),
+        (29, 28, 11, 4),
+        (29, 28, 10, 2),
+        (29, 28, 8, 6),
+        (29, 27, 26, 25),
+        (29, 27, 26, 22),
+        (29, 27, 26, 19),
+        (29, 27, 26, 17),
+        (29, 27, 26, 15),
+        (29, 27, 26, 11),
+        (29, 27, 25, 20),
+        (29, 27, 25, 14),
+        (29, 27, 25, 13),
+        (29, 27, 25, 7),
+        (29, 27, 24, 15),
+        (29, 27, 24, 11),
+        (29, 27, 24, 9),
+        (29, 27, 24, 8),
+        (29, 27, 24, 3),
+        ),
+    30: (
+        (30, 29, 28, 7),
+        (30, 29, 26, 24),
+        (30, 29, 26, 22),
+        (30, 29, 26, 4),
+        (30, 29, 24, 17),
+        (30, 29, 24, 12),
+        (30, 29, 23, 20),
+        (30, 29, 23, 18),
+        (30, 29, 23, 13),
+        (30, 29, 23, 8),
+        (30, 29, 22, 7),
+        (30, 29, 19, 17),
+        (30, 29, 19, 10),
+        (30, 29, 19, 8),
+        (30, 29, 18, 9),
+        (30, 29, 18, 3),
+        (30, 29, 17, 7),
+        (30, 29, 17, 5),
+        (30, 29, 16, 4),
+        (30, 29, 15, 14),
+        (30, 29, 14, 2),
+        (30, 29, 12, 3),
+        (30, 29, 10, 4),
+        (30, 29, 9, 6),
+        (30, 29, 8, 5),
+        (30, 28, 27, 6),
+        (30, 28, 26, 7),
+        (30, 28, 23, 17),
+        (30, 28, 23, 11),
+        (30, 28, 23, 10),
+        (30, 28, 23, 4),
+        (30, 28, 22, 17),
+        (30, 28, 21, 12),
+        (30, 28, 21, 7),
+        (30, 28, 20, 19),
+        (30, 28, 20, 17),
+        (30, 28, 19, 7),
+        (30, 28, 18, 7),
+        (30, 28, 16, 9),
+        (30, 28, 15, 12),
+        (30, 28, 14, 5),
+        ),
+    31: (
+        (31, 28),
+        (31, 25),
+        (31, 24),
+        (31, 18),
+        (31, 30, 29, 28),
+        (31, 30, 29, 25),
+        (31, 30, 29, 20),
+        (31, 30, 29, 19),
+        (31, 30, 29, 5),
+        (31, 30, 28, 24),
+        (31, 30, 28, 22),
+        (31, 30, 28, 18),
+        (31, 30, 28, 16),
+        (31, 30, 28, 13),
+        (31, 30, 28, 10),
+        (31, 30, 28, 8),
+        (31, 30, 28, 3),
+        (31, 30, 27, 16),
+        (31, 30, 26, 22),
+        (31, 30, 26, 8),
+        (31, 30, 25, 16),
+        (31, 30, 25, 9),
+        (31, 30, 25, 7),
+        (31, 30, 25, 5),
+        (31, 30, 24, 19),
+        (31, 30, 24, 16),
+        (31, 30, 24, 12),
+        (31, 30, 23, 20),
+        (31, 30, 23, 19),
+        (31, 30, 23, 5),
+        (31, 30, 22, 21),
+        (31, 30, 22, 20),
+        (31, 30, 22, 12),
+        (31, 30, 22, 4),
+        (31, 30, 21, 18),
+        (31, 30, 21, 10),
+        (31, 30, 20, 11),
+        (31, 30, 20, 8),
+        (31, 30, 20, 7),
+        (31, 30, 20, 1),
+        (31, 30, 19, 17),
+        ),
+    32: (
+        (32, 31, 30, 10),
+        (32, 31, 29, 1),
+        (32, 31, 26, 18),
+        (32, 31, 26, 9),
+        (32, 31, 26, 7),
+        (32, 31, 23, 10),
+        (32, 31, 22, 17),
+        (32, 31, 21, 16),
+        (32, 31, 21, 5),
+        (32, 31, 18, 10),
+        (32, 31, 16, 2),
+        (32, 31, 15, 10),
+        (32, 31, 14, 4),
+        (32, 31, 13, 8),
+        (32, 31, 9, 7),
+        (32, 31, 5, 4),
+        (32, 30, 29, 23),
+        (32, 30, 29, 20),
+        (32, 30, 29, 16),
+        (32, 30, 29, 15),
+        (32, 30, 27, 24),
+        (32, 30, 27, 21),
+        (32, 30, 27, 12),
+        (32, 30, 27, 8),
+        (32, 30, 26, 25),
+        (32, 30, 26, 13),
+        (32, 30, 25, 16),
+        (32, 30, 23, 16),
+        (32, 30, 23, 14),
+        (32, 30, 23, 4),
+        (32, 30, 21, 14),
+        (32, 30, 19, 8),
+        (32, 30, 19, 4),
+        (32, 30, 17, 3),
+        (32, 30, 15, 6),
+        (32, 30, 11, 8),
+        (32, 30, 11, 5),
+        (32, 30, 8, 3),
+        (32, 30, 7, 4),
+        (32, 29, 28, 19),
+        (32, 29, 27, 23),
+        ),
+    }
 
 if __name__ == '__main__':
     pass
```

### Comparing `zignal-0.6.0/zignal/measure/mls.py` & `zignal-0.7.0/zignal/measure/mls.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 Created on 22 Mar 2014
 
 @author: Ronny Andersson (ronny@andersson.tk)
 @copyright: (c) 2014 Ronny Andersson
 @license: MIT
 """
 
-# standard library
-from collections import deque
+# Standard library
 import logging
 import random
+from collections import deque
 
-# external libraries
+# Third party
 import numpy as np
 import scipy.signal
 
-# local libraries
+# Internal
 from zignal import Audio
 from zignal.filters.biquads import RBJ
 from zignal.filters.linearfilter import Filter
 
 # expose the measure.mlstaps.TAPS dictionary in the measure.mls namespace
-from .mlstaps import *
+from .mlstaps import TAPS  # isort:skip
 
 __all__ = [
-           'MLS',
-           'MLS_simple',
-           'get_random_taps',
-           'TAPS',
-           ]
+    'MLS',
+    'MLS_simple',
+    'get_random_taps',
+    'TAPS',
+    ]
+
 
 def get_random_taps(N):
     '''Select a random set of taps for given order N'''
     return random.choice(TAPS.get(N))
 
+
 class _MLS_base(object):
     '''Base class for Maximum Length Sequence (MLS) generation. This class
     implements the "tricky" bits when it comes to MLS sequences. An efficient
     generator is needed since MLS is based on shift registers where we are
     dealing with bits.
 
     It should not be needed to create an instance of this class directly. Use
@@ -56,37 +58,37 @@
 
     This class implements:
     * Generators
     * Circular Cross Correlation
     * Extraction of the impulse response
     '''
     def __init__(self, N=None, taps=None):
-        assert N    is not None, "Please specify MLS order"
+        assert N is not None, "Please specify MLS order"
         assert taps is not None, "Please specify feedback taps"
         assert isinstance(taps, (tuple, list))
         assert len(taps) != 0, "taps are empty!"
 
         self._logger    = logging.getLogger(__name__)
         self.N          = N
         self.L          = (2**N)-1
         self.taps       = taps
 
         sizeof_int = np.int64().dtype.itemsize
-        self._RAM_usage = (self.L*sizeof_int)/(1024**2) # in Mb
+        self._RAM_usage = (self.L*sizeof_int)/(1024**2)     # in Mb
 
     def __repr__(self):
-        return '_MLS_base(N=%i, taps=%s)' %(self.N, tuple(self.taps))
+        return '_MLS_base(N=%i, taps=%s)' % (self.N, tuple(self.taps))
 
     def __str__(self):
         s  = '=======================================\n'
-        s += 'classname        : %s\n'      %self.__class__.__name__
-        s += 'N                : %i\n'      %self.N
-        s += 'L=(2^N)-1        : %i\n'      %self.L
-        s += 'taps             : %s\n'      %str(self.taps)
-        s += "RAM              : %.1f [Mb] (one full sequence)\n" %self._RAM_usage
+        s += 'classname        : %s\n'      % self.__class__.__name__
+        s += 'N                : %i\n'      % self.N
+        s += 'L=(2^N)-1        : %i\n'      % self.L
+        s += 'taps             : %s\n'      % str(self.taps)
+        s += "RAM              : %.1f [Mb] (one full sequence)\n" % self._RAM_usage
         s += '-----------------:---------------------\n'
         return s
 
     def generator_bit(self):
         """Generate one bit at a time. This generator never finishes, it will
         generate bits forever. However, the sequence will repeat itself after
         (2^N)-1 steps.
@@ -156,16 +158,16 @@
         repeat=2. More repetitions will mean longer signal but better signal
         to noise ratio since we will average away any noise.
         """
 
         chunkgen        = self.generator_samples(chunk=self.L)
         full_sequence   = next(chunkgen)
         reps_sequence   = np.tile(full_sequence.T, repeats).T
-        self._logger.debug("May share memory: %s" %np.may_share_memory(full_sequence,
-                                                                       reps_sequence))
+        self._logger.debug("May share memory: %s" % np.may_share_memory(full_sequence,
+                                                                        reps_sequence))
         return reps_sequence
 
     def xcorr_circular(self, other):
         """Circular cross correlation. The difference between circular cross
         correlation and regular correlation is that with circular correlation
         we assume that the signal is repeating.
 
@@ -206,39 +208,54 @@
 
         # Correlation and convolution are related. Correlation in the time domain is *very*
         # slow for long sequences. Convolution in the frequecy domain is much faster. We can
         # use the convolution method if we "undo" the flip of the input signal. This is
         # equivalent to the correlation method. There might be some small (insignificant)
         # rounding errors but for a large array this should not be noticable.
         #
-        ### Flip comments to verify that correlation and convolution (with input flip) is
-        ### the same. Be careful, long sequences are slow to calculate using the
-        ### correlation method.
+        # ** Flip comments to verify that correlation and convolution (with input flip) is
+        # ** the same. Be careful, long sequences are slow to calculate using the
+        # ** correlation method.
         #xcorr   = scipy.signal.correlate(ref, other)
         xcorr = scipy.signal.fftconvolve(np.flipud(ref), other)
 
-        self._logger.debug("ref: %s" %np.array_str(ref.T,     max_line_width=200, precision=4, suppress_small=True))
-        self._logger.debug("xc : %s" %np.array_str(xcorr.T,   max_line_width=200, precision=4, suppress_small=True))
+        self._logger.debug("ref: %s" % np.array_str(
+            ref.T,      max_line_width=200, precision=4, suppress_small=True))
+        self._logger.debug("xc : %s" % np.array_str(
+            xcorr.T,    max_line_width=200, precision=4, suppress_small=True))
 
         del ref
 
         # slicing creates views which are cheap (points to the same array)
         x1 = xcorr[self.L:]         # right half (end)
         x2 = xcorr[:self.L-1]       # left halt (start)
-        self._logger.debug("x1 : %s" %np.array_str(x1.T,      max_line_width=200, precision=4, suppress_small=True))
-        self._logger.debug("x2 : %s" %np.array_str(x2.T,      max_line_width=200, precision=4, suppress_small=True))
 
-        x1[:]=x1+x2                 # assume circular sequence
-        self._logger.debug("xc : %s" %np.array_str(xcorr.T,   max_line_width=200, precision=4, suppress_small=True))
+        self._logger.debug("x1 : %s" % np.array_str(
+            x1.T,       max_line_width=200, precision=4, suppress_small=True))
+
+        self._logger.debug("x2 : %s" % np.array_str(
+            x2.T,       max_line_width=200, precision=4, suppress_small=True))
+
+        # assume circular sequence
+        x1[:] = x1+x2
+
+        self._logger.debug("xc : %s" % np.array_str(
+            xcorr.T,    max_line_width=200, precision=4, suppress_small=True))
 
-        norm = xcorr[self.L-1:]     # extract "impulse" + tail (right half)
-        self._logger.debug("nrm: %s" %np.array_str(norm.T,    max_line_width=200, precision=4, suppress_small=True))
+        # extract "impulse" + tail (right half)
+        norm = xcorr[self.L-1:]
 
-        norm[:] = norm/self.L       # normalise so that max <= 1.0
-        self._logger.debug("nrm: %s" %np.array_str(norm.T,    max_line_width=200, precision=4, suppress_small=True))
+        self._logger.debug("nrm: %s" % np.array_str(
+            norm.T,     max_line_width=200, precision=4, suppress_small=True))
+
+        # normalise so that max <= 1.0
+        norm[:] = norm/self.L
+
+        self._logger.debug("nrm: %s" % np.array_str(
+            norm.T,     max_line_width=200, precision=4, suppress_small=True))
 
         return norm
 
     def trim_and_avgerage(self, other):
         """It is assumed that at least two full MLSes are used and sent through the
         system we want to measure. By using m repeated sequences of MLSes we can throw
         away the first full sequence. This first part might be delayed because of
@@ -261,38 +278,38 @@
         #          [B_3],
         #          [C_1],
         #          [C_2],
         #          [C_3]]
 
         # throw away first full sequence
         trimmed = other[self.L:]
-        self._logger.debug("May share memory: %s" %np.may_share_memory(other, trimmed))
+        self._logger.debug("May share memory: %s" % np.may_share_memory(other, trimmed))
         #print(repr(trimmed))
         # data is [[B_1],
         #          [B_2],
         #          [B_3],
         #          [C_1],
         #          [C_2],
         #          [C_3]]
 
         repeats = len(trimmed)//self.L
-        self._logger.debug("repeats (first discared): %i" %repeats)
+        self._logger.debug("repeats (first discared): %i" % repeats)
 
         # reshape so we can average
         reshaped = trimmed.reshape((repeats, self.L))
         # data is [[B_1, B_2, B_3],
         #          [C_1, C_2, C_3]]
 
-        self._logger.debug("May share memory: %s" %np.may_share_memory(other, reshaped))
+        self._logger.debug("May share memory: %s" % np.may_share_memory(other, reshaped))
         #print(repr(reshaped))
 
         # the averaging finally creates a new array that has it's own data
         average = np.average(reshaped, axis=0)
 
-        average = np.expand_dims(average, axis=1) # up the ndim to 2
+        average = np.expand_dims(average, axis=1)   # up the ndim to 2
         # data is [[X_1],
         #          [X_2],
         #          [X_3]]
 
         return average
 
     def get_impulse(self, x):
@@ -306,14 +323,15 @@
         assert len(x) > self.L, "The first sequence will be thrown away"
 
         avg     = self.trim_and_avgerage(x)
         impulse = self.xcorr_circular(avg)
 
         return impulse
 
+
 class MLS(_MLS_base, Audio):
     """This class is a mixture of the MLS base class and the Audio class. The MLS data
     is the audio samples in the Audio class. Because we also know about sample rate
     here we can apply emphasis and de-emphasis on the samples. When plotting the FFT
     of the impulse response remember to use a rectangular window. This is perfectly
     valid since the MLS is cyclic by nature and will wrap around.
 
@@ -341,39 +359,39 @@
 
         _MLS_base.__init__(self, N=N, taps=taps)
         Audio.__init__(self, fs=fs, initialdata=self.get_full_sequence(repeats=repeats))
 
         self.repeats            = repeats
         self._length_impresp    = self.L/self.fs
         self._filter_emphasis   = Filter(B=B, A=A, fs=self.fs)
-        self._filter_deemphasis = Filter(B=A, A=B, fs=self.fs) # inverse filter
+        self._filter_deemphasis = Filter(B=A, A=B, fs=self.fs)  # inverse filter
 
         assert self._filter_emphasis.is_minimum_phase(), \
             "The emphasis filter must be minimum phase, i.e. possible to invert"
 
     def __repr__(self):
         B, A = self._filter_emphasis.get_coefficients()
 
         s = 'MLS(N=%i, taps=%s, fs=%r, repeats=%i, B=%s, A=%s)' \
-            %(self.N, tuple(self.taps), self.fs, self.repeats, tuple(B), tuple(A))
+            % (self.N, tuple(self.taps), self.fs, self.repeats, tuple(B), tuple(A))
 
         return s
 
     def __str__(self):
         B, A = self._filter_emphasis.get_coefficients()
 
         mls_string = _MLS_base.__str__(self)
         mls_string = "\n".join(mls_string.splitlines()[2:-1])
 
         s  = Audio.__str__(self)
-        s += '%s\n'                             %mls_string
-        s += 'repeats          : %i\n'          %self.repeats
-        s += 'len(impulse)     : %.3f [s]\n'    %self._length_impresp
-        s += 'emphasis filt. B : %s\n'          %str(B)
-        s += 'emphasis filt. A : %s\n'          %str(A)
+        s += '%s\n'                             % mls_string
+        s += 'repeats          : %i\n'          % self.repeats
+        s += 'len(impulse)     : %.3f [s]\n'    % self._length_impresp
+        s += 'emphasis filt. B : %s\n'          % str(B)
+        s += 'emphasis filt. A : %s\n'          % str(A)
         return s
 
     def apply_emphasis(self):
         """Apply emphasis by filtering the whole audio signal. If high freqencies are
         boosted noise will be suppressed. If low frequencies are boosted we will get
         better signal to noise ratio in the lower area of the frequency response.
         """
@@ -391,14 +409,15 @@
     def get_impulse(self, x):
         """Extract the impulse response. Returns an Audio instance.
         """
         imp = _MLS_base.get_impulse(self, x)
         y   = Audio(fs=self.fs, initialdata=imp)
         return y
 
+
 class MLS_simple(object):
     def __init__(self, N=16, fs=96000, repeats=3):
         """Simplified usage for quick access to an MLS that performs the required
         message calls in the right order. Can also be used as an example on how
         to use the MLS class.
 
         Example:
@@ -416,24 +435,24 @@
         self._mls = MLS(N=N, taps=TAPS[N][0], fs=fs, repeats=repeats, B=B, A=A)
         self._mls.apply_emphasis()
 
         # map the name to the internal representation of the samples
         self.samples = self._mls.samples
 
     def __repr__(self):
-        s = 'MLS_simple(N=%i fs=%r, repeats=%i)' %(self._mls.N, self._mls.fs, self._mls.repeats)
+        s = 'MLS_simple(N=%i fs=%r, repeats=%i)' % (self._mls.N, self._mls.fs, self._mls.repeats)
         return s
 
     def __str__(self):
         mls_string = str(self._mls)
         mls_string = "\n".join(mls_string.splitlines()[2:])
 
         s  = '=======================================\n'
-        s += 'classname        : %s\n'      %self.__class__.__name__
-        s += '%s' %str(mls_string)
+        s += 'classname        : %s\n'      % self.__class__.__name__
+        s += '%s' % str(mls_string)
         return s
 
     def get_impulse(self, x):
         """Extract the impulse response"""
         tmp = self._mls.apply_deemphasis(x)
         self._impulseresponse = self._mls.get_impulse(tmp)
         return self._impulseresponse
@@ -442,30 +461,37 @@
         """Plot the magnitude response. Phase is not included in this plot."""
         assert hasattr(self, "_impulseresponse"), "call get_impulse(...) before trying to plot"
 
         # A window function on the impulse response does not work here, since
         # that would scale the impulse wrong.
         self._impulseresponse.plot_fft(plotname=plotname, window='rectangular', normalise=False)
 
+
 if __name__ == '__main__':
-    logging.basicConfig(format='%(levelname)-7s: %(module)s.%(funcName)-15s %(message)s',
-                        level='DEBUG')
+    logging.basicConfig(
+        format="%(levelname)-8s: %(module)s.%(funcName)-15s %(message)s",
+        level="DEBUG",
+        )
+    # some libraries are noisy in DEBUG
+    logging.getLogger("matplotlib").setLevel(logging.INFO)
+    logging.getLogger("PIL").setLevel(logging.WARNING)
+
     fs  = 48000*2
     N   = 13
 
     #mls = _MLS_base(N=N, taps=TAPS[N][0])
     #mls = MLS(N=N, taps=TAPS[N][0], fs=fs)
 
     f = RBJ(filtertype="highshelf", gaindb=-10, f0=100, Q=0.707, fs=fs)
     B, A = f.get_coefficients()
     #mls = MLS(N=N, taps=TAPS[N][0], fs=fs, repeats=5, B=B, A=A)
 
     mls = MLS_simple(N=N, fs=fs, repeats=4)
 
-    print (repr(mls))
+    print(repr(mls))
     print(mls)
 
     y = mls.get_impulse(mls.samples)
     #mls.plot_fft()                                      # used with MLS_simple
     y.plot_fft(window='rectangular', normalise=False)   # used with MLS
 
     print('++ End of script ++')
```

### Comparing `zignal-0.6.0/zignal/audio.py` & `zignal-0.7.0/zignal/audio.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 Created on Dec 31, 2013
 
 @author: Ronny Andersson (ronny@andersson.tk)
 @copyright: (c) 2013 Ronny Andersson
 @license: MIT
 '''
 
-# standard library
+# Standard library
 import logging
 import os
 
-# external libraries
+# Third party
 import matplotlib.pyplot as plt
 import numpy as np
-import samplerate
-import scipy.signal
 import scipy.io.wavfile
+import scipy.signal
 
-#===================================================================================================
-# Classes
-#===================================================================================================
 
+# ==================================================================================================
+# Classes
+# ==================================================================================================
 class Audio(object):
     def __init__(self, channels=0, fs=96000, nofsamples=0, duration=None,
                  initialdata=None, dtype=np.float64):
         """Base class for audio processing. Samples are stored as a numpy array.
 
         We can create an instance by specifying a channel count and one of either
         a duration or a sample count parameter. The other way of creating an
@@ -45,15 +44,16 @@
         self.ch         = None  # number of channels
         self._comment   = ''
 
         if initialdata is None:
             # if we are not given any initial samples we create an empty array of
             # zeros for the audio samples.
             assert isinstance(channels, int)
-            assert not(nofsamples!=0 and duration is not None), "choose either samples or duration"
+            assert not (nofsamples != 0 and duration is not None), \
+                "choose either samples or duration"
 
             self.ch = channels
 
             if duration is not None:
                 self.nofsamples = int(duration*self.fs)
                 self.duration   = duration
             else:
@@ -65,17 +65,20 @@
 
         else:
             # An array of initial samples are given, use this to extract
             # channel count and durations.
             assert isinstance(initialdata, np.ndarray), \
                 'Only numpy arrays are allowed as initial data'
 
-            assert channels == 0, "parameter 'channels' is redundant if initial data is specified"
-            assert nofsamples == 0, "parameter 'nofsamples' is redundant if initial data is specified"
-            assert duration is None, "parameter 'duration' is redundant if initial data is specified"
+            assert channels == 0, \
+                "parameter 'channels' is redundant if initial data is specified"
+            assert nofsamples == 0, \
+                "parameter 'nofsamples' is redundant if initial data is specified"
+            assert duration is None, \
+                "parameter 'duration' is redundant if initial data is specified"
 
             # copy the data to avoid unexpected data corruption
             self.samples = initialdata.copy()
 
             if self.samples.ndim == 1:
                 # if the array is
                 #     array([ 1.,  1.,  1.])
@@ -92,35 +95,36 @@
 
             # initial data is assumed to have more samples than channels
             assert self.nofsamples > self.ch, 'shape must be (Nsamples, Nchannels)'
 
             self._set_duration()
 
         assert self.nofsamples is not None
-        assert self.duration   is not None
-        assert self.ch         is not None
+        assert self.duration is not None
+        assert self.ch is not None
 
     def __str__(self):
         s  = '=======================================\n'
-        s += 'classname        : %s\n'          %self.__class__.__name__
-        s += 'sample rate      : %.1f [Hz]\n'   %self.fs
-        s += 'channels         : %i\n'          %self.ch
-        s += 'duration         : %.3f [s]\n'    %self.duration
-        s += 'datatype         : %s\n'          %self.samples.dtype
-        s += 'samples per ch   : %i\n'          %self.nofsamples
-        s += 'data size        : %.3f [Mb]\n'   %(self.samples.nbytes/(1024*1024))
-        s += 'has comment      : %s\n'          %('yes' if len(self._comment)!=0 else 'no')
+        s += 'classname        : %s\n'          % self.__class__.__name__
+        s += 'sample rate      : %.1f [Hz]\n'   % self.fs
+        s += 'channels         : %i\n'          % self.ch
+        s += 'duration         : %.3f [s]\n'    % self.duration
+        s += 'datatype         : %s\n'          % self.samples.dtype
+        s += 'samples per ch   : %i\n'          % self.nofsamples
+        s += 'data size        : %.3f [Mb]\n'   % (self.samples.nbytes/(1024*1024))
+        s += 'bitrate          : %.2f [kbit/s]\n' % self.bitrate
+        s += 'has comment      : %s\n'          % ('yes' if len(self._comment) != 0 else 'no')
         if self.ch != 0:
             # += '-----------------:---------------------\n'
-            s += 'peak             : %s\n'  %np.array_str(self.peak()[0],
-                                                          precision=4, suppress_small=True)
-            s += 'RMS              : %s\n'  %np.array_str(self.rms(),
-                                                          precision=4, suppress_small=True)
-            s += 'crestfactor      : %s\n'  %np.array_str(self.crest_factor(),
-                                                          precision=4, suppress_small=True)
+            s += 'peak             : %s\n'  % np.array_str(self.peak()[0],
+                                                           precision=4, suppress_small=True)
+            s += 'RMS              : %s\n'  % np.array_str(self.rms(),
+                                                           precision=4, suppress_small=True)
+            s += 'crestfactor      : %s\n'  % np.array_str(self.crest_factor(),
+                                                           precision=4, suppress_small=True)
         s += '-----------------:---------------------\n'
         return s
 
     def __len__(self):
         return self.nofsamples
 
     def _set_duration(self):
@@ -138,81 +142,138 @@
 
         idx is always zero indexed since it refers to the numpy array. Channels
         are always indexed from one since this is the natural way of identifying
         channel numbers.
         """
         assert isinstance(samples, np.ndarray)
         assert len(samples) == self.nofsamples
-        self.samples[:,idx] = samples
+        self.samples[:, idx] = samples
+
+    @property
+    def bitrate(self):
+        """Calculate the overall bitrate, in kbit/s"""
+        bitrate = (self.fs * self.ch * self.samples.itemsize*8)/1000
+        return bitrate
 
     def copy(self):
         """deep:ish copy"""
         return Audio(fs=self.fs, initialdata=self.samples)
 
     def pretty_string_samples(self, idx_start=0, idx_end=20, precision=4, header=False):
         s = ''
         if header:
             t = '  '
             u = 'ch'
             for i in range(self.ch):
                 t += '-------:'
-                u += '  %2i   :' %(i+1)
+                u += '  %2i   :' % (i+1)
             t += '\n'
             u += '\n'
 
-            s += t  #   -------:-------:-------:
-            s += u  # ch   1   :   2   :   3   :
-            s += t  #   -------:-------:-------:
+            s += t  # -->   -------:-------:-------:
+            s += u  # --> ch   1   :   2   :   3   :
+            s += t  # -->   -------:-------:-------:
 
-        s += np.array_str(self.samples[idx_start:idx_end,:],
+        s += np.array_str(self.samples[idx_start:idx_end, :],
                           max_line_width=260,   # we can print 32 channels before linewrap
                           precision=precision,
                           suppress_small=True)
         if (idx_end-idx_start) < self.nofsamples:
-            s  = s[:-1] # strip the right ']' character
+            s  = s[:-1]     # strip the right ']' character
             s += '\n ...,\n'
-            lastlines = np.array_str(self.samples[-3:,:],
+            lastlines = np.array_str(self.samples[-3:, :],
                                      max_line_width=260,
                                      precision=precision,
                                      suppress_small=True)
-            s += ' %s\n' %lastlines[1:] # strip first '['
+            s += ' %s\n' % lastlines[1:]    # strip first '['
         return s
 
     def pad(self, nofsamples=0):
         """Zero pad *at the end* of the current audio data.
 
         increases duration by samples/fs
         """
         assert nofsamples >= 0, "Can't append negative number of samples"
         zeros = np.zeros((nofsamples, self.ch), dtype=self.samples.dtype)
         self.samples = np.append(self.samples, zeros, axis=0)
 
-        self.nofsamples=len(self.samples)
+        self.nofsamples = len(self.samples)
         self._set_duration()
 
+    def iter_chunks(self, chunksize=1024):
+        """
+        Splits the audio samples into chunks, to iterate over in block-based
+        processing. There are no restrictions on the chunk size, but in
+        practical implementations it is usually a power of two. This is not
+        a requirement here.
+
+        Chunks are sometimes called blocks, this is the same. So chunksize is
+        the same as blocksize.
+        """
+
+        chunks  = len(self.samples) // chunksize
+        missing = len(self.samples) % chunksize
+        self._logger.debug("chunksize        : %i", chunksize)
+        self._logger.debug("data shape       : %s", self.samples.shape)
+        self._logger.debug("chunks pre pad   : %i", chunks)
+        self._logger.debug("missing (modulo) : %i", missing)
+
+        # If the data doesn't add up to a full chunk we need to pad with zeros but
+        # first we need to calculate how many samples are missing for a full chunk.
+        if missing:
+            missing_samples = chunksize - missing
+            self._logger.debug("missing (samples): %s", missing_samples)
+
+            # Pad with zeros, assuming that all channels are equally long in the
+            # first place. A new array is created since the original data should
+            # be kept unchanged. This means that this iterator is not very memory
+            # efficient. This can be avoided if the data is padded to add up to
+            # a multiple of the chunksize before this method is called. If this is
+            # acceptable (changing the original data) then this iterator is very
+            # memory efficient since only a new view of the original data is
+            # created (if possible, not guaranteed)
+            padded = np.concatenate([self.samples, np.zeros((missing_samples, self.ch))])
+            self._logger.debug("padded shape     : %s", padded.shape)
+
+        else:
+            # Here the audio samples adds up to a multiple of the chunksize
+            self._logger.debug("*** No padding is needed")
+            padded = self.samples
+
+        padded_chunks = len(padded) // chunksize
+
+        self._logger.info("chunks (total)   : %i", padded_chunks)
+
+        reshape = padded.reshape((padded_chunks, chunksize, self.ch))
+
+        # Now finally iterate over all the chunks
+        for i in range(padded_chunks):
+            curr_start  = chunksize*i
+            curr_stop   = curr_start + chunksize - 1
+            self._logger.debug("current slice    : %10i %10i", curr_start, curr_stop)
+            yield reshape[i]
+
     def is_empty(self):
         """Check if all samples in all channels are zero, then file is empty."""
         return np.all(self.samples == 0)
 
     def is_probably_empty(self, limit=-80):
         """Check if the absolute peak is below <limit> dB"""
         peak, idx = self.peak()
         peak = np.abs(peak)
         self._logger.debug("abs(peak) is %s dB at %s sec",
-                          np.array_str(lin2db(peak),
-                                       precision=4, suppress_small=True),
-                          np.array_str(idx/self.fs,
-                                       precision=3, suppress_small=True),
-                          )
+                           np.array_str(lin2db(peak), precision=4, suppress_small=True),
+                           np.array_str(idx/self.fs, precision=3, suppress_small=True),
+                           )
         return np.all(peak <= db2lin(limit))
 
     def trim(self, start=None, end=None):
         """Trim samples **IN PLACE** """
         self.samples = self.samples[start:end]
-        self.nofsamples=len(self.samples)
+        self.nofsamples = len(self.samples)
         self._set_duration()
 
     def trim_sec(self, start=None, end=None):
         """Trim (in seconds) **IN PLACE** """
         self.trim(int(start*self.fs), int(end*self.fs))
 
     def _fade(self, millisec, direction):
@@ -226,15 +287,15 @@
         assert millisec >= 0, "Got a time machine?"
         assert direction in ("in", "out")
 
         fade_seconds = millisec/1000
         assert self.duration > fade_seconds, "fade cannot be longer than the length of the audio"
 
         sample_count = int(np.ceil(fade_seconds*self.fs))
-        self._logger.debug("fade %s sample count: %i" %(direction, sample_count))
+        self._logger.debug("fade %s sample count: %i" % (direction, sample_count))
 
         # generate the ramp
         if direction == "out":
             # ramp down
             ramp = np.linspace(1, 0, num=sample_count, endpoint=True)
         else:
             # ramp up
@@ -248,15 +309,15 @@
         else:
             gains = np.append(ramp, ones, axis=0)
 
         # expand the dimension so we get a one channels array of samples,
         # as in (samples, channels)
         gains = np.expand_dims(gains, axis=1)
 
-        assert len(gains) ==  len(self)
+        assert len(gains) == len(self)
 
         # repeat the gain vector so we get as many gain channels as all the channels
         gains = np.repeat(gains, self.ch, axis=1)
 
         assert gains.shape == self.samples.shape
 
         # apply gains
@@ -268,26 +329,26 @@
 
     def fade_out(self, millisec=30):
         """Fade out over 'millisec' seconds. Applies on *all* channels"""
         self._fade(millisec, "out")
 
     def delay(self, n, channel=1):
         """Delay channel x by n samples"""
-        self.samples[:,channel-1] = np.pad(self.samples[:,channel-1], (n, 0),
-                                           mode="constant")[:-n]
+        self.samples[:, channel-1] = \
+            np.pad(self.samples[:, channel-1], (n, 0), mode="constant")[:-n]
 
     def get_time(self):
         """Return a vector of time values, starting with t0=0. Useful when plotting."""
         return np.linspace(0, self.duration, num=self.nofsamples, endpoint=False)
 
     def get_channel(self, channel):
         assert channel != 0, "channel count starts at 1"
         assert channel <= self.ch, \
             "channel %i does not exist, %i channels available" % (channel, self.ch)
-        return Audio(fs=self.fs, initialdata=self.samples[:,channel-1])
+        return Audio(fs=self.fs, initialdata=self.samples[:, channel-1])
 
     def comment(self, comment=None):
         """Modify or return a string comment."""
         assert isinstance(comment, (str, type(None))), "A comment is a string"
 
         if comment is not None:
             self._comment = comment
@@ -323,24 +384,27 @@
 
         does zeropadding
         increases channel count
         """
         for i, other in enumerate(args):
             assert isinstance(other, Audio), "only Audio() instances can be used"
 
-            self._logger.debug("** iteration %02i --> appending %s" %((i+1), other.__class__.__name__))
-            assert self.fs == other.fs, "Sample rates must match (%s != %s)" %(self.fs, other.fs)
+            self._logger.debug(
+                "** iteration %02i --> appending %s" % ((i+1), other.__class__.__name__))
+
+            assert self.fs == other.fs, "Sample rates must match (%s != %s)" % (self.fs, other.fs)
             assert self.samples.dtype == other.samples.dtype, \
-                "Data types must match (%s != %s)"%(self.samples.dtype, other.samples.dtype)
+                "Data types must match (%s != %s)" % (self.samples.dtype, other.samples.dtype)
 
             max_nofsamples = max(self.nofsamples,  other.nofsamples)
             missingsamples = abs(self.nofsamples - other.nofsamples)
 
-            self._logger.debug("max nof samples: %i" %max_nofsamples)
-            self._logger.debug("appending %i new channel(s) and %i samples" %(other.ch, missingsamples))
+            self._logger.debug("max nof samples: %i" % max_nofsamples)
+            self._logger.debug(
+                "appending %i new channel(s) and %i samples" % (other.ch, missingsamples))
 
             if self.nofsamples > other.nofsamples:
                 self._logger.debug("self.nofsamples > other.nofsamples")
 
                 tmp = np.append(other.samples,
                                 np.zeros(((missingsamples), other.ch), dtype=other.samples.dtype),
                                 axis=0)
@@ -355,46 +419,47 @@
                 self.samples = np.append(tmp, other.samples, axis=1)
 
             else:
                 self._logger.debug("self.nofsamples == other.nofsamples")
                 self.samples = np.append(self.samples, other.samples, axis=1)
 
             self.ch = self.ch+other.ch
-            self.nofsamples=max_nofsamples
+            self.nofsamples = max_nofsamples
             self._set_duration()
 
     def concat(self, *args):
         """Concatenate (append) samples *after* the current audio data.
 
         example:
             x1 = 1234
             x2 = 5678
             x1.concat(x2) --> 12345678
 
         """
         for i, other in enumerate(args):
             assert isinstance(other, Audio), "only Audio() instances can be used"
 
-            self._logger.debug("** iteration %02i --> appending %s" %((i+1), other.__class__.__name__))
-            assert self.fs == other.fs, "Sample rates must match (%s != %s)" %(self.fs, other.fs)
+            self._logger.debug(
+                "** iteration %02i --> appending %s" % ((i+1), other.__class__.__name__))
+            assert self.fs == other.fs, "Sample rates must match (%s != %s)" % (self.fs, other.fs)
             assert self.samples.dtype == other.samples.dtype, \
-                "Data types must match (%s != %s)"%(self.samples.dtype, other.samples.dtype)
+                "Data types must match (%s != %s)" % (self.samples.dtype, other.samples.dtype)
             assert self.ch == other.ch, "channel count must match"
 
             self.samples = np.append(self.samples, other.samples, axis=0)
 
-            self.nofsamples=len(self.samples)
+            self.nofsamples = len(self.samples)
             self._set_duration()
 
     def gain(self, *args):
         """Apply gain to the audio samples. Always specify gain values in dB.
 
         Converts **IN PLACE**
         """
-        self._logger.debug('gains: %s' %str(args))
+        self._logger.debug('gains: %s' % str(args))
 
         dt  = self.samples.dtype
         lin = db2lin(args)
 
         # apply the (linear) gain
         self.samples = lin*self.samples
 
@@ -432,15 +497,15 @@
                 # We have to be careful when checking two's complement since the absolute value
                 # of the smallest possible value can't be represented without overflowing. For
                 # example: signed 16bit has range [-32768, 32767] so abs(-32768) cannot be
                 # represented in signed 16 bits --> use a bigger datatype
                 bigger  = np.asarray(self.samples, dtype=np.int64)
                 idx     = np.absolute(bigger).argmax(axis=0)
 
-            peak = np.array([self.samples[row,col] for col, row in enumerate(idx)])
+            peak = np.array([self.samples[row, col] for col, row in enumerate(idx)])
         else:
             # no samples are set but channels are configured
             idx  = np.zeros(self.ch, dtype=np.int64)
             peak = np.zeros(self.ch)
             peak[:] = float('nan')
 
         return peak, idx
@@ -477,30 +542,34 @@
         signed integer value. Converts **IN PLACE**
 
         Note: 24 bit signed integers and 8 bit unsigned integers currently unsupported.
         """
         assert targetbits in (8, 16, 32, 64)
         assert self.samples.dtype in (np.int8, np.int16, np.int32, np.int64,
                                       np.float32, np.float64)
-        dt = { 8 : 'int8',
-              16 : 'int16',
-              32 : 'int32',
-              64 : 'int64'}
+        dt = {
+            8  : 'int8',
+            16 : 'int16',
+            32 : 'int32',
+            64 : 'int64',
+            }
 
         sourcebits = self.samples.itemsize * 8
 
         if self.samples.dtype in (np.float32, np.float64):
-            self._logger.debug("source is %02i bits (float),   target is %2i bits (integer)"
-                              %(sourcebits, targetbits))
+            self._logger.debug(
+                "source is %02i bits (float),   target is %2i bits (integer)"
+                % (sourcebits, targetbits))
 
             self.samples = np.array(self.samples*(2**(targetbits-1)-1),
                                     dtype=dt.get(targetbits))
         else:
-            self._logger.debug("source is %02i bits (integer), target is %2i bits (integer)"
-                              %(sourcebits, targetbits))
+            self._logger.debug(
+                "source is %02i bits (integer), target is %2i bits (integer)"
+                % (sourcebits, targetbits))
             raise NotImplementedError("TODO: implement scale int->int")
 
     def convert_to_float(self, targetbits=64):
         """Scale integer values to equivalent floating point values
         between [-1.0, 1.0]. Converts **IN PLACE**
         """
         assert targetbits in (32, 64)
@@ -508,70 +577,82 @@
                                       np.float32, np.float64)
         dt = {32 : 'float32',
               64 : 'float64'}
 
         sourcebits = self.samples.itemsize * 8
 
         if self.samples.dtype in (np.int8, np.int16, np.int32, np.int64):
-            self._logger.debug("source is %02i bits (integer), target is %2i bits (float)"
-                              %(sourcebits, targetbits))
+            self._logger.debug(
+                "source is %02i bits (integer), target is %2i bits (float)"
+                % (sourcebits, targetbits))
 
             self.samples = np.array(self.samples/(2**(sourcebits-1)), dtype=dt.get(targetbits))
 
         else:
-            self._logger.debug("source is %02i bits (float),   target is %2i bits (float)"
-                              %(sourcebits, targetbits))
+            self._logger.debug(
+                "source is %02i bits (float),   target is %2i bits (float)"
+                % (sourcebits, targetbits))
 
             self.samples = np.array(self.samples, dtype=dt.get(targetbits))
 
     def write_wav_file(self, filename=None):
         """Save audio data to .wav file."""
 
         assert filename is not None, "Specify a filename, for example 'filename=audio.wav'"
 
-        self._logger.debug("writing file %s" %filename)
+        self._logger.debug("writing file %s" % filename)
         if self.samples.dtype == np.float64:
-            self._logger.warn("datatype is %s" %self.samples.dtype)
+            self._logger.warn("datatype is %s" % self.samples.dtype)
 
         try:
             scipy.io.wavfile.write(filename, int(self.fs), self.samples)
-        except:
-            self._logger.exception("Could not write file: '%s'" %filename)
+        except:     # noqa: E722
+            self._logger.exception("Could not write file: '%s'" % filename)
 
     def plot(self, ch=1, plotname=None, plotrange=(None, None), **kwargs):
         """Plot the audio data on a time domain plot.
 
         example:
 
             x1 = Sinetone(f0=0.2, fs=10, nofsamples=50)
             x1.plot(linestyle='--', marker='x', color='r', label='sine at 0.2Hz')
 
         """
 
         if ch != 'all':
             assert ch-1 < self.ch, "channel does not exist"
 
-        if plotrange[0] == None:
+        if plotrange[0] is None:
             plotrange = (0, plotrange[1])
-        if plotrange[1] == None:
+        if plotrange[1] is None:
             plotrange = (plotrange[0], self.duration)
 
         assert plotrange[0] >= 0 and plotrange[1] <= self.duration, "plotrange is out of bounds"
         assert plotrange[0] <= plotrange[1], "malformed plotrange"
 
         # Any fractional samples are truncated here
         samplerange = (int(plotrange[0]*self.fs), int(plotrange[1]*self.fs))
-        timerange = np.linspace(plotrange[0], plotrange[1], num=samplerange[1]-samplerange[0], endpoint=False)
+        timerange = np.linspace(
+            plotrange[0], plotrange[1], num=samplerange[1]-samplerange[0], endpoint=False)
 
         plt.figure(1)
-        plt.title("%s" %self.__class__.__name__)
+        plt.title("%s" % self.__class__.__name__)
         if ch != 'all':
-            plt.plot(timerange, self.samples[samplerange[0]:samplerange[1],ch-1], **kwargs)
+            plt.plot(timerange, self.samples[samplerange[0]:samplerange[1], ch-1], **kwargs)
         else:
-            plt.plot(timerange, self.samples[samplerange[0]:samplerange[1],:], **kwargs)
+            linestyles = ["-", ":", "-.", "--", ]
+            for i in range(self.ch):
+                plt.plot(
+                    timerange, self.samples[samplerange[0]:samplerange[1], i],
+                    label="ch: %02i" % (i+1),
+                    ls=linestyles[0],
+                    **kwargs)
+                linestyles.insert(0, linestyles.pop())  # cycle (rotate)
+            plt.legend(loc='best')
+
         plt.xlabel('Time [s]')
         plt.ylabel('Amplitude [linear]')
         if 'label' in kwargs:
             plt.legend(loc='best')
         plt.grid(True)
 
         if plotname is None:
@@ -579,24 +660,27 @@
         else:
             plt.savefig(plotname)
             plt.close(1)
 
     def plot_fft(self, plotname=None, window='hann', normalise=True, **kwargs):
         """Make a plot (in the frequency domain) of all channels"""
 
-        ymin = kwargs.get('ymin', -160) #dB
+        ymin = kwargs.get('ymin', -160)     # dB
+        linear = kwargs.get('linear', False)
 
         freq, mag = self.fft(window=window, normalise=normalise)
 
         fig_id = 1
         plt.figure(fig_id)
 
-        #plt.semilogx(freq, mag, **kwargs)   # plots all channel directly
         for ch in range(self.ch):
-            plt.semilogx(freq, mag[:,ch], label='ch%2i' %(ch+1))
+            if linear:
+                plt.plot(freq, mag[:, ch], label='ch%2i' % (ch+1))
+            else:
+                plt.semilogx(freq, mag[:, ch], label='ch%2i' % (ch+1))
 
         plt.xlim(left=1)    # we're not interested in freqs. below 1 Hz
         plt.ylim(bottom=ymin)
 
         plt.xlabel('Frequency [Hz]')
         plt.ylabel('Magnitude [dB]')
 
@@ -614,18 +698,18 @@
         fftsize = self.nofsamples
 
         # Avoid Mersenne Primes
         if fftsize in [(2**13)-1, (2**17)-1, (2**19)-1, (2**31)-1]:
             self._logger.warn("FFT size is a Mersenne Prime, increasing size by 1")
             fftsize = fftsize+1
 
-        self._logger.debug("fftsize: %i" %fftsize)
-        self._logger.debug("window : %s" %str(window))
+        self._logger.debug("fftsize: %i" % fftsize)
+        self._logger.debug("window : %s" % str(window))
 
-        win = scipy.signal.windows.get_window(window, Nx=self.nofsamples) # not fftsize!
+        win = scipy.signal.windows.get_window(window, Nx=self.nofsamples)   # not fftsize!
         win = np.expand_dims(win, axis=1)
         y   = self.samples*win
 
         Y   = np.fft.fft(y, n=fftsize, axis=0)
         if normalise:
             Y = Y/fftsize
 
@@ -640,83 +724,81 @@
     def dither(self, bits=16, distribution='TPDF'):
         raise NotImplementedError('TODO')
 
         assert distribution == 'TPDF', \
             "Only the Triangular Probability Density Function is implemented"
 
         # Triangular Probability Density Function
-        noise = np.random.triangular(-1, 0, 1, self.samples.shape)
+        #noise = np.random.triangular(-1, 0, 1, self.samples.shape)
 
-    def resample(self, targetrate=8000, converter_type="sinc_best"):
-        """Use the python bindings for the Secret Rabbit Code library
-        (aka libsamplerate) to perform sample rate conversion.
+    def decimate(self, N):
+        """
+        Throw away samples. Keep every Nth sample.
 
         Converts **IN PLACE**
 
-        https://pypi.org/project/samplerate/
-        http://www.mega-nerd.com/SRC/index.html
+        This is half of a downsampler. The other half would be to make sure
+        that the sampling theorem isn't violated for the new sample rate. So
+        the appropriate low pass filtering has to be done on the audio before
+        this metod is called, otherwise aliasing might occur.
         """
 
-        # From API docs:
-        # src_ratio : Equal to output_sample_rate / input_sample_rate.
-        ratio = targetrate / self.fs
-
-        self._logger.debug(
-            "source: %.2f destination: %.2f ratio %f",
-            self.fs, targetrate, ratio)
-
-        # We can use the simple API here since we always operate on the whole
-        # audio clip. See http://www.mega-nerd.com/SRC/api_simple.html
-        self.samples = samplerate.resample(
-            self.samples, ratio, converter_type=converter_type)
-
-        # The number of samples have changed, that is the whole point of
-        # this operation. Get the new values and calculate the new duration,
-        # hopefully that shouldn't change too much.
-        self.nofsamples, self.ch = self.samples.shape
-        self.fs = targetrate
-        self._set_duration()
+        self._logger.debug("decimate by factor N: %i", N)
+
+        # Use the slice operator. Efficient and fast. Will silently ignore the
+        # last incomplete chunk; for example 100 decimated by 3 leaves 1
+        # sample at the end that cannot be used.
+        self.samples = self.samples[::N]
+        self._logger.debug("decimated: %s", self.samples.shape)
+
+        self.nofsamples = len(self.samples)
+        self.set_sample_rate(self.fs/N)
+
+    def resample(self, *args, **kwargs):
+        # Previously used third party libsamplerate here. Does not install
+        # cleanly with pip (needs to compile from src, using cmake)
+        raise NotImplementedError("TODO")
 
     def set_sample_rate(self, new_fs):
         """Change the sample rate fs *without* up/down sample conversion.
         This would be the same as changing the playback speed. All data is
         left intact and only the time parameters (fs and duration) are
         changed.
         """
         ratio   = new_fs/self.fs
         self.fs = new_fs
 
-        self._logger.debug('ratio: %.3f' %ratio)
+        self._logger.debug('ratio: %.3f' % ratio)
         self._set_duration()
         return ratio
 
     def normalise(self):
         """Normalise samples so that the new range is
         [-1.0,  1.0] for floats
 
         Converts **IN PLACE**
 
         TODO: verify
         [-2^n, 2^n-1] for ints
         """
         peaks, unused_idx = self.peak()
-        self._logger.debug("raw peaks: %s" %peaks)
+        self._logger.debug("raw peaks: %s" % peaks)
 
         max_abs = np.max(np.absolute(peaks))
-        self._logger.debug("max_abs: %s" %max_abs)
+        self._logger.debug("max_abs: %s" % max_abs)
 
         self.samples = self.samples/max_abs
 
         peaks, unused_idx = self.peak()
-        self._logger.debug("new peaks: %s" %peaks)
+        self._logger.debug("new peaks: %s" % peaks)
 
-#===================================================================================================
-# Audio sub-classes
-#===================================================================================================
 
+# ==================================================================================================
+# Audio sub-classes
+# ==================================================================================================
 class Sinetone(Audio):
     def __init__(self, f0=997, fs=96000, duration=None, gaindb=0, nofsamples=0, phasedeg=0):
         """Generate a sine tone"""
         assert f0 < fs/2, "Sampling theorem is violated"
         Audio.__init__(self, channels=1, fs=fs, nofsamples=nofsamples, duration=duration)
 
         self.f0         = f0
@@ -728,30 +810,31 @@
     def _sine_gen(self, freq, pha):
         return np.sin(2*np.pi*freq*self.get_time()+np.deg2rad(pha))
 
     def __repr__(self):
         assert self.ch == 1, "If a channel has been appended we don't know anything about its data"
 
         s = 'Sinetone(f0=%r, fs=%r, nofsamples=%r, gaindb=%r, phasedeg=%r)' \
-            %(self.f0, self.fs, self.nofsamples,
-              lin2db(abs(float(self.peak()[0]))),  # only one channel here.
-              self.phasedeg)
+            % (self.f0, self.fs, self.nofsamples,
+               lin2db(abs(float(self.peak()[0]))),  # only one channel here.
+               self.phasedeg)
         return s
 
     def __str__(self):
         s  = Audio.__str__(self)
-        s += 'frequency        : %.1f [Hz]\n'   %self.f0
-        s += 'phase            : %.1f [deg]\n'  %self.phasedeg
+        s += 'frequency        : %.1f [Hz]\n'   % self.f0
+        s += 'phase            : %.1f [deg]\n'  % self.phasedeg
         s += '-----------------:---------------------\n'
         return s
 
     def set_sample_rate(self, new_fs):
         ratio = Audio.set_sample_rate(self, new_fs)
         self.f0 = ratio * self.f0
 
+
 class Sinetones(Sinetone):
     def __init__(self, *args, **kwargs):
         """Generate multiple sinetones. This is a quick way to generate multichannel audio.
         Each positional argument generates a sinetone at that channel. Setting the frequency
         to 0 guarantees that the channel is muted (contains samples with the value 0).
         Keywords accepted are similar to the ones used in the Sinetone() class.
 
@@ -827,53 +910,54 @@
         duration            = kwargs.pop('duration',    None)
         nofsamples          = kwargs.pop('nofsamples',  0)
         self._gaindb        = kwargs.pop('gaindb',      0)
         self.phasedeg       = kwargs.pop('phasedeg',    0)
         self.frequencies    = args
 
         for frequency in self.frequencies:
-            assert frequency < fs/2, "Sampling theorem is violated for frequency %.1f" %frequency
+            assert frequency < fs/2, "Sampling theorem is violated for frequency %.1f" % frequency
 
         if not isinstance(self._gaindb, int):
             assert len(self._gaindb) == len(self.frequencies), \
-                "set as many gains as channels used: %i != %i" %(len(self._gaindb),
-                                                                 len(self.frequencies))
+                "set as many gains as channels used: %i != %i" % (len(self._gaindb),
+                                                                  len(self.frequencies))
 
         Audio.__init__(self, channels=len(self.frequencies), fs=fs, nofsamples=nofsamples,
                        duration=duration)
 
         for i, frequency in enumerate(self.frequencies):
             if frequency != 0:
                 self._set_samples(idx=i, samples=self._sine_gen(frequency, self.phasedeg))
             else:
-                pass # channel is silence
+                pass    # channel is silence
 
         self.gain(self._gaindb)
 
     def __repr__(self):
         s = 'Sinetones(*%r, fs=%r, nofsamples=%r, gaindb=%r, phasedeg=%r)' \
-            %(list(self.frequencies), self.fs, self.nofsamples,self._gaindb,self.phasedeg)
+            % (list(self.frequencies), self.fs, self.nofsamples, self._gaindb, self.phasedeg)
         return s
 
     def __str__(self):
         s  = Audio.__str__(self)
-        s += 'phase (all ch)   : %.1f [deg]\n'  %self.phasedeg
+        s += 'phase (all ch)   : %.1f [deg]\n'  % self.phasedeg
         s += '                 :\n'
         for i, frequency in enumerate(self.frequencies):
             if frequency != 0:
-                s += 'channel %2i       : %.1f [Hz]\n'   %(i+1, frequency)
+                s += 'channel %2i       : %.1f [Hz]\n'   % (i+1, frequency)
             else:
-                s += 'channel %2i       :\n'   %(i+1)
+                s += 'channel %2i       :\n'   % (i+1)
         s += '-----------------:---------------------\n'
         return s
 
     def set_sample_rate(self, new_fs):
         ratio = Audio.set_sample_rate(self, new_fs)
         self.frequencies = [ratio*f for f in self.frequencies]
 
+
 class SquareWave(Audio):
     def __init__(self, f0=997, fs=96000, duration=None, gaindb=0, nofsamples=0,
                  phasedeg=0, dutycycle=0.5):
         """Generate an ideal squarewave."""
         assert f0 < fs/2, "Sampling theorem is violated"
         assert dutycycle < 1 and dutycycle > 0
         Audio.__init__(self, channels=1, fs=fs, nofsamples=nofsamples, duration=duration)
@@ -887,72 +971,74 @@
         self._set_samples(idx=0, samples=samples)
         self.gain(gaindb)
 
     def __repr__(self):
         assert self.ch == 1, "If a channel has been appended we don't know anything about its data"
 
         s = 'SquareWave(f0=%r, fs=%r, gaindb=%r, nofsamples=%r, phasedeg=%r, dutycycle=%r)' \
-            %(self.f0, self.fs,
-              lin2db(abs(float(self.peak()[0]))), # only one channel here.
-              self.nofsamples, self.phasedeg, self.dutycycle)
+            % (self.f0, self.fs,
+               lin2db(abs(float(self.peak()[0]))),   # only one channel here.
+               self.nofsamples, self.phasedeg, self.dutycycle)
         return s
 
     def __str__(self):
         s  = Audio.__str__(self)
-        s += 'frequency        : %.1f [Hz]\n'       %self.f0
-        s += 'phase            : %.1f [deg]\n'      %self.phasedeg
-        s += 'duty cycle       : %.3f (%4.1f%%)\n'  %(self.dutycycle, self.dutycycle*100)
+        s += 'frequency        : %.1f [Hz]\n'       % self.f0
+        s += 'phase            : %.1f [deg]\n'      % self.phasedeg
+        s += 'duty cycle       : %.3f (%4.1f%%)\n'  % (self.dutycycle, self.dutycycle*100)
         s += '-----------------:---------------------\n'
         return s
 
     def set_sample_rate(self, new_fs):
         ratio = Audio.set_sample_rate(self, new_fs)
         self.f0 = ratio * self.f0
 
+
 class FourierSeries(Sinetone):
     def __init__(self, f0=997, fs=96000, duration=None, gaindb=0, nofsamples=0,
                  phasedeg=0, harmonics=7,):
         """Construct a square wave by adding odd harmonics with decreasing
         amplitude, i.e. Fourier Series.
         """
         Sinetone.__init__(self, f0=f0, phasedeg=phasedeg, fs=fs, nofsamples=nofsamples,
                           duration=duration, gaindb=0)
 
         assert harmonics >= 0
 
         self.harmonics = harmonics
-        self._logger.debug("fundamental f0: %.1f" %f0)
+        self._logger.debug("fundamental f0: %.1f" % f0)
 
         for n in range(3, 2*(self.harmonics+1), 2):
             if n <= 15:
-                self._logger.debug("adding harmonic n: %2i with amplitude 1/%i" %(n, n))
+                self._logger.debug("adding harmonic n: %2i with amplitude 1/%i" % (n, n))
             if n == 17:
-                self._logger.debug("adding %i more harmonics..." %(self.harmonics-(n-3)//2))
+                self._logger.debug("adding %i more harmonics..." % (self.harmonics-(n-3)//2))
 
             #self.samples[:,0] += np.sin(2*np.pi*(n*f0)*self.get_time()+np.deg2rad(phasedeg*n))/n
-            self.samples[:,0] += (1/n)*self._sine_gen(n*f0, n*phasedeg)
+            self.samples[:, 0] += (1/n)*self._sine_gen(n*f0, n*phasedeg)
         self.gain(gaindb)
 
     def __repr__(self):
         assert self.ch == 1, "If a channel has been appended we don't know anything about its data"
 
         s = 'FourierSeries(f0=%r, fs=%r, gaindb=%r, nofsamples=%r, phasedeg=%r, harmonics=%r)' \
-            %(self.f0, self.fs,
-              lin2db(abs(float(self.peak()[0]))), # only one channel here.
-              self.nofsamples, self.phasedeg, self.harmonics)
+            % (self.f0, self.fs,
+               lin2db(abs(float(self.peak()[0]))),   # only one channel here.
+               self.nofsamples, self.phasedeg, self.harmonics)
         return s
 
     def __str__(self):
         s  = Sinetone.__str__(self)
         s = s.rstrip('-----------------:---------------------\n')
         s += '\n'
-        s += 'harmonics        : %i \n' %self.harmonics
+        s += 'harmonics        : %i \n' % self.harmonics
         s += '-----------------:---------------------\n'
         return s
 
+
 class Noise(Audio):
     colours = ('white', 'pink', 'brown', 'blue', 'violet', 'grey')
 
     def __init__(self, channels=1, fs=96000, duration=None, gaindb=-10, nofsamples=0,
                  colour='white'):
         """Generate uncorrelated noise.
 
@@ -960,163 +1046,177 @@
         pink        : -3dB per octave
         brown(ian)  : -6dB per octave
         blue        : +3dB per octave
         violet      : +6dB per octave
         grey        : equal loudness
         """
 
-        assert colour in Noise.colours, "choose the colour of the noise: %s" %str(Noise.colours)
+        assert colour in Noise.colours, "choose the colour of the noise: %s" % str(Noise.colours)
         Audio.__init__(self, channels=channels, fs=fs, nofsamples=nofsamples, duration=duration)
         # the distribution in np.random.uniform is half open, i.e -1.0 is
         # included but 1.0 is not. Possible fix: use integers instead, then
         # scale to floats. Might not work, since the integers will be
         # represented using twos complement and we then have an asymmetrical
         # range anyhow.
 
         self._colour = colour
 
         # first generate uniformly distributed noise, i.e. white noise. Then filter
         # to get the required shape.
         for ch in range(channels):
             self._set_samples(idx=ch,
                               samples=np.random.uniform(low=-1.0, high=1.0, size=self.nofsamples))
-        if self._colour=='pink':
+        if self._colour == 'pink':
             # -3dB per octave
             self._logger.debug("filtering to get pink noise")
             # http://dsp.stackexchange.com/q/322/6999
             B = [0.049922035, -0.095993537, 0.050612699, -0.004408786]
             A = [1, -2.494956002, 2.017265875, -0.522189400]
             self.samples = scipy.signal.lfilter(B, A, self.samples, axis=0)
 
-        elif self._colour=='brown':
+        elif self._colour == 'brown':
             # -6dB per octave
             raise NotImplementedError('TODO')
 
-        elif self._colour=='blue':
+        elif self._colour == 'blue':
             # +3dB per octave
             raise NotImplementedError('TODO')
 
-        elif self._colour=='violet':
+        elif self._colour == 'violet':
             # +6dB per octave
             raise NotImplementedError('TODO')
 
-        elif self._colour=='grey':
+        elif self._colour == 'grey':
             # equal loudness
             raise NotImplementedError('TODO')
 
         self.gain(gaindb)
 
     def __str__(self):
         s  = Audio.__str__(self)
-        s += 'colour           : %s\n'  %self._colour
+        s += 'colour           : %s\n'  % self._colour
         s += '-----------------:---------------------\n'
         return s
 
+
 class WavFile(Audio):
     def __init__(self, filename=None, scale2float=True):
         """Read a .wav file from disk"""
         assert filename is not None, "Specify a filename"
         self.filename = filename
 
         fs, samples = scipy.io.wavfile.read(filename)
         if samples.ndim == 1:
             samples = np.expand_dims(samples, axis=1)
 
         Audio.__init__(self, fs=fs, initialdata=samples)
 
-        del samples # just to make sure
+        del samples     # just to make sure
 
         if scale2float:
             self.convert_to_float(targetbits=64)
 
     def __str__(self):
         s  = Audio.__str__(self)
-        s += 'filename         : %s\n'  %os.path.basename(self.filename)
+        s += 'filename         : %s\n'  % os.path.basename(self.filename)
         s += '-----------------:---------------------\n'
         return s
 
-#===================================================================================================
-# Functions
-#===================================================================================================
 
+# ==================================================================================================
+# Functions
+# ==================================================================================================
 def lin2db(lin):
     with np.errstate(divide='ignore'):
         # linear value 0 is common (as -inf dB) so we ignore any division warnings
         db = 20*np.log10(lin)
     return db
 
+
 def pow2db(power):
     with np.errstate(divide='ignore'):
         # ignore any division warnings
         db = 10*np.log10(power)
     return db
 
+
 def db2lin(db):
     lin = np.power(10, np.array(db)/20)
     return lin
 
+
 def db2pow(db):
     power = np.power(10, np.array(db)/10)
     return power
 
+
 def speed_of_sound(temperature=20, medium='air'):
     """The speed of sound is depending on the medium and the temperature. For air at
     a temperature of 20 degree Celcius the speed of sound is approximately 343 [m/s]
     """
-    assert medium in ['air',], "TODO: water, iron"
+    assert medium in ['air', ], "TODO: water, iron"
 
     c = float('nan')
 
     if medium == 'air':
         c = 331.3*np.sqrt(1+temperature/273.15)
 
     return c
 
+
 def wavelength(frequency, speed=343.2):
     """Calculate the wavelength l of frequency f given the speed (of sound)"""
-    l = speed/frequency
-    return l
+    length = speed/frequency
+    return length
+
 
 def rad2hz(w0, fs=96000):
     """Calculate a normalised rotational frequency so that w0=2*pi --> f0=fs
 
                     w0
         f0 = fs * ------
                    2*pi
     """
     return fs*np.array(w0)/(2*np.pi)
 
+
 def hz2rad(f0, fs=96000):
     """Calculate a normalised angular frequency so that f0=fs --> w0=2*pi
 
                1
         w0 = ----- * 2*pi*f0
               fs
     """
     return (1/fs)*2*np.pi*np.array(f0)
 
+
 __all__ = [
-           # classes
-           'Audio',
-           'Sinetone',
-           'Sinetones',
-           'SquareWave',
-           'FourierSeries',
-           'Noise',
-           'WavFile',
-
-           # functions
-           'lin2db',
-           'pow2db',
-           'db2lin',
-           'db2pow',
-           'speed_of_sound',
-           'wavelength',
-           'rad2hz',
-           'hz2rad',
-           ]
+    # classes
+    'Audio',
+    'Sinetone',
+    'Sinetones',
+    'SquareWave',
+    'FourierSeries',
+    'Noise',
+    'WavFile',
+
+    # functions
+    'lin2db',
+    'pow2db',
+    'db2lin',
+    'db2pow',
+    'speed_of_sound',
+    'wavelength',
+    'rad2hz',
+    'hz2rad',
+    ]
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(levelname)-7s: %(module)s.%(funcName)-15s %(message)s',
-                        level='DEBUG')
+    logging.basicConfig(
+        format="%(levelname)-8s: %(module)s.%(funcName)-15s %(message)s",
+        level="DEBUG",
+        )
+    # some libraries are noisy in DEBUG
+    logging.getLogger("matplotlib").setLevel(logging.INFO)
+    logging.getLogger("PIL").setLevel(logging.WARNING)
 
     print('-- Done --')
```

### Comparing `zignal-0.6.0/zignal/sndcard.py` & `zignal-0.7.0/zignal/sndcard.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,47 @@
 Created on 15 Feb 2015
 
 @author: Ronny Andersson (ronny@andersson.tk)
 @copyright: (c) 2015 Ronny Andersson
 @license: MIT
 """
 
-# standard library
-from abc import ABCMeta, abstractmethod
+# Standard library
 import logging
 import warnings
+from abc import ABCMeta, abstractmethod
 
-# external libraries
+# Third party
 import numpy as np
+
+# Internal
+from zignal import Audio, Noise
+
 try:
     import pyaudio
 except ImportError:
-    warnings.warn("PyAudio not found. Will not be able to create sndcard instances", category=ImportWarning)
+    warnings.warn("PyAudio not found. Will not be able to create sndcard instances",
+                  category=ImportWarning)
 
-# local libraries
-from zignal import Audio, Noise
 
 def list_devices():
     """List all available sound cards."""
     return PA.list_devices()
 
-#===================================================================================================
+
+# ==================================================================================================
 # Abstract Base Class, inherit and implement the methods marked as @abstractmethod
-#===================================================================================================
+# ==================================================================================================
 class _Device(object, metaclass=ABCMeta):
     def __init__(self, *args, **kwargs):
         self._logger = logging.getLogger(__name__)
 
     def __str__(self):
         s  = '=======================================\n'
-        s += 'classname        : %s\n' %self.__class__.__name__
+        s += 'classname        : %s\n' % self.__class__.__name__
         return s
 
     def __enter__(self):
         self.open()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -64,17 +68,18 @@
 
     @abstractmethod
     def play_rec(self, x, **kwargs):
         """Play and record audio"""
         self._logger.debug("--- play_rec")
         assert isinstance(x, Audio)
 
-#===================================================================================================
+
+# ==================================================================================================
 # Stub class
-#===================================================================================================
+# ==================================================================================================
 class Stub(_Device):
     """Stub device that can be dropped in anywhere as a fake sound card.
     The record methods will return noise. This is intended to be used
     during development when a real device would block.
     """
 
     def play(self, x, **kwargs):
@@ -97,23 +102,24 @@
 
         # fake a signal with white noise
         n = Noise(channels=x.ch, fs=x.fs, nofsamples=x.nofsamples, gaindb=-60)
         n.convert_to_float(targetbits=32)
         y = Audio(fs=x.fs, initialdata=n.samples)
         return y
 
-#===================================================================================================
+
+# ==================================================================================================
 # PyAudio (Portaudio) implementation
-#===================================================================================================
+# ==================================================================================================
 class PA(_Device):
     """PyAudio wrapper. Uses the Audio base class as input signal and returns
     Audio instances after a recording. This implementation is using the blocking
     strategy."""
 
-    #--------------------------------------------------------------------------------
+    # -------------------------------------------------------------------------------
     #    Portaudio frame
     #
     #    http://music.columbia.edu/pipermail/portaudio/2007-January/006615.html
     #
     #    A 'frame' is all data required at a snapshot in time, where snapshots
     #    are the same as samplerate. This means that 2 ch of 16bit audio is
     #    a frame of size 32 bits
@@ -143,15 +149,15 @@
     #            |                   (32 bytes)                  |
     #            +-----------------------------------------------+
     #
     #    In other words, because we have audio data in a numpy vector
     #    where (rows,colums) --> (samples, channels) this means that each *row*
     #    is a frame.
     #
-    #--------------------------------------------------------------------------------
+    # -------------------------------------------------------------------------------
 
     def __init__(self, device_out='default', device_in='default'):
         """Set the device_out and/or device_in string based on the name of the
         sound card. An int can also be used if the id is known beforehand. Note that
         the id can change when another sound card is detected, for example when a USB
         card is connected. The available sound cards can be found by calling list_devices()
         """
@@ -168,28 +174,28 @@
         if isinstance(device_in, int):
             self._index_in = device_in
         else:
             self._index_in = self._get_id(name=device_in,  find_output=False)
 
     def __str__(self):
         s  = _Device.__str__(self)
-        s += 'portaudio        : %s %s\n'       %(pyaudio.get_portaudio_version(),
-                                                  pyaudio.get_portaudio_version_text())
-        s += 'pyaudio          : %s\n'          %pyaudio.__version__
-        s += 'output device    : id %i, %s\n'   %(self._index_out, self._device_out)
-        s += 'input device     : id %i, %s\n'   %(self._index_in,  self._device_in)
+        s += 'portaudio        : %s %s\n'       % (pyaudio.get_portaudio_version(),
+                                                   pyaudio.get_portaudio_version_text())
+        s += 'pyaudio          : %s\n'          % pyaudio.__version__
+        s += 'output device    : id %i, %s\n'   % (self._index_out, self._device_out)
+        s += 'input device     : id %i, %s\n'   % (self._index_in,  self._device_in)
         return s
 
     def _get_id(self, name=None, find_output=True):
         """Find the id of the sound card that matches the string name"""
         retval = -1
         pa_get_id = pyaudio.PyAudio()
 
         try:
-            if name=='default':
+            if name == 'default':
                 if find_output:
                     device = pa_get_id.get_default_output_device_info()
                     if device['maxOutputChannels'] > 0:
                         self._device_out = device['name']
                         retval = device['index']
 
                 else:
@@ -211,18 +217,18 @@
                             if device['name'] == name:
                                 retval = idx
                                 break
         finally:
             pa_get_id.terminate()
 
         if retval == -1:
-            s = "Device '%s' not found. Check the inputs and outputs arguments" %name
+            s = "Device '%s' not found. Check the inputs and outputs arguments" % name
             print(s)
             try:
-                print("Available devices: \n%s" %self.list_devices())
+                print("Available devices: \n%s" % self.list_devices())
             finally:
                 raise LookupError(s)
 
         return retval
 
     def open(self):
         """Open a PyAudio instance. This needs to be called before play(),
@@ -258,30 +264,33 @@
         the id can be found.
         """
 
         s  = ''
         s += '--------------------------------------------------------------------\n'
         s += 'id out  in  def.fs   API            name\n'
         s += '--------------------------------------------------------------------\n'
-        #--->| 0   2   2  44100.0  ALSA           Intel 82801AA-ICH: - (hw:0,0)
+        # -->| 0   2   2  44100.0  ALSA           Intel 82801AA-ICH: - (hw:0,0)
         pa_list_dev = pyaudio.PyAudio()
         try:
             for idx in range(pa_list_dev.get_device_count()):
                 device = pa_list_dev.get_device_info_by_index(idx)
-                s+='%2i %3i %3i %8.1f  %s %s\n' %(
+                s += '%2i %3i %3i %8.1f  %s %s\n' % (
                     device['index'],
                     device['maxOutputChannels'],
                     device['maxInputChannels'],
                     device['defaultSampleRate'],
-                    pa_list_dev.get_host_api_info_by_index(device['hostApi'])['name'].ljust(len('Windows WASAPI')),
+                    pa_list_dev.get_host_api_info_by_index(
+                        device['hostApi'])['name'].ljust(len('Windows WASAPI')),
                     device['name'],
                     )
             s += '\n'
-            s += 'default output device id: %i\n' %pa_list_dev.get_default_output_device_info()['index']
-            s += 'default input  device id: %i\n' %pa_list_dev.get_default_input_device_info()['index']
+            s += 'default output device id: %i\n' \
+                % pa_list_dev.get_default_output_device_info()['index']
+            s += 'default input  device id: %i\n' \
+                % pa_list_dev.get_default_input_device_info()['index']
             s += '--------------------------------------------------------------------\n'
         finally:
             pa_list_dev.terminate()
 
         return s
 
     def _data_format(self, x):
@@ -300,15 +309,15 @@
         elif x.samples.dtype == np.dtype(np.int16):
             self._logger.debug("pyaudio.paInt16")
             retval = pyaudio.paInt16
         elif x.samples.dtype == np.dtype(np.int32):
             self._logger.debug("pyaudio.paInt32")
             retval = pyaudio.paInt32
         else:
-            raise NotImplementedError("Data type not understood: %s" %x.samples.dtype)
+            raise NotImplementedError("Data type not understood: %s" % x.samples.dtype)
 
         return retval
 
     def _check_pow2(self, n):
         """Check that buffer size is a power of 2 (32, 64, ..., 1024, 2048, ...)"""
         check = 2**int(np.round(np.log2(n))) == n
         return check
@@ -320,22 +329,21 @@
         assert self._check_pow2(frames_per_buffer), \
             "Use a buffer size that is a power of 2 (1024, 2048, 4096, ...)"
 
         return True
 
     def _get_missing_frames(self, frames_per_buffer, length):
         """Calculate the number of frames missing to fill a buffer"""
-        missing_frames = frames_per_buffer - (length%frames_per_buffer)
+        missing_frames = frames_per_buffer - (length % frames_per_buffer)
 
-        self._logger.debug("frames per buffer : %i" %frames_per_buffer)
-        self._logger.debug("missing frames    : %i" %missing_frames)
+        self._logger.debug("frames per buffer : %i" % frames_per_buffer)
+        self._logger.debug("missing frames    : %i" % missing_frames)
 
         return missing_frames
 
-
     def play(self, x, frames_per_buffer=1024):
         """Play audio. If dropouts or buffer underruns occur try different
         values for the frames_per_buffer variable."""
 
         _Device.play(self, x)
         self._validate(frames_per_buffer)
 
@@ -345,24 +353,25 @@
         pad = Audio(channels=x.ch, fs=x.fs, nofsamples=missing_frames, dtype=x.samples.dtype)
 
         # append the missing frames to a copy of the audio to be played. We now have
         # audio that can be split into complete (full) buffers
         cpy = Audio(fs=x.fs, initialdata=x.samples)
         cpy.concat(pad)
 
-        assert len(cpy)%frames_per_buffer == 0
+        assert len(cpy) % frames_per_buffer == 0
 
-        stream = self.pa.open(format                = self._data_format(x),
-                              channels              = x.ch,
-                              rate                  = x.fs,
-                              frames_per_buffer     = frames_per_buffer,
-                              output_device_index   = self._index_out,
-                              input                 = False,
-                              output                = True,
-                              )
+        stream = self.pa.open(
+            format=self._data_format(x),
+            channels=x.ch,
+            rate=x.fs,
+            frames_per_buffer=frames_per_buffer,
+            output_device_index=self._index_out,
+            input=False,
+            output=True,
+            )
         try:
             self._logger.info("play: start")
             counter = 0
 
             # split the audio into chunks the size of one buffer, so we can
             # iterate over the audio in chunksizes of the same size as one buffer
             it = iter(np.split(cpy.samples, len(cpy)/frames_per_buffer))
@@ -374,17 +383,17 @@
 
             except StopIteration:
                 pass
 
             finally:
                 stream.stop_stream()
 
-            self._logger.debug("chunks played  : %i"    %counter)
-            self._logger.debug("samples played : %i"    %(counter*frames_per_buffer))
-            self._logger.debug("duration       : %.3f"  %(counter*frames_per_buffer/x.fs))
+            self._logger.debug("chunks played  : %i"    % counter)
+            self._logger.debug("samples played : %i"    % (counter*frames_per_buffer))
+            self._logger.debug("duration       : %.3f"  % (counter*frames_per_buffer/x.fs))
 
         finally:
             self._logger.debug("play: close stream")
             stream.close()
 
         self._logger.info("play: done")
 
@@ -401,27 +410,28 @@
         pad = Audio(channels=x.ch, fs=x.fs, nofsamples=missing_frames, dtype=x.samples.dtype)
 
         # append the missing frames to a copy of the audio to be played. We now have
         # audio that can be split into complete (full) buffers
         cpy = Audio(fs=x.fs, initialdata=x.samples)
         cpy.concat(pad)
 
-        assert len(cpy)%frames_per_buffer == 0
+        assert len(cpy) % frames_per_buffer == 0
 
         rec = Audio(channels=cpy.ch, fs=cpy.fs, nofsamples=len(cpy), dtype=cpy.samples.dtype)
 
-        stream = self.pa.open(format                = self._data_format(x),
-                              channels              = x.ch,
-                              rate                  = x.fs,
-                              frames_per_buffer     = frames_per_buffer,
-                              input_device_index    = self._index_in,
-                              output_device_index   = self._index_out,
-                              input                 = True,
-                              output                = True,
-                              )
+        stream = self.pa.open(
+            format=self._data_format(x),
+            channels=x.ch,
+            rate=x.fs,
+            frames_per_buffer=frames_per_buffer,
+            input_device_index=self._index_in,
+            output_device_index=self._index_out,
+            input=True,
+            output=True,
+            )
         try:
             self._logger.info("play_rec: start")
             counter = 0
 
             # split the audio into chunks the size of one buffer, so we can
             # iterate over the audio in chunksizes of the same size as one buffer
             it_out = iter(np.split(cpy.samples, len(cpy)/frames_per_buffer))
@@ -442,27 +452,27 @@
 
             except StopIteration:
                 pass
 
             finally:
                 stream.stop_stream()
 
-            self._logger.debug("chunks played  : %i"    %counter)
-            self._logger.debug("samples played : %i"    %(counter*frames_per_buffer))
-            self._logger.debug("duration       : %.3f"  %(counter*frames_per_buffer/x.fs))
+            self._logger.debug("chunks played  : %i"    % counter)
+            self._logger.debug("samples played : %i"    % (counter*frames_per_buffer))
+            self._logger.debug("duration       : %.3f"  % (counter*frames_per_buffer/x.fs))
 
         finally:
             self._logger.debug("play_rec: close stream")
             stream.close()
 
         # remove the padding (empty frames) added to fill the last buffer. Trim
         # at the start, since we can treat that as latency.
         rec.trim(start=missing_frames, end=None)
 
-        self._logger.debug("play_rec: trimmed %i samples from the start" %missing_frames)
+        self._logger.debug("play_rec: trimmed %i samples from the start" % missing_frames)
         self._check_if_clipped(rec)
         self._logger.info("play_rec: done")
 
         return rec
 
     def rec(self, duration=None, channels=1, fs=96000, frames_per_buffer=1024, dtype=np.float32):
         """Record. If dropouts or buffer underruns occur try different
@@ -473,24 +483,25 @@
 
         missing_frames = self._get_missing_frames(frames_per_buffer, int(duration*fs))
 
         nofsamples = missing_frames+int(duration*fs)
 
         rec = Audio(channels=channels, fs=fs, nofsamples=nofsamples, dtype=dtype)
 
-        assert len(rec)%frames_per_buffer == 0
+        assert len(rec) % frames_per_buffer == 0
 
-        stream = self.pa.open(format                = self._data_format(rec),
-                              channels              = rec.ch,
-                              rate                  = rec.fs,
-                              frames_per_buffer     = frames_per_buffer,
-                              input_device_index    = self._index_in,
-                              input                 = True,
-                              output                = False,
-                              )
+        stream = self.pa.open(
+            format=self._data_format(rec),
+            channels=rec.ch,
+            rate=rec.fs,
+            frames_per_buffer=frames_per_buffer,
+            input_device_index=self._index_in,
+            input=True,
+            output=False,
+            )
         try:
             self._logger.info("rec: start")
             counter = 0
 
             # split the audio into chunks the size of one buffer, so we can
             # iterate over the audio in chunksizes of the same size as one buffer
             it_in = iter(np.split(rec.samples, len(rec)/frames_per_buffer))
@@ -506,27 +517,27 @@
 
             except StopIteration:
                 pass
 
             finally:
                 stream.stop_stream()
 
-            self._logger.debug("chunks recorded : %i" %counter)
-            self._logger.debug("samples recorded: %i" %(counter*frames_per_buffer))
-            self._logger.debug("duration        : %.3f" %(counter*frames_per_buffer/rec.fs))
+            self._logger.debug("chunks recorded : %i" % counter)
+            self._logger.debug("samples recorded: %i" % (counter*frames_per_buffer))
+            self._logger.debug("duration        : %.3f" % (counter*frames_per_buffer/rec.fs))
 
         finally:
             self._logger.debug("rec: close stream")
             stream.close()
 
         # remove the padding (empty frames) added to fill the last buffer. Trim
         # at the start, since we can treat that as latency.
         rec.trim(start=missing_frames, end=None)
 
-        self._logger.debug("rec: trimmed %i samples from the start" %missing_frames)
+        self._logger.debug("rec: trimmed %i samples from the start" % missing_frames)
         self._check_if_clipped(rec)
         self._logger.info("rec: done")
 
         return rec
 
     def _check_if_clipped(self, rec):
         """check if the recording clipped, log the first clip for each channel"""
@@ -540,31 +551,37 @@
             # get the size of the integer type used, in bytes (2 for 16bit, 4 for 32bit)
             dt = np.dtype(rec.samples.dtype)
 
             # calculate the maximum possible postitive value. The maximum negative
             # value is max_possible_positive_value+1 (two's complement)
             max_possible_positive_value = 2**((8*dt.itemsize)-1) - 1
 
-        self._logger.debug("maximum possible positive value: %i" %max_possible_positive_value)
+        self._logger.debug("maximum possible positive value: %i" % max_possible_positive_value)
 
         for i, peaks in enumerate(zip(rec.peak()[0], rec.peak()[1])):
             peak_val, peak_pos = peaks
             # abs(-32768) overflows in signed 16 bit, use long(...) in py2 to get a bigger data type
             if abs(int(peak_val)) >= max_possible_positive_value:
                 clipped = True
                 clip_position = peak_pos/rec.fs
-                self._logger.warn("channel %02i clipped at %.3f" %(i+1, clip_position))
+                self._logger.warn("channel %02i clipped at %.3f" % (i+1, clip_position))
 
         return clipped
 
+
 __all__ = [
-           'list_devices',
-           'PA',
-           'Stub',
-           ]
+    'list_devices',
+    'PA',
+    'Stub',
+    ]
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(levelname)-7s: %(module)s.%(funcName)-15s %(message)s',
-                        level='DEBUG',
-                        )
+    logging.basicConfig(
+        format="%(levelname)-8s: %(module)s.%(funcName)-15s %(message)s",
+        level="DEBUG",
+        )
+    # some libraries are noisy in DEBUG
+    logging.getLogger("matplotlib").setLevel(logging.INFO)
+    logging.getLogger("PIL").setLevel(logging.WARNING)
+
     print(list_devices())
     print('++ End of script ++')
```

### Comparing `zignal-0.6.0/zignal/music/spn.py` & `zignal-0.7.0/zignal/music/spn.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 @copyright: (c) 2015 Ronny Andersson
 @license: MIT
 
 Scientific pitch notation (also known as American Standard Pitch Notation
 (ASPN) and International Pitch Notation (IPN))
 '''
 
-# standard library
+# Standard library
 import logging
 import re
 
+
 def key2index(key='A4'):
     """ Scientific pitch notation key mapped to an index
 
     Example:
 
        >>> key2index('A4')
        49
@@ -31,52 +32,53 @@
     """
 
     logger = logging.getLogger(__name__)
 
     valid_chars = "ABCDEFGb#x-0123456789"
 
     for c in key:
-        assert c in valid_chars, "Valid characters are: '%s'" %valid_chars
+        assert c in valid_chars, "Valid characters are: '%s'" % valid_chars
 
     m = re.match(r"(?P<note>^[A-G])(?P<half>b{0,3}|#{0,1}x{0,1})(?P<octave>[\-]?[0-9]+)", key)
     if m is None:
-        raise ValueError("Failed to match key '%s'" %key)
+        raise ValueError("Failed to match key '%s'" % key)
 
     matched = m.groupdict()
 
-    logger.debug("key: %s re: %s" %(key.ljust(4), matched))
+    logger.debug("key: %s re: %s" % (key.ljust(4), matched))
 
     octave  = int(matched.get('octave'))
     note    = matched.get('note')
     half    = matched.get('half')
 
     aug_or_dim = {
-                  'bbb' : -3,
-                  'bb'  : -2,
-                  'b'   : -1,
-                  '#'   :  1,
-                  'x'   :  2,
-                  '#x'  :  3,
-                  }
+        'bbb' : -3,
+        'bb'  : -2,
+        'b'   : -1,
+        '#'   :  1,
+        'x'   :  2,
+        '#x'  :  3,
+        }
 
     octave  = (octave-1)*12
     note    = " C D EF G A B".index(note)
     #          ^ ^ ^  ^ ^ ^ the spaces are important, we can 'index-search' the array
     half    = aug_or_dim.get(half, 0)
 
     # A0      = 1
     # A#0/Bb0 = 2
     # B0      = 3
     # C1      = 4
     pitch = 3 + octave + note + half
 
-    logger.debug("key: %s spn: %i" %(key.ljust(4), pitch))
+    logger.debug("key: %s spn: %i" % (key.ljust(4), pitch))
 
     return pitch
 
+
 def index2key(index=49):
     """Given the SPN index, return the corresponding SPN key
 
     Example:
 
         >>> index2key(1)
         'A0'
@@ -94,29 +96,35 @@
 
     notes   = ("C", "C#", "D", "D#", "E", "F", "F#", "G", "G#", "A", "A#", "B")
 
     # shift the index around so that
     #    C0 --> -8
     #    A0 -->  1
     #    C1 -->  4
-    notes_idx   = (index-3)%12 -1
-    octave      = (index+8)//12
+    notes_idx   = (index - 3) % 12 - 1
+    octave      = (index + 8) // 12
 
     # use the lookup table 'notes' to get the note name
     note        = notes[notes_idx]
 
-    logger.debug("index %3i notes_idx %3i: %s%i" %(index, notes_idx, note, octave))
+    logger.debug("index %3i notes_idx %3i: %s%i" % (index, notes_idx, note, octave))
 
-    spn_key = "%s%i" %(note, octave)
+    spn_key = "%s%i" % (note, octave)
 
     return spn_key
 
+
 __all__ = [
-           'key2index',
-           'index2key',
-           ]
+    'key2index',
+    'index2key',
+    ]
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(levelname)-7s: %(module)s.%(funcName)-15s %(message)s',
-                        level='DEBUG')
+    logging.basicConfig(
+        format="%(levelname)-8s: %(module)s.%(funcName)-15s %(message)s",
+        level="DEBUG",
+        )
+    # some libraries are noisy in DEBUG
+    logging.getLogger("matplotlib").setLevel(logging.INFO)
+    logging.getLogger("PIL").setLevel(logging.WARNING)
 
     print('-- Done --')
```

### Comparing `zignal-0.6.0/zignal/music/scales.py` & `zignal-0.7.0/zignal/music/scales.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Created on 21 Feb 2015
 
 @author: Ronny Andersson (ronny@andersson.tk)
 @copyright: (c) 2015 Ronny Andersson
 @license: MIT
 '''
 
-# standard library
+# Standard library
 import logging
 
-# external libraries
+# Third party
 import numpy as np
 
-# local libraries
+# Local folders
 from . import spn
 
+
 def equal_temperament(n):
     """Twelve-tone equal temperament (12TET) divides the octave into 12
     equal parts, making the interval between two ajacent notes the twelfth
     root of two.
 
     The argument n can be a number or a list/tuple/iterable.
 
@@ -27,14 +28,15 @@
     https://en.wikipedia.org/wiki/Equal_temperament
     """
 
     ratio = np.power(2, (np.array(n)/12))
 
     return ratio
 
+
 def piano_key2freq(n, a=49, tuning=440):
     """Twelve-tone equal temperament tuning for a theoretically ideal piano.
 
     The argument n can be a number or a list/tuple/iterable.
 
     The 49th key, called A4 is tuned to the reference (tuning) frequency, normally
     440Hz. The frequency is then given by
@@ -44,72 +46,83 @@
     https://en.wikipedia.org/wiki/Piano_key_frequencies
     """
 
     frequency = tuning*equal_temperament(np.array(n)-a)
 
     return frequency
 
+
 def piano_freq2key(f, a=49, tuning=440, quantise=False):
     """Frequency [f] to twelve-tone equal temperament tuning for a theoretically
     ideal piano, where 440Hz-->49
     """
 
     key = 12*np.log2(f/tuning) + a
 
     if quantise:
-        key = np.int(np.round(key))
+        key = int(np.round(key))
 
     return key
 
+
 def piano_note2freq(note, tuning=440):
     """Convert a piano note like 'C4' to 12TET frequency 261.6 Hz"""
     idx  = spn.key2index(note)
     freq = piano_key2freq(idx, tuning=tuning)
 
     return freq
 
+
 def piano_freq2note(f, tuning=440):
     """Given frequency f, calculate the nearest note in 12TET SPN notation"""
     idx = piano_freq2key(f, tuning=tuning, quantise=True)
     key = spn.index2key(idx)
 
     return key
 
+
 def midi_key2freq(n, tuning=440):
     """MIDI Tuning Standard. Convert midi note n to frequency f [Hz]. MIDI note 69
     equals 440 Hz, equal temperament.
 
     http://en.wikipedia.org/wiki/MIDI_Tuning_Standard
     """
 
     frequency = piano_key2freq(n, a=69, tuning=tuning)
 
     return frequency
 
+
 def midi_freq2key(f, tuning=440, quantise=False):
     """ MIDI Tuning Standard. Convert frequency f [Hz] to a midi note. MIDI note 69
     equals 440 Hz, equal temperament
 
     69+12*log2(f/440)
 
     http://en.wikipedia.org/wiki/MIDI_Tuning_Standard
     """
 
     midinote = piano_freq2key(f, a=69, tuning=tuning, quantise=quantise)
 
     return midinote
 
+
 __all__ = [
-           'equal_temperament',
-           'piano_key2freq',
-           'piano_freq2key',
-           'piano_note2freq',
-           'piano_freq2note',
-           'midi_key2freq',
-           'midi_freq2key',
-           ]
+    'equal_temperament',
+    'piano_key2freq',
+    'piano_freq2key',
+    'piano_note2freq',
+    'piano_freq2note',
+    'midi_key2freq',
+    'midi_freq2key',
+    ]
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(levelname)-7s: %(module)s.%(funcName)-15s %(message)s',
-                        level='DEBUG')
+    logging.basicConfig(
+        format="%(levelname)-8s: %(module)s.%(funcName)-15s %(message)s",
+        level="DEBUG",
+        )
+    # some libraries are noisy in DEBUG
+    logging.getLogger("matplotlib").setLevel(logging.INFO)
+    logging.getLogger("PIL").setLevel(logging.WARNING)
 
     print('-- Done --')
```

### Comparing `zignal-0.6.0/zignal/filters/linearfilter.py` & `zignal-0.7.0/zignal/filters/linearfilter.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 Created on 25 Jan 2014
 
 @author: Ronny Andersson (ronny@andersson.tk)
 @copyright: (c) 2014 Ronny Andersson
 @license: MIT
 """
 
-# standard library
+# Standard library
 import logging
 
-# external libraries
+# Third party
+import matplotlib.pyplot as plt
 import numpy as np
 import scipy.signal
-import matplotlib.pyplot as plt
 
-# local libraries
+# Internal
 from zignal import hz2rad, rad2hz
 
-#===================================================================================================
+
+# ==================================================================================================
 # Linear filter implementations
 #
 # Julius O. Smith III - Introduction to Digital Filters with audio applications
 # https://ccrma.stanford.edu/~jos/fp/
 #
-#===================================================================================================
+# ==================================================================================================
 class Filter(object):
     def __init__(self, B=None, A=None, fs=96000):
         """Standard linear recursive filter
 
                 b0 + b1*z^(-1) + b2*z^(-2) + ... + bn*z^(-n)
         H(z) = ------------------------
                 a0 + a1*z^(-1) + a2*z^(-2) + ... + an*z^(-n)
@@ -41,26 +42,26 @@
         self._B = None
         self._A = None
 
         self.set_coefficients(B=B, A=A)
 
     def __str__(self):
         s  = '=======================================\n'
-        s += 'classname        : %s\n'          %self.__class__.__name__
-        s += 'sample rate      : %.1f [Hz]\n'   %self.fs
-        s += 'feedforward  (B) : %s\n'          %str(self._B)
-        s += 'feedback     (A) : %s\n'          %str(self._A)
-        s += 'number of zeros  : %i\n'          %(len(self._B)-1)
-        s += 'number of poles  : %i\n'          %(len(self._A)-1)
-        s += 'minimum phase?   : %s\n'          %("Yes" if self.is_minimum_phase() else "No")
+        s += 'classname        : %s\n'          % self.__class__.__name__
+        s += 'sample rate      : %.1f [Hz]\n'   % self.fs
+        s += 'feedforward  (B) : %s\n'          % str(self._B)
+        s += 'feedback     (A) : %s\n'          % str(self._A)
+        s += 'number of zeros  : %i\n'          % (len(self._B)-1)
+        s += 'number of poles  : %i\n'          % (len(self._A)-1)
+        s += 'minimum phase?   : %s\n'          % ("Yes" if self.is_minimum_phase() else "No")
         s += '-----------------:---------------------\n'
         return s
 
     def __repr__(self):
-        return "Filter(B=%s, A=%s, fs=%s)" %(list(self._B), list(self._A), self.fs)
+        return "Filter(B=%s, A=%s, fs=%s)" % (list(self._B), list(self._A), self.fs)
 
     def filter_samples(self, samples):
         return scipy.signal.lfilter(self._B, self._A, samples, axis=0)
 
     def set_coefficients(self, B=None, A=None):
         """Set the filter coefficients.
 
@@ -97,15 +98,15 @@
         """Normalise the coefficients by dividing by A[0], effectively
         setting A[0]=1.0
         """
         assert len(self._A) >= 1
         assert len(self._B) >= 1
 
         a0 = self._A[0]
-        self._logger.debug("normalising using a0: %.4f" %a0)
+        self._logger.debug("normalising using a0: %.4f" % a0)
 
         self._B = self._B/a0
         self._A = self._A/a0
 
     def is_stable(self):
         """A filter is stable if all its poles are strictly inside the unit circle. A
         pole on the unit circle may be called marginally stable.
@@ -207,31 +208,31 @@
                 plt.savefig(filename)
             finally:
                 plt.close(1)
 
     def plot_pole_zero(self, filename=None):
         """Produce a plot with the location of all poles and zeros."""
         zeros, poles, gain = scipy.signal.tf2zpk(self._B, self._A)
-        self._logger.debug("zeros: %s" %zeros)
-        self._logger.debug("poles: %s" %poles)
-        self._logger.debug("gain : %s" %gain)
+        self._logger.debug("zeros: %s" % zeros)
+        self._logger.debug("poles: %s" % poles)
+        self._logger.debug("gain : %s" % gain)
 
         fig = plt.figure(1)
         ax = fig.add_subplot(111, aspect='equal')
-        circ = plt.Circle((0,0), radius=1, fill=False, color='black',
+        circ = plt.Circle((0, 0), radius=1, fill=False, color='black',
                           linestyle='dashed', linewidth=1.0)
         ax.add_patch(circ)
         ax.axhline(0, linestyle='dashed', color='black', linewidth=1.0)
         ax.axvline(0, linestyle='dashed', color='black', linewidth=1.0)
         ax.grid(True)
 
         ax.plot(poles.real, poles.imag, marker='x', ms=7.0, mew=1.5, mfc='blue', mec='blue',
-                ls='None', label='poles (%i)' %len(poles))
+                ls='None', label='poles (%i)' % len(poles))
         ax.plot(zeros.real, zeros.imag, marker='o', ms=7.0, mew=1.5, mfc='None', mec='red',
-                ls='None', label='zeros (%i)' %len(zeros))
+                ls='None', label='zeros (%i)' % len(zeros))
 
         ax.margins(0.1)
 
         # TODO: count multiples at (0,0)
 
         plt.legend(loc='best', numpoints=1)
         plt.title('Pole-zero locations')
@@ -268,14 +269,15 @@
             plt.show()
         else:
             try:
                 plt.savefig(filename)
             finally:
                 plt.close(1)
 
+
 class FIR(Filter):
     """Finite Impulse Response filter
 
     Also known as
      * nonrecursive filter
      * tapped delay line filter
      * moving average filter
@@ -285,21 +287,22 @@
     """
     def __init__(self, B=None, fs=96000):
         Filter.__init__(self, B=B, A=(1,), fs=fs)
 
     def __str__(self):
         s  = Filter.__str__(self)
         # += '-----------------:---------------------\n'
-        s += 'noise amplf.     : %s\n' %self.noise_amplification()
+        s += 'noise amplf.     : %s\n' % self.noise_amplification()
         return s
 
     def noise_amplification(self):
         '''The noise amplification is the sum of the squares of the coefficients'''
         return np.sum(np.power(self._B, 2))
 
+
 class IIR(Filter):
     """Infinite Impulse Response
 
     Also known as
      * recursive filter
      * Ladder filter
      * Lattice filter
@@ -309,27 +312,38 @@
     """
     def __init__(self, B=None, A=None, fs=96000):
         Filter.__init__(self, B=B, A=A, fs=fs)
 
     def __str__(self):
         s  = Filter.__str__(self)
         # += '-----------------:---------------------\n'
-        s += 'stable?          : %s\n' %("Yes" if self.is_stable() else "No")
+        s += 'stable?          : %s\n' % ("Yes" if self.is_stable() else "No")
         return s
 
-#===================================================================================================
-# Functions
-#===================================================================================================
 
+# ==================================================================================================
+# Functions
+# ==================================================================================================
 def normalised_frequency(f0=1000, fs=96000):
     '''Calculate a normalised frequency between [0.0, 1.0] where 1.0
     corresponds to pi [rad/sample]
     '''
     return f0/(fs/2)
 
-__all__ = ['Filter', 'FIR', 'IIR', 'normalised_frequency',]
+
+__all__ = [
+    'Filter',
+    'FIR',
+    'IIR',
+    'normalised_frequency',
+    ]
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(levelname)-7s: %(module)s.%(funcName)-15s %(message)s',
-                        level='DEBUG')
+    logging.basicConfig(
+        format="%(levelname)-8s: %(module)s.%(funcName)-15s %(message)s",
+        level="DEBUG",
+        )
+    # some libraries are noisy in DEBUG
+    logging.getLogger("matplotlib").setLevel(logging.INFO)
+    logging.getLogger("PIL").setLevel(logging.WARNING)
 
     print('++ End of script ++')
```

### Comparing `zignal-0.6.0/zignal/filters/biquads.py` & `zignal-0.7.0/zignal/filters/biquads.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 Created on 16 Feb 2014
 
 @author: Ronny Andersson (ronny@andersson.tk)
 @copyright: (c) 2014 Ronny Andersson
 @license: MIT
 """
 
-# standard library
+# Standard library
 import logging
 from abc import ABCMeta, abstractmethod
 
-# external libraries
+# Third party
 import numpy as np
 
-# local libraries
+# Internal
 from zignal.filters.linearfilter import IIR
 
+
 class Biquad(IIR):
     """Implements a two-pole, two-zeros biquadratic filter, biquad."""
     def __init__(self, B=None, A=None, fs=96000):
         IIR.__init__(self, B=B, A=A, fs=fs)
 
     def set_coefficients(self, B=None, A=None):
         """Overrides the method in the parent class so we can assure
         that we always have three B and three A coefficients.
         """
         self._logger.debug("set coefficients (class Biquad)")
 
-        self._B = np.array((1,0,0)) if B is None else np.array(B)
-        self._A = np.array((1,0,0)) if A is None else np.array(A)
+        self._B = np.array((1, 0, 0)) if B is None else np.array(B)
+        self._A = np.array((1, 0, 0)) if A is None else np.array(A)
 
         assert len(self._B) == 3, "Biquads have three B coefficients"
         assert len(self._A) == 3, "Biquads have three A coefficients"
 
+
 class BiquadNormalised(Biquad):
     """The normalised biquad always has A[0]=1.0
 
     This particular implementation keeps the number of coefficients to six in total,
     making sure that the normalise() method is called whenever we calculate the
     coefficients.
     """
@@ -48,20 +50,21 @@
         self._logger.debug("set coefficients (class BiquadNormalised)")
         Biquad.set_coefficients(self, B=B, A=A)
         self.normalise()
 
     def get_coefficients_Pd(self):
         """Return coefficients compatible with the [biquad~] object in Pd"""
         B, A = self.get_coefficients()
-        return (B[0], B[1], B[2], -A[1], -A[2]) #FIXME: Verify this
+        return (B[0], B[1], B[2], -A[1], -A[2])     # FIXME: Verify this
 
     def get_coefficients_MaxMSP(self):
         """Return coefficients compatible with the [biquad~] object in Max/MSP"""
         B, A = self.get_coefficients()
-        return (B[0], B[1], B[2], A[1], A[2])   #FIXME: Verify this
+        return (B[0], B[1], B[2], A[1], A[2])       # FIXME: Verify this
+
 
 class _BiquadParametric(BiquadNormalised, metaclass=ABCMeta):
     def __init__(self, filtertype=None, gaindb=0, f0=997, Q=0.707, fs=96000):
         BiquadNormalised.__init__(self, B=None, A=None, fs=fs)
 
         self._filtertype    = filtertype
         self._gaindb        = gaindb
@@ -121,14 +124,15 @@
         return s
 
     @abstractmethod
     def calculate_coefficients(self, filtertype=None, gaindb=None, f0=None, Q=None):
         # Implement this method in child class
         pass
 
+
 class RBJ(_BiquadParametric):
     """An implementation of the Audio EQ cookbook by Robert Bristow-Johnson
 
     Robert Bristow-Johnson - Cookbook formulae for audio EQ biquad filter coefficients
     http://www.musicdsp.org/files/Audio-EQ-Cookbook.txt
     """
 
@@ -171,15 +175,15 @@
             b2 =  (1 + _cos_w0)/2
             a0 =   1 + _alpha
             a1 =  -2 * _cos_w0
             a2 =   1 - _alpha
 
         elif filtertype == self.Types.bandpass1:
             # BPF:        H(s) = s / (s^2 + s/Q + 1)  (constant skirt gain, peak gain = Q)
-            b0 =   _sin_w0/2    #  =   Q*_alpha
+            b0 =   _sin_w0/2    # =   Q*_alpha
             b1 =   0
             b2 =  -_sin_w0/2    # =  -Q*_alpha
             a0 =   1 + _alpha
             a1 =  -2 * _cos_w0
             a2 =   1 - _alpha
 
         elif filtertype == self.Types.bandpass2:
@@ -234,18 +238,19 @@
             b2 =    _A*( (_A+1) + (_A-1)*_cos_w0 - 2*np.sqrt(_A)*_alpha )
             a0 =         (_A+1) - (_A-1)*_cos_w0 + 2*np.sqrt(_A)*_alpha
             a1 =     2*( (_A-1) - (_A+1)*_cos_w0                        )
             a2 =         (_A+1) - (_A-1)*_cos_w0 - 2*np.sqrt(_A)*_alpha
 
         else:
             valid = [i for i in vars(self.Types) if not i.startswith("__")]
-            raise NotImplementedError("Valid types are: %s" %valid)
+            raise NotImplementedError("Valid types are: %s" % valid)
 
         self.set_coefficients(B=(b0, b1, b2), A=(a0, a1, a2))
 
+
 class Zolzer(_BiquadParametric):
     """An implementation of Equalizer filters from DAFX - Zolzer et al."""
     class Types(object):
         lowpass     = 'lowpass'
         highpass    = 'highpass'
         peak        = 'peak'
         lowshelf    = 'lowshelf'
@@ -254,17 +259,17 @@
     def __init__(self, filtertype=None, gaindb=0, f0=997, Q=0.707, fs=96000):
         _BiquadParametric.__init__(self, filtertype=filtertype, gaindb=gaindb, f0=f0, Q=Q, fs=fs)
 
     def calculate_coefficients(self, filtertype=None, gaindb=None, f0=None, Q=None):
 
         K = np.tan(np.pi*f0/self.fs)
 
-        #------------
+        # -----------
         # peak
-        #------------
+        # -----------
         if filtertype == self.Types.peak:
             if gaindb > 0:
                 self._logger.debug('peak boost')
                 V0  = 10**(gaindb/20)
                 den =  1 +  1/Q * K + K**2
 
                 b0  = (1 + V0/Q * K + K**2)         / den
@@ -278,17 +283,17 @@
                 den =  1 + V0/Q * K + K**2
                 b0  = (1 +  1/Q * K + K**2)         / den
                 b1  = (          2 * (K**2 - 1))    / den
                 b2  = (1 -  1/Q * K + K**2)         / den
                 a1  = b1
                 a2  = (1 - V0/Q * K + K**2)         / den
 
-        #------------
+        # -----------
         # low shelf
-        #------------
+        # -----------
         elif filtertype == self.Types.lowshelf:
             # Parameter 'Q' is not used
             if gaindb > 0:
                 self._logger.debug('lowshelf boost')
                 V0  = 10**(gaindb/20)
                 den =  1+np.sqrt(2)*K + K**2
                 b0  = (1+np.sqrt(V0*2)*K + V0*K**2) / den
@@ -302,17 +307,17 @@
                 den =  1+np.sqrt(2*V0)*K + V0*K**2
                 b0  = (1+np.sqrt(2)*K + K**2)       / den
                 b1  = (2*(K**2-1))                  / den
                 b2  = (1-np.sqrt(2)*K + K**2)       / den
                 a1  = (2*(V0*K**2-1))               / den
                 a2  = (1-np.sqrt(2*V0)*K + V0*K**2) / den
 
-        #------------
+        # -----------
         # high shelf
-        #------------
+        # -----------
         elif filtertype == self.Types.highshelf:
             # Parameter 'Q' is not used
             if gaindb > 0:
                 self._logger.debug('highshelf boost')
                 V0  = 10**(gaindb/20)
                 den =  1+np.sqrt(2)*K + K**2
                 b0  = (V0+np.sqrt(V0*2)*K + K**2)   / den
@@ -325,31 +330,31 @@
                 V0  = 10**(-gaindb/20)
                 b0  = (1+np.sqrt(2)*K + K**2)           / (V0+np.sqrt(2*V0)*K +  K**2)
                 b1  = (2*(K**2-1))                      / (V0+np.sqrt(2*V0)*K +  K**2)
                 b2  = (1-np.sqrt(2)*K + K**2)           / (V0+np.sqrt(2*V0)*K +  K**2)
                 a1  = (2*(((K**2)/V0)-1))               / ( 1+np.sqrt(2/V0)*K + (K**2)/V0)
                 a2  = (1-np.sqrt(2/V0)*K + (K**2)/V0)   / ( 1+np.sqrt(2/V0)*K + (K**2)/V0)
 
-        #------------
+        # -----------
         # low pass
-        #------------
+        # -----------
         elif filtertype == self.Types.lowpass:
             # Parameter 'Q' is not used
             self._logger.debug('lowpass')
 
             den =  1+np.sqrt(2)*K + K**2
             b0  = (K**2)                    / den
             b1  = (2*K**2)                  / den
             b2  = (K**2)                    / den
             a1  = (2*(K**2-1))              / den
             a2  = (1-np.sqrt(2)*K + K**2)   / den
 
-        #------------
+        # -----------
         # high pass
-        #------------
+        # -----------
         elif filtertype == self.Types.highpass:
             # Parameter 'Q' is not used
             self._logger.debug('highpass')
 
             den =  1+np.sqrt(2)*K + K**2
             b0  = (1)                       / den
             b1  = (-2)                      / den
@@ -358,14 +363,24 @@
             a2  = (1-np.sqrt(2)*K + K**2)   / den
 
         else:
             raise NotImplementedError()
 
         self.set_coefficients(B=(b0, b1, b2), A=(1.0, a1, a2))
 
-__all__ = ['Biquad', 'RBJ', 'Zolzer',]
+
+__all__ = [
+    'Biquad',
+    'RBJ',
+    'Zolzer',
+    ]
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(levelname)-7s: %(module)s.%(funcName)-15s %(message)s',
-                        level='DEBUG')
+    logging.basicConfig(
+        format="%(levelname)-8s: %(module)s.%(funcName)-15s %(message)s",
+        level="DEBUG",
+        )
+    # some libraries are noisy in DEBUG
+    logging.getLogger("matplotlib").setLevel(logging.INFO)
+    logging.getLogger("PIL").setLevel(logging.WARNING)
 
     print('++ End of script ++')
```

### Comparing `zignal-0.6.0/README.md` & `zignal-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # zignal
 
 This is a python audio signal processing library.
 
-Python 2 is no longer supported, the last version to support python 2 is 0.2.0
-
 ## Example usage
 
     >>> import zignal
     >>>
     >>> x = zignal.Sinetone(fs=44100, f0=997, duration=0.1, gaindb=-20)
     >>> print(x)
     =======================================
@@ -54,37 +52,59 @@
     >>> f.plot_pole_zero()
     >>>
 
 See the examples folder for more examples.
 
 ## Requirements
 
-This library relies on numpy, scipy, matplotlib and optionally pyaudio (and nose for unit testing). It is recommended to create a virtual environment and let pip install the dependencies automatically.
+This library relies on numpy, scipy, matplotlib and optionally pyaudio. It is
+recommended to create a virtual environment and let pip install the
+dependencies automatically.
 
     python3 -m venv <name-of-virtualenv>
     . <name-of-virtualenv>/bin/activate
     pip install zignal
 
-Optionally, to be able to use a soundcard, first install the python development headers and the portaudio development files. On debian/ubuntu,
+Optionally, to be able to use a soundcard, first install the python development
+headers and the portaudio development files. On debian/ubuntu,
 
     sudo apt install python3-dev portaudio19-dev
 
 then run
 
     pip install zignal[sndcard]
 
 which will automatically build the portaudio library and then pyaudio.
 
 ## Local development
 
-Create a python3 virtualenv and install from the requirements.txt file to make the zignal library editable. Note that the python development headers (python3-dev) and portaudio19-dev must be installed first.
-
-    python3 -m venv zignaldev
-    . zignaldev/bin/activate
-    pip install -r requirements.txt
+Create a python3 virtualenv and install from the local source code to make the
+zignal library editable. Note that the python development headers (python3-dev)
+and portaudio19-dev must be installed first.
+
+    python3 -m venv venv_dev
+    . venv_dev/bin/activate
+    pip install --editable .[dev]
+
+By running `make` it is now possible to run isort, flake8 and also all the unit
+tests. They can also be executed directly from the command line, see the
+Makefile for the full commands to run.
+
+## Build a release
+
+    python3 -m venv venv_build
+    . ./venv_build/bin/activate
+    pip install --upgrade pip build
+    python3 -m build
 
 ## Design goals
 
-1.  Readability over efficiency. This is a python library for development and understanding of audio signal processing.
-2.  The initial goal is to write the functionality in pure python, with the use of numpy, scipy and matplotlib. See rule 1. If efficiency becomes an issue a c/c++ library might be implemented but the pure python code must remain the default choice.
-3.  Design for non real-time processing. Functionality to do real-time processing can be added if it does not break rule 1.
-4.  Self documentation. The code should aim to be well documented, in the source code itself.
+1.  Readability over efficiency. This is a python library for development and
+    understanding of audio signal processing.
+2.  The initial goal is to write the functionality in pure python, with the use
+    of numpy, scipy and matplotlib. See rule 1. If efficiency becomes an issue
+    a c/c++ library might be implemented but the pure python code must remain
+    the default choice.
+3.  Design for non real-time processing. Functionality to do real-time
+    processing can be added if it does not break rule 1.
+4.  Self documentation. The code should aim to be well documented, in the
+    source code itself.
```

