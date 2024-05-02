# Comparing `tmp/erlab-2.3.2.tar.gz` & `tmp/erlab-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.3.2.tar", last modified: Thu Apr 25 17:06:51 2024, max compression
+gzip compressed data, was "erlab-2.4.0.tar", last modified: Thu May  2 03:44:11 2024, max compression
```

## Comparing `erlab-2.3.2.tar` & `erlab-2.4.0.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.610054 erlab-2.3.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.562054 erlab-2.3.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.570054 erlab-2.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2200 2024-04-25 17:06:43.000000 erlab-2.3.2/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-25 17:06:43.000000 erlab-2.3.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-25 17:06:43.000000 erlab-2.3.2/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.570054 erlab-2.3.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-25 17:06:43.000000 erlab-2.3.2/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-25 17:06:43.000000 erlab-2.3.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-25 17:06:43.000000 erlab-2.3.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-25 17:06:43.000000 erlab-2.3.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-04-25 17:06:43.000000 erlab-2.3.2/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   119766 2024-04-25 17:06:48.000000 erlab-2.3.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-25 17:06:43.000000 erlab-2.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48058 2024-04-25 17:06:51.610054 erlab-2.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-25 17:06:43.000000 erlab-2.3.2/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5147 2024-04-25 17:06:43.000000 erlab-2.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.570054 erlab-2.3.2/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      495 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.574054 erlab-2.3.2/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    17632 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15196 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      224 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     4221 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.582054 erlab-2.3.2/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-25 17:06:43.000000 erlab-2.3.2/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.582054 erlab-2.3.2/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2604 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.586054 erlab-2.3.2/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    41262 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2598 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1291 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     9017 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    54332 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)    10710 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    26977 2024-04-25 17:06:44.000000 erlab-2.3.2/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      464 2024-04-25 17:06:44.000000 erlab-2.3.2/environment.yml
--rw-r--r--   0 root         (0) root         (0)     4689 2024-04-25 17:06:44.000000 erlab-2.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      315 2024-04-25 17:06:44.000000 erlab-2.3.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 17:06:51.610054 erlab-2.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.562054 erlab-2.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.586054 erlab-2.3.2/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-25 17:06:48.000000 erlab-2.3.2/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.586054 erlab-2.3.2/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      778 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25941 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    29991 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)     7133 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.590054 erlab-2.3.2/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5611 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.590054 erlab-2.3.2/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.590054 erlab-2.3.2/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10753 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9691 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6968 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12659 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20224 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    18225 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    10496 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10184 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.590054 erlab-2.3.2/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8481 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     5444 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.590054 erlab-2.3.2/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      231 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.594054 erlab-2.3.2/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      525 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14334 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21351 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    23024 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11793 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19282 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.594054 erlab-2.3.2/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19829 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.594054 erlab-2.3.2/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52047 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114573 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27450 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54842 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13599 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25433 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16051 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     2749 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54600 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.598054 erlab-2.3.2/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.598054 erlab-2.3.2/src/erlab/io/characterization/
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3091 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)    42722 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12251 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6998 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.598054 erlab-2.3.2/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3747 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     8166 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7667 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6806 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2533 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.598054 erlab-2.3.2/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.602053 erlab-2.3.2/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2113 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29615 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18641 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    39514 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    33231 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.602053 erlab-2.3.2/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-25 17:06:44.000000 erlab-2.3.2/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.606054 erlab-2.3.2/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48058 2024-04-25 17:06:51.000000 erlab-2.3.2/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4937 2024-04-25 17:06:51.000000 erlab-2.3.2/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 17:06:51.000000 erlab-2.3.2/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      502 2024-04-25 17:06:51.000000 erlab-2.3.2/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-25 17:06:51.000000 erlab-2.3.2/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.602053 erlab-2.3.2/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-25 17:06:44.000000 erlab-2.3.2/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-25 17:06:44.000000 erlab-2.3.2/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-25 17:06:44.000000 erlab-2.3.2/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.566054 erlab-2.3.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.606054 erlab-2.3.2/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5785 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4035 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.606054 erlab-2.3.2/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4497 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     6036 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_fit_models.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     1472 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/analysis/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 17:06:51.606054 erlab-2.3.2/tests/io/
--rw-r--r--   0 root         (0) root         (0)     9383 2024-04-25 17:06:44.000000 erlab-2.3.2/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.419917 erlab-2.4.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.371917 erlab-2.4.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.379917 erlab-2.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-05-02 03:44:03.000000 erlab-2.4.0/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-02 03:44:03.000000 erlab-2.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-02 03:44:03.000000 erlab-2.4.0/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.379917 erlab-2.4.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-05-02 03:44:03.000000 erlab-2.4.0/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-02 03:44:03.000000 erlab-2.4.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-02 03:44:03.000000 erlab-2.4.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-05-02 03:44:03.000000 erlab-2.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-02 03:44:03.000000 erlab-2.4.0/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   122940 2024-05-02 03:44:07.000000 erlab-2.4.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-05-02 03:44:03.000000 erlab-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48438 2024-05-02 03:44:11.419917 erlab-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-05-02 03:44:03.000000 erlab-2.4.0/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5147 2024-05-02 03:44:03.000000 erlab-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.379917 erlab-2.4.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.383917 erlab-2.4.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    17977 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15203 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.391917 erlab-2.4.0/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.391917 erlab-2.4.0/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.391917 erlab-2.4.0/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    41238 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)    12039 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54817 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    27564 2024-05-02 03:44:03.000000 erlab-2.4.0/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-02 03:44:03.000000 erlab-2.4.0/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     5353 2024-05-02 03:44:03.000000 erlab-2.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      315 2024-05-02 03:44:03.000000 erlab-2.4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 03:44:11.419917 erlab-2.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.371917 erlab-2.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.395917 erlab-2.4.0/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-02 03:44:07.000000 erlab-2.4.0/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.395917 erlab-2.4.0/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      792 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26105 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    30007 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)     7071 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.395917 erlab-2.4.0/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.399917 erlab-2.4.0/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.399917 erlab-2.4.0/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12739 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20223 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    18221 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    14968 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.399917 erlab-2.4.0/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5397 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.399917 erlab-2.4.0/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.403917 erlab-2.4.0/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      526 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14330 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21371 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23024 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11793 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19282 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.403917 erlab-2.4.0/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    20018 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.403917 erlab-2.4.0/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52053 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114641 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27909 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    57822 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25660 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16051 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    55581 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.403917 erlab-2.4.0/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.407917 erlab-2.4.0/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12313 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.407917 erlab-2.4.0/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     8166 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.407917 erlab-2.4.0/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.411917 erlab-2.4.0/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30448 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18686 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39760 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    37467 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.411917 erlab-2.4.0/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-05-02 03:44:03.000000 erlab-2.4.0/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.415917 erlab-2.4.0/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48438 2024-05-02 03:44:11.000000 erlab-2.4.0/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4937 2024-05-02 03:44:11.000000 erlab-2.4.0/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 03:44:11.000000 erlab-2.4.0/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-02 03:44:11.000000 erlab-2.4.0/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-02 03:44:11.000000 erlab-2.4.0/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.411917 erlab-2.4.0/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-02 03:44:03.000000 erlab-2.4.0/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-02 03:44:03.000000 erlab-2.4.0/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-02 03:44:03.000000 erlab-2.4.0/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.375917 erlab-2.4.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.411917 erlab-2.4.0/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5785 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.415917 erlab-2.4.0/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_fit_models.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 03:44:11.415917 erlab-2.4.0/tests/io/
+-rw-r--r--   0 root         (0) root         (0)     9385 2024-05-02 03:44:03.000000 erlab-2.4.0/tests/io/test_dataloader.py
```

### Comparing `erlab-2.3.2/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.4.0/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.4.0/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/.github/workflows/pr.yml` & `erlab-2.4.0/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/.github/workflows/release.yml` & `erlab-2.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/.gitignore` & `erlab-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/.pre-commit-config.yaml` & `erlab-2.4.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,14 @@
       - id: check-merge-conflict
       - id: mixed-line-ending
       - id: check-ast
 
   # Lint and format with ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.4.1
+    rev: v0.4.2
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
```

### Comparing `erlab-2.3.2/.readthedocs.yaml` & `erlab-2.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/CHANGELOG.md` & `erlab-2.4.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,77 @@
 # CHANGELOG
 
 
 
+## v2.4.0 (2024-05-02)
+
+### Chore
+
+* (**deps**) update dependencies ([`37c1b4b`](https://github.com/kmnhan/erlabpy/commit/37c1b4bf838eeaabeda9ee255fa22902f6ce955b))
+
+  Numbagg is now an optional dependency.
+
+### Documentation
+
+* improve documentation ([`8f23f99`](https://github.com/kmnhan/erlabpy/commit/8f23f9974672a8432ff1e6bd3fdc6ed01a82c937))
+
+* improve io documentation ([`4369d23`](https://github.com/kmnhan/erlabpy/commit/4369d23310c0ad91b41952d9ead4b87458fe107e))
+
+* fix PyQt version pinning to resolve build failures on Qt6.7 ([`433ee9e`](https://github.com/kmnhan/erlabpy/commit/433ee9ed13ea254c6d1e1c83531c9c89f9ff9698))
+
+### Feature
+
+* (**imagetool**) add method to update only the values ([`ca40fe4`](https://github.com/kmnhan/erlabpy/commit/ca40fe41a0320fd7843c86f95b68f8b6e19adca8))
+
+* add interpolation along a path ([`7366ec4`](https://github.com/kmnhan/erlabpy/commit/7366ec4db600617e585c724d05aafea387456cf2))
+
+  The `slice_along_path` function has been added to `analysis.interpolate`, which enables easy interpolation along a evenly spaced path that is specified by its vertices and step size. The path can have an arbitrary number of dimensions and points.
+
+### Fix
+
+* (**io**) remove direct display call in interactive summary ([`d44b3a5`](https://github.com/kmnhan/erlabpy/commit/d44b3a56aecfb054a38d944c5c8b7f45d362cf3b))
+
+  This was causing duplicated plots.
+
+* (**plotting**) add some validation checks to `plot_array` ([`2e0753c`](https://github.com/kmnhan/erlabpy/commit/2e0753c90ffbe6fdd05af210ac6a4dbfa9aba899))
+
+  The functions `plot_array` and `plot_array_2d` now checks if the input array coordinates are uniformly spaced. If they are not, a warning is issued and the user is informed that the plot may not be accurate.
+
+* (**plotting**) increase default colorbar size ([`3208399`](https://github.com/kmnhan/erlabpy/commit/32083990e9e77df6e94b2b0836bc1f9764cfaaf7))
+
+  The default `width` argument to `nice_colorbar` is changed to 8 points. This ensures visibility in subplots, especially when constrained layout is used.
+
+* delay interactive imports until called ([`ad15910`](https://github.com/kmnhan/erlabpy/commit/ad15910f921cb5ffffc388e7a5e02832935f8547))
+
+### Refactor
+
+* various cleanup ([`2b38397`](https://github.com/kmnhan/erlabpy/commit/2b383970b602507b6efedbf396f14d470db60d8f))
+
+  Improve docstring formatting and tweak linter settings
+
+### Style
+
+* remove % formatting ([`ae18a34`](https://github.com/kmnhan/erlabpy/commit/ae18a341f36542c2f39d72b0dd975dbe640c7e24))
+
+### Unknown
+
+* Merge pull request #30 from kmnhan/pre-commit-ci-update-config ([`a550367`](https://github.com/kmnhan/erlabpy/commit/a5503679cf4c432a6c01cc4c0715c21d77136a8b))
+
+  [pre-commit.ci] pre-commit autoupdate
+
+* Merge pull request #28 from kmnhan/dev-2.4 ([`5d1f8fc`](https://github.com/kmnhan/erlabpy/commit/5d1f8fc840a7a807c35b0915ac572fa3ec2bfb49))
+
+  2.4 Release
+
+* [pre-commit.ci] pre-commit autoupdate ([`3c351cc`](https://github.com/kmnhan/erlabpy/commit/3c351cc255dc31010b2c5fab2d134531f00a4dac))
+
+  updates:
+  - [github.com/astral-sh/ruff-pre-commit: v0.4.1 → v0.4.2](https://github.com/astral-sh/ruff-pre-commit/compare/v0.4.1...v0.4.2)
+
+
 ## v2.3.2 (2024-04-25)
 
 ### Chore
 
 * pin PyQt due to tests failing on Qt6.7 ([`9dee08c`](https://github.com/kmnhan/erlabpy/commit/9dee08cd8a9ac2ac16b9b9a1cd96ce537b7104cb))
 
 ### Fix
```

### Comparing `erlab-2.3.2/LICENSE` & `erlab-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/PKG-INFO` & `erlab-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.3.2
+Version: 2.4.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,46 +696,55 @@
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
 Requires-Dist: igor2>=0.5.6
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: lmfit!=1.3.0,>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: numba>=0.59.0
-Requires-Dist: numbagg>=0.8.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
 Requires-Dist: qtawesome>=1.3.1
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: uncertainties>=3.1.4
 Requires-Dist: varname>=0.13.0
 Requires-Dist: xarray>=2024.02.0
+Provides-Extra: complete
+Requires-Dist: erlab[dev,misc,perf,viz]; extra == "complete"
+Provides-Extra: viz
+Requires-Dist: cmasher; extra == "viz"
+Requires-Dist: cmocean; extra == "viz"
+Requires-Dist: colorcet; extra == "viz"
+Requires-Dist: hvplot; extra == "viz"
+Requires-Dist: ipywidgets; extra == "viz"
+Provides-Extra: perf
+Requires-Dist: numbagg>=0.8.1; extra == "perf"
+Requires-Dist: bottleneck>=1.3.8; extra == "perf"
+Provides-Extra: misc
+Requires-Dist: iminuit>=2.25.2; extra == "misc"
+Requires-Dist: csaps>=1.1.0; extra == "misc"
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: python-semantic-release; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: sphinx-qt-documentation; extra == "docs"
 Requires-Dist: pybtex; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: python-semantic-release; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Provides-Extra: viz
-Requires-Dist: cmasher; extra == "viz"
-Requires-Dist: cmocean; extra == "viz"
-Requires-Dist: colorcet; extra == "viz"
-Requires-Dist: hvplot; extra == "viz"
-Requires-Dist: ipywidgets; extra == "viz"
 
 <h1 align="center">
 ERLabPy
 </h1>
 <p align="center">
     <a href="https://pypi.org/project/erlab/" alt="Supported Python Versions">
         <img src="https://img.shields.io/pypi/pyversions/erlab?logo=python&logoColor=white" /></a>
```

### Comparing `erlab-2.3.2/PythonInterface.ipf` & `erlab-2.4.0/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/README.md` & `erlab-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/Makefile` & `erlab-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/environment.yml` & `erlab-2.4.0/docs/environment.yml`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,14 @@
   - sphinx-autodoc-typehints
   - sphinx-copybutton
   - sphinxcontrib-bibtex
   - pybtex
   - nbsphinx
   - furo
   - sphinx-design
-  - pyperclip
   - ipywidgets
   - pip:
     - pyqt6>=6.2.2
+    - PyQt6-Qt6<6.7.0
     - csaps
     - sphinx-qt-documentation
     - -e .
```

### Comparing `erlab-2.3.2/docs/make.bat` & `erlab-2.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/conf.py` & `erlab-2.4.0/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,17 +67,15 @@
 
 # -- Linkcode settings -------------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html
 
 
 # based on numpy doc/source/conf.py
 def linkcode_resolve(domain, info):
-    """
-    Determine the URL corresponding to Python object
-    """
+    """Determine the URL corresponding to Python object."""
     if domain != "py":
         return None
 
     modname = info["module"]
     fullname = info["fullname"]
 
     submod = sys.modules.get(modname)
@@ -119,51 +117,57 @@
 
 
 # -- Autosummary and autodoc settings ----------------------------------------
 
 autosummary_generate = True
 autosummary_generate_overwrite = True
 
-autodoc_inherit_docstrings = False
-autodoc_typehints = "description"
-autodoc_typehints_format = "short"
 autodoc_class_signature = "mixed"
-autodoc_member_order = "bysource"
+autodoc_member_order = "groupwise"
 autodoc_default_options = {
     "members": True,
     "undoc-members": True,
-    # "exclude-members":("sigDataChanged",),
     "show-inheritance": False,
 }
+autodoc_typehints = "description"
 autodoc_typehints_description_target = "documented"
+# autodoc_type_aliases = {}
+autodoc_typehints_format = "short"
+autodoc_preserve_defaults = True
+autodoc_inherit_docstrings = False
 
-# autodoc_type_aliases = {
-# "numpy.float64": "float",
-# "float64": "float",
-# }
 
 # -- Napoleon settings -------------------------------------------------------
 
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 # napoleon_include_init_with_doc = False
 # napoleon_include_private_with_doc = False
 napoleon_include_special_with_doc = True
 # napoleon_use_admonition_for_examples = False
-# napoleon_use_admonition_for_notes = False
+napoleon_use_admonition_for_notes = True
 # napoleon_use_admonition_for_references = False
-# napoleon_use_ivar = False
+napoleon_use_ivar = True
 napoleon_use_param = True
+napoleon_use_keyword = False
 # napoleon_use_rtype = True
 napoleon_preprocess_types = True
-# napoleon_type_aliases = {
-#     "array-like": "ndarray <numpy.ndarray>",
-#     "numpy.float64": "float",
-#     "float64": "float",
-# }
+
+napoleon_type_aliases = {
+    "np.float32": "float32",
+    "numpy.float32": "float32",
+    "np.float64": "float64",
+    "numpy.float64": "float64",
+    "xr.DataArray": "xarray.DataArray",
+    "array-like": "`array-like <numpy.typing.ArrayLike>`",
+    "array_like": "`array-like <numpy.typing.ArrayLike>`",
+    "ColorType": "`ColorType <matplotlib.typing.ColorType>`",
+    "RGBColorType": "`RGBColorType <matplotlib.typing.RGBColorType>`",
+    "RGBAColorType": "`RGBAColorType <matplotlib.typing.RGBAColorType>`",
+}
 napoleon_attr_annotations = True
 napoleon_custom_sections = [("Signals", "params_style")]
 
 # -- nbsphinx options --------------------------------------------------------
 
 nbsphinx_execute_arguments = [
     "--InlineBackend.figure_formats={'svg', 'pdf'}",
@@ -210,16 +214,17 @@
 
 @pybtex.style.template.node
 def top_level(children, data):
     return pybtex.style.template.sentence(sep=", ")[children].format_data(data)
 
 
 class APSStyle(pybtex.style.formatting.unsrt.Style):
-    """
-    APS style for BibTeX formatting, adapted from the conf.py file of the `mitiq
+    """APS style for BibTeX formatting.
+
+    Adapted from the conf.py file of the `mitiq
     library<https://github.com/unitaryfund/mitiq>`_.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.abbreviate_names = True
 
@@ -461,22 +466,22 @@
                 <svg stroke="currentColor" fill="currentColor" stroke-width="0" viewBox="0 0 16 16">
                     <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"></path>
                 </svg>
             """,
             "class": "",
         },
     ],
-    "light_css_variables": {
-        "color-brand-primary": "#6d50bf",
-        "color-brand-content": "#6d50bf",
-    },
-    "dark_css_variables": {
-        "color-brand-primary": "#a180ff",
-        "color-brand-content": "#a180ff",
-    },
+    # "light_css_variables": {
+    #     "color-brand-primary": "#6d50bf",
+    #     "color-brand-content": "#6d50bf",
+    # },
+    # "dark_css_variables": {
+    #     "color-brand-primary": "#a180ff",
+    #     "color-brand-content": "#a180ff",
+    # },
 }
 
 # -- LaTeX options -----------------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#latex-options
 
 latex_engine = "lualatex"
 latex_show_pagerefs = True
```

### Comparing `erlab-2.3.2/docs/source/contributing.rst` & `erlab-2.4.0/docs/source/contributing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
       The ``editable_mode=compat`` setting enables static analysis tools to work with
       the package. See `this issue <https://github.com/pypa/setuptools/issues/3518>`_
       for more information.
 
    .. code-block:: sh
 
-     pip install -e . --config-settings editable_mode=compat
+     pip install -e ".[dev]" --config-settings editable_mode=compat
 
 
 Updating the editable installation
 ----------------------------------
 
 * For minor updates with editable installs, it is sufficient to just :ref:`update the
   main branch <update-main-branch>`.
```

### Comparing `erlab-2.3.2/docs/source/getting-started.rst` & `erlab-2.4.0/docs/source/getting-started.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 The recommended way to install ERLabPy is via conda. If you do not have conda installed,
 follow the :ref:`installation instructions <Installing conda>`. Once you have a working
 conda environment, you can install ERLabPy with the conda command line tool: ::
 
   conda install -c conda-forge erlab
 
+Add any `optional dependencies`_ you want to install to the command above.
+
 .. hint::
 
   If you are using macOS, you might experience degraded performance with the
   default BLAS and LAPACK libraries. For Apple Silicon macs, use `Accelerate
   <https://developer.apple.com/accelerate/>`_: ::
 
     conda install "libblas=*=*accelerate"
@@ -27,15 +29,22 @@
 
   To prevent conda from switching back to the default libraries, see the
   `conda-forge documentation
   <https://conda-forge.org/docs/maintainer/knowledge_base/#switching-blas-implementation>`_.
 
 If you don’t use conda, you can install ERLabPy with pip: ::
 
-  pip install erlab
+  python -m pip install erlab
+
+Optional dependency groups can be installed with the following commands: ::
+
+  python -m pip install erlab[viz]       # Install optional dependencies for visualization
+  python -m pip install erlab[perf]      # Install optional dependencies for performance
+  python -m pip install erlab[misc]      # Install miscellaneous optional dependencies
+  python -m pip install erlab[complete]  # Install all optional dependencies
 
 If you wish to install ERLabPy from source, see the :doc:`contributing`.
 
 Dependencies
 ============
 
 ERLabPy is installed with many different python libraries. Some key packages and
@@ -66,52 +75,61 @@
 ERLabPy also requires a Qt library such as PyQt5, PyQt6, PySide2, or PySide6. To
 ensure compatibility and keep the namespace clean, ERLabPy imports Qt bindings
 from `qtpy <https://github.com/spyder-ide/qtpy>`_, which will automatically
 select the appropriate library based on what is installed.
 
 See the :doc:`user-guide/index` to start using ERLabPy!
 
-Notes on compatibility
-----------------------
-
-- ERLabPy is tested on Python 3.11 and 3.12. It is not guaranteed to work on older
-  versions of Python.
-- There are some `known compatibility issues
-  <https://github.com/kmnhan/erlabpy/issues/17>`_ with PyQt5 and PySide2, so it is
-  recommended to use the newer PyQt6 or PySide6 if possible.
-- If you meet any unexpected behaviour while using IPython's `autoreload extension
-  <https://ipython.readthedocs.io/en/stable/config/extensions/autoreload.html>`_, try
-  excluding the following modules: ::
-
-    %aimport -erlab.io.dataloader -erlab.accessors
+.. _optional dependencies:
 
 Optional dependencies
 ---------------------
 
-The following packages are optional dependencies that are not installed by
-default. They are used in only specific functions, or is not used at all but is
-listed just for convenience.
+The following packages are optional dependencies that are not installed by default. They
+are only used in specific functions, or is not used at all but is listed just for
+convenience.
 
 .. list-table::
     :header-rows: 1
     :stub-columns: 1
     :widths: auto
 
     * - Package
       - Description
     * - `csaps <https://github.com/espdev/csaps>`_
       - Multidimensional smoothing splines
+    * - `ipywidgets <https://github.com/jupyter-widgets/ipywidgets>`_
+      - Interactive widgets
     * - `hvplot <https://github.com/holoviz/hvplot>`_ and `bokeh
         <https://github.com/bokeh/bokeh>`_
       - Interactive plotting
     * - `cmasher <https://cmasher.readthedocs.io>`_,
         `cmocean <https://matplotlib.org/cmocean/>`_, and
         `colorcet <https://colorcet.holoviz.org>`_
       - More colormaps!
-
-For a full list of dependencies and optional dependencies, take a look at the ``[project]`` and ``[project.optional-dependencies]`` section in
-`pyproject.toml <https://github.com/kmnhan/erlabpy/blob/main/pyproject.toml>`_:
+    * - `numbagg <https://github.com/numbagg/numbagg>`_ and `bottleneck
+        <https://github.com/pydata/bottleneck>`_
+      - Fast multidimensional aggregation, accelerates xarray
+
+For a full list of dependencies and optional dependencies, take a look at the
+``[project]`` and ``[project.optional-dependencies]`` section in `pyproject.toml
+<https://github.com/kmnhan/erlabpy/blob/main/pyproject.toml>`_:
 
 .. literalinclude:: ../../pyproject.toml
    :language: toml
    :start-at: dependencies = [
    :end-before: [project.urls]
+
+
+Notes on compatibility
+----------------------
+
+- ERLabPy is tested on Python 3.11 and 3.12. It is not guaranteed to work on older
+  versions of Python.
+- There are some `known compatibility issues
+  <https://github.com/kmnhan/erlabpy/issues/17>`_ with PyQt5 and PySide2, so it is
+  recommended to use the newer PyQt6 or PySide6 if possible.
+- If you meet any unexpected behaviour while using IPython's `autoreload extension
+  <https://ipython.readthedocs.io/en/stable/config/extensions/autoreload.html>`_, try
+  excluding the following modules: ::
+
+    %aimport -erlab.io.dataloader -erlab.accessors
```

### Comparing `erlab-2.3.2/docs/source/images/flowchart_multiple.pdf` & `erlab-2.4.0/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/images/flowchart_single.pdf` & `erlab-2.4.0/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/images/imagetool_dark.png` & `erlab-2.4.0/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/images/imagetool_light.png` & `erlab-2.4.0/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/images/ktool_1_dark.png` & `erlab-2.4.0/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/images/ktool_1_light.png` & `erlab-2.4.0/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/images/ktool_2_dark.png` & `erlab-2.4.0/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/images/ktool_2_light.png` & `erlab-2.4.0/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/index.rst` & `erlab-2.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/pyplots/norms.py` & `erlab-2.4.0/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/reference.rst` & `erlab-2.4.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/refs.bib` & `erlab-2.4.0/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.4.0/docs/source/user-guide/curve-fitting.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999328181565024%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [4]}}, 30: {'source': {insert: [(5, '    "*

 * *            "p0_center=-0.6,\\n')], delete: [5]}}, 60: {'source': {insert: [(9, '    "*

 * *            "p0_center=-0.6,\\n')], delete: [9]}}}"}*

```diff
@@ -41,15 +41,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import erlab.plotting.erplot as eplt\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import xarray as xr\n",
-                "\n",
                 "from erlab.io.exampledata import generate_data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -419,15 +418,15 @@
             "outputs": [],
             "source": [
                 "from erlab.analysis.fit.models import MultiPeakModel\n",
                 "\n",
                 "model = MultiPeakModel(npeaks=4, peak_shapes=[\"lorentzian\"], fd=False, convolve=True)\n",
                 "\n",
                 "params = model.make_params(\n",
-                "    p0_center=-0.59,\n",
+                "    p0_center=-0.6,\n",
                 "    p1_center=-0.45,\n",
                 "    p2_center=0.45,\n",
                 "    p3_center=0.6,\n",
                 "    p0_width=0.02,\n",
                 "    p1_width=0.02,\n",
                 "    p2_width=0.02,\n",
                 "    p3_width=0.02,\n",
@@ -991,15 +990,15 @@
                 "\n",
                 "model = MultiPeakModel(npeaks=4, peak_shapes=[\"lorentzian\"], fd=False, convolve=True)\n",
                 "\n",
                 "m = Minuit.from_lmfit(\n",
                 "    model,\n",
                 "    mdc,\n",
                 "    mdc.kx,\n",
-                "    p0_center=-0.59,\n",
+                "    p0_center=-0.6,\n",
                 "    p1_center=-0.45,\n",
                 "    p2_center=0.45,\n",
                 "    p3_center=0.6,\n",
                 "    p0_width=0.02,\n",
                 "    p1_width=0.02,\n",
                 "    p2_width=0.02,\n",
                 "    p3_width=0.02,\n",
```

### Comparing `erlab-2.3.2/docs/source/user-guide/imagetool.rst` & `erlab-2.4.0/docs/source/user-guide/imagetool.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/user-guide/index.rst` & `erlab-2.4.0/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/user-guide/indexing.ipynb` & `erlab-2.4.0/docs/source/user-guide/indexing.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615024250440918%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'dat = generate_data(seed=1).T')], delete: [2]}}, 14: "*

 * *            "{'source': {insert: [(15, 'In addition to the `powerful interpolation methods\\n'), "*

 * *            "(16, '<https://docs.xarray.dev/en/latest/user-guide/interpolation.html>`_ provided "*

 * *            "by\\n'), (17, ':mod:`xarray`, ERLabPy provides a convenient way to interpolate data "*

 * *            "along an arbitrary\\n'), (18, 'path.\\n'), (20, 'Consider a Γ-M-K-Γ high symmetry "*

 * *            "path giv […]*

```diff
@@ -43,15 +43,15 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from erlab.io.exampledata import generate_data\n",
                 "\n",
-                "dat = generate_data(seed=1)"
+                "dat = generate_data(seed=1).T"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "082ec477",
             "metadata": {
@@ -224,21 +224,101 @@
                 "   This part of the user guide is still under construction. For now, see\n",
                 "   :mod:`erlab.analysis.mask`. For the full list of packages and modules provided by\n",
                 "   ERLabPy, see :doc:`../reference`.\n",
                 "\n",
                 "Interpolation\n",
                 "-------------\n",
                 "\n",
-                ".. admonition:: Work in Progress\n",
-                "   :class: warning\n",
+                "In addition to the `powerful interpolation methods\n",
+                "<https://docs.xarray.dev/en/latest/user-guide/interpolation.html>`_ provided by\n",
+                ":mod:`xarray`, ERLabPy provides a convenient way to interpolate data along an arbitrary\n",
+                "path.\n",
+                "\n",
+                "Consider a \u0393-M-K-\u0393 high symmetry path given as a list of kx and ky coordinates:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4ab13824",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import erlab.plotting.erplot as eplt\n",
+                "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
+                "\n",
+                "a = 6.97\n",
+                "kx = [0, 2 * np.pi / (a * np.sqrt(3)), 2 * np.pi / (a * np.sqrt(3)), 0]\n",
+                "ky = [0, 0, 2 * np.pi / (a * 3), 0]\n",
+                "\n",
                 "\n",
-                "   This part of the user guide is still under construction. For now, please refer to the\n",
-                "   `interpolation section of the xarray user guide\n",
-                "   <https://docs.xarray.dev/en/latest/user-guide/interpolation.html>`_. For the full\n",
-                "   list of packages and modules provided by ERLabPy, see :doc:`../reference`."
+                "dat.qsel(eV=-0.2).qplot(aspect=\"equal\", cmap=\"Greys\")\n",
+                "plt.plot(kx, ky, \"o-\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "be5e2a2d",
+            "metadata": {},
+            "source": [
+                "To interpolate the data along this path with a step of 0.01 \u00c5$^{-1}$, we can use the following code:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bf4ec3c2",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import erlab.analysis as era\n",
+                "\n",
+                "dat_sliced = era.interpolate.slice_along_path(\n",
+                "    dat, vertices={\"kx\": kx, \"ky\": ky}, step_size=0.01\n",
+                ")\n",
+                "dat_sliced"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "84418499",
+            "metadata": {},
+            "source": [
+                "We can see that the data has been interpolated along the path. The new coordinate `path` contains the distance along the path, and the dimensions `kx` and `ky` are now expressed in terms of `path`.\n",
+                "\n",
+                "The distance along the path can be calculated as the sum of the distances between consecutive points in the path."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c00bb21c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dat_sliced.plot(cmap=\"Greys\")\n",
+                "eplt.fermiline()\n",
+                "\n",
+                "# Distance between each pair of consecutive points\n",
+                "distances = np.linalg.norm(np.diff(np.vstack([kx, ky]), axis=-1), axis=0)\n",
+                "seg_coords = np.concatenate(([0], np.cumsum(distances)))\n",
+                "\n",
+                "plt.xticks(seg_coords, labels=[\"\u0393\", \"M\", \"K\", \"\u0393\"])\n",
+                "plt.xlim(0, seg_coords[-1])\n",
+                "for seg in seg_coords[1:-1]:\n",
+                "    plt.axvline(seg, ls=\"--\", c=\"k\", lw=1)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "5a9036d9",
+            "metadata": {},
+            "source": [
+                "You will learn more about plotting in the next section."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -250,13 +330,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.8"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `erlab-2.3.2/docs/source/user-guide/io.ipynb` & `erlab-2.4.0/docs/source/user-guide/io.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999605263157895%*

 * *Differences: {"'cells'": "{12: {'source': {insert: [(46, '    }\\n'), (47, '    # Any additional metadata you "*

 * *            "want to add to the data. Note that attributes defined\\n'), (48, '    # here will not "*

 * *            "be transformed into coordinates. If you wish to promote some fixed\\n'), (49, '    # "*

 * *            "attributes to coordinates, add them to additional_coords.\\n'), (50, '\\n'), (51, "*

 * *            "'    additional_coords = {}\\n'), (52, '    # Additional non-dimension coordinates to "*

 * *            "b […]*

```diff
@@ -673,15 +673,22 @@
                 "    )\n",
                 "    # Attributes to be used as coordinates. Place all attributes that we don't want to\n",
                 "    # lose when merging multiple file scans here.\n",
                 "\n",
                 "    additional_attrs = {\n",
                 "        \"configuration\": 1,  # Experimental geometry. Required for momentum conversion\n",
                 "        \"sample_workfunction\": 4.3,\n",
-                "    }  # Any additional metadata you want to add to the data\n",
+                "    }\n",
+                "    # Any additional metadata you want to add to the data. Note that attributes defined\n",
+                "    # here will not be transformed into coordinates. If you wish to promote some fixed\n",
+                "    # attributes to coordinates, add them to additional_coords.\n",
+                "\n",
+                "    additional_coords = {}\n",
+                "    # Additional non-dimension coordinates to be added to the data, for instance the\n",
+                "    # photon energy for lab-based ARPES.\n",
                 "\n",
                 "    skip_validate = False\n",
                 "\n",
                 "    always_single = False\n",
                 "\n",
                 "    def identify(self, num, data_dir):\n",
                 "        coord_dict = {}\n",
```

### Comparing `erlab-2.3.2/docs/source/user-guide/kconv.ipynb` & `erlab-2.4.0/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/docs/source/user-guide/plotting.ipynb` & `erlab-2.4.0/docs/source/user-guide/plotting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956715593434344%*

 * *Differences: {"'cells'": "{17: {'source': {insert: [(2, 'Suppose we want to plot constant energy surfaces at "*

 * *            'specific binding energies, say, at `[-0.4, -0.2, 0.0]`. We could create three '*

 * *            "subplots and iterate over the axes.')], delete: [2]}}, 19: {'metadata': {'vscode': "*

 * *            "OrderedDict([('languageId', 'raw')])}, 'source': ['Here, we plotted each constant "*

 * *            "energy surface with :func:`plot_array\\n', '<erlab.plotting.general.plot_array>`. To "*

 * *            "remove the du […]*

```diff
@@ -273,56 +273,71 @@
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
                 "What if we want to plot multiple slices at once? We should create subplots to place the slices. *plt.subplots* is very useful in managing multiple axes and figures. If you are unfamiliar with the syntax, visit the [relevant matplotlib documentation](https://matplotlib.org/stable/gallery/subplots_axes_and_figures/subplots_demo.html).\n",
                 "\n",
-                "Suppose we want to plot constant energy surfaces at specific binding energies, say, at `[-0.4, -0.2, 0.0]`. We could create three subplots and iterate over the list, plotting each slice on each subplot. We would also want to label each plot with their binding energy. "
+                "Suppose we want to plot constant energy surfaces at specific binding energies, say, at `[-0.4, -0.2, 0.0]`. We could create three subplots and iterate over the axes."
             ]
         },
         {
-            "cell_type": "raw",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "editable": true,
-                "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
+            "outputs": [],
             "source": [
-                "We use three functions from ERLabPy to achieve this:\n",
-                ":func:`plot_array <erlab.plotting.general.plot_array>`\\ ,\n",
-                ":func:`label_subplot_properties <erlab.plotting.annotations.label_subplot_properties>`\\ , and\n",
-                ":func:`clean_labels <erlab.plotting.erplot.clean_labels>`\\ ."
+                "energies = [-0.4, -0.2, 0.0]\n",
+                "\n",
+                "fig, axs = plt.subplots(1, 3, layout=\"compressed\", sharey=True)\n",
+                "for energy, ax in zip(energies, axs):\n",
+                "    const_energy_surface = dat.qsel(eV=energy)\n",
+                "    eplt.plot_array(const_energy_surface, ax=ax, gamma=0.5, aspect=\"equal\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "raw",
             "metadata": {
                 "editable": true,
+                "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
-                "tags": []
+                "tags": [],
+                "vscode": {
+                    "languageId": "raw"
+                }
             },
+            "source": [
+                "Here, we plotted each constant energy surface with :func:`plot_array\n",
+                "<erlab.plotting.general.plot_array>`. To remove the duplicated y axis labels and add\n",
+                "some annotations, we can use :func:`clean_labels <erlab.plotting.erplot.clean_labels>`\n",
+                "and :func:`label_subplot_properties\n",
+                "<erlab.plotting.annotations.label_subplot_properties>`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
             "outputs": [],
             "source": [
-                "energies = [-0.4, -0.2, 0.0]\n",
-                "\n",
                 "fig, axs = plt.subplots(1, 3, layout=\"compressed\", sharey=True)\n",
-                "\n",
                 "for energy, ax in zip(energies, axs):\n",
                 "    const_energy_surface = dat.qsel(eV=energy)\n",
                 "    eplt.plot_array(const_energy_surface, ax=ax, gamma=0.5, aspect=\"equal\")\n",
                 "\n",
                 "eplt.clean_labels(axs)  # removes shared y labels\n",
-                "eplt.label_subplot_properties(axs, values=dict(Eb=energies))  # annotates energy"
+                "eplt.label_subplot_properties(axs, values={\"Eb\": energies})  # annotates energy"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
@@ -395,15 +410,17 @@
                 "fig, axs = eplt.plot_slices([dat], ky=[0.0, 0.1, 0.3], gamma=0.5, figsize=(6, 2))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Here, we notice that the first two plots slices through regions with less spectral weight, so the color across the three subplots are not on the same scale. This may be misleading in some occasions where intensity across different slices are important. Luckily, we have a function that can unify the color limits across multiple axes. The same effect can be achieved by passing on `same_limits=True` to `plot_slices`."
+                "Here, we notice that the first two plots slices through regions with less spectral weight, so the color across the three subplots are not on the same scale. This may be misleading in some occasions where intensity across different slices are important. Luckily, we have a function that can unify the color limits across multiple axes.\n",
+                "\n",
+                "The same effect can be achieved by passing on `same_limits=True` to `plot_slices`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "scrolled": true
@@ -424,15 +441,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, axs = eplt.plot_slices([dat], ky=[0.0, 0.1, 0.3], gamma=0.5, figsize=(6, 2))\n",
-                "eplt.unify_clim(axs, target=axs[0, 1])"
+                "eplt.unify_clim(axs, target=axs.flat[1])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
```

### Comparing `erlab-2.3.2/pyproject.toml` & `erlab-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,46 +24,51 @@
 dependencies = [
     "h5netcdf>=1.2.0",
     "igor2>=0.5.6",
     "joblib>=1.3.2",
     "lmfit>=1.2.0,!=1.3.0",
     "matplotlib>=3.8.0",
     "numba>=0.59.0",
-    "numbagg>=0.8.1",
     "numpy>=1.26.0",
     "pyperclip>=1.8.2",
     "pyqtgraph>=0.13.1",
     "qtawesome>=1.3.1",
     "qtpy>=2.4.1",
     "scipy>=1.12.0",
     "tqdm>=4.66.2",
     "uncertainties>=3.1.4",
     "varname>=0.13.0",
     "xarray>=2024.02.0",
 ]
 
 [project.optional-dependencies]
+complete = ["erlab[viz,perf,misc,dev]"]
+viz = ["cmasher", "cmocean", "colorcet", "hvplot", "ipywidgets"]
+perf = ["numbagg>=0.8.1", "bottleneck>=1.3.8"]
+misc = ["iminuit>=2.25.2", "csaps>=1.1.0"]
+dev = [
+    "mypy",
+    "pre-commit",
+    "pytest-xdist",
+    "pytest",
+    "python-semantic-release",
+    "ruff",
+]
 docs = [
     "sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-copybutton",
     "sphinxcontrib-bibtex",
+    "sphinx-qt-documentation",
     "pybtex",
     "nbsphinx",
     "furo",
     "sphinx-design",
 ]
-dev = [
-    "pytest",
-    "pytest-xdist",
-    "python-semantic-release",
-    "ruff",
-    "pre-commit",
-]
-viz = ["cmasher", "cmocean", "colorcet", "hvplot", "ipywidgets"]
+
 
 [project.urls]
 Documentation = "https://erlabpy.readthedocs.io"
 Repository = "https://github.com/kmnhan/erlabpy.git"
 Issues = "https://github.com/kmnhan/erlabpy/issues"
 Changelog = "https://github.com/kmnhan/erlabpy/blob/main/CHANGELOG.md"
 
@@ -128,43 +133,54 @@
 
 [tool.ruff]
 line-length = 88
 indent-width = 4
 
 [tool.ruff.lint]
 select = [
+    "F",
     "E4",
     "E7",
     "E9",
-    "F",
+    "W",
+    "I",
+    "D",
+    "UP",
     "B",
     "C4",
     "FA",
     "ICN",
     "PIE",
     "PT",
     "Q",
     "RSE",
     "TID",
     "TCH",
+    "INT",
+    # "ARG",
     # "PTH",
     # "FIX",
     "TRY",
     "FLY",
     "NPY",
     "PERF",
+    # "FURB",
     "RUF",
 ]
 ignore = [
     "ICN001", # Import conventions
     "TRY003", # Long exception messages
+    "D100",   # Missing docstring in public module
+    "D101",   # Missing docstring in public class
+    "D102",   # Missing docstring in public method
+    "D103",   # Missing docstring in public function
+    "D104",   # Missing docstring in public package
+    "D105",   # Missing docstring in magic method
 ]
-extend-select = [
-    "UP", # pyupgrade
-]
+extend-select = []
 allowed-confusables = [
     "×",
     "−",
     "𝑎",
     "𝒂",
     "𝑏",
     "𝒃",
@@ -175,14 +191,17 @@
     "𝛼",
     "γ",
     "𝛾",
     "ν",
     "α",
 ]
 
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
 line-ending = "auto"
 docstring-code-format = true
 docstring-code-line-length = "dynamic"
@@ -197,20 +216,23 @@
 
 [tool.mypy]
 plugins = ["numpy.typing.mypy_plugin"]
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 allow_redefinition = true
+check_untyped_defs = false
 exclude = [
     "^docs/",
     "^tests/",
     "_deprecated/",
     "interactive/fermiedge.py",
-    "io/",
+    "interactive/bzplot.py",
+    "interactive/curvefittingtool.py",
+    "io/plugins/",
 ]
 
 [[tool.mypy.overrides]]
 module = [
     "astropy.*",
     "h5netcdf.*",
     "igor2.*",
```

### Comparing `erlab-2.3.2/src/erlab/accessors/__init__.py` & `erlab-2.4.0/src/erlab/accessors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 .. autosummary::
    :toctree: generated
 
    utils
    kspace
    fit
 
-"""
+"""  # noqa: D205
 
 __all__ = [
+    "ImageToolAccessor",
     "ModelFitDataArrayAccessor",
     "ModelFitDatasetAccessor",
-    "ParallelFitDataArrayAccessor",
     "MomentumAccessor",
     "OffsetView",
-    "ImageToolAccessor",
+    "ParallelFitDataArrayAccessor",
     "PlotAccessor",
     "SelectionAccessor",
 ]
 
 from erlab.accessors.fit import (
     ModelFitDataArrayAccessor,
     ModelFitDatasetAccessor,
```

### Comparing `erlab-2.3.2/src/erlab/accessors/fit.py` & `erlab-2.4.0/src/erlab/accessors/fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "ParallelFitDataArrayAccessor",
 ]
 
 import copy
 import itertools
 import warnings
 from collections.abc import Hashable, Iterable, Mapping, Sequence
-from typing import TYPE_CHECKING, Any, Literal
+from typing import TYPE_CHECKING, Any, Literal, cast
 
 import joblib
 import lmfit
 import numpy as np
 import tqdm.auto
 import xarray as xr
 
@@ -41,19 +41,18 @@
     to_broadcast = {}
     for k, v in d.items():
         if isinstance(v, xr.DataArray | xr.Dataset):
             to_broadcast[k] = v
         else:
             to_broadcast[k] = xr.DataArray(v)
 
-    for k, v in zip(
-        to_broadcast.keys(), xr.broadcast(*to_broadcast.values()), strict=True
-    ):
-        d[k] = v
-    return d
+    d = dict(
+        zip(to_broadcast.keys(), xr.broadcast(*to_broadcast.values()), strict=True)
+    )
+    return cast(dict[str, xr.DataArray], d)
 
 
 def _concat_along_keys(d: dict[str, xr.DataArray], dim_name: str) -> xr.DataArray:
     return xr.concat(d.values(), d.keys()).rename(concat_dim=dim_name)
 
 
 def _parse_params(
@@ -371,15 +370,17 @@
             y = Y.ravel()
 
             if skipna:
                 mask = np.all([np.any(~np.isnan(x), axis=0), ~np.isnan(y)], axis=0)
                 x = x[:, mask]
                 y = y[mask]
                 if not len(y):
-                    modres = lmfit.model.ModelResult(model, model.make_params(), data=y)
+                    modres: lmfit.model.ModelResult = lmfit.model.ModelResult(
+                        model, model.make_params(), data=y
+                    )
                     modres.success = False
                     return popt, perr, pcov, stats, data, best, modres
             else:
                 mask = np.full_like(y, True)
 
             x = np.squeeze(x)
 
@@ -413,35 +414,39 @@
                         warnings.warn(
                             f"`guess` is not implemented for {model}, "
                             "using supplied initial parameters",
                             stacklevel=1,
                         )
                         initial_params = model.make_params().update(initial_params)
             try:
-                modres: lmfit.model.ModelResult = model.fit(
+                modres = model.fit(
                     y, **indep_var_kwargs, params=initial_params, **kwargs
                 )
             except ValueError:
                 if errors == "raise":
                     raise
                 modres = lmfit.model.ModelResult(model, initial_params, data=y)
                 modres.success = False
                 return popt, perr, pcov, stats, data, best, modres
             else:
                 if modres.success:
-                    popt, perr = [], []
+                    popt_list, perr_list = [], []
                     for name in param_names:
                         p = modres.params[name]
-                        popt.append(p.value if p.value is not None else np.nan)
-                        perr.append(p.stderr if p.stderr is not None else np.nan)
+                        popt_list.append(p.value if p.value is not None else np.nan)
+                        perr_list.append(p.stderr if p.stderr is not None else np.nan)
 
-                    popt, perr = np.array(popt), np.array(perr)
+                    popt, perr = np.array(popt_list), np.array(perr_list)
 
-                    stats = [getattr(modres, s) for s in stat_names]
-                    stats = np.array([s if s is not None else np.nan for s in stats])
+                    stats = np.array(
+                        [
+                            s if s is not None else np.nan
+                            for s in [getattr(modres, s) for s in stat_names]
+                        ]
+                    )
 
                     if modres.covar is not None:
                         var_names = modres.var_names
                         for vi in range(modres.nvarys):
                             i = param_names.index(var_names[vi])
                             for vj in range(modres.nvarys):
                                 j = param_names.index(var_names[vj])
@@ -546,27 +551,29 @@
             parallel_kw.setdefault("prefer", "processes")
 
             parallel_obj = joblib.Parallel(**parallel_kw)
 
             if parallel_obj.return_generator:
                 out_dicts = tqdm.auto.tqdm(  # type: ignore[call-overload]
                     parallel_obj(
-                        joblib.delayed(_output_wrapper)(name, da)
-                        for name, da in self._obj.data_vars.items()
+                        itertools.starmap(
+                            joblib.delayed(_output_wrapper), self._obj.data_vars.items()
+                        )
                     ),
                     **tqdm_kw,
                 )
             else:
                 with joblib_progress(**tqdm_kw) as _:
                     out_dicts = parallel_obj(
-                        joblib.delayed(_output_wrapper)(name, da)
-                        for name, da in self._obj.data_vars.items()
+                        itertools.starmap(
+                            joblib.delayed(_output_wrapper), self._obj.data_vars.items()
+                        )
                     )
             result = type(self._obj)(
-                dict(itertools.chain.from_iterable(d.items() for d in out_dicts))  # type: ignore[call-overload]
+                dict(itertools.chain.from_iterable(d.items() for d in out_dicts))
             )
             del out_dicts
 
         else:
             result = type(self._obj)()
             for name, da in tqdm.auto.tqdm(self._obj.data_vars.items(), **tqdm_kw):  # type: ignore[call-overload]
                 _output_wrapper(name, da, result)
@@ -598,19 +605,15 @@
         .replace("Dataset.polyfit", "DataArray.polyfit")
         .replace("[var]_", "")
     )
 
 
 @xr.register_dataarray_accessor("parallel_fit")
 class ParallelFitDataArrayAccessor(ERLabDataArrayAccessor):
-    """
-    `xarray.DataArray.parallel_fit` accessor for fitting lmfit models in parallel along
-    a single dimension.
-
-    """
+    """`xarray.DataArray.parallel_fit` accessor for fitting lmfit models in parallel."""
 
     _VAR_KEYS: tuple[str, ...] = (
         "modelfit_results",
         "modelfit_coefficients",
         "modelfit_stderr",
         "modelfit_covariance",
         "modelfit_stats",
```

### Comparing `erlab-2.3.2/src/erlab/accessors/kspace.py` & `erlab-2.4.0/src/erlab/accessors/kspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 import numpy as np
 import xarray as xr
 
 from erlab.accessors.utils import ERLabDataArrayAccessor
 from erlab.analysis.interpolate import interpn
 from erlab.analysis.kspace import AxesConfiguration, get_kconv_func, kz_func
 from erlab.constants import rel_kconv, rel_kzconv
-from erlab.interactive.kspace import KspaceTool, ktool
 
 
 def only_angles(method=None):
-    """
-    A decorator that ensures the data is in angle space before executing the decorated
-    method.
+    """Decorate methods that require data to be in angle space.
+
+    Ensures the data is in angle space before executing the decorated method.
 
     If the data is not in angle space (i.e., if "kx" or "ky" dimensions are present), a
     `ValueError` is raised.
     """
 
     def wrapper(method):
         @functools.wraps(method)
@@ -41,17 +40,17 @@
 
     if method is not None:
         return wrapper(method)
     return wrapper
 
 
 def only_momentum(method=None):
-    """
-    A decorator that ensures the data is in momentum space before executing the
-    decorated method.
+    """Decorate methods that require data to be in momentum space.
+
+    Ensure the data is in momentum space before executing the decorated method.
 
     If the data is not in momentum space (i.e., if "kx" nor "ky" dimensions are
     present), a `ValueError` is raised.
     """
 
     def wrapper(method):
         @functools.wraps(method)
@@ -151,24 +150,24 @@
         return out
 
     def update(
         self,
         other: dict[str, float] | Iterable[tuple[str, float]] | None = None,
         **kwargs,
     ) -> "OffsetView":
-        """Updates the offset view with the provided key-value pairs."""
+        """Update the offset view with the provided key-value pairs."""
         if other is not None:
             for k, v in other.items() if isinstance(other, dict) else other:
                 self[str(k)] = v
         for k, v in kwargs.items():
             self[k] = v
         return self
 
     def items(self) -> ItemsView[str, float]:
-        """Returns a view of the offset view as a list of (key, value) pairs."""
+        """Return a view of the offset view as a list of (key, value) pairs."""
         return dict(self).items()
 
     def reset(self) -> "OffsetView":
         """Reset all angle offsets to zero."""
         for k in self._obj.kspace.valid_offset_keys:
             self[k] = 0.0
         return self
@@ -183,15 +182,15 @@
     potential, work function, angle resolution, slit axis, momentum axes, angle
     parameters, and offsets.
 
     """
 
     @property
     def configuration(self) -> AxesConfiguration:
-        """Returns the experimental configuration.
+        """Return the experimental configuration.
 
         For a properly implemented data loader, the configuration attribute must be set
         on data import. See :class:`erlab.analysis.kspace.AxesConfiguration` for
         details.
         """
         if "configuration" not in self._obj.attrs:
             raise ValueError(
@@ -219,15 +218,14 @@
 
         Example
         -------
         >>> data.kspace.inner_potential = 13.0
         >>> data.kspace.inner_potential
         13.0
         """
-
         if "inner_potential" in self._obj.attrs:
             return float(self._obj.attrs["inner_potential"])
         else:
             warnings.warn(
                 "Inner potential not found in data attributes, assuming 10 eV",
                 stacklevel=1,
             )
@@ -252,15 +250,14 @@
 
         Example
         -------
         >>> data.kspace.work_function = 4.5
         >>> data.kspace.work_function
         4.5
         """
-
         if "sample_workfunction" in self._obj.attrs:
             return float(self._obj.attrs["sample_workfunction"])
         else:
             warnings.warn(
                 "Work function not found in data attributes, assuming 4.5 eV",
                 stacklevel=1,
             )
@@ -276,45 +273,44 @@
 
         Checks for the ``angle_resolution`` attribute of the data. If not found, a
         default value of 0.1° is silently assumed.
 
         This property is used in `best_kp_resolution` upon estimating momentum step
         sizes through `estimate_resolution`.
         """
-
         try:
             return float(self._obj.attrs["angle_resolution"])
         except KeyError:
             # warnings.warn(
             #     "Angle resolution not found in data attributes, assuming 0.1 degrees"
             # )
             return 0.1
 
     @angle_resolution.setter
     def angle_resolution(self, value: float):
         self._obj.attrs["angle_resolution"] = float(value)
 
     @property
     def slit_axis(self) -> Literal["kx", "ky"]:
-        """Returns the momentum axis parallel to the slit.
+        """Return the momentum axis parallel to the slit.
 
         Returns
         -------
         str
             Returns ``'kx'`` for type 1 configurations, ``'ky'`` otherwise.
         """
         match self.configuration:
             case AxesConfiguration.Type1 | AxesConfiguration.Type1DA:
                 return "kx"
             case _:
                 return "ky"
 
     @property
     def other_axis(self) -> Literal["kx", "ky"]:
-        """Returns the momentum axis perpendicular to the slit.
+        """Return the momentum axis perpendicular to the slit.
 
         Returns
         -------
         str
             Returns ``'ky'`` for type 1 configurations, ``'kx'`` otherwise.
         """
         match self.configuration:
@@ -322,15 +318,15 @@
                 return "ky"
             case _:
                 return "kx"
 
     @property
     @only_angles
     def momentum_axes(self) -> tuple[Literal["kx", "ky", "kz"], ...]:
-        """Returns the momentum axes of the data after conversion.
+        """Return the momentum axes of the data after conversion.
 
         Returns
         -------
         tuple
             For photon energy dependent scans, it returns the slit axis and ``'kz'``.
             For maps, it returns ``'kx'`` and ``'ky'``. Otherwise, it returns only the
             slit axis.
@@ -384,21 +380,21 @@
 
     @property
     def kinetic_energy(self) -> xr.DataArray:
         return self.hv - self.work_function + self.binding_energy
 
     @property
     def has_eV(self) -> bool:
-        """Returns `True` if object has an energy axis."""
+        """Return `True` if object has an energy axis."""
         return "eV" in self._obj.dims
 
     @property
     @only_angles
     def has_hv(self) -> bool:
-        """Returns `True` for photon energy dependent data."""
+        """Return `True` for photon energy dependent data."""
         return self._obj["hv"].size > 1
 
     @property
     @only_angles
     def has_beta(self) -> bool:
         """Check if the coordinate array for :math:`β` has more than one element.
 
@@ -442,15 +438,14 @@
         Returns
         -------
         OffsetView
             A mapping between valid offset keys and their corresponding offsets.
 
         Examples
         --------
-
         - View all offsets
 
           >>> data.kspace.offsets
           {'delta': 0.0, 'xi': 0.0, 'beta': 0.0}
 
         - View single offset
 
@@ -496,17 +491,17 @@
 
         self._offsetview.reset()
         self._offsetview.update(offset_dict)
 
     @property
     @only_angles
     def best_kp_resolution(self) -> float:
-        r"""
-        Estimates the minimum in-plane momentum resolution based on the kinetic energy
-        and angular resolution:
+        r"""Estimate the minimum in-plane momentum resolution.
+
+        The resolution is estimated with the kinetic energy and angular resolution:
 
         .. math:: \Delta k_{\parallel} \sim \sqrt{2 m_e E_k/\hbar^2} \cos(\alpha) \Delta\alpha
 
         """
         min_Ek = np.amin(self.kinetic_energy.values)
         max_angle = max(np.abs(self.alpha.values))
         return (
@@ -515,17 +510,18 @@
             * np.cos(np.deg2rad(max_angle))
             * np.deg2rad(self.angle_resolution)
         )
 
     @property
     @only_angles
     def best_kz_resolution(self) -> float:
-        r"""
-        Estimates the minimum out-of-plane momentum resolution based on the mean free
-        path :cite:p:`seah1979imfp` and the kinetic energy.
+        r"""Estimate the minimum out-of-plane momentum resolution.
+
+        The resolution is estimated based on the mean free path :cite:p:`seah1979imfp`
+        and the kinetic energy.
 
         .. math:: \Delta k_z \sim 1/\lambda
 
         """
         kin = self.kinetic_energy.values
         c1, c2 = 641.0, 0.096
         imfp = (c1 / (kin**2) + c2 * np.sqrt(kin)) * 10
@@ -537,26 +533,24 @@
             kz = kz_func(self.kinetic_energy, self.inner_potential, kx, ky)
             return {"kx": kx, "ky": ky, "kz": kz}
         else:
             return {"kx": kx, "ky": ky}
 
     def estimate_bounds(self) -> dict[Literal["kx", "ky", "kz"], tuple[float, float]]:
         """
-        Estimates the bounds of the data in momentum space based on the available
-        parameters.
+        Estimate the bounds of the data in momentum space.
 
         Returns
         -------
         bounds : dict[str, tuple[float, float]]
             A dictionary containing the estimated bounds for each parameter. The keys of
             the dictionary are 'kx', 'ky', and 'kz' (for :math:`hν`-dependent data). The
             values are tuples representing the minimum and maximum values.
 
         """
-
         return {
             k: (v.values.min(), v.values.max())
             for k, v in self._get_transformed_coords().items()
         }
 
     @only_angles
     def estimate_resolution(
@@ -668,28 +662,26 @@
         xarray.DataArray
             The DataArray with transformed coordinates.
         """
         return self._obj.assign_coords(self._get_transformed_coords())
 
     @only_angles
     def _get_coord_for_conversion(self, name: Hashable) -> xr.DataArray:
-        """
-        Get the coordinte array for given dimension name. This just ensures that the
-        energy coordinates are given as binding energy.
+        """Get the coordinte array for given dimension name.
+
+        This just ensures that the energy coordinates are given as binding energy.
         """
         if name == "eV":
             return self.binding_energy
         else:
             return self._obj[name]
 
     @only_angles
     def _data_ensure_binding(self) -> xr.DataArray:
-        """
-        Returns the data while ensuring that the energy axis is in binding energy.
-        """
+        """Return the data while ensuring that the energy axis is in binding energy."""
         return self._obj.assign_coords(eV=self.binding_energy)
 
     @only_angles
     def convert(
         self,
         bounds: dict[str, tuple[float, float]] | None = None,
         resolution: dict[str, float] | None = None,
@@ -753,15 +745,14 @@
         .. code-block:: python
 
             bounds = {"kx": (0.0, 1.0), "ky": (-1.0, 1.0)}
             resolution = {"kx": 0.01, "ky": 0.01}
             converted_data = data.kspace.convert(bounds, resolution)
 
         """
-
         if bounds is None:
             bounds = {}
 
         if resolution is None:
             resolution = {}
 
         if not silent:
@@ -866,23 +857,25 @@
         ).assign_coords({k: v.squeeze() for k, v in coords_for_transform.items()})
 
         if not silent:
             print(f"Interpolated in {time.perf_counter() - t_start:.3f} s")
 
         return out
 
-    def interactive(self, **kwargs) -> KspaceTool:
+    def interactive(self, **kwargs):
         """Open the interactive momentum space conversion tool."""
+        from erlab.interactive.kspace import ktool
+
         if self._obj.ndim < 3:
             raise ValueError("Interactive tool requires three-dimensional data.")
         return ktool(self._obj, **kwargs)
 
     @only_momentum
     def hv_to_kz(self, hv: float) -> xr.DataArray:
-        """Returns :math:`k_z` for a given photon energy.
+        """Return :math:`k_z` for a given photon energy.
 
         Useful when creating overlays on :math:`hν`-dependent data.
 
         Parameters
         ----------
         hv
             Photon energy in eV.
```

### Comparing `erlab-2.3.2/src/erlab/accessors/utils.py` & `erlab-2.4.0/src/erlab/accessors/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from collections.abc import Hashable, Mapping
 from typing import Any, TypeGuard, TypeVar, cast
 
 import matplotlib.pyplot as plt
 import xarray as xr
 
 import erlab.plotting.erplot as eplt
-from erlab.interactive.imagetool import ImageTool, itool
 
 T = TypeVar("T")
 
 # Used as the key corresponding to a DataArray's variable when converting
 # arbitrary DataArray objects to datasets, from xarray.core.dataarray
 _THIS_ARRAY: str = "<this-array>"
 
@@ -59,18 +58,19 @@
 
 
 @xr.register_dataarray_accessor("qplot")
 class PlotAccessor(ERLabDataArrayAccessor):
     """`xarray.DataArray.qplot` accessor for plotting data."""
 
     def __call__(self, *args, **kwargs):
-        """
-        Plot the data. If a 2D data array is provided, it is plotted using
-        :func:`plot_array <erlab.plotting.general.plot_array>`. Otherwise, it is
-        equivalent to calling :meth:`xarray.DataArray.plot`.
+        """Plot the data.
+
+        If a 2D data array is provided, it is plotted using :func:`plot_array
+        <erlab.plotting.general.plot_array>`. Otherwise, it is equivalent to calling
+        :meth:`xarray.DataArray.plot`.
 
         Parameters
         ----------
         *args
             Positional arguments to be passed to the plotting function.
         **kwargs
             Keyword arguments to be passed to the plotting function.
@@ -89,27 +89,26 @@
             return out
 
 
 @xr.register_dataarray_accessor("qshow")
 class ImageToolAccessor(ERLabDataArrayAccessor):
     """`xarray.DataArray.qshow` accessor for interactive visualization."""
 
-    def __call__(self, *args, **kwargs) -> ImageTool | list[ImageTool] | None:
+    def __call__(self, *args, **kwargs):
+        from erlab.interactive.imagetool import itool
+
         if len(self._obj.dims) >= 2:
             return itool(self._obj, *args, **kwargs)
         else:
             raise ValueError("Data must have at leasst two dimensions.")
 
 
 @xr.register_dataarray_accessor("qsel")
 class SelectionAccessor(ERLabDataArrayAccessor):
-    """
-    `xarray.DataArray.qsel` accessor for conveniently selecting and averaging
-    data.
-    """
+    """`xarray.DataArray.qsel` accessor for convenient selection and averaging."""
 
     def __call__(
         self,
         indexers: Mapping[Hashable, float | slice] | None = None,
         *,
         verbose: bool = False,
         **indexers_kwargs,
@@ -150,15 +149,14 @@
             The selected and averaged data.
 
         Raises
         ------
         ValueError
             If a specified dimension is not present in the data.
         """
-
         indexers = either_dict_or_kwargs(indexers, indexers_kwargs, "qsel")
 
         # Bin widths for each dimension, zero if width not specified
         bin_widths: dict[Hashable, float] = {}
 
         for dim in indexers:
             if not str(dim).endswith("_width"):
```

### Comparing `erlab-2.3.2/src/erlab/analysis/__init__.py` & `erlab-2.4.0/src/erlab/analysis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,17 +26,20 @@
     "mask_with_hex_bz",
     "mask_with_polygon",
     "polygon_mask",
     "polygon_mask_points",
     "rotateinplane",
     "rotatestackinplane",
     "shift",
+    "slice_along_path",
 ]
 
+from erlab.analysis import fit, gold, image, interpolate, mask  # noqa: F401
 from erlab.analysis.gold import correct_with_edge
+from erlab.analysis.interpolate import slice_along_path
 from erlab.analysis.mask import (
     mask_with_hex_bz,
     mask_with_polygon,
     polygon_mask,
     polygon_mask_points,
 )
 from erlab.analysis.transform import rotateinplane, rotatestackinplane
```

### Comparing `erlab-2.3.2/src/erlab/analysis/correlation.py` & `erlab-2.4.0/src/erlab/analysis/correlation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Macros for correlation analysis."""
 
-__all__ = ["acf2", "acf2stack", "match_dims", "xcorr1d"]
+__all__ = ["acf2", "acf2stack", "xcorr1d"]
 
 
 import itertools
 
 import joblib
 import numpy as np
 import scipy.signal
@@ -44,17 +44,15 @@
         acf_nan[acf_nan < 1e7 * np.finfo(float).eps] = np.nan
         return acf / acf_nan
     else:
         return acf
 
 
 def acf2(arr, mode: str = "full", method: str = "fft"):
-    """
-    Calculate the autocorrelation function (ACF) of a two-dimensional array including
-    nan values.
+    """Calculate the autocorrelation function (ACF) of a 2D array including nans.
 
     Parameters
     ----------
     arr
         The input array for which the ACF needs to be calculated.
     mode
         The mode of the ACF calculation, by default ``"full"``. For more information,
@@ -148,26 +146,17 @@
             }
         )
         if all(i in out.dims for i in ["kx", "ky"]):
             out = out.rename({"kx": "qx", "ky": "qy"})
     return out
 
 
-def match_dims(da1: xr.DataArray, da2: xr.DataArray):
-    """
-    Returns the second array interpolated with the coordinates of the first array,
-    making them the same size.
-
-    """
-    return da2.interp({dim: da1[dim] for dim in da2.dims})
-
-
 def xcorr1d(in1: xr.DataArray, in2: xr.DataArray, method="direct"):
-    """Performs 1-dimensional correlation analysis on `xarray.DataArray` s."""
-    in2 = match_dims(in1, in2)
+    """Perform 1-dimensional correlation analysis on `xarray.DataArray` s."""
+    in2 = in2.interp_like(in1)
     out = in1.copy(deep=True)
     xind = scipy.signal.correlation_lags(in1.values.size, in2.values.size, mode="same")
     xzero = np.flatnonzero(xind == 0)[0]
     out.values = scipy.signal.correlate(
         in1.fillna(0).values, in2.fillna(0).values, mode="same", method=method
     )
     out[in1.dims[0]] = out[in1.dims[0]] - out[in1.dims[0]][xzero]
```

### Comparing `erlab-2.3.2/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.4.0/src/erlab/analysis/fit/functions/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     "bcs_gap",
     "do_convolve",
     "do_convolve_2d",
     "dynes",
     "fermi_dirac",
     "fermi_dirac_linbkg",
     "fermi_dirac_linbkg_broad",
-    "gaussian_wh",
     "gaussian",
-    "lorentzian_wh",
+    "gaussian_wh",
     "lorentzian",
+    "lorentzian_wh",
     "step_broad",
     "step_linbkg_broad",
 ]
 
 from erlab.analysis.fit.functions.dynamic import (
     FermiEdge2dFunction,
     MultiPeakFunction,
@@ -43,14 +43,14 @@
     bcs_gap,
     do_convolve,
     do_convolve_2d,
     dynes,
     fermi_dirac,
     fermi_dirac_linbkg,
     fermi_dirac_linbkg_broad,
-    gaussian_wh,
     gaussian,
-    lorentzian_wh,
+    gaussian_wh,
     lorentzian,
+    lorentzian_wh,
     step_broad,
     step_linbkg_broad,
 )
```

### Comparing `erlab-2.3.2/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.4.0/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "MultiPeakFunction",
     "PolynomialFunction",
     "get_args_kwargs",
 ]
 import functools
 import inspect
 from collections.abc import Callable, Sequence
-from typing import Any, TypedDict, no_type_check, ClassVar
+from typing import Any, ClassVar, TypedDict, no_type_check
 
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 
 from erlab.analysis.fit.functions.general import (
     TINY,
@@ -121,24 +121,24 @@
         super().__init__()
         self.degree = degree
 
     @property
     def argnames(self) -> list[str]:
         return ["x"] + [f"c{i}" for i in range(self.degree + 1)]
 
-    def __call__(self, x, *coeffs, **params):
+    def __call__(self, x, *coeffs: float, **params):
         if len(coeffs) != self.degree + 1:
-            coeffs = [params[f"c{d}"] for d in range(self.degree + 1)]
+            coeffs = tuple(params[f"c{d}"] for d in range(self.degree + 1))
         if isinstance(x, np.ndarray):
             return np.polynomial.polynomial.polyval(x, coeffs)
         else:
-            coeffs = xr.DataArray(
+            coeffs_xr = xr.DataArray(
                 np.asarray(coeffs), coords={"degree": np.arange(self.degree + 1)}
             )
-            return xr.polyval(x, coeffs)
+            return xr.polyval(x, coeffs_xr)
 
 
 class MultiPeakFunction(DynamicFunction):
     """A callable class for a multi-peak model.
 
     Parameters
     ----------
@@ -227,22 +227,22 @@
         for i, func in enumerate(self.peak_funcs):
             args += [f"p{i}_{arg}" for arg in self.peak_all_args[func]["args"][1:]]
         return args
 
     @property
     def kwargs(self):
         kws = [
-            ("lin_bkg", 0),
-            ("const_bkg", 0),
+            ("lin_bkg", 0.0),
+            ("const_bkg", 0.0),
         ]
         if self.fd:
             kws += [
                 ("efermi", 0.0),  # fermi level
-                ("temp", 30),  # temperature
-                ("offset", 0),
+                ("temp", 30.0),  # temperature
+                ("offset", 0.0),
             ]
         if self.convolve:
             kws += [("resolution", 0.02)]
 
         for i, func in enumerate(self.peak_funcs):
             for arg, val in dict(self.peak_all_args[func]["kwargs"]).items():
                 kws.append((f"p{i}_{arg}", val))
```

### Comparing `erlab-2.3.2/src/erlab/analysis/fit/functions/general.py` & `erlab-2.4.0/src/erlab/analysis/fit/functions/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,24 @@
     "bcs_gap",
     "do_convolve",
     "do_convolve_2d",
     "dynes",
     "fermi_dirac",
     "fermi_dirac_linbkg",
     "fermi_dirac_linbkg_broad",
-    "gaussian_wh",
     "gaussian",
-    "lorentzian_wh",
+    "gaussian_wh",
     "lorentzian",
+    "lorentzian_wh",
     "step_broad",
     "step_linbkg_broad",
 ]
 
 from collections.abc import Callable
+
 import numba
 import numpy as np
 import numpy.typing as npt
 import scipy.special
 
 from erlab.constants import kb_eV
 
@@ -79,15 +80,14 @@
     -------
     extended
         The domain of the kernel.
     gauss
         The gaussian kernel defined on `extended`.
 
     """
-
     delta_x = x[1] - x[0]
 
     sigma = abs(resolution) / np.sqrt(8 * np.log(2))  # resolution given in FWHM
     n_pad = int(sigma * pad / delta_x + 0.5)
     x_pad = n_pad * delta_x
 
     extended = np.linspace(x[0] - x_pad, x[-1] + x_pad, 2 * n_pad + len(x))
@@ -259,18 +259,15 @@
     temp: float,
     resolution: float,
     back0: float,
     back1: float,
     dos0: float,
     dos1: float,
 ) -> npt.NDArray[np.float64]:
-    """
-    Resolution-broadened Fermi-dirac edge with linear backgrounds above and below the
-    fermi level.
-    """
+    """Resolution-broadened Fermi edge with linear backgrounds above and below EF."""
     return do_convolve(
         x,
         fermi_dirac_linbkg,
         resolution=resolution,
         center=center,
         temp=temp,
         back0=back0,
@@ -299,18 +296,15 @@
     center: float,
     sigma: float,
     back0: float,
     back1: float,
     dos0: float,
     dos1: float,
 ):
-    """
-    A linear density of states multiplied with a resolution broadened step function with
-    a linear background.
-    """
+    """Resolution broadened step function with linear backgrounds."""
     return (back0 + back1 * x) + (dos0 - back0 + (dos1 - back1) * x) * (
         step_broad(x, center, sigma, 1.0)
     )
 
 
 @numba.njit()
 def bcs_gap(
@@ -321,15 +315,15 @@
     .. math::
 
         \Delta(T) \simeq a \cdot k_B T_c \cdot \tanh\left(b \sqrt{\frac{T_c}{T} -
         1}\right)
 
     Parameters
     ----------
-    x : array_like
+    x : array-like
         The temperature values in kelvins at which to calculate the BCS gap.
     a
         Proportionality constant. Default is 1.76.
     b
         Proportionality constant. Default is 1.74.
     tc
         The critical temperature in Kelvins. Default is 100.0.
@@ -341,30 +335,30 @@
             out[i] = a * kb_eV * tc * np.tanh(b * np.sqrt(tc / x[i] - 1))
         else:
             out[i] = 0.0
     return out
 
 
 def dynes(x, n0=1.0, gamma=0.003, delta=0.01):
-    r"""The Dynes formula for superconducting density of states.
+    r"""Dynes formula for superconducting density of states.
 
     The formula is given by :cite:p:`dynes1978dynes`:
 
     .. math::
 
         f(x) = N_0  \text{Re}\left[\frac{|x| + i \Gamma}{\sqrt{(|x| + i \Gamma)^2 -
         \Delta^2}}\right]
 
     where :math:`x` is the binding energy, :math:`N_0` is the normal-state density of
     states at the Fermi level, :math:`\Gamma` is the broadening term, and :math:`\Delta`
     is the superconducting energy gap.
 
     Parameters
     ----------
-    x : array_like
+    x : array-like
         The input array of energy in eV.
     n0
         :math:`N_0`, by default 1.0.
     gamma
         :math:`\Gamma`, by default 0.003.
     delta
         The superconducting energy gap :math:`\Delta`, by default 0.01.
```

### Comparing `erlab-2.3.2/src/erlab/analysis/fit/minuit.py` & `erlab-2.4.0/src/erlab/analysis/fit/minuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,26 +67,24 @@
         pass
 
     def __exit__(self, *args: object) -> None:
         plt.close(self.fig)
 
 
 class Minuit(iminuit.Minuit):
-    """A subclass of `iminuit.Minuit` that provides additional functionality for fitting
-    `lmfit` library models.
+    """`iminuit.Minuit` with additional functionality.
 
     This class extends the functionality of the `iminuit.Minuit` class by providing a
     convenient method `from_lmfit` to initialize the `Minuit` object from an
     `lmfit.Model` object.
 
     For more information on the `iminuit` library, see its documentation.
 
     Examples
     --------
-
     >>> import lmfit.models
     >>> import numpy as np
     >>> from erlab.analysis.fit.minuit import Minuit
 
     >>> # Create an lmfit.Model object
     >>> model = lmfit.models.LinearModel()
```

### Comparing `erlab-2.3.2/src/erlab/analysis/fit/models.py` & `erlab-2.4.0/src/erlab/analysis/fit/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Models for fitting data."""
 
 __all__ = [
     "BCSGapModel",
     "DynesModel",
-    "FermiEdgeModel",
     "FermiEdge2dModel",
+    "FermiEdgeModel",
     "MultiPeakModel",
     "PolynomialModel",
     "StepEdgeModel",
 ]
 
 import lmfit
 import numba
@@ -108,18 +108,18 @@
         np.array(data[-len_fit:], dtype=np.float64),
         deg=1,
     )
     return n0, m0, n1, m1
 
 
 class FermiEdgeModel(lmfit.Model):
-    """
-    Fermi-dirac function with linear background above and below the fermi level,
-    convolved with a gaussian kernel.
+    """Model for fitting a Fermi edge with a linear background.
 
+    The model function is a Fermi-dirac function with linear background above and below
+    the fermi level, convolved with a gaussian kernel.
     """
 
     __doc__ = __doc__ + lmfit.models.COMMON_INIT_DOC
 
     @staticmethod
     def LinearBroadFermiDirac(
         x,
```

### Comparing `erlab-2.3.2/src/erlab/analysis/fit/spline.py` & `erlab-2.4.0/src/erlab/analysis/fit/spline.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     Returns
     -------
     out : xarray.DataArray
         Smoothing spline evaluated at `arr` coordinates.
     spl : csaps.ISmoothingSpline
         The spline object.
     """
-
     kwargs.setdefault("normalizedsmooth", True)
     coords = [arr[d].values for d in arr.dims]
     spl = csaps.csaps(coords, arr.values, **kwargs)
     out = xr.DataArray(
         data=spl(coords),
         dims=arr.dims,
         coords={arr.dims[i]: coords[i] for i in range(arr.ndim)},
```

### Comparing `erlab-2.3.2/src/erlab/analysis/gold.py` & `erlab-2.4.0/src/erlab/analysis/gold.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,14 @@
         The fitted center values and their standard errors, returned when `return_full`
         is `False`.
     fitresults
         A dataset containing the full fit results, returned when `return_full` is
         `True`.
 
     """
-
     if fast:
         params = lmfit.create_params()
         model_cls: lmfit.Model = StepEdgeModel
     else:
         if temp is None:
             temp = gold.attrs["temp_sample"]
         params = lmfit.create_params(temp={"value": temp, "vary": vary_temp})
```

### Comparing `erlab-2.3.2/src/erlab/analysis/image.py` & `erlab-2.4.0/src/erlab/analysis/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Note
 ----
 For scipy-based filter functions, the default value of the `mode` argument is 'nearest',
 unlike the scipy default of 'reflect'.
 """
 
-from collections.abc import Collection, Mapping, Sequence, Sized, Hashable
+from collections.abc import Collection, Hashable, Mapping, Sequence, Sized
 
 import numpy as np
 import numpy.typing as npt
 import scipy
 import scipy.ndimage
 import xarray as xr
 from numba import carray, cfunc, types
@@ -201,15 +201,14 @@
     - The input array is assumed to be regularly spaced.
 
     See Also
     --------
     :func:`scipy.ndimage.gaussian_laplace` : The underlying function used to apply the
         filter.
     """
-
     if isinstance(sigma, Mapping):
         sigma_dict = dict(sigma)
     elif np.isscalar(sigma):
         sigma_dict = dict.fromkeys(darr.dims, sigma)
     elif isinstance(sigma, Collection):
         sigma_dict = dict(zip(darr.dims, sigma, strict=True))
     else:
@@ -275,15 +274,14 @@
     This function calculates the gradient magnitude of an input array by applying a
     filter to the input array using the given dx and dy values. The filter is defined by
     a kernel function that computes the squared difference between each element of the
     input array and the central element, divided by the corresponding distance value.
     The gradient magnitude is then calculated as the square root of the sum of the
     squared differences.
     """
-
     dxy = np.sqrt(dx**2 + dy**2)
     dist = np.array([[dxy, dy, dxy], [dx, 0.0, dx], [dxy, dy, dxy]]).flatten()
 
     @cfunc(
         types.intc(
             types.CPointer(types.float64),
             types.intp,
@@ -374,15 +372,14 @@
         If the input DataArray is not 2D.
 
     Note
     ----
     - The input array is assumed to be regularly spaced.
     - Any zero gradient values are replaced with NaN.
     """
-
     if darr.ndim != 2:
         raise ValueError("DataArray must be 2D")
 
     xvals = darr[darr.dims[1]].values
     yvals = darr[darr.dims[0]].values
 
     dx = abs(xvals[1] - xvals[0])
@@ -501,15 +498,14 @@
     ValueError
         If the input DataArray is not 2D.
 
     Note
     ----
     The input array is assumed to be regularly spaced.
     """
-
     if darr.ndim != 2:
         raise ValueError("DataArray must be 2D")
 
     xvals = darr[darr.dims[1]].values
     yvals = darr[darr.dims[0]].values
 
     dx = xvals[1] - xvals[0]
```

### Comparing `erlab-2.3.2/src/erlab/analysis/interpolate.py` & `erlab-2.4.0/src/erlab/analysis/interpolate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,25 @@
-"""Fast linear interpolation."""
+"""Utilities for interpolation."""
 
-__all__ = ["FastInterpolator", "interpn"]
+__all__ = ["FastInterpolator", "interpn", "slice_along_path"]
 
+import itertools
 import math
 import warnings
-from collections.abc import Sequence
+from collections.abc import Hashable, Mapping, Sequence
+from typing import cast
 
 import numba
 import numpy as np
+import numpy.typing as npt
 import scipy.interpolate
 import xarray as xr
 import xarray.core.missing
 
-
-@numba.njit(nogil=True, inline="always")
-def _do_interp1(x, v0, v1):
-    return v0 * (1 - x) + v1 * x
-
-
-@numba.njit(nogil=True, inline="always")
-def _do_interp2(x, y, v0, v1, v2, v3):
-    return _do_interp1(y, _do_interp1(x, v0, v1), _do_interp1(x, v2, v3))
-
-
-@numba.njit(nogil=True, inline="always")
-def _do_interp3(x, y, z, v0, v1, v2, v3, v4, v5, v6, v7):
-    return _do_interp1(
-        z, _do_interp2(x, y, v0, v1, v2, v3), _do_interp2(x, y, v4, v5, v6, v7)
-    )
-
-
-# @numba.njit
-# def _do_interp2(x, y, v0, v1, v2, v3):
-#     return _do_interp1(y, v0 * (1 - x) + v1 * x, v2 * (1 - x) + v3 * x)
-
-
-# @numba.njit
-# def _do_interp3(x, y, z, v0, v1, v2, v3, v4, v5, v6, v7):
-#     return (
-#         _do_interp2(x, y, v0, v1, v2, v3) * (1 - z)
-#         + _do_interp2(x, y, v4, v5, v6, v7) * z
-#     )
-
-
-@numba.njit(nogil=True, inline="always")
-def _calc_interp1(values, v0):
-    i0 = math.floor(v0)
-    n0 = values.size
-    j0 = min(i0 + 1, n0 - 1)
-    return _do_interp1(v0 - i0, values[i0], values[j0])
-
-
-@numba.njit(nogil=True, inline="always")
-def _calc_interp2(values, v0, v1):
-    i0, i1 = math.floor(v0), math.floor(v1)
-    n0, n1 = values.shape
-    j0, j1 = min(i0 + 1, n0 - 1), min(i1 + 1, n1 - 1)
-    return _do_interp2(
-        v0 - i0,
-        v1 - i1,
-        values[i0, i1],
-        values[j0, i1],
-        values[i0, j1],
-        values[j0, j1],
-    )
-
-
-@numba.njit(nogil=True, inline="always")
-def _calc_interp3(values, v0, v1, v2):
-    i0, i1, i2 = math.floor(v0), math.floor(v1), math.floor(v2)
-    n0, n1, n2 = values.shape
-    j0, j1, j2 = min(i0 + 1, n0 - 1), min(i1 + 1, n1 - 1), min(i2 + 1, n2 - 1)
-    return _do_interp3(
-        v0 - i0,
-        v1 - i1,
-        v2 - i2,
-        values[i0, i1, i2],
-        values[j0, i1, i2],
-        values[i0, j1, i2],
-        values[j0, j1, i2],
-        values[i0, i1, j2],
-        values[j0, i1, j2],
-        values[i0, j1, j2],
-        values[j0, j1, j2],
-    )
-
-
-@numba.njit(nogil=True, inline="always")
-def _val2ind(val, coord):
-    if val > coord[-1] or val < coord[0]:
-        return np.nan
-    else:
-        return np.divide(val - coord[0], coord[1] - coord[0])
-
-
-@numba.njit(nogil=True, parallel=True)
-def _interp1(x, values, xc, fill_value=np.nan):
-    n = len(xc)
-
-    arr_new = np.empty(n, values.dtype)
-
-    for m in numba.prange(n):
-        v0 = _val2ind(xc[m], x)
-
-        if np.isnan(v0):
-            arr_new[m] = fill_value
-        else:
-            arr_new[m] = _calc_interp1(values, v0)
-    return arr_new
-
-
-@numba.njit(nogil=True, parallel=True)
-def _interp2(x, y, values, xc, yc, fill_value=np.nan):
-    n = len(xc)
-
-    arr_new = np.empty(n, values.dtype)
-
-    for m in numba.prange(n):
-        v0, v1 = _val2ind(xc[m], x), _val2ind(yc[m], y)
-
-        if np.isnan(v0) or np.isnan(v1):
-            arr_new[m] = fill_value
-        else:
-            arr_new[m] = _calc_interp2(values, v0, v1)
-    return arr_new
-
-
-@numba.njit(nogil=True, parallel=True)
-def _interp3(x, y, z, values, xc, yc, zc, fill_value=np.nan):
-    n = len(xc)
-
-    arr_new = np.empty(n, values.dtype)
-
-    for m in numba.prange(n):
-        v0, v1, v2 = _val2ind(xc[m], x), _val2ind(yc[m], y), _val2ind(zc[m], z)
-
-        if np.isnan(v0) or np.isnan(v1) or np.isnan(v2):
-            arr_new[m] = fill_value
-        else:
-            arr_new[m] = _calc_interp3(values, v0, v1, v2)
-    return arr_new
-
-
-def _get_interp_func(ndim):
-    if ndim == 3:
-        return _interp3
-    elif ndim == 2:
-        return _interp2
-    elif ndim == 1:
-        return _interp1
-    else:
-        raise ValueError("Fast interpolation only supported for 2D or 3D")
-
-
-def _check_even(arr):
-    dif = np.diff(arr)
-    if dif.size == 0:
-        return False
-    return np.allclose(dif, dif[0])
+from erlab.accessors.utils import either_dict_or_kwargs
 
 
 class FastInterpolator(scipy.interpolate.RegularGridInterpolator):
     """Fast linear multidimensional interpolation on evenly spaced coordinates.
 
     This is an extension from `scipy.interpolate.RegularGridInterpolator` with vast
     performance improvements and integration with `xarray`.
@@ -329,14 +187,275 @@
     """
     interp = FastInterpolator(
         points, values, method=method, bounds_error=bounds_error, fill_value=fill_value
     )
     return interp(xi)
 
 
+@numba.njit(nogil=True, inline="always")
+def _do_interp1(x, v0, v1):
+    return v0 * (1 - x) + v1 * x
+
+
+@numba.njit(nogil=True, inline="always")
+def _do_interp2(x, y, v0, v1, v2, v3):
+    return _do_interp1(y, _do_interp1(x, v0, v1), _do_interp1(x, v2, v3))
+
+
+@numba.njit(nogil=True, inline="always")
+def _do_interp3(x, y, z, v0, v1, v2, v3, v4, v5, v6, v7):
+    return _do_interp1(
+        z, _do_interp2(x, y, v0, v1, v2, v3), _do_interp2(x, y, v4, v5, v6, v7)
+    )
+
+
+@numba.njit(nogil=True, inline="always")
+def _calc_interp1(values, v0):
+    i0 = math.floor(v0)
+    n0 = values.size
+    j0 = min(i0 + 1, n0 - 1)
+    return _do_interp1(v0 - i0, values[i0], values[j0])
+
+
+@numba.njit(nogil=True, inline="always")
+def _calc_interp2(values, v0, v1):
+    i0, i1 = math.floor(v0), math.floor(v1)
+    n0, n1 = values.shape
+    j0, j1 = min(i0 + 1, n0 - 1), min(i1 + 1, n1 - 1)
+    return _do_interp2(
+        v0 - i0,
+        v1 - i1,
+        values[i0, i1],
+        values[j0, i1],
+        values[i0, j1],
+        values[j0, j1],
+    )
+
+
+@numba.njit(nogil=True, inline="always")
+def _calc_interp3(values, v0, v1, v2):
+    i0, i1, i2 = math.floor(v0), math.floor(v1), math.floor(v2)
+    n0, n1, n2 = values.shape
+    j0, j1, j2 = min(i0 + 1, n0 - 1), min(i1 + 1, n1 - 1), min(i2 + 1, n2 - 1)
+    return _do_interp3(
+        v0 - i0,
+        v1 - i1,
+        v2 - i2,
+        values[i0, i1, i2],
+        values[j0, i1, i2],
+        values[i0, j1, i2],
+        values[j0, j1, i2],
+        values[i0, i1, j2],
+        values[j0, i1, j2],
+        values[i0, j1, j2],
+        values[j0, j1, j2],
+    )
+
+
+@numba.njit(nogil=True, inline="always")
+def _val2ind(val, coord):
+    if val > coord[-1] or val < coord[0]:
+        return np.nan
+    else:
+        return np.divide(val - coord[0], coord[1] - coord[0])
+
+
+@numba.njit(nogil=True, parallel=True)
+def _interp1(x, values, xc, fill_value=np.nan):
+    n = len(xc)
+
+    arr_new = np.empty(n, values.dtype)
+
+    for m in numba.prange(n):
+        v0 = _val2ind(xc[m], x)
+
+        if np.isnan(v0):
+            arr_new[m] = fill_value
+        else:
+            arr_new[m] = _calc_interp1(values, v0)
+    return arr_new
+
+
+@numba.njit(nogil=True, parallel=True)
+def _interp2(x, y, values, xc, yc, fill_value=np.nan):
+    n = len(xc)
+
+    arr_new = np.empty(n, values.dtype)
+
+    for m in numba.prange(n):
+        v0, v1 = _val2ind(xc[m], x), _val2ind(yc[m], y)
+
+        if np.isnan(v0) or np.isnan(v1):
+            arr_new[m] = fill_value
+        else:
+            arr_new[m] = _calc_interp2(values, v0, v1)
+    return arr_new
+
+
+@numba.njit(nogil=True, parallel=True)
+def _interp3(x, y, z, values, xc, yc, zc, fill_value=np.nan):
+    n = len(xc)
+
+    arr_new = np.empty(n, values.dtype)
+
+    for m in numba.prange(n):
+        v0, v1, v2 = _val2ind(xc[m], x), _val2ind(yc[m], y), _val2ind(zc[m], z)
+
+        if np.isnan(v0) or np.isnan(v1) or np.isnan(v2):
+            arr_new[m] = fill_value
+        else:
+            arr_new[m] = _calc_interp3(values, v0, v1, v2)
+    return arr_new
+
+
+def _get_interp_func(ndim):
+    if ndim == 3:
+        return _interp3
+    elif ndim == 2:
+        return _interp2
+    elif ndim == 1:
+        return _interp1
+    else:
+        raise ValueError("Fast interpolation only supported for 2D or 3D")
+
+
+def _check_even(arr):
+    dif = np.diff(arr)
+    if dif.size == 0:
+        return False
+    return np.allclose(dif, dif[0])
+
+
+def slice_along_path(
+    darr: xr.DataArray,
+    vertices: Mapping[Hashable, Sequence],
+    step_size: float | None = None,
+    dim_name: str = "path",
+    interp_kwargs: dict | None = None,
+    **vertices_kwargs,
+) -> xr.DataArray:
+    """Interpolate a DataArray along a path defined by a sequence of vertices.
+
+    Parameters
+    ----------
+    darr
+        The data array to interpolate.
+    vertices
+        Dictionary specifying the vertices of the path along which to interpolate the
+        DataArray. The keys of the dictionary should correspond to the dimensions of the
+        DataArray along which to interpolate.
+    step_size
+        The step size to use for the interpolation. This determines the number of points
+        along the path at which the data array will be interpolated. If None, the step
+        size is determined automatically as the smallest step size of the coordinates
+        along the dimensions of the vertices if all coordinates are evenly spaced. If
+        there exists a dimension where the coordinates are not evenly spaced,
+        `step_size` must be specified.
+    dim_name
+        The name of the new dimension that corresponds to the distance along the
+        interpolated path. Default is "path".
+    interp_kwargs
+        Additional keyword arguments passed to `xarray.DataArray.interp`.
+    **vertices_kwargs
+        The keyword arguments form of `vertices`. One of `vertices` or `vertices_kwargs`
+        must be provided.
+
+    Returns
+    -------
+    interpolated : DataArray
+        New dataarray on the new coordinate.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> import xarray as xr
+    >>> from erlab.analysis.interpolate import slice_along_path
+    >>> x = np.linspace(0, 10, 11)
+    >>> y = np.linspace(0, 10, 11)
+    >>> z = np.linspace(0, 10, 11)
+    >>> data = np.random.rand(11, 11, 11)
+    >>> darr = xr.DataArray(data, coords={"x": x, "y": y, "z": z}, dims=["x", "y", "z"])
+    >>> vertices = {"x": [0, 5, 10], "y": [0, 5, 10], "z": [0, 5, 10]}
+    >>> interp = slice_along_path(darr, vertices)
+
+    See Also
+    --------
+    xarray.DataArray.interp
+
+    """
+    interp_kwargs = interp_kwargs or {}
+    vertices = dict(
+        either_dict_or_kwargs(vertices, vertices_kwargs, "slice_along_path")
+    )
+
+    for dim, vert in vertices.items():
+        if dim not in darr.dims:
+            raise ValueError(f"Dimension {dim} not found in data array")
+
+        # Convert to numpy array
+        vert_arr = np.asarray(vert)
+        if vert_arr.ndim != 1:
+            raise ValueError("Each vertex must be 1-dimensional")
+        vertices[dim] = vert_arr
+
+    if not all(len(p) == len(next(iter(vertices.values()))) for p in vertices.values()):
+        raise ValueError("Vertices must have the same length along all dimensions")
+
+    if step_size is None:
+        step_size = np.inf
+        for dim in vertices:
+            dif = np.diff(darr[dim].values)
+            if np.allclose(dif, dif[0], equal_nan=True):
+                step_size = min(step_size, np.abs(dif[0]))
+
+        if not np.isfinite(cast(float, step_size)):
+            raise ValueError("Could not determine step size automatically")
+    else:
+        if not np.isfinite(step_size):
+            raise ValueError("Step size must be finite")
+        if step_size <= 0:
+            raise ValueError("Step size must be positive")
+
+    points: npt.NDArray[np.floating] = np.array(list(vertices.values())).T
+
+    # Calculate number of points for each segment
+    num_points = [
+        round(np.linalg.norm(p2 - p1) / step_size) - 1  # type: ignore[call-overload,operator]
+        for p1, p2 in itertools.pairwise(points)
+    ]
+    # Generate points for each segment
+    segments = [
+        np.linspace(points[i], points[i + 1], num, axis=-1, endpoint=False)
+        for i, num in enumerate(num_points[:-1])
+    ]
+    segments.append(
+        np.linspace(points[-2], points[-1], num_points[-1] + 1, axis=-1, endpoint=True)
+    )
+
+    # Concatenate the points
+    points_arr = np.concatenate(segments, axis=-1)
+    points_arr = np.atleast_2d(points_arr)  # Ensure 2D for 1D paths
+
+    # Distance between each pair of consecutive points
+    distances = np.linalg.norm(np.diff(points_arr, axis=-1), axis=0)
+
+    # Cumulative sum of the distances
+    path_coord = np.concatenate(([0], np.cumsum(distances)))
+
+    interp_coords = [
+        xr.DataArray(p, dims=dim_name, coords={dim_name: path_coord})
+        for p in points_arr
+    ]
+    return darr.interp(
+        dict(zip(vertices.keys(), interp_coords, strict=False)), **interp_kwargs
+    )
+
+
+# Monkey patch xarray to make fast interpolator available
+
 _get_interpolator_nd_original = xarray.core.missing._get_interpolator_nd
 _get_interpolator_original = xarray.core.missing._get_interpolator
 
 
 def _get_interpolator_fast(method, **kwargs):
     if method == "linearfast":
         method = "linear"
```

### Comparing `erlab-2.3.2/src/erlab/analysis/kspace.py` & `erlab-2.4.0/src/erlab/analysis/kspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 import erlab.constants
 import erlab.io
 import erlab.lattice
 
 
 class AxesConfiguration(enum.IntEnum):
-    """
-    Enum class representing different types of axes configurations. See Ref.
-    :cite:p:`ishida2018kconv`.
+    """Enum class representing different types of axes configurations.
+
+    See Ref. :cite:p:`ishida2018kconv`.
 
     """
 
     Type1 = 1
     Type2 = 2
     Type1DA = 3
     Type2DA = 4
@@ -39,43 +39,44 @@
 def _kz_func_inv(kz, inner_potential, kx, ky):
     k_perp_sq = kx**2 + ky**2
     k_z_sq = kz**2
     return k_perp_sq + k_z_sq - inner_potential / erlab.constants.rel_kzconv
 
 
 def _kperp_func(k_tot_sq, kx, ky):
-    r""":math:`\sqrt{k^2 - k_x^2 - k_y^2}`"""
+    r""":math:`\sqrt{k^2 - k_x^2 - k_y^2}`."""
     return np.sqrt(np.clip(k_tot_sq - kx**2 - ky**2, a_min=0, a_max=None))
 
 
 def kz_func(kinetic_energy, inner_potential, kx, ky):
-    r"""
-    Calculate :math:`k_z` from the given kinetic energy, inner potential, and
-    :math:`k_x`, :math:`k_y` with
+    r"""Calculate the out-of-plane momentum.
+
+    :math:`k_z` is computed from the given kinetic energy :math:`E_k`, inner potential
+    :math:`V_0`, and in-plane momenta :math:`k_x`, and :math:`k_y` by
 
     .. math::
 
         k_z = \sqrt{k^2 - k_x^2 - k_y^2 + \frac{2 m_e V_0}{\hbar^2}}
 
-    where :math:`k = \frac{\sqrt{2 m_e E_k}}{\hbar}`.
+    where :math:`k =\sqrt{2 m_e E_k}/\hbar`.
     """
     k_tot = erlab.constants.rel_kconv * np.sqrt(kinetic_energy)
     k_perp_sq = k_tot**2 - kx**2 - ky**2
     k_z_sq = k_perp_sq + inner_potential / erlab.constants.rel_kzconv
     return np.sqrt(np.clip(k_z_sq, a_min=0, a_max=None))
 
 
 def get_kconv_func(
     kinetic_energy: float | npt.NDArray | xarray.DataArray,
     configuration: AxesConfiguration,
     angle_params: dict[str, float],
 ) -> tuple[Callable, Callable]:
-    """
-    Returns the appropriate momentum conversion functions based on the given
-    configuration and kinetic energy.
+    """Return appropriate momentum conversion functions.
+
+    The appropriate function is created by the given configuration and kinetic energy.
 
     Parameters
     ----------
     kinetic_energy
         The kinetic energy in eV.
     configuration
         Experimental configuration.
```

### Comparing `erlab-2.3.2/src/erlab/analysis/mask/__init__.py` & `erlab-2.4.0/src/erlab/analysis/mask/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,16 +151,15 @@
     else:
         return mask
 
 
 def mask_with_hex_bz(
     kxymap: xr.DataArray, a: float = 3.54, rotate: float = 0.0, invert: bool = False
 ) -> xr.DataArray:
-    """Returns map masked with a hexagonal BZ."""
-
+    """Return map masked with a hexagonal BZ."""
     if "kx" in kxymap.dims or "qx" in kxymap.dims:
         dims = ("kx", "ky")
 
     d = 2 * np.pi / (a * 3)
     ang = rotate + np.array([0, 60, 120, 180, 240, 300])
     vertices = np.array(
         [[2 * d * np.cos(t), 2 * d * np.sin(t)] for t in np.deg2rad(ang)]
@@ -173,16 +172,15 @@
     y,
     a: float = 3.54,
     rotate: float = 0,
     offset: tuple[float, float] = (0.0, 0.0),
     reciprocal: bool = False,
     invert: bool = False,
 ) -> npt.NDArray[np.bool_]:
-    """Returns a mask for given points."""
-
+    """Return a mask for given points."""
     if reciprocal:
         d = 2 * np.pi / (a * 3)
     else:
         d = a
     ang = rotate + np.array([0, 60, 120, 180, 240, 300])
     vertices = np.array(
         [
```

### Comparing `erlab-2.3.2/src/erlab/analysis/mask/polygon.py` & `erlab-2.4.0/src/erlab/analysis/mask/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""
-Point-in-polygon algorithm adapted from the `CGAL C++ library
+"""Point-in-polygon algorithm.
+
+The implementation has been adapted from the `CGAL C++ library
 <https://doc.cgal.org/5.3.2/Polygon/index.html>`_.
 
 """
 
 from __future__ import annotations
 
 import enum
@@ -54,15 +55,15 @@
 @numba.njit(nogil=True, cache=True)
 def _get_argmax_all(arr):
     return np.nonzero(arr == arr.max())[0]
 
 
 @numba.njit(nogil=True, cache=True)
 def left_vertex(points: Annotated[npt.NDArray[np.float64], Literal[1, 2]]) -> int:
-    """Returns the index of the leftmost point of a polygon.
+    """Return the index of the leftmost point of a polygon.
 
     In case of a tie, the point with the smallest y-coordinate is taken.
 
     Parameters
     ----------
     points
         Input array of polygon vertices.
@@ -74,15 +75,15 @@
     """
     ind = _get_argmin_all(points[:, 0].astype(np.float32))
     return ind[np.argmin(points[ind][:, 1])]
 
 
 @numba.njit(nogil=True, cache=True)
 def right_vertex(points: Annotated[npt.NDArray[np.float64], Literal[1, 2]]):
-    """Returns the index of the rightmost point of a polygon.
+    """Return the index of the rightmost point of a polygon.
 
     In case of a tie, the point with the largest y-coordinate is taken.
 
     Parameters
     ----------
     points
         Input array of polygon vertices.
@@ -132,15 +133,15 @@
     return _orientation(points[low], point, points[high])
 
 
 @numba.njit(nogil=True, cache=True)
 def bounded_side_bool(
     points: npt.NDArray[np.float64], point: tuple[float, float], boundary: bool = True
 ) -> bool:
-    """Computes whether a point lies inside a polygon using `bounded_side`.
+    """Compute whether a point lies inside a polygon using `bounded_side`.
 
     Parameters
     ----------
     points
         (N, 2) input array of polygon vertices.
     point
         2-tuple of float specifying point of interest.
@@ -162,15 +163,15 @@
             return boundary
         case _:
             return False
 
 
 @numba.njit(nogil=True, cache=True)
 def bounded_side(points: npt.NDArray[np.float64], point: tuple[float, float]) -> Side:
-    """Computes if a point is inside, outside, or on the boundary of a polygon.
+    """Compute if a point is inside, outside, or on the boundary of a polygon.
 
     The polygon is defined by the sequence of points [first,last). Being inside is
     defined by the odd-even rule. If the point is on a polygon edge, a special value is
     returned. A simple polygon divides the plane in an unbounded and a bounded region.
     According to the definition points in the bounded region are inside the polygon.
 
     Parameters
@@ -190,15 +191,14 @@
     We shoot a horizontal ray from the point to the right and count the number of
     intersections with polygon segments. If the number of intersections is odd, the
     point is inside. We don't count intersections with horizontal segments. With
     non-horizontal segments, the top vertex is considered to be part of the segment, but
     the bottom vertex is not. (Segments are half-closed).
 
     """
-
     last = len(points) - 1
     if last < 2:
         return Side.ON_UNBOUNDED_SIDE
 
     is_inside = False
 
     cur_y_comp_res = _comp_y(points[0], point)
```

### Comparing `erlab-2.3.2/src/erlab/analysis/transform.py` & `erlab-2.4.0/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/analysis/utilities.py` & `erlab-2.4.0/src/erlab/analysis/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     >>> shift_arr = xr.DataArray([1, 0, 2], dims=["x"])
     >>> shifted = erlab.analysis.utilities.shift(darr, shift_arr, along="y")
     >>> print(shifted)
     <xarray.DataArray (x: 3, y: 3)> Size: 72B
     nan 1.0 2.0 4.0 5.0 6.0 nan nan 7.0
     Dimensions without coordinates: x, y
     """
-
     shift_kwargs.setdefault("order", 1)
     shift_kwargs.setdefault("mode", "constant")
     if shift_kwargs["mode"] == "constant":
         shift_kwargs.setdefault("cval", np.nan)
 
     if not isinstance(shift, xr.DataArray):
         shift = xr.DataArray(float(shift))
```

### Comparing `erlab-2.3.2/src/erlab/constants.py` & `erlab-2.4.0/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/__init__.py` & `erlab-2.4.0/src/erlab/interactive/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Interactive plotting based on Qt and pyqtgraph
+Interactive plotting based on Qt and pyqtgraph.
 
 .. currentmodule:: erlab.interactive
 
 Interactive tools
 =================
 
 .. autosummary::
```

### Comparing `erlab-2.3.2/src/erlab/interactive/bzplot.py` & `erlab-2.4.0/src/erlab/interactive/bzplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Literal
+from typing import Literal, cast
 
 import mpl_toolkits
 import numpy as np
 import numpy.typing as npt
 from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qtagg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib.figure import Figure
@@ -11,35 +11,39 @@
 
 import erlab.plotting.erplot as eplt
 from erlab.interactive.utilities import ParameterGroup
 from erlab.lattice import abc2avec, avec2abc, to_real, to_reciprocal
 
 
 class BZPlotter(QtWidgets.QMainWindow):
+    """
+    Interactive Brillouin zone plotter.
+
+    Parameters
+    ----------
+    params :
+        Input parameter for plotting. If `param_type` is 'lattice', it must be a
+        6-tuple containing the lengths a, b, c and angles alpha, beta, gamma.
+        Otherwise, it must be a 3 by 3 numpy array with each row vector containing
+        each real/reciprocal lattice vector. If not provided, a hexagonal lattice is
+        shown by default.
+    param_type
+        Specifies the param_type of the input parameters. Valid param_types are
+        `'lattice'`, `'avec'`, `'bvec'`. By default, `'bvec'` is assumed.
+    """
+
     def __init__(
         self,
         params: tuple[float, ...] | npt.NDArray[np.float64] | None = None,
         param_type: Literal["lattice", "avec", "bvec"] | None = None,
     ) -> None:
-        """
-        Parameters
-        ----------
-        params :
-            Input parameter for plotting. If `param_type` is 'lattice', it must be a
-            6-tuple containing the lengths a, b, c and angles alpha, beta, gamma.
-            Otherwise, it must be a 3 by 3 numpy array with each row vector containing
-            each real/reciprocal lattice vector. If not provided, a hexagonal lattice is
-            shown by default.
-        param_type
-            Specifies the param_type of the input parameters. Valid param_types are
-            `'lattice'`, `'avec'`, `'bvec'`. By default, `'bvec'` is assumed.
-        """
-        self.qapp = QtCore.QCoreApplication.instance()
+        self.qapp = cast(QtWidgets.QApplication, QtWidgets.QApplication.instance())
         if not self.qapp:
             self.qapp = QtWidgets.QApplication(sys.argv)
+
         super().__init__()
 
         if params is None:
             params = np.array(
                 [
                     [2.05238966, 0.0, 0.0],
                     [1.02619483, 1.77742159, 0.0],
@@ -60,15 +64,14 @@
                 raise TypeError("Lattice vectors must be a 3 by 3 numpy array.")
 
             if param_type == "avec":
                 bvec = to_reciprocal(params)
             elif param_type == "bvec":
                 bvec = params
 
-        self.controls = None
         self.plot = BZPlotWidget(bvec)
         self.setCentralWidget(self.plot)
 
         self.controls = LatticeWidget(bvec)
         self.controls.sigChanged.connect(self.plot.set_bvec)
 
         self.__post_init__(execute=True)
@@ -275,15 +278,15 @@
 
         # self.params_latt.sigParameterChanged.connect(self.latt_changed)
         # self.params_avec.sigParameterChanged.connect(self.avec_changed)
         # self.params_bvec.sigParameterChanged.connect(self.bvec_changed)
 
     def closeEvent(self, event):
         super().closeEvent(event)
-        QtCore.QCoreApplication.instance().quit()
+        QtWidgets.QApplication.instance().quit()
 
     def block_params_signals(self, b: bool):
         self.params_latt.blockSignals(b)
         self.params_avec.blockSignals(b)
         self.params_bvec.blockSignals(b)
 
     def latt_changed(self):
```

### Comparing `erlab-2.3.2/src/erlab/interactive/colors.py` & `erlab-2.4.0/src/erlab/interactive/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,40 +97,40 @@
             self.thumbnails_loaded = True
         super().showPopup()
 
     def setPopupMinimumWidthForItems(self):
         view = self.view()
         fm = self.fontMetrics()
         maxWidth = max(
-            [fm.boundingRect(self.itemText(i)).width() for i in range(self.count())]
+            fm.boundingRect(self.itemText(i)).width() for i in range(self.count())
         )
-        if maxWidth:
+        if maxWidth and view is not None:
             view.setMinimumWidth(maxWidth)
 
     @QtCore.Slot()
     def nextIndex(self):
         self.wheelEvent(
             QtGui.QWheelEvent(
-                QtCore.QPoint(0, 0),
-                QtCore.QPoint(0, 0),
+                QtCore.QPointF(0, 0),
+                QtCore.QPointF(0, 0),
                 QtCore.QPoint(0, 0),
                 QtCore.QPoint(0, -15),
                 QtCore.Qt.MouseButton.NoButton,
                 QtCore.Qt.KeyboardModifier.NoModifier,
                 QtCore.Qt.ScrollPhase.ScrollUpdate,
                 True,
             )
         )
 
     @QtCore.Slot()
     def previousIndex(self):
         self.wheelEvent(
             QtGui.QWheelEvent(
-                QtCore.QPoint(0, 0),
-                QtCore.QPoint(0, 0),
+                QtCore.QPointF(0, 0),
+                QtCore.QPointF(0, 0),
                 QtCore.QPoint(0, 0),
                 QtCore.QPoint(0, 15),
                 QtCore.Qt.MouseButton.NoButton,
                 QtCore.Qt.KeyboardModifier.NoModifier,
                 QtCore.Qt.ScrollPhase.ScrollUpdate,
                 True,
             )
@@ -593,15 +593,15 @@
             all_cmaps = _mpl
         else:
             all_cmaps = local + _mpl
     return list(dict.fromkeys(all_cmaps))
 
 
 def pg_colormap_from_name(name: str, skipCache: bool = True) -> pg.ColorMap:
-    """Gets a :class:`pyqtgraph.ColorMap` from its name.
+    """Get a :class:`pyqtgraph.ColorMap` from its name.
 
     Parameters
     ----------
     name
         A valid colormap name.
     skipCache
         Whether to skip cache, by default `True`. Passed onto
@@ -669,15 +669,15 @@
     pg.colormap._mapCache = {}  # disable cache to reduce memory usage
     return cmap
 
 
 def pg_colormap_to_QPixmap(
     cmap: str | pg.ColorMap, w: int = 64, h: int = 16, skipCache: bool = True
 ) -> QtGui.QPixmap:
-    """Converts a :class:`pyqtgraph.ColorMap` to a ``w``-by-``h`` QPixmap thumbnail.
+    """Convert a :class:`pyqtgraph.ColorMap` to a ``w``-by-``h`` QPixmap thumbnail.
 
     Parameters
     ----------
     cmap
         The colormap.
     w, h
         Specifies the dimension of the pixmap.
@@ -686,15 +686,14 @@
         :func:`pg_colormap_from_name`.
 
     Returns
     -------
     PySide6.QtGui.QPixmap
 
     """
-
     if isinstance(cmap, str):
         cmap = pg_colormap_from_name(cmap, skipCache=skipCache)
     # cmap_arr = np.reshape(cmap.getColors()[:, None], (1, -1, 4), order='C')
     # cmap_arr = np.reshape(
     # cmap.getLookupTable(0, 1, w, alpha=True)[:, None], (1, -1, 4),
     # order='C')
     cmap_arr = cmap.getLookupTable(0, 1, w, alpha=True)[:, None]
```

### Comparing `erlab-2.3.2/src/erlab/interactive/curvefittingtool.py` & `erlab-2.4.0/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/derivative.py` & `erlab-2.4.0/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/dtool.ui` & `erlab-2.4.0/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/fermiedge.py` & `erlab-2.4.0/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.4.0/src/erlab/interactive/imagetool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 
 from __future__ import annotations
 
 __all__ = ["ImageTool", "itool"]
 
 import gc
 import sys
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, Literal, cast
 
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 from qtpy import QtCore, QtWidgets
 
 import erlab.io
 from erlab.interactive.imagetool.controls import (
     ItoolBinningControls,
     ItoolColormapControls,
     ItoolCrosshairControls,
 )
 from erlab.interactive.imagetool.core import ImageSlicerArea, SlicerLinkProxy
 from erlab.interactive.utilities import DictMenuBar, copy_to_clipboard
+from erlab.io.plugins.merlin import BL403Loader
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Sequence
 
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
 
@@ -83,15 +84,14 @@
     - If `link` is True, the ImageTool windows will be synchronized.
 
     Examples
     --------
     >>> itool(data, cmap="gray", gamma=0.5)
     >>> itool(data_list, link=True)
     """
-
     qapp = QtWidgets.QApplication.instance()
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
 
     if isinstance(qapp, QtWidgets.QApplication):
         qapp.setStyle("Fusion")
 
@@ -403,15 +403,17 @@
         self.action_dict["snapCursorAct"].blockSignals(False)
 
         cmap_props = self.slicer_area.colormap_properties
         for ca, k in zip(
             self.colorAct, ["reversed", "highContrast", "zeroCentered"], strict=True
         ):
             ca.blockSignals(True)
-            ca.setChecked(cmap_props[k])
+            ca.setChecked(
+                cmap_props[cast(Literal["reversed", "highContrast", "zeroCentered"], k)]
+            )
             ca.blockSignals(False)
 
     def _set_colormap_options(self):
         self.slicer_area.set_colormap(
             reversed=self.colorAct[0].isChecked(),
             highContrast=self.colorAct[1].isChecked(),
             zeroCentered=self.colorAct[2].isChecked(),
@@ -420,18 +422,19 @@
     def _copy_cursor_val(self):
         copy_to_clipboard(str(self.slicer_area.array_slicer._values))
 
     def _copy_cursor_idx(self):
         copy_to_clipboard(str(self.slicer_area.array_slicer._indices))
 
     def _open_file(self):
+        merlin_loader = cast(BL403Loader, erlab.io.loaders["merlin"])
         valid_loaders: dict[str, tuple[Callable, dict]] = {
             "xarray HDF5 Files (*.h5)": (erlab.io.load_hdf5, {}),
-            "ALS BL4.0.3 Raw Data (*.pxt)": (erlab.io.loaders["merlin"].load, {}),
-            "ALS BL4.0.3 Live (*.ibw)": (erlab.io.loaders["merlin"].load_live, {}),
+            "ALS BL4.0.3 Raw Data (*.pxt)": (merlin_loader.load, {}),
+            "ALS BL4.0.3 Live (*.ibw)": (merlin_loader.load_live, {}),
             "DA30 Raw Data (*.ibw *.pxt *.zip)": (erlab.io.loaders["da30"].load, {}),
             "SSRL BL5-2 Raw Data (*.h5)": (erlab.io.loaders["ssrl52"].load, {}),
             "NetCDF Files (*.nc *.nc4 *.cdf)": (xr.load_dataarray, {}),
         }
 
         dialog = QtWidgets.QFileDialog(self)
         dialog.setAcceptMode(QtWidgets.QFileDialog.AcceptMode.AcceptOpen)
```

### Comparing `erlab-2.3.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.4.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-.. deprecated:: 0.1
+.. deprecated:: 0.1.
 
     This module is deprecated, and is only kept for reference purposes.
     Use `erlab.interactive.imagetool` instead.
 
 """
 
 import sys
@@ -26,15 +26,15 @@
 from matplotlib.ticker import AutoLocator
 from matplotlib.widgets import Widget
 
 __all__ = ["mpl_itool"]
 
 
 def qt_style_names():
-    """Return a list of styles, default platform style first"""
+    """Return a list of styles, default platform style first."""
     default_style_name = QtWidgets.QApplication.style().objectName().lower()
     result = []
     for style in QtWidgets.QStyleFactory.keys():
         if style.lower() == default_style_name:
             result.insert(0, style)
         else:
             result.append(style)
@@ -42,15 +42,15 @@
 
 
 def change_style(style_name):
     QtWidgets.QApplication.setStyle(QtWidgets.QStyleFactory.create(style_name))
 
 
 def colormap_to_QPixmap(name: str, h=64):
-    """Convert matplotlib colormap to a 256-by-`h` QPixmap"""
+    """Convert matplotlib colormap to a 256-by-`h` QPixmap."""
     cmap = plt.colormaps[name]
     cmap_arr = cmap(np.tile(np.linspace(0, 1, 256), (h, 1))) * 255
     img = QtGui.QImage(
         cmap_arr.astype(np.uint8).data,
         cmap_arr.shape[1],
         cmap_arr.shape[0],
         QtGui.QImage.Format_RGBA8888,
@@ -167,16 +167,15 @@
         self.setColor(self._default)
 
     def setColor(self, color):
         self._color = color
         self.colorChanged.emit(color.getRgbF())
         if self._color:
             self.setStyleSheet(
-                "QWidget { background-color: %s; border: 0; }"
-                % self._color.name(QtGui.QColor.HexArgb)
+                f"QWidget {{ background-color: {self._color.name(QtGui.QColor.HexArgb)}; border: 0; }}"
             )
         else:
             self.setStyleSheet("")
 
     def color(self):
         return self._color
 
@@ -1045,17 +1044,18 @@
 
 class ImageToolNavBar(NavigationToolbar2QT):
     def __init__(self, canvas, parent, coordinates=True):
         self.parent = parent
         NavigationToolbar2QT.__init__(self, canvas, parent, coordinates=coordinates)
 
     def _icon(self, name):
-        """
-        Construct a `.QIcon` from an image file *name*, including the extension
-        and relative to Matplotlib's "images" data directory.
+        """Construct a `.QIcon` from an image file name.
+
+        The name must include the extension and be given relative to Matplotlib's
+        "images" data directory.
         """
         name = name.replace(".png", "")
         icons_dict = {
             # back = qta.icon('ph.arrow-arc-left-fill'),
             # forward = qta.icon('ph.arrow-arc-right-fill'),
             # filesave = qta.icon('ph.floppy-disk-fill'),
             # home = qta.icon('ph.corners-out-fill'),
```

### Comparing `erlab-2.3.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.4.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-.. deprecated:: 0.1
+.. deprecated:: 0.1.
 
     This module is deprecated, and is only kept for reference purposes.
     Use `erlab.interactive.imagetool` instead.
 
 """
 
 import colorsys
 import enum
+import importlib
 import sys
 import weakref
 from itertools import chain, compress
 from time import perf_counter
 
 import matplotlib.mathtext
 import numba
-import numbagg
 import numpy as np
 import pyqtgraph as pg
 import qtawesome as qta
 from matplotlib import colors as mcolors
 from matplotlib import figure, rc_context
 from matplotlib.backends import backend_agg, backend_svg
 from matplotlib.font_manager import FontProperties
@@ -34,14 +34,20 @@
 )
 from erlab.interactive.utilities import parse_data, xImageItem
 
 # pg.setConfigOption('useNumba', True)
 # pg.setConfigOption('background', 'w')
 # pg.setConfigOption('foreground', 'k')
 
+if importlib.util.find_spec("numbagg"):
+    import numbagg
+
+    _general_nanmean_func = numbagg.nanmean
+else:
+    _general_nanmean_func = np.nanmean
 
 __all__ = ["itool_", "pg_itool"]
 
 suppressnanwarning = np.testing.suppress_warnings()
 suppressnanwarning.filter(RuntimeWarning, r"All-NaN (slice|axis) encountered")
 
 
@@ -239,15 +245,15 @@
                 "`objectName` argument to set a new name."
             )
         # self.setStyleSheet("QGroupBox#" + name + " {border:0;}")
         self.setContentsMargins(0, 0, 0, 0)
 
 
 def qt_style_names():
-    """Return a list of styles, default platform style first"""
+    """Return a list of styles, default platform style first."""
     default_style_name = QtWidgets.QApplication.style().objectName().lower()
     result = []
     for style in QtWidgets.QStyleFactory.keys():
         if style.lower() == default_style_name:
             result.insert(0, style)
         else:
             result.append(style)
@@ -358,16 +364,15 @@
         self.setColor(self._default)
 
     def setColor(self, color):
         self._color = color
         self.colorChanged.emit(color.getRgbF())
         if self._color:
             self.setStyleSheet(
-                "QWidget { background-color: %s; border: 0; }"
-                % self._color.name(QtGui.QColor.HexArgb)
+                f"QWidget {{ background-color: {self._color.name(QtGui.QColor.HexArgb)}; border: 0; }}"
             )
         else:
             self.setStyleSheet("")
 
     def color(self):
         return self._color
 
@@ -500,15 +505,15 @@
     def changeEvent(self, evt):
         if evt.type() == QtCore.QEvent.PaletteChange:
             self.label.updateStyle()
         super().changeEvent(evt)
 
 
 def get_pixmap_label(s: str, prop=None, dpi=300, **text_kw):
-    """Creates a QtGui.QPixmap from a mathtext string.
+    """Create a QtGui.QPixmap from a mathtext string.
 
     Parameters
     ----------
     s : str
         Mathtext string to be rendered.
     prop : matplotlib.font_manager.FontProperties
         Font properties.
@@ -516,19 +521,17 @@
         Dots per inch of the created pixmap.
     **text_kw : dict, optional
         Extra arguments to `matplotlib.figure.Figure.text`: refer to the
         `matplotlib` documentation for a list of all possible arguments.
 
     Returns
     -------
-
     A QtGui.QPixmap object.
 
     """
-
     parser = matplotlib.mathtext.MathTextParser("path")
     if prop is None:
         prop = FontProperties(size=9)
     width, height, depth, _, _ = parser.parse(s, dpi=72, prop=prop)
     fig = figure.Figure(figsize=(width / 72.0, height / 72.0), dpi=dpi)
     fig.patch.set_facecolor("none")
     text_kw["fontproperties"] = prop
@@ -541,15 +544,15 @@
     pixmap = QtGui.QPixmap(img.rgbSwapped())
     return pixmap
 
 
 def get_svg_label(
     s: str, outfile: QtCore.QTemporaryFile, prop=None, dpi=300, **text_kw
 ):
-    """Creates an SVG image from a mathtext string.
+    """Create an SVG image from a mathtext string.
 
     Parameters
     ----------
     s : str
         Mathtext string to be rendered.
     outfile : QtCore.QTemporaryFile
         Output temp file to store the SVG.
@@ -563,15 +566,14 @@
 
     Returns
     -------
     filename : str
         Name of the output file containing the rendered SVG.
 
     """
-
     parser = matplotlib.mathtext.MathTextParser("path")
     if prop is None:
         prop = FontProperties(size=12)
     width, height, depth, _, _ = parser.parse(s, dpi=1000, prop=prop)
     fig = figure.Figure(figsize=(width / 1000.0, height / 1000.0), dpi=dpi)
     fig.patch.set_facecolor("none")
     text_kw["fontproperties"] = prop
@@ -884,17 +886,14 @@
     Signals
     -------
     sigDataChanged()
     sigIndexChanged(indices, values)
 
     """
 
-    # !TODO: ctrl + A to view all
-    # !TODO: auto adjust limits on transpose
-
     sigDataChanged = QtCore.Signal(object)  #: :meta private:
     sigIndexChanged = QtCore.Signal(list, list)  #: :meta private:
 
     _only_axis = ("x", "y", "z", "t")
     _only_maps = "maps"
 
     def _get_middle_index(self, x):
@@ -1420,15 +1419,15 @@
             #     if ax in self.ci.items.keys():
             #         self.removeItem(ax)
             #     self.addItem(ax, *ref_dims[a])
             self.addItem(self.axes[group[0]], *anchors[0], *ref_dims[axis][2:])
             self.addItem(self.axes[group[1]], *anchors[1], *ref_dims[axis][2:])
 
     def set_labels(self, labels=None):
-        """labels: list or tuple of str"""
+        """labels: list or tuple of str."""
         if labels is None:
             labels = self.data_dims
         # 0: default, 1: svg, 2: pixmap
         labelmode = ItoolAxisItem.LabelType.TextLabel
         if labelmode is ItoolAxisItem.LabelType.TextLabel:
             labels_ = labels
         else:
@@ -1577,15 +1576,15 @@
 
     def _measure_fps(self):
         now = perf_counter()
         fps = 1.0 / (now - self._fpsLastUpdate)
         self._fpsLastUpdate = now
         w = 0.8
         self._avg_fps = self._avg_fps * (1 - w) + fps * w
-        self.axes[1].setTitle("%0.2f fps" % self._avg_fps)
+        self.axes[1].setTitle(f"{self._avg_fps:0.2f} fps")
 
     def labelify(self, text):
         """Prettify some frequently used axis labels."""
         labelformats = {
             "kx": "$k_x$",
             "ky": "$k_y$",
             "kz": "$k_z$",
@@ -1694,33 +1693,33 @@
         axis -= 1
         if not self.averaged[axis + 1]:
             return self.data_vals_T[
                 (slice(None),) * (axis % self.data_ndim)
                 + (self._get_bin_slice(axis + 1),)
             ].squeeze(axis=axis)
         else:
-            return numbagg.nanmean(
+            return _general_nanmean_func(
                 self.data_vals_T[
                     (slice(None),) * (axis % self.data_ndim)
                     + (self._get_bin_slice(axis + 1),)
                 ],
                 axis=axis,
             )
 
     def _binned_profile(self, avg_axis):
         if not any(self.averaged):
             return self._block_slicer(avg_axis, [self._last_ind[i] for i in avg_axis])
         slices = tuple(self._get_bin_slice(ax) for ax in avg_axis)
         return self._block_slice_avg(avg_axis, slices)
         # self._slice_block = self._block_slicer(avg_axis, slices)
-        # return numbagg.nanmean(self._slice_block, axis=[(ax - 1) for ax in avg_axis])
+        # return _general_nanmean_func(self._slice_block, axis=[(ax - 1) for ax in avg_axis])
 
     def _block_slice_avg(self, axis=None, slices=None):
         axis = [(ax - 1) % self.data_ndim for ax in axis]
-        return numbagg.nanmean(
+        return _general_nanmean_func(
             self.data_vals_T[
                 tuple(
                     slices[axis.index(d)] if d in axis else slice(None)
                     for d in range(self.data_ndim)
                 )
             ],
             axis=axis,
@@ -1793,15 +1792,15 @@
         if (Qmods & QtCore.Qt.ControlModifier) == QtCore.Qt.ControlModifier:
             mods.append("control")
         if (Qmods & QtCore.Qt.AltModifier) == QtCore.Qt.AltModifier:
             mods.append("alt")
         return mods
 
     def _get_mouse_datapos(self, plot, pos):
-        """Returns mouse position in data coords"""
+        """Return mouse position in data coords."""
         mouse_point = plot.vb.mapSceneToView(pos)
         return mouse_point.x(), mouse_point.y()
 
     def onMouseDrag(self, evt):
         try:
             axis_ind, datapos = self._get_curr_axes_index(evt.scenePos())
         except AttributeError:
@@ -2309,15 +2308,14 @@
                    continuous lines)
     extendToEdge   If True, extend the curves to reach the exact edges of
                    the data.
     path           if True, return a QPainterPath rather than a list of
                    vertex coordinates.
     ============== =========================================================
     """
-
     if path is True:
         connected = True
     np.nan_to_num(data, copy=False)
     if extendToEdge:
         data = fast_isocurve_extend(data)
 
     # mark everything below the isosurface level
@@ -3050,15 +3048,15 @@
                 self.load_thumbnail(i)
             self.thumbnails_loaded = True
         super().showPopup()
 
     def setPopupMinimumWidthForItems(self):
         view = self.view()
         fm = self.fontMetrics()
-        maxWidth = max([fm.width(self.itemText(i)) for i in range(self.count())])
+        maxWidth = max(fm.width(self.itemText(i)) for i in range(self.count()))
         if maxWidth:
             view.setMinimumWidth(maxWidth)
 
     def hidePopup(self):
         self.activated.emit(self.currentIndex())
         self.textActivated.emit(self.currentText())
         self.currentIndexChanged.emit(self.currentIndex())
```

### Comparing `erlab-2.3.2/src/erlab/interactive/imagetool/controls.py` & `erlab-2.4.0/src/erlab/interactive/imagetool/controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
+"""Widgets for controlling `ImageSlicerArea`."""
+
 from __future__ import annotations
 
 __all__ = [
-    "ColorControls",
     "ItoolBinningControls",
+    "ItoolColorControls",
     "ItoolColormapControls",
+    "ItoolControlsBase",
     "ItoolCrosshairControls",
 ]
 
-from typing import TYPE_CHECKING
+import types
+from typing import TYPE_CHECKING, cast
 
 import numpy as np
 import pyqtgraph as pg
 import qtawesome as qta
 from qtpy import QtCore, QtGui, QtWidgets
-import types
+
 from erlab.interactive.colors import ColorMapComboBox, ColorMapGammaWidget
 from erlab.interactive.utilities import BetterSpinBox
 
 if TYPE_CHECKING:
-    import xarray as xr
     from collections.abc import Mapping
 
+    import xarray as xr
+
     from erlab.interactive.imagetool.core import ImageSlicerArea
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
 
 class IconButton(QtWidgets.QPushButton):
     ICON_ALIASES: Mapping[str, str] = types.MappingProxyType(
         {
@@ -134,18 +139,18 @@
         return self.slicer_area.n_cursors
 
     @property
     def current_cursor(self) -> int:
         return self.slicer_area.current_cursor
 
     def initialize_layout(self):
-        self.setLayout(QtWidgets.QHBoxLayout(self))
-        self.layout().setContentsMargins(0, 0, 0, 0)
-
-        self.layout().setSpacing(3)
+        layout = QtWidgets.QHBoxLayout(self)
+        self.setLayout(layout)
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(3)
 
     def initialize_widgets(self):
         for ctrl in self.sub_controls:
             if isinstance(ctrl, ItoolControlsBase):
                 ctrl.initialize_widgets()
 
     def connect_signals(self):
@@ -178,27 +183,27 @@
         if isinstance(self._slicer_area, ItoolControlsBase):
             return self._slicer_area.slicer_area
         else:
             return self._slicer_area
 
     @slicer_area.setter
     def slicer_area(self, value: ImageSlicerArea):
-        """
-        Initially, the goal was to be able to control multiple `ImageSlicerArea`s
-        with a single control widget, so the control widgets were designed with easy
-        connection and disconnection of signals in mind. However, this has become
-        largely unnecessary since we now have `SlicerLinkProxy` as a translation layer
-        between multiple `ImageSlicerArea`s with individual control widgets. Hence, this
-        method will remain unused for the time being.
+        """Set the `ImageSlicerArea` instance for the control widget.
+
+        Initially, the goal was to be able to control multiple `ImageSlicerArea`s with a
+        single control widget, so the control widgets were designed with easy connection
+        and disconnection of signals in mind. However, this has become largely
+        unnecessary since we now have `SlicerLinkProxy` as a translation layer between
+        multiple `ImageSlicerArea`s with individual control widgets. Hence, this method
+        will remain unused for the time being.
 
         Also, in principle, most of the control widgets along with the menu bar should
         be re-written to use QActions...
 
         """
-
         # ignore until https://bugreports.qt.io/browse/PYSIDE-229 is fixed
         try:
             self.disconnect_signals()
         except RuntimeError:
             pass
         self._slicer_area = value
         clear_layout(self.layout())
@@ -301,20 +306,23 @@
             self.values_layouts[0].addWidget(self.spin_dat, 2, 0, 1, 3)
         else:
             self.values_layouts[0].addWidget(self.btn_add, 0, 1, 1, 1)
             self.values_layouts[0].addWidget(self.btn_rem, 0, 2, 1, 1)
             self.values_layouts[0].addWidget(self.btn_snap, 0, 3, 1, 1)
             self.values_layouts[0].addWidget(self.cb_cursors, 0, 0, 1, 1)
             self.values_layouts[0].addWidget(self.spin_dat, 0, 4, 1, 1)
-        self.layout().addWidget(self.values_groups[0])
+        cast(QtWidgets.QLayout, self.layout()).addWidget(self.values_groups[0])
 
         # info widgets
         self.label_dim = tuple(
-            QtWidgets.QPushButton(grp, checkable=True) for grp in self.values_groups[1:]
+            QtWidgets.QPushButton(grp) for grp in self.values_groups[1:]
         )
+        for lab in self.label_dim:
+            lab.setCheckable(True)
+
         self.spin_idx = tuple(
             BetterSpinBox(
                 grp,
                 integer=True,
                 singleStep=1,
                 wrapping=False,
                 minimumWidth=60,
@@ -360,15 +368,15 @@
                 self.values_layouts[i + 1].addWidget(self.spin_val[i], 2, 0, 1, 2)
             else:
                 self.values_layouts[i + 1].addWidget(self.label_dim[i], 0, 0, 1, 1)
                 self.values_layouts[i + 1].addWidget(self.btn_transpose[i], 0, 1, 1, 1)
                 self.values_layouts[i + 1].addWidget(self.spin_idx[i], 0, 2, 1, 1)
                 self.values_layouts[i + 1].addWidget(self.spin_val[i], 0, 3, 1, 1)
 
-            self.layout().addWidget(self.values_groups[i + 1])
+            cast(QtWidgets.QLayout, self.layout()).addWidget(self.values_groups[i + 1])
 
     def _transpose_axes(self, idx):
         if self.data.ndim == 4:
             if idx == 3:
                 self.slicer_area.swap_axes(0, 2)
             else:
                 self.slicer_area.swap_axes(idx, (idx + 1) % 4)
@@ -522,15 +530,15 @@
         self.update_spins()
 
     @QtCore.Slot(str)
     def setActiveCursor(self, value: str):
         self.slicer_area.set_current_cursor(self.cb_cursors.findText(value))
 
 
-class ColorControls(ItoolControlsBase):
+class ItoolColorControls(ItoolControlsBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def initialize_widgets(self):
         self.btn_reverse = IconButton(
             on="invert",
             off="invert_off",
@@ -554,18 +562,19 @@
             checkable=True,
             toolTip="Lock color limits",
         )
         self.btn_reverse.toggled.connect(self.update_colormap)
         self.btn_contrast.toggled.connect(self.update_colormap)
         self.btn_zero.toggled.connect(self.update_colormap)
 
-        self.layout().addWidget(self.btn_reverse)
-        self.layout().addWidget(self.btn_contrast)
-        self.layout().addWidget(self.btn_zero)
-        self.layout().addWidget(self.btn_lock)
+        layout = cast(QtWidgets.QLayout, self.layout())
+        layout.addWidget(self.btn_reverse)
+        layout.addWidget(self.btn_contrast)
+        layout.addWidget(self.btn_zero)
+        layout.addWidget(self.btn_lock)
 
     def update(self):
         self.btn_reverse.blockSignals(True)
         self.btn_contrast.blockSignals(True)
         self.btn_zero.blockSignals(True)
         self.btn_lock.blockSignals(True)
 
@@ -610,36 +619,38 @@
         super().__init__(*args, **kwargs)
 
     def initialize_layout(self):
         if self.orientation == QtCore.Qt.Orientation.Vertical:
             self.setLayout(QtWidgets.QVBoxLayout(self))
         else:
             self.setLayout(QtWidgets.QHBoxLayout(self))
-        self.layout().setContentsMargins(0, 0, 0, 0)
 
-        self.layout().setSpacing(3)
+        layout = cast(QtWidgets.QBoxLayout, self.layout())
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(3)
 
     def initialize_widgets(self):
         super().initialize_widgets()
         self.cb_colormap = ColorMapComboBox(self, maximumWidth=175)
         self.cb_colormap.textActivated.connect(self.change_colormap)
 
         self.gamma_widget = ColorMapGammaWidget(spin_cls=BetterSpinBox)
         self.gamma_widget.valueChanged.connect(
             lambda g: self.slicer_area.set_colormap(gamma=g)
         )
         self.gamma_widget.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed
         )
 
-        self.misc_controls = self.add_control(ColorControls(self))
+        self.misc_controls = self.add_control(ItoolColorControls(self))
 
-        self.layout().addWidget(self.cb_colormap)
-        self.layout().addWidget(self.gamma_widget)
-        self.layout().addWidget(self.misc_controls)
+        layout = cast(QtWidgets.QBoxLayout, self.layout())
+        layout.addWidget(self.cb_colormap)
+        layout.addWidget(self.gamma_widget)
+        layout.addWidget(self.misc_controls)
 
     def update(self):
         super().update()
         if isinstance(self.slicer_area.colormap, str):
             self.cb_colormap.setDefaultCmap(self.slicer_area.colormap)
         self.gamma_widget.blockSignals(True)
         self.gamma_widget.setValue(self.slicer_area.colormap_properties["gamma"])
@@ -662,17 +673,18 @@
 
 class ItoolBinningControls(ItoolControlsBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def initialize_layout(self):
         self.setLayout(QtWidgets.QGridLayout(self))
-        self.layout().setContentsMargins(0, 0, 0, 0)
 
-        self.layout().setSpacing(3)
+        layout = cast(QtWidgets.QGridLayout, self.layout())
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(3)
 
     def initialize_widgets(self):
         super().initialize_widgets()
         self.labels = tuple(QtWidgets.QLabel() for _ in range(self.data.ndim))
         self.spins = tuple(
             BetterSpinBox(
                 self,
@@ -694,19 +706,20 @@
 
         self.all_btn = IconButton(
             on="all_cursors",
             checkable=True,
             toolTip="Apply for all cursors",
         )
 
+        layout = cast(QtWidgets.QGridLayout, self.layout())
         for i in range(self.data.ndim):
-            self.layout().addWidget(self.labels[i], 0, i, 1, 1)
-            self.layout().addWidget(self.spins[i], 1, i, 1, 1)
-        self.layout().addWidget(self.reset_btn, 2, 0, 1, 1)
-        self.layout().addWidget(self.all_btn, 2, 1, 1, 1)
+            layout.addWidget(self.labels[i], 0, i, 1, 1)
+            layout.addWidget(self.spins[i], 1, i, 1, 1)
+        layout.addWidget(self.reset_btn, 2, 0, 1, 1)
+        layout.addWidget(self.all_btn, 2, 1, 1, 1)
         # for spin in self.spins:
         # spin.setMinimumWidth(60)
 
     def _update_bin(self, axis, n):
         if self.all_btn.isChecked():
             self.slicer_area.set_bin_all(axis, n)
         else:
```

### Comparing `erlab-2.3.2/src/erlab/interactive/imagetool/core.py` & `erlab-2.4.0/src/erlab/interactive/imagetool/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,17 +111,15 @@
 def link_slicer(
     func: Callable | None = None,
     *,
     indices: bool = False,
     steps: bool = False,
     color: bool = False,
 ):
-    """
-    An internal decorator for choosing which functions to sync accross multiple
-    instances of `ImageSlicerArea`.
+    """Sync decorated methods across multiple `ImageSlicerArea` instances.
 
     Parameters
     ----------
     func
         The method to sync across multiple instances of `ImageSlicerArea`.
     indices
         If `True`, the input argument named `value` given to `func` are interpreted as
@@ -149,17 +147,23 @@
             if args[0].is_linked:
                 if not skip_sync:
                     all_args = inspect.Signature.from_callable(func).bind(
                         *args, **kwargs
                     )
                     all_args.apply_defaults()
                     obj: ImageSlicerArea = all_args.arguments.pop("self")
-                    obj._linking_proxy.sync(
-                        obj, func.__name__, all_args.arguments, indices, steps, color
-                    )
+                    if obj._linking_proxy is not None:
+                        obj._linking_proxy.sync(
+                            obj,
+                            func.__name__,
+                            all_args.arguments,
+                            indices,
+                            steps,
+                            color,
+                        )
             return out
 
         return wrapped
 
     if func is not None:
         return my_decorator(func)
     return my_decorator
@@ -201,15 +205,15 @@
         source: ImageSlicerArea,
         funcname: str,
         arguments: dict[str, Any],
         indices: bool,
         steps: bool,
         color: bool,
     ):
-        """The core method that propagates changes across multiple `ImageSlicerArea`s.
+        """Propagate changes across multiple `ImageSlicerArea`s.
 
         This method is invoked every time a method decorated with :func:`link_slicer` in
         a linked `ImageSlicerArea` is called.
 
         Parameters
         ----------
         source
@@ -329,30 +333,30 @@
 
     sigDataChanged = QtCore.Signal()  #: :meta private:
     sigCurrentCursorChanged = QtCore.Signal(int)  #: :meta private:
     sigViewOptionChanged = QtCore.Signal()  #: :meta private:
 
     @property
     def sigCursorCountChanged(self) -> QtCore.SignalInstance:
-        """:meta private:"""
+        """:meta private:"""  # noqa: D400
         return self.array_slicer.sigCursorCountChanged
 
     @property
     def sigIndexChanged(self) -> QtCore.SignalInstance:
-        """:meta private:"""
+        """:meta private:"""  # noqa: D400
         return self.array_slicer.sigIndexChanged
 
     @property
     def sigBinChanged(self) -> QtCore.SignalInstance:
-        """:meta private:"""
+        """:meta private:"""  # noqa: D400
         return self.array_slicer.sigBinChanged
 
     @property
     def sigShapeChanged(self) -> QtCore.SignalInstance:
-        """:meta private:"""
+        """:meta private:"""  # noqa: D400
         return self.array_slicer.sigShapeChanged
 
     def __init__(
         self,
         parent: QtWidgets.QWidget | None = None,
         data: xr.DataArray | npt.ArrayLike | None = None,
         cmap: str | pg.ColorMap = "magma",
@@ -401,15 +405,15 @@
         self.cursor_colors: list[QtGui.QColor] = [self.COLORS[0]]
 
         self._colorbar = ItoolColorBar(self)
         layout.addWidget(self._colorbar)
         self._colorbar.setVisible(False)
 
         pkw = {"image_cls": image_cls, "plotdata_cls": plotdata_cls}
-        self.manual_limits: dict[str, list[list[float]]] = {}
+        self.manual_limits: dict[str, list[float]] = {}
         self._plots: tuple[ItoolGraphicsLayoutWidget, ...] = (
             ItoolGraphicsLayoutWidget(self, image=True, display_axis=(0, 1), **pkw),
             ItoolGraphicsLayoutWidget(self, display_axis=(0,), **pkw),
             ItoolGraphicsLayoutWidget(self, display_axis=(1,), is_vertical=True, **pkw),
             ItoolGraphicsLayoutWidget(self, display_axis=(2,), **pkw),
             ItoolGraphicsLayoutWidget(self, image=True, display_axis=(0, 2), **pkw),
             ItoolGraphicsLayoutWidget(self, image=True, display_axis=(2, 1), **pkw),
@@ -454,15 +458,15 @@
 
         if self.bench:
             print("\n")
 
     def on_close(self):
         self.array_slicer.clear_cache()
         self.data.close()
-        if hasattr(self, "_data"):
+        if hasattr(self, "_data") and self._data is not None:
             self._data.close()
             del self._data
 
     def connect_axes_signals(self):
         for ax in self.axes:
             ax.connect_signals()
 
@@ -476,15 +480,16 @@
         self.sigShapeChanged.connect(self.refresh_all)
         self.sigCursorCountChanged.connect(lambda: self.set_colormap(update=True))
 
     def add_link(self, proxy: SlicerLinkProxy):
         proxy.add(self)
 
     def remove_link(self):
-        self._linking_proxy.remove(self)
+        if self.is_linked:
+            cast(SlicerLinkProxy, self._linking_proxy).remove(self)
 
     @property
     def is_linked(self) -> bool:
         return self._linking_proxy is not None
 
     @property
     def colormap(self) -> str | pg.ColorMap:
@@ -510,24 +515,24 @@
         else:
             profile_axes = [1, 2, 3, 6]
 
         return tuple(self.get_axes(ax) for ax in profile_axes)
 
     @property
     def main_image(self) -> ItoolPlotItem:
-        """returns the main PlotItem"""
+        """Return the main PlotItem."""
         return self.get_axes(0)
 
     @property
     def images(self) -> tuple[ItoolPlotItem, ...]:
         return (self.main_image, *self.slices)
 
     @property
     def axes(self) -> tuple[ItoolPlotItem, ...]:
-        """Currently valid subset of self._plots"""
+        """Currently valid subset of self._plots."""
         return self.images + self.profiles
 
     @property
     def _imageitems(self) -> tuple[ItoolImageItem, ...]:
         return tuple(im for ax in self.images for im in ax.slicer_data_items)
 
     @property
@@ -614,14 +619,30 @@
         if update:
             self.refresh_current()
         self.sigCurrentCursorChanged.emit(cursor)
 
     def set_data(
         self, data: xr.DataArray | npt.ArrayLike, rad2deg: bool | Iterable[str] = False
     ):
+        """Set the data to be displayed.
+
+        Parameters
+        ----------
+        data
+            The data to be displayed. If a `xarray.DataArray` is given, the
+            dimensions and coordinates are used to determine the axes of the plots. If a
+            :class:`xarray.Dataset` is given, the first data variable is used. If a
+            :class:`numpy.ndarray` is given, it is converted to a `xarray.DataArray`
+            with default dimensions.
+        rad2deg
+            If `True`, converts coords along dimensions that have angle-like names to
+            degrees. If an iterable of strings is given, coordinates for dimensions that
+            correspond to the given strings are converted.
+
+        """
         if hasattr(self, "_array_slicer"):
             n_cursors_old = self.n_cursors
             if isinstance(self._data, xr.DataArray):
                 self._data.close()
             del self._data
             self.disconnect_axes_signals()
         else:
@@ -666,14 +687,60 @@
         self.sigDataChanged.emit()
 
         # self.refresh_current()
         self.set_colormap(update=True)
         self._colorbar.cb.setImageItem()
         self.lock_levels(False)
 
+    def update_values(self, values: npt.NDArray | xr.DataArray, update: bool = True):
+        """Update only the values of the data.
+
+        The coords and shape of the data array are not changed.
+
+        Parameters
+        ----------
+        values
+            The new values to be set. If a `xarray.DataArray` is given, the dimensions
+            must match the current data array. If a `numpy.ndarray` is given, the shape
+            must match the current data array. Note that if the user has transposed the
+            current data array, passing a `numpy.ndarray` with the original shape will
+            fail.
+        update
+            If `True`, the plots are updated after setting the new values.
+
+        Note
+        ----
+        This method only checks for matching dimension name and shape, and does not
+        check for equal coordinate values.
+
+        """
+        if isinstance(values, xr.DataArray):
+            if self.array_slicer._obj.ndim != values.ndim:
+                raise ValueError("DataArray dimensions do not match")
+            if set(self.array_slicer._obj.dims) != set(values.dims):
+                raise ValueError("DataArray dimensions do not match")
+
+            if self.array_slicer._obj.dims != values.dims:
+                values = values.transpose(*self.array_slicer._obj.dims)
+            if self.array_slicer._obj.shape != values.shape:
+                raise ValueError("DataArray shape does not match")
+
+            values = values.values
+        else:
+            if self.array_slicer._obj.shape != values.shape:
+                raise ValueError(
+                    "Data shape does not match. Array is "
+                    f"{self.array_slicer._obj.shape} but {values.shape} given"
+                )
+        self.array_slicer._obj[:] = values
+
+        if update:
+            self.array_slicer.clear_val_cache(include_vals=True)
+            self.refresh_all(only_plots=True)
+
     @QtCore.Slot(int, int)
     @link_slicer
     def swap_axes(self, ax1: int, ax2: int):
         self.array_slicer.swap_axes(ax1, ax2)
 
     @QtCore.Slot(int, int, bool)
     @link_slicer(indices=True)
@@ -844,15 +911,15 @@
     def adjust_layout(
         self,
         horiz_pad: int = 45,
         vert_pad: int = 30,
         font_size: float = 11.0,
         r: tuple[float, float, float, float] = (1.2, 1.5, 3.0, 1.0),
     ):
-        """Determines the padding and aspect ratios.
+        """Determine the padding and aspect ratios.
 
         Parameters
         ----------
         horiz_pad, vert_pad
             Reserved space for the x and y axes.
         font_size
             Font size in points.
@@ -875,15 +942,14 @@
                  │           │       │   │
             r[2] │     0     │   5   │ 2 │
                  │           │       │   │
                  └───────────┴───────┴───┘
                   r[3] * r[2]
 
         """
-
         font = QtGui.QFont()
         font.setPointSizeF(float(font_size))
 
         valid_axis: tuple[tuple[Literal[0, 1], ...], ...] = (
             (1, 0, 0, 1),
             (1, 1, 0, 0),
             (0, 0, 1, 1),
@@ -1229,15 +1295,15 @@
             self.axis_dims,
             self.vb.state["autoRange"],
             self.vb.state["viewRange"],
             strict=True,
         ):
             if dim is not None:
                 if auto:
-                    self.slicer_area.manual_limits.pop("dim", None)
+                    self.slicer_area.manual_limits.pop(dim, None)
                 else:
                     self.slicer_area.manual_limits[dim] = rng
 
     def update_manual_range(self):
         if self.is_independent:
             return
         self.set_range_from(self.slicer_area.manual_limits)
@@ -1506,28 +1572,30 @@
 
     def set_active_cursor(self, index: int):
         if self.is_image:
             for i, item in enumerate(self.slicer_data_items):
                 item.setVisible(i == index)
 
     def save_current_data(self, fileName=None):
+        default_name = "data"
+        if self.slicer_area._data is not None:
+            default_name = str(self.slicer_area._data.name)
+
         if fileName is None:
             self.fileDialog = QtWidgets.QFileDialog()
             self.fileDialog.setFileMode(QtWidgets.QFileDialog.FileMode.AnyFile)
             self.fileDialog.setAcceptMode(QtWidgets.QFileDialog.AcceptMode.AcceptSave)
             self.fileDialog.setNameFilter("xarray HDF5 Files (*.h5)")
             if pg.PlotItem.lastFileDir is not None:
                 self.fileDialog.setDirectory(
-                    os.path.join(
-                        pg.PlotItem.lastFileDir, f"{self.slicer_area._data.name}.h5"
-                    )
+                    os.path.join(pg.PlotItem.lastFileDir, f"{default_name}.h5")
                 )
             else:
                 self.fileDialog.setDirectory(
-                    os.path.join(os.getcwd(), f"{self.slicer_area._data.name}.h5")
+                    os.path.join(os.getcwd(), f"{default_name}.h5")
                 )
             self.fileDialog.show()
             self.fileDialog.fileSelected.connect(self.save_current_data)
             return
 
         fileName = str(fileName)
         pg.PlotItem.lastFileDir = os.path.dirname(fileName)
```

### Comparing `erlab-2.3.2/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.4.0/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-"""
-This module provides a fast, parallelized version of nanmean that supports multiple axes
-based on numba. Enables efficient real-time multidimensional binning.
+"""Fast parallelized averaging for multidimensional arrays.
+
+This module provides a numba-based fast, parallelized version of nanmean that supports
+multiple axes. This enables efficient real-time multidimensional binning.
 
 """
 
-__all__ = ["fast_nanmean"]
+__all__ = ["NANMEAN_FUNCS", "fast_nanmean", "fast_nanmean_skipcheck"]
 
-from collections.abc import Collection
+import importlib
+from collections.abc import Callable, Collection
 
 import numba
 import numba.core.registry
 import numba.typed
-import numbagg
 import numpy as np
 import numpy.typing as npt
 
+if importlib.util.find_spec("numbagg"):
+    import numbagg
+
+    _general_nanmean_func: Callable = numbagg.nanmean
+else:
+    _general_nanmean_func = np.nanmean
+
+# _SIG_N_M: List of signatures that reduces from N to M dimensions.
+
 _SIG_2_1 = [
     numba.types.Array(numba.float64, 1, "C")(numba.types.Array(numba.float32, 2, "C")),
     numba.types.Array(numba.float64, 1, "C")(numba.types.Array(numba.float32, 2, "A")),
     numba.types.Array(numba.float64, 1, "C")(numba.types.Array(numba.float64, 2, "C")),
     numba.types.Array(numba.float64, 1, "C")(numba.types.Array(numba.float64, 2, "A")),
 ]
 _SIG_3_1 = [
@@ -269,15 +279,15 @@
     n = a.shape[0]
     output = np.empty(n, dtype=np.float64)
     for i in numba.prange(n):
         output[i] = np.nanmean(a[i, :, :, :])
     return output
 
 
-nanmean_funcs = {
+NANMEAN_FUNCS: dict[int, dict[int | frozenset[int], Callable]] = {
     2: {
         0: _nanmean_2_0,
         1: _nanmean_2_1,
         frozenset({0}): _nanmean_2_0,
         frozenset({1}): _nanmean_2_1,
     },
     3: {
@@ -307,78 +317,91 @@
         frozenset({1, 3}): _nanmean_4_13,
         frozenset({2, 3}): _nanmean_4_23,
         frozenset({0, 1, 2}): _nanmean_4_012,
         frozenset({0, 1, 3}): _nanmean_4_013,
         frozenset({0, 2, 3}): _nanmean_4_023,
         frozenset({1, 2, 3}): _nanmean_4_123,
     },
-}
+}  #: Mapping from array dimensions to axis combinations to corresponding functions.
 
 
 def fast_nanmean(
     a: npt.NDArray[np.float32 | np.float64], axis: int | Collection[int] | None = None
 ) -> npt.NDArray[np.float32 | np.float64] | np.float64:
-    """A fast, parallelized arithmetic mean for floating point arrays that ignores NaNs.
+    """Compute the mean for floating point arrays while ignoring NaNs.
 
     Parameters
     ----------
     a
         A numpy array of floats.
     axis
         Axis or iterable of axis along which the means are computed. If `None`, the mean
         of the flattend array is computed.
 
     Returns
     -------
     numpy.ndarray or float
         The calculated mean. The output array is always C-contiguous.
 
-    Note
-    ----
-    Parallelization is only applied for :code:`N`-dimensional arrays with :code:`N <= 4`
-    and :code:`len(axis) < N`. For bigger :code:`N`, :obj:`numbagg.nanmean` is used. For
-    calculating the average of a flattened array (:code:`axis = None` or
-    :code:`len(axis) == N`), the :obj:`numba` implemenation of :obj:`numpy.nanmean` is
-    used. This function does not keep the input dimensions, i.e., the output is
-    squeezed.
+    Notes
+    -----
+    - Parallelization is only applied for ``N``-dimensional arrays with ``N <= 4`` and
+      ``len(axis) < N``.
+
+    - For calculating the average of a flattened array (``axis = None`` or ``len(axis)
+      == N``), the `numba` implemenation of `numpy.nanmean` is used.
+
+    - For bigger ``N``, ``numbagg.nanmean`` is used if `numbagg
+      <https://github.com/numbagg/numbagg>`_ is installed. Otherwise, the calculation
+      falls back to `numpy.nanmean`.
+
+    - This function does not keep the input dimensions, i.e., the output is squeezed.
+
+    - For single precision input, the calculation is performed in double precision and
+      converted back to single precision. This may lead to different results compared to
+      `numpy.nanmean`.
 
     """
     if a.ndim == 1 or axis is None:
         return _nanmean_all(a)
     elif a.ndim > 4:
-        return np.ascontiguousarray(numbagg.nanmean(a, axis))  # type: ignore[arg-type]
+        return np.ascontiguousarray(
+            _general_nanmean_func(a.astype(np.float64), axis), dtype=a.dtype
+        )
     if isinstance(axis, Collection):
         if len(axis) == a.ndim:
             return _nanmean_all(a)
         axis = frozenset(x % a.ndim for x in axis)
     else:
         axis = axis % a.ndim
-    return nanmean_funcs[a.ndim][axis](a).astype(a.dtype)
+    return NANMEAN_FUNCS[a.ndim][axis](a).astype(a.dtype)
 
 
-def _fast_nanmean_skipcheck(
+def fast_nanmean_skipcheck(
     a: npt.NDArray[np.float32 | np.float64], axis: int | Collection[int]
 ) -> npt.NDArray[np.float32 | np.float64] | np.float64:
-    """A version of `fast_nanmean` with near-zero overhead. Meant for internal use.
+    """Compute the mean for specific floating point arrays while ignoring NaNs.
 
-    Strict assumptions on the input parameters allow skipping some checks.
+    This is a version of `fast_nanmean` with near-zero overhead meant for internal use.
+    Strict assumptions on the input parameters allow skipping some checks. Failure to
+    meet these assumptions may lead to undefined behavior.
 
     Parameters
     ----------
     a
-        A numpy array of floats. :code:`a.ndim` must be one of 2, 3, and 4.
+        A numpy array of floats. ``a.ndim`` must be one of 2, 3, and 4.
     axis
         Axis or iterable of axis along which the means are computed. All elements must
-        be nonnegative integers that are less than or equal to :code:`a.ndim`, i.e.,
+        be nonnegative integers that are less than or equal to ``a.ndim``, i.e.,
         negative indexing is not allowed.
 
     Returns
     -------
     numpy.ndarray or float
         The calculated mean. The output array is always C-contiguous.
 
     """
     if isinstance(axis, Collection):
         if len(axis) == a.ndim:
             return _nanmean_all(a)
         axis = frozenset(axis)
-    return nanmean_funcs[a.ndim][axis](a).astype(a.dtype)
+    return NANMEAN_FUNCS[a.ndim][axis](a).astype(a.dtype)
```

### Comparing `erlab-2.3.2/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.4.0/src/erlab/interactive/imagetool/slicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from typing import TYPE_CHECKING
 
 import numba
 import numpy as np
 import numpy.typing as npt
 from qtpy import QtCore
 
-from erlab.interactive.imagetool.fastbinning import _fast_nanmean_skipcheck
+from erlab.interactive.imagetool.fastbinning import fast_nanmean_skipcheck
 
 if TYPE_CHECKING:
-    from collections.abc import Sequence, Hashable
+    from collections.abc import Hashable, Sequence
 
     import xarray as xr
 
 VALID_NDIM = (2, 3, 4)
 
 _signature_array_rect = [
     numba.types.UniTuple(numba.float32, 4)(
@@ -225,20 +225,20 @@
         elif mn < np.float32(0.0):
             return -mx
         else:
             return mn
 
     @property
     def limits(self) -> tuple[float, float]:
-        """Returns the global minima and maxima of the data."""
+        """Return the global minima and maxima of the data."""
         return self.nanmin, self.nanmax
 
     @staticmethod
     def validate_array(data: xr.DataArray) -> xr.DataArray:
-        """Validates a given :class:`xarray.DataArray`.
+        """Validate a given :class:`xarray.DataArray`.
 
         If data has two momentum axes (``kx`` and ``ky``), set them (and ``eV`` if
         exists) as the first two (or three) dimensions. Then, checks the data for
         non-uniform coordinates, which are converted to indices. Finally, converts the
         coordinates to C-contiguous float32. If input data values neither float32 nor
         float64, a conversion to float64 is attempted.
 
@@ -278,33 +278,38 @@
             ).swap_dims({d: d + "_idx"})
 
         return data
 
     def reset_property_cache(self, propname: str) -> None:
         self.__dict__.pop(propname, None)
 
-    def clear_dim_cache(self):
+    def clear_dim_cache(self, include_vals: bool = False):
         for prop in (
             "coords",
             "coords_uniform",
             "incs",
             "incs_uniform",
             "lims",
             "lims_uniform",
-            "data_vals_T",
         ):
             self.reset_property_cache(prop)
 
-    def clear_val_cache(self):
+        if include_vals:
+            self.reset_property_cache("data_vals_T")
+
+    def clear_val_cache(self, include_vals: bool = False):
         for prop in ("nanmax", "nanmin", "absnanmax", "absnanmin"):
             self.reset_property_cache(prop)
 
+        if include_vals:
+            self.reset_property_cache("data_vals_T")
+
     def clear_cache(self):
         self.clear_dim_cache()
-        self.clear_val_cache()
+        self.clear_val_cache(include_vals=True)
 
     def set_array(
         self, xarray_obj: xr.DataArray, validate: bool = True, reset: bool = False
     ) -> None:
         if hasattr(self, "_obj"):
             del self._obj
 
@@ -312,17 +317,17 @@
             self._obj: xr.DataArray = self.validate_array(xarray_obj)
         else:
             self._obj = xarray_obj
         self._nonuniform_axes: list[int] = [
             i for i, d in enumerate(self._obj.dims) if str(d).endswith("_idx")
         ]
 
-        self.clear_dim_cache()
+        self.clear_dim_cache(include_vals=True)
         if validate:
-            self.clear_val_cache()
+            self.clear_val_cache(include_vals=False)
 
         if reset:
             self._bins: list[list[int]] = [[1] * self._obj.ndim]
             self._indices: list[list[int]] = [
                 [s // 2 - (1 if s % 2 == 0 else 0) for s in self._obj.shape]
             ]
             self._values: list[list[np.float32]] = [
@@ -395,15 +400,15 @@
             axes += self.set_bin(cursor, i, x, update=False)
         if update:
             self.sigBinChanged.emit(cursor, tuple(axes))
 
     @QtCore.Slot(int, int, int, bool, result=list)
     def set_bin(
         self, cursor: int, axis: int, value: int, update: bool = True
-    ) -> list[int | None]:
+    ) -> list[int]:
         if value is None:
             return []
         if int(value) != value:
             raise TypeError("bins must have integer type")
         self._bins[cursor][axis] = int(value)
         if update:
             self.sigBinChanged.emit(cursor, (axis,))
@@ -699,15 +704,15 @@
     ) -> npt.NDArray[np.floating] | np.floating:
         axis_val = (axis - 1) % self._obj.ndim
         if not self.get_binned(cursor)[axis]:
             return self.data_vals_T[
                 (slice(None),) * axis_val + (self._bin_slice(cursor, axis),)
             ].squeeze(axis=axis_val)
         else:
-            return _fast_nanmean_skipcheck(
+            return fast_nanmean_skipcheck(
                 self.data_vals_T[
                     (slice(None),) * axis_val + (self._bin_slice(cursor, axis),)
                 ],
                 axis=axis_val,
             )
 
     def _bin_along_multiaxis(
@@ -721,10 +726,10 @@
         selected = self.data_vals_T[
             tuple(
                 slices[axis.index(d)] if d in axis else slice(None)
                 for d in range(self._obj.ndim)
             )
         ]
         if any(self.get_binned(cursor)):
-            return _fast_nanmean_skipcheck(selected, axis=axis)
+            return fast_nanmean_skipcheck(selected, axis=axis)
         else:
             return selected
```

### Comparing `erlab-2.3.2/src/erlab/interactive/kspace.py` & `erlab-2.4.0/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/ktool.ui` & `erlab-2.4.0/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/masktool.py` & `erlab-2.4.0/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/interactive/utilities.py` & `erlab-2.4.0/src/erlab/interactive/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 from __future__ import annotations
 
 import re
 import sys
 import types
 import warnings
-from typing import TYPE_CHECKING, Any, Literal, cast
+from typing import TYPE_CHECKING, Any, Literal, cast, no_type_check
 
 import numpy as np
 import numpy.typing as npt
 import pyperclip
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtGui, QtWidgets
 
 from erlab.interactive.colors import BetterImageItem, pg_colormap_powernorm
 
 if TYPE_CHECKING:
     from collections.abc import Mapping
 
+    from pyqtgraph.GraphicsScene.mouseEvents import MouseDragEvent
+
 __all__ = [
     "AnalysisWidgetBase",
     "AnalysisWindow",
     "BetterAxisItem",
     "BetterSpinBox",
     "DictMenuBar",
     "ParameterGroup",
@@ -31,15 +33,15 @@
     "gen_function_code",
     "gen_single_function_code",
     "parse_data",
     "xImageItem",
 ]
 
 
-def parse_data(data):
+def parse_data(data) -> xr.DataArray:
     if isinstance(data, xr.Dataset):
         raise TypeError(
             "input argument data must be a xarray.DataArray or a "
             "numpy.ndarray. Create an xarray.DataArray "
             "first, either with indexing on the Dataset or by "
             "invoking the `to_array()` method."
         ) from None
@@ -56,26 +58,25 @@
     h, w = data_lims[0][-1] - y, data_lims[1][-1] - x
     y += 0.5 * data_incs[0]
     x += 0.5 * data_incs[1]
     return QtCore.QRectF(x, y, w, h)
 
 
 def copy_to_clipboard(content: str | list[str]) -> str:
-    """Convenience function for clipboard handling.
+    """Copy content to the clipboard.
 
     Parameters
     ----------
     content
         The content to be copied.
 
     Returns
     -------
     str
         The copied content.
-
     """
     if isinstance(content, list):
         content = "\n".join(content)
     pyperclip.copy(content)
     return content
 
 
@@ -85,15 +86,15 @@
             arg = arg[1:-1]
         else:
             arg = f'"{arg}"'
     return arg
 
 
 def gen_single_function_code(funcname: str, *args: tuple, **kwargs):
-    """Generates the string for a Python function call.
+    """Generate the string for a Python function call.
 
     The first argument is the name of the function, and subsequent arguments are
     passed as positional arguments. Keyword arguments are also supported.
 
     Parameters
     ----------
     funcname
@@ -133,15 +134,15 @@
         # If code fits in one line, remove newlines
         code = " ".join([s.strip() for s in code.split("\n")])
         code = code.replace(", )", ")").replace("( ", "(")
     return code
 
 
 def gen_function_code(copy: bool = True, **kwargs):
-    r"""Copies the Python code for function calls to the clipboard.
+    r"""Copy the Python code for function calls to the clipboard.
 
     The result can be copied to your clipboard in a form that can be pasted into an
     interactive Python session or Jupyter notebook cell.
 
     Parameters
     ----------
     copy
@@ -224,15 +225,15 @@
         self._is_compact = compact
         self._is_discrete = discrete
         self._is_scientific = scientific
         self._decimal_significant = significant
         self.setDecimals(decimals)
 
         self._value = value
-        self._lastvalue = None
+        self._lastvalue: float | None = None
         self._min = -np.inf
         self._max = np.inf
         self._step = 1 if self._only_int else 0.01
 
         kwargs.setdefault("correctionMode", self.CorrectionMode.CorrectToPreviousValue)
         kwargs.setdefault("keyboardTracking", False)
 
@@ -395,15 +396,17 @@
 
         if self._only_int and np.isfinite(val):
             val = round(val)
 
         self._lastvalue, self._value = self._value, val
 
         self.valueChanged.emit(self.value())
-        self.lineEdit().setText(self.text())
+        line = self.lineEdit()
+        if line is not None:
+            line.setText(self.text())
         self.textChanged.emit(self.text())
 
     def fixup(self, input):
         # Called when the spinbox loses focus with an invalid or intermediate string
         return self.textFromValue(self._lastvalue)
 
     def validate(self, strn, pos):
@@ -420,29 +423,36 @@
                 ret = QtGui.QValidator.State.Invalid
 
         # note: if text is invalid, we don't change the textValid flag since the text
         # will be forced to its previous state anyway
         return (ret, strn, pos)
 
     def editingFinishedEvent(self):
-        self.setValue(self.valueFromText(self.lineEdit().text()))
+        line = self.lineEdit()
+        if line is not None:
+            self.setValue(self.valueFromText(line.text()))
 
     def keyPressEvent(self, evt):
-        if evt == QtGui.QKeySequence.StandardKey.Copy:
-            if (not evt.isAutoRepeat()) and self.lineEdit().hasSelectedText():
-                copy_to_clipboard(self.lineEdit().selectedText())
+        line = self.lineEdit()
+        if line is not None:
+            if evt == QtGui.QKeySequence.StandardKey.Copy:
+                if (not evt.isAutoRepeat()) and line.hasSelectedText():
+                    copy_to_clipboard(line.selectedText())
+            else:
+                super().keyPressEvent(evt)
         else:
             super().keyPressEvent(evt)
 
     def _updateHeight(self):
         if self._is_compact:
             self.setFixedHeight(QtGui.QFontMetrics(self.font()).height() + 3)
 
     def _get_offset(self):
-        spin = QtWidgets.QDoubleSpinBox(self, minimum=0, maximum=0)
+        spin = QtWidgets.QDoubleSpinBox(self)
+        spin.setRange(0, 0)
         w = (
             spin.minimumSizeHint().width()
             - QtGui.QFontMetrics(spin.font())
             .boundingRect(spin.textFromValue(0.0))
             .width()
         )
         spin.setDisabled(True)
@@ -490,15 +500,15 @@
             return self.logTickStrings(values, scale, spacing)
 
         places = max(0, np.ceil(-np.log10(spacing * scale)))
         strings = []
         for v in values:
             vs = v * scale
             if abs(vs) < 0.001 or abs(vs) >= 10000:
-                vstr = "%g" % vs
+                vstr = f"{vs:g}"
             else:
                 vstr = ("%%0.%df" % places) % vs
             strings.append(vstr.replace("-", "−"))
         return strings
 
     def labelString(self):
         if self.labelUnits == "":
@@ -506,30 +516,29 @@
                 units = ""
             else:
                 # units = re.sub(
                 #     r"1E\+?(\-?)0?(\d?\d)",
                 #     r"10<sup>\1\2</sup>",
                 #     f"(×{1.0 / self.autoSIPrefixScale:.3G})",
                 # )#.replace("-", "−")
+                search = re.search(
+                    r"1E\+?(\-?)0?(\d?\d)",
+                    f"{1.0 / self.autoSIPrefixScale:.3G}",
+                )
+                if search is not None:
+                    units = "".join(search.groups())
 
-                try:
-                    units = "".join(
-                        re.search(
-                            r"1E\+?(\-?)0?(\d?\d)",
-                            f"{1.0 / self.autoSIPrefixScale:.3G}",
-                        ).groups()
-                    )
                     for k, v in zip(
                         ("0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "-"),
                         ("⁰", "¹", "²", "³", "⁴", "⁵", "⁶", "⁷", "⁸", "⁹", "⁻"),
                         strict=True,
                     ):
                         units = units.replace(k, v)
                     units = f"10{units}"
-                except AttributeError:
+                else:
                     units = f"{1.0 / self.autoSIPrefixScale:.3G}"
                 units = f"(×{units})"
 
         else:
             units = f"({self.labelUnitPrefix}{self.labelUnits})"
 
         if self.labelText == "":
@@ -543,15 +552,15 @@
 
     def setLabel(self, text=None, units=None, unitPrefix=None, **args):
         # `None` input is kept for backward compatibility!
         self.labelText = text or ""
         self.labelUnits = units or ""
         self.labelUnitPrefix = unitPrefix or ""
         if len(args) > 0:
-            self.labelStyle = args
+            self.labelStyle: dict = args
         # Account empty string and `None` for units and text
         visible = bool(text or units)
         if text == units == "":
             visible = True
         self.showLabel(visible)
         self._updateLabel()
 
@@ -675,17 +684,18 @@
             param_info["min"] = float(self.minimum())
         if np.isfinite(self.maximum()):
             param_info["max"] = float(self.maximum())
         return {self.prefix() + self.param_name: param_info}
 
 
 class xImageItem(BetterImageItem):
-    """
-    :class:`pyqtgraph.ImageItem` with additional functionality, including
-    :class:`xarray.DataArray` support and auto limits based on histogram analysis.
+    """:class:`pyqtgraph.ImageItem` with additional functionality.
+
+    This class provides :class:`xarray.DataArray` support and auto limits based on
+    histogram analysis.
 
     Parameters
     ----------
     image
         Image data.
     **kwargs
         Additional arguments to :class:`pyqtgraph.ImageItem`.
@@ -696,15 +706,15 @@
 
     """
 
     sigToleranceChanged = QtCore.Signal(float, float)  #: :meta private:
 
     def __init__(self, image: npt.NDArray | None = None, **kwargs):
         super().__init__(image, **kwargs)
-        self.cut_tolerance = (30, 30)
+        self.cut_tolerance = [30, 30]
         self.data_array: None | xr.DataArray = None
 
     def set_cut_tolerance(self, cut_tolerance):
         try:
             self.cut_tolerance = list(cut_tolerance.__iter__)
         except AttributeError:
             self.cut_tolerance = [cut_tolerance] * 2
@@ -745,14 +755,15 @@
             if pi is not None:
                 pi.setLabel("left", data.dims[0])
                 pi.setLabel("bottom", data.dims[1])
 
         self.setImage(img, rect=rect, **kargs)
         self.data_array = data
 
+    @no_type_check
     def getMenu(self):
         if self.menu is None:
             if not self.removable:
                 self.menu = QtWidgets.QMenu()
             else:
                 super().getMenu()
             if self.menu is not None:
@@ -804,15 +815,14 @@
 
     Signals
     -------
     sigParameterChanged(dict)
 
     Examples
     --------
-
     >>> ParameterGroup(
         **{
             "a": QtWidgets.QDoubleSpinBox(range=(0, 1), singleStep=0.01, value=0.2),
             "b": dict(qwtype="dblspin", range=(0, 2), singleStep=0.04),
             "c": QtWidgets.QSlider(range=(0, 10000))
         }
     )
@@ -907,15 +917,15 @@
                 "fitparam",
             ]
             | None
         ) = None,
         **kwargs,
     ):
         """
-        Initializes the :class:`PySide6.QtWidgets.QWidget` corresponding to ``qwtype``.
+        Initialize the :class:`PySide6.QtWidgets.QWidget` corresponding to ``qwtype``.
 
         Parameters
         ----------
         qwtype
             Type of the widget, must a key of :obj:`ParameterGroup.VALID_QWTYPE`.
 
         """
@@ -997,17 +1007,20 @@
         if value is not None:
             widget.setValue(value)
 
         return widget
 
     def set_values(self, **kwargs):
         for k, v in kwargs.items():
-            self.widgets[k].blockSignals(True)
-            self.widgets[k].setValue(v)
-            self.widgets[k].blockSignals(False)
+            widget = self.widgets[k]
+            widget.blockSignals(True)
+            if hasattr(widget, "setValue"):
+                widget.setValue(v)
+            widget.blockSignals(False)
+
         self.sigParameterChanged.emit(kwargs)
 
     def widget_value(self, widget: str | QtWidgets.QWidget):
         if isinstance(widget, str):
             widget = self.widgets[widget]
         if isinstance(
             widget,
@@ -1144,14 +1157,15 @@
     @property
     def roi_limits(self):
         x0, y0 = self.roi.state["pos"]
         w, h = self.roi.state["size"]
         x1, y1 = x0 + w, y0 + h
         return x0, y0, x1, y1
 
+    @no_type_check
     def update_pos(self):
         self.widgets["x0"].setMaximum(self.widgets["x1"].value())
         self.widgets["y0"].setMaximum(self.widgets["y1"].value())
         self.widgets["x1"].setMinimum(self.widgets["x0"].value())
         self.widgets["y1"].setMinimum(self.widgets["y0"].value())
         for pos, spin in zip(self.roi_limits, self.roi_spin, strict=True):
             spin.blockSignals(True)
@@ -1173,20 +1187,21 @@
         vb = self.roi.parentItem().getViewBox()
 
         if not toggle:
             vb.mouseDragEvent = self._drag_evt_old
             vb.setMouseMode(self._state_old)
             vb.rbScaleBox.setPen(pg.mkPen((255, 255, 100), width=1))
             vb.rbScaleBox.setBrush(pg.mkBrush(255, 255, 0, 100))
-            vb.setCursor(QtGui.QCursor(QtCore.Qt.ArrowCursor))
+
+            vb.setCursor(QtGui.QCursor(QtCore.Qt.CursorShape.ArrowCursor))
             return
 
-        vb.setCursor(QtGui.QCursor(QtCore.Qt.CrossCursor))
-        self._state_old = vb.state["mouseMode"]
-        self._drag_evt_old = vb.mouseDragEvent
+        vb.setCursor(QtGui.QCursor(QtCore.Qt.CursorShape.CrossCursor))
+        self._state_old: int = vb.state["mouseMode"]
+        self._drag_evt_old: MouseDragEvent = vb.mouseDragEvent
 
         vb.setMouseMode(pg.ViewBox.RectMode)
         vb.rbScaleBox.setPen(pg.mkPen((255, 255, 255), width=1))
         vb.rbScaleBox.setBrush(pg.mkBrush(255, 255, 255, 100))
 
         def mouseDragEventCustom(ev, axis=None):
             ev.accept()
@@ -1252,15 +1267,15 @@
         title=None,
         layout="horizontal",
         data_is_input=True,
         analysisWidget=None,
         *args,
         **kwargs,
     ):
-        self.qapp = QtCore.QCoreApplication.instance()
+        self.qapp = cast(QtWidgets.QApplication, QtWidgets.QApplication.instance())
         if not self.qapp:
             self.qapp = QtWidgets.QApplication(sys.argv)
         self.qapp.setStyle("Fusion")
 
         super().__init__()
 
         self.data = parse_data(data)
@@ -1269,18 +1284,20 @@
         self.setWindowTitle(title)
 
         self._main = QtWidgets.QWidget(self)
         self.setCentralWidget(self._main)
 
         self.controlgroup = QtWidgets.QWidget()
         if layout == "vertical":
-            self.layout = QtWidgets.QVBoxLayout(self._main)
-            self.controls = QtWidgets.QHBoxLayout(self.controlgroup)
+            layout = QtWidgets.QVBoxLayout(self._main)
+            self.controls: QtWidgets.QBoxLayout = QtWidgets.QHBoxLayout(
+                self.controlgroup
+            )
         elif layout == "horizontal":
-            self.layout = QtWidgets.QHBoxLayout(self._main)
+            layout = QtWidgets.QHBoxLayout(self._main)
             self.controls = QtWidgets.QVBoxLayout(self.controlgroup)
         else:
             raise ValueError("Layout must be 'vertical' or 'horizontal'.")
 
         if analysisWidget is None:
             self.aw = AnalysisWidgetBase(*args, **kwargs)
         elif isinstance(analysisWidget, type):
@@ -1298,22 +1315,22 @@
             # "set_pre_function_args",
             # "set_main_function",
             # "set_main_function_args",
             # "refresh_output",
             # "refresh_all",
         ]:
             setattr(self, n, getattr(self.aw, n))
-        self.layout.addWidget(self.aw)
-        self.layout.addWidget(self.controlgroup)
+        layout.addWidget(self.aw)
+        layout.addWidget(self.controlgroup)
 
-        self.layout.setContentsMargins(QtCore.QMargins(0, 0, 0, 0))
-        self.layout.setSpacing(0)
+        layout.setContentsMargins(QtCore.QMargins(0, 0, 0, 0))
+        layout.setSpacing(0)
         self.controlgroup.setContentsMargins(QtCore.QMargins(0, 0, 0, 0))
         if data_is_input:
-            self.set_input(data)
+            self.aw.set_input(data)
 
     def __post_init__(self, execute=None):
         self.show()
         self.activateWindow()
         self.raise_()
 
         if execute is None:
@@ -1336,15 +1353,15 @@
         cb = cast(QtWidgets.QApplication, QtWidgets.QApplication.instance()).clipboard()
         if event is not None and cb is not None and cb.text(cb.Mode.Clipboard) != "":
             pyperclip.copy(cb.text(cb.Mode.Clipboard))
         return super().closeEvent(event)
 
 
 class AnalysisWidgetBase(pg.GraphicsLayoutWidget):
-    """AnalysisWidgetBase
+    """AnalysisWidgetBase.
 
     Parameters
     ----------
     orientation
         Sets the orientation of the plots, by default "vertical"
     num_ax
         Sets the number of axes.
@@ -1368,15 +1385,15 @@
             self.is_vertical = False
         elif orientation == "vertical":
             self.is_vertical = True
         else:
             raise ValueError("Orientation must be 'vertical' or 'horizontal'.")
         self.cut_to_data = cut_to_data
 
-        self.input = None
+        self.input: None | xr.DataArray = None
 
         self.initialize_layout(num_ax)
 
         for i in range(1, num_ax):
             if link in ("x", "both"):
                 self.axes[i].setXLink(self.axes[0])
             if link in ("y", "both"):
@@ -1418,18 +1435,18 @@
             self.ci.layout.setRowStretchFactor(i, factor)
         else:
             self.ci.layout.setColumnStretchFactor(i, factor)
 
     def set_input(self, data=None):
         if data is not None:
             self.input = parse_data(data)
-        self.images[0].setDataArray(
-            self.input,
-            cut_to_data=self.cut_to_data in ("in", "both"),
-        )
+            self.images[0].setDataArray(
+                self.input,
+                cut_to_data=self.cut_to_data in ("in", "both"),
+            )
 
     def add_roi(self, i):
         self.roi[i] = pg.ROI(
             [-0.1, -0.5],
             [0.3, 0.5],
             parent=self.images[i],
             rotatable=False,
@@ -1443,39 +1460,50 @@
         self.axes[i].addItem(self.roi[i])
         self.roi[i].setZValue(10)
         return self.roi[i]
 
 
 class ComparisonWidget(AnalysisWidgetBase):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, num_ax=2, **kwargs)
+        kwargs["num_ax"] = 2
+        super().__init__(*args, **kwargs)
         self.prefunc = lambda x: x
         self.mainfunc = lambda x: x
         self.prefunc_only_values = False
         self.mainfunc_only_values = False
         self.prefunc_kwargs = {}
         self.mainfunc_kwargs = {}
 
     def call_prefunc(self, x):
         if self.prefunc_only_values:
-            x = np.asarray(x)
-        return self.prefunc(x, **self.prefunc_kwargs)
+            xval = np.asarray(x)
+        else:
+            xval = x
+        return self.prefunc(xval, **self.prefunc_kwargs)
 
     def set_input(self, data=None):
         if data is not None:
             self.input_ = parse_data(data)
 
         self.input = self.call_prefunc(self.input_)
         if self.prefunc_only_values:
+            if not isinstance(self.input, np.ndarray):
+                raise TypeError(
+                    "Pre-function must return a numpy array when `only_values` is True."
+                )
             self.images[0].setImage(
                 np.ascontiguousarray(self.input),
                 rect=array_rect(self.input_),
                 cut_to_data=self.cut_to_data in ("in", "both"),
             )
         else:
+            if not isinstance(self.input, xr.DataArray):
+                raise TypeError(
+                    "Pre-function must return a DataArray when `only_values` is False."
+                )
             self.images[0].setDataArray(
                 self.input,
                 cut_to_data=self.cut_to_data in ("in", "both"),
             )
 
     def set_pre_function(self, func, only_values=False, **kwargs):
         self.prefunc_only_values = only_values
```

### Comparing `erlab-2.3.2/src/erlab/io/__init__.py` & `erlab-2.4.0/src/erlab/io/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 For instructions on how to write a custom loader, see
 :doc:`/generated/erlab.io.dataloader`.
 
 
 Examples
 --------
-
 - View all registered loaders:
 
   >>> erlab.io.loaders
 
 - Load data by explicitly specifying the loader:
 
   >>> dat = erlab.io.loaders["merlin"].load(...)
```

### Comparing `erlab-2.3.2/src/erlab/io/characterization/resistance.py` & `erlab-2.4.0/src/erlab/io/characterization/resistance.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 physics lab III equipment.
 
 """
 
 import os
 import re
 from io import StringIO
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 __all__ = ["load_resistance_physlab"]
 
 
 def load_resistance_physlab(path: str, **kwargs) -> xr.Dataset:
-    """Loads resistance measurement acquired with physics lab III equipment.
+    """Load resistance measurement acquired with physics lab III equipment.
 
     Parameters
     ----------
     path
         Local path to ``.dat`` file.
 
     Returns
@@ -46,15 +47,15 @@
             )
         )
 
 
 def _load_resistance_physlab_old(
     path: str, encoding: str = "windows-1252", **kwargs
 ) -> xr.Dataset:
-    """Loads resistance measurement acquired with physics lab III equipment.
+    """Load resistance measurement acquired with physics lab III equipment.
 
     Parameters
     ----------
     path
         Local path to ``.dat`` file.
     encoding
         Encoding passed onto `open`, defaults to ``'windows-1252'``.
@@ -82,22 +83,22 @@
         reserr   (temp) float64 0.001551 0.001202 ... 0.001027 0.001125
 
     Plot resistance versus temperature:
 
     >>> data.res.plot()
 
     """
-    with open(path, encoding=encoding) as file:
-        content = re.sub(
-            r"(e[-+]\d{3}) {2,3}(-?)",
-            "\\g<1>\\t \\g<2>",
-            file.read(),
-            count=0,
-            flags=re.MULTILINE,
-        )
+    content = re.sub(
+        r"(e[-+]\d{3}) {2,3}(-?)",
+        "\\g<1>\\t \\g<2>",
+        Path(path).read_text(encoding),
+        count=0,
+        flags=re.MULTILINE,
+    )
+
     content = content.replace("-1.#IO", "   nan")
     data = np.genfromtxt(
         StringIO(content),
         delimiter="\t",
         skip_header=3,
         usecols=[2, 3, 4, 5, 6, 7],
         **kwargs,
```

### Comparing `erlab-2.3.2/src/erlab/io/characterization/xrd.py` & `erlab-2.4.0/src/erlab/io/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/io/dataloader.py` & `erlab-2.4.0/src/erlab/io/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-r"""Base functionality for implementing data loaders
+r"""Base functionality for implementing data loaders.
 
 This module provides a base class `LoaderBase` for implementing data loaders. Data
 loaders are plugins used to load data from various file formats. Each data loader that
 subclasses `LoaderBase` is registered on import in `loaders`.
 
 Loaded ARPES data must contain several attributes and coordinates. See the
 implementation of `LoaderBase.validate` for details.
@@ -44,23 +44,23 @@
 
 def _is_monotonic(arr: npt.NDArray) -> np.bool_:
     dif = np.diff(arr)
     return np.all(dif >= 0) or np.all(dif <= 0)
 
 
 class ValidationError(Exception):
-    """This exception is raised when the loaded data fails validation checks."""
+    """Raised when the loaded data fails validation checks."""
 
 
 class ValidationWarning(UserWarning):
-    """This warning is issued when the loaded data fails validation checks."""
+    """Issued when the loaded data fails validation checks."""
 
 
 class LoaderNotFoundError(Exception):
-    """This exception is raised when a loader is not found in the registry."""
+    """Raised when a loader is not found in the registry."""
 
     def __init__(self, key: str):
         super().__init__(f"Loader for name or alias {key} not found in the registry")
 
 
 class LoaderBase:
     """Base class for all data loaders."""
@@ -111,15 +111,19 @@
     """
     If `True`, validation check will raise a `ValidationError` on the first failure
     instead of warning. Useful for debugging data loaders.
     """
 
     @property
     def name_map_reversed(self) -> dict[str, str]:
-        """A reversed version of the name_map dictionary."""
+        """A reversed version of the name_map dictionary.
+
+        This property is useful for mapping original names to new names.
+
+        """
         return self.reverse_mapping(self.name_map)
 
     @staticmethod
     def reverse_mapping(mapping: Mapping[str, str | Iterable[str]]) -> dict[str, str]:
         """Reverse the given mapping dictionary to form a one-to-one mapping.
 
         Parameters
@@ -217,15 +221,14 @@
             %H:%M:%S".
 
         - For other types:
             The value is returned as is.
 
         Examples
         --------
-
         >>> formatter(np.array([0.1, 0.15, 0.2]))
         '0.1→0.2 (0.05, 3)'
 
         >>> formatter(np.array([1.0, 2.0, 2.1]))
         '1→2.1 (3)'
 
         >>> formatter(np.array([1.0, 2.1, 2.0]))
@@ -420,18 +423,19 @@
         data_dir: str | os.PathLike,
         usecache: bool = True,
         *,
         cache: bool = True,
         display: bool = True,
         **kwargs,
     ) -> pandas.DataFrame | pandas.io.formats.style.Styler | None:
-        """
-        Takes a path to a directory and summarizes the data in the directory to a table
-        `pandas.DataFrame`, much like a log file. This is useful for quickly inspecting
-        the contents of a directory.
+        """Summarize the data in the given directory.
+
+        Takes a path to a directory and summarizes the data in the directory to a table,
+        much like a log file. This is useful for quickly inspecting the contents of a
+        directory.
 
         The dataframe is formatted using the style from :meth:`get_styler
         <erlab.io.dataloader.LoaderBase.get_styler>` and displayed in the IPython shell.
         Results are cached in a pickle file in the directory.
 
         Parameters
         ----------
@@ -450,22 +454,28 @@
             the IPython shell is not detected, the dataframe styler will be returned.
         **kwargs
             Additional keyword arguments to be passed to `generate_summary`.
 
         Returns
         -------
         df : pandas.DataFrame or pandas.io.formats.style.Styler or None
-            Summary of the data in the directory. If `display` is `False`, the DataFrame
-            is returned. If `display` is `True` and the IPython shell is detected, the
-            summary will be displayed, and `None` will be returned. If `display` is
-            `True` but the IPython shell is not detected, the styler for the summary
-            DataFrame will be returned.
+            Summary of the data in the directory.
 
-        """
+            - If `display` is `False`, the summary DataFrame is returned.
+
+            - If `display` is `True` and the IPython shell is detected, the summary will
+              be displayed, and `None` will be returned.
+
+              * If `ipywidgets` is installed, an interactive widget will be returned
+                instead of `None`.
 
+            - If `display` is `True` but the IPython shell is not detected, the styler
+              for the summary DataFrame will be returned.
+
+        """
         if not os.path.isdir(data_dir):
             raise FileNotFoundError(f"Directory {data_dir} not found")
 
         pkl_path = os.path.join(data_dir, ".summary.pkl")
         df = None
         if usecache:
             try:
@@ -498,15 +508,15 @@
 
                 with pandas.option_context(
                     "display.max_rows", len(df), "display.max_columns", len(df.columns)
                 ):
                     display(styled)  # type: ignore[misc]
 
                 if importlib.util.find_spec("ipywidgets"):
-                    display(self.isummarize(df=df))  # type: ignore[misc]
+                    return self._isummarize(df)
 
                 return None
 
         except NameError:
             pass
 
         return styled
@@ -535,14 +545,17 @@
             raise ImportError(
                 "ipywidgets and IPython is required for interactive summaries"
             )
         if df is None:
             kwargs["display"] = False
             df = cast(pandas.DataFrame, self.summarize(**kwargs))
 
+        self._isummarize(df)
+
+    def _isummarize(self, df: pandas.DataFrame):
         import matplotlib.pyplot as plt
         from ipywidgets import (
             HTML,
             Button,
             Dropdown,
             FloatSlider,
             HBox,
@@ -592,21 +605,26 @@
                         os.path.splitext(os.path.basename(path))[0]
                     )
                     if idx is not None:
                         n_scans = len(self.identify(idx, os.path.dirname(path))[0])
                         if n_scans > 1 and not full:
                             full_button.disabled = False
 
-                self._temp_data = self.load(path, single=not full)
+                out = self.load(path, single=not full)
+                if isinstance(out, xr.DataArray):
+                    self._temp_data = out
+                del out
 
                 data_info.value = _format_data_info(series)
+            if self._temp_data is None:
+                return
 
             if self._temp_data.ndim == 4:
                 # If the data is 4D, average over the last dimension, making it 3D
-                self._temp_data = self._temp_data.mean(self._temp_data.dims[-1])
+                self._temp_data = self._temp_data.mean(str(self._temp_data.dims[-1]))
 
             if self._temp_data.ndim == 3:
                 dim_sel.unobserve(_update_sliders, "value")
                 coord_sel.unobserve(_update_plot, "value")
 
                 dim_sel.options = self._temp_data.dims
                 # Set the default dimension to the one with the smallest size
@@ -639,15 +657,15 @@
 
             scan_coords = self._temp_data[dim_sel.value].values
 
             dim_sel.unobserve(_update_sliders, "value")
             coord_sel.unobserve(_update_plot, "value")
 
             coord_sel.step = abs(scan_coords[1] - scan_coords[0])
-            coord_sel.max = 1e100  # To ensure max > min always
+            coord_sel.max = 1e100  # To ensure max > min before setting bounds
             coord_sel.min = scan_coords.min()
             coord_sel.max = scan_coords.max()
 
             coord_sel.observe(_update_plot, "value")
             dim_sel.observe(_update_sliders, "value")
 
         def _update_plot(_):
@@ -657,32 +675,33 @@
                 plot_data = self._temp_data.qsel({dim_sel.value: coord_sel.value})
             else:
                 plot_data = self._temp_data
 
             out.clear_output(wait=True)
             with out:
                 plot_data.qplot(ax=plt.gca())
-                # Remove automatic title from xarray
-                plt.title("")
+                plt.title("")  # Remove automatically generated title
 
                 # Add line at Fermi level if the data is 2D and has an energy dimension
                 if plot_data.ndim == 2 and "eV" in plot_data.dims:
+                    # Check if binding
                     if plot_data["eV"].values[0] * plot_data["eV"].values[-1] < 0:
                         eplt.fermiline(
                             orientation="h" if plot_data.dims[0] == "eV" else "v"
                         )
-
                 show_inline_matplotlib_plots()
 
         def _next(_):
+            # Select next row
             idx = list(df.index).index(data_select.value)
             if idx + 1 < len(df.index):
                 data_select.value = list(df.index)[idx + 1]
 
         def _prev(_):
+            # Select previous row
             idx = list(df.index).index(data_select.value)
             if idx - 1 >= 0:
                 data_select.value = list(df.index)[idx - 1]
 
         prev_button = Button(description="Prev", layout=Layout(width="50px"))
         prev_button.on_click(_prev)
 
@@ -692,15 +711,15 @@
         full_button = Button(description="Load full", layout=Layout(width="100px"))
         full_button.on_click(lambda _: _update_data(None, full=True))
 
         buttons = [prev_button, next_button]
         if not self.always_single:
             buttons.append(full_button)
 
-        data_select = Select(options=list(df.index), value=next(iter(df.index)))
+        data_select = Select(options=list(df.index), value=next(iter(df.index)), rows=8)
         data_select.observe(_update_data, "value")
 
         data_info = HTML()
 
         dim_sel = Dropdown()
         dim_sel.observe(_update_sliders, "value")
 
@@ -753,14 +772,17 @@
 
         This method takes a scan index and transforms it into a list of file paths and
         coordinates. For scans spread over multiple files, the coordinates must be a
         dictionary mapping scan axes names to scan coordinates. For single file scans,
         the list should contain only one file path and coordinates must be an empty
         dictionary.
 
+        The keys of the coordinates must be transformed to new names prior to returning
+        by using the mapping returned by the `name_map_reversed` property.
+
         Parameters
         ----------
         num
             The index of the scan to identify.
         data_dir
             The directory containing the data.
 
@@ -776,16 +798,19 @@
 
         """
         raise NotImplementedError("method must be implemented in the subclass")
 
     def infer_index(self, name: str) -> tuple[int | None, dict[str, Any]]:
         """Infer the index for the given file name.
 
-        This method takes a file name and tries to infer the scan index from it. If the
-        index can be inferred, it is returned; otherwise, `None` should be returned.
+        This method takes a file name with the path and extension stripped, and tries to
+        infer the scan index from it. If the index can be inferred, it is returned along
+        with additional keyword arguments that should be passed to `load`. If the index
+        is not found, `None` should be returned for the index, and an empty dictionary
+        for additional keyword arguments.
 
         Parameters
         ----------
         name
             The base name of the file without the path and extension.
 
         Returns
@@ -801,17 +826,19 @@
         This method is used to determine all files for a given scan. Hence, for loaders
         with `always_single` set to `True`, this method does not have to be implemented.
 
         """
         raise NotImplementedError("method must be implemented in the subclass")
 
     def generate_summary(self, data_dir: str | os.PathLike) -> pandas.DataFrame:
-        """Takes a path to a directory and summarizes the data in the directory to a
-        pandas DataFrame, much like a log file. This is useful for quickly inspecting
-        the contents of a directory.
+        """Generate a dataframe summarizing the data in the given directory.
+
+        Takes a path to a directory and summarizes the data in the directory to a pandas
+        DataFrame, much like a log file. This is useful for quickly inspecting the
+        contents of a directory.
 
         Parameters
         ----------
         data_dir
             Path to a directory.
 
         Returns
@@ -1002,15 +1029,15 @@
     def __new__(cls):
         if not isinstance(cls.__instance, cls):
             cls.__instance = super().__new__(cls)
         return cls.__instance
 
     @classmethod
     def instance(cls) -> Self:
-        """Returns the registry instance."""
+        """Return the registry instance."""
         return cls()
 
 
 class LoaderRegistry(RegistryBase):
     loaders: ClassVar[dict[str, LoaderBase | type[LoaderBase]]] = {}
     """Registered loaders \n\n:meta hide-value:"""
 
@@ -1109,15 +1136,14 @@
           >>> erlab.io.set_loader("ssrl52", data_dir="/path/to/dir1")
           >>> dat_ssrl_1 = erlab.io.load(...)
           >>> with erlab.io.loader_context("merlin", data_dir="/path/to/dir2"):
           ...     dat_merlin = erlab.io.load(...)
           >>> dat_ssrl_2 = erlab.io.load(...)
 
         """
-
         if loader is None and data_dir is None:
             raise ValueError(
                 "At least one of loader or data_dir must be specified in the context"
             )
 
         if loader is not None:
             old_loader: LoaderBase | None = self.current_loader
```

### Comparing `erlab-2.3.2/src/erlab/io/exampledata.py` & `erlab-2.4.0/src/erlab/io/exampledata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Generates simple simulated ARPES data for testing purposes."""
 
 __all__ = ["generate_data", "generate_data_angles"]
 
-from collections.abc import Sequence
+from collections.abc import Hashable, Sequence
+from typing import cast
 
 import numpy as np
 import scipy.ndimage
 import xarray as xr
 
 import erlab.analysis.image
 import erlab.analysis.kspace
@@ -220,15 +221,14 @@
 
     Returns
     -------
     xarray.DataArray
         The generated data with coordinates for alpha, beta, and eV.
 
     """
-
     if isinstance(angrange, dict):
         alpha = np.linspace(*angrange["alpha"], shape[0])
         beta = np.linspace(*angrange["beta"], shape[1])
     elif isinstance(angrange, tuple):
         alpha = np.linspace(*angrange, shape[0])
         beta = np.linspace(*angrange, shape[1])
     else:
@@ -371,15 +371,15 @@
     data = data * count
 
     if noise:
         rng = np.random.default_rng(seed)
         data[:] = rng.poisson(data).astype(float)
 
     data = erlab.analysis.image.gaussian_filter(
-        data, sigma={"eV": Eres, "alpha": angres}
+        data, sigma=cast(dict[Hashable, float], {"eV": Eres, "alpha": angres})
     )
 
     if noise:
         data[:] = scipy.ndimage.gaussian_filter(
             rng.poisson(data).astype(float), sigma=ccd_sigma
         )
```

### Comparing `erlab-2.3.2/src/erlab/io/igor.py` & `erlab-2.4.0/src/erlab/io/igor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
+from typing import Any
 
 import h5netcdf
 import igor2.binarywave
 import igor2.packed
 import igor2.record
-from typing import Any
 import numpy as np
 import xarray as xr
 
 __all__ = ["load_experiment", "load_igor_hdf5", "load_wave"]
 
 
 def _load_experiment_raw(
@@ -63,15 +63,15 @@
     folder: str | None = None,
     *,
     prefix: str | None = None,
     ignore: list[str] | None = None,
     recursive: bool = False,
     **kwargs,
 ) -> xr.Dataset:
-    """Loads waves from an igor experiment (`.pxp`) file.
+    """Load waves from an igor experiment (`.pxp`) file.
 
     Parameters
     ----------
     filename
         The experiment file.
     folder
         Target folder within the experiment, given as a slash-separated string. If
@@ -141,14 +141,15 @@
     ----------
     wave
         The wave to load. It can be provided as a dictionary, an instance of
         `igor2.record.WaveRecord`, or a string representing the path to the wave file.
     data_dir
         The directory where the wave file is located. This parameter is only used if
         `wave` is a string or `PathLike` object. If `None`, `wave` must be a valid path.
+
     Returns
     -------
     xarray.DataArray
         The loaded wave.
 
     Raises
     ------
```

### Comparing `erlab-2.3.2/src/erlab/io/plugins/__init__.py` & `erlab-2.4.0/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/io/plugins/da30.py` & `erlab-2.4.0/src/erlab/io/plugins/da30.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-"""
-Base class for implementing loaders that can load data acquired with Scienta Omicron's
-DA30L analyzer using ``SES.exe``. Must be subclassed to implement the actual loading.
+"""Loader for Scienta Omicron DA30L analyzer with SES.
+
+Provides a base class for implementing loaders that can load data acquired with Scienta
+Omicron's DA30L analyzer using ``SES.exe``. Must be subclassed to implement the actual
+loading.
 """
 
 import configparser
 import os
 import tempfile
 import zipfile
 from typing import ClassVar
+
 import numpy as np
 import xarray as xr
 
 from erlab.io.dataloader import LoaderBase
 from erlab.io.igor import load_experiment, load_wave
```

### Comparing `erlab-2.3.2/src/erlab/io/plugins/kriss.py` & `erlab-2.4.0/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/io/plugins/merlin.py` & `erlab-2.4.0/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/io/plugins/ssrl52.py` & `erlab-2.4.0/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/io/utilities.py` & `erlab-2.4.0/src/erlab/io/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 
 import os
 import warnings
 from collections.abc import Sequence
 
 import numpy as np
 import numpy.typing as npt
-
 import xarray as xr
 
 
 def showfitsinfo(path: str | os.PathLike):
-    """Prints raw metadata from a ``.fits`` file.
+    """Print raw metadata from a ``.fits`` file.
 
     Parameters
     ----------
     path
         Local path to ``.fits`` file.
 
     """
@@ -38,15 +37,15 @@
 
 def get_files(
     directory,
     extensions: Sequence[str] | None = None,
     contains: str | None = None,
     notcontains: str | None = None,
 ) -> list[str]:
-    """Returns a list of files in a directory with the given extensions.
+    """Return a list of files in a directory with the given extensions.
 
     Parameters
     ----------
     directory
         Target directory.
     extensions
         List of extensions to filter for. If not provided, all files are returned.
@@ -57,15 +56,14 @@
 
     Returns
     -------
     files : list of str
         List of files in the directory.
 
     """
-
     files = []
 
     for f in os.listdir(directory):
         if extensions is not None and os.path.splitext(f)[1] not in extensions:
             continue
         if contains is not None and contains not in f:
             continue
@@ -163,15 +161,15 @@
 
 def save_as_hdf5(
     data: xr.DataArray | xr.Dataset,
     filename: str | os.PathLike,
     igor_compat: bool = True,
     **kwargs,
 ):
-    """Saves data in ``HDF5`` format.
+    """Save data in ``HDF5`` format.
 
     Parameters
     ----------
     data
         `xarray.DataArray` to save.
     filename
         Target file name.
@@ -216,15 +214,15 @@
             var: {"compression": "gzip", "compression_opts": 9} for var in data.coords
         },
         **kwargs,
     )
 
 
 def save_as_netcdf(data: xr.DataArray, filename: str | os.PathLike, **kwargs):
-    """Saves data in ``netCDF4`` format.
+    """Save data in ``netCDF4`` format.
 
     Discards invalid ``netCDF4`` attributes and produces a warning.
 
     Parameters
     ----------
     data
         `xarray.DataArray` to save.
@@ -237,12 +235,7 @@
     """
     kwargs.setdefault("engine", "h5netcdf")
     fix_attr_format(data).to_netcdf(
         filename,
         encoding={var: {"zlib": True, "complevel": 5} for var in data.coords},
         **kwargs,
     )
-
-
-def save_as_fits():
-    # TODO
-    raise NotImplementedError
```

### Comparing `erlab-2.3.2/src/erlab/lattice.py` & `erlab-2.4.0/src/erlab/lattice.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 import numpy as np
 import numpy.typing as npt
 
 
 def angle_between(v1: npt.NDArray[np.float64], v2: npt.NDArray[np.float64]) -> float:
-    """Returns the angle between two vectors.
+    """Return the angle between two vectors.
 
     Parameters
     ----------
     v1, v2:
         1D array of length 3, specifying a vector.
 
     Returns
@@ -27,15 +27,15 @@
     """
     return np.rad2deg(np.arccos(np.clip(np.dot(v1, v2), -1.0, 1.0)))
 
 
 def abc2avec(
     a: float, b: float, c: float, alpha: float, beta: float, gamma: float
 ) -> npt.NDArray:
-    """Constructs lattice vectors from lattice parameters."""
+    """Construct lattice vectors from lattice parameters."""
     alpha, beta, gamma = np.deg2rad(alpha), np.deg2rad(beta), np.deg2rad(gamma)
     sa, ca, sb, cb, cg = (
         np.sin(alpha),
         np.cos(alpha),
         np.sin(beta),
         np.cos(beta),
         np.cos(gamma),
@@ -51,24 +51,24 @@
         ]
     )
 
 
 def avec2abc(
     avec: npt.NDArray[np.float64],
 ) -> tuple[np.floating, np.floating, np.floating, float, float, float]:
-    """Determines lattice parameters from lattice vectors."""
+    """Determine lattice parameters from lattice vectors."""
     a, b, c = (np.linalg.norm(x) for x in avec)
     alpha = angle_between(avec[1] / b, avec[2] / c)
     beta = angle_between(avec[2] / c, avec[0] / a)
     gamma = angle_between(avec[0] / a, avec[1] / b)
     return a, b, c, alpha, beta, gamma
 
 
 def to_reciprocal(avec: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
-    """Constructs the reciprocal lattice vectors from real lattice vectors.
+    """Construct the reciprocal lattice vectors from real lattice vectors.
 
     Parameters
     ----------
     avec
         Real lattice vectors, given as a 3 by 3 numpy array with each basis vector given
         in each row.
 
@@ -77,15 +77,15 @@
     bvec
         The reciprocal lattice vectors.
     """
     return 2 * np.pi * np.linalg.inv(avec).T
 
 
 def to_real(bvec: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
-    """Constructs the real lattice vectors from reciprocal lattice vectors.
+    """Construct the real lattice vectors from reciprocal lattice vectors.
 
     Parameters
     ----------
     bvec
         Reciprocal lattice vectors, given as a 3 by 3 numpy array with each basis vector
         given in each row.
```

### Comparing `erlab-2.3.2/src/erlab/parallel.py` & `erlab-2.4.0/src/erlab/parallel.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 import joblib._parallel_backends
 import tqdm.auto
 from qtpy import QtCore
 
 
 @contextlib.contextmanager
 def joblib_progress(file=None, **kwargs):
-    """Context manager to patch joblib to report into tqdm progress bar given as
-    argument"""
-
+    """Patches joblib to report into a tqdm progress bar."""
     if file is None:
         file = sys.stdout
 
     tqdm_object = tqdm.auto.tqdm(iterable=None, file=file, **kwargs)
 
     def tqdm_print_progress(self):
         if self.n_completed_tasks > tqdm_object.n:
```

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.4.0/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.4.0/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/__init__.py` & `erlab-2.4.0/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/annotations.py` & `erlab-2.4.0/src/erlab/plotting/annotations.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,64 @@
     "pico",
     "femto",
     "atto",
     "zepto",
     "yocto",
 )  #: Names of the SI prefixes.
 
+PRETTY_NAMES: dict[str, tuple[str, str]] = {
+    "temperature": ("Temperature", "Temperature"),
+    "T": (r"\ensuremath{T}", r"$T$"),
+    "beta": (r"\ensuremath{\beta}", r"$\beta$"),
+    "theta": (r"\ensuremath{\theta}", r"$\theta$"),
+    "chi": (r"\ensuremath{\chi}", r"$\chi$"),
+    "alpha": (r"\ensuremath{\alpha}", r"$\alpha$"),
+    "psi": (r"\ensuremath{\psi}", r"$\psi$"),
+    "phi": (r"\ensuremath{\phi}", r"$\phi$"),
+    "xi": (r"\ensuremath{\xi}", r"$\xi$"),
+    "Eb": (r"\ensuremath{E}", r"$E$"),
+    "Ek": (r"\ensuremath{E_{\text{kin}}}", r"$E_{\text{kin}}$"),
+    "eV": (r"\ensuremath{E-E_F}", r"$E-E_F$"),
+    "kx": (r"\ensuremath{k_{x}}", r"$k_x$"),
+    "ky": (r"\ensuremath{k_{y}}", r"$k_y$"),
+    "kz": (r"\ensuremath{k_{z}}", r"$k_z$"),
+    "kp": (r"\ensuremath{k_{\parallel}}", r"$k_\parallel$"),
+    "hv": (r"\ensuremath{h\nu}", r"$h\nu$"),
+}
+"""Pretty names for labeling plots.
+
+The first element is for LaTeX, and the second is for plain text.
+
+"""
+
+PRETTY_UNITS: dict[str, tuple[str, str]] = {
+    "temperature": (r"K", r"K"),
+    "T": (r"K", r"K"),
+    "theta": (r"deg", r"deg"),
+    "beta": (r"deg", r"deg"),
+    "psi": (r"deg", r"deg"),
+    "chi": (r"deg", r"deg"),
+    "alpha": (r"deg", r"deg"),
+    "phi": (r"deg", r"deg"),
+    "xi": (r"deg", r"deg"),
+    "Eb": (r"eV", r"eV"),
+    "Ek": (r"eV", r"eV"),
+    "eV": (r"eV", r"eV"),
+    "hv": (r"eV", r"eV"),
+    "kx": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
+    "ky": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
+    "kz": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
+    "kp": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
+}
+"""Pretty units for labeling plots.
+
+The first element is for LaTeX, and the second is for plain text.
+
+"""
+
 
 def _alph_label(val, prefix, suffix, numeric, capital):
     """Generate labels from string or integer."""
     if isinstance(val, int | np.integer) or val.isdigit():
         if numeric:
             val = str(val)
         else:
@@ -119,15 +169,15 @@
     try:
         return m.group(1)
     except IndexError:
         return None
 
 
 def get_si_str(si: int) -> str:
-    """Returns the SI prefix string to be plotted by :mod:`matplotlib`.
+    """Return the SI prefix string to be plotted by :mod:`matplotlib`.
 
     Parameters
     ----------
     si : int
         Exponent of 10 corresponding to a SI prefix.
 
     Returns
@@ -141,91 +191,59 @@
     else:
         try:
             return SI_PREFIXES[si]
         except KeyError as e:
             raise ValueError("Invalid SI prefix.") from e
 
 
-def name_for_dim(dim_name, escaped=True):
-    name = {
-        "temperature": ("Temperature", "Temperature"),
-        "T": (r"\ensuremath{T}", r"$T$"),
-        "beta": (r"\ensuremath{\beta}", r"$\beta$"),
-        "theta": (r"\ensuremath{\theta}", r"$\theta$"),
-        "chi": (r"\ensuremath{\chi}", r"$\chi$"),
-        "alpha": (r"\ensuremath{\alpha}", r"$\alpha$"),
-        "psi": (r"\ensuremath{\psi}", r"$\psi$"),
-        "phi": (r"\ensuremath{\phi}", r"$\phi$"),
-        "xi": (r"\ensuremath{\xi}", r"$\xi$"),
-        "Eb": (r"\ensuremath{E}", r"$E$"),
-        "eV": (r"\ensuremath{E-E_F}", r"$E-E_F$"),
-        "kx": (r"\ensuremath{k_{x}}", r"$k_x$"),
-        "ky": (r"\ensuremath{k_{y}}", r"$k_y$"),
-        "kz": (r"\ensuremath{k_{z}}", r"$k_z$"),
-        "kp": (r"\ensuremath{k_{\parallel}}", r"$k_\parallel$"),
-        "hv": (r"\ensuremath{h\nu}", r"$h\nu$"),
-    }.get(dim_name)
+def name_for_dim(dim_name: str, escaped: bool = True) -> str:
+    names: tuple[str, str] | None = PRETTY_NAMES.get(dim_name)
 
-    if name is None:
+    if names is None:
         name = dim_name
     else:
-        name = name[0] if plt.rcParams["text.usetex"] else name[1]
+        name = names[0] if plt.rcParams["text.usetex"] else names[1]
 
     if not escaped:
         name = name.replace("$", "")
     return name
 
 
-def unit_for_dim(dim_name, deg2rad=False):
-    unit = {
-        "temperature": (r"K", r"K"),
-        "T": (r"K", r"K"),
-        "theta": (r"deg", r"deg"),
-        "beta": (r"deg", r"deg"),
-        "psi": (r"deg", r"deg"),
-        "chi": (r"deg", r"deg"),
-        "alpha": (r"deg", r"deg"),
-        "phi": (r"deg", r"deg"),
-        "xi": (r"deg", r"deg"),
-        "Eb": (r"eV", r"eV"),
-        "eV": (r"eV", r"eV"),
-        "hv": (r"eV", r"eV"),
-        "kx": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
-        "ky": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
-        "kz": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
-        "kp": (r"Å\ensuremath{{}^{-1}}", r"Å${}^{-1}$"),
-    }.get(dim_name)
+def unit_for_dim(dim_name: str, deg2rad: bool = False) -> str:
+    units: tuple[str, str] | None = PRETTY_UNITS.get(dim_name)
 
-    if unit is None:
+    if units is None:
         unit = ""
     else:
-        unit = unit[0] if plt.rcParams["text.usetex"] else unit[1]
+        unit = units[0] if plt.rcParams["text.usetex"] else units[1]
+
     if deg2rad:
         unit = unit.replace("deg", "rad")
     return unit
 
 
-def label_for_dim(dim_name, deg2rad=False, escaped=True):
+def label_for_dim(dim_name: str, deg2rad: bool = False, escaped: bool = True) -> str:
     name = name_for_dim(dim_name, escaped=escaped)
     unit = unit_for_dim(dim_name, deg2rad=deg2rad)
     if unit == "":
         return name
     else:
         return f"{name} ({unit})"
 
 
-def parse_special_point(name):
+def parse_special_point(name: str) -> str:
     special_points = {"G": r"\Gamma", "D": r"\Delta"}
-    try:
+
+    if name in special_points.keys():
         return special_points[name]
-    except KeyError:
+    else:
         return name
 
 
-def parse_point_labels(name: str, roman=True, bar=False):
+def parse_point_labels(name: str, roman: bool = True, bar: bool = False) -> str:
     name = parse_special_point(name)
 
     if name.endswith("*"):
         name = name[:-1]
         if roman:
             format_str = r"\mathdefault{{{}}}^*"
         else:
@@ -459,15 +477,14 @@
         Set the font size. The default is ``'medium'`` for axes, and ``'large'`` for
         figures.
     **kwargs
         Extra arguments to `matplotlib.text.Text`: refer to the `matplotlib`
         documentation for a list of all possible arguments.
 
     """
-
     kwargs["fontweight"] = fontweight
     if plt.rcParams["text.usetex"] & (fontweight == "bold"):
         prefix = "\\textbf{" + prefix
         suffix = suffix + "}"
         kwargs.pop("fontweight")
 
     axlist = np.array(axes, dtype=object).flatten(order=order)
@@ -579,15 +596,14 @@
         Set the font size. The default is ``'medium'`` for axes, and ``'large'`` for
         figures.
     **kwargs
         Extra arguments to `matplotlib.text.Text`: refer to the `matplotlib`
         documentation for a list of all possible arguments.
 
     """
-
     kwargs["fontweight"] = fontweight
     if plt.rcParams["text.usetex"] & (fontweight == "bold"):
         prefix = "\\textbf{" + prefix
         suffix = suffix + "}"
         kwargs.pop("fontweight")
 
     axlist = np.array(axes, dtype=object).flatten(order=order)
@@ -760,31 +776,34 @@
         label_ax.set_yticklabels(
             [parse_point_labels(lab, roman, bar) for lab in labels]
         )
         # label_ax.set_zorder(a.get_zorder())
         label_ax.set_frame_on(False)
 
 
-# TODO: fix format using name_for_dim and unit_for_dim
 def plot_hv_text(ax, val, x=0.025, y=0.975, **kwargs):
-    s = "$h\\nu=" + str(val) + "$~eV"
+    name = name_for_dim("hv", escaped=False)
+    unit = unit_for_dim("hv")
+    s = f"${name}={val}$ {unit}"
     ax.text(
         x,
         y,
         s,
         family="serif",
         horizontalalignment="left",
         verticalalignment="top",
         transform=ax.transAxes,
         **kwargs,
     )
 
 
 def plot_hv_text_right(ax, val, x=1 - 0.025, y=0.975, **kwargs):
-    s = "$h\\nu=" + str(val) + "$~eV"
+    name = name_for_dim("hv", escaped=False)
+    unit = unit_for_dim("hv")
+    s = f"${name}={val}$ {unit}"
     ax.text(
         x,
         y,
         s,
         family="serif",
         horizontalalignment="right",
         verticalalignment="top",
@@ -835,15 +854,20 @@
     def __init__(self, si: int = 0, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._si_exponent = int(si)
 
     def __call__(self, x, pos=None):
         self.orderOfMagnitude += self._si_exponent
 
-        sigfigs = int(re.match(r".*{%1.(\d+)f}", self.format).group(1))
+        match_format = re.match(r".*{%1.(\d+)f}", self.format)
+        if match_format is None:
+            # Match failed, may be due to changes in matplotlib
+            raise RuntimeError("Failed to match format string. Please report this bug")
+
+        sigfigs = int(match_format.group(1))
         self.format = self.format.replace(
             f"%1.{sigfigs}f", f"%1.{max(0, sigfigs + self._si_exponent)}f"
         )
         val = super().__call__(x, pos)
 
         self.orderOfMagnitude -= self._si_exponent
         return val
@@ -855,16 +879,17 @@
     si: int = 0,
     *,
     prefix: bool = True,
     power: bool = False,
 ):
     """Rescales ticks and adds an SI prefix to the axis label.
 
-    Useful when you want to rescale the ticks. For example, when plotting a cut from a
-    low pass energy scan, you might want to convert the energy units from eV to meV.
+    Useful when you want to rescale the ticks without actually rescaling the data. For
+    example, when plotting a cut from a low pass energy scan, you might want to convert
+    the energy units from eV to meV.
 
     Using this function on an axis where the major locator is not the default formatter
     `matplotlib.ticker.ScalarFormatter` will result in undefined behavior.
 
     Parameters
     ----------
     ax
@@ -944,15 +969,15 @@
     ] = "lower right",
     pad: float = 0.1,
     borderpad: float = 0.5,
     sep: float = 3.0,
     frameon: bool = False,
     **kwargs,
 ):
-    """
+    """Add a size bar to an axes.
 
     Parameters
     ----------
     ax
         The `matplotlib.axes.Axes` instance to place the size bar in.
     value
         Length of the size bar in terms of `unit`.
@@ -977,15 +1002,14 @@
     frameon
         If True, draw a box around the horizontal bar and label.
     **kwargs
         Keyword arguments forwarded to
         `mpl_toolkits.axes_grid1.anchored_artists.AnchoredSizeBar`.
 
     """
-
     size = value / resolution
     unit = get_si_str(si) + unit
     value = np.around(value / 10**si, decimals=decimals)
     if int(value) == value:
         value = int(value)
     if label is None:
         label = f"{value} {unit}"
```

### Comparing `erlab-2.3.2/src/erlab/plotting/atoms.py` & `erlab-2.4.0/src/erlab/plotting/atoms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+"""Plot atoms.
+
 Classes and functions for plotting atoms and bonds in a crystal structure using
 matplotlib's 3D plotting capabilities.
 
 Some of the projection code was adapted from kwant.
 
 """
 
@@ -22,15 +23,15 @@
 import numpy.typing as npt
 from matplotlib.typing import ColorType
 
 __all__ = ["Atom3DCollection", "Bond3DCollection", "CrystalProperty"]
 
 
 def sunflower_sphere(n: int = 100) -> npt.NDArray[np.float64]:
-    """Returns n points on a sphere using the sunflower algorithm."""
+    """Return n points on a sphere using the sunflower algorithm."""
     indices = np.arange(0, n, dtype=float) + 0.5
 
     phi = np.arccos(1 - 2 * indices / n)
     theta = np.pi * (1 + 5**0.5) * indices
 
     return np.c_[
         np.cos(theta) * np.sin(phi), np.sin(theta) * np.sin(phi), np.cos(phi)
@@ -93,16 +94,19 @@
     rc[:2] = transform(*rc, proj)[:2]
 
     coords = rp - rc[:2]
     return np.linalg.norm(coords, axis=0).mean()
 
 
 def _zalpha(colors, zs):
-    """Modified from `mpl_toolkits.mplot3d.art3d` to modifies the brightness of the
-    color based on depth, rather than setting the transparency."""
+    """Set alpha based on zdepth.
+
+    Modified from `mpl_toolkits.mplot3d.art3d` to modifies the brightness of the
+    color based on depth, rather than setting the transparency.
+    """
     if len(colors) == 0 or len(zs) == 0:
         return np.zeros((0, 4))
     norm = plt.Normalize(min(zs), max(zs))
     sats = 1 - norm(zs) * 0.7
     rgba = np.broadcast_to(matplotlib.colors.to_rgba_array(colors), (len(zs), 4))
     rgba = rgba.T * sats
     rgba += 1 - sats
@@ -187,17 +191,15 @@
     #     self._factor = (
     #         self._sz_real * ((args[0] + args[3]) / 2) * 72.0 / self.figure.dpi
     #     )
     #     super().draw(renderer)
 
 
 class Bond3DCollection(mpl_toolkits.mplot3d.art3d.Line3DCollection):
-    """
-    A subclass of `mpl_toolkits.mplot3d.art3d.Line3DCollection` representing a
-    collection of 3D bonds.
+    """A collection of 3D lines that represents bonds in a crystal structure.
 
     Parameters
     ----------
     segments
         List of segments representing the bonds.
     scale_linewidths
         Boolean indicating whether to scale the linewidths based on the plot's
@@ -251,18 +253,19 @@
         radii: Iterable[float] | None = None,
         colors: Iterable[ColorType] | None = None,
         repeat: tuple[int, int, int] = (1, 1, 1),
         bounds: Mapping[Literal["x", "y", "z"], tuple[float, float]] | None = None,
         mask: Callable | None = None,
         r_factor: float = 0.4,
     ):
-        """
-        A class that stores the information required to plot a three dimensional crystal
-        structure. The crystal can be repeated along the lattice vectors, and can be
-        masked. Bonds can be added between atoms.
+        """Properties of a crystal structure for plotting.
+
+        Stores the information required to plot a three dimensional crystal structure.
+        The crystal can be repeated along the lattice vectors, and can be masked. Bonds
+        can be added between atoms.
 
         Parameters
         ----------
         atom_pos
             A dictionary of atom positions in the unit cell, where the keys are the atom
             names and the values are the positions of the atoms. The positions can be
             given as a (N, 3) numpy array or a list of N numpy arrays of shape (3,).
@@ -467,15 +470,14 @@
         bond_kw
             Keyword arguments passed onto `Bond3DCollection`
         atom_kw
             Keyword arguments passed onto `mpl_toolkits.mplot3d.Axes3D.scatter` used to
             plot the atoms.
 
         """
-
         if ax is None:
             ax = plt.gcf().add_subplot(projection="3d")
         ax = cast(mpl_toolkits.mplot3d.Axes3D, ax)
 
         if clean_axes:
             ax.set_facecolor("none")
             ax.xaxis.set_pane_color((1, 1, 1, 0))
```

### Comparing `erlab-2.3.2/src/erlab/plotting/bz.py` & `erlab-2.4.0/src/erlab/plotting/bz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """Utilities for plotting Brillouin zones."""
 
 __all__ = ["get_bz_edge", "plot_hex_bz"]
 
 import itertools
+from typing import Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
 import scipy.spatial
 from matplotlib.patches import RegularPolygon
 
 from erlab.plotting.colors import axes_textcolor
 
-abbrv_kws = {
-    "facecolor": ["fc", "none"],
-    "linestyle": ["ls", "--"],
-    "linewidth": ["lw", 0.5],
+abbrv_kws: dict[str, tuple[str, Any]] = {
+    "facecolor": ("fc", "none"),
+    "linestyle": ("ls", "--"),
+    "linewidth": ("lw", 0.5),
 }
 
 
 def get_bz_edge(
     basis: npt.NDArray[np.float64],
     reciprocal: bool = True,
     extend: tuple[int, ...] | None = None,
 ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
-    """Calculates the edge of the first Brillouin zone (BZ) from lattice vectors.
+    """Calculate the edge of the first Brillouin zone (BZ) from lattice vectors.
 
     Parameters
     ----------
     basis
         ``(N, N)`` numpy array where ``N = 2``or ``3`` with each row containing the
         lattice vectors.
     reciprocal
@@ -113,17 +114,15 @@
 
     return lines_arr, vertices_arr
 
 
 def plot_hex_bz(
     a=3.54, rotate=0.0, offset=(0.0, 0.0), reciprocal=True, ax=None, **kwargs
 ):
-    """
-    Plots a 2D hexagonal BZ overlay on the specified axes.
-    """
+    """Plot a 2D hexagonal BZ overlay on the specified axes."""
     kwargs.setdefault("zorder", 5)
     for k, v in abbrv_kws.items():
         kwargs[k] = kwargs.pop(k, kwargs.pop(*v))
     if ax is None:
         ax = plt.gca()
     if np.iterable(ax):
         return [
```

### Comparing `erlab-2.3.2/src/erlab/plotting/colors.py` & `erlab-2.4.0/src/erlab/plotting/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,42 +56,43 @@
 import matplotlib.colorbar
 import matplotlib.colors
 import matplotlib.image
 import matplotlib.pyplot as plt
 import matplotlib.transforms
 import numpy as np
 import numpy.typing as npt
-from matplotlib.typing import ColorType
+from matplotlib.typing import ColorType, RGBColorType
 
 
 class InversePowerNorm(matplotlib.colors.Normalize):
-    r"""
+    r"""Inverse power-law normalization.
+
     Linearly map a given value to the 0-1 range and then apply an inverse power-law
     normalization over that range.
 
-    For values :math:`x`, `matplotlib.colors.PowerNorm` calculates
-    :math:`x^\gamma`, whereas `InversePowerNorm` calculates :math:`1-x^{1/\gamma}`.
-    This provides higher contrast for values closer to ``vmin``.
+    For values :math:`x`, `matplotlib.colors.PowerNorm` calculates :math:`x^\gamma`,
+    whereas `InversePowerNorm` calculates :math:`1-x^{1/\gamma}`. This provides higher
+    contrast for values closer to ``vmin``.
 
     Parameters
     ----------
     gamma
         Power law normalization parameter. If equal to 1, the colormap is linear.
     vmin, vmax
-        If ``vmin`` and/or ``vmax`` is not given, they are initialized from the
-        minimum and maximum value, respectively, of the first input
-        processed; i.e., ``__call__(A)`` calls ``autoscale_None(A)``
+        If ``vmin`` and/or ``vmax`` is not given, they are initialized from the minimum
+        and maximum value, respectively, of the first input processed; i.e.,
+        ``__call__(A)`` calls ``autoscale_None(A)``
     clip
-        If ``True`` values falling outside the range ``[vmin, vmax]``,
-        are mapped to 0 or 1, whichever is closer, and masked values are
-        set to 1.  If ``False`` masked values remain masked.
-
-        Clipping silently defeats the purpose of setting the over, under,
-        and masked colors in a colormap, so it is likely to lead to
-        surprises; therefore the default is ``clip=False``.
+        If ``True`` values falling outside the range ``[vmin, vmax]``, are mapped to 0
+        or 1, whichever is closer, and masked values are set to 1.  If ``False`` masked
+        values remain masked.
+
+        Clipping silently defeats the purpose of setting the over, under, and masked
+        colors in a colormap, so it is likely to lead to surprises; therefore the
+        default is ``clip=False``.
 
     """
 
     def __init__(
         self,
         gamma: float,
         vmin: float | None = None,
@@ -104,14 +105,15 @@
     def __call__(self, value, clip=None):
         if clip is None:
             clip = self.clip
 
         result, is_scalar = self.process_value(value)
 
         self.autoscale_None(result)
+
         gamma = self.gamma
         vmin, vmax = self.vmin, self.vmax
         if vmin > vmax:
             raise ValueError("minvalue must be less than or equal to maxvalue")
         elif vmin == vmax:
             result.fill(0)
         else:
@@ -267,17 +269,15 @@
     ):
         super().__init__(vcenter=vcenter, vmin=vmin, vmax=vmax)
         self.gamma = gamma
         self._func = _diverging_powernorm
         self._func_i = _diverging_powernorm_inv
 
     def __call__(self, value, clip=None):
-        """
-        Map value to the interval [0, 1]. The clip argument is unused.
-        """
+        """Map value to the interval [0, 1]. The clip argument is unused."""
         result, is_scalar = self.process_value(value)
 
         self.autoscale_None(result)
         gamma = self.gamma
         vmin, vcenter, vmax = self.vmin, self.vcenter, self.vmax
         if not vmin <= vcenter <= vmax:
             raise ValueError("vmin, vcenter, vmax must increase monotonically")
@@ -340,17 +340,15 @@
     ):
         super().__init__(vcenter=vcenter, halfrange=halfrange, clip=clip)
         self.gamma = gamma
         self._func = _diverging_powernorm
         self._func_i = _diverging_powernorm_inv
 
     def __call__(self, value, clip=None):
-        """
-        Map value to the interval [0, 1].
-        """
+        """Map value to the interval [0, 1]."""
         if clip is None:
             clip = self.clip
 
         result, is_scalar = self.process_value(value)
 
         self.autoscale_None(result)
         gamma = self.gamma
@@ -458,15 +456,15 @@
         self._func = _diverging_inversepowernorm
         self._func_i = _diverging_inversepowernorm_inv
 
 
 def get_mappable(
     ax: matplotlib.axes.Axes, image_only: bool = False, silent: bool = False
 ) -> matplotlib.cm.ScalarMappable | None:
-    """Gets the `matplotlib.cm.ScalarMappable` from a given `matplotlib.axes.Axes`.
+    """Get the `matplotlib.cm.ScalarMappable` from a given `matplotlib.axes.Axes`.
 
     Parameters
     ----------
     ax
         Parent axes.
     image_only
         Only consider images as a valid mappable, by default `False`.
@@ -549,15 +547,15 @@
 def proportional_colorbar(
     mappable: matplotlib.cm.ScalarMappable | None = None,
     cax: matplotlib.axes.Axes | None = None,
     ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] | None = None,
     **kwargs,
 ) -> matplotlib.colorbar.Colorbar:
     """
-    Replaces the current colorbar or creates a new colorbar with proportional spacing.
+    Replace the current colorbar or creates a new colorbar with proportional spacing.
 
     The default behavior of colorbars in `matplotlib` does not support colors
     proportional to data in different norms. This function circumvents this behavior.
 
     Parameters
     ----------
     mappable
@@ -628,17 +626,14 @@
 
     ticks = mappable.colorbar.get_ticks()
     if cax is None:
         mappable.colorbar.remove()
     kwargs.setdefault("ticks", ticks)
     kwargs.setdefault("cmap", mappable.cmap)
     kwargs.setdefault("norm", mappable.norm)
-    kwargs.setdefault("pad", 0.05)
-    kwargs.setdefault("fraction", 0.05)
-    kwargs.setdefault("aspect", 25)
 
     cbar = plt.colorbar(
         mappable=mappable,
         cax=cax,
         ax=ax,
         spacing="proportional",
         boundaries=kwargs["norm"].inverse(np.linspace(0, 1, kwargs["cmap"].N)),
@@ -755,15 +750,15 @@
         self.set_pad(pad)
 
     def __call__(self, ax, renderer):
         return matplotlib.transforms.TransformedBbox(
             matplotlib.transforms.Bbox.from_bounds(*self._size_to_bounds(ax)),
             self._transAxes
             + matplotlib.transforms.ScaledTranslation(
-                *self.pads, ax.figure.dpi_scale_trans
+                self.pads[0], self.pads[1], ax.figure.dpi_scale_trans
             )
             - ax.figure.transSubfigure,
         )
 
     def set_pad(self, pad):
         pad_num = False
         if isinstance(pad, Number):
@@ -823,28 +818,27 @@
     if horiz:
         cax = _ez_inset(ax, h, w, pad=(0, -w - pad / 72), **kwargs)
     else:
         cax = _ez_inset(ax, w, h, pad=(-w - pad / 72, 0), **kwargs)
     return cax
 
 
-# TODO: fix colorbar size properly
 def nice_colorbar(
     ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] | None = None,
     mappable: matplotlib.cm.ScalarMappable | None = None,
-    width: float = 5.0,
+    width: float = 8.0,
     aspect: float = 5.0,
     pad: float = 3.0,
     minmax: bool = False,
     orientation: Literal["vertical", "horizontal"] = "vertical",
     floating=False,
     ticklabels: Sequence[str] | None = None,
     **kwargs,
 ):
-    r"""Creates a colorbar with fixed width and aspect to ensure uniformity of plots.
+    r"""Create a colorbar with fixed width and aspect to ensure uniformity of plots.
 
     Parameters
     ----------
     ax
         The `matplotlib.axes.Axes` instance in which the colorbar is drawn.
     mappable
         The mappable whose colormap and norm will be used.
@@ -865,15 +859,14 @@
 
     Returns
     -------
     cbar : matplotlib.colorbar.Colorbar
         The created colorbar.
 
     """
-
     is_horizontal = orientation == "horizontal"
 
     if ax is None:
         ax = plt.gca()
 
     if floating:
         if isinstance(ax, np.ndarray):
@@ -896,27 +889,33 @@
 
     else:
         if isinstance(ax, Iterable):
             if not isinstance(ax, np.ndarray):
                 ax = np.array(ax, dtype=object)
             bbox = matplotlib.transforms.Bbox.union(
                 [
-                    x.get_window_extent().transformed(
-                        x.figure.dpi_scale_trans.inverted()
-                    )
+                    x.get_position(original=True)
+                    .frozen()
+                    .transformed(x.figure.transFigure)
+                    .transformed(x.figure.dpi_scale_trans.inverted())
                     for x in ax.flat
                 ]
             )
         else:
             fig = ax.get_figure()
 
             if fig is None:
                 raise RuntimeError("Axes is not attached to a figure")
 
-            bbox = ax.get_window_extent().transformed(fig.dpi_scale_trans.inverted())
+            bbox = (
+                ax.get_position(original=True)
+                .frozen()
+                .transformed(fig.transFigure)
+                .transformed(fig.dpi_scale_trans.inverted())
+            )
 
         if orientation == "horizontal":
             kwargs["anchor"] = (1, 1)
             kwargs["location"] = "top"
             kwargs["fraction"] = width / (72 * bbox.height)
             kwargs["pad"] = pad / (72 * bbox.height)
             kwargs["shrink"] = width * aspect / (72 * bbox.width)
@@ -950,28 +949,31 @@
         cbar.ax.set_box_aspect(1 / aspect)
     else:
         cbar.ax.set_box_aspect(aspect)
 
     return cbar
 
 
-def flatten_transparency(rgba: npt.NDArray, background: Sequence[float] | None = None):
+def flatten_transparency(rgba: npt.NDArray, background: RGBColorType | None = None):
     """
     Flatten the transparency of an RGBA image by blending it with a background color.
 
     Parameters
     ----------
     rgba
         The input RGBA image as a numpy array.
-    background
-        The background color to blend with. Defaults to white ``(1, 1, 1)``.
+    background : RGBColorType, optional
+        The background color to blend with. Defaults to white.
 
     """
     if background is None:
         background = (1, 1, 1)
+    else:
+        background = matplotlib.colors.to_rgb(background)
+
     original_shape = rgba.shape
     rgba = rgba.reshape(-1, 4)
     rgb = rgba[:, :-1]
     a = rgba[:, -1][:, np.newaxis]
     rgb *= a
     rgb += (1 - a) * background
     return rgb.reshape(original_shape[:-1] + (3,))
@@ -1094,15 +1096,15 @@
     cmap
         The colormap to use for the color axis. If `None`, a predefined linear segmented
         colormap is used.
     lnorm
         The normalization for the lightness axes.
     cnorm
         The normalization for the color axes.
-    background
+    background : ColorType, optional
         The background color. If `None`, it is set to white.
     N
         The number of levels in the colormap. Default is 256. The resulting colormap
         will have a shape of ``(N, N, 4)``, where the last dimension represents the RGBA
         values.
 
     Returns
@@ -1158,21 +1160,21 @@
 
 
 def color_distance(c1: ColorType, c2: ColorType) -> float:
     """Calculate the color distance between two matplotlib colors.
 
     Parameters
     ----------
-    c1, c2
+    c1, c2 : ColorType
         Color to calculate the distance between in any format that
         :func:`matplotlib.colors.to_rgb` can handle.
 
     Returns
     -------
-    float
+    distance : float
         The color distance between the two colors.
 
     Note
     ----
     The color distance is calculated using the Euclidean distance formula in the RGB
     color space. The formula takes into account the perceptual differences between
     colors.
@@ -1192,15 +1194,15 @@
 
 
 def close_to_white(c: ColorType) -> bool:
     """Check if a given color is closer to white than black.
 
     Parameters
     ----------
-    c
+    c : ColorType
         Color in any format that :func:`matplotlib.colors.to_rgb` can handle.
 
     Returns
     -------
     bool
         `True` if the color is closer to white than black, `False` otherwise.
     """
@@ -1224,36 +1226,35 @@
     mx = hist.argmax()
     return im.to_rgba(edges[mx : mx + 2].mean())
 
 
 def image_is_light(
     im: matplotlib.image._ImageBase | matplotlib.collections.QuadMesh,
 ) -> bool:
-    """
-    Determines if an image is *light* or *dark* by checking whether the prominent color
-    is closer to white than black.
+    """Determine if an image is *light* or *dark*.
 
+    Checks whether the prominent color is closer to white than black.
     """
     return close_to_white(prominent_color(im))
 
 
 def axes_textcolor(
     ax: matplotlib.axes.Axes, light: ColorType = "k", dark: ColorType = "w"
 ):
     """Determine the text color based on the color of the mappable in an axes.
 
     Parameters
     ----------
-    ax
+    ax : matplotlib.axes.Axes
         The axes object for which the text color needs to be determined.
-    light
+    light : ColorType
         The *light* color, returned when :func:`image_is_light
         <erlab.plotting.colors.image_is_light>` returns `False`. Default is ``'w'``
         (white).
-    dark
+    dark : ColorType
         The *dark* color, returned when :func:`image_is_light
         <erlab.plotting.colors.image_is_light>` returns `True`. Default is ``'k'``
         (black).
 
     """
     c = light
     mappable = get_mappable(ax, silent=True)
```

### Comparing `erlab-2.3.2/src/erlab/plotting/erplot.py` & `erlab-2.4.0/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/general.py` & `erlab-2.4.0/src/erlab/plotting/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,20 @@
     "plot_array",
     "plot_array_2d",
     "plot_slices",
 ]
 
 import contextlib
 import copy
+import warnings
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any, Literal, Union, cast
 
 import matplotlib
+import matplotlib.colorbar
 import matplotlib.colors
 import matplotlib.image
 import matplotlib.patches
 import matplotlib.path
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
@@ -39,14 +41,16 @@
     gen_2d_colormap,
     nice_colorbar,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Collection, Sequence
 
+    from matplotlib.typing import ColorType
+
 figure_width_ref = {
     "aps": [3.4, 7.0],
     "aip": [3.37, 6.69],
     "nature": [88 / 25.4, 180 / 25.4],
 }
 
 
@@ -162,25 +166,25 @@
         self.linev = ax.axvline(ax.get_xbound()[0], **lineprops)
         with plt.rc_context({"text.usetex": False}):
             self.label = ax.text(0.95, 0.95, "", **textprops)
         self.background = None
         self.needclear = False
 
     def clear(self, event):
-        """Internal event handler to clear the cursor."""
+        """Clear the cursor."""
         if self.ignore(event):
             return
         if self.useblit:
             self.background = self.canvas.copy_from_bbox(self.ax.bbox)
         self.linev.set_visible(False)
         self.lineh.set_visible(False)
         self.label.set_visible(False)
 
     def onmove(self, event):
-        """Internal event handler to draw the cursor when the mouse moves."""
+        """Draw the cursor when the mouse moves."""
         if self.ignore(event):
             return
         if not self.canvas.widgetlock.available(self):
             return
         if event.inaxes != self.ax:
             self.linev.set_visible(False)
             self.lineh.set_visible(False)
@@ -252,35 +256,51 @@
 
     Returns
     -------
     matplotlib.axes.Axes
 
 
     """
-
     return _ez_inset(parent_axes, width, height, pad, loc, **kwargs)
 
 
-def array_extent(data: xr.DataArray) -> tuple[float, float, float, float]:
-    """
-    Gets the extent of a :class:`xarray.DataArray` to be used in
-    :func:`matplotlib.pyplot.imshow`.
+def array_extent(
+    darr: xr.DataArray, rtol: float = 1.0e-5, atol: float = 1.0e-8
+) -> tuple[float, float, float, float]:
+    """Get the extent of a :class:`xarray.DataArray`.
+
+    The extent can be used as the `extent` argument in :func:`matplotlib.pyplot.imshow`.
 
     Parameters
     ----------
-    data
+    darr
         A two-dimensional :class:`xarray.DataArray`.
+    rtol, atol
+        Tolerance for the coordinates to be considered evenly spaced. The default values
+        are consistent with `numpy.isclose`.
 
     Returns
     -------
     x0, x1, y0, y1 : float
 
     """
+    if darr.ndim != 2:
+        raise ValueError("Input array must be 2D")
+
+    data_coords = tuple(darr[dim].values for dim in darr.dims)
+    for dim, coord in zip(darr.dims, data_coords, strict=True):
+        dif = np.diff(coord)
+        if not np.allclose(dif, dif[0], rtol=rtol, atol=atol):
+            warnings.warn(
+                f"Coordinates for {dim} are not evenly spaced, and the plot may not be "
+                "accurate. Use `DataArray.plot`, `xarray.plot.pcolormesh` or "
+                "`matplotlib.pyplot.pcolormesh` for non-evenly spaced data.",
+                stacklevel=2,
+            )
 
-    data_coords = tuple(data[dim].values for dim in data.dims)
     data_incs = tuple(coord[1] - coord[0] for coord in data_coords)
     data_lims = tuple((coord[0], coord[-1]) for coord in data_coords)
     y0, x0 = data_lims[0][0] - 0.5 * data_incs[0], data_lims[1][0] - 0.5 * data_incs[1]
     y1, x1 = (
         data_lims[0][-1] + 0.5 * data_incs[0],
         data_lims[1][-1] + 0.5 * data_incs[1],
     )
@@ -297,22 +317,24 @@
     norm: matplotlib.colors.Normalize | None = None,
     xlim: float | tuple[float, float] | None = None,
     ylim: float | tuple[float, float] | None = None,
     crop: bool = False,
     rad2deg: bool | Iterable[str] = False,
     func: Callable | None = None,
     func_args: dict | None = None,
+    rtol: float = 1.0e-5,
+    atol: float = 1.0e-8,
     **improps,
 ) -> matplotlib.image.AxesImage:
-    """Plots a 2D :class:`xarray.DataArray` using :func:`matplotlib.pyplot.imshow`.
+    """Plot a 2D :class:`xarray.DataArray` using :func:`matplotlib.pyplot.imshow`.
 
     Parameters
     ----------
     arr
-        A two-dimensional :class:`xarray.DataArray` to be plotted.
+        A two-dimensional :class:`xarray.DataArray` with evenly spaced coordinates.
     ax
         The target :class:`matplotlib.axes.Axes`.
     colorbar
         Whether to plot a colorbar.
     colorbar_kw
         Keyword arguments passed onto :func:`erlab.plotting.colors.nice_colorbar`.
     xlim, ylim
@@ -324,14 +346,18 @@
         iterable of `str` is given, only the coordinates that correspond to the given
         strings are converted.
     func
         A callable that processes the values prior to display. Its output must have the
         same shape as the input.
     func_args
         Keyword arguments passed onto `func`.
+    rtol, atol
+        By default, the input array is checked for evenly spaced coordinates. ``rtol``
+        and ``atol`` are the tolerances for the coordinates to be considered evenly
+        spaced. The default values are consistent with `numpy.isclose`.
     **improps
         Keyword arguments passed onto :func:`matplotlib.axes.Axes.imshow`.
 
     Returns
     -------
     matplotlib.image.AxesImage
 
@@ -375,15 +401,15 @@
         colorbar_kw.setdefault("extend", "max")
 
     if norm is None:
         norm = copy.deepcopy(matplotlib.colors.PowerNorm(gamma, **norm_kw))
 
     improps_default = {
         "interpolation": "none",
-        "extent": array_extent(arr),
+        "extent": array_extent(arr, rtol, atol),
         "aspect": "auto",
         "origin": "lower",
         "rasterized": True,
     }
     for k, v in improps_default.items():
         improps.setdefault(k, v)
 
@@ -420,22 +446,92 @@
     *,
     normalize_with_larr: bool = False,
     xlim: float | tuple[float, float] | None = None,
     ylim: float | tuple[float, float] | None = None,
     cmap: matplotlib.colors.Colormap | str | None = None,
     lnorm: matplotlib.colors.Normalize | None = None,
     cnorm: matplotlib.colors.Normalize | None = None,
-    background: Any = None,
+    background: ColorType | None = None,
     colorbar: bool = True,
     cax: matplotlib.axes.Axes | None = None,
     colorbar_kw: dict | None = None,
     imshow_kw: dict | None = None,
     N: int = 256,
+    rtol: float = 1.0e-5,
+    atol: float = 1.0e-8,
     **indexers_kwargs,
-):
+) -> tuple[matplotlib.image.AxesImage, matplotlib.colorbar.Colorbar | None]:
+    """
+    Plot a 2D array with associated color array.
+
+    The lightness array represents the intensity values, while the color array
+    represents some other property. The arrays must have the same shape.
+
+    Parameters
+    ----------
+    larr
+        The 2D array representing the lightness values.
+    carr
+        The 2D array representing the color values.
+    ax
+        The axes on which to plot the array. If None, the current axes will be used.
+    normalize_with_larr
+        Whether to normalize the color array with the lightness array. Default is False.
+    xlim
+        The x-axis limits for the plot. If a float, it represents the symmetric limits
+        around 0. If a tuple, it represents the lower and upper limits. If None, the
+        limits are determined from the data.
+    ylim
+        The y-axis limits for the plot. If a float, it represents the symmetric limits
+        around 0. If a tuple, it represents the lower and upper limits. If None, the
+        limits are determined from the data.
+    cmap
+        The colormap to use for the color array. If None, a linear segmented colormap
+        consisting of blue, black, and red is used.
+    lnorm
+        The normalization object for the lightness array.
+    cnorm
+        The normalization object for the color array.
+    background
+        The background color to use for the plot. If None, white is used.
+    colorbar
+        Whether to create a colorbar. Default is `True`.
+    cax
+        The axes on which to create the colorbar if `colorbar` is `True`. If None, a new
+        axes will be created for the colorbar.
+    colorbar_kw
+        Additional keyword arguments to pass to `matplotlib.pyplot.colorbar`.
+    imshow_kw
+        Additional keyword arguments to pass to `matplotlib.pyplot.imshow`.
+    N
+        The number of levels in the colormap. Default is 256.
+    rtol, atol
+        By default, the input array is checked for evenly spaced coordinates. ``rtol``
+        and ``atol`` are the tolerances for the coordinates to be considered evenly
+        spaced. The default values are consistent with `numpy.isclose`.
+    **indexers_kwargs : dict
+        Additional keyword arguments to pass to `qsel` to select the data to plot. Note
+        that the resulting data after the selection must be 2D.
+
+    Returns
+    -------
+    im : matplotlib.image.AxesImage
+        The plotted image.
+    cb : matplotlib.colorbar.Colorbar or None
+        The colorbar associated with the plot. If `colorbar` is False, None is returned.
+
+    Example
+    -------
+    >>> import erlab.plotting.erplot as eplt
+    >>> import matplotlib.pyplot as plt
+    >>> import xarray as xr
+    >>> larr = xr.DataArray([[1, 2, 3], [4, 5, 6]])
+    >>> carr = xr.DataArray([[0.1, 0.2, 0.3], [0.4, 0.5, 0.6]])
+    >>> eplt.plot_array_2d(larr, carr)
+    """
     if lnorm is None:
         lnorm = plt.Normalize()
     else:
         lnorm = copy.deepcopy(lnorm)
     if cnorm is None:
         cnorm = plt.Normalize()
     else:
@@ -453,14 +549,18 @@
     for k, v in improps_default.items():
         imshow_kw.setdefault(k, v)
     if ax is None:
         ax = plt.gca()
 
     larr = larr.qsel(**indexers_kwargs).copy(deep=True)
     carr = carr.qsel(**indexers_kwargs).copy(deep=True)
+
+    if larr.shape != carr.shape:
+        raise ValueError("Lightness and color array must have the same shape")
+
     sel_kw = {}
 
     if xlim is not None:
         if not isinstance(xlim, Iterable):
             xlim = (-xlim, xlim)
         sel_kw[larr.dims[1]] = slice(*xlim)
 
@@ -513,15 +613,15 @@
         cax.imshow(
             cmap_img.transpose(1, 0, 2),
             extent=(lmin, lmax, cmin, cmax),
             origin="lower",
             aspect="auto",
         )
 
-    im = ax.imshow(img, extent=array_extent(larr), **imshow_kw)
+    im = ax.imshow(img, extent=array_extent(larr, rtol, atol), **imshow_kw)
     ax.set_xlabel(str(larr.dims[0]))
     ax.set_ylabel(str(larr.dims[1]))
     fancy_labels(ax)
 
     if colorbar:
         return im, cb
     else:
@@ -535,15 +635,15 @@
     color: str | tuple[float, float, float] | tuple[float, float, float, float] = "C0",
     cmap: str | matplotlib.colors.Colormap | None = None,
     transpose: bool = False,
     reverse: bool = False,
     ax: matplotlib.axes.Axes | None = None,
     **kwargs,
 ) -> matplotlib.image.AxesImage:
-    """Applies a gradient fill to a line plot.
+    """Apply a gradient fill to a line plot.
 
     Parameters
     ----------
     x, y
         Data of the plot to fill under.
     y0
         The minimum y value of the gradient. If `None`, defaults to the minimum of `y`.
@@ -997,15 +1097,15 @@
 
 def fermiline(
     ax: matplotlib.axes.Axes | None = None,
     value: float = 0.0,
     orientation: Literal["h", "v"] = "h",
     **kwargs,
 ) -> matplotlib.lines.Line2D | MultipleLine2D:
-    """Plots a constant energy line to denote the Fermi level.
+    """Plot a constant energy line to denote the Fermi level.
 
     Parameters
     ----------
     ax
         The `matplotlib.axes.Axes` to annotate.
     value
         The coordinate of the line. Defaults to 0, assuming binding energy.
```

### Comparing `erlab-2.3.2/src/erlab/plotting/plot3d.py` & `erlab-2.4.0/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.4.0/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.4.0/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.4.0/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.4.0/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.4.0/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.4.0/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/src/erlab.egg-info/PKG-INFO` & `erlab-2.4.0/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.3.2
+Version: 2.4.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,46 +696,55 @@
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
 Requires-Dist: igor2>=0.5.6
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: lmfit!=1.3.0,>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: numba>=0.59.0
-Requires-Dist: numbagg>=0.8.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
 Requires-Dist: qtawesome>=1.3.1
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: uncertainties>=3.1.4
 Requires-Dist: varname>=0.13.0
 Requires-Dist: xarray>=2024.02.0
+Provides-Extra: complete
+Requires-Dist: erlab[dev,misc,perf,viz]; extra == "complete"
+Provides-Extra: viz
+Requires-Dist: cmasher; extra == "viz"
+Requires-Dist: cmocean; extra == "viz"
+Requires-Dist: colorcet; extra == "viz"
+Requires-Dist: hvplot; extra == "viz"
+Requires-Dist: ipywidgets; extra == "viz"
+Provides-Extra: perf
+Requires-Dist: numbagg>=0.8.1; extra == "perf"
+Requires-Dist: bottleneck>=1.3.8; extra == "perf"
+Provides-Extra: misc
+Requires-Dist: iminuit>=2.25.2; extra == "misc"
+Requires-Dist: csaps>=1.1.0; extra == "misc"
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: python-semantic-release; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: sphinx-qt-documentation; extra == "docs"
 Requires-Dist: pybtex; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: python-semantic-release; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Provides-Extra: viz
-Requires-Dist: cmasher; extra == "viz"
-Requires-Dist: cmocean; extra == "viz"
-Requires-Dist: colorcet; extra == "viz"
-Requires-Dist: hvplot; extra == "viz"
-Requires-Dist: ipywidgets; extra == "viz"
 
 <h1 align="center">
 ERLabPy
 </h1>
 <p align="center">
     <a href="https://pypi.org/project/erlab/" alt="Supported Python Versions">
         <img src="https://img.shields.io/pypi/pyversions/erlab?logo=python&logoColor=white" /></a>
```

### Comparing `erlab-2.3.2/src/erlab.egg-info/SOURCES.txt` & `erlab-2.4.0/src/erlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/templates/.macros.j2` & `erlab-2.4.0/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/tests/accessors/test_fit.py` & `erlab-2.4.0/tests/accessors/test_fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/tests/accessors/test_kspace.py` & `erlab-2.4.0/tests/accessors/test_kspace.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 import xarray
 import xarray.testing
-from erlab.io.exampledata import generate_data_angles
 from erlab.analysis.kspace import AxesConfiguration
+from erlab.io.exampledata import generate_data_angles
 
 
 @pytest.fixture()
 def map():
     return generate_data_angles(shape=(10, 10, 10), assign_attributes=True)
```

### Comparing `erlab-2.3.2/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.4.0/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/tests/analysis/test_fit_functions_general.py` & `erlab-2.4.0/tests/analysis/test_fit_functions_general.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,28 +51,40 @@
     x = np.linspace(0, 10, 5)
 
     def testfunc(x):
         return x
 
     resolution = 1.0
     expected = np.array(
-        [-6.61744490e-24, 5.87148334e00, 1.17429667e01, 1.76144500e01, 2.34859334e01]
+        [
+            -6.61744490e-24,
+            5.87148334e00,
+            1.17429667e01,
+            1.76144500e01,
+            2.34859334e01,
+        ]
     )
     result = do_convolve(x, testfunc, resolution)
     assert np.allclose(result, expected)
 
     # Test case 2: Convolve a sine function with a Gaussian kernel
     x = np.linspace(0, 2 * np.pi, 5)
 
     def testfunc(x):
         return np.sin(x)
 
     resolution = 0.5
     expected = np.array(
-        [0.00000000e00, 2.95132925e00, 3.61433592e-16, -2.95132925e00, -7.22867185e-16]
+        [
+            0.00000000e00,
+            2.95132925e00,
+            3.61433592e-16,
+            -2.95132925e00,
+            -7.22867185e-16,
+        ]
     )
     result = do_convolve(x, testfunc, resolution)
     assert np.allclose(result, expected)
 
 
 def test_gaussian_wh():
     x = np.linspace(0, 10, 100)
```

### Comparing `erlab-2.3.2/tests/analysis/test_fit_models.py` & `erlab-2.4.0/tests/analysis/test_fit_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+import erlab.analysis.fit.models as models
 import numpy as np
 import xarray as xr
 
-import erlab.analysis.fit.models as models
-
 
 def test_fermi_edge_model():
     # Create a test input DataArray
     x = np.linspace(-0.1, 0.1, 100)
     data = np.zeros_like(x)
 
     # Create an instance of FermiEdgeModel
```

### Comparing `erlab-2.3.2/tests/analysis/test_image.py` & `erlab-2.4.0/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/tests/analysis/test_kspace.py` & `erlab-2.4.0/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/tests/analysis/test_utilities.py` & `erlab-2.4.0/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.2/tests/io/test_dataloader.py` & `erlab-2.4.0/tests/io/test_dataloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     # Generate a map
     beta_coords = np.linspace(2, 7, 10)
 
     for i, beta in enumerate(beta_coords):
         erlab.io.save_as_hdf5(
             make_data(beta=beta, temp=20.0, hv=50.0),
-            filename=f"{tmp_dir.name}/data_001_S{str(i+1).zfill(3)}.h5",
+            filename=f"{tmp_dir.name}/data_001_S{str(i + 1).zfill(3)}.h5",
             igor_compat=False,
         )
 
     # Write scan coordinates to a csv file
     with open(f"{tmp_dir.name}/data_001_axis.csv", "w", newline="") as file:
         writer = csv.writer(file)
         writer.writerow(["Index", "Polar"])
```

