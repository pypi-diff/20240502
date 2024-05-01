# Comparing `tmp/spleenseg-1.2.26.tar.gz` & `tmp/spleenseg-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleenseg-1.2.26.tar", last modified: Wed May  1 23:32:09 2024, max compression
+gzip compressed data, was "spleenseg-1.2.4.tar", last modified: Sun Apr 28 15:13:17 2024, max compression
```

## Comparing `spleenseg-1.2.26.tar` & `spleenseg-1.2.4.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.295155 spleenseg-1.2.26/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-17 00:36:10.000000 spleenseg-1.2.26/LICENSE
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    10319 2024-05-01 23:32:09.295155 spleenseg-1.2.26/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8577 2024-05-01 23:30:41.000000 spleenseg-1.2.26/README.md
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9143 2024-05-01 23:32:07.000000 spleenseg-1.2.26/README.rst
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      238 2024-04-26 18:25:29.000000 spleenseg-1.2.26/requirements.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-05-01 23:32:09.295155 spleenseg-1.2.26/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1903 2024-04-30 22:21:09.000000 spleenseg-1.2.26/setup.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.291822 spleenseg-1.2.26/spleenseg/
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.291822 spleenseg-1.2.26/spleenseg/comms/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     4878 2024-04-30 22:32:17.000000 spleenseg-1.2.26/spleenseg/comms/rpc.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.291822 spleenseg-1.2.26/spleenseg/core/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    24201 2024-04-26 18:36:17.000000 spleenseg-1.2.26/spleenseg/core/neuralnet.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.291822 spleenseg-1.2.26/spleenseg/models/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3221 2024-04-26 18:36:17.000000 spleenseg-1.2.26/spleenseg/models/data.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.291822 spleenseg-1.2.26/spleenseg/plotting/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2113 2024-04-26 18:36:17.000000 spleenseg-1.2.26/spleenseg/plotting/plotting.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     8620 2024-05-01 23:25:52.000000 spleenseg-1.2.26/spleenseg/spleenseg.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7133 2024-05-01 23:25:29.000000 spleenseg-1.2.26/spleenseg/splparser.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.291822 spleenseg-1.2.26/spleenseg/transforms/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7650 2024-04-24 22:01:17.000000 spleenseg-1.2.26/spleenseg/transforms/transforms.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-05-01 23:32:09.291822 spleenseg-1.2.26/spleenseg.egg-info/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    10319 2024-05-01 23:32:09.000000 spleenseg-1.2.26/spleenseg.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      442 2024-05-01 23:32:09.000000 spleenseg-1.2.26/spleenseg.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-05-01 23:32:09.000000 spleenseg-1.2.26/spleenseg.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       55 2024-05-01 23:32:09.000000 spleenseg-1.2.26/spleenseg.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      251 2024-05-01 23:32:09.000000 spleenseg-1.2.26/spleenseg.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       98 2024-05-01 23:32:09.000000 spleenseg-1.2.26/spleenseg.egg-info/top_level.txt
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.917607 spleenseg-1.2.4/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1069 2024-04-17 00:36:10.000000 spleenseg-1.2.4/LICENSE
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     8016 2024-04-28 15:13:17.917607 spleenseg-1.2.4/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6405 2024-04-26 18:36:17.000000 spleenseg-1.2.4/README.md
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6841 2024-04-28 15:13:16.000000 spleenseg-1.2.4/README.rst
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      238 2024-04-26 18:25:29.000000 spleenseg-1.2.4/requirements.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-04-28 15:13:17.917607 spleenseg-1.2.4/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1876 2024-04-26 18:34:46.000000 spleenseg-1.2.4/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/core/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    24201 2024-04-26 18:36:17.000000 spleenseg-1.2.4/spleenseg/core/neuralnet.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/models/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     3221 2024-04-26 18:36:17.000000 spleenseg-1.2.4/spleenseg/models/data.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/plotting/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2113 2024-04-26 18:36:17.000000 spleenseg-1.2.4/spleenseg/plotting/plotting.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     9173 2024-04-26 18:39:18.000000 spleenseg-1.2.4/spleenseg/spleenseg.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg/transforms/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     7650 2024-04-24 22:01:17.000000 spleenseg-1.2.4/spleenseg/transforms/transforms.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/spleenseg.egg-info/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     8016 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      418 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       55 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      251 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       82 2024-04-28 15:13:17.000000 spleenseg-1.2.4/spleenseg.egg-info/top_level.txt
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-04-28 15:13:17.914273 spleenseg-1.2.4/tests/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      662 2024-04-17 00:36:10.000000 spleenseg-1.2.4/tests/test_example.py
```

### Comparing `spleenseg-1.2.26/LICENSE` & `spleenseg-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.26/PKG-INFO` & `spleenseg-1.2.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleenseg
-Version: 1.2.26
+Version: 1.2.4
 Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
 Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
@@ -55,28 +55,28 @@
 Abstract
 --------
 
 Based off Project MONAI’s `spleen segmentation
 notebook <https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/spleen_segmentation_3d.ipynb>`__,
 this plugin implements both the *training* and *inference* phases of the
 notebook, using data supplied in the *parent* plugin (see
-Implementation).
-
-For the most part, the python notebook code could have been mostly used
-*verbatim* in the plugin; however, in this example considerable and
-deeper refactoring was performed. Other than of course now being a
-complete stand alone implementation, this plugin allows for *continuous*
-(or *continued*) training, as well as saving examples of all
-training/validation/inference datasets as NIfTI volumes to allow for
-better understanding of the process.
+Implementation). For the most part, the python notebook code can be used
+*verbatim* in the plugin; however, in this example some deeper
+refactoring (adding typing, and some refactoring) to improve its use as
+a stand-alone application.
+
+In general, notebooks are not ideal for batch usage, and often cells
+repeat code used elsewhere in the notebook. This plugin code
+consolidated and generalized many of these cells into functions,
+reducing the overall code footprint considerably.
 
 For the *training* phase, the parent plugin provides input images
-(training and labeled) and the output is a model (``pth`` or ``ONNX``
-format). For the *inference* phase, the input is a model file, an image
-(or more) to analyze, and the output is a segmented volume file.
+(training and labeled) and the output is a model (``pth`` and ``ONNX``
+format). For the *inference* phase, the input is a model file, and an
+image with the output being a segmented result.
 
 Implementation
 --------------
 
 The original notebook is a largely self-contained *monolithic*
 application. Exemplar input data is pulled from the web, and the
 notebook proceeds from there. In the case of this ChRIS plugin, some
@@ -88,28 +88,16 @@
 Installation
 ------------
 
 ``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__
 *plugin*, meaning it can run from either within *ChRIS* or the
 command-line.
 
-On the metal
-~~~~~~~~~~~~
-
-Despite being a ChRIS plugin, *on the metal* development/usage is
-supported. Simply check out the repository and do a ``pip install`` to
-either a local ``venv`` or an existing one:
-
-.. code:: bash
-
-   pip install -U ./
-   spleenseg --help
-
-Apptainer
-~~~~~~~~~
+Local Usage
+-----------
 
 To get started with local command-line usage, use
 `Apptainer <https://apptainer.org/>`__ (a.k.a. Singularity) to run
 ``pl-monai_spleenseg`` as a container:
 
 .. code:: shell
 
@@ -118,65 +106,14 @@
 
 To print its available options, run:
 
 .. code:: shell
 
    apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train --help
 
-Usage
------
-
-.. code:: html
-
-       ARGS
-           [--mode <inference|training>]
-           The mode of operation. If the actual text "training" text has any additional characters,
-           then the epoch training is skipped and only the post-training logic is executed --
-           this allows the system to operate as if in training mode, but only perform the post
-           training steps. For example, "--mode trainingPost" would invoke this mode.
-
-           If the mode is specified as <model>@<remote> (e.g. splsegv1@http://pfms.org/api/v1/)
-           then the pfms server at (in this example) http://pfms.org with base route /api/v1/
-           is used to perform remote inference. Here, the model called "splsegv1" on the remote
-           pfms server will be used to run inference. The return from this call is a NIfTI
-           segmented volume saved in the <outputDir>.
-
-           [--man]
-           If specified, print this help page and quit.
-
-           [--version]
-           If specified, print the version and quit.
-
-           [--logTransformVols]
-           If specified, log a set of intermediary NIfTI volumes as used for training,
-           validation, spacing, and inference.
-
-           [--useModel <modelFile>]
-           If specified, use <modelFile> for inference or continued training.
-
-           [--trainImageDir <train> --trainLabelsDir <label>]
-           In the <inputDir>, the name of the directory containing files for training
-           with their corresponding label targets.
-
-           [--testImageDir]
-           In the <inputDir> the name of the directory containing images for inference.
-
-           [--device <device>]
-           The device to use, typically "cpu" or "cuda:0".
-
-           [--determinismSeed <seed>]
-           Set the training seed.
-
-           [--maxEpochs <count>]
-           The max number of training epochs.
-
-           [--validateSize <size>]
-           In the training space, the number of images that should be used for validation
-           and not training.
-
 Examples
 --------
 
 ``spleenseg_train`` requires two positional arguments: a directory
 containing input data, and a directory containing output data (graphs
 and “model” files). In this plugin, data is downloaded from
 `medicaldecathelon <http://medicaldecathelon.com>`__. To get this data,
@@ -216,15 +153,15 @@
 
 Create some ``output`` directory, and using our ``$MONAI_DATA_DIR``, we
 can run the plugin:
 
 .. code:: shell
 
    mkdir outgoing/
-   apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg \
+   apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg_train \
            [--args] $MONAI_DATA_DIR outgoing/
 
 Development
 -----------
 
 Instructions for developers.
 
@@ -242,17 +179,17 @@
 
 Mount the source code ``spleenseg_train.py`` into a container to try out
 changes without rebuild.
 
 .. code:: shell
 
    docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-       -v $PWD/spleenseg/spleenseg.py:/usr/local/lib/python3.12/site-packages/spleenseg/spleenseg.py:ro \
+       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.12/site-packages/spleenseg_train.py:ro \
        -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
-       localhost/fnndsc/pl-monai_spleenseg spleenseg /incoming /outgoing
+       localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
 
 Testing
 ~~~~~~~
 
 Run unit tests using ``pytest``. It’s recommended to rebuild the image
 to ensure that sources are up-to-date. Use the option
 ``--build-arg extras_require=dev`` to install extra dependencies for
```

### Comparing `spleenseg-1.2.26/README.md` & `spleenseg-1.2.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -4,109 +4,49 @@
 [![MIT License](https://img.shields.io/github/license/fnndsc/pl-monai_spleenseg)](https://github.com/FNNDSC/pl-monai_spleenseg/blob/main/LICENSE)
 [![ci](https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml/badge.svg)](https://github.com/FNNDSC/pl-monai_spleenseg/actions/workflows/ci.yml)
 
 `pl-monai_spleenseg` is a [_ChRIS_](https://chrisproject.org/) _DS_ plugin based off Project MONAI's spleen segmentation exemplar. This plugin implements the training and inference phases as two distinct modes of operation. For training, input files are a set of training examples (images and segmented images) and output files are training plots and weight (model) files in `pth` and `ONNX` format. For inference, input files are a model file and an image to segment.
 
 ## Abstract
 
-Based off Project MONAI's [spleen segmentation notebook](https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/spleen_segmentation_3d.ipynb), this plugin implements both the _training_ and _inference_ phases of the notebook, using data supplied in the _parent_ plugin (see Implementation).
+Based off Project MONAI's [spleen segmentation notebook](https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/spleen_segmentation_3d.ipynb), this plugin implements both the _training_ and _inference_ phases of the notebook, using data supplied in the _parent_ plugin (see Implementation). For the most part, the python notebook code can be used _verbatim_ in the plugin; however, in this example some deeper refactoring (adding typing, and some refactoring) to improve its use as a stand-alone application.
 
-For the most part, the python notebook code could have been mostly used _verbatim_ in the plugin; however, in this example considerable and deeper refactoring was performed. Other than of course now being a complete stand alone implementation, this plugin allows for _continuous_ (or _continued_) training, as well as saving examples of all training/validation/inference datasets as NIfTI volumes to allow for better understanding of the process.
+In general, notebooks are not ideal for batch usage, and often cells repeat code used elsewhere in the notebook. This plugin code consolidated and generalized many of these cells into functions, reducing the overall code footprint considerably.
 
-For the _training_ phase, the parent plugin provides input images (training and labeled) and the output is a model (`pth` or `ONNX` format). For the _inference_ phase, the input is a model file, an image (or more) to analyze, and the output is a segmented volume file.
+For the _training_ phase, the parent plugin provides input images (training and labeled) and the output is a model (`pth` and `ONNX` format). For the _inference_ phase, the input is a model file, and an image with the output being a segmented result.
 
 ## Implementation
 
 The original notebook is a largely self-contained _monolithic_ application. Exemplar input data is pulled from the web, and the notebook proceeds from there. In the case of this ChRIS plugin, some straightforward organizational changes are necessary. The training data is assumed to already have been downloaded _a priori_ and is provided to this plugin by its _parent_. Outputs of the training are model weight filesTh.
 
 ## Installation
 
 `pl-monai_spleenseg` is a _[ChRIS](https://chrisproject.org/) plugin_, meaning it can
 run from either within _ChRIS_ or the command-line.
 
-### On the metal
-
-Despite being a ChRIS plugin, _on the metal_ development/usage is supported. Simply check out the repository and do a `pip install` to either a local `venv` or an existing one:
-
-```bash
-pip install -U ./
-spleenseg --help
-```
-
-### Apptainer
+## Local Usage
 
 To get started with local command-line usage, use [Apptainer](https://apptainer.org/) (a.k.a. Singularity) to run `pl-monai_spleenseg` as a container:
 
 ```shell
 apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train \
             [--args values...] input/ output/
 ```
 
 To print its available options, run:
 
 ```shell
 apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train --help
 ```
 
-## Usage
-
-```html
-    ARGS
-        [--mode <inference|training>]
-        The mode of operation. If the actual text "training" text has any additional characters,
-        then the epoch training is skipped and only the post-training logic is executed --
-        this allows the system to operate as if in training mode, but only perform the post
-        training steps. For example, "--mode trainingPost" would invoke this mode.
-
-        If the mode is specified as <model>@<remote> (e.g. splsegv1@http://pfms.org/api/v1/)
-        then the pfms server at (in this example) http://pfms.org with base route /api/v1/
-        is used to perform remote inference. Here, the model called "splsegv1" on the remote
-        pfms server will be used to run inference. The return from this call is a NIfTI
-        segmented volume saved in the <outputDir>.
-
-        [--man]
-        If specified, print this help page and quit.
-
-        [--version]
-        If specified, print the version and quit.
-
-        [--logTransformVols]
-        If specified, log a set of intermediary NIfTI volumes as used for training,
-        validation, spacing, and inference.
-
-        [--useModel <modelFile>]
-        If specified, use <modelFile> for inference or continued training.
-
-        [--trainImageDir <train> --trainLabelsDir <label>]
-        In the <inputDir>, the name of the directory containing files for training
-        with their corresponding label targets.
-
-        [--testImageDir]
-        In the <inputDir> the name of the directory containing images for inference.
-
-        [--device <device>]
-        The device to use, typically "cpu" or "cuda:0".
-
-        [--determinismSeed <seed>]
-        Set the training seed.
-
-        [--maxEpochs <count>]
-        The max number of training epochs.
-
-        [--validateSize <size>]
-        In the training space, the number of images that should be used for validation
-        and not training.
-
-```
-
 ## Examples
 
 `spleenseg_train` requires two positional arguments: a directory containing input data, and a directory containing output data (graphs and "model" files). In this plugin, data is downloaded from [medicaldecathelon](http://medicaldecathelon.com). To get this data, first set an environment variable pointing at the directory to contain the pulled and unpacked data:
 
-```bash
+```bash 
 export MONAI_DATA_DIR=/some/dir
 ```
 
 now, you can pull the data with this python snippet:
 
 ```python
 # You probably will need to
@@ -124,23 +64,23 @@
 data_dir = os.path.join(root_dir, "Task09_Spleen")
 if not os.path.exists(data_dir):
     download_and_extract(resource, compressed_file, root_dir, md5)
 ```
 
 Or simply run the supplied `trainingDataPull.py` script (which is essentially the above code):
 
-```bash
+```bash 
 python trainingDataPull.py
 ```
 
 Create some `output` directory, and using our `$MONAI_DATA_DIR`, we can run the plugin:
 
 ```shell
 mkdir outgoing/
-apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg \
+apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg_train \
         [--args] $MONAI_DATA_DIR outgoing/
 ```
 
 ## Development
 
 Instructions for developers.
 
@@ -154,17 +94,17 @@
 
 ### Running
 
 Mount the source code `spleenseg_train.py` into a container to try out changes without rebuild.
 
 ```shell
 docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-    -v $PWD/spleenseg/spleenseg.py:/usr/local/lib/python3.12/site-packages/spleenseg/spleenseg.py:ro \
+    -v $PWD/spleenseg_train.py:/usr/local/lib/python3.12/site-packages/spleenseg_train.py:ro \
     -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
-    localhost/fnndsc/pl-monai_spleenseg spleenseg /incoming /outgoing
+    localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
 ```
 
 ### Testing
 
 Run unit tests using `pytest`. It's recommended to rebuild the image to ensure that sources are up-to-date. Use the option `--build-arg extras_require=dev` to install extra dependencies for testing.
 
 ```shell
```

### Comparing `spleenseg-1.2.26/README.rst` & `spleenseg-1.2.4/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 Abstract
 --------
 
 Based off Project MONAI’s `spleen segmentation
 notebook <https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/spleen_segmentation_3d.ipynb>`__,
 this plugin implements both the *training* and *inference* phases of the
 notebook, using data supplied in the *parent* plugin (see
-Implementation).
-
-For the most part, the python notebook code could have been mostly used
-*verbatim* in the plugin; however, in this example considerable and
-deeper refactoring was performed. Other than of course now being a
-complete stand alone implementation, this plugin allows for *continuous*
-(or *continued*) training, as well as saving examples of all
-training/validation/inference datasets as NIfTI volumes to allow for
-better understanding of the process.
+Implementation). For the most part, the python notebook code can be used
+*verbatim* in the plugin; however, in this example some deeper
+refactoring (adding typing, and some refactoring) to improve its use as
+a stand-alone application.
+
+In general, notebooks are not ideal for batch usage, and often cells
+repeat code used elsewhere in the notebook. This plugin code
+consolidated and generalized many of these cells into functions,
+reducing the overall code footprint considerably.
 
 For the *training* phase, the parent plugin provides input images
-(training and labeled) and the output is a model (``pth`` or ``ONNX``
-format). For the *inference* phase, the input is a model file, an image
-(or more) to analyze, and the output is a segmented volume file.
+(training and labeled) and the output is a model (``pth`` and ``ONNX``
+format). For the *inference* phase, the input is a model file, and an
+image with the output being a segmented result.
 
 Implementation
 --------------
 
 The original notebook is a largely self-contained *monolithic*
 application. Exemplar input data is pulled from the web, and the
 notebook proceeds from there. In the case of this ChRIS plugin, some
@@ -47,28 +47,16 @@
 Installation
 ------------
 
 ``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__
 *plugin*, meaning it can run from either within *ChRIS* or the
 command-line.
 
-On the metal
-~~~~~~~~~~~~
-
-Despite being a ChRIS plugin, *on the metal* development/usage is
-supported. Simply check out the repository and do a ``pip install`` to
-either a local ``venv`` or an existing one:
-
-.. code:: bash
-
-   pip install -U ./
-   spleenseg --help
-
-Apptainer
-~~~~~~~~~
+Local Usage
+-----------
 
 To get started with local command-line usage, use
 `Apptainer <https://apptainer.org/>`__ (a.k.a. Singularity) to run
 ``pl-monai_spleenseg`` as a container:
 
 .. code:: shell
 
@@ -77,65 +65,14 @@
 
 To print its available options, run:
 
 .. code:: shell
 
    apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train --help
 
-Usage
------
-
-.. code:: html
-
-       ARGS
-           [--mode <inference|training>]
-           The mode of operation. If the actual text "training" text has any additional characters,
-           then the epoch training is skipped and only the post-training logic is executed --
-           this allows the system to operate as if in training mode, but only perform the post
-           training steps. For example, "--mode trainingPost" would invoke this mode.
-
-           If the mode is specified as <model>@<remote> (e.g. splsegv1@http://pfms.org/api/v1/)
-           then the pfms server at (in this example) http://pfms.org with base route /api/v1/
-           is used to perform remote inference. Here, the model called "splsegv1" on the remote
-           pfms server will be used to run inference. The return from this call is a NIfTI
-           segmented volume saved in the <outputDir>.
-
-           [--man]
-           If specified, print this help page and quit.
-
-           [--version]
-           If specified, print the version and quit.
-
-           [--logTransformVols]
-           If specified, log a set of intermediary NIfTI volumes as used for training,
-           validation, spacing, and inference.
-
-           [--useModel <modelFile>]
-           If specified, use <modelFile> for inference or continued training.
-
-           [--trainImageDir <train> --trainLabelsDir <label>]
-           In the <inputDir>, the name of the directory containing files for training
-           with their corresponding label targets.
-
-           [--testImageDir]
-           In the <inputDir> the name of the directory containing images for inference.
-
-           [--device <device>]
-           The device to use, typically "cpu" or "cuda:0".
-
-           [--determinismSeed <seed>]
-           Set the training seed.
-
-           [--maxEpochs <count>]
-           The max number of training epochs.
-
-           [--validateSize <size>]
-           In the training space, the number of images that should be used for validation
-           and not training.
-
 Examples
 --------
 
 ``spleenseg_train`` requires two positional arguments: a directory
 containing input data, and a directory containing output data (graphs
 and “model” files). In this plugin, data is downloaded from
 `medicaldecathelon <http://medicaldecathelon.com>`__. To get this data,
@@ -175,15 +112,15 @@
 
 Create some ``output`` directory, and using our ``$MONAI_DATA_DIR``, we
 can run the plugin:
 
 .. code:: shell
 
    mkdir outgoing/
-   apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg \
+   apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg_train \
            [--args] $MONAI_DATA_DIR outgoing/
 
 Development
 -----------
 
 Instructions for developers.
 
@@ -201,17 +138,17 @@
 
 Mount the source code ``spleenseg_train.py`` into a container to try out
 changes without rebuild.
 
 .. code:: shell
 
    docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-       -v $PWD/spleenseg/spleenseg.py:/usr/local/lib/python3.12/site-packages/spleenseg/spleenseg.py:ro \
+       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.12/site-packages/spleenseg_train.py:ro \
        -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
-       localhost/fnndsc/pl-monai_spleenseg spleenseg /incoming /outgoing
+       localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
 
 Testing
 ~~~~~~~
 
 Run unit tests using ``pytest``. It’s recommended to rebuild the image
 to ensure that sources are up-to-date. Use the option
 ``--build-arg extras_require=dev`` to install extra dependencies for
```

### Comparing `spleenseg-1.2.26/setup.py` & `spleenseg-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     long_description=readme(),
     author="FNNDSC",
     author_email="dev@babyMRI.org",
     url="https://github.com/FNNDSC/pl-monai_spleenseg",
     packages=[
         "spleenseg",
         "spleenseg/core",
-        "spleenseg/comms",
         "spleenseg/models",
         "spleenseg/plotting",
         "spleenseg/transforms",
     ],
     install_requires=requirements,
     data_files=[("", ["requirements.txt"])],
     license="MIT",
```

### Comparing `spleenseg-1.2.26/spleenseg/core/neuralnet.py` & `spleenseg-1.2.4/spleenseg/core/neuralnet.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.26/spleenseg/models/data.py` & `spleenseg-1.2.4/spleenseg/models/data.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.26/spleenseg/plotting/plotting.py` & `spleenseg-1.2.4/spleenseg/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.26/spleenseg/spleenseg.py` & `spleenseg-1.2.4/spleenseg/spleenseg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,126 @@
 #!/usr/bin/env python
 
-# from collections.abc import Iterable
+from collections.abc import Iterable
 from pathlib import Path
-from argparse import Namespace
+from argparse import ArgumentParser, Namespace, ArgumentDefaultsHelpFormatter
+from dataclasses import dataclass
 
-# from dataclasses import dataclass
-
-# from matplotlib.pyplot import plot
+from matplotlib.pyplot import plot
 from monai.config.deviceconfig import print_config
-
-# from contextlib import redirect_stderr
-# from io import StringIO
+from contextlib import redirect_stderr
+from io import StringIO
 
 # import os
 import sys
 import re
 import pudb
-
-# from typing import Any, Optional, Callable
+from typing import Any, Optional, Callable
 
 from spleenseg.core import neuralnet
 from spleenseg.models.data import TrainingParams
-
-# from spleenseg.transforms import transforms
+from spleenseg.transforms import transforms
 from spleenseg.plotting import plotting
-from spleenseg.comms import rpc
 import warnings
 from pyfiglet import Figlet
 
-from chris_plugin import chris_plugin
-
 warnings.filterwarnings(
     "ignore",
     message="For details about installing the optional dependencies, please visit:",
 )
 
+from chris_plugin import chris_plugin, PathMapper
+
+__version__ = "1.2.4"
 
 DISPLAY_TITLE = r"""
 
 ███████╗██████╗ ██╗     ███████╗███████╗███╗   ██╗███████╗███████╗ ██████╗
 ██╔════╝██╔══██╗██║     ██╔════╝██╔════╝████╗  ██║██╔════╝██╔════╝██╔════╝
 ███████╗██████╔╝██║     █████╗  █████╗  ██╔██╗ ██║███████╗█████╗  ██║  ███╗
 ╚════██║██╔═══╝ ██║     ██╔══╝  ██╔══╝  ██║╚██╗██║╚════██║██╔══╝  ██║   ██║
 ███████║██║     ███████╗███████╗███████╗██║ ╚████║███████║███████╗╚██████╔╝
 ╚══════╝╚═╝     ╚══════╝╚══════╝╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝ ╚═════╝
 """
 
-__version__ = "1.2.26"
-import spleenseg.splparser as spl
 
-description: str = """
+parser = ArgumentParser(
+    description="""
 A ChRIS DS plugin based on Project MONAI 3D Spleen Segmentation.
 This plugin implements both training and inference, with some
 refactoring and pervasive type hinting.
-"""
+    """,
+    formatter_class=ArgumentDefaultsHelpFormatter,
+)
+parser.add_argument(
+    "--mode",
+    type=str,
+    default="training",
+    help="mode of behaviour: training or inference",
+)
+parser.add_argument(
+    "--logTransformVols",
+    default=False,
+    action="store_true",
+    help="If specified, save intermediary and inference data as NIfTI volumes",
+)
+parser.add_argument(
+    "--useModel",
+    type=str,
+    default="model.pth",
+    help="model to use for inference processing",
+)
+parser.add_argument(
+    "--trainImageDir",
+    type=str,
+    default="imagesTr",
+    help="name of directory containing training images",
+)
+parser.add_argument(
+    "--trainLabelsDir",
+    type=str,
+    default="labelsTr",
+    help="name of directory containing training labels",
+)
+parser.add_argument(
+    "--testImageDir",
+    type=str,
+    default="imagesTs",
+    help="name of directory containing test data",
+)
+parser.add_argument(
+    "--device",
+    type=str,
+    default="cpu",
+    help="GPU/CPU device to use",
+)
+parser.add_argument(
+    "--determinismSeed",
+    type=int,
+    default=42,
+    help="the determinism seed for training/evaluation",
+)
+parser.add_argument(
+    "--maxEpochs",
+    type=int,
+    default=600,
+    help="max number of epochs to consider",
+)
+parser.add_argument(
+    "--validateSize",
+    type=int,
+    default=9,
+    help="size of the validation set in the input raw/label space",
+)
+parser.add_argument(
+    "--pattern", type=str, default="**/[!._]*nii.gz", help="filter glob for input files"
+)
+parser.add_argument(
+    "-V", "--version", action="version", version=f"%(prog)s {__version__}"
+)
 
 
 def trainingData_prep(options: Namespace) -> list[dict[str, str]]:
     """
     Generates a list of dictionary entries, each of which is simply the name
     of an image file and its corresponding label file.
     """
@@ -102,17 +165,14 @@
     return trainingSet, validateSet
 
 
 def envDetail_print(options: Namespace, **kwargs):
     """
     Custom version of print_config() that suppresses the optional dependencies message.
     """
-    if options.man:
-        spl.manPage_print()
-        sys.exit(1)
     print(DISPLAY_TITLE)
     f = Figlet(font="doom")
     print(f.renderText(f"{options.mode}"))
     print(f"Device = {options.device}")
     print_config()
 
 
@@ -167,40 +227,16 @@
     neuralNet.testingFileSet = testingData_prep(options)
 
     neuralNet.infer_usingModel(modelFile_inputdirGet(options))
 
     return inferenceOK
 
 
-def inference_pfmsDo(neuralNet: neuralnet.NeuralNet, options: Namespace) -> bool:
-    # pudb.set_trace()
-    neuralNet.testingFileSet = testingData_prep(options)
-    remoteInfo: list[str] = options.mode.split("@")
-    modelID: str = remoteInfo[0]
-    url: str = remoteInfo[1]
-    rpcOptions: Namespace = rpc.parser_interpret(rpc.parser_setup(""), asModule=True)
-    rpcOptions.modelID = modelID
-    rpcOptions.pfms = url
-    rpcOptions.do = "infer"
-    rpcOptions.outputdir = options.outputdir
-    count: int
-    inputDict: dict[str, str]
-    for count, inputDict in enumerate(neuralNet.testingFileSet):
-        rpcOptions.outputfile = f"output-{count}.nii.gz"
-        rpcOptions.NIfTIfile = inputDict["image"]
-        print(f"{rpcOptions.NIfTIfile:46} ━━━🭬 [{rpcOptions.pfms}] ━━━🭬 ", end="")
-        remote = rpc.Rpc(rpcOptions)
-        remote.do()
-
-
-sparser = spl.parser_setup(description)
-
-
 @chris_plugin(
-    parser=sparser,
+    parser=parser,
     title="Spleen 3D image segmentation (MONAI)",
     category="",  # ref. https://chrisstore.co/plugins
     min_memory_limit="16Gi",  # supported units: Mi, Gi
     min_cpu_limit="1000m",  # millicores, e.g. "1000m" = 1 CPU core
     min_gpu_limit=0,  # set min_gpu_limit=1 to enable GPU
 )
 def main(options: Namespace, inputdir: Path, outputdir: Path):
@@ -215,20 +251,16 @@
     """
 
     # pudb.set_trace()
 
     envDetail_print(options)
     env_outputDirsMake(options)
     neuralNet: neuralnet.NeuralNet = neuralnet.NeuralNet(options)
-
     if "training" in options.mode:
         training_do(neuralNet, options)
 
     if "inference" in options.mode:
         inference_do(neuralNet, options)
 
-    if "http" in options.mode:
-        inference_pfmsDo(neuralNet, options)
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `spleenseg-1.2.26/spleenseg/transforms/transforms.py` & `spleenseg-1.2.4/spleenseg/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `spleenseg-1.2.26/spleenseg.egg-info/PKG-INFO` & `spleenseg-1.2.4/spleenseg.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleenseg
-Version: 1.2.26
+Version: 1.2.4
 Summary: A ChRIS DS plugin heavily hacked off project MONAI's spleen segmenation notebook
 Home-page: https://github.com/FNNDSC/pl-monai_spleenseg
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
@@ -55,28 +55,28 @@
 Abstract
 --------
 
 Based off Project MONAI’s `spleen segmentation
 notebook <https://github.com/Project-MONAI/tutorials/blob/main/3d_segmentation/spleen_segmentation_3d.ipynb>`__,
 this plugin implements both the *training* and *inference* phases of the
 notebook, using data supplied in the *parent* plugin (see
-Implementation).
-
-For the most part, the python notebook code could have been mostly used
-*verbatim* in the plugin; however, in this example considerable and
-deeper refactoring was performed. Other than of course now being a
-complete stand alone implementation, this plugin allows for *continuous*
-(or *continued*) training, as well as saving examples of all
-training/validation/inference datasets as NIfTI volumes to allow for
-better understanding of the process.
+Implementation). For the most part, the python notebook code can be used
+*verbatim* in the plugin; however, in this example some deeper
+refactoring (adding typing, and some refactoring) to improve its use as
+a stand-alone application.
+
+In general, notebooks are not ideal for batch usage, and often cells
+repeat code used elsewhere in the notebook. This plugin code
+consolidated and generalized many of these cells into functions,
+reducing the overall code footprint considerably.
 
 For the *training* phase, the parent plugin provides input images
-(training and labeled) and the output is a model (``pth`` or ``ONNX``
-format). For the *inference* phase, the input is a model file, an image
-(or more) to analyze, and the output is a segmented volume file.
+(training and labeled) and the output is a model (``pth`` and ``ONNX``
+format). For the *inference* phase, the input is a model file, and an
+image with the output being a segmented result.
 
 Implementation
 --------------
 
 The original notebook is a largely self-contained *monolithic*
 application. Exemplar input data is pulled from the web, and the
 notebook proceeds from there. In the case of this ChRIS plugin, some
@@ -88,28 +88,16 @@
 Installation
 ------------
 
 ``pl-monai_spleenseg`` is a `ChRIS <https://chrisproject.org/>`__
 *plugin*, meaning it can run from either within *ChRIS* or the
 command-line.
 
-On the metal
-~~~~~~~~~~~~
-
-Despite being a ChRIS plugin, *on the metal* development/usage is
-supported. Simply check out the repository and do a ``pip install`` to
-either a local ``venv`` or an existing one:
-
-.. code:: bash
-
-   pip install -U ./
-   spleenseg --help
-
-Apptainer
-~~~~~~~~~
+Local Usage
+-----------
 
 To get started with local command-line usage, use
 `Apptainer <https://apptainer.org/>`__ (a.k.a. Singularity) to run
 ``pl-monai_spleenseg`` as a container:
 
 .. code:: shell
 
@@ -118,65 +106,14 @@
 
 To print its available options, run:
 
 .. code:: shell
 
    apptainer exec docker://fnndsc/pl-monai_spleenseg spleenseg_train --help
 
-Usage
------
-
-.. code:: html
-
-       ARGS
-           [--mode <inference|training>]
-           The mode of operation. If the actual text "training" text has any additional characters,
-           then the epoch training is skipped and only the post-training logic is executed --
-           this allows the system to operate as if in training mode, but only perform the post
-           training steps. For example, "--mode trainingPost" would invoke this mode.
-
-           If the mode is specified as <model>@<remote> (e.g. splsegv1@http://pfms.org/api/v1/)
-           then the pfms server at (in this example) http://pfms.org with base route /api/v1/
-           is used to perform remote inference. Here, the model called "splsegv1" on the remote
-           pfms server will be used to run inference. The return from this call is a NIfTI
-           segmented volume saved in the <outputDir>.
-
-           [--man]
-           If specified, print this help page and quit.
-
-           [--version]
-           If specified, print the version and quit.
-
-           [--logTransformVols]
-           If specified, log a set of intermediary NIfTI volumes as used for training,
-           validation, spacing, and inference.
-
-           [--useModel <modelFile>]
-           If specified, use <modelFile> for inference or continued training.
-
-           [--trainImageDir <train> --trainLabelsDir <label>]
-           In the <inputDir>, the name of the directory containing files for training
-           with their corresponding label targets.
-
-           [--testImageDir]
-           In the <inputDir> the name of the directory containing images for inference.
-
-           [--device <device>]
-           The device to use, typically "cpu" or "cuda:0".
-
-           [--determinismSeed <seed>]
-           Set the training seed.
-
-           [--maxEpochs <count>]
-           The max number of training epochs.
-
-           [--validateSize <size>]
-           In the training space, the number of images that should be used for validation
-           and not training.
-
 Examples
 --------
 
 ``spleenseg_train`` requires two positional arguments: a directory
 containing input data, and a directory containing output data (graphs
 and “model” files). In this plugin, data is downloaded from
 `medicaldecathelon <http://medicaldecathelon.com>`__. To get this data,
@@ -216,15 +153,15 @@
 
 Create some ``output`` directory, and using our ``$MONAI_DATA_DIR``, we
 can run the plugin:
 
 .. code:: shell
 
    mkdir outgoing/
-   apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg \
+   apptainer exec docker://fnndsc/pl-monai_spleenseg:latest spleenseg_train \
            [--args] $MONAI_DATA_DIR outgoing/
 
 Development
 -----------
 
 Instructions for developers.
 
@@ -242,17 +179,17 @@
 
 Mount the source code ``spleenseg_train.py`` into a container to try out
 changes without rebuild.
 
 .. code:: shell
 
    docker run --rm -it --userns=host -u $(id -u):$(id -g) \
-       -v $PWD/spleenseg/spleenseg.py:/usr/local/lib/python3.12/site-packages/spleenseg/spleenseg.py:ro \
+       -v $PWD/spleenseg_train.py:/usr/local/lib/python3.12/site-packages/spleenseg_train.py:ro \
        -v $PWD/in:/incoming:ro -v $PWD/out:/outgoing:rw -w /outgoing \
-       localhost/fnndsc/pl-monai_spleenseg spleenseg /incoming /outgoing
+       localhost/fnndsc/pl-monai_spleenseg spleenseg_train /incoming /outgoing
 
 Testing
 ~~~~~~~
 
 Run unit tests using ``pytest``. It’s recommended to rebuild the image
 to ensure that sources are up-to-date. Use the option
 ``--build-arg extras_require=dev`` to install extra dependencies for
```

