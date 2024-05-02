# Comparing `tmp/bluepyemodel-0.0.98.tar.gz` & `tmp/bluepyemodel-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyemodel-0.0.98.tar", last modified: Tue Mar 19 17:03:09 2024, max compression
+gzip compressed data, was "bluepyemodel-0.0.99.tar", last modified: Wed Apr  3 12:52:40 2024, max compression
```

## Comparing `bluepyemodel-0.0.98.tar` & `bluepyemodel-0.0.99.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.624549 bluepyemodel-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.516549 bluepyemodel-0.0.98/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.524549 bluepyemodel-0.0.98/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.gitreview
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-03-19 17:03:09.624549 bluepyemodel-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.524549 bluepyemodel-0.0.98/bluepyemodel/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.524549 bluepyemodel-0.0.98/bluepyemodel/access_point/
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/access_point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/access_point/access_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    32799 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/access_point/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.524549 bluepyemodel-0.0.98/bluepyemodel/data/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/data/ISI_CV_Shai2015.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/data/spike_rheobase_pA_BeaulieuLaroche2021.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.528549 bluepyemodel-0.0.98/bluepyemodel/ecode/
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/apwaveform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/comb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/customfromfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.568549 bluepyemodel-0.0.98/bluepyemodel/ecode/data/
--rw-r--r--   0 runner    (1001) docker     (127) 30348440 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/data/NoiseOU3.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2574923 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/data/SubWhiteNoise.txt
--rw-r--r--   0 runner    (1001) docker     (127) 30349652 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/data/WhiteNoise.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/dehyperpol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/dendrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/firepattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/hyperdepol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/idrest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/iv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/negcheops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/noiseou3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/poscheops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/probampanmda_ems.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/random_square_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/sahp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/sinespec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/spikerec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/stimulus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/subwhitenoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/thresholdaddition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/ecode/whitenoise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.604549 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/efeatures_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/target.py
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/targets_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/targets_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/trace_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.604549 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    20506 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    56938 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.608549 bluepyemodel-0.0.98/bluepyemodel/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/efeature_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/efel_feature_bpem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    39234 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/fitness_calculator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20211 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/protocol_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    30889 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/recordings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.608549 bluepyemodel-0.0.98/bluepyemodel/export_emodel/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/export_emodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/export_emodel/export_emodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.608549 bluepyemodel-0.0.98/bluepyemodel/export_emodel/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/export_emodel/templates/cell_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/export_emodel/templates/cell_template_neurodamus.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/export_emodel/templates/cell_template_neurodamus_sbo.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/export_emodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.608549 bluepyemodel-0.0.98/bluepyemodel/model/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/distribution_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/mechanism_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/model_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/model_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/morphology_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/morphology_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/neuron_model_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/parameter_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.612549 bluepyemodel-0.0.98/bluepyemodel/optimisation/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/optimisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/optimisation/optimisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.612549 bluepyemodel-0.0.98/bluepyemodel/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tasks/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.612549 bluepyemodel-0.0.98/bluepyemodel/tasks/emodel_creation/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tasks/emodel_creation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46147 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tasks/emodel_creation/optimisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tasks/luigi_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tasks/luigi_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.612549 bluepyemodel-0.0.98/bluepyemodel/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tools/mechanisms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tools/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tools/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tools/multiprotocols_efeatures_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tools/search_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.612549 bluepyemodel-0.0.98/bluepyemodel/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/bluepyemodel/validation/validation_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.524549 bluepyemodel-0.0.98/bluepyemodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-03-19 17:03:09.000000 bluepyemodel-0.0.98/bluepyemodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-19 17:03:09.000000 bluepyemodel-0.0.98/bluepyemodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:03:09.000000 bluepyemodel-0.0.98/bluepyemodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-19 17:03:09.000000 bluepyemodel-0.0.98/bluepyemodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-19 17:03:09.000000 bluepyemodel-0.0.98/bluepyemodel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.612549 bluepyemodel-0.0.98/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.612549 bluepyemodel-0.0.98/doc/images/
--rw-r--r--   0 runner    (1001) docker     (127)   150944 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/images/classes_schema.png
--rw-r--r--   0 runner    (1001) docker     (127)   249834 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/images/pipeline.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.616549 bluepyemodel-0.0.98/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.616549 bluepyemodel-0.0.98/doc/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   170536 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/doc/source/logo/BluePyEModelBanner.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.520549 bluepyemodel-0.0.98/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.620549 bluepyemodel-0.0.98/examples/L5PC/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/LICENSE_CC-BY-CA-SA-4.0
--rw-r--r--   0 runner    (1001) docker     (127)    25073 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1472 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/analysis.sbatch
--rwxr-xr-x   0 runner    (1001) docker     (127)      965 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/analysis.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.620549 bluepyemodel-0.0.98/examples/L5PC/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.620549 bluepyemodel-0.0.98/examples/L5PC/config/extract_config/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/config/extract_config/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.620549 bluepyemodel-0.0.98/examples/L5PC/config/features/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/config/features/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.620549 bluepyemodel-0.0.98/examples/L5PC/config/params/
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/config/params/pyr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/config/recipes.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/create_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/download_ephys_data.sh
--rw-r--r--   0 runner    (1001) docker     (127)   301850 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/exploit_models.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)     1357 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/export_hoc.sbatch
--rwxr-xr-x   0 runner    (1001) docker     (127)      912 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/export_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1406 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/extract.sbatch
--rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/extract.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.620549 bluepyemodel-0.0.98/examples/L5PC/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/CaDynamics_DC0.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ca_HVA.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ca_HVA2.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/KdShu2007.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/NaTg.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/NaTg2.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/SKv3_1.mod
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/StochKv2.mod
--rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/mechanisms/StochKv3.mod
--rw-r--r--   0 runner    (1001) docker     (127)   144199 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/monitor_optimisation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/monitor_optimisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:03:09.620549 bluepyemodel-0.0.98/examples/L5PC/morphologies/
--rw-r--r--   0 runner    (1001) docker     (127)   604981 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/morphologies/C060114A5.asc
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/optimisation.sbatch
--rwxr-xr-x   0 runner    (1001) docker     (127)     1679 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/optimisation.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/examples/L5PC/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 17:03:09.624549 bluepyemodel-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-19 17:03:00.000000 bluepyemodel-0.0.98/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.703287 bluepyemodel-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.599285 bluepyemodel-0.0.99/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.603286 bluepyemodel-0.0.99/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.gitreview
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-03 12:52:40.703287 bluepyemodel-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.603286 bluepyemodel-0.0.99/bluepyemodel/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.607286 bluepyemodel-0.0.99/bluepyemodel/access_point/
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/access_point/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/access_point/access_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32789 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/access_point/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.607286 bluepyemodel-0.0.99/bluepyemodel/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/data/ISI_CV_Shai2015.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/data/spike_rheobase_pA_BeaulieuLaroche2021.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.611286 bluepyemodel-0.0.99/bluepyemodel/ecode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/apwaveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/comb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/customfromfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.647286 bluepyemodel-0.0.99/bluepyemodel/ecode/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 30348440 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/data/NoiseOU3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2574923 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/data/SubWhiteNoise.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 30349652 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/data/WhiteNoise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/dehyperpol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/dendrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/firepattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/hyperdepol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/idrest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/iv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/negcheops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/noiseou3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/poscheops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/probampanmda_ems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/random_square_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/sahp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/sinespec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/spikerec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/stimulus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/subwhitenoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/thresholdaddition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/ecode/whitenoise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.687286 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/efeatures_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/targets_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/targets_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/trace_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.687286 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20506 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56938 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.687286 bluepyemodel-0.0.99/bluepyemodel/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/efeature_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/efel_feature_bpem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39234 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/fitness_calculator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20211 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/protocol_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30889 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.687286 bluepyemodel-0.0.99/bluepyemodel/export_emodel/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/export_emodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/export_emodel/export_emodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.687286 bluepyemodel-0.0.99/bluepyemodel/export_emodel/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/export_emodel/templates/cell_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/export_emodel/templates/cell_template_neurodamus.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/export_emodel/templates/cell_template_neurodamus_sbo.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/export_emodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.691287 bluepyemodel-0.0.99/bluepyemodel/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/distribution_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/mechanism_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/model_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/model_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/morphology_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/morphology_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/neuron_model_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/parameter_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.691287 bluepyemodel-0.0.99/bluepyemodel/optimisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/optimisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/optimisation/optimisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.691287 bluepyemodel-0.0.99/bluepyemodel/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tasks/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.691287 bluepyemodel-0.0.99/bluepyemodel/tasks/emodel_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tasks/emodel_creation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46147 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tasks/emodel_creation/optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tasks/luigi_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tasks/luigi_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.691287 bluepyemodel-0.0.99/bluepyemodel/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tools/mechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tools/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tools/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tools/multiprotocols_efeatures_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tools/search_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.695287 bluepyemodel-0.0.99/bluepyemodel/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/bluepyemodel/validation/validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.607286 bluepyemodel-0.0.99/bluepyemodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-03 12:52:40.000000 bluepyemodel-0.0.99/bluepyemodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-03 12:52:40.000000 bluepyemodel-0.0.99/bluepyemodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:52:40.000000 bluepyemodel-0.0.99/bluepyemodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 12:52:40.000000 bluepyemodel-0.0.99/bluepyemodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 12:52:40.000000 bluepyemodel-0.0.99/bluepyemodel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.695287 bluepyemodel-0.0.99/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.695287 bluepyemodel-0.0.99/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   150944 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/images/classes_schema.png
+-rw-r--r--   0 runner    (1001) docker     (127)   249834 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/images/pipeline.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.695287 bluepyemodel-0.0.99/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.695287 bluepyemodel-0.0.99/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   170536 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/doc/source/logo/BluePyEModelBanner.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.599285 bluepyemodel-0.0.99/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.699287 bluepyemodel-0.0.99/examples/L5PC/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (127)    25073 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1472 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/analysis.sbatch
+-rwxr-xr-x   0 runner    (1001) docker     (127)      965 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/analysis.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.699287 bluepyemodel-0.0.99/examples/L5PC/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.699287 bluepyemodel-0.0.99/examples/L5PC/config/extract_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/config/extract_config/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.699287 bluepyemodel-0.0.99/examples/L5PC/config/features/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/config/features/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.699287 bluepyemodel-0.0.99/examples/L5PC/config/params/
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/config/params/pyr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/config/recipes.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1067 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/create_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/download_ephys_data.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   301850 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/exploit_models.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1357 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/export_hoc.sbatch
+-rwxr-xr-x   0 runner    (1001) docker     (127)      912 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/export_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1406 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/extract.sbatch
+-rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/extract.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.703287 bluepyemodel-0.0.99/examples/L5PC/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ca_HVA.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/KdShu2007.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/NaTg2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/StochKv2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/mechanisms/StochKv3.mod
+-rw-r--r--   0 runner    (1001) docker     (127)   144199 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/monitor_optimisation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/monitor_optimisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:52:40.703287 bluepyemodel-0.0.99/examples/L5PC/morphologies/
+-rw-r--r--   0 runner    (1001) docker     (127)   604981 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/morphologies/C060114A5.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/optimisation.sbatch
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1679 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/optimisation.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/examples/L5PC/targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:52:40.703287 bluepyemodel-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-03 12:52:32.000000 bluepyemodel-0.0.99/tox.ini
```

### Comparing `bluepyemodel-0.0.98/.github/workflows/release.yml` & `bluepyemodel-0.0.99/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/.github/workflows/test.yml` & `bluepyemodel-0.0.99/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/.gitignore` & `bluepyemodel-0.0.99/.gitignore`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/.gitlab-ci.yml` & `bluepyemodel-0.0.99/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/.pylintrc` & `bluepyemodel-0.0.99/.pylintrc`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/.zenodo.json` & `bluepyemodel-0.0.99/.zenodo.json`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/CONTRIBUTING.md` & `bluepyemodel-0.0.99/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/COPYING` & `bluepyemodel-0.0.99/COPYING`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/LICENSE.txt` & `bluepyemodel-0.0.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/PKG-INFO` & `bluepyemodel-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepyemodel
-Version: 0.0.98
+Version: 0.0.99
 Summary: Blue Brain Python Electrical Modeling Pipeline
 Home-page: https://github.com/BlueBrain/BluePyEModel
 Author: Blue Brain Project, EPFL
 Author-email: 
 License: Apache-2.0
 Keywords: computational neuroscience,simulation,analysis,parameters,Blue Brain Project
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bluepyemodel-0.0.98/README.rst` & `bluepyemodel-0.0.99/README.rst`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/access_point/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/access_point/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/access_point/access_point.py` & `bluepyemodel-0.0.99/bluepyemodel/access_point/access_point.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/access_point/local.py` & `bluepyemodel-0.0.99/bluepyemodel/access_point/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,17 +690,17 @@
 
         models = []
         for mod_data in self.get_final_content().values():
             if mod_data["emodel"] in emodels:
                 models.append(self.format_emodel_data(mod_data))
 
         filtered_models = []
-        api_metadata = self.emodel_metadata.for_resource()
+        api_metadata = self.emodel_metadata.as_dict()
         for m in models:
-            model_metadata = m.emodel_metadata.for_resource()
+            model_metadata = m.emodel_metadata.as_dict()
             for f, v in api_metadata.items():
                 if f in model_metadata and v != model_metadata[f]:
                     break
             else:
                 filtered_models.append(m)
 
         return filtered_models
```

### Comparing `bluepyemodel-0.0.98/bluepyemodel/data/spike_rheobase_pA_BeaulieuLaroche2021.csv` & `bluepyemodel-0.0.99/bluepyemodel/data/spike_rheobase_pA_BeaulieuLaroche2021.csv`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/data/utils.py` & `bluepyemodel-0.0.99/bluepyemodel/data/utils.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/apwaveform.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/apwaveform.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/comb.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/comb.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/customfromfile.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/customfromfile.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/data/NoiseOU3.txt` & `bluepyemodel-0.0.99/bluepyemodel/ecode/data/NoiseOU3.txt`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/data/SubWhiteNoise.txt` & `bluepyemodel-0.0.99/bluepyemodel/ecode/data/SubWhiteNoise.txt`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/data/WhiteNoise.txt` & `bluepyemodel-0.0.99/bluepyemodel/ecode/data/WhiteNoise.txt`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/dehyperpol.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/dehyperpol.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/dendrite.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/dendrite.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/firepattern.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/firepattern.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/hyperdepol.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/hyperdepol.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/idrest.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/idrest.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/iv.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/iv.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/negcheops.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/negcheops.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/noise.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/noise.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/noiseou3.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/noiseou3.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/poscheops.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/poscheops.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/probampanmda_ems.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/probampanmda_ems.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/ramp.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/random_square_inputs.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/random_square_inputs.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/sahp.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/sahp.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/sinespec.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/sinespec.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/spikerec.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/spikerec.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/stimulus.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/stimulus.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/subwhitenoise.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/subwhitenoise.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/thresholdaddition.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/thresholdaddition.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/ecode/whitenoise.py` & `bluepyemodel-0.0.99/bluepyemodel/ecode/whitenoise.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/auto_targets.py` & `bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/efeatures_extraction.py` & `bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/efeatures_extraction.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/target.py` & `bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/target.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/targets_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/targets_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/targets_configurator.py` & `bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/targets_configurator.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/efeatures_extraction/trace_file.py` & `bluepyemodel-0.0.99/bluepyemodel/efeatures_extraction/trace_file.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_metadata.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import string
 
 
+def update_metadata_dict(metadata_dict, var, new_key):
+    """Update metadata dict with new key and variable if not None."""
+    if var is not None and var != "None":
+        metadata_dict[new_key] = var
+
+
 class EModelMetadata:
     """Contains the metadata of an emodel such as its e-model name or its brain region. These
     metadata can be understood as a unique identifier of an e-model.
 
     This class is a backend class and is not meant to be used directly by the user."""
 
     def __init__(
@@ -128,48 +134,74 @@
         if self.mtype:
             annotation_list.append(self.mtype_annotation_dict())
         if self.ttype:
             annotation_list.append(self.ttype_annotation_dict())
 
         return annotation_list
 
-    def get_metadata_dict(self):
+    def as_dict_for_resource(self):
         """Metadata as a dict, with keys consistent with nexus."""
 
-        metadata = {}
+        metadata_dict = {}
+
+        update_metadata_dict(metadata_dict, self.emodel, "eModel")
+        update_metadata_dict(metadata_dict, self.etype, "eType")
+        update_metadata_dict(metadata_dict, self.ttype, "tType")
+        update_metadata_dict(metadata_dict, self.mtype, "mType")
+        update_metadata_dict(metadata_dict, self.iteration, "iteration")
+        update_metadata_dict(metadata_dict, self.synapse_class, "synapseClass")
+        # rename species into subject and brain_region into brainLocation
+        update_metadata_dict(metadata_dict, self.species, "subject")
+        update_metadata_dict(metadata_dict, self.brain_region, "brainLocation")
+        # we do not want allen_notation in resource metadata
+
+        return metadata_dict
+
+    def as_dict_for_resource_legacy(self):
+        """Metadata as a dict, with keys consistent with legacy nexus."""
+
+        metadata_dict = {}
 
         for k, v in vars(self).items():
             # we do not want allen_notation in resource metadata
             if v and v != "None" and k != "allen_notation":
                 # rename species into subject and brain_region into brainLocation
                 if k == "species":
-                    metadata["subject"] = v
+                    metadata_dict["subject"] = v
                 elif k == "brain_region":
-                    metadata["brainLocation"] = v
+                    metadata_dict["brainLocation"] = v
                 else:
-                    metadata[k] = v
+                    metadata_dict[k] = v
 
-        return metadata
+        return metadata_dict
 
     def filters_for_resource(self):
         """Metadata used for filtering, without the annotation list"""
-        return self.get_metadata_dict()
+        return self.as_dict_for_resource()
+
+    def filters_for_resource_legacy(self):
+        """Legacy metadata used for filtering, without the annotation list"""
+        return self.as_dict_for_resource_legacy()
 
     def for_resource(self):
         """Metadata to add to a resource to register.
 
         DO NOT use for filtering. For filtering, use self.filters_for_resource() instead.
         """
 
-        metadata = self.get_metadata_dict()
+        metadata = self.as_dict_for_resource()
 
         metadata["annotation"] = self.annotation_list()
 
         return metadata
 
+    def as_dict(self):
+        """Metadata as dict."""
+        return vars(self)
+
     def as_string(self, seed=None, use_allen_notation=True):
         s = ""
 
         for k in ["emodel", "etype", "ttype", "mtype", "species", "brain_region", "iteration"]:
             v = getattr(self, k)
             if use_allen_notation and k == "brain_region" and self.allen_notation:
                 v = self.allen_notation
```

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_pipeline.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_pipeline.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_script.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_script.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_settings.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_settings.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/emodel_workflow.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/emodel_workflow.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/emodel_pipeline/plotting.py` & `bluepyemodel-0.0.99/bluepyemodel/emodel_pipeline/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/efeature_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/efeature_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/efel_feature_bpem.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/efel_feature_bpem.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/evaluation.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/evaluator.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/fitness_calculator_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/fitness_calculator_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/modifiers.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/modifiers.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/protocol_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/protocol_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/protocols.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/protocols.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/recordings.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/recordings.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/evaluation/utils.py` & `bluepyemodel-0.0.99/bluepyemodel/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/export_emodel/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/export_emodel/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/export_emodel/export_emodel.py` & `bluepyemodel-0.0.99/bluepyemodel/export_emodel/export_emodel.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/export_emodel/templates/cell_template.jinja2` & `bluepyemodel-0.0.99/bluepyemodel/export_emodel/templates/cell_template.jinja2`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/export_emodel/templates/cell_template_neurodamus.jinja2` & `bluepyemodel-0.0.99/bluepyemodel/export_emodel/templates/cell_template_neurodamus.jinja2`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/export_emodel/templates/cell_template_neurodamus_sbo.jinja2` & `bluepyemodel-0.0.99/bluepyemodel/export_emodel/templates/cell_template_neurodamus_sbo.jinja2`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/export_emodel/utils.py` & `bluepyemodel-0.0.99/bluepyemodel/export_emodel/utils.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/distribution_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/model/distribution_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/mechanism_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/model/mechanism_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/model.py` & `bluepyemodel-0.0.99/bluepyemodel/model/model.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/model_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/model/model_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/model_configurator.py` & `bluepyemodel-0.0.99/bluepyemodel/model/model_configurator.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/morphology_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/model/morphology_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/morphology_utils.py` & `bluepyemodel-0.0.99/bluepyemodel/model/morphology_utils.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/neuron_model_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/model/neuron_model_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/parameter_configuration.py` & `bluepyemodel-0.0.99/bluepyemodel/model/parameter_configuration.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/model/utils.py` & `bluepyemodel-0.0.99/bluepyemodel/model/utils.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/optimisation/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/optimisation/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/optimisation/optimisation.py` & `bluepyemodel-0.0.99/bluepyemodel/optimisation/optimisation.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tasks/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tasks/config.py` & `bluepyemodel-0.0.99/bluepyemodel/tasks/config.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tasks/emodel_creation/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/tasks/emodel_creation/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tasks/emodel_creation/optimisation.py` & `bluepyemodel-0.0.99/bluepyemodel/tasks/emodel_creation/optimisation.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tasks/luigi_custom.py` & `bluepyemodel-0.0.99/bluepyemodel/tasks/luigi_custom.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tasks/luigi_tools.py` & `bluepyemodel-0.0.99/bluepyemodel/tasks/luigi_tools.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tools/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tools/mechanisms.py` & `bluepyemodel-0.0.99/bluepyemodel/tools/mechanisms.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tools/morphology.py` & `bluepyemodel-0.0.99/bluepyemodel/tools/morphology.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tools/multiprocessing.py` & `bluepyemodel-0.0.99/bluepyemodel/tools/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tools/multiprotocols_efeatures_utils.py` & `bluepyemodel-0.0.99/bluepyemodel/tools/multiprotocols_efeatures_utils.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tools/search_pdfs.py` & `bluepyemodel-0.0.99/bluepyemodel/tools/search_pdfs.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/tools/utils.py` & `bluepyemodel-0.0.99/bluepyemodel/tools/utils.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/validation/__init__.py` & `bluepyemodel-0.0.99/bluepyemodel/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/validation/validation.py` & `bluepyemodel-0.0.99/bluepyemodel/validation/validation.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel/validation/validation_functions.py` & `bluepyemodel-0.0.99/bluepyemodel/validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/bluepyemodel.egg-info/PKG-INFO` & `bluepyemodel-0.0.99/bluepyemodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepyemodel
-Version: 0.0.98
+Version: 0.0.99
 Summary: Blue Brain Python Electrical Modeling Pipeline
 Home-page: https://github.com/BlueBrain/BluePyEModel
 Author: Blue Brain Project, EPFL
 Author-email: 
 License: Apache-2.0
 Keywords: computational neuroscience,simulation,analysis,parameters,Blue Brain Project
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bluepyemodel-0.0.98/bluepyemodel.egg-info/SOURCES.txt` & `bluepyemodel-0.0.99/bluepyemodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/doc/Makefile` & `bluepyemodel-0.0.99/doc/Makefile`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/doc/images/classes_schema.png` & `bluepyemodel-0.0.99/doc/images/classes_schema.png`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/doc/images/pipeline.png` & `bluepyemodel-0.0.99/doc/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/doc/source/conf.py` & `bluepyemodel-0.0.99/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/doc/source/logo/BluePyEModelBanner.jpg` & `bluepyemodel-0.0.99/doc/source/logo/BluePyEModelBanner.jpg`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/LICENSE.txt` & `bluepyemodel-0.0.99/examples/L5PC/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/LICENSE_CC-BY-CA-SA-4.0` & `bluepyemodel-0.0.99/examples/L5PC/LICENSE_CC-BY-CA-SA-4.0`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/README.rst` & `bluepyemodel-0.0.99/examples/L5PC/README.rst`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/analysis.sbatch` & `bluepyemodel-0.0.99/examples/L5PC/analysis.sbatch`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/analysis.sh` & `bluepyemodel-0.0.99/examples/L5PC/analysis.sh`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/config/params/pyr.json` & `bluepyemodel-0.0.99/examples/L5PC/config/params/pyr.json`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/config/recipes.json` & `bluepyemodel-0.0.99/examples/L5PC/config/recipes.json`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/create_venv.sh` & `bluepyemodel-0.0.99/examples/L5PC/create_venv.sh`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/download_ephys_data.sh` & `bluepyemodel-0.0.99/examples/L5PC/download_ephys_data.sh`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/exploit_models.ipynb` & `bluepyemodel-0.0.99/examples/L5PC/exploit_models.ipynb`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/export_hoc.sbatch` & `bluepyemodel-0.0.99/examples/L5PC/export_hoc.sbatch`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/export_hoc.sh` & `bluepyemodel-0.0.99/examples/L5PC/export_hoc.sh`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/extract.sbatch` & `bluepyemodel-0.0.99/examples/L5PC/extract.sbatch`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/extract.sh` & `bluepyemodel-0.0.99/examples/L5PC/extract.sh`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/CaDynamics_DC0.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/CaDynamics_DC0.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ca_HVA.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ca_HVA2.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ca_HVA2.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ca_LVAst.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/Ih.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/K_Pst.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/K_Tst.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/KdShu2007.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/KdShu2007.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/NaTg.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/NaTg.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/NaTg2.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/NaTg2.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/Nap_Et2.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/SK_E2.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/SKv3_1.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/StochKv2.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/StochKv2.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/mechanisms/StochKv3.mod` & `bluepyemodel-0.0.99/examples/L5PC/mechanisms/StochKv3.mod`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/monitor_optimisation.ipynb` & `bluepyemodel-0.0.99/examples/L5PC/monitor_optimisation.ipynb`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/monitor_optimisation.py` & `bluepyemodel-0.0.99/examples/L5PC/monitor_optimisation.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/morphologies/C060114A5.asc` & `bluepyemodel-0.0.99/examples/L5PC/morphologies/C060114A5.asc`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/optimisation.sbatch` & `bluepyemodel-0.0.99/examples/L5PC/optimisation.sbatch`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/optimisation.sh` & `bluepyemodel-0.0.99/examples/L5PC/optimisation.sh`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/pipeline.py` & `bluepyemodel-0.0.99/examples/L5PC/pipeline.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/examples/L5PC/targets.py` & `bluepyemodel-0.0.99/examples/L5PC/targets.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/setup.py` & `bluepyemodel-0.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyemodel-0.0.98/tox.ini` & `bluepyemodel-0.0.99/tox.ini`

 * *Files identical despite different names*

