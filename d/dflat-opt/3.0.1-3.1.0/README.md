# Comparing `tmp/dflat_opt-3.0.1.tar.gz` & `tmp/dflat_opt-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflat_opt-3.0.1.tar", last modified: Mon Apr 22 21:17:57 2024, max compression
+gzip compressed data, was "dflat_opt-3.1.0.tar", last modified: Thu May  2 01:31:32 2024, max compression
```

## Comparing `dflat_opt-3.0.1.tar` & `dflat_opt-3.1.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)       64 2024-04-22 21:17:02.000000 dflat_opt-3.0.1/MANIFEST.in
--rw-r--r--   0 deanhazineh  (1000) deanhazineh  (1000)     7593 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/PKG-INFO
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.848944 dflat_opt-3.0.1/dflat/
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.848944 dflat_opt-3.0.1/dflat/GDSII/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      108 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/GDSII/__init__.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6074 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/GDSII/assemble.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1179 2024-04-12 00:40:30.000000 dflat_opt-3.0.1/dflat/GDSII/gds_utils.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/__init__.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/initialize/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      110 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/initialize/__init__.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     5657 2024-04-19 16:57:45.000000 dflat_opt-3.0.1/dflat/initialize/interleave.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6434 2024-04-19 16:58:01.000000 dflat_opt-3.0.1/dflat/initialize/lenses.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/metasurface/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      194 2024-04-22 19:40:07.000000 dflat_opt-3.0.1/dflat/metasurface/__init__.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)    18552 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/metasurface/datasets.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1632 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/metasurface/latent.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     5005 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/metasurface/load_utils.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      689 2024-04-11 19:09:23.000000 dflat_opt-3.0.1/dflat/metasurface/nn.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     5131 2024-04-11 19:14:38.000000 dflat_opt-3.0.1/dflat/metasurface/nn_siren.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4739 2024-04-19 17:34:49.000000 dflat_opt-3.0.1/dflat/metasurface/optical_model.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4082 2024-04-20 20:41:18.000000 dflat_opt-3.0.1/dflat/metasurface/reverse_lookup.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     7963 2024-04-11 21:46:56.000000 dflat_opt-3.0.1/dflat/metasurface/trainer.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/plot_utilities/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      138 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/plot_utilities/__init__.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2600 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/plot_utilities/mp_format.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     3950 2024-04-22 21:10:31.000000 dflat_opt-3.0.1/dflat/plot_utilities/vis.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/propagation/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)       97 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/propagation/__init__.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)    38579 2024-04-22 20:56:08.000000 dflat_opt-3.0.1/dflat/propagation/propagators.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     8098 2024-04-22 21:06:05.000000 dflat_opt-3.0.1/dflat/propagation/psf.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      662 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/propagation/util.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/radial_tranforms/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      193 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/radial_tranforms/__init__.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     3993 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/radial_tranforms/hankel_ops.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     8171 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/radial_tranforms/radial_ops.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/render/
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/render/QE_Estimates/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1948 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/QE_Estimates/QE_CMOS_Pregius.csv
--rwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)    33362 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/QE_Estimates/RGB_Basler_Ace2_QE.csv
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      526 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/QE_Estimates/readme.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      182 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/render/__init__.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/render/color_space/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     3535 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/color_space/1931RGBFunctions.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4000 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/color_space/1931XYZFunctions.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     5051 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/render/fft_convolve.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2335 2024-04-11 23:14:38.000000 dflat_opt-3.0.1/dflat/render/fronto_planar_renderer.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat/render/illuminants/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     7019 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/illuminants/D65.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      167 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/illuminants/readme.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6936 2024-04-15 18:27:14.000000 dflat_opt-3.0.1/dflat/render/util_meas.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1859 2024-04-11 15:17:42.000000 dflat_opt-3.0.1/dflat/render/util_sensor.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1905 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/dflat/render/util_spectral.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/dflat_opt.egg-info/
--rw-r--r--   0 deanhazineh  (1000) deanhazineh  (1000)     7593 2024-04-22 21:17:57.000000 dflat_opt-3.0.1/dflat_opt.egg-info/PKG-INFO
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1747 2024-04-22 21:17:57.000000 dflat_opt-3.0.1/dflat_opt.egg-info/SOURCES.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)        1 2024-04-22 21:17:57.000000 dflat_opt-3.0.1/dflat_opt.egg-info/dependency_links.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      139 2024-04-22 21:17:57.000000 dflat_opt-3.0.1/dflat_opt.egg-info/requires.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)        6 2024-04-22 21:17:57.000000 dflat_opt-3.0.1/dflat_opt.egg-info/top_level.txt
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6702 2024-04-19 17:31:08.000000 dflat_opt-3.0.1/readme.md
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      754 2024-04-22 21:17:57.856944 dflat_opt-3.0.1/setup.cfg
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      173 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/setup.py
-drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-22 21:17:57.852944 dflat_opt-3.0.1/tests/
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1773 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_fourier_convolution.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1964 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_hsi_to_rgb.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4373 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_initialize.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1307 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_metasurface_datasets.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1188 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_metasurface_loader.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1622 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_metasurface_reverse_lookup.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2348 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_metasurface_util.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6997 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_propagation.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2596 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_radial_transforms.py
--rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1877 2024-04-12 01:20:35.000000 dflat_opt-3.0.1/tests/test_render.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.534774 dflat_opt-3.1.0/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)       64 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/MANIFEST.in
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     7336 2024-05-02 01:31:32.534774 dflat_opt-3.1.0/PKG-INFO
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/GDSII/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      108 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/GDSII/__init__.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6074 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/GDSII/assemble.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1179 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/GDSII/gds_utils.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/__init__.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/initialize/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      110 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/initialize/__init__.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     5657 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/initialize/interleave.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6434 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/initialize/lenses.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/metasurface/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      194 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/metasurface/__init__.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)    18552 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/metasurface/datasets.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1864 2024-04-30 16:13:04.000000 dflat_opt-3.1.0/dflat/metasurface/latent.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4990 2024-05-01 20:24:30.000000 dflat_opt-3.1.0/dflat/metasurface/load_utils.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2728 2024-05-02 00:31:52.000000 dflat_opt-3.1.0/dflat/metasurface/nn.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     3285 2024-05-02 00:31:26.000000 dflat_opt-3.1.0/dflat/metasurface/nn_siren.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4679 2024-05-02 00:32:07.000000 dflat_opt-3.1.0/dflat/metasurface/optical_model.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4145 2024-05-01 20:26:03.000000 dflat_opt-3.1.0/dflat/metasurface/reverse_lookup.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     7963 2024-05-01 20:24:46.000000 dflat_opt-3.1.0/dflat/metasurface/trainer.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/plot_utilities/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      138 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/plot_utilities/__init__.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2600 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/plot_utilities/mp_format.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     3166 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/plot_utilities/vis.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/propagation/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)       81 2024-04-30 22:39:22.000000 dflat_opt-3.1.0/dflat/propagation/__init__.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)    34275 2024-05-02 00:41:24.000000 dflat_opt-3.1.0/dflat/propagation/propagators.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)    33168 2024-05-02 00:53:29.000000 dflat_opt-3.1.0/dflat/propagation/propagators_legacy.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      662 2024-04-30 21:52:30.000000 dflat_opt-3.1.0/dflat/propagation/util.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/radial_tranforms/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      193 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/radial_tranforms/__init__.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     3993 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/radial_tranforms/hankel_ops.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     8171 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/radial_tranforms/radial_ops.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/render/
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/render/QE_Estimates/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1948 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/QE_Estimates/QE_CMOS_Pregius.csv
+-rwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)    33362 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/QE_Estimates/RGB_Basler_Ace2_QE.csv
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      526 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/QE_Estimates/readme.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      182 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/__init__.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/render/color_space/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     3535 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/color_space/1931RGBFunctions.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4000 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/color_space/1931XYZFunctions.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     5184 2024-05-02 00:46:01.000000 dflat_opt-3.1.0/dflat/render/fft_convolve.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2566 2024-05-02 00:48:02.000000 dflat_opt-3.1.0/dflat/render/fronto_planar_renderer.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat/render/illuminants/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     7019 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/illuminants/D65.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      167 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/illuminants/readme.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6936 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/util_meas.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1859 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/util_sensor.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1905 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/dflat/render/util_spectral.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.530774 dflat_opt-3.1.0/dflat_opt.egg-info/
+-rw-r--r--   0 deanhazineh  (1000) deanhazineh  (1000)     7336 2024-05-02 01:31:32.000000 dflat_opt-3.1.0/dflat_opt.egg-info/PKG-INFO
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1795 2024-05-02 01:31:32.000000 dflat_opt-3.1.0/dflat_opt.egg-info/SOURCES.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)        1 2024-05-02 01:31:32.000000 dflat_opt-3.1.0/dflat_opt.egg-info/dependency_links.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      139 2024-05-02 01:31:32.000000 dflat_opt-3.1.0/dflat_opt.egg-info/requires.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)        6 2024-05-02 01:31:32.000000 dflat_opt-3.1.0/dflat_opt.egg-info/top_level.txt
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     6839 2024-05-01 22:53:50.000000 dflat_opt-3.1.0/readme.md
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      754 2024-05-02 01:31:32.534774 dflat_opt-3.1.0/setup.cfg
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      173 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/setup.py
+drwxrwxr-x   0 deanhazineh  (1000) deanhazineh  (1000)        0 2024-05-02 01:31:32.534774 dflat_opt-3.1.0/tests/
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1773 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_fourier_convolution.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1964 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_hsi_to_rgb.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4373 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_initialize.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1307 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_metasurface_datasets.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1188 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_metasurface_loader.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1622 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_metasurface_reverse_lookup.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)      791 2024-04-30 16:23:37.000000 dflat_opt-3.1.0/tests/test_metasurface_util.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4704 2024-04-30 22:39:22.000000 dflat_opt-3.1.0/tests/test_propagation.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     4786 2024-05-02 00:55:18.000000 dflat_opt-3.1.0/tests/test_propagation_legacy.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     2596 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_radial_transforms.py
+-rw-rw-r--   0 deanhazineh  (1000) deanhazineh  (1000)     1877 2024-04-30 14:53:18.000000 dflat_opt-3.1.0/tests/test_render.py
```

### Comparing `dflat_opt-3.0.1/PKG-INFO` & `dflat_opt-3.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,17 @@
 Metadata-Version: 2.1
 Name: dflat_opt
-Version: 3.0.1
+Version: 3.1.0
 Summary: D-Flat is a forward and inverse design framework for flat optics. Although specially geared for the design of metasurfaces, it may be used broadly for end-to-end imaging and sensing task.
 Home-page: https://github.com/DeanHazineh/DFlat
 Author: Dean Hazineh
 Author-email: dhazineh@g.harvard.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: pytest
-Requires-Dist: pytest-cov
-Requires-Dist: requests
-Requires-Dist: setuptools
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: moviepy
-Requires-Dist: pyhank
-Requires-Dist: einops
-Requires-Dist: tqdm
-Requires-Dist: pandas
-Requires-Dist: opencv-python
-Requires-Dist: gdspy
-Requires-Dist: mat73
-Requires-Dist: omegaconf
-Requires-Dist: natsort
 
 <div align="center">
   <img src=/docs/DFlat_Long.png alt="Dflat" width="500"/>
 </div>
 <div align="center">
   <img src=/docs/autoGDS_metalens.png alt="Dflat" width="500"/>
 </div>
@@ -68,18 +51,19 @@
 ```
 
 ## Version Notes (v3.0.0)
 
 Updated on April 11, 2024 | V2 -> V3
 - Documentation is still in development :o 
 - (v3) You can now donwload this package from the PyPi Index!
-- (v3) Datasets and pre-trained models are now downloaded when called insetad of during install. Models are now initialized by their name instead of by paths to config files. 
+- (v3) Datasets and pre-trained models are now downloaded when called insetad of during install. Models are now initialized by their name instead of by paths to config files.
+- (v3) Memory problems? Gradient checkpointing is added throughout reducing memory when using DFLat at the cost of slightly slower runtimes. 
 - (v2) This repository is the home for the new and maintained version of DFlat. It replaces DFlat-Tensorflow.
-- (v2) Note that this package is no longer a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in February 2024.
-- (v2) The structure of the software is completely revamped and the algorithms used--in particular for field propagation--are not the same as before. The original pytorch version (now deprecated) is archived and kept as a branch.
+- (v2) Note that this package is no longer a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in February 2024. I recommend switching!
+- (v2) The structure of the software is completely revamped and the algorithms used throughout are not the same as before. The original pytorch version (now deprecated) is archived and kept as a branch.
 
 ## Usage and Documentation
 
 Detailed documentation for the rewritten package and a new project page will be released in the future. For now, we highlight two resources for developers and researchers:
 - A script used to train neural models can be found in `scripts/trainer.ipynb`. The model architecture is specified in the config.yaml file and you can play around with editing it. 
 - A simple demo of the workflow can be found at `scripts/demo.ipynb`.
```

#### html2text {}

```diff
@@ -1,19 +1,14 @@
-Metadata-Version: 2.1 Name: dflat_opt Version: 3.0.1 Summary: D-Flat is a
+Metadata-Version: 2.1 Name: dflat_opt Version: 3.1.0 Summary: D-Flat is a
 forward and inverse design framework for flat optics. Although specially geared
 for the design of metasurfaces, it may be used broadly for end-to-end imaging
 and sensing task. Home-page: https://github.com/DeanHazineh/DFlat Author: Dean
 Hazineh Author-email: dhazineh@g.harvard.edu Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Requires-Python: >=3.9
-Description-Content-Type: text/markdown Requires-Dist: pytest Requires-Dist:
-pytest-cov Requires-Dist: requests Requires-Dist: setuptools Requires-Dist:
-numpy Requires-Dist: scipy Requires-Dist: matplotlib Requires-Dist: moviepy
-Requires-Dist: pyhank Requires-Dist: einops Requires-Dist: tqdm Requires-Dist:
-pandas Requires-Dist: opencv-python Requires-Dist: gdspy Requires-Dist: mat73
-Requires-Dist: omegaconf Requires-Dist: natsort
+Description-Content-Type: text/markdown
                                     [Dflat]
                                     [Dflat]
 # An End-to-End Design Framework for Diffractive Optics and Metasurface-Based
 Vision Systems ![Python](https://img.shields.io/badge/python-3670A0?style=for-
 the-badge&logo=python&logoColor=ffdd54) ![PyTorch](https://img.shields.io/
 badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)]
@@ -43,19 +38,21 @@
 simply via: ``` pip install dflat_opt ``` You may also find it beneficial to
 work directly with the repository in editable mode via: ``` git clone https://
 github.com/DeanHazineh/DFlat pip install -e . ``` ## Version Notes (v3.0.0)
 Updated on April 11, 2024 | V2 -> V3 - Documentation is still in development :
 o - (v3) You can now donwload this package from the PyPi Index! - (v3) Datasets
 and pre-trained models are now downloaded when called insetad of during
 install. Models are now initialized by their name instead of by paths to config
-files. - (v2) This repository is the home for the new and maintained version of
-DFlat. It replaces DFlat-Tensorflow. - (v2) Note that this package is no longer
-a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in
-February 2024. - (v2) The structure of the software is completely revamped and
-the algorithms used--in particular for field propagation--are not the same as
+files. - (v3) Memory problems? Gradient checkpointing is added throughout
+reducing memory when using DFLat at the cost of slightly slower runtimes. -
+(v2) This repository is the home for the new and maintained version of DFlat.
+It replaces DFlat-Tensorflow. - (v2) Note that this package is no longer a
+direct port of pytorch-tensorflow but is a complete rewrite (re-)released in
+February 2024. I recommend switching! - (v2) The structure of the software is
+completely revamped and the algorithms used throughout are not the same as
 before. The original pytorch version (now deprecated) is archived and kept as a
 branch. ## Usage and Documentation Detailed documentation for the rewritten
 package and a new project page will be released in the future. For now, we
 highlight two resources for developers and researchers: - A script used to
 train neural models can be found in `scripts/trainer.ipynb`. The model
 architecture is specified in the config.yaml file and you can play around with
 editing it. - A simple demo of the workflow can be found at `scripts/
```

### Comparing `dflat_opt-3.0.1/dflat/GDSII/assemble.py` & `dflat_opt-3.1.0/dflat/GDSII/assemble.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/GDSII/gds_utils.py` & `dflat_opt-3.1.0/dflat/GDSII/gds_utils.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/initialize/interleave.py` & `dflat_opt-3.1.0/dflat/initialize/interleave.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/initialize/lenses.py` & `dflat_opt-3.1.0/dflat/initialize/lenses.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/metasurface/datasets.py` & `dflat_opt-3.1.0/dflat/metasurface/datasets.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/metasurface/latent.py` & `dflat_opt-3.1.0/dflat/metasurface/latent.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 import torch
 
 
-def latent_to_param(z_latent, pmin=0, pmax=1, func="tanh"):
+def latent_to_param(z_latent, pmin=0, pmax=1, func="sigmoid"):
     """Takes a latent tensor (defined on domain R[-inf, inf]) and returns the corresponding param tensor
         (defined on domain R[pmin, pmax]).
 
     Args:
-        `z_latent` (tf.float): Latent tensor
-        `pmin` (tf.float, optional): minimum param value. Defaults to 0.
-        `pmax` (tf.float, optional): maximum param value. Defaults to 1.
+        `z_latent` (float): Latent tensor
+        `pmin` (float, optional): minimum param value. Defaults to 0.
+        `pmax` (float, optional): maximum param value. Defaults to 1.
 
     Returns:
-        `tf.float`: param tensor of equivalent shape
+        `float`: param tensor of equivalent shape
 
     """
-    assert func in ["sigmoid", "tanh", "sine"]
+    assert func in ["sigmoid", "tanh"]
     z_latent = torch.tensor(z_latent) if not torch.is_tensor(z_latent) else z_latent
 
-    if func == "tanh":
-        return ((torch.tanh(z_latent) + 1) / 2 * (pmax - pmin)) + pmin
-    elif func == "sigmoid":
-        return 1 / (1 + torch.exp(-z_latent))
+    if func == "sigmoid":
+        p = 1 / (1 + torch.exp(-z_latent))
+    elif func == "tanh":
+        p = (torch.tanh(z_latent) + 1) / 2
+    else:
+        raise ValueError("Unexpected error, invalid func method encountered.")
 
+    # Allow remapping of min and max parameter bounds for subsections of libraries
+    return p * (pmax - pmin) + pmin
 
-def param_to_latent(p_param, pmin=0.0, pmax=1.0, func="tanh"):
+
+def param_to_latent(p_param, pmin=0.0, pmax=1.0, func="sigmoid", eps=1e-6):
     """Takes a param tensor (defined on domain R[pmin, pmax]) and returns the corresponding latent tensor
     (defined on domain R[-inf, inf]).
 
     Args:
-        `p_param` (tf.float): Param tensor
-        `pmin` (tf.float, optional): minimum param value. Defaults to 0.
-        `pmax` (tf.float, optional): maximum param value. Defaults to 1.
+        `p_param` (float): Param tensor
+        `pmin` (float, optional): minimum param value. Defaults to 0.
+        `pmax` (float, optional): maximum param value. Defaults to 1.
 
     Returns:
-        `tf.float`: Latent tensor of equivalent shape
+        `float`: Latent tensor of equivalent shape
     """
-    assert func in ["sigmoid", "tanh", "sine"]
-    p_param = torch.tensor(p_param) if not torch.is_tensor(p_param) else p_param
+    assert func in ["sigmoid", "tanh"]
+
+    # Avoid division by zero
+    minp = max(eps, pmin)
+    maxp = min(1 - eps, pmax)
+    p = (torch.clip(p_param, minp, maxp) - minp) / (pmax - pmin)
+
+    if func == "sigmoid":
+        z = torch.log(p / (1 - p))
+    elif func == "tanh":
+        z = torch.atanh(p * 2 - 1)
+    else:
+        raise ValueError("unexpected error, invalid func method encountered.")
 
-    if func == "tanh":
-        return torch.atanh(
-            (torch.clip(p_param, pmin, pmax) - pmin) / (pmax - pmin) * 2 - 1
-        )
-    elif func == "sigmoid":
-        return torch.log(p_param / (1 - p_param))
+    return z
```

### Comparing `dflat_opt-3.0.1/dflat/metasurface/load_utils.py` & `dflat_opt-3.1.0/dflat/metasurface/load_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,61 +12,64 @@
     "Nanocylinders_Si3N4_U300H600": "https://www.dropbox.com/scl/fi/2zv2ipx2jkncj4yndj3e2/Nanocylinders_Si3N4_U300H600.zip?rlkey=ctvejtgika2po25m25etug3x9&dl=1",
     "Nanocylinders_Si3N4_U350H600": "https://www.dropbox.com/scl/fi/524ax6e8undt9qoahlo65/Nanocylinders_Si3N4_U350H600.zip?rlkey=cd413i3cncplfddnmhxrciybl&dl=1",
     "Nanocylinders_TiO2_U200H600": "https://www.dropbox.com/scl/fi/nl9fhmfmsz41dilth6uis/Nanocylinders_TiO2_U200H600.zip?rlkey=i5xol70u0wq7k19q3dsmyuz3a&dl=1",
     "Nanocylinders_TiO2_U250H600": "https://www.dropbox.com/scl/fi/n5coocd6bcbdrl88jaler/Nanocylinders_TiO2_U250H600.zip?rlkey=am9vad3ssskoc7bntqdxy0ts2&dl=1",
     "Nanocylinders_TiO2_U300H600": "https://www.dropbox.com/scl/fi/sn44f2xzadcrag0jgzdsq/Nanocylinders_TiO2_U300H600.zip?rlkey=5hivknv8cvfy3gzzsyolb8bz5&dl=1",
     "Nanocylinders_TiO2_U350H600": "https://www.dropbox.com/scl/fi/43mf1xidor3mti9dv8bce/Nanocylinders_TiO2_U350H600.zip?rlkey=cyj6xb3reh5iv2rj9l1byxk27&dl=1",
     "Nanoellipse_TiO2_U350H600": "https://www.dropbox.com/scl/fi/6phh6a0kztbccy76vzwjd/Nanoellipse_TiO2_U350H600.zip?rlkey=0hn8cr2kgs3t9134kmrhf1ogx&dl=1",
-    "Nanofins_TiO2_U350H600": "https://www.dropbox.com/scl/fi/co65yfwugkvugi7r8bqaj/Nanofins_TiO2_U350H600.zip?rlkey=8e0pzvzul8xlzl9szf15lbrzx&dl=1"
-    }
+    "Nanofins_TiO2_U350H600": "https://www.dropbox.com/scl/fi/co65yfwugkvugi7r8bqaj/Nanofins_TiO2_U350H600.zip?rlkey=8e0pzvzul8xlzl9szf15lbrzx&dl=1",
+}
+
 
 def model_config_path(model_name):
     dir_path = Path("DFlat/Models/")
     dir_path.mkdir(parents=True, exist_ok=True)
 
     config_exists = os.path.exists(os.path.join(dir_path, model_name, "config.yaml"))
     if not config_exists:
         print("Downloading the model from online storage.")
-        zip_path = dir_path / "data.zip"  
+        zip_path = dir_path / "data.zip"
         load_url = req_paths[model_name]
 
         with requests.get(load_url, stream=True) as response:
             response.raise_for_status()
-            with open(zip_path, 'wb') as file:
-                for chunk in response.iter_content(chunk_size=8192): 
+            with open(zip_path, "wb") as file:
+                for chunk in response.iter_content(chunk_size=8192):
                     file.write(chunk)
 
-        with zipfile.ZipFile(zip_path, 'r') as zip_ref:
+        with zipfile.ZipFile(zip_path, "r") as zip_ref:
             zip_ref.extractall(dir_path)
-        
+
         zip_path.unlink()
 
     config_path = os.path.join(dir_path, model_name, "config.yaml")
     ckpt_path = os.path.join("DFlat/Models/", model_name, "model.ckpt")
     if not os.path.exists(ckpt_path):
         ckpt_path = None
 
     return config_path, ckpt_path
 
+
 def load_optical_model(model_name):
     """Loads a neural optical model.
 
     Args:
         model_name (str): Name of the model from path "./DFlat/Models/NAME" or if not present, downloads the pre-trained model from online.
 
     Returns:
         nn.Module: Model with pretrained weights loaded if ckpt_path is specified.
     """
 
     config_path, ckpt_path = model_config_path(model_name)
     config = OmegaConf.load(config_path)
-    
+
     optical_model = instantiate_from_config(config.model, ckpt_path, strict=True)
     return optical_model
 
+
 def instantiate_from_config(config_model, ckpt_path=None, strict=False):
     assert "target" in config_model, "Expected key `target` to instantiate."
     target_str = config_model["target"]
     print(f"Target Module: {target_str}")
     loaded_module = get_obj_from_str(target_str)(**config_model.get("params", dict()))
 
     if ckpt_path is not None and ckpt_path != "None":
@@ -78,14 +81,15 @@
         missing, unexpected = loaded_module.load_state_dict(sd, strict=strict)
         print(
             f"Restored {target_str} with {len(missing)} missing and {len(unexpected)} unexpected keys"
         )
 
     return loaded_module
 
+
 def get_obj_from_str(string, reload=False):
     module, cls = string.rsplit(".", 1)
     if reload:
         module_imp = importlib.import_module(module)
         importlib.reload(module_imp)
 
     return getattr(importlib.import_module(module, package=None), cls)
@@ -111,8 +115,7 @@
     trainer = get_obj_from_str(config_trainer["target"])(
         config_model,
         ckpt_path,
         dataset,
         **config_trainer.get("params", dict()),
     )
     return trainer
-
```

### Comparing `dflat_opt-3.0.1/dflat/metasurface/optical_model.py` & `dflat_opt-3.1.0/dflat/metasurface/optical_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 import numpy as np
 
 from .load_utils import instantiate_from_config
 from .load_utils import get_obj_from_str
 
 
 class NeuralCells(nn.Module):
-    def __init__(self, nn_config, param_bounds, trainable_model=False):
+    def __init__(self, nn_config, param_bounds, use_checkpoint=True, **kwargs):
         """Initializes a neural cell model from a config dictionary.
 
         Args:
             nn_config (dict): config dictionary
             param_bounds (list): List of min and max bounds for each design parameter (in units of m). The last nested list must correspond to wavelength.
             trainable_model (bool, optional): Flag to set model parameters to trainable (requires grad). Defaults to False.
         """
         super().__init__()
+
+        if "trainable_model" in kwargs:
+            print(
+                "Note: trainable_model key in NeuralCells is deprecated. Model will be set to requires_grad."
+            )
         self.dim_in = nn_config.params.dim_in
         self.dim_out = nn_config.params.dim_out
-        self.model = self._initialize_model(nn_config, trainable_model)
+        self.model = instantiate_from_config(
+            nn_config, ckpt_path=nn_config["ckpt_path"], strict=False
+        )
         self.param_bounds = param_bounds
         self.loss = get_obj_from_str(nn_config.loss)()
+        self.use_checkpoint = use_checkpoint
 
     def training_step(self, x, y):
         pred = self.model(x)
         return self.loss(pred, y)
 
     def forward(self, params, wavelength, pre_normalized=True):
         """Predict the cell optical response from the passed in design parameters and wavelength
@@ -109,23 +117,11 @@
         out = (
             torch.stack(out, dim=-1)
             if torch.is_tensor(params)
             else np.stack(out, axis=-1)
         )
         return out
 
-    def _initialize_model(self, config, trainable_model):
-        model = instantiate_from_config(
-            config, ckpt_path=config["ckpt_path"], strict=False
-        )
-
-        if not trainable_model:
-            model = model.eval()
-            for param in model.parameters():
-                param.requires_grad = False
-
-        return model
-
 
 class NeuralFields(nn.Module):
     def __init__(self, nn_config, trainable_model=False):
         pass
```

### Comparing `dflat_opt-3.0.1/dflat/metasurface/reverse_lookup.py` & `dflat_opt-3.1.0/dflat/metasurface/reverse_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     phase,
     wavelength_set_m,
     model_name,
     lr=1e-1,
     err_thresh=1e-2,
     max_iter=1000,
     opt_phase_only=False,
-    force_cpu=False
+    force_cpu=False,
 ):
     """Given a stack of wavelength dependent amplitude and phase profiles, runs a reverse optimization to identify the nanostructures that
     implements the desired profile across wavelength by minimizing the mean absolute errors of complex fields.
 
     Args:
         amp (float): Target amplitude of shape [B, Pol, Lam, H, W].
         phase (float): Target phase of shape [B, Pol, Lam, H, W].
@@ -35,21 +35,20 @@
     B, P, L, H, W = amp.shape
     assert amp.shape == phase.shape
     assert (
         len(wavelength_set_m) == L
     ), "Wavelength list should match amp,phase wavelength dim (dim3)."
 
     if force_cpu:
-        device='cpu'
+        device = "cpu"
     else:
         device = "cuda" if torch.cuda.is_available() else "cpu"
-    
+
     print(f"Running optimization with device {device}")
     model = load_optical_model(model_name).to(device)
-
     pg = model.dim_out // 3
     assert pg == P, f"Polarization dimension of amp, phase (dim1) expected to be {pg}."
 
     # z = np.random.rand(B, H, W, model.dim_in - 1)
     z = np.zeros((B, H, W, model.dim_in - 1))
     z = torch.tensor(z, device=device, dtype=torch.float32, requires_grad=True)
     wavelength = (
@@ -57,19 +56,27 @@
         if not torch.is_tensor(wavelength_set_m)
         else wavelength_set_m
     )
     wavelength = wavelength.to(dtype=torch.float32, device=device)
     wavelength = model.normalize_wavelength(wavelength)
 
     # optimize
-    optimizer = optim.Adam([z], lr=lr)
+    optimizer = optim.AdamW([z], lr=lr)
     torch_zero = torch.tensor(0.0, dtype=z.dtype, device=device)
 
-    amp = torch.tensor(amp, dtype=torch.float32, device=device) if not torch.is_tensor(amp) else amp.to(dtype=torch.float32, device=device)
-    phase = torch.tensor(phase, dtype=torch.float32, device=device) if not torch.is_tensor(phase) else phase.to(dtype=torch.float32, device=device)
+    amp = (
+        torch.tensor(amp, dtype=torch.float32, device=device)
+        if not torch.is_tensor(amp)
+        else amp.to(dtype=torch.float32, device=device)
+    )
+    phase = (
+        torch.tensor(phase, dtype=torch.float32, device=device)
+        if not torch.is_tensor(phase)
+        else phase.to(dtype=torch.float32, device=device)
+    )
     target_field = torch.complex(amp, torch_zero) * torch.exp(
         torch.complex(torch_zero, phase)
     )
 
     err = 1e3
     steps = 0
     err_list = []
```

### Comparing `dflat_opt-3.0.1/dflat/metasurface/trainer.py` & `dflat_opt-3.1.0/dflat/metasurface/trainer.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/plot_utilities/mp_format.py` & `dflat_opt-3.1.0/dflat/plot_utilities/mp_format.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/plot_utilities/vis.py` & `dflat_opt-3.1.0/dflat/plot_utilities/vis.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,45 +60,14 @@
         append_images=images[1:],
         duration=duration,
         loop=loop,
     )
     return
 
 
-def gif_from_saved_images(
-    filepath, filetag, savename, fps, deleteFrames=True, verbose=False, loop=0
-):
-    print("Call GIF generator")
-    images = []
-    png_files = natsorted(
-        [
-            f
-            for f in os.listdir(filepath)
-            if f.startswith(filetag) and f.endswith(".png")
-        ]
-    )
-    for file in png_files:
-        file_path = os.path.join(filepath, file)
-        images.append(Image.open(file_path))
-        if verbose:
-            print("Write image file as frame: " + file)
-        if deleteFrames:
-            os.remove(file_path)
-
-    duration = int(1000 / fps)
-    images[0].save(
-        filepath + savename,
-        save_all=True,
-        append_images=images[1:],
-        duration=duration,
-        loop=loop,
-    )
-    return
-
-
 def plot_3d_stack(img, rgb, zoom, save_to, show=True, view=[12, 12], crop_dim=None):
     img = np.clip(np.flipud(img), 0, 1)
     rgb = np.clip(np.flipud(rgb), 0, 1)
     fig = plt.figure(figsize=(5, 5))
     ax = fig.add_subplot(111, projection="3d")
 
     H, W, C = img.shape
```

### Comparing `dflat_opt-3.0.1/dflat/propagation/propagators.py` & `dflat_opt-3.1.0/dflat/propagation/propagators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import torch
 import numpy as np
 import torch.nn as nn
 import torch.nn.functional as F
+from torch.utils.checkpoint import checkpoint
 from torch.fft import fftshift, ifftshift, fft2, ifft2
+from einops import rearrange
+
 from .util import cart_grid
 from dflat.radial_tranforms import (
     qdht,
     iqdht,
     general_interp_regular_1d_grid,
     radial_2d_transform,
     radial_2d_transform_wrapped_phase,
@@ -18,33 +21,38 @@
     def __init__(
         self,
         in_size,
         in_dx_m,
         out_distance_m,
         out_size,
         out_dx_m,
+        wavelength_set_m,
         out_resample_dx_m,
         manual_upsample_factor,
         radial_symmetry,
     ):
         super().__init__()
         # Quick checks on the inputs
         out_resample_dx_m = out_dx_m if out_resample_dx_m is None else out_resample_dx_m
-        assert isinstance(radial_symmetry, bool)
-        assert manual_upsample_factor >= 1
-        assert isinstance(out_distance_m, float)
+        assert isinstance(radial_symmetry, bool), "radial symmetry must be boolean."
+        assert manual_upsample_factor >= 1, "manual_upsample factor must >= 1."
+        assert isinstance(out_distance_m, float), "out_distance_m must be float."
+        assert isinstance(
+            wavelength_set_m, (list, np.ndarray)
+        ), "wavelength_set_m must be a list or numpy array."
         for obj in [in_size, in_dx_m, out_size, out_dx_m, out_resample_dx_m]:
-            assert len(obj) == 2
+            assert len(obj) == 2, "Expected len 2 list for inputs."
 
         # Move to attributes and convert lists to numpy arrays
         self.in_size = np.array(in_size).astype(int)
         self.in_dx_m = np.array(in_dx_m)
         self.out_distance_m = out_distance_m
         self.out_size = np.array(out_size).astype(int)
         self.out_dx_m = np.array(out_dx_m)
+        self.wavelength_set_m = np.array(wavelength_set_m)
         self.out_resample_dx_m = np.array(out_resample_dx_m)
         self.manual_upsample_factor = manual_upsample_factor
         self.radial_symmetry = radial_symmetry
 
         # Run additional assertions required for calculations
         self._validate_inputs()
 
@@ -73,59 +81,365 @@
 
     def _unit_conversion(self):
         convert_keys = [
             "in_dx_m",
             "out_distance_m",
             "out_dx_m",
             "out_resample_dx_m",
+            "wavelength_set_m",
         ]
         for key in convert_keys:
             obj = self.__dict__[key]
             new_name = key[:-2]
 
             if isinstance(obj, float) or isinstance(obj, np.ndarray):
                 setattr(self, new_name, obj * self.rescale)
             elif obj is None:
                 setattr(self, new_name, None)
             else:
                 raise ValueError("In key conversion, ran into unknown datatype")
 
 
+class FresnelPropagation(BaseFrequencySpace):
+    def __init__(
+        self,
+        in_size,
+        in_dx_m,
+        out_distance_m,
+        out_size,
+        out_dx_m,
+        wavelength_set_m,
+        out_resample_dx_m=None,
+        manual_upsample_factor=1,
+        radial_symmetry=False,
+        verbose=False,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(
+            in_size,
+            in_dx_m,
+            out_distance_m,
+            out_size,
+            out_dx_m,
+            wavelength_set_m,
+            out_resample_dx_m,
+            manual_upsample_factor,
+            radial_symmetry,
+        )
+        self.verbose = verbose
+        self._init_calc_params()
+        self._init_fresnel_constants()
+
+    def _init_calc_params(self):
+        # Determine a manual_upsample_factor as a forced use to avoid field cropping
+        factor = self.out_dx * self.out_size * self.in_dx / self.out_distance
+        upsample_factors = factor[:, None] / self.wavelength_set[None, :]
+        manual_upsample = np.array(
+            [self.manual_upsample_factor, self.manual_upsample_factor]
+        )
+        upsample_factors = np.maximum(upsample_factors, manual_upsample[:, None]).T
+
+        # Compute the input grid and upsampled size when we upsample the input field
+        calc_in_dx = self.in_dx / upsample_factors
+        in_length = self.in_dx * self.in_size
+        calc_samplesM = np.rint(in_length / calc_in_dx)
+        calc_samplesM = np.where(
+            np.mod(calc_samplesM, 2) == 0, calc_samplesM + 1, calc_samplesM
+        )
+
+        self.calc_samplesM = calc_samplesM
+        self.calc_samplesM_r = calc_samplesM[-1] // 2
+        self.manual_upsample_factor = upsample_factors
+
+        # Update the calculation grid corresponding to the upsampled integer number of samples
+        self.calc_in_dx = in_length / calc_samplesM
+
+        # Determine zero-padding required to hit an output target discretization
+        estN = np.ceil(
+            self.wavelength_set[:, None]
+            * self.out_distance
+            / self.out_dx[None, :]
+            / self.calc_in_dx
+        )
+
+        estN = np.where(np.mod(estN, 2) == 0, estN + 1, estN)
+        estN = np.where(estN < self.calc_samplesM, self.calc_samplesM, estN)
+
+        pad_in = (estN - self.calc_samplesM) / 2
+        self.pad_in = pad_in.astype(int)
+
+        # Define the resulting output grid. For all wavelengths, the output value should be very close or much smaller
+        self.calc_samplesN = estN
+        self.calc_out_dx = (
+            self.wavelength_set[:, None] * self.out_distance / self.calc_in_dx / estN
+        )
+
+        if self.verbose == True:
+            print("Initializing the Fresnel Method: ")
+            print(f"   - in_size: {self.in_size}, calc_in_size:")
+            for i in range(len(self.wavelength_set)):
+                print(f"      {calc_samplesM[i,:]},")
+
+            print(f"   - padded_calc_in_size: ")
+            for i in range(len(self.wavelength_set)):
+                print(f"      {self.calc_samplesN[i,:]},")
+
+            print(f"   - in_dx: {self.in_dx}, calc_in_dx: ")
+            for i in range(len(self.wavelength_set)):
+                print(f"      {calc_in_dx[i,:]},")
+
+            print(f"   - out_dx: {self.out_dx}, calc_out_dx: ")
+            for i in range(len(self.wavelength_set)):
+                print(f"      {self.calc_out_dx[i,:]},")
+
+    def _init_fresnel_constants(self):
+        # Save compute time be pre-initializing tensors for the fresnel calculation
+        self.quad_term_in = []
+        self.ang_fx = []
+        self.x = []
+        self.out_phase = []
+        self.norm = []
+        for i, lam in enumerate(self.wavelength_set):
+            x, y = cart_grid(
+                self.calc_samplesN[i], self.calc_in_dx[i], self.radial_symmetry
+            )
+            self.x.append(x)
+
+            quadratic_term = np.pi / lam / self.out_distance * (x**2 + y**2)
+            self.quad_term_in.append(quadratic_term)
+
+            if self.radial_symmetry:
+                fx = torch.arange(
+                    0,
+                    1 / 2 / self.calc_in_dx[i, -1],
+                    1 / self.calc_in_dx[i, -1] / self.calc_samplesN[i, -1],
+                )
+                self.ang_fx.append(fx)
+                norm = torch.tensor(
+                    1.0
+                    / np.sqrt(
+                        np.prod(self.calc_in_dx[i])
+                        * np.prod(self.calc_out_dx[i])
+                        * np.prod(self.calc_samplesN[i])
+                    )
+                )
+            else:
+                norm = torch.tensor(
+                    np.sqrt(
+                        np.prod(self.calc_in_dx[i])
+                        / np.prod(self.calc_out_dx[i])
+                        / np.prod(self.calc_samplesN[i])
+                    )
+                )
+            self.norm.append(norm)
+
+            xo, yo = cart_grid(
+                self.calc_samplesN[i], self.calc_out_dx[i], self.radial_symmetry
+            )
+            out_phase = (
+                2
+                * np.pi
+                / lam
+                * (self.out_distance + (xo**2 + yo**2) / 2 / self.out_distance)
+            )
+            self.out_phase.append(out_phase)
+
+        self.calc_in_dx = torch.tensor(self.calc_in_dx)
+        self.calc_out_dx = torch.tensor(self.calc_out_dx)
+        self.calc_samplesN = torch.tensor(self.calc_samplesN)
+        self.torch_zero = torch.tensor(0.0)
+        return
+
+    def forward(self, amplitude, phase, **kwargs):
+        """Propagates a complex field from an input plane to a planar output plane a distance out_distance_m.
+
+        Args:
+            amplitude (float): Field amplitude of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
+            phase (float): Field phase of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
+        """
+        if "wavelength_set_m" in kwargs:
+            raise ValueError(
+                "The 'wavelength_set_m' is not expected in this model. "
+                "Please use the propagator from dflat.propagation.propagators_legacy class that accepts wavelength as a forward input."
+            )
+
+        assert amplitude.shape == phase.shape, "amplitude and phase must be same shape."
+        assert (
+            len(self.wavelength_set) == amplitude.shape[-3] or amplitude.shape[-3] == 1
+        ), "Wavelength dimensions don't match"
+        if self.radial_symmetry:
+            assert amplitude.shape[-2] == 1, "Radial flag requires 1D input not 2D."
+            assert amplitude.shape[-1] == self.in_size[-1] // 2 + 1
+        else:
+            assert all(
+                amplitude.shape[-2:] == self.in_size
+            ), f"Input field size does not match init in_size {self.in_size}."
+
+        device = "cuda" if torch.cuda.is_available() else "cpu"
+        amplitude = (
+            torch.tensor(amplitude, dtype=torch.float32).to(device)
+            if not torch.is_tensor(amplitude)
+            else amplitude.to(dtype=torch.float32)
+        )
+        phase = (
+            torch.tensor(phase, dtype=torch.float32).to(device)
+            if not torch.is_tensor(phase)
+            else phase.to(dtype=torch.float32)
+        )
+
+        return checkpoint(self._forward, amplitude, phase, **kwargs)
+
+    def _forward(self, amplitude, phase, **kwargs):
+        # Upsample and pad the field prior to fourier-based propagation transformation
+        amplitude, phase = self._regularize_field(amplitude, phase)
+
+        # propagate by the fresnel method
+        amplitude, phase = self.fresnel_transform(amplitude, phase)
+
+        # Transform field back to the specified output grid
+        amplitude, phase = self._resample_field(amplitude, phase)
+
+        # Convert to 2D and return to final sensor size
+        for i, (amp, ph) in enumerate(zip(amplitude, phase)):
+            if self.radial_symmetry:
+                amp = radial_2d_transform(amp.squeeze(-2))
+                ph = radial_2d_transform_wrapped_phase(ph.squeeze(-2))
+
+            phase[i] = resize_with_crop_or_pad(ph, *self.out_size, False)
+            amplitude[i] = resize_with_crop_or_pad(amp, *self.out_size, False)
+
+        amplitude = torch.cat(amplitude, axis=-3)
+        phase = torch.cat(phase, axis=-3)
+
+        return amplitude, phase
+
+    def fresnel_transform(self, amplitude, phase):
+        radial_symmetry = self.radial_symmetry
+        dtype = amplitude[0].dtype
+        device = amplitude[0].device
+        torch_zero = self.torch_zero.to(dtype=dtype, device=device)
+
+        for i, lam in enumerate(self.wavelength_set):
+            in_quad_term = self.quad_term_in[i].to(dtype=dtype, device=device)
+            transform_term = torch.complex(amplitude[i], torch_zero) * torch.exp(
+                torch.complex(torch_zero, phase[i] + in_quad_term)
+            )
+
+            if radial_symmetry:
+                fx = self.ang_fx[i].to(dtype=dtype, device=device)
+                x = torch.squeeze(self.x[i].to(dtype=dtype, device=device))
+                norm = self.norm[i].to(dtype=dtype, device=device)
+                norm = torch.complex(norm, torch_zero)
+                kr, wavefront = qdht(x, transform_term)
+                wavefront = (
+                    general_interp_regular_1d_grid(kr / 2 / np.pi, fx, wavefront) * norm
+                )
+            else:
+                norm = self.norm[i].to(dtype=dtype, device=device)
+                norm = torch.complex(norm, torch_zero)
+                wavefront = fftshift(fft2(ifftshift(transform_term))) * norm
+
+            # add the complex phase term on the output
+            phase_add = self.out_phase[i].to(dtype=dtype, device=device)
+            amplitude[i] = torch.abs(wavefront)
+            phase[i] = torch.angle(
+                wavefront * torch.exp(torch.complex(torch_zero, phase_add))
+            )
+
+        return amplitude, phase
+
+    def _regularize_field(self, amplitude, phase):
+        # Natural broadcasting of the wavelength dimension cannot be done for Fresnel case
+        if amplitude.shape[-3] == 1:
+            amplitude = amplitude.repeat(1, len(self.wavelength_set), 1, 1)
+            phase = phase.repeat(1, len(self.wavelength_set), 1, 1)
+
+        method = "nearest-exact"
+        samplesM = self.calc_samplesM
+        radial_symmetry = self.radial_symmetry
+
+        ampl_list = []
+        phase_list = []
+        for i, _ in enumerate(self.wavelength_set):
+            # Resample the input field via nearest neighbors interpolation
+            # Nearest matches openCV's implementation but torch recommends using nearest-exact
+            resize_to = (
+                np.array([1, samplesM[i, 1] // 2 + 1])
+                if radial_symmetry
+                else samplesM[i]
+            )
+            resize_to = tuple([int(_) for _ in resize_to])
+            ampl = F.interpolate(amplitude[:, i : i + 1], size=resize_to, mode=method)
+            ph = F.interpolate(phase[:, i : i + 1], size=resize_to, mode=method)
+
+            # Add padding -- this changes the output grid dx so we need to pad per wavelength
+            # Thus what follows will be a jagged tensor (for now a list)
+            padi = self.pad_in[i]
+            paddings = (
+                [0, padi[1], 0, 0, 0, 0, 0, 0]
+                if radial_symmetry
+                else [padi[1], padi[1], padi[0], padi[0], 0, 0, 0, 0]
+            )
+            ampl_list.append(F.pad(ampl, paddings, mode="constant", value=0))
+            phase_list.append(F.pad(ph, paddings, mode="constant", value=0))
+
+        return ampl_list, phase_list
+
+    def _resample_field(self, amplitude, phase):
+        nl = len(amplitude)
+        for i in range(nl):
+            scale = tuple(self.calc_out_dx[i] / self.out_resample_dx)
+            if self.radial_symmetry:
+                scale = (1, scale[-1])
+
+            phase[i] = torch.atan2(
+                F.interpolate(torch.sin(phase[i]), scale_factor=scale, mode="area"),
+                F.interpolate(torch.cos(phase[i]), scale_factor=scale, mode="area"),
+            )
+            amplitude[i] = F.interpolate(amplitude[i], scale_factor=scale, mode="area")
+
+        return amplitude, phase
+
+
 class ASMPropagation(BaseFrequencySpace):
     def __init__(
         self,
         in_size,
         in_dx_m,
         out_distance_m,
         out_size,
         out_dx_m,
+        wavelength_set_m,
         out_resample_dx_m=None,
         manual_upsample_factor=1,
         radial_symmetry=False,
         FFTPadFactor=1.0,
+        verbose=False,
     ):
         super().__init__(
             in_size,
             in_dx_m,
             out_distance_m,
             out_size,
             out_dx_m,
+            wavelength_set_m,
             out_resample_dx_m,
             manual_upsample_factor,
             radial_symmetry,
         )
+        self.verbose = verbose
         self._init_calc_params()
         self.FFTPadFactor = FFTPadFactor
 
     def _init_calc_params(self):
-        in_dx = self.in_dx
-        out_dx = self.out_dx
-
         # calc_in_dx should be smaller than the out_dx requested by the user.
         # This is because the output sampling grid will match input
+        in_dx = self.in_dx
+        out_dx = self.out_dx
         calc_in_dx = in_dx / self.manual_upsample_factor
         calc_in_dx = np.where(calc_in_dx < out_dx, calc_in_dx, out_dx)
 
         # Given the new calculation grid size, we should change the number of samples (odd) taken
         # at the input grid so that the originally data is correctly represented.
         in_length = in_dx * self.in_size
         calc_samplesM = np.rint(in_length / calc_in_dx)
@@ -133,17 +447,16 @@
             np.mod(calc_samplesM, 2) == 0, calc_samplesM + 1, calc_samplesM
         )
         calc_samplesM_r = calc_samplesM[-1] // 2
         self.calc_samplesM = calc_samplesM
         self.calc_samplesM_r = calc_samplesM_r
 
         # Update the calculation grid corresponding to the upsampled integer number of samples
-        self.calc_in_dx = in_length / calc_samplesM
-
         # For ASM, the output grid size is the same as the input so update this quantity
+        self.calc_in_dx = in_length / calc_samplesM
         self.calc_out_dx = self.calc_in_dx
 
         # For the ASM case, we already checked that the in grid dx is smaller or equal to the sensor grid dx
         # Now we should pad to ensure that out fields are calculated on the entire sensing space requested by user
         desired_span = self.out_size * self.out_resample_dx
         current_span = self.calc_out_dx * calc_samplesM
         pad_in = np.rint(
@@ -156,25 +469,39 @@
 
         calc_samplesN = 2 * pad_in + calc_samplesM
         calc_samplesN_r = calc_samplesN[-1] // 2 + 1
         self.calc_samplesN = calc_samplesN
         self.calc_samplesN_r = calc_samplesN_r
         self.pad_in = pad_in
 
-    def forward(self, amplitude, phase, wavelength_set_m):
+        if self.verbose:
+            print("Initializing the Angular Spectrum Method")
+            print(
+                f"   - in_size: {self.in_size}, calc_in_size: {self.calc_samplesM}, padded_calc_in_size: {self.calc_samplesN}"
+            )
+            print(f"   - in_dx: {self.in_dx}, calc_in_dx: {self.calc_in_dx}")
+            print(f"   - out_dx: {self.out_dx}, calc_out_dx: {self.calc_out_dx}")
+            print(f"   - Resampling to grid size: {self.out_resample_dx}")
+
+    def forward(self, amplitude, phase, **kwargs):
         """Propagates a complex field from an input plane to a planar output plane a distance out_distance_m.
 
         Args:
             amplitude (float): Field amplitude of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
             phase (float): Field phase of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
         """
+        if "wavelength_set_m" in kwargs:
+            raise ValueError(
+                "The 'wavelength_set_m' is not expected in this model. "
+                "Please use the propagator from dflat.propagation.propagators_legacy class that accepts wavelength as a forward input."
+            )
 
         assert amplitude.shape == phase.shape, "amplitude and phase must be same shape."
         assert (
-            len(wavelength_set_m) == amplitude.shape[-3] or amplitude.shape[-3] == 1
+            len(self.wavelength_set) == amplitude.shape[-3] or amplitude.shape[-3] == 1
         ), "Wavelength dimensions don't match"
         if self.radial_symmetry:
             assert amplitude.shape[-2] == 1, "Radial flag requires 1D input not 2D."
             assert amplitude.shape[-1] == self.in_size[-1] // 2 + 1
         else:
             assert all(
                 amplitude.shape[-2:] == self.in_size
@@ -187,46 +514,43 @@
             else amplitude.to(dtype=torch.float32)
         )
         phase = (
             torch.tensor(phase, dtype=torch.float32).to(device)
             if not torch.is_tensor(phase)
             else phase.to(dtype=torch.float32)
         )
-        wavelength_set = (
-            torch.tensor(
-                np.array(wavelength_set_m) * self.rescale, dtype=amplitude.dtype
-            ).to(amplitude.device)
-            if not torch.is_tensor(wavelength_set_m)
-            else wavelength_set_m.to(dtype=amplitude.dtype)
-        )
 
+        return checkpoint(self._forward, amplitude, phase, **kwargs)
+
+    def _forward(self, amplitude, phase, **kwargs):
         # Upsample and pad the field prior to fft-based propagation transformation
         amplitude, phase = self._regularize_field(amplitude, phase)
 
         # propagate by the asm method
-        amplitude, phase = self.ASM_transform(amplitude, phase, wavelength_set)
+        amplitude, phase = self.ASM_transform(amplitude, phase)
 
         # Transform field back to the specified output grid and convert to 2D
         amplitude, phase = self._resample_field(amplitude, phase)
         if self.radial_symmetry:
             amplitude = radial_2d_transform(amplitude.squeeze(-2))
             phase = radial_2d_transform_wrapped_phase(phase.squeeze(-2))
 
         # Crop or pad with zeros to the final sensor size
         phase = resize_with_crop_or_pad(phase, *self.out_size, False)
         amplitude = resize_with_crop_or_pad(amplitude, *self.out_size, False)
 
         return amplitude, phase
 
-    def ASM_transform(self, amplitude, phase, wavelength_set):
+    def ASM_transform(self, amplitude, phase):
         init_shape = amplitude.shape
         dtype = amplitude.dtype
         device = amplitude.device
         torch_zero = torch.tensor([0.0], dtype=dtype).to(device)
         FFTPadFactor = self.FFTPadFactor
+        wavelength_set = torch.tensor(self.wavelength_set, dtype=dtype, device=device)
 
         # Optionally zero pad the input before conducting a fourier transform
         padhalf = [int(n * self.FFTPadFactor) for n in init_shape[-2:]]
         paddings = (
             (0, padhalf[1], 0, 0, 0, 0, 0, 0)
             if self.radial_symmetry
             else (padhalf[1], padhalf[1], padhalf[0], padhalf[0], 0, 0, 0, 0)
@@ -276,15 +600,14 @@
         outputwavefront = resize_with_crop_or_pad(
             outputwavefront, *init_shape[-2:], self.radial_symmetry
         )
 
         return torch.abs(outputwavefront), torch.angle(outputwavefront)
 
     def _resample_field(self, amplitude, phase):
-        # Reinterpolate the phase with area averaging and the amplitude with area sum
         scale = tuple(self.calc_out_dx / self.out_resample_dx)
         if self.radial_symmetry:
             scale = (1, scale[-1])
 
         phase = torch.atan2(
             F.interpolate(torch.sin(phase), scale_factor=scale, mode="area"),
             F.interpolate(torch.cos(phase), scale_factor=scale, mode="area"),
@@ -313,653 +636,224 @@
         )
         amplitude = F.pad(amplitude, paddings, mode="constant", value=0)
         phase = F.pad(phase, paddings, mode="constant", value=0)
 
         return amplitude, phase
 
 
-# Note that the best way to do this would be to compute an upsample factor for each wavelength but
-# this substantially increases the codes complexity and in most use cases it is not needed. We will for
-# now just let users manually define a suitable upsample amount for all cases if they are in the regime
-# where this matters.
-class FresnelPropagation(BaseFrequencySpace):
+class PointSpreadFunction(nn.Module):
     def __init__(
         self,
         in_size,
         in_dx_m,
         out_distance_m,
         out_size,
         out_dx_m,
+        wavelength_set_m,
         out_resample_dx_m=None,
         manual_upsample_factor=1,
         radial_symmetry=False,
-        *args,
-        **kwargs,
+        diffraction_engine="ASM",
+        verbose=False,
     ):
-        super().__init__(
+        super().__init__()
+
+        assert isinstance(
+            diffraction_engine, str
+        ), "diffraction engine must be a string"
+        assert isinstance(
+            wavelength_set_m, (list, np.ndarray)
+        ), "wavelengths must be passed as a list."
+
+        diffraction_engine = diffraction_engine.lower()
+        assert diffraction_engine in [
+            "asm",
+            "fresnel",
+        ], "Diffraction engine must be either 'asm' or 'fresnel'"
+
+        propagator = (
+            ASMPropagation if diffraction_engine == "asm" else FresnelPropagation
+        )
+        self.propagator = propagator(
             in_size,
             in_dx_m,
             out_distance_m,
             out_size,
             out_dx_m,
+            wavelength_set_m,
             out_resample_dx_m,
             manual_upsample_factor,
             radial_symmetry,
+            verbose=verbose,
         )
-        self._init_calc_params()
 
-    def forward(self, amplitude, phase, wavelength_set_m):
-        """Propagates a complex field from an input plane to a planar output plane a distance out_distance_m.
+        self.rescale = 1e6  # Convert m to um
+        self.wavelength_set = torch.tensor(wavelength_set_m) * self.rescale
+        self.in_size = in_size
+        self.in_dx_m = in_dx_m
+        self.out_resample_dx = (
+            out_dx_m if out_resample_dx_m is None else out_resample_dx_m
+        )
+        self.radial_symmetry = radial_symmetry
+
+    def forward(
+        self,
+        amplitude,
+        phase,
+        ps_locs_m,
+        aperture=None,
+        normalize_to_aperture=True,
+        **kwargs,
+    ):
+        """_summary_
 
         Args:
-            amplitude (float): Field amplitude of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
-            phase (float): Field phase of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
-        """
+            amplitude (tensor): Lens amplitude of shape [... L H W], where L may equal 1 for broadcasting.
+            phase (tensor): Lens phase of shape [... L H W], where L may equal 1 for broadcasting.
+            ps_locs_m (tensor): Array point-source locations of shape [N x 3] where each column corresponds to Y, X, Depth
+            aperture (Tensor, optional): Field aperture applied on the lens the same rank as amplitude
+                and with the same H W dimensions. Defaults to None.
+            normalize_to_aperture (bool, optional): If true the energy in the PSF will be normalized to the total energy
+                incident on the optic/aperture. Defaults to True.
 
-        assert amplitude.shape == phase.shape, "amplitude and phase must be same shape."
+        Returns:
+            List: Returns point-spread function intensity and phase of shape [B P Z L H W].
+        """
+        if "wavelength_set_m" in kwargs:
+            raise ValueError(
+                "The 'wavelength_set_m' is not expected in this model. "
+                "Please use the propagator from dflat.propagation.propagators_legacy class that accepts wavelength as a forward input."
+            )
         assert (
-            len(wavelength_set_m) == amplitude.shape[-3] or amplitude.shape[-3] == 1
-        ), "Wavelength dimensions don't match"
+            amplitude.shape == phase.shape
+        ), "ampl and phase should be the same shape."
+        assert len(amplitude.shape) >= 4, "field profile must be at least rank 4"
+        assert (
+            len(self.wavelength_set) == amplitude.shape[-3] or amplitude.shape[-3] == 1
+        ), "Mismatch in number of simulation wavelengths and wavelength dimension of profile."
+        ps_locs_m = np.array(ps_locs_m) if not torch.is_tensor(ps_locs_m) else ps_locs_m
+        assert len(ps_locs_m.shape) == 2
+        assert ps_locs_m.shape[-1] == 3
         if self.radial_symmetry:
             assert amplitude.shape[-2] == 1, "Radial flag requires 1D input not 2D."
             assert amplitude.shape[-1] == self.in_size[-1] // 2 + 1
         else:
-            assert all(
-                amplitude.shape[-2:] == self.in_size
+            assert (
+                list(amplitude.shape[-2:]) == self.in_size
             ), f"Input field size does not match init in_size {self.in_size}."
+        if aperture is not None:
+            assert aperture.shape[-2:] == amplitude.shape[-2:]
+            assert len(aperture.shape) == len(amplitude.shape)
 
-        device = "cuda" if torch.cuda.is_available() else "cpu"
         amplitude = (
-            torch.tensor(amplitude, dtype=torch.float32).to(device)
+            torch.tensor(amplitude, dtype=torch.float32)
             if not torch.is_tensor(amplitude)
             else amplitude.to(dtype=torch.float32)
         )
         phase = (
-            torch.tensor(phase, dtype=torch.float32).to(device)
+            torch.tensor(phase, dtype=torch.float32)
             if not torch.is_tensor(phase)
             else phase.to(dtype=torch.float32)
         )
-        wavelength_set = (
-            torch.tensor(
-                np.array(wavelength_set_m) * self.rescale, dtype=amplitude.dtype
-            ).to(amplitude.device)
-            if not torch.is_tensor(wavelength_set_m)
-            else wavelength_set_m.to(dtype=amplitude.dtype) * self.rescale
-        )
-
-        # Upsample and pad the field prior to fourier-based propagation transformation
-        amplitude, phase = self._regularize_field(amplitude, phase, wavelength_set)
-
-        # propagate by the fresnel method
-        amplitude, phase = self.fresnel_transform(amplitude, phase, wavelength_set)
-
-        # Transform field back to the specified output grid
-        amplitude, phase = self._resample_field(amplitude, phase)
-
-        # Convert to 2D and return to final sensor size
-        for i, (amp, ph) in enumerate(zip(amplitude, phase)):
-            if self.radial_symmetry:
-                amp = radial_2d_transform(amp.squeeze(-2))
-                ph = radial_2d_transform_wrapped_phase(ph.squeeze(-2))
-
-            phase[i] = resize_with_crop_or_pad(ph, *self.out_size, False)
-            amplitude[i] = resize_with_crop_or_pad(amp, *self.out_size, False)
-
-        amplitude = torch.cat(amplitude, axis=-3)
-        phase = torch.cat(phase, axis=-3)
-
-        return amplitude, phase
-
-    def fresnel_transform(self, amplitude, phase, wavelength_set):
-        radial_symmetry = self.radial_symmetry
-        dtype = amplitude[0].dtype
-        device = amplitude[0].device
-        torch_zero = torch.tensor(0.0, dtype=dtype, device=device)
-
-        for i, lam in enumerate(wavelength_set):
-            # Define grid and compute quadratic term
-            insize = amplitude[i].shape[-2:]
-            x, y = torch.meshgrid(
-                torch.arange(0, insize[-1], dtype=dtype, device=device),
-                torch.arange(0, insize[-2], dtype=dtype, device=device),
-                indexing="xy",
-            )
-            if not radial_symmetry:
-                x = x - (x.shape[-1] // 2)
-                y = y - (y.shape[-2] // 2)
-
-            quadratic_term = (
-                np.pi
-                / lam
-                / self.out_distance
-                * ((x * self.calc_in_dx[-1]) ** 2 + (y * self.calc_in_dx[-2]) ** 2)
+        if aperture is not None:
+            aperture = (
+                torch.tensor(aperture, dtype=torch.float32, device=amplitude.device)
+                if not torch.is_tensor(aperture)
+                else aperture.to(dtype=torch.float32)
             )
 
-            transform_term = torch.complex(amplitude[i], torch_zero) * torch.exp(
-                torch.complex(torch_zero, phase[i] + quadratic_term)
-            )
-
-            # propagate with qdht or fft2
-            if radial_symmetry:
-                ang_fx = torch.arange(
-                    0,
-                    1 / 2 / self.calc_in_dx[-1],
-                    1 / self.calc_in_dx[-1] / self.calc_samplesN[i, -1],
-                    dtype=dtype,
-                    device=device,
-                )
-                norm = torch.tensor(
-                    1
-                    / np.sqrt(
-                        (
-                            np.prod(self.calc_in_dx)
-                            * np.prod(self.calc_out_dx[i])
-                            * np.prod(self.calc_samplesN[i])
-                        )
-                    ),
-                    dtype=dtype,
-                    device=device,
-                )
-                kr, wavefront = qdht(
-                    torch.squeeze(x * self.calc_in_dx[-1]), transform_term
-                )
-                wavefront = general_interp_regular_1d_grid(
-                    kr / 2 / np.pi, ang_fx, wavefront
-                ) * torch.complex(norm, torch_zero)
-            else:
-                norm = torch.tensor(
-                    np.sqrt(
-                        np.prod(self.calc_in_dx)
-                        / np.prod(self.calc_out_dx[i])
-                        / np.prod(self.calc_samplesN[i])
-                    ),
-                    dtype=torch.float32,
-                    device=device,
-                )
-                wavefront = fftshift(fft2(ifftshift(transform_term))) * torch.complex(
-                    norm, torch_zero
-                )
-
-            # add the complex phase term on the output
-            phase_add = (
-                2
-                * np.pi
-                / lam
-                * (
-                    self.out_distance
-                    + (
-                        (x * self.calc_out_dx[i, -1]) ** 2
-                        + (y * self.calc_out_dx[i, -2]) ** 2
-                    )
-                    / 2
-                    / self.out_distance
-                )
-            )
-
-            amplitude[i] = torch.abs(wavefront)
-            phase[i] = torch.angle(
-                wavefront * torch.exp(torch.complex(torch_zero, phase_add))
-            )
-
-        return amplitude, phase
-
-    def _resample_field(self, amplitude, phase):
-        # Reinterpolate the phase with area averaging and the amplitude with area sum
-        nl = len(amplitude)
-        for i in range(nl):
-            scale = tuple(self.calc_out_dx[i] / self.out_resample_dx)
-            if self.radial_symmetry:
-                scale = (1, scale[-1])
-
-            phase[i] = torch.atan2(
-                F.interpolate(torch.sin(phase[i]), scale_factor=scale, mode="area"),
-                F.interpolate(torch.cos(phase[i]), scale_factor=scale, mode="area"),
-            )
-            amplitude[i] = F.interpolate(amplitude[i], scale_factor=scale, mode="area")
-
-        return amplitude, phase
-
-    def _regularize_field(self, amplitude, phase, wavelength_set):
-        # Natural broadcasting of the wavelength dimension cannot be done for Fresnel case
-        if amplitude.shape[-3] == 1:
-            amplitude = amplitude.repeat(1, len(wavelength_set), 1, 1)
-            phase = phase.repeat(1, len(wavelength_set), 1, 1)
-
-        # Resample the input field via nearest neighbors interpolation
-        # Nearest matches openCV's implementation but torch recommends using nearest-exact
-        method = "nearest-exact"
-        samplesM = self.calc_samplesM
-        radial_symmetry = self.radial_symmetry
-        resize_to = np.array([1, samplesM[1] // 2 + 1]) if radial_symmetry else samplesM
-        resize_to = tuple([int(_) for _ in resize_to])
-        amplitude = F.interpolate(amplitude, size=resize_to, mode=method)
-        phase = F.interpolate(phase, size=resize_to, mode=method)
+        # Reshape B P L H  W to B L H W
+        init_shape = amplitude.shape
+        amplitude = amplitude.view(-1, *init_shape[-3:])
+        phase = phase.view(-1, *init_shape[-3:])
 
-        # Add padding -- this changes the output grid dx so we need to pad per wavelength
-        # Thus what follows will be a jagged tensor (for now a list)
-        estN = np.ceil(
-            wavelength_set[:, None].cpu().numpy()
-            * self.out_distance
-            / self.out_dx[None, :]
-            / self.calc_in_dx
-        )
-        estN = np.where(np.mod(estN, 2) == 0, estN + 1, estN)
-        estN = np.where(estN < self.calc_samplesM, self.calc_samplesM, estN)
-        estN = np.where(estN < self.calc_samplesN, self.calc_samplesN, estN)
+        # Apply incident wavefront
+        N = amplitude.shape[0]
+        Z = len(ps_locs_m)
+        amplitude, phase = self._incident_wavefront(amplitude, phase, ps_locs_m)
+        if aperture is not None:
+            amplitude = amplitude * aperture
+
+        # Propagate field to sensor
+        amplitude = rearrange(amplitude, "Z N L H W -> (N Z) L H W")
+        phase = rearrange(phase, "Z N L H W -> (N Z) L H W")
+        amplitude, phase = self.propagator(amplitude, phase)
+        amplitude = rearrange(amplitude, "(N Z) L H W -> N Z L H W", N=N, Z=Z)
+        phase = rearrange(phase, "(N Z) L H W -> N Z L H W", N=N, Z=Z)
+
+        # Return to the original shape before returning
+        out_shape = amplitude.shape
+        amplitude = amplitude.view(*init_shape[:-3], *out_shape[-4:])
+        phase = phase.view(*init_shape[:-3], *out_shape[-4:])
+
+        amplitude = amplitude**2
+        normalization = (
+            np.prod(self.out_resample_dx) / self.aperture_energy(aperture)
+        ).to(dtype=amplitude.dtype, device=amplitude.device)
+        if normalize_to_aperture:
+            return amplitude * normalization, phase
+        else:
+            return amplitude, phase
 
-        pad_in = (estN - self.calc_samplesM) / 2
-        pad_in = pad_in.astype(int)
+    def _incident_wavefront(self, amplitude, phase, ps_locs_m):
+        # Z N L H W
+        # Expand dimension to hold point_sources
+        device = amplitude.device
+        amplitude = amplitude[None].to(dtype=torch.float64)
+        phase = phase[None].to(dtype=torch.float64)
+        torch_zero = torch.tensor([0.0], dtype=torch.float64, device=device)
+        wavelength_set = self.wavelength_set.to(dtype=torch.float64, device=device)
 
-        # Now redefine the exact output calculation grid
-        self.calc_samplesN = estN
-        self.calc_out_dx = (
-            wavelength_set[:, None].cpu().numpy()
-            * self.out_distance
-            / self.calc_in_dx
-            / estN
-        )
+        k = 2 * np.pi / wavelength_set
+        k = k[None, None, :, None, None]
 
-        ampl_list = []
-        phase_list = []
-        for i, _ in enumerate(wavelength_set):
-            padi = pad_in[i]
-            paddings = (
-                [0, padi[1], 0, 0, 0, 0, 0, 0]
-                if radial_symmetry
-                else [padi[1], padi[1], padi[0], padi[0], 0, 0, 0, 0]
-            )
-            ampl_list.append(
-                F.pad(amplitude[:, i : i + 1], paddings, mode="constant", value=0)
-            )
-            phase_list.append(
-                F.pad(phase[:, i : i + 1], paddings, mode="constant", value=0)
+        ps_locs = (
+            torch.tensor(
+                np.array(ps_locs_m) * self.rescale, dtype=torch.float64, device=device
             )
-
-        return ampl_list, phase_list
-
-    def _init_calc_params(self):
-        # Compute the input grid and upsampled size when we upsample the input field
-        in_dx = self.in_dx
-
-        calc_in_dx = in_dx / self.manual_upsample_factor
-        in_length = in_dx * self.in_size
-        calc_samplesM = np.rint(in_length / calc_in_dx)
-        calc_samplesM = np.where(
-            np.mod(calc_samplesM, 2) == 0, calc_samplesM + 1, calc_samplesM
+            if not torch.is_tensor(ps_locs_m)
+            else ps_locs_m.to(dtype=torch.float64, device=device) * self.rescale
         )
-        calc_samplesM_r = calc_samplesM[-1] // 2
-        self.calc_samplesM = calc_samplesM
-        self.calc_samplesM_r = calc_samplesM_r
+        psx = ps_locs[:, 0][:, None, None, None, None]
+        psy = ps_locs[:, 1][:, None, None, None, None]
+        psz = ps_locs[:, 2][:, None, None, None, None]
+
+        x, y = cart_grid(
+            self.in_size,
+            list(np.array(self.in_dx_m) * self.rescale),
+            self.radial_symmetry,
+            torch.float64,
+            device,
+        )
+        x = x[None, None, None]
+        y = y[None, None, None]
+        distance = torch.sqrt((x - psx) ** 2 + (y - psy) ** 2 + psz**2)  # Z x H x W
+
+        wavefront = torch.complex(amplitude, torch_zero) * torch.exp(
+            torch.complex(torch_zero, phase + k * distance)
+        )
+
+        return torch.abs(wavefront).to(dtype=torch.float32), torch.angle(wavefront).to(
+            dtype=torch.float32
+        )
+
+    @torch.no_grad()
+    def aperture_energy(self, aperture):
+        in_size = self.in_size
+        sz = [
+            1,
+            1,
+            1 if self.radial_symmetry else in_size[-2],
+            in_size[-1] // 2 + 1 if self.radial_symmetry else in_size[-1],
+        ]
 
-        # Update the calculation grid corresponding to the upsampled integer number of samples
-        self.calc_in_dx = in_length / calc_samplesM
+        fieldblock2d = aperture if aperture is not None else torch.ones(size=sz)
+        if self.radial_symmetry:
+            fieldblock2d = radial_2d_transform(fieldblock2d.squeeze(-2))
 
-        # The fourier transform implies that the number of samples in the output grid will match the
-        # input grid. To compute on the full output_plane, we should zero pad if needed in input (keep odd)
-        calc_samplesN = np.where(
-            self.out_size > self.in_size, self.out_size, self.in_size
-        )
-        self.calc_samplesN = np.where(
-            np.mod(calc_samplesN, 2) == 0, calc_samplesN + 1, calc_samplesN
-        )
-
-        # For the Fresnel Engine, the output field grid size is tuned by zero-padding the input field
-        # We should then zero-pad more, dependent on wavelength, to get the output pixel size. This will
-        # be computed on the fly in forward call
-
-
-# Initially started playing around with calculating the correct upsample factor to avoid cropped
-# field calculations. It utlimately is not a trivial tweak given the current class structure
-# class FresnelPropagation(BaseFrequencySpace):
-#     def __init__(
-#         self,
-#         in_size,
-#         in_dx_m,
-#         out_distance_m,
-#         out_size,
-#         out_dx_m,
-#         out_resample_dx_m=None,
-#         manual_upsample_factor=1,
-#         radial_symmetry=False,
-#         *args,
-#         **kwargs,
-#     ):
-#         super().__init__(
-#             in_size,
-#             in_dx_m,
-#             out_distance_m,
-#             out_size,
-#             out_dx_m,
-#             out_resample_dx_m,
-#             manual_upsample_factor,
-#             radial_symmetry,
-#         )
-#         self._init_calc_params()
-
-#     def forward(self, amplitude, phase, wavelength_set_m):
-#         """Propagates a complex field from an input plane to a planar output plane a distance out_distance_m.
-
-#         Args:
-#             amplitude (float): Field amplitude of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
-#             phase (float): Field phase of shape (Batch, Lambda, *in_size) or (Batch, Lambda, 1, in_size_r).
-#         """
-
-#         assert amplitude.shape == phase.shape, "amplitude and phase must be same shape."
-#         assert (
-#             len(wavelength_set_m) == amplitude.shape[-3] or amplitude.shape[-3] == 1
-#         ), "Wavelength dimensions don't match"
-#         if self.radial_symmetry:
-#             assert amplitude.shape[-2] == 1, "Radial flag requires 1D input not 2D."
-#             assert amplitude.shape[-1] == self.in_size[-1] // 2 + 1
-#         else:
-#             assert all(
-#                 amplitude.shape[-2:] == self.in_size
-#             ), f"Input field size does not match init in_size {self.in_size}."
-
-#         device = "cuda" if torch.cuda.is_available() else "cpu"
-#         amplitude = (
-#             torch.tensor(amplitude, dtype=torch.float32).to(device)
-#             if not torch.is_tensor(amplitude)
-#             else amplitude.to(dtype=torch.float32)
-#         )
-#         phase = (
-#             torch.tensor(phase, dtype=torch.float32).to(device)
-#             if not torch.is_tensor(phase)
-#             else phase.to(dtype=torch.float32)
-#         )
-#         wavelength_set = (
-#             torch.tensor(
-#                 np.array(wavelength_set_m) * self.rescale, dtype=amplitude.dtype
-#             ).to(amplitude.device)
-#             if not torch.is_tensor(wavelength_set_m)
-#             else wavelength_set_m.to(dtype=amplitude.dtype)
-#         )
-
-#         # Upsample and pad the field prior to fourier-based propagation transformation
-#         amplitude, phase = self._regularize_field(amplitude, phase, wavelength_set)
-
-#         # propagate by the fresnel method
-#         amplitue, phase = self.fresnel_transform(amplitude, phase, wavelength_set)
-
-#         # Transform field back to the specified output grid
-#         amplitude, phase = self._resample_field(amplitude, phase)
-
-#         # Convert to 2D and return to final sensor size
-#         for i, (amp, ph) in enumerate(zip(amplitude, phase)):
-#             if self.radial_symmetry:
-#                 amp = radial_2d_transform(amp.squeeze(-2))
-#                 ph = radial_2d_transform_wrapped_phase(ph.squeeze(-2))
-
-#             phase[i] = resize_with_crop_or_pad(ph, *self.out_size, False)
-#             amplitude[i] = resize_with_crop_or_pad(amp, *self.out_size, False)
-
-#         amplitude = torch.cat(amplitude, axis=-3)
-#         phase = torch.cat(phase, axis=-3)
-
-#         return amplitude, phase
-
-#     def fresnel_transform(self, amplitude, phase, wavelength_set):
-#         radial_symmetry = self.radial_symmetry
-#         dtype = amplitude[0].dtype
-#         device = amplitude[0].device
-#         torch_zero = torch.tensor(0.0, dtype=dtype, device=device)
-
-#         for i, lam in enumerate(wavelength_set):
-#             # Define grid and compute quadratic term
-#             insize = amplitude[i].shape[-2:]
-#             x, y = torch.meshgrid(
-#                 torch.arange(0, insize[-1], dtype=dtype, device=device),
-#                 torch.arange(0, insize[-2], dtype=dtype, device=device),
-#                 indexing="xy",
-#             )
-#             if not radial_symmetry:
-#                 x = x - (x.shape[-1] // 2)
-#                 y = y - (y.shape[-2] // 2)
-
-#             quadratic_term = (
-#                 np.pi
-#                 / lam
-#                 / self.out_distance
-#                 * ((x * self.calc_in_dx[-1]) ** 2 + (y * self.calc_in_dx[-2]) ** 2)
-#             )
-
-#             transform_term = torch.complex(amplitude[i], torch_zero) * torch.exp(
-#                 torch.complex(torch_zero, phase[i] + quadratic_term)
-#             )
-
-#             # propagate with qdht or fft2
-#             if radial_symmetry:
-#                 ang_fx = torch.arange(
-#                     0,
-#                     1 / 2 / self.calc_in_dx[-1],
-#                     1 / self.calc_in_dx[-1] / self.calc_samplesN[i, -1],
-#                     dtype=dtype,
-#                     device=device,
-#                 )
-#                 norm = torch.tensor(
-#                     1
-#                     / np.sqrt(
-#                         (
-#                             np.prod(self.calc_in_dx)
-#                             * np.prod(self.calc_out_dx[i])
-#                             * np.prod(self.calc_samplesN[i])
-#                         )
-#                     ),
-#                     dtype=dtype,
-#                     device=device,
-#                 )
-#                 kr, wavefront = qdht(
-#                     torch.squeeze(x * self.calc_in_dx[-1]), transform_term
-#                 )
-#                 wavefront = general_interp_regular_1d_grid(
-#                     kr / 2 / np.pi, ang_fx, wavefront
-#                 ) * torch.complex(norm, torch_zero)
-#             else:
-#                 norm = torch.tensor(
-#                     np.sqrt(
-#                         np.prod(self.calc_in_dx)
-#                         / np.prod(self.calc_out_dx[i])
-#                         / np.prod(self.calc_samplesN[i])
-#                     ),
-#                     dtype=torch.float32,
-#                     device=device,
-#                 )
-#                 wavefront = fftshift(fft2(ifftshift(transform_term))) * torch.complex(
-#                     norm, torch_zero
-#                 )
-
-#             # add the complex phase term on the output
-#             phase_add = (
-#                 2
-#                 * np.pi
-#                 / lam
-#                 * (
-#                     self.out_distance
-#                     + (
-#                         (x * self.calc_out_dx[i, -1]) ** 2
-#                         + (y * self.calc_out_dx[i, -2]) ** 2
-#                     )
-#                     / 2
-#                     / self.out_distance
-#                 )
-#             )
-
-#             amplitude[i] = torch.abs(wavefront)
-#             phase[i] = torch.angle(
-#                 wavefront * torch.exp(torch.complex(torch_zero, phase_add))
-#             )
-
-#         return amplitude, phase
-
-#     def _resample_field(self, amplitude, phase):
-#         # Reinterpolate the phase with area averaging and the amplitude with area sum
-#         nl = len(amplitude)
-#         for i in range(nl):
-#             scale = tuple(self.calc_out_dx[i] / self.out_resample_dx)
-#             if self.radial_symmetry:
-#                 scale = (1, scale[-1])
-
-#             phase[i] = torch.atan2(
-#                 F.interpolate(torch.sin(phase[i]), scale_factor=scale, mode="area"),
-#                 F.interpolate(torch.cos(phase[i]), scale_factor=scale, mode="area"),
-#             )
-#             amplitude[i] = F.interpolate(amplitude[i], scale_factor=scale, mode="area")
-
-#         return amplitude, phase
-
-#     def _regularize_field(self, amplitude, phase, wavelength_set):
-#         # Natural broadcasting of the wavelength dimension cannot be done for Fresnel case
-#         if amplitude.shape[-3] == 1:
-#             amplitude = amplitude.repeat(1, len(wavelength_set), 1, 1)
-#             phase = phase.repeat(1, len(wavelength_set), 1, 1)
-
-#         # Resample the input field via nearest neighbors interpolation
-#         # Nearest matches openCV's implementation but torch recommends using nearest-exact
-#         method = "nearest-exact"
-
-#         # We actually should enforce a new manual upsampling to ensure full field calculations
-#         # If you remove this, you can get cropped outputs
-#         force_factor = np.round(
-#             self.out_dx_m[None]
-#             * self.out_size[None]
-#             * self.in_dx_m[None]
-#             / wavelength_set[:, None, None].cpu().numpy()
-#             * self.rescale
-#             / self.out_distance_m
-#         )
-#         manual_upsample = [self.manual_upsample_factor, self.manual_upsample_factor]
-#         in_length = self.in_dx * self.in_size
-#         ampl_list = []
-#         phase_list = []
-#         for i in range(len(wavelength_set)):
-#             # For simplicity, just use one upsample factor
-#             use_upsample = np.maximum(force_factor[i], manual_upsample).max()
-#             calc_in_dx = self.in_dx / use_upsample
-#             calc_samplesM = np.rint(in_length / calc_in_dx)
-
-#             # Update the calculation grid corresponding to the upsampled integer number of samples
-#             calc_in_dx = in_length / calc_samplesM
-#             calc_samplesN = np.where(
-#                 self.out_size > self.in_size, self.out_size, self.in_size
-#             )
-
-#             radial_symmetry = self.radial_symmetry
-#             resize_to = (
-#                 np.array([1, calc_samplesM[1] // 2 + 1])
-#                 if radial_symmetry
-#                 else calc_samplesM
-#             )
-#             resize_to = tuple([int(_) for _ in resize_to])
-#             amplitude = F.interpolate(amplitude, size=resize_to, mode=method)
-#             phase = F.interpolate(phase, size=resize_to, mode=method)
-
-#             # Add padding -- this changes the output grid dx so we need to pad per wavelength
-#             # Thus what follows will be a jagged tensor (for now a list)
-#             estN = np.ceil(
-#                 wavelength_set[:, None].cpu().numpy()
-#                 * self.out_distance
-#                 / self.out_dx[None, :]
-#                 / calc_in_dx
-#             )
-#             estN = np.where(np.mod(estN, 2) == 0, estN + 1, estN)
-
-#             estN = np.where(estN < calc_samplesM, calc_samplesM, estN)
-#             estN = np.where(estN < calc_samplesN, calc_samplesN, estN)
-#             pad_in = (estN - self.calc_samplesM) / 2
-#             pad_in = pad_in.astype(int)
-
-#             # Now redefine the exact output calculation grid
-#             self.calc_out_dx = (
-#                 wavelength_set[:, None].cpu().numpy()
-#                 * self.out_distance
-#                 / calc_in_dx
-#                 / estN
-#             )
-
-#             padi = pad_in[i]
-#             paddings = (
-#                 [0, padi[1], 0, 0, 0, 0, 0, 0]
-#                 if radial_symmetry
-#                 else [padi[1], padi[1], padi[0], padi[0], 0, 0, 0, 0]
-#             )
-#             ampl_list.append(
-#                 F.pad(amplitude[:, i : i + 1], paddings, mode="constant", value=0)
-#             )
-#             phase_list.append(
-#                 F.pad(phase[:, i : i + 1], paddings, mode="constant", value=0)
-#             )
-
-#         return ampl_list, phase_list
-
-#     def _init_calc_params(self):
-#         # # Compute the input grid and upsampled size when we upsample the input field
-#         # in_dx = self.in_dx
-#         # in_length = in_dx * self.in_size
-
-#         # calc_in_dx = in_dx / self.manual_upsample_factor
-#         # calc_samplesM = np.rint(in_length / calc_in_dx)
-#         # calc_samplesM = np.where(
-#         #     np.mod(calc_samplesM, 2) == 0, calc_samplesM + 1, calc_samplesM
-#         # )
-#         # calc_samplesM_r = calc_samplesM[-1] // 2
-#         # self.calc_samplesM = calc_samplesM
-#         # self.calc_samplesM_r = calc_samplesM_r
-
-#         # # Update the calculation grid corresponding to the upsampled integer number of samples
-#         # self.calc_in_dx = in_length / calc_samplesM
-
-#         # # The fourier transform implies that the number of samples in the output grid will match the
-#         # # input grid. To compute on the full output_plane, we should zero pad if needed in input (keep odd)
-
-#         # calc_samplesN = np.where(
-#         #     self.out_size > self.in_size, self.out_size, self.in_size
-#         # )
-#         # self.calc_samplesN = np.where(
-#         #     np.mod(calc_samplesN, 2) == 0, calc_samplesN + 1, calc_samplesN
-#         # )
-
-#         # # For the Fresnel Engine, the output field grid size is tuned by zero-padding the input field
-#         # # We should then zero-pad more, dependent on wavelength, to get the output pixel size. This will
-#         # # be computed on the fly in forward call
-#         return
-#
-#
-# if __name__ == "__main__":
-#     import numpy as np
-#     import matplotlib.pyplot as plt
-
-#     from dflat.initialize import focusing_lens
-#     from dflat.propagation import ASMPropagation, FresnelPropagation
-
-#     in_size = [701, 701]
-#     in_dx_m = [500e-9, 500e-9]
-#     wavelength_set_m = [532e-9]
-#     depth_set_m = [1.0]
-#     fshift_set_m = [[0.0, 0.0]]
-#     out_distance_m = 500e-6
-
-#     lens_t, lens_phi, aperture = focusing_lens(
-#         in_size,
-#         in_dx_m,
-#         wavelength_set_m,
-#         depth_set_m,
-#         fshift_set_m,
-#         out_distance_m,
-#         aperture_radius_m=150e-6,
-#     )
-
-#     print(lens_t.shape, aperture.shape)
-#     lens_t = lens_t * aperture
-#     lens_phi = lens_phi * aperture
-
-#     fig, ax = plt.subplots(1, 2)
-#     ax[0].imshow(lens_t[0], vmin=0, vmax=1)
-#     ax[1].imshow(lens_phi[0])
-
-#     out_size = in_size
-#     out_dx_m = in_dx_m
-#     out_distance_m = 100e-6
-#     propagator = FresnelPropagation(
-#         in_size, in_dx_m, out_distance_m, out_size, out_dx_m, manual_upsample_factor=1
-#     )
+        in_energy = torch.sum(
+            fieldblock2d**2 * np.prod(self.in_dx_m),
+            dim=(-1, -2),
+            keepdim=True,
+        )[None]
 
-#     out_t, out_phi = propagator(lens_t[None], lens_phi[None], [500e-9, 600e-9, 700e-9])
+        return in_energy
```

### Comparing `dflat_opt-3.0.1/dflat/propagation/util.py` & `dflat_opt-3.1.0/dflat/propagation/util.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/radial_tranforms/hankel_ops.py` & `dflat_opt-3.1.0/dflat/radial_tranforms/hankel_ops.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/radial_tranforms/radial_ops.py` & `dflat_opt-3.1.0/dflat/radial_tranforms/radial_ops.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/QE_Estimates/QE_CMOS_Pregius.csv` & `dflat_opt-3.1.0/dflat/render/QE_Estimates/QE_CMOS_Pregius.csv`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/QE_Estimates/RGB_Basler_Ace2_QE.csv` & `dflat_opt-3.1.0/dflat/render/QE_Estimates/RGB_Basler_Ace2_QE.csv`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/QE_Estimates/readme.txt` & `dflat_opt-3.1.0/dflat/render/QE_Estimates/readme.txt`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/color_space/1931RGBFunctions.txt` & `dflat_opt-3.1.0/dflat/render/color_space/1931RGBFunctions.txt`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/color_space/1931XYZFunctions.txt` & `dflat_opt-3.1.0/dflat/render/color_space/1931XYZFunctions.txt`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/fft_convolve.py` & `dflat_opt-3.1.0/dflat/render/fft_convolve.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import torch
 import torch.nn.functional as F
+from torch.utils.checkpoint import checkpoint
 from torch.fft import fftshift, ifftshift, fft2, ifft2, rfft2, irfft2
 from dflat.radial_tranforms import resize_with_crop_or_pad
 
 
 def general_convolve(image, filter, rfft=False):
     """Runs the Fourier space convolution between an image and filter, where the filter kernels may have a different size from the image shape.
 
@@ -42,16 +43,17 @@
         padby[2:4] = [filt_ny // 2, filt_ny // 2]
     image = F.pad(image, padby, mode="constant", value=0.0)
 
     ### Pad the psf to match the new image dimensionality
     image_shape = image.shape
     filter_resh = resize_with_crop_or_pad(filter, *image_shape[-2:], radial_flag=False)
 
-    ### Run the convolution
-    image = torch.real(fourier_convolve(image, filter_resh, rfft))
+    ### Run the convolution (Defualt to using a checkpoint of the fourier transform)
+    image = checkpoint(fourier_convolve, image, filter_resh, rfft)
+    image = torch.real(image)
 
     ### Undo odd padding if it was done before FFT
     image = resize_with_crop_or_pad(image, *init_image_shape[-2:], False)
     return image
 
 
 def weiner_deconvolve(image, filter, const=1e-4, abs=False):
```

### Comparing `dflat_opt-3.0.1/dflat/render/fronto_planar_renderer.py` & `dflat_opt-3.1.0/dflat/render/fronto_planar_renderer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import numpy as np
 import torch
 import torch.nn as nn
 from einops import rearrange
+from torch.utils.checkpoint import checkpoint
 
 from .fft_convolve import general_convolve
 from dflat.radial_tranforms import resize_with_crop_or_pad
 from .util_meas import hsi_to_rgb
 
 
 class Fronto_Planar_Renderer_Incoherent(nn.Module):
     def __init__(self):
         super().__init__()
 
-    def forward(
-        self,
-        psf_intensity,
-        scene_radiance,
-        rfft=True,
-        crop_to_psf_dim=False,
-    ):
+    def forward(self, psf_intensity, scene_radiance, rfft=True, crop_to_psf_dim=False):
         if len(scene_radiance.shape) == 5:
             scene_radiance = scene_radiance[None]
         psf_shape = psf_intensity.shape
         srad_shape = scene_radiance.shape
         # psf has shape  [B P Z L H W]
         # scene radiance [1 P Z L H W]
 
@@ -42,20 +37,25 @@
         )
         scene_radiance = (
             torch.tensor(scene_radiance, dtype=torch.float32)
             if not torch.is_tensor(scene_radiance)
             else scene_radiance.to(dtype=torch.float32)
         )
 
+        return checkpoint(
+            self._forward, psf_intensity, scene_radiance, rfft, crop_to_psf_dim
+        )
+
+    def _forward(self, psf_intensity, scene_radiance, rfft, crop_to_psf_dim):
         # Run the spatial convolution
         meas = general_convolve(scene_radiance, psf_intensity, rfft)
         if crop_to_psf_dim:
-            resize_with_crop_or_pad(meas, *psf_shape[-2:], False)
+            resize_with_crop_or_pad(meas, *psf_intensity.shape[-2:], False)
 
-        # Add noise
+        # Add noise or other image stuff here
         ## TO be updated and added later
         return meas
 
     def rgb_measurement(self, meas, wavelength_set_m, bayer_mosaic=False, gamma=True):
         B, P, Z, L, H, W = meas.shape
         meas = hsi_to_rgb(
             rearrange(meas, "B P Z L H W -> (B P Z) H W L", B=B, P=P, Z=Z),
```

### Comparing `dflat_opt-3.0.1/dflat/render/illuminants/D65.txt` & `dflat_opt-3.1.0/dflat/render/illuminants/D65.txt`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/util_meas.py` & `dflat_opt-3.1.0/dflat/render/util_meas.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/util_sensor.py` & `dflat_opt-3.1.0/dflat/render/util_sensor.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat/render/util_spectral.py` & `dflat_opt-3.1.0/dflat/render/util_spectral.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/dflat_opt.egg-info/PKG-INFO` & `dflat_opt-3.1.0/dflat_opt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,17 @@
 Metadata-Version: 2.1
-Name: dflat_opt
-Version: 3.0.1
+Name: dflat-opt
+Version: 3.1.0
 Summary: D-Flat is a forward and inverse design framework for flat optics. Although specially geared for the design of metasurfaces, it may be used broadly for end-to-end imaging and sensing task.
 Home-page: https://github.com/DeanHazineh/DFlat
 Author: Dean Hazineh
 Author-email: dhazineh@g.harvard.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: pytest
-Requires-Dist: pytest-cov
-Requires-Dist: requests
-Requires-Dist: setuptools
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: moviepy
-Requires-Dist: pyhank
-Requires-Dist: einops
-Requires-Dist: tqdm
-Requires-Dist: pandas
-Requires-Dist: opencv-python
-Requires-Dist: gdspy
-Requires-Dist: mat73
-Requires-Dist: omegaconf
-Requires-Dist: natsort
 
 <div align="center">
   <img src=/docs/DFlat_Long.png alt="Dflat" width="500"/>
 </div>
 <div align="center">
   <img src=/docs/autoGDS_metalens.png alt="Dflat" width="500"/>
 </div>
@@ -68,18 +51,19 @@
 ```
 
 ## Version Notes (v3.0.0)
 
 Updated on April 11, 2024 | V2 -> V3
 - Documentation is still in development :o 
 - (v3) You can now donwload this package from the PyPi Index!
-- (v3) Datasets and pre-trained models are now downloaded when called insetad of during install. Models are now initialized by their name instead of by paths to config files. 
+- (v3) Datasets and pre-trained models are now downloaded when called insetad of during install. Models are now initialized by their name instead of by paths to config files.
+- (v3) Memory problems? Gradient checkpointing is added throughout reducing memory when using DFLat at the cost of slightly slower runtimes. 
 - (v2) This repository is the home for the new and maintained version of DFlat. It replaces DFlat-Tensorflow.
-- (v2) Note that this package is no longer a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in February 2024.
-- (v2) The structure of the software is completely revamped and the algorithms used--in particular for field propagation--are not the same as before. The original pytorch version (now deprecated) is archived and kept as a branch.
+- (v2) Note that this package is no longer a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in February 2024. I recommend switching!
+- (v2) The structure of the software is completely revamped and the algorithms used throughout are not the same as before. The original pytorch version (now deprecated) is archived and kept as a branch.
 
 ## Usage and Documentation
 
 Detailed documentation for the rewritten package and a new project page will be released in the future. For now, we highlight two resources for developers and researchers:
 - A script used to train neural models can be found in `scripts/trainer.ipynb`. The model architecture is specified in the config.yaml file and you can play around with editing it. 
 - A simple demo of the workflow can be found at `scripts/demo.ipynb`.
```

#### html2text {}

```diff
@@ -1,19 +1,14 @@
-Metadata-Version: 2.1 Name: dflat_opt Version: 3.0.1 Summary: D-Flat is a
+Metadata-Version: 2.1 Name: dflat-opt Version: 3.1.0 Summary: D-Flat is a
 forward and inverse design framework for flat optics. Although specially geared
 for the design of metasurfaces, it may be used broadly for end-to-end imaging
 and sensing task. Home-page: https://github.com/DeanHazineh/DFlat Author: Dean
 Hazineh Author-email: dhazineh@g.harvard.edu Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Requires-Python: >=3.9
-Description-Content-Type: text/markdown Requires-Dist: pytest Requires-Dist:
-pytest-cov Requires-Dist: requests Requires-Dist: setuptools Requires-Dist:
-numpy Requires-Dist: scipy Requires-Dist: matplotlib Requires-Dist: moviepy
-Requires-Dist: pyhank Requires-Dist: einops Requires-Dist: tqdm Requires-Dist:
-pandas Requires-Dist: opencv-python Requires-Dist: gdspy Requires-Dist: mat73
-Requires-Dist: omegaconf Requires-Dist: natsort
+Description-Content-Type: text/markdown
                                     [Dflat]
                                     [Dflat]
 # An End-to-End Design Framework for Diffractive Optics and Metasurface-Based
 Vision Systems ![Python](https://img.shields.io/badge/python-3670A0?style=for-
 the-badge&logo=python&logoColor=ffdd54) ![PyTorch](https://img.shields.io/
 badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)]
@@ -43,19 +38,21 @@
 simply via: ``` pip install dflat_opt ``` You may also find it beneficial to
 work directly with the repository in editable mode via: ``` git clone https://
 github.com/DeanHazineh/DFlat pip install -e . ``` ## Version Notes (v3.0.0)
 Updated on April 11, 2024 | V2 -> V3 - Documentation is still in development :
 o - (v3) You can now donwload this package from the PyPi Index! - (v3) Datasets
 and pre-trained models are now downloaded when called insetad of during
 install. Models are now initialized by their name instead of by paths to config
-files. - (v2) This repository is the home for the new and maintained version of
-DFlat. It replaces DFlat-Tensorflow. - (v2) Note that this package is no longer
-a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in
-February 2024. - (v2) The structure of the software is completely revamped and
-the algorithms used--in particular for field propagation--are not the same as
+files. - (v3) Memory problems? Gradient checkpointing is added throughout
+reducing memory when using DFLat at the cost of slightly slower runtimes. -
+(v2) This repository is the home for the new and maintained version of DFlat.
+It replaces DFlat-Tensorflow. - (v2) Note that this package is no longer a
+direct port of pytorch-tensorflow but is a complete rewrite (re-)released in
+February 2024. I recommend switching! - (v2) The structure of the software is
+completely revamped and the algorithms used throughout are not the same as
 before. The original pytorch version (now deprecated) is archived and kept as a
 branch. ## Usage and Documentation Detailed documentation for the rewritten
 package and a new project page will be released in the future. For now, we
 highlight two resources for developers and researchers: - A script used to
 train neural models can be found in `scripts/trainer.ipynb`. The model
 architecture is specified in the config.yaml file and you can play around with
 editing it. - A simple demo of the workflow can be found at `scripts/
```

### Comparing `dflat_opt-3.0.1/dflat_opt.egg-info/SOURCES.txt` & `dflat_opt-3.1.0/dflat_opt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 dflat/metasurface/reverse_lookup.py
 dflat/metasurface/trainer.py
 dflat/plot_utilities/__init__.py
 dflat/plot_utilities/mp_format.py
 dflat/plot_utilities/vis.py
 dflat/propagation/__init__.py
 dflat/propagation/propagators.py
-dflat/propagation/psf.py
+dflat/propagation/propagators_legacy.py
 dflat/propagation/util.py
 dflat/radial_tranforms/__init__.py
 dflat/radial_tranforms/hankel_ops.py
 dflat/radial_tranforms/radial_ops.py
 dflat/render/__init__.py
 dflat/render/fft_convolve.py
 dflat/render/fronto_planar_renderer.py
@@ -50,9 +50,10 @@
 tests/test_hsi_to_rgb.py
 tests/test_initialize.py
 tests/test_metasurface_datasets.py
 tests/test_metasurface_loader.py
 tests/test_metasurface_reverse_lookup.py
 tests/test_metasurface_util.py
 tests/test_propagation.py
+tests/test_propagation_legacy.py
 tests/test_radial_transforms.py
 tests/test_render.py
```

### Comparing `dflat_opt-3.0.1/readme.md` & `dflat_opt-3.1.0/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,18 +40,19 @@
 ```
 
 ## Version Notes (v3.0.0)
 
 Updated on April 11, 2024 | V2 -> V3
 - Documentation is still in development :o 
 - (v3) You can now donwload this package from the PyPi Index!
-- (v3) Datasets and pre-trained models are now downloaded when called insetad of during install. Models are now initialized by their name instead of by paths to config files. 
+- (v3) Datasets and pre-trained models are now downloaded when called insetad of during install. Models are now initialized by their name instead of by paths to config files.
+- (v3) Memory problems? Gradient checkpointing is added throughout reducing memory when using DFLat at the cost of slightly slower runtimes. 
 - (v2) This repository is the home for the new and maintained version of DFlat. It replaces DFlat-Tensorflow.
-- (v2) Note that this package is no longer a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in February 2024.
-- (v2) The structure of the software is completely revamped and the algorithms used--in particular for field propagation--are not the same as before. The original pytorch version (now deprecated) is archived and kept as a branch.
+- (v2) Note that this package is no longer a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in February 2024. I recommend switching!
+- (v2) The structure of the software is completely revamped and the algorithms used throughout are not the same as before. The original pytorch version (now deprecated) is archived and kept as a branch.
 
 ## Usage and Documentation
 
 Detailed documentation for the rewritten package and a new project page will be released in the future. For now, we highlight two resources for developers and researchers:
 - A script used to train neural models can be found in `scripts/trainer.ipynb`. The model architecture is specified in the config.yaml file and you can play around with editing it. 
 - A simple demo of the workflow can be found at `scripts/demo.ipynb`.
```

#### html2text {}

```diff
@@ -31,19 +31,21 @@
 simply via: ``` pip install dflat_opt ``` You may also find it beneficial to
 work directly with the repository in editable mode via: ``` git clone https://
 github.com/DeanHazineh/DFlat pip install -e . ``` ## Version Notes (v3.0.0)
 Updated on April 11, 2024 | V2 -> V3 - Documentation is still in development :
 o - (v3) You can now donwload this package from the PyPi Index! - (v3) Datasets
 and pre-trained models are now downloaded when called insetad of during
 install. Models are now initialized by their name instead of by paths to config
-files. - (v2) This repository is the home for the new and maintained version of
-DFlat. It replaces DFlat-Tensorflow. - (v2) Note that this package is no longer
-a direct port of pytorch-tensorflow but is a complete rewrite (re-)released in
-February 2024. - (v2) The structure of the software is completely revamped and
-the algorithms used--in particular for field propagation--are not the same as
+files. - (v3) Memory problems? Gradient checkpointing is added throughout
+reducing memory when using DFLat at the cost of slightly slower runtimes. -
+(v2) This repository is the home for the new and maintained version of DFlat.
+It replaces DFlat-Tensorflow. - (v2) Note that this package is no longer a
+direct port of pytorch-tensorflow but is a complete rewrite (re-)released in
+February 2024. I recommend switching! - (v2) The structure of the software is
+completely revamped and the algorithms used throughout are not the same as
 before. The original pytorch version (now deprecated) is archived and kept as a
 branch. ## Usage and Documentation Detailed documentation for the rewritten
 package and a new project page will be released in the future. For now, we
 highlight two resources for developers and researchers: - A script used to
 train neural models can be found in `scripts/trainer.ipynb`. The model
 architecture is specified in the config.yaml file and you can play around with
 editing it. - A simple demo of the workflow can be found at `scripts/
```

### Comparing `dflat_opt-3.0.1/setup.cfg` & `dflat_opt-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dflat_opt
-version = 3.0.1
+version = 3.1.0
 author = Dean Hazineh
 author_email = dhazineh@g.harvard.edu
 description = D-Flat is a forward and inverse design framework for flat optics. Although specially geared for the design of metasurfaces, it may be used broadly for end-to-end imaging and sensing task.
 long_description_content_type = text/markdown
 long_description = file: readme.md
 url = https://github.com/DeanHazineh/DFlat
 classifiers =
```

### Comparing `dflat_opt-3.0.1/tests/test_fourier_convolution.py` & `dflat_opt-3.1.0/tests/test_fourier_convolution.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/tests/test_hsi_to_rgb.py` & `dflat_opt-3.1.0/tests/test_hsi_to_rgb.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/tests/test_initialize.py` & `dflat_opt-3.1.0/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/tests/test_metasurface_datasets.py` & `dflat_opt-3.1.0/tests/test_metasurface_datasets.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/tests/test_metasurface_loader.py` & `dflat_opt-3.1.0/tests/test_metasurface_loader.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/tests/test_metasurface_reverse_lookup.py` & `dflat_opt-3.1.0/tests/test_metasurface_reverse_lookup.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/tests/test_radial_transforms.py` & `dflat_opt-3.1.0/tests/test_radial_transforms.py`

 * *Files identical despite different names*

### Comparing `dflat_opt-3.0.1/tests/test_render.py` & `dflat_opt-3.1.0/tests/test_render.py`

 * *Files identical despite different names*

