# Comparing `tmp/fave_syllabify-0.1.2.tar.gz` & `tmp/fave_syllabify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fave_syllabify-0.1.2.tar", max compression
+gzip compressed data, was "fave_syllabify-0.1.3.tar", max compression
```

## Comparing `fave_syllabify-0.1.2.tar` & `fave_syllabify-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-02-18 17:18:47.446023 fave_syllabify-0.1.2/LICENSE
--rw-r--r--   0        0        0     2372 2024-02-26 13:32:34.086907 fave_syllabify-0.1.2/README.md
--rw-r--r--   0        0        0      805 2024-02-26 13:04:12.569337 fave_syllabify-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      120 2024-02-25 22:28:40.885315 fave_syllabify-0.1.2/src/fave_syllabify/__init__.py
--rw-r--r--   0        0        0     5317 2024-02-26 12:01:22.162440 fave_syllabify-0.1.2/src/fave_syllabify/syllabify.py
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 fave_syllabify-0.1.2/setup.py
--rw-r--r--   0        0        0     2857 1970-01-01 00:00:00.000000 fave_syllabify-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-18 17:18:47.446023 fave_syllabify-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2372 2024-05-02 21:04:25.855091 fave_syllabify-0.1.3/README.md
+-rw-r--r--   0        0        0      805 2024-05-02 21:04:25.858873 fave_syllabify-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-02 21:04:25.859187 fave_syllabify-0.1.3/src/fave_syllabify/__init__.py
+-rw-r--r--   0        0        0     5322 2024-05-02 21:04:25.859524 fave_syllabify-0.1.3/src/fave_syllabify/syllabify.py
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 fave_syllabify-0.1.3/setup.py
+-rw-r--r--   0        0        0     2857 1970-01-01 00:00:00.000000 fave_syllabify-0.1.3/PKG-INFO
```

### Comparing `fave_syllabify-0.1.2/LICENSE` & `fave_syllabify-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fave_syllabify-0.1.2/README.md` & `fave_syllabify-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fave_syllabify-0.1.2/pyproject.toml` & `fave_syllabify-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "fave-syllabify"
-version = "0.1.2"
+version = "0.1.3"
 description = "Syllabify force-aligned textgrids"
 authors = ["JoFrhwld <JoFrhwld@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "fave_syllabify", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aligned-textgrid = "^0.6.3"
+aligned-textgrid = "^0.6.6"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 pytest-cov = "^4.1.0"
 coverage = "^7.4.3"
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `fave_syllabify-0.1.2/src/fave_syllabify/syllabify.py` & `fave_syllabify-0.1.3/src/fave_syllabify/syllabify.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,15 @@
         if n.fol.label == "coda":
             n.coda = n.fol.first
             n.fuse_rightwards(lambda x,y: x)
 
 
 def syllabify_tg(tg: AlignedTextGrid):
     """Syllabify an entire AlignedTextGrid
+    
     Args:
         tg (AlignedTextGrid): The textgrid to syllabify
     """
 
     tg_entry_classes = {
         c.__name__ 
         for gr in tg.entry_classes
```

### Comparing `fave_syllabify-0.1.2/setup.py` & `fave_syllabify-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['fave_syllabify']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aligned-textgrid>=0.6.3,<0.7.0']
+['aligned-textgrid>=0.6.6,<0.7.0']
 
 setup_kwargs = {
     'name': 'fave-syllabify',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Syllabify force-aligned textgrids',
     'long_description': '# fave-syllabify\n\n\n![](https://img.shields.io/badge/Lifecycle-Maturing-lightgreen@2x.png)\n![PyPI version](https://badge.fury.io/py/fave-syllabify.svg) [![Lint and\nTest](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-syllabify/actions/workflows/lint-and-test.yml/badge.svg)](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-syllabify/actions/workflows/lint-and-test.yml)\n[![Build\nDocs](https://github.com/Forced-Alignment-and-Vowel-Extraction/fave-syllabify/actions/workflows/build_docs.yml/badge.svg)](https://forced-alignment-and-vowel-extraction.github.io/fave-syllabify/)\n[![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-syllabify/graph/badge.svg?token=WDBJ0O9P6L)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/fave-syllabify)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10708119.svg)](https://doi.org/10.5281/zenodo.10708119)\n\nSyllabify a force-aligned TextGrid\n\n## Installation\n\n``` bash\npip install fave-syllabify\n```\n\n## Usage\n\nImport classes and functions\n\n``` python\nfrom aligned_textgrid import AlignedTextGrid, custom_classes\nfrom fave_syllabify import syllabify_tg\nfrom pathlib import Path\n```\n\nRead in a textgrid\n\n``` python\ntg = AlignedTextGrid(\n    textgrid_path=Path(\n        "docs",\n        "data",\n        "josef-fruehwald_speaker.TextGrid"\n    ),\n    entry_classes=custom_classes(\n        ["Word", "Phone"]\n    )\n)\n\nprint(tg)\n```\n\n    AlignedTextGrid with 1 groups named [\'group_0\'] each with [2] tiers. [[\'Word\', \'Phone\']]\n\nSyllabify the textgrid\n\n``` python\nsyllabify_tg(tg)\n\nprint(tg)\n```\n\n    AlignedTextGrid with 1 groups named [\'group_0\'] each with [4] tiers. [[\'Word\', \'Syllable\', \'SylPart\', \'Phone\']]\n\n### Exploring the syllabification\n\n``` python\nword_tier = tg.group_0.Word\nraindrops = word_tier[5]\n\nprint(raindrops.label)\n```\n\n    raindrops\n\nEach syllable is labelled with its stress.\n\n``` python\nprint([\n    syl.label \n    for syl in raindrops.contains\n])\n```\n\n    [\'syl-1\', \'syl-2\']\n\nEach syllable contains its constituent parts in a flat hierarchy\n(there’s no rhyme constituent).\n\n``` python\nsyl = raindrops.first.fol\nprint([\n    part.label\n    for part in syl.contains\n])\n```\n\n    [\'onset\', \'nucleus\', \'coda\']\n\nEach constituent contains its relevant phone.\n\n``` python\nonset = syl.onset\nprint([\n    phone.label\n    for phone in onset\n])\n```\n\n    [\'D\', \'R\']\n',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fave_syllabify-0.1.2/PKG-INFO` & `fave_syllabify-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fave-syllabify
-Version: 0.1.2
+Version: 0.1.3
 Summary: Syllabify force-aligned textgrids
 License: GPLv3
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aligned-textgrid (>=0.6.3,<0.7.0)
+Requires-Dist: aligned-textgrid (>=0.6.6,<0.7.0)
 Description-Content-Type: text/markdown
 
 # fave-syllabify
 
 
 ![](https://img.shields.io/badge/Lifecycle-Maturing-lightgreen@2x.png)
 ![PyPI version](https://badge.fury.io/py/fave-syllabify.svg) [![Lint and
```

