# Comparing `tmp/librosa-0.9.1.tar.gz` & `tmp/librosa-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/librosa/librosa/dist/tmpl8kc6uxd/librosa-0.9.1.tar", last modified: Tue Feb 15 23:14:39 2022, max compression
+gzip compressed data, was "/home/runner/work/librosa/librosa/dist/tmpjm71qqwd/librosa-0.9.2.tar", last modified: Mon Jun 27 11:25:30 2022, max compression
```

## Comparing `librosa-0.9.1.tar` & `librosa-0.9.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 23:14:39.000000 librosa-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     4226 2022-02-15 23:14:29.000000 librosa-0.9.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-02-15 23:14:29.000000 librosa-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-02-15 23:14:29.000000 librosa-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-02-15 23:14:29.000000 librosa-0.9.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-15 23:14:29.000000 librosa-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5586 2022-02-15 23:14:39.000000 librosa-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4328 2022-02-15 23:14:29.000000 librosa-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa/
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    23605 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/beat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa/core/
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51648 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)    44406 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/constantq.py
--rw-r--r--   0 runner    (1001) docker     (121)    60320 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/fft.py
--rw-r--r--   0 runner    (1001) docker     (121)    10051 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/harmonic.py
--rw-r--r--   0 runner    (1001) docker     (121)    18045 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/notation.py
--rw-r--r--   0 runner    (1001) docker     (121)    31584 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/pitch.py
--rw-r--r--   0 runner    (1001) docker     (121)    85837 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/core/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)    19708 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/decompose.py
--rw-r--r--   0 runner    (1001) docker     (121)    46253 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/display.py
--rw-r--r--   0 runner    (1001) docker     (121)    21823 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/effects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa/feature/
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9666 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/feature/inverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     9849 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/feature/rhythm.py
--rw-r--r--   0 runner    (1001) docker     (121)    64375 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/feature/spectral.py
--rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/feature/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    48102 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    19666 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/onset.py
--rw-r--r--   0 runner    (1001) docker     (121)    38529 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/segment.py
--rw-r--r--   0 runner    (1001) docker     (121)    60492 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/_nnls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3722 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa/util/example_data/
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/example_data/index.json
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/example_data/registry.txt
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7058 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/files.py
--rw-r--r--   0 runner    (1001) docker     (121)    12053 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/matching.py
--rw-r--r--   0 runner    (1001) docker     (121)    68986 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-02-15 23:14:29.000000 librosa-0.9.1/librosa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5586 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-15 23:14:39.000000 librosa-0.9.1/librosa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-02-15 23:14:29.000000 librosa-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-02-15 23:14:39.000000 librosa-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-02-15 23:14:29.000000 librosa-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:25:30.000000 librosa-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-06-27 11:25:16.000000 librosa-0.9.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-06-27 11:25:16.000000 librosa-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4307 2022-06-27 11:25:16.000000 librosa-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2022-06-27 11:25:16.000000 librosa-0.9.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-27 11:25:16.000000 librosa-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6865 2022-06-27 11:25:30.000000 librosa-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-06-27 11:25:16.000000 librosa-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa/
+-rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23605 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/beat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52824 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44406 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/constantq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60320 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/fft.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10051 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18045 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/notation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31584 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/pitch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86321 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/core/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19708 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46253 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21999 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/effects.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa/feature/
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9667 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/feature/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9849 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/feature/rhythm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    64376 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/feature/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/feature/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48102 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19666 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/onset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38530 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/segment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61072 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/_nnls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3722 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa/util/example_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/example_data/index.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/example_data/registry.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7306 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/files.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12053 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/matching.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68986 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-06-27 11:25:16.000000 librosa-0.9.2/librosa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6865 2022-06-27 11:25:29.000000 librosa-0.9.2/librosa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-27 11:25:29.000000 librosa-0.9.2/librosa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-27 11:25:30.000000 librosa-0.9.2/librosa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-27 11:25:16.000000 librosa-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-06-27 11:25:30.000000 librosa-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-27 11:25:16.000000 librosa-0.9.2/setup.py
```

### Comparing `librosa-0.9.1/AUTHORS.md` & `librosa-0.9.2/AUTHORS.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,22 @@
 * N. Dorukhan Sergin <https://github.com/dorukhansergin>
 * Paul Biberstein <https://github.com/P-bibs>
 * Myungchul Keum <https://github.com/dofuuz>
 * Daniel Faronbi <https://github.com/dafaronbi>
 * Iran Roman <https://github.com/iranroman>
 * philstem <https://github.com/philstem>
 * Alex Malins <https://github.com/alexmalins>
+* i-aky-y <https://github.com/i-aky-y>
+* Asmitha Krishnakumar <https://github.com/Asmitha-K>
+* Chandrashekhar Ramaprasad <https://github.com/cr2007>
+* Xiao-Ming <https://github.com/Xiao-Ming>
+* Will Monroe <https://github.com/futurulus>
+* Lorenz Nickel <https://github.com/LorenzNickel>
 
 Some feature extraction code was based on <https://github.com/ronw/frontend> by Ron Weiss.
 
-Large portions of LibROSA were ported from MATLAB code by Dan Ellis <http://www.ee.columbia.edu/~dpwe/resources/matlab/>.
+Large portions of librosa were ported from MATLAB code by Dan Ellis <http://www.ee.columbia.edu/~dpwe/resources/matlab/>.
 
 Some spectral features were ported from original MATLAB implementations by Erik Schmidt and Jeff Scott
 at the Drexel METlab <http://music.ece.drexel.edu/>
 
 Additional thanks to Emanuele Coviello and Erik Schmidt for testing, bug reports and fixes.
```

### Comparing `librosa-0.9.1/CODE_OF_CONDUCT.md` & `librosa-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/CONTRIBUTING.md` & `librosa-0.9.2/CONTRIBUTING.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,16 +11,22 @@
 
 1. Fork the [project repository](http://github.com/librosa/librosa):
    click on the 'Fork' button near the top of the page. This creates
    a copy of the code under your account on the GitHub server.
 
 2. Clone this copy to your local disk:
 
-          $ git clone git@github.com:YourLogin/librosa.git
+          $ git clone --recursive git@github.com:YourLogin/librosa.git
           $ cd librosa 
+          $ git pull --recurse-submodules
+
+    These commands will clone the main librosa repository, as well as the submodule
+    that contains testing data.  This should work automatically, but you may also
+    want to read [Working with Submodules](https://github.blog/2016-02-01-working-with-submodules/)
+    for a better understanding of how this works.
 
 3. Remove any previously installed librosas:
             
           $ pip uninstall librosa
 
 and install your local copy with testing dependencies:
 
@@ -38,15 +44,15 @@
           $ git add modified_files
           $ git commit
 
    to record your changes in Git, then push them to GitHub with:
 
           $ git push -u origin my-feature
 
-Finally, go to the web page of the your fork of the librosa repo,
+Finally, go to the web page of your fork of the librosa repo,
 and click 'Pull request' to send your changes to the maintainers for
 review. This will send an email to the committers.
 
 (If any of the above seems like magic to you, then look up the 
 [Git documentation](http://git-scm.com/documentation) on the web.)
 
 It is recommended to check that your contribution complies with the
```

### Comparing `librosa-0.9.1/LICENSE.md` & `librosa-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/PKG-INFO` & `librosa-0.9.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,147 +1,208 @@
-Metadata-Version: 2.1
-Name: librosa
-Version: 0.9.1
-Summary: Python module for audio and music processing
-Home-page: https://librosa.org
-Author: Brian McFee, librosa development team
-Author-email: brian.mcfee@nyu.edu
-License: ISC
-Project-URL: Documentation, https://librosa.org/doc
-Project-URL: Download, https://github.com/librosa/librosa/releases
-Project-URL: Source, https://github.com/librosa/librosa
-Project-URL: Tracker, https://github.com/librosa/librosa/issues
-Project-URL: Discussion forum, https://groups.google.com/g/librosa
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Framework :: Matplotlib
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: display
-License-File: LICENSE.md
+[![librosa logo](docs/img/librosa_logo_text.svg)](https://librosa.org/)
+
+# librosa
+
 
-librosa
-=======
 A python package for music and audio analysis.  
 
 [![PyPI](https://img.shields.io/pypi/v/librosa.svg)](https://pypi.python.org/pypi/librosa)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/librosa/badges/version.svg)](https://anaconda.org/conda-forge/librosa)
 [![License](https://img.shields.io/pypi/l/librosa.svg)](https://github.com/librosa/librosa/blob/main/LICENSE.md)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.591533.svg)](https://doi.org/10.5281/zenodo.591533)
 
 [![CI](https://github.com/librosa/librosa/actions/workflows/ci.yml/badge.svg)](https://github.com/librosa/librosa/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/librosa/librosa/branch/main/graph/badge.svg?token=ULWnUHaIJC)](https://codecov.io/gh/librosa/librosa)
+[![Docs](https://github.com/librosa/librosa/actions/workflows/docs.yml/badge.svg)](https://github.com/librosa/librosa/actions/workflows/docs.yml)
+
+#  Table of Contents
+
+- [Documentation](#Documentation)
+- [Installation](#Installation)
+  - [Using PyPI](#using-pypi)
+  - [Using Anaconda](#using-anaconda)
+  - [Building From Source](#building-from-source)
+  - [Hints for Installation](#hints-for-the-installation)
+    - [`soundfile`](#soundfile)
+    - [`audioread` and MP3 support](#audioread-and-mp3-support)
+      - [Linux (`apt get`)](#linux-apt-get)
+      - [Linux (`yum`)](#linux-yum)
+      - [Mac](#mac)
+      - [Windows](#windows)
+- [Discussion](#discussion)
+- [Citing](#citing)
+
+---
+
+## Documentation
 
 
-Documentation
--------------
 See https://librosa.org/doc/ for a complete reference manual and introductory tutorials.
 
 The [advanced example gallery](https://librosa.org/doc/latest/advanced.html) should give you a quick sense of the kinds
 of things that librosa can do.
 
-Installation
-------------
+---
+
+[Back To Top ↥](#librosa)
+
+
+## Installation
+
+
+### Using PyPI
 
 The latest stable release is available on PyPI, and you can install it by saying
 ```
-pip install librosa
+python -m pip install librosa
 ```
 
-Anaconda users can install using ``conda-forge``:
+### Using Anaconda
+
+Anaconda users can install using ```conda-forge```:
 ```
 conda install -c conda-forge librosa
 ```
 
-To build librosa from source, say `python setup.py build`.
-Then, to install librosa, say `python setup.py install`.
-If all went well, you should be able to execute the demo scripts under `examples/`
-(OS X users should follow the installation guide given below).
+### Building from source
+
+To build librosa from source, say 
+```
+python setup.py build
+```
+Then, to install librosa, say 
+```
+python setup.py install
+```
+If all went well, you should be able to execute the following commands from a python console:
+```
+import librosa
+librosa.show_versions()
+```
+This should print out a description of your software environment, along with the installed versions of other packages used by librosa.
+
+📝 OS X users should follow the installation guide given below.
 
 Alternatively, you can download or clone the repository and use `pip` to handle dependencies:
 
 ```
 unzip librosa.zip
-pip install -e librosa
+python -m pip install -e librosa
 ```
 or
+
 ```
 git clone https://github.com/librosa/librosa.git
-pip install -e librosa
+python -m pip install -e librosa
 ```
 
 By calling `pip list` you should see `librosa` now as an installed package:
 ```
 librosa (0.x.x, /path/to/librosa)
 ```
 
+---
+
+[Back To Top ↥](#librosa)
+
 ### Hints for the Installation
 
 `librosa` uses `soundfile` and `audioread` to load audio files.
-Note that `soundfile` does not currently support MP3, which will cause librosa to
+
+📝 Note that `soundfile` does not currently support MP3, which will cause librosa to
 fall back on the `audioread` library.
 
-#### soundfile
+### `soundfile`
 
 If you're using `conda` to install librosa, then most audio coding dependencies (except MP3) will be handled automatically.
 
 If you're using `pip` on a Linux environment, you may need to install `libsndfile`
 manually.  Please refer to the [SoundFile installation documentation](https://pysoundfile.readthedocs.io/#installation) for details.
 
-#### audioread and MP3 support
+### `audioread` and MP3 support
 
 To fuel `audioread` with more audio-decoding power (e.g., for reading MP3 files),
 you may need to install either *ffmpeg* or *GStreamer*.
 
-*Note that on some platforms, `audioread` needs at least one of the programs to work properly.*
+📝*Note that on some platforms, `audioread` needs at least one of the programs to work properly.*
 
 If you are using Anaconda, install *ffmpeg* by calling
+
 ```
 conda install -c conda-forge ffmpeg
 ```
 
 If you are not using Anaconda, here are some common commands for different operating systems:
 
-* Linux (apt-get): `apt-get install ffmpeg` or `apt-get install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly`
-* Linux (yum): `yum install ffmpeg` or `yum install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly`
-* Mac: `brew install ffmpeg` or `brew install gstreamer`
-* Windows: download ffmpeg binaries from this [website](https://www.gyan.dev/ffmpeg/builds/) or gstreamer binaries from this [website](https://gstreamer.freedesktop.org/)
+- ####  Linux (`apt-get`): 
+
+```
+apt-get install ffmpeg
+```
+or
+ 
+```
+apt-get install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly
+```
+- #### Linux (`yum`):
+```
+yum install ffmpeg
+```
+or
+
+
+```
+yum install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly
+```
+
+- #### Mac: 
+```
+brew install ffmpeg
+```
+or
+
+```
+brew install gstreamer
+```
+
+- #### Windows: 
+
+download ffmpeg binaries from this [website](https://www.gyan.dev/ffmpeg/builds/) or gstreamer binaries from this [website](https://gstreamer.freedesktop.org/)
 
 For GStreamer, you also need to install the Python bindings with 
+
 ```
-pip install pygobject
+python -m pip install pygobject
 ```
 
-Discussion
-----------
+---
+
+[Back To Top ↥](#librosa)
+
+## Discussion
+
 
 Please direct non-development questions and discussion topics to our web forum at
 https://groups.google.com/forum/#!forum/librosa
 
+---
+
+[Back To Top ↥](#librosa)
+
+## Citing
 
-Citing
-------
 
 If you want to cite librosa in a scholarly work, there are two ways to do it.
 
 - If you are using the library for your work, for the sake of reproducibility, please cite
   the version you used as indexed at Zenodo:
 
     [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.591533.svg)](https://doi.org/10.5281/zenodo.591533)
 
 - If you wish to cite librosa for its design, motivation etc., please cite the paper
   published at SciPy 2015:
 
     McFee, Brian, Colin Raffel, Dawen Liang, Daniel PW Ellis, Matt McVicar, Eric Battenberg, and Oriol Nieto. "librosa: Audio and music signal analysis in python." In Proceedings of the 14th python in science conference, pp. 18-25. 2015.
 
+---
 
+[Back To Top ↥](#librosa)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `librosa-0.9.1/librosa/__init__.py` & `librosa-0.9.2/librosa/__init__.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/_cache.py` & `librosa-0.9.2/librosa/_cache.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/beat.py` & `librosa-0.9.2/librosa/beat.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/__init__.py` & `librosa-0.9.2/librosa/core/__init__.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/audio.py` & `librosa-0.9.2/librosa/core/audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,27 +60,28 @@
     Audio will be automatically resampled to the given rate
     (default ``sr=22050``).
 
     To preserve the native sampling rate of the file, use ``sr=None``.
 
     Parameters
     ----------
-    path : string, int, pathlib.Path, soundfile.SoundFile or file-like object
+    path : string, int, pathlib.Path, soundfile.SoundFile, audioread object, or file-like object
         path to the input file.
 
         Any codec supported by `soundfile` or `audioread` will work.
 
         Any string file paths, or any object implementing Python's
         file interface (e.g. `pathlib.Path`) are supported as `path`.
 
         If the codec is supported by `soundfile`, then `path` can also be
         an open file descriptor (int) or an existing `soundfile.SoundFile` object.
 
-        On the contrary, if the codec is not supported by `soundfile`
-        (for example, MP3), then `path` must be a file path (string or `pathlib.Path`).
+        Pre-constructed audioread decoders are also supported here, see the example
+        below.  This can be used, for example, to force a specific decoder rather
+        than relying upon audioread to select one for you.
 
     sr : number > 0 [scalar]
         target sampling rate
 
         'None' uses the native sampling rate
 
     mono : bool
@@ -139,67 +140,96 @@
     >>> filename = librosa.ex('brahms')
     >>> y, sr = librosa.load(filename, offset=15.0, duration=5.0)
     >>> y
     array([0.146, 0.144, ..., 0.128, 0.015], dtype=float32)
     >>> sr
     22050
 
+    >>> # Load using an already open SoundFile object
+    >>> import soundfile
+    >>> sfo = soundfile.SoundFile(librosa.ex('brahms'))
+    >>> y, sr = librosa.load(sfo)
+
+    >>> # Load using an already open audioread object
+    >>> import audioread.ffdec  # Use ffmpeg decoder
+    >>> aro = audioread.ffdec.FFmpegAudioFile(librosa.ex('brahms'))
+    >>> y, sr = librosa.load(aro)
     """
 
-    try:
-        if isinstance(path, sf.SoundFile):
-            # If the user passed an existing soundfile object,
-            # we can use it directly
-            context = path
-        else:
-            # Otherwise, create the soundfile object
-            context = sf.SoundFile(path)
-
-        with context as sf_desc:
-            sr_native = sf_desc.samplerate
-            if offset:
-                # Seek to the start of the target read
-                sf_desc.seek(int(offset * sr_native))
-            if duration is not None:
-                frame_duration = int(duration * sr_native)
+    if isinstance(path, tuple(audioread.available_backends())):
+        # Force the audioread loader if we have a reader object already
+        y, sr_native = __audioread_load(path, offset, duration, dtype)
+    else:
+        # Otherwise try soundfile first, and then fall back if necessary
+        try:
+            y, sr_native = __soundfile_load(path, offset, duration, dtype)
+
+        except RuntimeError as exc:
+            # If soundfile failed, try audioread instead
+            if isinstance(path, (str, pathlib.PurePath)):
+                warnings.warn("PySoundFile failed. Trying audioread instead.", stacklevel=2)
+                y, sr_native = __audioread_load(path, offset, duration, dtype)
             else:
-                frame_duration = -1
-
-            # Load the target number of frames, and transpose to match librosa form
-            y = sf_desc.read(frames=frame_duration, dtype=dtype, always_2d=False).T
-
-    except RuntimeError as exc:
-        # If soundfile failed, try audioread instead
-        if isinstance(path, (str, pathlib.PurePath)):
-            warnings.warn("PySoundFile failed. Trying audioread instead.", stacklevel=2)
-            y, sr_native = __audioread_load(path, offset, duration, dtype)
-        else:
-            raise (exc)
+                raise exc
 
     # Final cleanup for dtype and contiguity
     if mono:
         y = to_mono(y)
 
     if sr is not None:
         y = resample(y, orig_sr=sr_native, target_sr=sr, res_type=res_type)
 
     else:
         sr = sr_native
 
     return y, sr
 
 
+def __soundfile_load(path, offset, duration, dtype):
+    """Load an audio buffer using soundfile."""
+    if isinstance(path, sf.SoundFile):
+        # If the user passed an existing soundfile object,
+        # we can use it directly
+        context = path
+    else:
+        # Otherwise, create the soundfile object
+        context = sf.SoundFile(path)
+
+    with context as sf_desc:
+        sr_native = sf_desc.samplerate
+        if offset:
+            # Seek to the start of the target read
+            sf_desc.seek(int(offset * sr_native))
+        if duration is not None:
+            frame_duration = int(duration * sr_native)
+        else:
+            frame_duration = -1
+
+        # Load the target number of frames, and transpose to match librosa form
+        y = sf_desc.read(frames=frame_duration, dtype=dtype, always_2d=False).T
+
+    return y, sr_native
+
+
 def __audioread_load(path, offset, duration, dtype):
     """Load an audio buffer using audioread.
 
     This loads one block at a time, and then concatenates the results.
     """
 
     y = []
-    with audioread.audio_open(path) as input_file:
+
+    if isinstance(path, tuple(audioread.available_backends())):
+        # If we have an audioread object already, don't bother opening
+        reader = path
+    else:
+        # If the input was not an audioread object, try to open it
+        reader = audioread.audio_open(path)
+
+    with reader as input_file:
         sr_native = input_file.samplerate
         n_channels = input_file.channels
 
         s_start = int(np.round(sr_native * offset)) * n_channels
 
         if duration is None:
             s_end = np.inf
```

### Comparing `librosa-0.9.1/librosa/core/constantq.py` & `librosa-0.9.2/librosa/core/constantq.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/convert.py` & `librosa-0.9.2/librosa/core/convert.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/fft.py` & `librosa-0.9.2/librosa/core/fft.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/harmonic.py` & `librosa-0.9.2/librosa/core/harmonic.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/notation.py` & `librosa-0.9.2/librosa/core/notation.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/pitch.py` & `librosa-0.9.2/librosa/core/pitch.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/core/spectrum.py` & `librosa-0.9.2/librosa/core/spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     - ``np.abs(D[..., f, t])`` is the magnitude of frequency bin ``f``
       at frame ``t``, and
 
     - ``np.angle(D[..., f, t])`` is the phase of frequency bin ``f``
       at frame ``t``.
 
     The integers ``t`` and ``f`` can be converted to physical units by means
-    of the utility functions `frames_to_sample` and `fft_frequencies`.
+    of the utility functions `frames_to_samples` and `fft_frequencies`.
 
     Parameters
     ----------
     y : np.ndarray [shape=(..., n)], real-valued
         input signal. Multi-channel is supported.
 
     n_fft : int > 0 [scalar]
@@ -1164,16 +1164,26 @@
            [-4.342e-12, -1.543e+00, ..., -1.794e+00, -2.419e+00],
            [-3.142e+00, -3.142e+00, ...,  0.000e+00,  0.000e+00]],
           dtype=float32)
 
     """
 
     mag = np.abs(D)
+
+    # Prevent NaNs and return magnitude 0, phase 1+0j for zero
+    zeros_to_ones = mag == 0
+    mag_nonzero = mag + zeros_to_ones
+    # Compute real and imaginary separately, because complex division can
+    # produce NaNs when denormalized numbers are involved (< ~2e-39 for
+    # complex64, ~5e-309 for complex128)
+    phase = np.empty_like(D, dtype=util.dtype_r2c(D.dtype))
+    phase.real = D.real / mag_nonzero + zeros_to_ones
+    phase.imag = D.imag / mag_nonzero
+
     mag **= power
-    phase = np.exp(1.0j * np.angle(D))
 
     return mag, phase
 
 
 @deprecate_positional_args
 def phase_vocoder(D, *, rate, hop_length=None, n_fft=None):
     """Phase vocoder.  Given an STFT matrix D, speed up by a factor of ``rate``
@@ -1499,15 +1509,15 @@
         If callable, the reference value is computed as ``ref(S)``.
 
     amin : float > 0 [scalar]
         minimum threshold for ``abs(S)`` and ``ref``
 
     top_db : float >= 0 [scalar]
         threshold the output at ``top_db`` below the peak:
-        ``max(10 * log10(S)) - top_db``
+        ``max(10 * log10(S/ref)) - top_db``
 
     Returns
     -------
     S_db : np.ndarray
         ``S_db ~= 10 * log10(S) - 10 * log10(ref)``
 
     See Also
@@ -1629,15 +1639,16 @@
 
 
 @deprecate_positional_args
 @cache(level=30)
 def amplitude_to_db(S, *, ref=1.0, amin=1e-5, top_db=80.0):
     """Convert an amplitude spectrogram to dB-scaled spectrogram.
 
-    This is equivalent to ``power_to_db(S**2)``, but is provided for convenience.
+    This is equivalent to ``power_to_db(S**2, ref=ref**2, amin=amin**2, top_db=top_db)``,
+    but is provided for convenience.
 
     Parameters
     ----------
     S : np.ndarray
         input amplitude
 
     ref : scalar or callable
@@ -1648,15 +1659,15 @@
         If callable, the reference value is computed as ``ref(S)``.
 
     amin : float > 0 [scalar]
         minimum threshold for ``S`` and ``ref``
 
     top_db : float >= 0 [scalar]
         threshold the output at ``top_db`` below the peak:
-        ``max(20 * log10(S)) - top_db``
+        ``max(20 * log10(S/ref)) - top_db``
 
     Returns
     -------
     S_db : np.ndarray
         ``S`` measured in dB
 
     See Also
@@ -1694,15 +1705,15 @@
 @deprecate_positional_args
 @cache(level=30)
 def db_to_amplitude(S_db, *, ref=1.0):
     """Convert a dB-scaled spectrogram to an amplitude spectrogram.
 
     This effectively inverts `amplitude_to_db`::
 
-        db_to_amplitude(S_db) ~= 10.0**(0.5 * (S_db + log10(ref)/10))
+        db_to_amplitude(S_db) ~= 10.0**(0.5 * S_db/10 + log10(ref))
 
     Parameters
     ----------
     S_db : np.ndarray
         dB-scaled spectrogram
     ref : number > 0
         Optional reference power.
```

### Comparing `librosa-0.9.1/librosa/decompose.py` & `librosa-0.9.2/librosa/decompose.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/display.py` & `librosa-0.9.2/librosa/display.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/effects.py` & `librosa-0.9.2/librosa/effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,14 +441,17 @@
 
     # Convert to decibels and slice out the mse channel
     db = core.amplitude_to_db(mse[..., 0, :], ref=ref, top_db=None)
 
     # Aggregate everything but the time dimension
     if db.ndim > 1:
         db = np.apply_over_axes(aggregate, db, range(db.ndim - 1))
+        # Squeeze out leading singleton dimensions here
+        # We always want to keep the trailing dimension though
+        db = np.squeeze(db, axis=tuple(range(db.ndim - 1)))
 
     return db > -top_db
 
 
 @deprecate_positional_args
 def trim(
     y, *, top_db=60, ref=np.max, frame_length=2048, hop_length=512, aggregate=np.max
@@ -586,15 +589,15 @@
 
     # Stack the results back as an ndarray
     return edges.reshape((-1, 2))
 
 
 @deprecate_positional_args
 def preemphasis(y, *, coef=0.97, zi=None, return_zf=False):
-    """Pre-emphasize an audio signal with a first-order auto-regressive filter:
+    """Pre-emphasize an audio signal with a first-order differencing filter:
 
         y[n] -> y[n] - coef * y[n-1]
 
     Parameters
     ----------
     y : np.ndarray [shape=(..., n)]
         Audio signal. Multi-channel is supported.
```

### Comparing `librosa-0.9.1/librosa/feature/__init__.py` & `librosa-0.9.2/librosa/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/feature/inverse.py` & `librosa-0.9.2/librosa/feature/inverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         idx = np.arange(1, 1 + n_mfcc, dtype=mfcc.dtype)
         idx = expand_to(idx, ndim=mfcc.ndim, axes=-2)
         lifter_sine = 1 + lifter * 0.5 * np.sin(np.pi * idx / lifter)
 
         # raise a UserWarning if lifter array includes critical values
         if np.any(np.abs(lifter_sine) < np.finfo(lifter_sine.dtype).eps):
             warnings.warn(
-                message="lifter array includes critial values that may invoke underflow.",
+                message="lifter array includes critical values that may invoke underflow.",
                 category=UserWarning,
                 stacklevel=2,
             )
 
         # lifter mfcc values
         mfcc = mfcc / (lifter_sine + tiny(mfcc))
```

### Comparing `librosa-0.9.1/librosa/feature/rhythm.py` & `librosa-0.9.2/librosa/feature/rhythm.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/feature/spectral.py` & `librosa-0.9.2/librosa/feature/spectral.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     >>> librosa.display.specshow(librosa.amplitude_to_db(S, ref=np.max),
     ...                          y_axis='log', x_axis='time', ax=ax)
     >>> ax.plot(times, cent.T, label='Spectral centroid', color='w')
     >>> ax.legend(loc='upper right')
     >>> ax.set(title='log Power spectrogram')
     """
 
-    # input is time domain:y or spectrogam:s
+    # input is time domain:y or spectrogram:s
     #
 
     S, n_fft = _spectrogram(
         y=y,
         S=S,
         n_fft=n_fft,
         hop_length=hop_length,
@@ -1050,15 +1050,15 @@
         `librosa.reassigned_spectrogram`
 
     Returns
     -------
     coefficients : np.ndarray [shape=(..., order+1, t)]
         polynomial coefficients for each frame.
 
-        ``coeffecients[..., 0, :]`` corresponds to the highest degree (``order``),
+        ``coefficients[..., 0, :]`` corresponds to the highest degree (``order``),
 
         ``coefficients[..., 1, :]`` corresponds to the next highest degree (``order-1``),
 
         down to the constant term ``coefficients[..., order, :]``.
 
     Examples
     --------
```

### Comparing `librosa-0.9.1/librosa/feature/utils.py` & `librosa-0.9.2/librosa/feature/utils.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/filters.py` & `librosa-0.9.2/librosa/filters.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/onset.py` & `librosa-0.9.2/librosa/onset.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/segment.py` & `librosa-0.9.2/librosa/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,18 +165,18 @@
 
     Plot the feature and recurrence matrices
 
     >>> import matplotlib.pyplot as plt
     >>> fig, ax = plt.subplots(ncols=2, sharex=True, sharey=True)
     >>> imgsim = librosa.display.specshow(xsim, x_axis='s', y_axis='s',
     ...                          hop_length=hop_length, ax=ax[0])
-    >>> ax[0].set(title='Binary recurrence (symmetric)')
+    >>> ax[0].set(title='Binary cross-similarity (symmetric)')
     >>> imgaff = librosa.display.specshow(xsim_aff, x_axis='s', y_axis='s',
     ...                          cmap='magma_r', hop_length=hop_length, ax=ax[1])
-    >>> ax[1].set(title='Affinity recurrence')
+    >>> ax[1].set(title='Cross-affinity')
     >>> ax[1].label_outer()
     >>> fig.colorbar(imgsim, ax=ax[0], orientation='horizontal', ticks=[0, 1])
     >>> fig.colorbar(imgaff, ax=ax[1], orientation='horizontal')
     """
     data_ref = np.atleast_2d(data_ref)
     data = np.atleast_2d(data)
```

### Comparing `librosa-0.9.1/librosa/sequence.py` & `librosa-0.9.2/librosa/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1093,14 +1093,19 @@
 
     This implementation uses the standard Viterbi decoding algorithm
     for observation likelihood sequences, under the assumption that
     ``P[Obs(t) | State(t) = s]`` is proportional to
     ``P[State(t) = s | Obs(t)] / P[State(t) = s]``, where the denominator
     is the marginal probability of state ``s`` occurring as given by ``p_state``.
 
+    Note that because the denominator ``P[State(t) = s]`` is not explicitly
+    calculated, the resulting probabilities (or log-probabilities) are not
+    normalized.  If using the `return_logp=True` option (see below),
+    be aware that the "probabilities" may not sum to (and may exceed) 1.
+
     Parameters
     ----------
     prob : np.ndarray [shape=(..., n_states, n_steps), non-negative]
         ``prob[s, t]`` is the probability of state ``s`` conditional on
         the observation at time ``t``.
         Must be non-negative and sum to 1 along each column.
     transition : np.ndarray [shape=(n_states, n_states), non-negative]
@@ -1120,16 +1125,16 @@
     -------
     Either ``states`` or ``(states, logp)``:
     states : np.ndarray [shape=(..., n_steps,)]
         The most likely state sequence.
         If ``prob`` contains multiple input channels,
         then each channel is decoded independently.
     logp : scalar [float] or np.ndarray
-        If ``return_logp=True``, the log probability of ``states`` given
-        the observations.
+        If ``return_logp=True``, the (unnormalized) log probability
+        of ``states`` given the observations.
 
     See Also
     --------
     viterbi :
         Viterbi decoding from observation likelihoods
     viterbi_binary :
         Viterbi decoding for multi-label, conditional state likelihoods
@@ -1298,14 +1303,18 @@
     states to be mutually exclusive.  `viterbi_binary` is implemented by
     transforming the multi-label decoding problem to a collection
     of binary Viterbi problems (one for each *state* or label).
 
     The output is a binary matrix ``states[s, t]`` indicating whether each
     state ``s`` is active at time ``t``.
 
+    Like `viterbi_discriminative`, the probabilities of the optimal state sequences
+    are not normalized here.  If using the `return_logp=True` option (see below),
+    be aware that the "probabilities" may not sum to (and may exceed) 1.
+
     Parameters
     ----------
     prob : np.ndarray [shape=(..., n_steps,) or (..., n_states, n_steps)], non-negative
         ``prob[s, t]`` is the probability of state ``s`` being active
         conditional on the observation at time ``t``.
         Must be non-negative and less than 1.
 
@@ -1328,24 +1337,24 @@
         is assumed.
 
     p_init : np.ndarray [shape=(n_states,)]
         Optional: initial state distribution.
         If not provided, it is assumed to be uniform.
 
     return_logp : bool
-        If ``True``, return the log-likelihood of the state sequence.
+        If ``True``, return the (unnormalized) log-likelihood of the state sequences.
 
     Returns
     -------
     Either ``states`` or ``(states, logp)``:
     states : np.ndarray [shape=(..., n_states, n_steps)]
         The most likely state sequence.
     logp : np.ndarray [shape=(..., n_states,)]
-        If ``return_logp=True``, the log probability of each state activation
-        sequence ``states``
+        If ``return_logp=True``, the (unnormalized) log probability of each
+        state activation sequence ``states``
 
     See Also
     --------
     viterbi :
         Viterbi decoding from observation likelihoods
     viterbi_discriminative :
         Viterbi decoding for discriminative (mutually exclusive) state predictions
```

### Comparing `librosa-0.9.1/librosa/util/__init__.py` & `librosa-0.9.2/librosa/util/__init__.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/util/_nnls.py` & `librosa-0.9.2/librosa/util/_nnls.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/util/decorators.py` & `librosa-0.9.2/librosa/util/decorators.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/util/deprecation.py` & `librosa-0.9.2/librosa/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/util/example_data/index.json` & `librosa-0.9.2/librosa/util/example_data/index.json`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/util/example_data/registry.txt` & `librosa-0.9.2/librosa/util/example_data/registry.txt`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/util/files.py` & `librosa-0.9.2/librosa/util/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,20 @@
 
     >>> # Only get the first 10 files
     >>> files = librosa.util.find_files('~/Music', limit=10)
 
     >>> # Or last 10 files
     >>> files = librosa.util.find_files('~/Music', offset=-10)
 
+    >>> # Avoid including search patterns in the path string
+    >>> import glob
+    >>> directory = '~/[202206] Music'
+    >>> directory = glob.escape(directory)  # Escape the special characters
+    >>> files = librosa.util.find_files(directory)
+
     Parameters
     ----------
     directory : str
         Path to look for files
 
     ext : str or list of str
         A file extension or list of file extensions to include in the search.
```

### Comparing `librosa-0.9.1/librosa/util/matching.py` & `librosa-0.9.2/librosa/util/matching.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa/util/utils.py` & `librosa-0.9.2/librosa/util/utils.py`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/librosa.egg-info/PKG-INFO` & `librosa-0.9.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: librosa
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python module for audio and music processing
 Home-page: https://librosa.org
 Author: Brian McFee, librosa development team
 Author-email: brian.mcfee@nyu.edu
 License: ISC
 Project-URL: Documentation, https://librosa.org/doc
 Project-URL: Download, https://github.com/librosa/librosa/releases
 Project-URL: Source, https://github.com/librosa/librosa
 Project-URL: Tracker, https://github.com/librosa/librosa/issues
 Project-URL: Discussion forum, https://groups.google.com/g/librosa
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Framework :: Matplotlib
 Classifier: Programming Language :: Python :: 3
@@ -26,122 +25,215 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: display
 License-File: LICENSE.md
 
-librosa
-=======
+[![librosa logo](docs/img/librosa_logo_text.svg)](https://librosa.org/)
+
+# librosa
+
+
 A python package for music and audio analysis.  
 
 [![PyPI](https://img.shields.io/pypi/v/librosa.svg)](https://pypi.python.org/pypi/librosa)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/librosa/badges/version.svg)](https://anaconda.org/conda-forge/librosa)
 [![License](https://img.shields.io/pypi/l/librosa.svg)](https://github.com/librosa/librosa/blob/main/LICENSE.md)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.591533.svg)](https://doi.org/10.5281/zenodo.591533)
 
 [![CI](https://github.com/librosa/librosa/actions/workflows/ci.yml/badge.svg)](https://github.com/librosa/librosa/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/librosa/librosa/branch/main/graph/badge.svg?token=ULWnUHaIJC)](https://codecov.io/gh/librosa/librosa)
+[![Docs](https://github.com/librosa/librosa/actions/workflows/docs.yml/badge.svg)](https://github.com/librosa/librosa/actions/workflows/docs.yml)
+
+#  Table of Contents
+
+- [Documentation](#Documentation)
+- [Installation](#Installation)
+  - [Using PyPI](#using-pypi)
+  - [Using Anaconda](#using-anaconda)
+  - [Building From Source](#building-from-source)
+  - [Hints for Installation](#hints-for-the-installation)
+    - [`soundfile`](#soundfile)
+    - [`audioread` and MP3 support](#audioread-and-mp3-support)
+      - [Linux (`apt get`)](#linux-apt-get)
+      - [Linux (`yum`)](#linux-yum)
+      - [Mac](#mac)
+      - [Windows](#windows)
+- [Discussion](#discussion)
+- [Citing](#citing)
+
+---
+
+## Documentation
 
 
-Documentation
--------------
 See https://librosa.org/doc/ for a complete reference manual and introductory tutorials.
 
 The [advanced example gallery](https://librosa.org/doc/latest/advanced.html) should give you a quick sense of the kinds
 of things that librosa can do.
 
-Installation
-------------
+---
+
+[Back To Top ↥](#librosa)
+
+
+## Installation
+
+
+### Using PyPI
 
 The latest stable release is available on PyPI, and you can install it by saying
 ```
-pip install librosa
+python -m pip install librosa
 ```
 
-Anaconda users can install using ``conda-forge``:
+### Using Anaconda
+
+Anaconda users can install using ```conda-forge```:
 ```
 conda install -c conda-forge librosa
 ```
 
-To build librosa from source, say `python setup.py build`.
-Then, to install librosa, say `python setup.py install`.
-If all went well, you should be able to execute the demo scripts under `examples/`
-(OS X users should follow the installation guide given below).
+### Building from source
+
+To build librosa from source, say 
+```
+python setup.py build
+```
+Then, to install librosa, say 
+```
+python setup.py install
+```
+If all went well, you should be able to execute the following commands from a python console:
+```
+import librosa
+librosa.show_versions()
+```
+This should print out a description of your software environment, along with the installed versions of other packages used by librosa.
+
+📝 OS X users should follow the installation guide given below.
 
 Alternatively, you can download or clone the repository and use `pip` to handle dependencies:
 
 ```
 unzip librosa.zip
-pip install -e librosa
+python -m pip install -e librosa
 ```
 or
+
 ```
 git clone https://github.com/librosa/librosa.git
-pip install -e librosa
+python -m pip install -e librosa
 ```
 
 By calling `pip list` you should see `librosa` now as an installed package:
 ```
 librosa (0.x.x, /path/to/librosa)
 ```
 
+---
+
+[Back To Top ↥](#librosa)
+
 ### Hints for the Installation
 
 `librosa` uses `soundfile` and `audioread` to load audio files.
-Note that `soundfile` does not currently support MP3, which will cause librosa to
+
+📝 Note that `soundfile` does not currently support MP3, which will cause librosa to
 fall back on the `audioread` library.
 
-#### soundfile
+### `soundfile`
 
 If you're using `conda` to install librosa, then most audio coding dependencies (except MP3) will be handled automatically.
 
 If you're using `pip` on a Linux environment, you may need to install `libsndfile`
 manually.  Please refer to the [SoundFile installation documentation](https://pysoundfile.readthedocs.io/#installation) for details.
 
-#### audioread and MP3 support
+### `audioread` and MP3 support
 
 To fuel `audioread` with more audio-decoding power (e.g., for reading MP3 files),
 you may need to install either *ffmpeg* or *GStreamer*.
 
-*Note that on some platforms, `audioread` needs at least one of the programs to work properly.*
+📝*Note that on some platforms, `audioread` needs at least one of the programs to work properly.*
 
 If you are using Anaconda, install *ffmpeg* by calling
+
 ```
 conda install -c conda-forge ffmpeg
 ```
 
 If you are not using Anaconda, here are some common commands for different operating systems:
 
-* Linux (apt-get): `apt-get install ffmpeg` or `apt-get install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly`
-* Linux (yum): `yum install ffmpeg` or `yum install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly`
-* Mac: `brew install ffmpeg` or `brew install gstreamer`
-* Windows: download ffmpeg binaries from this [website](https://www.gyan.dev/ffmpeg/builds/) or gstreamer binaries from this [website](https://gstreamer.freedesktop.org/)
+- ####  Linux (`apt-get`): 
+
+```
+apt-get install ffmpeg
+```
+or
+ 
+```
+apt-get install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly
+```
+- #### Linux (`yum`):
+```
+yum install ffmpeg
+```
+or
+
+
+```
+yum install gstreamer1.0-plugins-base gstreamer1.0-plugins-ugly
+```
+
+- #### Mac: 
+```
+brew install ffmpeg
+```
+or
+
+```
+brew install gstreamer
+```
+
+- #### Windows: 
+
+download ffmpeg binaries from this [website](https://www.gyan.dev/ffmpeg/builds/) or gstreamer binaries from this [website](https://gstreamer.freedesktop.org/)
 
 For GStreamer, you also need to install the Python bindings with 
+
 ```
-pip install pygobject
+python -m pip install pygobject
 ```
 
-Discussion
-----------
+---
+
+[Back To Top ↥](#librosa)
+
+## Discussion
+
 
 Please direct non-development questions and discussion topics to our web forum at
 https://groups.google.com/forum/#!forum/librosa
 
+---
+
+[Back To Top ↥](#librosa)
+
+## Citing
 
-Citing
-------
 
 If you want to cite librosa in a scholarly work, there are two ways to do it.
 
 - If you are using the library for your work, for the sake of reproducibility, please cite
   the version you used as indexed at Zenodo:
 
     [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.591533.svg)](https://doi.org/10.5281/zenodo.591533)
 
 - If you wish to cite librosa for its design, motivation etc., please cite the paper
   published at SciPy 2015:
 
     McFee, Brian, Colin Raffel, Dawen Liang, Daniel PW Ellis, Matt McVicar, Eric Battenberg, and Oriol Nieto. "librosa: Audio and music signal analysis in python." In Proceedings of the 14th python in science conference, pp. 18-25. 2015.
 
+---
 
+[Back To Top ↥](#librosa)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `librosa-0.9.1/librosa.egg-info/SOURCES.txt` & `librosa-0.9.2/librosa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librosa-0.9.1/setup.cfg` & `librosa-0.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
-	audioread >= 2.1.5
+	audioread >= 2.1.9
 	numpy >= 1.17.0
 	scipy >= 1.2.0
 	scikit-learn >= 0.19.1
 	joblib >= 0.14
 	decorator >= 4.0.10
 	resampy >= 0.2.2
 	numba >= 0.45.1
@@ -59,15 +59,15 @@
 [options.package_data]
 librosa = util/example_data/*
 
 [options.extras_require]
 docs = 
 	numpydoc
 	sphinx != 1.3.1
-	sphinx_rtd_theme==0.5.*
+	sphinx_rtd_theme==1.*
 	numba < 0.50
 	matplotlib >= 3.3.0
 	sphinx-multiversion >= 0.2.3
 	sphinx-gallery >= 0.7
 	mir_eval >= 0.5
 	ipython >= 7.0
 	sphinxcontrib-svg2pdfconverter
```

