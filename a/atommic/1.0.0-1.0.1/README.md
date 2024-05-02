# Comparing `tmp/atommic-1.0.0.tar.gz` & `tmp/atommic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atommic-1.0.0.tar", last modified: Mon Apr  8 06:38:47 2024, max compression
+gzip compressed data, was "atommic-1.0.1.tar", last modified: Thu May  2 08:55:08 2024, max compression
```

## Comparing `atommic-1.0.0.tar` & `atommic-1.0.1.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:47.224858 atommic-1.0.0/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11558 2024-04-08 01:02:32.000000 atommic-1.0.0/LICENSE
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    13249 2024-04-08 06:38:47.224858 atommic-1.0.0/PKG-INFO
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    12046 2024-04-08 01:02:32.000000 atommic-1.0.0/README.md
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.277541 atommic-1.0.0/atommic/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      347 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.511915 atommic-1.0.0/atommic/cli/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      539 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/cli/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     7710 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/cli/launch.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.558793 atommic-1.0.0/atommic/collections/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.590040 atommic-1.0.0/atommic/collections/common/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      412 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.730666 atommic-1.0.0/atommic/collections/common/callbacks/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      222 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/callbacks/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2487 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/callbacks/callbacks.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    17805 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/callbacks/ema.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.855824 atommic-1.0.0/atommic/collections/common/data/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      396 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/data/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    17752 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/data/mri_loader.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    38150 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/data/subsample.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.980912 atommic-1.0.0/atommic/collections/common/losses/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      372 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/losses/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2276 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/losses/aggregator.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4171 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/losses/wasserstein.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.059149 atommic-1.0.0/atommic/collections/common/metrics/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      168 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/metrics/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3694 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/metrics/global_average_loss_metric.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.137272 atommic-1.0.0/atommic/collections/common/nn/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/nn/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    17807 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/nn/base.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.387416 atommic-1.0.0/atommic/collections/common/parts/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      513 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/parts/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     9818 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/parts/coil_sensitivity_maps.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    10427 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/parts/fft.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      299 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/parts/patch_utils.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)   136845 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/parts/transforms.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    36656 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/common/parts/utils.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.434292 atommic-1.0.0/atommic/collections/motioncorrection/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      348 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/motioncorrection/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.528045 atommic-1.0.0/atommic/collections/motioncorrection/parts/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      159 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/motioncorrection/parts/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    16013 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/motioncorrection/parts/motionsimulation.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.574914 atommic-1.0.0/atommic/collections/multitask/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      339 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.606172 atommic-1.0.0/atommic/collections/multitask/rs/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      409 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:38.699916 atommic-1.0.0/atommic/collections/multitask/rs/data/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      146 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/data/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    26458 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/data/mrirs_loader.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:39.137777 atommic-1.0.0/atommic/collections/multitask/rs/nn/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      628 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    92626 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/base.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    10663 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:39.278497 atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11260 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr_base/idslr_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8296 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr_unet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    15616 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/mtlrs.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:39.403645 atommic-1.0.0/atommic/collections/multitask/rs/nn/mtlrs_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/mtlrs_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    16530 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/mtlrs_base/mtlrs_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6686 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/recseg_unet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    12894 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/segnet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    12325 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:39.638116 atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     9270 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/convlstm.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5130 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/convlstm_unet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    13998 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/seranet_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:39.747489 atommic-1.0.0/atommic/collections/multitask/rs/parts/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      152 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/parts/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    63022 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/multitask/rs/parts/transforms.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:39.794364 atommic-1.0.0/atommic/collections/quantitative/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      368 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:39.872492 atommic-1.0.0/atommic/collections/quantitative/data/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      162 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/data/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    13884 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/data/qmri_loader.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.106864 atommic-1.0.0/atommic/collections/quantitative/nn/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      211 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)   123035 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/base.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    24860 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qcirim.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.278740 atommic-1.0.0/atommic/collections/quantitative/nn/qrim_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qrim_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     9569 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qrim_base/qrim_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5666 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qrim_base/utils.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11613 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qvarnet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.389391 atommic-1.0.0/atommic/collections/quantitative/nn/qvarnet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qvarnet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5698 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qvarnet_base/qvarnet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4319 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/nn/qzf.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.498764 atommic-1.0.0/atommic/collections/quantitative/parts/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      151 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/parts/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    94718 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/quantitative/parts/transforms.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.545638 atommic-1.0.0/atommic/collections/reconstruction/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      376 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.623766 atommic-1.0.0/atommic/collections/reconstruction/data/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      301 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/data/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    38110 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/data/mri_reconstruction_loader.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.752942 atommic-1.0.0/atommic/collections/reconstruction/losses/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      225 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/losses/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1808 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/losses/na.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3033 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/losses/ssim.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:40.826976 atommic-1.0.0/atommic/collections/reconstruction/metrics/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      170 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/metrics/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8982 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/metrics/reconstruction_metrics.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:41.592989 atommic-1.0.0/atommic/collections/reconstruction/nn/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1359 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    67401 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/base.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3853 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/ccnn.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:41.671115 atommic-1.0.0/atommic/collections/reconstruction/nn/ccnn_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/ccnn_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6582 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/ccnn_base/ccnn_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11959 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/cirim.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    10530 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/crnn.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:41.780891 atommic-1.0.0/atommic/collections/reconstruction/nn/crnn_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/crnn_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     9697 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/crnn_base/crnn_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:41.893175 atommic-1.0.0/atommic/collections/reconstruction/nn/crossdomain_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/crossdomain_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    13884 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/crossdomain_base/crossdomain_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:41.970738 atommic-1.0.0/atommic/collections/reconstruction/nn/didn_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/didn_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    12284 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/didn_base/didn_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5875 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/dunet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11777 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/jointicnet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8588 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/kikinet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8712 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/lpd.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4130 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/modl.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:42.064488 atommic-1.0.0/atommic/collections/reconstruction/nn/modl_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/modl_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8547 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/modl_base/modl_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4457 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/multidomainnet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:42.174088 atommic-1.0.0/atommic/collections/reconstruction/nn/multidomainnet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/multidomainnet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    18300 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/multidomainnet_base/multidomainnet_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:42.283463 atommic-1.0.0/atommic/collections/reconstruction/nn/mwcnn_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/mwcnn_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    15425 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/mwcnn_base/mwcnn_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:42.377358 atommic-1.0.0/atommic/collections/reconstruction/nn/primaldualnet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/primaldualnet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3736 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/primaldualnet_base/primaldualnet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3244 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/proximal_gradient.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     7088 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/recurrentvarnet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:42.518339 atommic-1.0.0/atommic/collections/reconstruction/nn/recurrentvarnet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/recurrentvarnet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    15004 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/recurrentvarnet_base/recurrentvarnet_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:42.768453 atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5036 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/conv_layers.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    12115 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/rim_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3002 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/rim_utils.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    17337 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/rnn_cells.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:42.940288 atommic-1.0.0/atommic/collections/reconstruction/nn/sigmanet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/sigmanet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    21030 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/sigmanet_base/dc_layers.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11676 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/sigmanet_base/sensitivity_net.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3342 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/unet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.034039 atommic-1.0.0/atommic/collections/reconstruction/nn/unet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/unet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11833 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/unet_base/unet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4210 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/varnet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.143415 atommic-1.0.0/atommic/collections/reconstruction/nn/varnet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/varnet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4441 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/varnet_base/varnet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5949 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/vsnet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.237163 atommic-1.0.0/atommic/collections/reconstruction/nn/vsnet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/vsnet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6382 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/vsnet_base/vsnet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     9116 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/xpdnet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2628 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/nn/zf.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.346912 atommic-1.0.0/atommic/collections/reconstruction/parts/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      166 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/parts/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      421 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/reconstruction/parts/transforms.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.393787 atommic-1.0.0/atommic/collections/segmentation/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      365 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.487539 atommic-1.0.0/atommic/collections/segmentation/data/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      314 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/data/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    62170 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/data/mri_segmentation_loader.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.659453 atommic-1.0.0/atommic/collections/segmentation/losses/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      230 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/losses/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2941 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/losses/cross_entropy.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    10530 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/losses/dice.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2738 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/losses/utils.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:43.737677 atommic-1.0.0/atommic/collections/segmentation/metrics/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      400 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/metrics/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    28604 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/metrics/segmentation_metrics.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:44.239245 atommic-1.0.0/atommic/collections/segmentation/nn/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      692 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1575 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/attentionunet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:44.316796 atommic-1.0.0/atommic/collections/segmentation/nn/attentionunet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/attentionunet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6724 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/attentionunet_base/attentionunet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    44547 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/base.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4314 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/dynunet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:44.410549 atommic-1.0.0/atommic/collections/segmentation/nn/dynunet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/dynunet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    20505 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/dynunet_base/dynunet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3830 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/lambdaunet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:44.504295 atommic-1.0.0/atommic/collections/segmentation/nn/lambdaunet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/lambdaunet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    12346 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/lambdaunet_base/lambdaunet_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5968 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/segmentationnet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1510 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/unet.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3396 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/unet3d.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:44.613681 atommic-1.0.0/atommic/collections/segmentation/nn/unet3d_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/unet3d_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6063 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/unet3d_base/unet3d_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4273 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/unetr.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:44.738643 atommic-1.0.0/atommic/collections/segmentation/nn/unetr_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/unetr_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    30144 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/unetr_base/unetr_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.035592 atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    10007 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/patchembedding.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8049 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/transformer_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    14490 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/utils.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4831 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/vit_block.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3711 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vnet.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.129457 atommic-1.0.0/atommic/collections/segmentation/nn/vnet_base/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vnet_base/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    10810 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/nn/vnet_base/vnet_block.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.207916 atommic-1.0.0/atommic/collections/segmentation/parts/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      162 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/parts/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      421 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/collections/segmentation/parts/transforms.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      752 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/constants.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.249743 atommic-1.0.0/atommic/core/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      147 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/__init__.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.442767 atommic-1.0.0/atommic/core/classes/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/classes/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    45287 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/classes/common.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3155 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/classes/dataset.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    12637 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/classes/export.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      413 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/classes/loss.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    77454 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/classes/modelPT.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.661581 atommic-1.0.0/atommic/core/conf/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/conf/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5333 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/conf/hydra_runner.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     7517 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/conf/modelPT.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8321 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/conf/optimizers.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6448 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/conf/schedulers.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2016 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/conf/trainer.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.739704 atommic-1.0.0/atommic/core/connectors/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/connectors/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    30048 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/connectors/save_restore_connector.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:45.911579 atommic-1.0.0/atommic/core/neural_types/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/neural_types/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3610 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/neural_types/axes.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      784 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/neural_types/comparison.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3774 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/neural_types/elements.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     9793 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/neural_types/neural_type.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:46.193264 atommic-1.0.0/atommic/core/optim/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     8924 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/adafactor.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3019 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/lion.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    47954 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/lr_scheduler.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5728 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/novograd.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    23726 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/optimizer_with_main_params.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6819 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/optimizers.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4366 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/optim/radam.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:46.287015 atommic-1.0.0/atommic/core/utils/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/utils/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1502 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/utils/neural_type_utils.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     6683 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/utils/numba_utils.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:46.365141 atommic-1.0.0/atommic/core/utils/process_launcher/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/utils/process_launcher/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    15965 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/core/utils/process_launcher/launcher.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      873 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/package_info.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:46.756110 atommic-1.0.0/atommic/utils/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      313 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    13915 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/app_state.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    17816 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/atommic_logging.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:46.849861 atommic-1.0.0/atommic/utils/callbacks/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      235 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/callbacks/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    15488 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/callbacks/atommic_model_checkpoint.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5830 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/callbacks/preemption.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1036 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/cast_utils.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:47.037361 atommic-1.0.0/atommic/utils/decorators/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/decorators/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2642 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/decorators/deprecated.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      902 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/decorators/experimental.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     3463 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/decorators/port_docs.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5858 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/env_var_parsing.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      292 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/exceptions.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    48645 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/exp_manager.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     9646 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/export_utils.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:47.162364 atommic-1.0.0/atommic/utils/formaters/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       53 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/formaters/__init__.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     5366 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/formaters/base.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1162 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/formaters/colors.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1359 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/formaters/utils.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1244 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/get_rank.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2254 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/lightning_logger_patch.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1011 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/metaclasses.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    24406 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/model_utils.py
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     4277 2024-04-08 01:02:32.000000 atommic-1.0.0/atommic/utils/timers.py
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:37.449416 atommic-1.0.0/atommic.egg-info/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    13249 2024-04-08 06:38:32.000000 atommic-1.0.0/atommic.egg-info/PKG-INFO
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)    11081 2024-04-08 06:38:36.000000 atommic-1.0.0/atommic.egg-info/SOURCES.txt
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)        1 2024-04-08 06:38:32.000000 atommic-1.0.0/atommic.egg-info/dependency_links.txt
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)       45 2024-04-08 06:38:32.000000 atommic-1.0.0/atommic.egg-info/entry_points.txt
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)        1 2024-04-08 06:38:32.000000 atommic-1.0.0/atommic.egg-info/not-zip-safe
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      388 2024-04-08 06:38:32.000000 atommic-1.0.0/atommic.egg-info/requires.txt
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)        8 2024-04-08 06:38:32.000000 atommic-1.0.0/atommic.egg-info/top_level.txt
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     2560 2024-04-08 01:02:33.000000 atommic-1.0.0/pyproject.toml
-drwxrwxrwx   0 wdika     (1000) wdika     (1000)        0 2024-04-08 06:38:47.193610 atommic-1.0.0/requirements/
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)      412 2024-04-08 01:02:33.000000 atommic-1.0.0/requirements/requirements.txt
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     1177 2024-04-08 06:38:47.224858 atommic-1.0.0/setup.cfg
--rwxrwxrwx   0 wdika     (1000) wdika     (1000)     7305 2024-04-08 01:02:33.000000 atommic-1.0.0/setup.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.105577 atommic-1.0.1/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11558 2024-04-29 15:46:39.000000 atommic-1.0.1/LICENSE
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    16179 2024-05-02 08:55:08.105577 atommic-1.0.1/PKG-INFO
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    14996 2024-05-02 08:41:46.000000 atommic-1.0.1/README.md
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.015577 atommic-1.0.1/atommic/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      347 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/cli/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      539 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/cli/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     7710 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/cli/launch.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/common/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      412 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/common/callbacks/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      222 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/callbacks/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2487 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/callbacks/callbacks.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    17805 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/callbacks/ema.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/common/data/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      396 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/data/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    17752 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/data/mri_loader.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    38150 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/data/subsample.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/common/losses/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      372 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/losses/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2276 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/losses/aggregator.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4171 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/losses/wasserstein.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/common/metrics/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      168 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/metrics/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3694 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/metrics/global_average_loss_metric.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/common/nn/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/nn/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    17807 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/nn/base.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/common/parts/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      513 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/parts/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     9818 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/parts/coil_sensitivity_maps.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    10427 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/parts/fft.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      299 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/parts/patch_utils.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)   136845 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/parts/transforms.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    36656 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/common/parts/utils.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.025577 atommic-1.0.1/atommic/collections/motioncorrection/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      348 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/motioncorrection/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/motioncorrection/parts/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      159 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/motioncorrection/parts/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    16013 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/motioncorrection/parts/motionsimulation.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      339 2024-04-29 15:46:39.000000 atommic-1.0.1/atommic/collections/multitask/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/rs/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      409 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/rs/data/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      146 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/data/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    26458 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/data/mrirs_loader.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/rs/nn/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      628 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    92626 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/base.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    10663 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11260 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr_base/idslr_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8296 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr_unet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    15616 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/mtlrs.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/rs/nn/mtlrs_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/mtlrs_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    16530 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/mtlrs_base/mtlrs_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6686 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/recseg_unet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    12894 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/segnet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    12325 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     9270 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/convlstm.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5130 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/convlstm_unet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    13998 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/seranet_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/multitask/rs/parts/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      152 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/parts/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    63022 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/multitask/rs/parts/transforms.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/quantitative/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      368 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.035577 atommic-1.0.1/atommic/collections/quantitative/data/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      162 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/data/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    13884 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/data/qmri_loader.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/quantitative/nn/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      211 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)   123035 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/base.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    24860 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qcirim.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/quantitative/nn/qrim_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qrim_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     9569 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qrim_base/qrim_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5666 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qrim_base/utils.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11613 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qvarnet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/quantitative/nn/qvarnet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qvarnet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5698 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qvarnet_base/qvarnet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4319 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/nn/qzf.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/quantitative/parts/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      151 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/parts/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    94718 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/quantitative/parts/transforms.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/reconstruction/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      376 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/reconstruction/data/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      301 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/data/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    38110 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/data/mri_reconstruction_loader.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/reconstruction/losses/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      225 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/losses/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1808 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/losses/na.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3033 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/losses/ssim.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.045577 atommic-1.0.1/atommic/collections/reconstruction/metrics/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      170 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/metrics/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8982 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/metrics/reconstruction_metrics.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.055577 atommic-1.0.1/atommic/collections/reconstruction/nn/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1359 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    67401 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/base.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3853 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/ccnn.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.055577 atommic-1.0.1/atommic/collections/reconstruction/nn/ccnn_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/ccnn_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6582 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/ccnn_base/ccnn_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11959 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/cirim.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    10530 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/crnn.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.055577 atommic-1.0.1/atommic/collections/reconstruction/nn/crnn_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/crnn_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     9697 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/crnn_base/crnn_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.055577 atommic-1.0.1/atommic/collections/reconstruction/nn/crossdomain_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/crossdomain_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    13884 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/crossdomain_base/crossdomain_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.055577 atommic-1.0.1/atommic/collections/reconstruction/nn/didn_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/didn_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    12284 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/didn_base/didn_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5875 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/dunet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11777 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/jointicnet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8588 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/kikinet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8712 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/lpd.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4130 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/modl.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/modl_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/modl_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8547 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/modl_base/modl_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4457 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/multidomainnet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/multidomainnet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/multidomainnet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    18300 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/multidomainnet_base/multidomainnet_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/mwcnn_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/mwcnn_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    15425 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/mwcnn_base/mwcnn_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/primaldualnet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/primaldualnet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3736 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/primaldualnet_base/primaldualnet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3244 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/proximal_gradient.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     7088 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/recurrentvarnet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/recurrentvarnet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/recurrentvarnet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    15004 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/recurrentvarnet_base/recurrentvarnet_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5036 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/conv_layers.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    12115 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/rim_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3002 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/rim_utils.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    17337 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/rnn_cells.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/sigmanet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/sigmanet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    21030 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/sigmanet_base/dc_layers.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11676 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/sigmanet_base/sensitivity_net.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3342 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/unet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/unet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/unet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11833 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/unet_base/unet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4210 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/varnet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/varnet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/varnet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4441 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/varnet_base/varnet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5949 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/vsnet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/nn/vsnet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/vsnet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6382 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/vsnet_base/vsnet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     9116 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/xpdnet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2628 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/nn/zf.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/reconstruction/parts/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      166 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/parts/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      421 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/reconstruction/parts/transforms.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.065577 atommic-1.0.1/atommic/collections/segmentation/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      365 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/data/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      314 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/data/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    62170 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/data/mri_segmentation_loader.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/losses/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      230 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/losses/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2941 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/losses/cross_entropy.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    10530 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/losses/dice.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2738 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/losses/utils.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/metrics/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      400 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/metrics/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    28604 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/metrics/segmentation_metrics.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/nn/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      692 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1575 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/attentionunet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/nn/attentionunet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/attentionunet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6724 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/attentionunet_base/attentionunet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    44547 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/base.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4314 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/dynunet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/nn/dynunet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/dynunet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    20505 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/dynunet_base/dynunet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3830 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/lambdaunet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/nn/lambdaunet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/lambdaunet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    12346 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/lambdaunet_base/lambdaunet_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5968 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/segmentationnet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1510 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/unet.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3396 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/unet3d.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/nn/unet3d_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/unet3d_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6063 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/unet3d_base/unet3d_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4273 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/unetr.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.075577 atommic-1.0.1/atommic/collections/segmentation/nn/unetr_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/unetr_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    30144 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/unetr_base/unetr_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.085577 atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    10007 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/patchembedding.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8049 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/transformer_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    14490 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/utils.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4831 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/vit_block.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3711 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vnet.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.085577 atommic-1.0.1/atommic/collections/segmentation/nn/vnet_base/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vnet_base/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    10810 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/nn/vnet_base/vnet_block.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.085577 atommic-1.0.1/atommic/collections/segmentation/parts/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      162 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/parts/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      421 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/collections/segmentation/parts/transforms.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      752 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/constants.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.085577 atommic-1.0.1/atommic/core/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      147 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/__init__.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.085577 atommic-1.0.1/atommic/core/classes/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/classes/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    45287 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/classes/common.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3155 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/classes/dataset.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    12637 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/classes/export.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      413 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/classes/loss.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    77454 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/classes/modelPT.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.085577 atommic-1.0.1/atommic/core/conf/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/conf/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5333 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/conf/hydra_runner.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     7517 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/conf/modelPT.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8321 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/conf/optimizers.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6448 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/conf/schedulers.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2016 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/conf/trainer.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.085577 atommic-1.0.1/atommic/core/connectors/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/connectors/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    30048 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/connectors/save_restore_connector.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.095577 atommic-1.0.1/atommic/core/neural_types/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:40.000000 atommic-1.0.1/atommic/core/neural_types/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3610 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/neural_types/axes.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      784 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/neural_types/comparison.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3774 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/neural_types/elements.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     9793 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/neural_types/neural_type.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.095577 atommic-1.0.1/atommic/core/optim/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     8924 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/adafactor.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3019 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/lion.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    47954 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/lr_scheduler.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5728 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/novograd.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    23726 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/optimizer_with_main_params.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6819 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/optimizers.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4366 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/optim/radam.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.095577 atommic-1.0.1/atommic/core/utils/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/utils/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1502 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/utils/neural_type_utils.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     6683 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/utils/numba_utils.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.095577 atommic-1.0.1/atommic/core/utils/process_launcher/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/utils/process_launcher/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    15965 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/core/utils/process_launcher/launcher.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      873 2024-05-02 08:35:08.000000 atommic-1.0.1/atommic/package_info.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.105577 atommic-1.0.1/atommic/utils/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      313 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    13915 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/app_state.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    17816 2024-05-01 20:03:25.000000 atommic-1.0.1/atommic/utils/atommic_logging.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.105577 atommic-1.0.1/atommic/utils/callbacks/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      235 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/callbacks/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    15488 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/callbacks/atommic_model_checkpoint.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5830 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/callbacks/preemption.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1036 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/cast_utils.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.105577 atommic-1.0.1/atommic/utils/decorators/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/decorators/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2642 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/decorators/deprecated.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      902 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/decorators/experimental.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     3463 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/decorators/port_docs.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5858 2024-05-01 20:03:33.000000 atommic-1.0.1/atommic/utils/env_var_parsing.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      292 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/exceptions.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    48645 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/exp_manager.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     9646 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/export_utils.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.105577 atommic-1.0.1/atommic/utils/formaters/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       53 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/formaters/__init__.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     5366 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/formaters/base.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1162 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/formaters/colors.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1359 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/formaters/utils.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1244 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/get_rank.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2254 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/lightning_logger_patch.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1011 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/metaclasses.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    24406 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/model_utils.py
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     4277 2024-04-29 15:46:41.000000 atommic-1.0.1/atommic/utils/timers.py
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.015577 atommic-1.0.1/atommic.egg-info/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    16179 2024-05-02 08:55:07.000000 atommic-1.0.1/atommic.egg-info/PKG-INFO
+-rw-r--r--   0 wdika     (1000) wdika     (1000)    11081 2024-05-02 08:55:07.000000 atommic-1.0.1/atommic.egg-info/SOURCES.txt
+-rw-r--r--   0 wdika     (1000) wdika     (1000)        1 2024-05-02 08:55:07.000000 atommic-1.0.1/atommic.egg-info/dependency_links.txt
+-rw-r--r--   0 wdika     (1000) wdika     (1000)       45 2024-05-02 08:55:07.000000 atommic-1.0.1/atommic.egg-info/entry_points.txt
+-rw-r--r--   0 wdika     (1000) wdika     (1000)        1 2024-05-02 08:55:07.000000 atommic-1.0.1/atommic.egg-info/not-zip-safe
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      388 2024-05-02 08:55:07.000000 atommic-1.0.1/atommic.egg-info/requires.txt
+-rw-r--r--   0 wdika     (1000) wdika     (1000)        8 2024-05-02 08:55:07.000000 atommic-1.0.1/atommic.egg-info/top_level.txt
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     2560 2024-04-29 15:46:45.000000 atommic-1.0.1/pyproject.toml
+drwxr-xr-x   0 wdika     (1000) wdika     (1000)        0 2024-05-02 08:55:08.105577 atommic-1.0.1/requirements/
+-rw-r--r--   0 wdika     (1000) wdika     (1000)      412 2024-04-29 15:46:45.000000 atommic-1.0.1/requirements/requirements.txt
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     1177 2024-05-02 08:55:08.105577 atommic-1.0.1/setup.cfg
+-rw-r--r--   0 wdika     (1000) wdika     (1000)     7305 2024-04-29 15:46:45.000000 atommic-1.0.1/setup.py
```

### Comparing `atommic-1.0.0/LICENSE` & `atommic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/PKG-INFO` & `atommic-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atommic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)
 Home-page: https://github.com/wdika/atommic
 Download-URL: https://github.com/wdika/atommic/releases
 Author: Dimitris Karkalousos
 Author-email: d.karkalousos@amsterdamumc.nl
 Maintainer: Dimitris Karkalousos
 Maintainer-email: d.karkalousos@amsterdamumc.nl
@@ -27,89 +27,145 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10, <=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)
 [![HuggingFace](https://img.shields.io/badge/HuggingFace-Models-blue)](https://huggingface.co/wdika)
-[![GitHub issues](https://img.shields.io/github/issues/wdika/atommic)]()
+[![DockerHub](https://img.shields.io/badge/DockerHub-Link-blue)](docker.io/wdika/atommic)
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/atommic.svg)](https://badge.fury.io/py/atommic)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/atommic)](https://pypi.org/project/atommic/)
+[![GitHub issues](https://img.shields.io/github/issues/wdika/atommic)](https://github.com/wdika/atommic/issues)
+[![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atommic)](https://pypi.org/project/atommic/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]()
-<p align="center">
-    <img src="assets/atommic-logo.png" alt="Your Image" width="600" />
+<p align="center" style="margin-top: -40px; margin-bottom: -80px;">
+    <img src="assets/atommic-logo.png" alt="ATOMMIC-logo" width="600" />
 </p>
 
-# 👋 Introduction
+<div align="center">
+<span style="font-size:24px;">
+
+  [📜](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4801289)
+  [🤗](https://huggingface.co/wdika)
+  [🐳](docker.io/wdika/atommic)
+  [📦](https://pypi.org/project/atommic)
+  [📚](https://atommic.readthedocs.io/)
 
-The [Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)](https://github.com/wdika/atommic) is a
-toolbox for applying AI methods for **accelerated MRI reconstruction (REC)**, **MRI segmentation (SEG)**,
-**quantitative MR imaging (qMRI)**, as well as **multitask learning (MTL)**, i.e., performing multiple tasks
-simultaneously, such as reconstruction and segmentation. Each task is implemented in a separate collection, which
-consists of data loaders, transformations, models, metrics, and losses. **ATOMMIC** is designed to be modular and
-extensible, and it is easy to add new tasks, models, and datasets. **ATOMMIC** uses
-[PyTorch Lightning](https://www.pytorchlightning.ai/) for feasible high-performance multi-GPU/multi-node
-mixed-precision training.
+</div>
+
+## 👋 Introduction
+
+The [Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)](https://github.com/wdika/atommic) is a toolbox for applying AI methods for **accelerated MRI reconstruction (REC)**, **MRI segmentation (SEG)**, **quantitative MR imaging (qMRI)**, as well as **multitask learning (MTL)**, i.e., performing multiple tasks simultaneously, such as reconstruction and segmentation. Each task is implemented in a separate collection consisting of data loaders, transformations, models, metrics, and losses. **ATOMMIC** is designed to be modular and extensible on new tasks, models, and datasets. **ATOMMIC** uses [PyTorch Lightning](https://www.pytorchlightning.ai/) for feasible high-performance multi-GPU/multi-node mixed-precision training.
 
 ![ATOMMIC Schematic Overview](assets/atommic-schematic_overview.png)
 
-The schematic overview of **ATOMMIC** showcases the main components of the toolbox. First, we need an [MRI Dataset](README.md#mri-datasets) (e.g., **CC359**). Next, we need to define the high-level parameters, such as the [task and the model](../mri/collections.html), the [undersampling](../mri/undersampling.html), the [transforms](../mri/transforms.html), the [optimizer](../core/core.html#optimization), the [scheduler](../core/core.html#learning-rate-schedulers), the [loss](../mri/losses.html), the [trainer parameters](../core/core.html#training), and the [experiment manager](../core/exp_manager.html). All these parameters are defined in a `.yaml` file using [Hydra](https://hydra.cc/) and [OmegaConf](https://omegaconf.readthedocs.io/).
+The schematic overview of **ATOMMIC** showcases the main components of the toolbox. First, we need an [MRI Dataset](README.md#mri-datasets) (e.g., **CC359**). Next, we need to define the high-level parameters, such as the [task and the model](https://atommic.readthedocs.io/en/latest/mri/collections.html), the [undersampling](https://atommic.readthedocs.io/en/latest/mri//undersampling.html), the [transforms](https://atommic.readthedocs.io/en/latest/mri//transforms.html), the [optimizer](https://atommic.readthedocs.io/en/latest/core/core.html#optimization), the [scheduler](https://atommic.readthedocs.io/en/latest/core/core.html#learning-rate-schedulers), the [loss](https://atommic.readthedocs.io/en/latest/mri/losses.html), the [trainer parameters](https://atommic.readthedocs.io/en/latest/core/core.html#training), and the [experiment manager](https://atommic.readthedocs.io/en/latest/core/exp_manager.html). All these parameters are defined in a `.yaml` file using [Hydra](https://hydra.cc/) and [OmegaConf](https://omegaconf.readthedocs.io/).
+
+The trained model is an `.atommic` [module](https://atommic.readthedocs.io/en/latest/core/export.html), exported with [ONNX](https://onnx.ai/) and [TorchScript](https://pytorch.org/docs/stable/jit.html) support, which can be used for inference. The `.atommic` module can also be uploaded on [HuggingFace](https://huggingface.co/). Pretrained models are available on our [HF](https://huggingface.co/wdika) account and can be downloaded and used for inference.
+
+## 🛠️ Installation
+
+**ATOMMIC** is best to be installed in a Conda environment.
+
+### 🐍 Conda
+```
+conda create -n atommic python=3.10
+conda activate atommic
+```
+
+### 📦 Pip
+Use this installation mode if you want the latest released version.
+
+```bash
+pip install atommic
+```
+
+### From source
+
+Use this installation mode if you are contributing to atommic.
+
+```bash
+git clone https://github.com/wdika/atommic
+cd atommic
+bash ./reinstall.sh
+```
+
+### 🐳 Docker containers
 
-The trained model is an `.atommic` [module](../core/export.html), exported with [ONNX](https://onnx.ai/) and [TorchScript](https://pytorch.org/docs/stable/jit.html) support, which can be used for inference. The `.atommic` module can also be uploaded on [HuggingFace](https://huggingface.co/). Pretrained models are available on our [HF](https://huggingface.co/wdika) account and can be downloaded and used for inference.
+An atommic container is available at dockerhub, you can pull it with:
+```bash
+docker pull wdika/atommic
+```
+
+You can also build an atommic container with:
+```bash
+DOCKER_BUILDKIT=1 docker build -f Dockerfile -t atommic:latest .
+```
+
+You can run the container with:
+```bash
+docker run --gpus all -it --rm -v /home/user/configs:/config atommic:latest atommic run -c /config/config.yaml
+```
+where ```/config/config.yaml``` is the path to your local configuration file.
+
+Or you can run it interactively with:
+```bash
+docker run --gpus all -it --rm -p 8888:8888 atommic:latest /bin/bash -c "./start-jupyter.sh"
+```
 
 ## 🚀 Quick Start Guide
 
-The best way to get started with ATOMMIC is to start with one of the [tutorials](tutorials.html):
+The best way to get started with ATOMMIC is with one of the [tutorials](https://atommic.readthedocs.io/en/latest/starthere/tutorials.html):
+
+- [ATOMMIC Primer](https://github.com/wdika/atommic/blob/main/tutorials/00_ATOMMIC_Primer.ipynb) - demonstrates how to use ATOMMIC.
+- [ATOMMIC MRI transforms](https://github.com/wdika/atommic/blob/main/tutorials/01_ATOMMIC_MRI_transforms.ipynb) - demonstrates how to use ATOMMIC to undersample MRI data.
+- [ATOMMIC MRI undersampling](https://github.com/wdika/atommic/blob/main/tutorials/02_ATOMMIC_MRI_undersampling.ipynb) - demonstrates how to use ATOMMIC to apply transforms to MRI data.
+- [ATOMMIC Upload Model on HuggingFace](https://github.com/wdika/atommic/blob/main/tutorials/03_ATOMMIC_Upload_Model_On_HF.ipynb) - demonstrates how to upload a model on HuggingFace.
 
-- [ATOMMIC Primer](https://github.com/wdika/atommic/tutorials/00_ATOMMIC_Primer.ipynb) - demonstrates how to use ATOMMIC.
-- [ATOMMIC MRI transforms](https://github.com/wdika/atommic/tutorials/01_ATOMMIC_MRI_transforms.ipynb) - demonstrates how to use ATOMMIC to undersample MRI data.
-- [ATOMMIC MRI undersampling](https://github.com/wdika/atommic/tutorials/02_ATOMMIC_MRI_undersampling.ipynb) - demonstrates how to use ATOMMIC to apply transforms to MRI data.
-- [ATOMMIC Upload Model on HuggingFace](https://github.com/wdika/atommic/tutorials/03_ATOMMIC_Upload_Model_On_HF.ipynb) - demonstrates how to upload a model on HuggingFace.
+You can also check the [projects](https://github.com/wdika/atommic/tree/main/projects) page to see how to use ATOMMIC for specific tasks and public datasets.
 
-You can also check the [projects](projects.html) page to see how to use ATOMMIC for specific tasks and public datasets.
+Pre-trained models are available on HuggingFace [🤗](https://huggingface.co/wdika).
 
-### **ATOMMIC paper is fully reproducible. Please check [here](projects/ATOMMIC_paper/README.md) for more information.**
+### **ATOMMIC paper is fully reproducible. Please check [here](https://github.com/wdika/atommic/tree/main/projects/ATOMMIC_paper/README.md) for more information.**
 
 ## 🤖 Training & Testing
 
-Training and testing models in **ATOMMIC** is intuitive and easy. You just need to properly configure the `.yaml`
-file and just run the following command:
+Training and testing models in **ATOMMIC** is intuitive and easy. You just need to properly configure a `.yaml` file and run the following command:
 
 ```bash
 atommic run -c path-to-config-file
 ```
 
 ## ⚙️ Configuration
 
-1. Choose the **task** and the **model**, according to the [collections](../mri/collections.html).
+1. Choose the **task** and the **model**, according to the [collections](https://atommic.readthedocs.io/en/latest/mri/collections.html).
 
 2. Choose the **dataset** and the **dataset parameters**, according to the [datasets](README.md#mri-datasets) or your own dataset.
 
-3. Choose the [undersampling](../mri/transforms.html).
+3. Choose the [undersampling](https://atommic.readthedocs.io/en/latest/mri/transforms.html).
 
-4. Choose the [transforms](../mri/transforms.html).
+4. Choose the [transforms](https://atommic.readthedocs.io/en/latest/mri/transforms.html).
 
-5. Choose the [losses](../mri/losses.html).
+5. Choose the [losses](https://atommic.readthedocs.io/en/latest/mri/losses.html).
 
-6. Choose the [optimizer](../core/core.html#optimization).
+6. Choose the [optimizer](https://atommic.readthedocs.io/en/latest/core/core.html#optimization).
 
-7. Choose the [scheduler](../core/core.html#learning-rate-schedulers).
+7. Choose the [scheduler](https://atommic.readthedocs.io/en/latest/core/core.html#learning-rate-schedulers).
 
-8. Choose the [trainer parameters](../core/core.html#training).
+8. Choose the [trainer parameters](https://atommic.readthedocs.io/en/latest/core/core.html#training).
 
-9. Choose the [experiment manager](../core/exp_manager.html).
+9. Choose the [experiment manager](https://atommic.readthedocs.io/en/latest/core/exp_manager.html).
 
-You can also check the [projects](projects.html) page to see how to configure the `.yaml` file for specific tasks.
+You can also check the [projects](https://github.com/wdika/atommic/tree/main/projects/) page to see how to configure the `.yaml` file for specific tasks.
 
 ## 🗂️ Collections
 
-**ATOMMIC** is organized into [collections](../mri/collections.html), each of which implements a specific task. The following collections are currently available, implementing various models as listed:
+**ATOMMIC** is organized into [collections](https://atommic.readthedocs.io/en/latest/mri/collections.html), each of which implements a specific task. The following collections are currently available, implementing various models as listed:
 
 ### MultiTask Learning (MTL)
 1. End-to-End Recurrent Attention Network (`SERANet`), 2. Image domain Deep Structured Low-Rank Network (`IDSLR`), 3. Image domain Deep Structured Low-Rank UNet (`IDSLRUNet`), 4. Multi-Task Learning for MRI Reconstruction and Segmentation (`MTLRS`), 5. Reconstruction Segmentation method using UNet (`RecSegUNet`), 6. Segmentation Network MRI (`SegNet`).
 
 ### Quantitative MR Imaging (qMRI)
 1. Quantitative Recurrent Inference Machines (`qRIMBlock`), 2. Quantitative End-to-End Variational Network (`qVarNet`), 3. Quantitative Cascades of Independently Recurrent Inference Machines (`qCIRIM`).
 
@@ -119,100 +175,64 @@
 ### MRI Segmentation (SEG)
 1. `SegmentationAttentionUNet`, 2. `SegmentationDYNUNet`, 3. `SegmentationLambdaUNet`, 4. `SegmentationUNet`, 5. `Segmentation3DUNet`, 6. `SegmentationUNetR`, 7. `SegmentationVNet`.
 
 ## MRI Datasets
 
 **ATOMMIC** supports public datasets, as well as private datasets. The following public datasets are supported natively:
 
-- [AHEAD](projects/MTL/ahead.html): Supports the `(qMRI)` and `(REC)` tasks.
-- [BraTS 2023 Adult Glioma](projects/SEG/brats2023adultglioma.html): Supports the `(SEG)` task.
-- [CC359](projects/REC/cc359.html): Supports the `(REC)` task.
-- [fastMRI Brains Multicoil](projects/REC/fastmribrainsmulticoil.html): Supports the `(REC)` task.
-- [fastMRI Knees Multicoil](projects/REC/fastmrikneesmulticoil.html): Supports the `(REC)` task.
-- [fastMRI Knees Singlecoil](projects/REC/fastmrikneessinglecoil.html): Supports the `(REC)` task.
-- [ISLES 2022 Sub Acute Stroke](projects/SEG/isles2022subacutestroke.html): Supports the `(SEG)` task.
-- [SKM-TEA](projects/REC/skmtea.html): Supports the `(REC)`, `(SEG)`, and `(MTL)` tasks.
-- [Stanford Knees](projects/REC/stanfordknees2019.html): Supports the `(REC)` task.
-
-## 🛠️ Installation
-
-**ATOMMIC** is best to be installed in a Conda environment.
-
-### 🐍 Conda
-```
-conda create -n atommic python=3.10
-conda activate atommic
-```
-
-### 📦 Pip
-Use this installation mode if you want the latest released version.
-
-```bash
-pip install atommic
-```
-
-### From source
-
-Use this installation mode if you are contributing to atommic.
-
-```bash
-git clone https://github.com/wdika/atommic
-cd atommic
-bash ./reinstall.sh
-```
-
-### 🐳 Docker containers
-To build an atommic container with Dockerfile from a branch,  please run
-
-```bash
-  DOCKER_BUILDKIT=1 docker build -f Dockerfile -t atommic:latest.
-```
-
-As [NeMo](https://github.com/NVIDIA/NeMo) suggests, if you choose to work with the `main` branch, use NVIDIA's PyTorch container version [21.05-py3](https://ngc.nvidia.com/containers/nvidia:pytorch/tags), then install from GitHub.
-
-```bash
-    docker run --gpus all -it --rm -v <atommic_github_folder>:/ATOMMIC --shm-size=8g \
-    -p 8888:8888 -p 6006:6006 --ulimit memlock=-1 --ulimit \
-    stack=67108864 --device=/dev/snd nvcr.io/nvidia/pytorch:21.05-py3
-```
+- [AHEAD](https://github.com/wdika/atommic/tree/main/projects/qMRI/AHEAD): Supports the `(qMRI)` and `(REC)` tasks.
+- [BraTS 2023 Adult Glioma](https://github.com/wdika/atommic/tree/main/projects/SEG/BraTS2023AdultGlioma): Supports the `(SEG)` task.
+- [CC359](https://github.com/wdika/atommic/tree/main/projects/REC/CC359): Supports the `(REC)` task.
+- [fastMRI Brains Multicoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIBrainsMulticoil): Supports the `(REC)` task.
+- [fastMRI Knees Multicoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIKneesMulticoil): Supports the `(REC)` task.
+- [fastMRI Knees Singlecoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIKneesSinglecoil): Supports the `(REC)` task.
+- [ISLES 2022 Sub Acute Stroke](https://github.com/wdika/atommic/tree/main/projects/SEG/ISLES2022SubAcuteStroke): Supports the `(SEG)` task.
+- [SKM-TEA](https://github.com/wdika/atommic/tree/main/projects/MTL/rs/SKMTEA): Supports the `(REC)`, `(SEG)`, and `(MTL)` tasks.
+- [Stanford Knees](https://github.com/wdika/atommic/tree/main/projects/REC/StanfordKnees2019): Supports the `(REC)` task.
 
 ## 📚 API Documentation
 
 [![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 
 Access the API Documentation [here](https://atommic.readthedocs.io/en/latest/index.html)
 
 ## 📄 License
 
 **ATOMMIC** is under [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-
 ## 📖 Citation
 
 If you use ATOMMIC in your research, please cite as follows:
 
 ```BibTeX
-@misc{atommic,
-    author = {Karkalousos Dimitrios, Isqum Ivana, Marquering Henk, Caan Matthan},
-    title = {ATOMMIC: Advanced Toolbox for Multitask Medical Imaging Consistency},
-    year = {2023},
-    url = {https://github.com/wdika/atommic},
-}
+@article{Karkalousos_2024,
+   title={Atommic: An Advanced Toolbox for Multitask Medical Imaging Consistency to Facilitate Artificial Intelligence Applications from Acquisition to Analysis in Magnetic Resonance Imaging},
+   url={http://dx.doi.org/10.2139/ssrn.4801289},
+   DOI={10.2139/ssrn.4801289},
+   publisher={Elsevier BV},
+   author={Karkalousos, Dimitrios and Išgum, Ivana and Marquering, Henk and Caan, Matthan  W.A.},
+   year={2024}}
 ```
 
 ## 🔗 References
 
-The following papers have used ATOMMIC:
+ATOMMIC has been used or is referenced in the following papers:
+
+1. Karkalousos, Dimitrios and Išgum, Ivana and Marquering, Henk and Caan, Matthan W.A., Atommic: An Advanced Toolbox for Multitask Medical Imaging Consistency to Facilitate Artificial Intelligence Applications from Acquisition to Analysis in Magnetic Resonance Imaging. Available at SSRN: https://ssrn.com/abstract=4801289 or http://dx.doi.org/10.2139/ssrn.4801289
+
+2. Karkalousos, D., Išgum, I., Marquering, H. A., & Caan, M. W. A. (2024). ATOMMIC: An Advanced Toolbox for Multitask Medical Imaging Consistency to facilitate Artificial Intelligence applications from acquisition to analysis in Magnetic Resonance Imaging. https://doi.org/10.2139/ssrn.4801289
+
+3. Karkalousos, D., Isgum, I., Marquering, H., & Caan, M. W. A. (2024, April 27). The Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC): A Deep Learning framework to facilitate Magnetic Resonance Imaging. Medical Imaging with Deep Learning. https://openreview.net/forum?id=HxTZr9yA0N
 
-1. Karkalousos, D., Isgum, I., Marquering, H. &amp; Caan, M.W.A.. (2024). MultiTask Learning for accelerated-MRI Reconstruction and Segmentation of Brain Lesions in Multiple Sclerosis. <i>Medical Imaging with Deep Learning</i>, in <i>Proceedings of Machine Learning Research</i> 227:991-1005 Available from https://proceedings.mlr.press/v227/karkalousos24a.html.
+4. Karkalousos, D., Isgum, I., Marquering, H. &amp; Caan, M.W.A.. (2024). MultiTask Learning for accelerated-MRI Reconstruction and Segmentation of Brain Lesions in Multiple Sclerosis. <i>Medical Imaging with Deep Learning</i>, in <i>Proceedings of Machine Learning Research</i> 227:991-1005 Available from https://proceedings.mlr.press/v227/karkalousos24a.html.
 
-2. Zhang, C., Karkalousos, D., Bazin, P. L., Coolen, B. F., Vrenken, H., Sonke, J. J., Forstmann, B. U., Poot, D. H. J., & Caan, M. W. A. (2022). A unified model for reconstruction and R2* mapping of accelerated 7T data using the quantitative recurrent inference machine. NeuroImage, 264. [DOI](https://doi.org/10.1016/j.neuroimage.2022.119680)
+5. Zhang, C., Karkalousos, D., Bazin, P. L., Coolen, B. F., Vrenken, H., Sonke, J. J., Forstmann, B. U., Poot, D. H. J., & Caan, M. W. A. (2022). A unified model for reconstruction and R2* mapping of accelerated 7T data using the quantitative recurrent inference machine. NeuroImage, 264. [DOI](https://doi.org/10.1016/j.neuroimage.2022.119680)
 
-3. Karkalousos, D., Noteboom, S., Hulst, H. E., Vos, F. M., & Caan, M. W. A. (2022). Assessment of data consistency through cascades of independently recurrent inference machines for fast and robust accelerated MRI reconstruction. Physics in Medicine & Biology. [DOI](https://doi.org/10.1088/1361-6560/AC6CC2)
+6. Karkalousos, D., Noteboom, S., Hulst, H. E., Vos, F. M., & Caan, M. W. A. (2022). Assessment of data consistency through cascades of independently recurrent inference machines for fast and robust accelerated MRI reconstruction. Physics in Medicine & Biology. [DOI](https://doi.org/10.1088/1361-6560/AC6CC2)
 
 ## 📧 Contact
 
 For any questions, please contact Dimitris Karkalousos @ [d.karkalousos@amsterdamumc.nl](mailto:d.karkalousos@amsterdamumc.nl).
 
 ## ⚠️🙏 Disclaimer & Acknowledgements
 
-> **Note:** ATOMMIC is built on top of [NeMo](https://github.com/NVIDIA/NeMo). NeMo is under Apache 2.0 license, so we are allowed to use it. We also assume that it is allowed to use the NeMo documentation, as long as we cite it and we always refer to the baselines everywhere and in the code and docs. ATOMMIC also includes implementations of reconstruction methods from [fastMRI](https://github.com/facebookresearch/fastMRI) and [DIRECT](https://github.com/NKI-AI/direct), and segmentation methods from [MONAI](https://github.com/Project-MONAI/MONAI), as well as other codebases which are always cited on the corresponding files. All methods in ATOMMIC are reimplemented and not called from the original libraries, allowing for full reproducibility, support, and easy extension. ATOMMIC is an open-source project under the Apache 2.0 license.
+> **Note:** ATOMMIC is built on top of [NeMo](https://github.com/NVIDIA/NeMo). NeMo is under Apache 2.0 license, so we are allowed to use it. We also assume that we can use the NeMo documentation basis as long as we cite it and always refer to the baselines everywhere in the code and docs. ATOMMIC also includes implementations of reconstruction methods from [fastMRI](https://github.com/facebookresearch/fastMRI) and [DIRECT](https://github.com/NKI-AI/direct), and segmentation methods from [MONAI](https://github.com/Project-MONAI/MONAI), as well as other codebases which are always cited on the corresponding files. All methods in ATOMMIC are reimplemented and not called from the original libraries, allowing for full reproducibility, support, and easy extension. ATOMMIC is an open-source project under the Apache 2.0 license.
```

### Comparing `atommic-1.0.0/README.md` & `atommic-1.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,140 @@
 # Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)
 [![HuggingFace](https://img.shields.io/badge/HuggingFace-Models-blue)](https://huggingface.co/wdika)
-[![GitHub issues](https://img.shields.io/github/issues/wdika/atommic)]()
+[![DockerHub](https://img.shields.io/badge/DockerHub-Link-blue)](docker.io/wdika/atommic)
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/atommic.svg)](https://badge.fury.io/py/atommic)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/atommic)](https://pypi.org/project/atommic/)
+[![GitHub issues](https://img.shields.io/github/issues/wdika/atommic)](https://github.com/wdika/atommic/issues)
+[![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atommic)](https://pypi.org/project/atommic/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]()
-<p align="center">
-    <img src="assets/atommic-logo.png" alt="Your Image" width="600" />
+<p align="center" style="margin-top: -40px; margin-bottom: -80px;">
+    <img src="assets/atommic-logo.png" alt="ATOMMIC-logo" width="600" />
 </p>
 
-# 👋 Introduction
+<div align="center">
+<span style="font-size:24px;">
+
+  [📜](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4801289)
+  [🤗](https://huggingface.co/wdika)
+  [🐳](docker.io/wdika/atommic)
+  [📦](https://pypi.org/project/atommic)
+  [📚](https://atommic.readthedocs.io/)
 
-The [Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)](https://github.com/wdika/atommic) is a
-toolbox for applying AI methods for **accelerated MRI reconstruction (REC)**, **MRI segmentation (SEG)**,
-**quantitative MR imaging (qMRI)**, as well as **multitask learning (MTL)**, i.e., performing multiple tasks
-simultaneously, such as reconstruction and segmentation. Each task is implemented in a separate collection, which
-consists of data loaders, transformations, models, metrics, and losses. **ATOMMIC** is designed to be modular and
-extensible, and it is easy to add new tasks, models, and datasets. **ATOMMIC** uses
-[PyTorch Lightning](https://www.pytorchlightning.ai/) for feasible high-performance multi-GPU/multi-node
-mixed-precision training.
+</div>
+
+## 👋 Introduction
+
+The [Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)](https://github.com/wdika/atommic) is a toolbox for applying AI methods for **accelerated MRI reconstruction (REC)**, **MRI segmentation (SEG)**, **quantitative MR imaging (qMRI)**, as well as **multitask learning (MTL)**, i.e., performing multiple tasks simultaneously, such as reconstruction and segmentation. Each task is implemented in a separate collection consisting of data loaders, transformations, models, metrics, and losses. **ATOMMIC** is designed to be modular and extensible on new tasks, models, and datasets. **ATOMMIC** uses [PyTorch Lightning](https://www.pytorchlightning.ai/) for feasible high-performance multi-GPU/multi-node mixed-precision training.
 
 ![ATOMMIC Schematic Overview](assets/atommic-schematic_overview.png)
 
-The schematic overview of **ATOMMIC** showcases the main components of the toolbox. First, we need an [MRI Dataset](README.md#mri-datasets) (e.g., **CC359**). Next, we need to define the high-level parameters, such as the [task and the model](../mri/collections.html), the [undersampling](../mri/undersampling.html), the [transforms](../mri/transforms.html), the [optimizer](../core/core.html#optimization), the [scheduler](../core/core.html#learning-rate-schedulers), the [loss](../mri/losses.html), the [trainer parameters](../core/core.html#training), and the [experiment manager](../core/exp_manager.html). All these parameters are defined in a `.yaml` file using [Hydra](https://hydra.cc/) and [OmegaConf](https://omegaconf.readthedocs.io/).
+The schematic overview of **ATOMMIC** showcases the main components of the toolbox. First, we need an [MRI Dataset](README.md#mri-datasets) (e.g., **CC359**). Next, we need to define the high-level parameters, such as the [task and the model](https://atommic.readthedocs.io/en/latest/mri/collections.html), the [undersampling](https://atommic.readthedocs.io/en/latest/mri//undersampling.html), the [transforms](https://atommic.readthedocs.io/en/latest/mri//transforms.html), the [optimizer](https://atommic.readthedocs.io/en/latest/core/core.html#optimization), the [scheduler](https://atommic.readthedocs.io/en/latest/core/core.html#learning-rate-schedulers), the [loss](https://atommic.readthedocs.io/en/latest/mri/losses.html), the [trainer parameters](https://atommic.readthedocs.io/en/latest/core/core.html#training), and the [experiment manager](https://atommic.readthedocs.io/en/latest/core/exp_manager.html). All these parameters are defined in a `.yaml` file using [Hydra](https://hydra.cc/) and [OmegaConf](https://omegaconf.readthedocs.io/).
+
+The trained model is an `.atommic` [module](https://atommic.readthedocs.io/en/latest/core/export.html), exported with [ONNX](https://onnx.ai/) and [TorchScript](https://pytorch.org/docs/stable/jit.html) support, which can be used for inference. The `.atommic` module can also be uploaded on [HuggingFace](https://huggingface.co/). Pretrained models are available on our [HF](https://huggingface.co/wdika) account and can be downloaded and used for inference.
+
+## 🛠️ Installation
+
+**ATOMMIC** is best to be installed in a Conda environment.
+
+### 🐍 Conda
+```
+conda create -n atommic python=3.10
+conda activate atommic
+```
+
+### 📦 Pip
+Use this installation mode if you want the latest released version.
+
+```bash
+pip install atommic
+```
+
+### From source
+
+Use this installation mode if you are contributing to atommic.
+
+```bash
+git clone https://github.com/wdika/atommic
+cd atommic
+bash ./reinstall.sh
+```
+
+### 🐳 Docker containers
 
-The trained model is an `.atommic` [module](../core/export.html), exported with [ONNX](https://onnx.ai/) and [TorchScript](https://pytorch.org/docs/stable/jit.html) support, which can be used for inference. The `.atommic` module can also be uploaded on [HuggingFace](https://huggingface.co/). Pretrained models are available on our [HF](https://huggingface.co/wdika) account and can be downloaded and used for inference.
+An atommic container is available at dockerhub, you can pull it with:
+```bash
+docker pull wdika/atommic
+```
+
+You can also build an atommic container with:
+```bash
+DOCKER_BUILDKIT=1 docker build -f Dockerfile -t atommic:latest .
+```
+
+You can run the container with:
+```bash
+docker run --gpus all -it --rm -v /home/user/configs:/config atommic:latest atommic run -c /config/config.yaml
+```
+where ```/config/config.yaml``` is the path to your local configuration file.
+
+Or you can run it interactively with:
+```bash
+docker run --gpus all -it --rm -p 8888:8888 atommic:latest /bin/bash -c "./start-jupyter.sh"
+```
 
 ## 🚀 Quick Start Guide
 
-The best way to get started with ATOMMIC is to start with one of the [tutorials](tutorials.html):
+The best way to get started with ATOMMIC is with one of the [tutorials](https://atommic.readthedocs.io/en/latest/starthere/tutorials.html):
+
+- [ATOMMIC Primer](https://github.com/wdika/atommic/blob/main/tutorials/00_ATOMMIC_Primer.ipynb) - demonstrates how to use ATOMMIC.
+- [ATOMMIC MRI transforms](https://github.com/wdika/atommic/blob/main/tutorials/01_ATOMMIC_MRI_transforms.ipynb) - demonstrates how to use ATOMMIC to undersample MRI data.
+- [ATOMMIC MRI undersampling](https://github.com/wdika/atommic/blob/main/tutorials/02_ATOMMIC_MRI_undersampling.ipynb) - demonstrates how to use ATOMMIC to apply transforms to MRI data.
+- [ATOMMIC Upload Model on HuggingFace](https://github.com/wdika/atommic/blob/main/tutorials/03_ATOMMIC_Upload_Model_On_HF.ipynb) - demonstrates how to upload a model on HuggingFace.
 
-- [ATOMMIC Primer](https://github.com/wdika/atommic/tutorials/00_ATOMMIC_Primer.ipynb) - demonstrates how to use ATOMMIC.
-- [ATOMMIC MRI transforms](https://github.com/wdika/atommic/tutorials/01_ATOMMIC_MRI_transforms.ipynb) - demonstrates how to use ATOMMIC to undersample MRI data.
-- [ATOMMIC MRI undersampling](https://github.com/wdika/atommic/tutorials/02_ATOMMIC_MRI_undersampling.ipynb) - demonstrates how to use ATOMMIC to apply transforms to MRI data.
-- [ATOMMIC Upload Model on HuggingFace](https://github.com/wdika/atommic/tutorials/03_ATOMMIC_Upload_Model_On_HF.ipynb) - demonstrates how to upload a model on HuggingFace.
+You can also check the [projects](https://github.com/wdika/atommic/tree/main/projects) page to see how to use ATOMMIC for specific tasks and public datasets.
 
-You can also check the [projects](projects.html) page to see how to use ATOMMIC for specific tasks and public datasets.
+Pre-trained models are available on HuggingFace [🤗](https://huggingface.co/wdika).
 
-### **ATOMMIC paper is fully reproducible. Please check [here](projects/ATOMMIC_paper/README.md) for more information.**
+### **ATOMMIC paper is fully reproducible. Please check [here](https://github.com/wdika/atommic/tree/main/projects/ATOMMIC_paper/README.md) for more information.**
 
 ## 🤖 Training & Testing
 
-Training and testing models in **ATOMMIC** is intuitive and easy. You just need to properly configure the `.yaml`
-file and just run the following command:
+Training and testing models in **ATOMMIC** is intuitive and easy. You just need to properly configure a `.yaml` file and run the following command:
 
 ```bash
 atommic run -c path-to-config-file
 ```
 
 ## ⚙️ Configuration
 
-1. Choose the **task** and the **model**, according to the [collections](../mri/collections.html).
+1. Choose the **task** and the **model**, according to the [collections](https://atommic.readthedocs.io/en/latest/mri/collections.html).
 
 2. Choose the **dataset** and the **dataset parameters**, according to the [datasets](README.md#mri-datasets) or your own dataset.
 
-3. Choose the [undersampling](../mri/transforms.html).
+3. Choose the [undersampling](https://atommic.readthedocs.io/en/latest/mri/transforms.html).
 
-4. Choose the [transforms](../mri/transforms.html).
+4. Choose the [transforms](https://atommic.readthedocs.io/en/latest/mri/transforms.html).
 
-5. Choose the [losses](../mri/losses.html).
+5. Choose the [losses](https://atommic.readthedocs.io/en/latest/mri/losses.html).
 
-6. Choose the [optimizer](../core/core.html#optimization).
+6. Choose the [optimizer](https://atommic.readthedocs.io/en/latest/core/core.html#optimization).
 
-7. Choose the [scheduler](../core/core.html#learning-rate-schedulers).
+7. Choose the [scheduler](https://atommic.readthedocs.io/en/latest/core/core.html#learning-rate-schedulers).
 
-8. Choose the [trainer parameters](../core/core.html#training).
+8. Choose the [trainer parameters](https://atommic.readthedocs.io/en/latest/core/core.html#training).
 
-9. Choose the [experiment manager](../core/exp_manager.html).
+9. Choose the [experiment manager](https://atommic.readthedocs.io/en/latest/core/exp_manager.html).
 
-You can also check the [projects](projects.html) page to see how to configure the `.yaml` file for specific tasks.
+You can also check the [projects](https://github.com/wdika/atommic/tree/main/projects/) page to see how to configure the `.yaml` file for specific tasks.
 
 ## 🗂️ Collections
 
-**ATOMMIC** is organized into [collections](../mri/collections.html), each of which implements a specific task. The following collections are currently available, implementing various models as listed:
+**ATOMMIC** is organized into [collections](https://atommic.readthedocs.io/en/latest/mri/collections.html), each of which implements a specific task. The following collections are currently available, implementing various models as listed:
 
 ### MultiTask Learning (MTL)
 1. End-to-End Recurrent Attention Network (`SERANet`), 2. Image domain Deep Structured Low-Rank Network (`IDSLR`), 3. Image domain Deep Structured Low-Rank UNet (`IDSLRUNet`), 4. Multi-Task Learning for MRI Reconstruction and Segmentation (`MTLRS`), 5. Reconstruction Segmentation method using UNet (`RecSegUNet`), 6. Segmentation Network MRI (`SegNet`).
 
 ### Quantitative MR Imaging (qMRI)
 1. Quantitative Recurrent Inference Machines (`qRIMBlock`), 2. Quantitative End-to-End Variational Network (`qVarNet`), 3. Quantitative Cascades of Independently Recurrent Inference Machines (`qCIRIM`).
 
@@ -88,100 +144,64 @@
 ### MRI Segmentation (SEG)
 1. `SegmentationAttentionUNet`, 2. `SegmentationDYNUNet`, 3. `SegmentationLambdaUNet`, 4. `SegmentationUNet`, 5. `Segmentation3DUNet`, 6. `SegmentationUNetR`, 7. `SegmentationVNet`.
 
 ## MRI Datasets
 
 **ATOMMIC** supports public datasets, as well as private datasets. The following public datasets are supported natively:
 
-- [AHEAD](projects/MTL/ahead.html): Supports the `(qMRI)` and `(REC)` tasks.
-- [BraTS 2023 Adult Glioma](projects/SEG/brats2023adultglioma.html): Supports the `(SEG)` task.
-- [CC359](projects/REC/cc359.html): Supports the `(REC)` task.
-- [fastMRI Brains Multicoil](projects/REC/fastmribrainsmulticoil.html): Supports the `(REC)` task.
-- [fastMRI Knees Multicoil](projects/REC/fastmrikneesmulticoil.html): Supports the `(REC)` task.
-- [fastMRI Knees Singlecoil](projects/REC/fastmrikneessinglecoil.html): Supports the `(REC)` task.
-- [ISLES 2022 Sub Acute Stroke](projects/SEG/isles2022subacutestroke.html): Supports the `(SEG)` task.
-- [SKM-TEA](projects/REC/skmtea.html): Supports the `(REC)`, `(SEG)`, and `(MTL)` tasks.
-- [Stanford Knees](projects/REC/stanfordknees2019.html): Supports the `(REC)` task.
-
-## 🛠️ Installation
-
-**ATOMMIC** is best to be installed in a Conda environment.
-
-### 🐍 Conda
-```
-conda create -n atommic python=3.10
-conda activate atommic
-```
-
-### 📦 Pip
-Use this installation mode if you want the latest released version.
-
-```bash
-pip install atommic
-```
-
-### From source
-
-Use this installation mode if you are contributing to atommic.
-
-```bash
-git clone https://github.com/wdika/atommic
-cd atommic
-bash ./reinstall.sh
-```
-
-### 🐳 Docker containers
-To build an atommic container with Dockerfile from a branch,  please run
-
-```bash
-  DOCKER_BUILDKIT=1 docker build -f Dockerfile -t atommic:latest.
-```
-
-As [NeMo](https://github.com/NVIDIA/NeMo) suggests, if you choose to work with the `main` branch, use NVIDIA's PyTorch container version [21.05-py3](https://ngc.nvidia.com/containers/nvidia:pytorch/tags), then install from GitHub.
-
-```bash
-    docker run --gpus all -it --rm -v <atommic_github_folder>:/ATOMMIC --shm-size=8g \
-    -p 8888:8888 -p 6006:6006 --ulimit memlock=-1 --ulimit \
-    stack=67108864 --device=/dev/snd nvcr.io/nvidia/pytorch:21.05-py3
-```
+- [AHEAD](https://github.com/wdika/atommic/tree/main/projects/qMRI/AHEAD): Supports the `(qMRI)` and `(REC)` tasks.
+- [BraTS 2023 Adult Glioma](https://github.com/wdika/atommic/tree/main/projects/SEG/BraTS2023AdultGlioma): Supports the `(SEG)` task.
+- [CC359](https://github.com/wdika/atommic/tree/main/projects/REC/CC359): Supports the `(REC)` task.
+- [fastMRI Brains Multicoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIBrainsMulticoil): Supports the `(REC)` task.
+- [fastMRI Knees Multicoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIKneesMulticoil): Supports the `(REC)` task.
+- [fastMRI Knees Singlecoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIKneesSinglecoil): Supports the `(REC)` task.
+- [ISLES 2022 Sub Acute Stroke](https://github.com/wdika/atommic/tree/main/projects/SEG/ISLES2022SubAcuteStroke): Supports the `(SEG)` task.
+- [SKM-TEA](https://github.com/wdika/atommic/tree/main/projects/MTL/rs/SKMTEA): Supports the `(REC)`, `(SEG)`, and `(MTL)` tasks.
+- [Stanford Knees](https://github.com/wdika/atommic/tree/main/projects/REC/StanfordKnees2019): Supports the `(REC)` task.
 
 ## 📚 API Documentation
 
 [![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 
 Access the API Documentation [here](https://atommic.readthedocs.io/en/latest/index.html)
 
 ## 📄 License
 
 **ATOMMIC** is under [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-
 ## 📖 Citation
 
 If you use ATOMMIC in your research, please cite as follows:
 
 ```BibTeX
-@misc{atommic,
-    author = {Karkalousos Dimitrios, Isqum Ivana, Marquering Henk, Caan Matthan},
-    title = {ATOMMIC: Advanced Toolbox for Multitask Medical Imaging Consistency},
-    year = {2023},
-    url = {https://github.com/wdika/atommic},
-}
+@article{Karkalousos_2024,
+   title={Atommic: An Advanced Toolbox for Multitask Medical Imaging Consistency to Facilitate Artificial Intelligence Applications from Acquisition to Analysis in Magnetic Resonance Imaging},
+   url={http://dx.doi.org/10.2139/ssrn.4801289},
+   DOI={10.2139/ssrn.4801289},
+   publisher={Elsevier BV},
+   author={Karkalousos, Dimitrios and Išgum, Ivana and Marquering, Henk and Caan, Matthan  W.A.},
+   year={2024}}
 ```
 
 ## 🔗 References
 
-The following papers have used ATOMMIC:
+ATOMMIC has been used or is referenced in the following papers:
+
+1. Karkalousos, Dimitrios and Išgum, Ivana and Marquering, Henk and Caan, Matthan W.A., Atommic: An Advanced Toolbox for Multitask Medical Imaging Consistency to Facilitate Artificial Intelligence Applications from Acquisition to Analysis in Magnetic Resonance Imaging. Available at SSRN: https://ssrn.com/abstract=4801289 or http://dx.doi.org/10.2139/ssrn.4801289
+
+2. Karkalousos, D., Išgum, I., Marquering, H. A., & Caan, M. W. A. (2024). ATOMMIC: An Advanced Toolbox for Multitask Medical Imaging Consistency to facilitate Artificial Intelligence applications from acquisition to analysis in Magnetic Resonance Imaging. https://doi.org/10.2139/ssrn.4801289
+
+3. Karkalousos, D., Isgum, I., Marquering, H., & Caan, M. W. A. (2024, April 27). The Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC): A Deep Learning framework to facilitate Magnetic Resonance Imaging. Medical Imaging with Deep Learning. https://openreview.net/forum?id=HxTZr9yA0N
 
-1. Karkalousos, D., Isgum, I., Marquering, H. &amp; Caan, M.W.A.. (2024). MultiTask Learning for accelerated-MRI Reconstruction and Segmentation of Brain Lesions in Multiple Sclerosis. <i>Medical Imaging with Deep Learning</i>, in <i>Proceedings of Machine Learning Research</i> 227:991-1005 Available from https://proceedings.mlr.press/v227/karkalousos24a.html.
+4. Karkalousos, D., Isgum, I., Marquering, H. &amp; Caan, M.W.A.. (2024). MultiTask Learning for accelerated-MRI Reconstruction and Segmentation of Brain Lesions in Multiple Sclerosis. <i>Medical Imaging with Deep Learning</i>, in <i>Proceedings of Machine Learning Research</i> 227:991-1005 Available from https://proceedings.mlr.press/v227/karkalousos24a.html.
 
-2. Zhang, C., Karkalousos, D., Bazin, P. L., Coolen, B. F., Vrenken, H., Sonke, J. J., Forstmann, B. U., Poot, D. H. J., & Caan, M. W. A. (2022). A unified model for reconstruction and R2* mapping of accelerated 7T data using the quantitative recurrent inference machine. NeuroImage, 264. [DOI](https://doi.org/10.1016/j.neuroimage.2022.119680)
+5. Zhang, C., Karkalousos, D., Bazin, P. L., Coolen, B. F., Vrenken, H., Sonke, J. J., Forstmann, B. U., Poot, D. H. J., & Caan, M. W. A. (2022). A unified model for reconstruction and R2* mapping of accelerated 7T data using the quantitative recurrent inference machine. NeuroImage, 264. [DOI](https://doi.org/10.1016/j.neuroimage.2022.119680)
 
-3. Karkalousos, D., Noteboom, S., Hulst, H. E., Vos, F. M., & Caan, M. W. A. (2022). Assessment of data consistency through cascades of independently recurrent inference machines for fast and robust accelerated MRI reconstruction. Physics in Medicine & Biology. [DOI](https://doi.org/10.1088/1361-6560/AC6CC2)
+6. Karkalousos, D., Noteboom, S., Hulst, H. E., Vos, F. M., & Caan, M. W. A. (2022). Assessment of data consistency through cascades of independently recurrent inference machines for fast and robust accelerated MRI reconstruction. Physics in Medicine & Biology. [DOI](https://doi.org/10.1088/1361-6560/AC6CC2)
 
 ## 📧 Contact
 
 For any questions, please contact Dimitris Karkalousos @ [d.karkalousos@amsterdamumc.nl](mailto:d.karkalousos@amsterdamumc.nl).
 
 ## ⚠️🙏 Disclaimer & Acknowledgements
 
-> **Note:** ATOMMIC is built on top of [NeMo](https://github.com/NVIDIA/NeMo). NeMo is under Apache 2.0 license, so we are allowed to use it. We also assume that it is allowed to use the NeMo documentation, as long as we cite it and we always refer to the baselines everywhere and in the code and docs. ATOMMIC also includes implementations of reconstruction methods from [fastMRI](https://github.com/facebookresearch/fastMRI) and [DIRECT](https://github.com/NKI-AI/direct), and segmentation methods from [MONAI](https://github.com/Project-MONAI/MONAI), as well as other codebases which are always cited on the corresponding files. All methods in ATOMMIC are reimplemented and not called from the original libraries, allowing for full reproducibility, support, and easy extension. ATOMMIC is an open-source project under the Apache 2.0 license.
+> **Note:** ATOMMIC is built on top of [NeMo](https://github.com/NVIDIA/NeMo). NeMo is under Apache 2.0 license, so we are allowed to use it. We also assume that we can use the NeMo documentation basis as long as we cite it and always refer to the baselines everywhere in the code and docs. ATOMMIC also includes implementations of reconstruction methods from [fastMRI](https://github.com/facebookresearch/fastMRI) and [DIRECT](https://github.com/NKI-AI/direct), and segmentation methods from [MONAI](https://github.com/Project-MONAI/MONAI), as well as other codebases which are always cited on the corresponding files. All methods in ATOMMIC are reimplemented and not called from the original libraries, allowing for full reproducibility, support, and easy extension. ATOMMIC is an open-source project under the Apache 2.0 license.
```

### Comparing `atommic-1.0.0/atommic/cli/__init__.py` & `atommic-1.0.1/atommic/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/cli/launch.py` & `atommic-1.0.1/atommic/cli/launch.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/callbacks/callbacks.py` & `atommic-1.0.1/atommic/collections/common/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/callbacks/ema.py` & `atommic-1.0.1/atommic/collections/common/callbacks/ema.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/data/mri_loader.py` & `atommic-1.0.1/atommic/collections/common/data/mri_loader.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/data/subsample.py` & `atommic-1.0.1/atommic/collections/common/data/subsample.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/losses/aggregator.py` & `atommic-1.0.1/atommic/collections/common/losses/aggregator.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/losses/wasserstein.py` & `atommic-1.0.1/atommic/collections/common/losses/wasserstein.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/metrics/global_average_loss_metric.py` & `atommic-1.0.1/atommic/collections/common/metrics/global_average_loss_metric.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/nn/base.py` & `atommic-1.0.1/atommic/collections/common/nn/base.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/parts/__init__.py` & `atommic-1.0.1/atommic/collections/common/parts/__init__.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/parts/coil_sensitivity_maps.py` & `atommic-1.0.1/atommic/collections/common/parts/coil_sensitivity_maps.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/parts/fft.py` & `atommic-1.0.1/atommic/collections/common/parts/fft.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/parts/transforms.py` & `atommic-1.0.1/atommic/collections/common/parts/transforms.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/common/parts/utils.py` & `atommic-1.0.1/atommic/collections/common/parts/utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/motioncorrection/parts/motionsimulation.py` & `atommic-1.0.1/atommic/collections/motioncorrection/parts/motionsimulation.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/data/mrirs_loader.py` & `atommic-1.0.1/atommic/collections/multitask/rs/data/mrirs_loader.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/__init__.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/base.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/base.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr_base/idslr_block.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr_base/idslr_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/idslr_unet.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/idslr_unet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/mtlrs.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/mtlrs.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/mtlrs_base/mtlrs_block.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/mtlrs_base/mtlrs_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/recseg_unet.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/recseg_unet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/segnet.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/segnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/convlstm.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/convlstm.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/convlstm_unet.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/convlstm_unet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/nn/seranet_base/seranet_block.py` & `atommic-1.0.1/atommic/collections/multitask/rs/nn/seranet_base/seranet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/multitask/rs/parts/transforms.py` & `atommic-1.0.1/atommic/collections/multitask/rs/parts/transforms.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/data/qmri_loader.py` & `atommic-1.0.1/atommic/collections/quantitative/data/qmri_loader.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/nn/base.py` & `atommic-1.0.1/atommic/collections/quantitative/nn/base.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/nn/qcirim.py` & `atommic-1.0.1/atommic/collections/quantitative/nn/qcirim.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/nn/qrim_base/qrim_block.py` & `atommic-1.0.1/atommic/collections/quantitative/nn/qrim_base/qrim_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/nn/qrim_base/utils.py` & `atommic-1.0.1/atommic/collections/quantitative/nn/qrim_base/utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/nn/qvarnet.py` & `atommic-1.0.1/atommic/collections/quantitative/nn/qvarnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/nn/qvarnet_base/qvarnet_block.py` & `atommic-1.0.1/atommic/collections/quantitative/nn/qvarnet_base/qvarnet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/nn/qzf.py` & `atommic-1.0.1/atommic/collections/quantitative/nn/qzf.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/quantitative/parts/transforms.py` & `atommic-1.0.1/atommic/collections/quantitative/parts/transforms.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/data/mri_reconstruction_loader.py` & `atommic-1.0.1/atommic/collections/reconstruction/data/mri_reconstruction_loader.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/losses/na.py` & `atommic-1.0.1/atommic/collections/reconstruction/losses/na.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/losses/ssim.py` & `atommic-1.0.1/atommic/collections/reconstruction/losses/ssim.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/metrics/reconstruction_metrics.py` & `atommic-1.0.1/atommic/collections/reconstruction/metrics/reconstruction_metrics.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/__init__.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/base.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/base.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/ccnn.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/ccnn.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/ccnn_base/ccnn_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/ccnn_base/ccnn_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/cirim.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/cirim.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/crnn.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/crnn.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/crnn_base/crnn_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/crnn_base/crnn_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/crossdomain_base/crossdomain_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/crossdomain_base/crossdomain_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/didn_base/didn_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/didn_base/didn_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/dunet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/dunet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/jointicnet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/jointicnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/kikinet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/kikinet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/lpd.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/lpd.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/modl.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/modl.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/modl_base/modl_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/modl_base/modl_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/multidomainnet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/multidomainnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/multidomainnet_base/multidomainnet_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/multidomainnet_base/multidomainnet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/mwcnn_base/mwcnn_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/mwcnn_base/mwcnn_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/primaldualnet_base/primaldualnet_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/primaldualnet_base/primaldualnet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/proximal_gradient.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/proximal_gradient.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/recurrentvarnet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/recurrentvarnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/recurrentvarnet_base/recurrentvarnet_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/recurrentvarnet_base/recurrentvarnet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/conv_layers.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/conv_layers.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/rim_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/rim_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/rim_utils.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/rim_utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/rim_base/rnn_cells.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/rim_base/rnn_cells.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/sigmanet_base/dc_layers.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/sigmanet_base/dc_layers.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/sigmanet_base/sensitivity_net.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/sigmanet_base/sensitivity_net.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/unet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/unet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/unet_base/unet_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/unet_base/unet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/varnet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/varnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/varnet_base/varnet_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/varnet_base/varnet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/vsnet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/vsnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/vsnet_base/vsnet_block.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/vsnet_base/vsnet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/xpdnet.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/xpdnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/reconstruction/nn/zf.py` & `atommic-1.0.1/atommic/collections/reconstruction/nn/zf.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/data/mri_segmentation_loader.py` & `atommic-1.0.1/atommic/collections/segmentation/data/mri_segmentation_loader.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/losses/cross_entropy.py` & `atommic-1.0.1/atommic/collections/segmentation/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/losses/dice.py` & `atommic-1.0.1/atommic/collections/segmentation/losses/dice.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/losses/utils.py` & `atommic-1.0.1/atommic/collections/segmentation/losses/utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/metrics/segmentation_metrics.py` & `atommic-1.0.1/atommic/collections/segmentation/metrics/segmentation_metrics.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/__init__.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/attentionunet.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/attentionunet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/attentionunet_base/attentionunet_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/attentionunet_base/attentionunet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/base.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/base.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/dynunet.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/dynunet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/dynunet_base/dynunet_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/dynunet_base/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/lambdaunet.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/lambdaunet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/lambdaunet_base/lambdaunet_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/lambdaunet_base/lambdaunet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/segmentationnet.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/segmentationnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/unet.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/unet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/unet3d.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/unet3d.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/unet3d_base/unet3d_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/unet3d_base/unet3d_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/unetr.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/unetr.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/unetr_base/unetr_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/unetr_base/unetr_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/patchembedding.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/patchembedding.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/transformer_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/transformer_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/utils.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/vit_base/vit_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/vit_base/vit_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/vnet.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/vnet.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/collections/segmentation/nn/vnet_base/vnet_block.py` & `atommic-1.0.1/atommic/collections/segmentation/nn/vnet_base/vnet_block.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/constants.py` & `atommic-1.0.1/atommic/constants.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/classes/common.py` & `atommic-1.0.1/atommic/core/classes/common.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/classes/dataset.py` & `atommic-1.0.1/atommic/core/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/classes/export.py` & `atommic-1.0.1/atommic/core/classes/export.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/classes/modelPT.py` & `atommic-1.0.1/atommic/core/classes/modelPT.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/conf/hydra_runner.py` & `atommic-1.0.1/atommic/core/conf/hydra_runner.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/conf/modelPT.py` & `atommic-1.0.1/atommic/core/conf/modelPT.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/conf/optimizers.py` & `atommic-1.0.1/atommic/core/conf/optimizers.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/conf/schedulers.py` & `atommic-1.0.1/atommic/core/conf/schedulers.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/conf/trainer.py` & `atommic-1.0.1/atommic/core/conf/trainer.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/connectors/save_restore_connector.py` & `atommic-1.0.1/atommic/core/connectors/save_restore_connector.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/neural_types/axes.py` & `atommic-1.0.1/atommic/core/neural_types/axes.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/neural_types/comparison.py` & `atommic-1.0.1/atommic/core/neural_types/comparison.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/neural_types/elements.py` & `atommic-1.0.1/atommic/core/neural_types/elements.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/neural_types/neural_type.py` & `atommic-1.0.1/atommic/core/neural_types/neural_type.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/optim/adafactor.py` & `atommic-1.0.1/atommic/core/optim/adafactor.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/optim/lion.py` & `atommic-1.0.1/atommic/core/optim/lion.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/optim/lr_scheduler.py` & `atommic-1.0.1/atommic/core/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/optim/novograd.py` & `atommic-1.0.1/atommic/core/optim/novograd.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/optim/optimizer_with_main_params.py` & `atommic-1.0.1/atommic/core/optim/optimizer_with_main_params.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/optim/optimizers.py` & `atommic-1.0.1/atommic/core/optim/optimizers.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/optim/radam.py` & `atommic-1.0.1/atommic/core/optim/radam.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/utils/neural_type_utils.py` & `atommic-1.0.1/atommic/core/utils/neural_type_utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/utils/numba_utils.py` & `atommic-1.0.1/atommic/core/utils/numba_utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/core/utils/process_launcher/launcher.py` & `atommic-1.0.1/atommic/core/utils/process_launcher/launcher.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/package_info.py` & `atommic-1.0.1/atommic/package_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding=utf-8
 
 MAJOR = 1
 MINOR = 0
-PATCH = 0
+PATCH = 1
 PRE_RELEASE = ""
 
 # Use the following formatting: (major, minor, patch, pre-release)
 VERSION = (MAJOR, MINOR, PATCH, PRE_RELEASE)
 
 __shortversion__ = ".".join(map(str, VERSION[:3]))
 __version__ = ".".join(map(str, VERSION[:3])) + "".join(VERSION[3:])
```

### Comparing `atommic-1.0.0/atommic/utils/app_state.py` & `atommic-1.0.1/atommic/utils/app_state.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/atommic_logging.py` & `atommic-1.0.1/atommic/utils/atommic_logging.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/callbacks/atommic_model_checkpoint.py` & `atommic-1.0.1/atommic/utils/callbacks/atommic_model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/callbacks/preemption.py` & `atommic-1.0.1/atommic/utils/callbacks/preemption.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/cast_utils.py` & `atommic-1.0.1/atommic/utils/cast_utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/decorators/deprecated.py` & `atommic-1.0.1/atommic/utils/decorators/deprecated.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/decorators/experimental.py` & `atommic-1.0.1/atommic/utils/decorators/experimental.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/decorators/port_docs.py` & `atommic-1.0.1/atommic/utils/decorators/port_docs.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/env_var_parsing.py` & `atommic-1.0.1/atommic/utils/env_var_parsing.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/exp_manager.py` & `atommic-1.0.1/atommic/utils/exp_manager.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/export_utils.py` & `atommic-1.0.1/atommic/utils/export_utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/formaters/base.py` & `atommic-1.0.1/atommic/utils/formaters/base.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/formaters/colors.py` & `atommic-1.0.1/atommic/utils/formaters/colors.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/formaters/utils.py` & `atommic-1.0.1/atommic/utils/formaters/utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/get_rank.py` & `atommic-1.0.1/atommic/utils/get_rank.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/lightning_logger_patch.py` & `atommic-1.0.1/atommic/utils/lightning_logger_patch.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/metaclasses.py` & `atommic-1.0.1/atommic/utils/metaclasses.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/model_utils.py` & `atommic-1.0.1/atommic/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic/utils/timers.py` & `atommic-1.0.1/atommic/utils/timers.py`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/atommic.egg-info/PKG-INFO` & `atommic-1.0.1/atommic.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atommic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)
 Home-page: https://github.com/wdika/atommic
 Download-URL: https://github.com/wdika/atommic/releases
 Author: Dimitris Karkalousos
 Author-email: d.karkalousos@amsterdamumc.nl
 Maintainer: Dimitris Karkalousos
 Maintainer-email: d.karkalousos@amsterdamumc.nl
@@ -27,89 +27,145 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10, <=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)
 [![HuggingFace](https://img.shields.io/badge/HuggingFace-Models-blue)](https://huggingface.co/wdika)
-[![GitHub issues](https://img.shields.io/github/issues/wdika/atommic)]()
+[![DockerHub](https://img.shields.io/badge/DockerHub-Link-blue)](docker.io/wdika/atommic)
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/atommic.svg)](https://badge.fury.io/py/atommic)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/atommic)](https://pypi.org/project/atommic/)
+[![GitHub issues](https://img.shields.io/github/issues/wdika/atommic)](https://github.com/wdika/atommic/issues)
+[![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atommic)](https://pypi.org/project/atommic/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]()
-<p align="center">
-    <img src="assets/atommic-logo.png" alt="Your Image" width="600" />
+<p align="center" style="margin-top: -40px; margin-bottom: -80px;">
+    <img src="assets/atommic-logo.png" alt="ATOMMIC-logo" width="600" />
 </p>
 
-# 👋 Introduction
+<div align="center">
+<span style="font-size:24px;">
+
+  [📜](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4801289)
+  [🤗](https://huggingface.co/wdika)
+  [🐳](docker.io/wdika/atommic)
+  [📦](https://pypi.org/project/atommic)
+  [📚](https://atommic.readthedocs.io/)
 
-The [Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)](https://github.com/wdika/atommic) is a
-toolbox for applying AI methods for **accelerated MRI reconstruction (REC)**, **MRI segmentation (SEG)**,
-**quantitative MR imaging (qMRI)**, as well as **multitask learning (MTL)**, i.e., performing multiple tasks
-simultaneously, such as reconstruction and segmentation. Each task is implemented in a separate collection, which
-consists of data loaders, transformations, models, metrics, and losses. **ATOMMIC** is designed to be modular and
-extensible, and it is easy to add new tasks, models, and datasets. **ATOMMIC** uses
-[PyTorch Lightning](https://www.pytorchlightning.ai/) for feasible high-performance multi-GPU/multi-node
-mixed-precision training.
+</div>
+
+## 👋 Introduction
+
+The [Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC)](https://github.com/wdika/atommic) is a toolbox for applying AI methods for **accelerated MRI reconstruction (REC)**, **MRI segmentation (SEG)**, **quantitative MR imaging (qMRI)**, as well as **multitask learning (MTL)**, i.e., performing multiple tasks simultaneously, such as reconstruction and segmentation. Each task is implemented in a separate collection consisting of data loaders, transformations, models, metrics, and losses. **ATOMMIC** is designed to be modular and extensible on new tasks, models, and datasets. **ATOMMIC** uses [PyTorch Lightning](https://www.pytorchlightning.ai/) for feasible high-performance multi-GPU/multi-node mixed-precision training.
 
 ![ATOMMIC Schematic Overview](assets/atommic-schematic_overview.png)
 
-The schematic overview of **ATOMMIC** showcases the main components of the toolbox. First, we need an [MRI Dataset](README.md#mri-datasets) (e.g., **CC359**). Next, we need to define the high-level parameters, such as the [task and the model](../mri/collections.html), the [undersampling](../mri/undersampling.html), the [transforms](../mri/transforms.html), the [optimizer](../core/core.html#optimization), the [scheduler](../core/core.html#learning-rate-schedulers), the [loss](../mri/losses.html), the [trainer parameters](../core/core.html#training), and the [experiment manager](../core/exp_manager.html). All these parameters are defined in a `.yaml` file using [Hydra](https://hydra.cc/) and [OmegaConf](https://omegaconf.readthedocs.io/).
+The schematic overview of **ATOMMIC** showcases the main components of the toolbox. First, we need an [MRI Dataset](README.md#mri-datasets) (e.g., **CC359**). Next, we need to define the high-level parameters, such as the [task and the model](https://atommic.readthedocs.io/en/latest/mri/collections.html), the [undersampling](https://atommic.readthedocs.io/en/latest/mri//undersampling.html), the [transforms](https://atommic.readthedocs.io/en/latest/mri//transforms.html), the [optimizer](https://atommic.readthedocs.io/en/latest/core/core.html#optimization), the [scheduler](https://atommic.readthedocs.io/en/latest/core/core.html#learning-rate-schedulers), the [loss](https://atommic.readthedocs.io/en/latest/mri/losses.html), the [trainer parameters](https://atommic.readthedocs.io/en/latest/core/core.html#training), and the [experiment manager](https://atommic.readthedocs.io/en/latest/core/exp_manager.html). All these parameters are defined in a `.yaml` file using [Hydra](https://hydra.cc/) and [OmegaConf](https://omegaconf.readthedocs.io/).
+
+The trained model is an `.atommic` [module](https://atommic.readthedocs.io/en/latest/core/export.html), exported with [ONNX](https://onnx.ai/) and [TorchScript](https://pytorch.org/docs/stable/jit.html) support, which can be used for inference. The `.atommic` module can also be uploaded on [HuggingFace](https://huggingface.co/). Pretrained models are available on our [HF](https://huggingface.co/wdika) account and can be downloaded and used for inference.
+
+## 🛠️ Installation
+
+**ATOMMIC** is best to be installed in a Conda environment.
+
+### 🐍 Conda
+```
+conda create -n atommic python=3.10
+conda activate atommic
+```
+
+### 📦 Pip
+Use this installation mode if you want the latest released version.
+
+```bash
+pip install atommic
+```
+
+### From source
+
+Use this installation mode if you are contributing to atommic.
+
+```bash
+git clone https://github.com/wdika/atommic
+cd atommic
+bash ./reinstall.sh
+```
+
+### 🐳 Docker containers
 
-The trained model is an `.atommic` [module](../core/export.html), exported with [ONNX](https://onnx.ai/) and [TorchScript](https://pytorch.org/docs/stable/jit.html) support, which can be used for inference. The `.atommic` module can also be uploaded on [HuggingFace](https://huggingface.co/). Pretrained models are available on our [HF](https://huggingface.co/wdika) account and can be downloaded and used for inference.
+An atommic container is available at dockerhub, you can pull it with:
+```bash
+docker pull wdika/atommic
+```
+
+You can also build an atommic container with:
+```bash
+DOCKER_BUILDKIT=1 docker build -f Dockerfile -t atommic:latest .
+```
+
+You can run the container with:
+```bash
+docker run --gpus all -it --rm -v /home/user/configs:/config atommic:latest atommic run -c /config/config.yaml
+```
+where ```/config/config.yaml``` is the path to your local configuration file.
+
+Or you can run it interactively with:
+```bash
+docker run --gpus all -it --rm -p 8888:8888 atommic:latest /bin/bash -c "./start-jupyter.sh"
+```
 
 ## 🚀 Quick Start Guide
 
-The best way to get started with ATOMMIC is to start with one of the [tutorials](tutorials.html):
+The best way to get started with ATOMMIC is with one of the [tutorials](https://atommic.readthedocs.io/en/latest/starthere/tutorials.html):
+
+- [ATOMMIC Primer](https://github.com/wdika/atommic/blob/main/tutorials/00_ATOMMIC_Primer.ipynb) - demonstrates how to use ATOMMIC.
+- [ATOMMIC MRI transforms](https://github.com/wdika/atommic/blob/main/tutorials/01_ATOMMIC_MRI_transforms.ipynb) - demonstrates how to use ATOMMIC to undersample MRI data.
+- [ATOMMIC MRI undersampling](https://github.com/wdika/atommic/blob/main/tutorials/02_ATOMMIC_MRI_undersampling.ipynb) - demonstrates how to use ATOMMIC to apply transforms to MRI data.
+- [ATOMMIC Upload Model on HuggingFace](https://github.com/wdika/atommic/blob/main/tutorials/03_ATOMMIC_Upload_Model_On_HF.ipynb) - demonstrates how to upload a model on HuggingFace.
 
-- [ATOMMIC Primer](https://github.com/wdika/atommic/tutorials/00_ATOMMIC_Primer.ipynb) - demonstrates how to use ATOMMIC.
-- [ATOMMIC MRI transforms](https://github.com/wdika/atommic/tutorials/01_ATOMMIC_MRI_transforms.ipynb) - demonstrates how to use ATOMMIC to undersample MRI data.
-- [ATOMMIC MRI undersampling](https://github.com/wdika/atommic/tutorials/02_ATOMMIC_MRI_undersampling.ipynb) - demonstrates how to use ATOMMIC to apply transforms to MRI data.
-- [ATOMMIC Upload Model on HuggingFace](https://github.com/wdika/atommic/tutorials/03_ATOMMIC_Upload_Model_On_HF.ipynb) - demonstrates how to upload a model on HuggingFace.
+You can also check the [projects](https://github.com/wdika/atommic/tree/main/projects) page to see how to use ATOMMIC for specific tasks and public datasets.
 
-You can also check the [projects](projects.html) page to see how to use ATOMMIC for specific tasks and public datasets.
+Pre-trained models are available on HuggingFace [🤗](https://huggingface.co/wdika).
 
-### **ATOMMIC paper is fully reproducible. Please check [here](projects/ATOMMIC_paper/README.md) for more information.**
+### **ATOMMIC paper is fully reproducible. Please check [here](https://github.com/wdika/atommic/tree/main/projects/ATOMMIC_paper/README.md) for more information.**
 
 ## 🤖 Training & Testing
 
-Training and testing models in **ATOMMIC** is intuitive and easy. You just need to properly configure the `.yaml`
-file and just run the following command:
+Training and testing models in **ATOMMIC** is intuitive and easy. You just need to properly configure a `.yaml` file and run the following command:
 
 ```bash
 atommic run -c path-to-config-file
 ```
 
 ## ⚙️ Configuration
 
-1. Choose the **task** and the **model**, according to the [collections](../mri/collections.html).
+1. Choose the **task** and the **model**, according to the [collections](https://atommic.readthedocs.io/en/latest/mri/collections.html).
 
 2. Choose the **dataset** and the **dataset parameters**, according to the [datasets](README.md#mri-datasets) or your own dataset.
 
-3. Choose the [undersampling](../mri/transforms.html).
+3. Choose the [undersampling](https://atommic.readthedocs.io/en/latest/mri/transforms.html).
 
-4. Choose the [transforms](../mri/transforms.html).
+4. Choose the [transforms](https://atommic.readthedocs.io/en/latest/mri/transforms.html).
 
-5. Choose the [losses](../mri/losses.html).
+5. Choose the [losses](https://atommic.readthedocs.io/en/latest/mri/losses.html).
 
-6. Choose the [optimizer](../core/core.html#optimization).
+6. Choose the [optimizer](https://atommic.readthedocs.io/en/latest/core/core.html#optimization).
 
-7. Choose the [scheduler](../core/core.html#learning-rate-schedulers).
+7. Choose the [scheduler](https://atommic.readthedocs.io/en/latest/core/core.html#learning-rate-schedulers).
 
-8. Choose the [trainer parameters](../core/core.html#training).
+8. Choose the [trainer parameters](https://atommic.readthedocs.io/en/latest/core/core.html#training).
 
-9. Choose the [experiment manager](../core/exp_manager.html).
+9. Choose the [experiment manager](https://atommic.readthedocs.io/en/latest/core/exp_manager.html).
 
-You can also check the [projects](projects.html) page to see how to configure the `.yaml` file for specific tasks.
+You can also check the [projects](https://github.com/wdika/atommic/tree/main/projects/) page to see how to configure the `.yaml` file for specific tasks.
 
 ## 🗂️ Collections
 
-**ATOMMIC** is organized into [collections](../mri/collections.html), each of which implements a specific task. The following collections are currently available, implementing various models as listed:
+**ATOMMIC** is organized into [collections](https://atommic.readthedocs.io/en/latest/mri/collections.html), each of which implements a specific task. The following collections are currently available, implementing various models as listed:
 
 ### MultiTask Learning (MTL)
 1. End-to-End Recurrent Attention Network (`SERANet`), 2. Image domain Deep Structured Low-Rank Network (`IDSLR`), 3. Image domain Deep Structured Low-Rank UNet (`IDSLRUNet`), 4. Multi-Task Learning for MRI Reconstruction and Segmentation (`MTLRS`), 5. Reconstruction Segmentation method using UNet (`RecSegUNet`), 6. Segmentation Network MRI (`SegNet`).
 
 ### Quantitative MR Imaging (qMRI)
 1. Quantitative Recurrent Inference Machines (`qRIMBlock`), 2. Quantitative End-to-End Variational Network (`qVarNet`), 3. Quantitative Cascades of Independently Recurrent Inference Machines (`qCIRIM`).
 
@@ -119,100 +175,64 @@
 ### MRI Segmentation (SEG)
 1. `SegmentationAttentionUNet`, 2. `SegmentationDYNUNet`, 3. `SegmentationLambdaUNet`, 4. `SegmentationUNet`, 5. `Segmentation3DUNet`, 6. `SegmentationUNetR`, 7. `SegmentationVNet`.
 
 ## MRI Datasets
 
 **ATOMMIC** supports public datasets, as well as private datasets. The following public datasets are supported natively:
 
-- [AHEAD](projects/MTL/ahead.html): Supports the `(qMRI)` and `(REC)` tasks.
-- [BraTS 2023 Adult Glioma](projects/SEG/brats2023adultglioma.html): Supports the `(SEG)` task.
-- [CC359](projects/REC/cc359.html): Supports the `(REC)` task.
-- [fastMRI Brains Multicoil](projects/REC/fastmribrainsmulticoil.html): Supports the `(REC)` task.
-- [fastMRI Knees Multicoil](projects/REC/fastmrikneesmulticoil.html): Supports the `(REC)` task.
-- [fastMRI Knees Singlecoil](projects/REC/fastmrikneessinglecoil.html): Supports the `(REC)` task.
-- [ISLES 2022 Sub Acute Stroke](projects/SEG/isles2022subacutestroke.html): Supports the `(SEG)` task.
-- [SKM-TEA](projects/REC/skmtea.html): Supports the `(REC)`, `(SEG)`, and `(MTL)` tasks.
-- [Stanford Knees](projects/REC/stanfordknees2019.html): Supports the `(REC)` task.
-
-## 🛠️ Installation
-
-**ATOMMIC** is best to be installed in a Conda environment.
-
-### 🐍 Conda
-```
-conda create -n atommic python=3.10
-conda activate atommic
-```
-
-### 📦 Pip
-Use this installation mode if you want the latest released version.
-
-```bash
-pip install atommic
-```
-
-### From source
-
-Use this installation mode if you are contributing to atommic.
-
-```bash
-git clone https://github.com/wdika/atommic
-cd atommic
-bash ./reinstall.sh
-```
-
-### 🐳 Docker containers
-To build an atommic container with Dockerfile from a branch,  please run
-
-```bash
-  DOCKER_BUILDKIT=1 docker build -f Dockerfile -t atommic:latest.
-```
-
-As [NeMo](https://github.com/NVIDIA/NeMo) suggests, if you choose to work with the `main` branch, use NVIDIA's PyTorch container version [21.05-py3](https://ngc.nvidia.com/containers/nvidia:pytorch/tags), then install from GitHub.
-
-```bash
-    docker run --gpus all -it --rm -v <atommic_github_folder>:/ATOMMIC --shm-size=8g \
-    -p 8888:8888 -p 6006:6006 --ulimit memlock=-1 --ulimit \
-    stack=67108864 --device=/dev/snd nvcr.io/nvidia/pytorch:21.05-py3
-```
+- [AHEAD](https://github.com/wdika/atommic/tree/main/projects/qMRI/AHEAD): Supports the `(qMRI)` and `(REC)` tasks.
+- [BraTS 2023 Adult Glioma](https://github.com/wdika/atommic/tree/main/projects/SEG/BraTS2023AdultGlioma): Supports the `(SEG)` task.
+- [CC359](https://github.com/wdika/atommic/tree/main/projects/REC/CC359): Supports the `(REC)` task.
+- [fastMRI Brains Multicoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIBrainsMulticoil): Supports the `(REC)` task.
+- [fastMRI Knees Multicoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIKneesMulticoil): Supports the `(REC)` task.
+- [fastMRI Knees Singlecoil](https://github.com/wdika/atommic/tree/main/projects/REC/fastMRIKneesSinglecoil): Supports the `(REC)` task.
+- [ISLES 2022 Sub Acute Stroke](https://github.com/wdika/atommic/tree/main/projects/SEG/ISLES2022SubAcuteStroke): Supports the `(SEG)` task.
+- [SKM-TEA](https://github.com/wdika/atommic/tree/main/projects/MTL/rs/SKMTEA): Supports the `(REC)`, `(SEG)`, and `(MTL)` tasks.
+- [Stanford Knees](https://github.com/wdika/atommic/tree/main/projects/REC/StanfordKnees2019): Supports the `(REC)` task.
 
 ## 📚 API Documentation
 
 [![Documentation Status](https://readthedocs.org/projects/atommic/badge/?version=latest)](https://atommic.readthedocs.io/en/latest/?badge=latest)
 
 Access the API Documentation [here](https://atommic.readthedocs.io/en/latest/index.html)
 
 ## 📄 License
 
 **ATOMMIC** is under [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-
 ## 📖 Citation
 
 If you use ATOMMIC in your research, please cite as follows:
 
 ```BibTeX
-@misc{atommic,
-    author = {Karkalousos Dimitrios, Isqum Ivana, Marquering Henk, Caan Matthan},
-    title = {ATOMMIC: Advanced Toolbox for Multitask Medical Imaging Consistency},
-    year = {2023},
-    url = {https://github.com/wdika/atommic},
-}
+@article{Karkalousos_2024,
+   title={Atommic: An Advanced Toolbox for Multitask Medical Imaging Consistency to Facilitate Artificial Intelligence Applications from Acquisition to Analysis in Magnetic Resonance Imaging},
+   url={http://dx.doi.org/10.2139/ssrn.4801289},
+   DOI={10.2139/ssrn.4801289},
+   publisher={Elsevier BV},
+   author={Karkalousos, Dimitrios and Išgum, Ivana and Marquering, Henk and Caan, Matthan  W.A.},
+   year={2024}}
 ```
 
 ## 🔗 References
 
-The following papers have used ATOMMIC:
+ATOMMIC has been used or is referenced in the following papers:
+
+1. Karkalousos, Dimitrios and Išgum, Ivana and Marquering, Henk and Caan, Matthan W.A., Atommic: An Advanced Toolbox for Multitask Medical Imaging Consistency to Facilitate Artificial Intelligence Applications from Acquisition to Analysis in Magnetic Resonance Imaging. Available at SSRN: https://ssrn.com/abstract=4801289 or http://dx.doi.org/10.2139/ssrn.4801289
+
+2. Karkalousos, D., Išgum, I., Marquering, H. A., & Caan, M. W. A. (2024). ATOMMIC: An Advanced Toolbox for Multitask Medical Imaging Consistency to facilitate Artificial Intelligence applications from acquisition to analysis in Magnetic Resonance Imaging. https://doi.org/10.2139/ssrn.4801289
+
+3. Karkalousos, D., Isgum, I., Marquering, H., & Caan, M. W. A. (2024, April 27). The Advanced Toolbox for Multitask Medical Imaging Consistency (ATOMMIC): A Deep Learning framework to facilitate Magnetic Resonance Imaging. Medical Imaging with Deep Learning. https://openreview.net/forum?id=HxTZr9yA0N
 
-1. Karkalousos, D., Isgum, I., Marquering, H. &amp; Caan, M.W.A.. (2024). MultiTask Learning for accelerated-MRI Reconstruction and Segmentation of Brain Lesions in Multiple Sclerosis. <i>Medical Imaging with Deep Learning</i>, in <i>Proceedings of Machine Learning Research</i> 227:991-1005 Available from https://proceedings.mlr.press/v227/karkalousos24a.html.
+4. Karkalousos, D., Isgum, I., Marquering, H. &amp; Caan, M.W.A.. (2024). MultiTask Learning for accelerated-MRI Reconstruction and Segmentation of Brain Lesions in Multiple Sclerosis. <i>Medical Imaging with Deep Learning</i>, in <i>Proceedings of Machine Learning Research</i> 227:991-1005 Available from https://proceedings.mlr.press/v227/karkalousos24a.html.
 
-2. Zhang, C., Karkalousos, D., Bazin, P. L., Coolen, B. F., Vrenken, H., Sonke, J. J., Forstmann, B. U., Poot, D. H. J., & Caan, M. W. A. (2022). A unified model for reconstruction and R2* mapping of accelerated 7T data using the quantitative recurrent inference machine. NeuroImage, 264. [DOI](https://doi.org/10.1016/j.neuroimage.2022.119680)
+5. Zhang, C., Karkalousos, D., Bazin, P. L., Coolen, B. F., Vrenken, H., Sonke, J. J., Forstmann, B. U., Poot, D. H. J., & Caan, M. W. A. (2022). A unified model for reconstruction and R2* mapping of accelerated 7T data using the quantitative recurrent inference machine. NeuroImage, 264. [DOI](https://doi.org/10.1016/j.neuroimage.2022.119680)
 
-3. Karkalousos, D., Noteboom, S., Hulst, H. E., Vos, F. M., & Caan, M. W. A. (2022). Assessment of data consistency through cascades of independently recurrent inference machines for fast and robust accelerated MRI reconstruction. Physics in Medicine & Biology. [DOI](https://doi.org/10.1088/1361-6560/AC6CC2)
+6. Karkalousos, D., Noteboom, S., Hulst, H. E., Vos, F. M., & Caan, M. W. A. (2022). Assessment of data consistency through cascades of independently recurrent inference machines for fast and robust accelerated MRI reconstruction. Physics in Medicine & Biology. [DOI](https://doi.org/10.1088/1361-6560/AC6CC2)
 
 ## 📧 Contact
 
 For any questions, please contact Dimitris Karkalousos @ [d.karkalousos@amsterdamumc.nl](mailto:d.karkalousos@amsterdamumc.nl).
 
 ## ⚠️🙏 Disclaimer & Acknowledgements
 
-> **Note:** ATOMMIC is built on top of [NeMo](https://github.com/NVIDIA/NeMo). NeMo is under Apache 2.0 license, so we are allowed to use it. We also assume that it is allowed to use the NeMo documentation, as long as we cite it and we always refer to the baselines everywhere and in the code and docs. ATOMMIC also includes implementations of reconstruction methods from [fastMRI](https://github.com/facebookresearch/fastMRI) and [DIRECT](https://github.com/NKI-AI/direct), and segmentation methods from [MONAI](https://github.com/Project-MONAI/MONAI), as well as other codebases which are always cited on the corresponding files. All methods in ATOMMIC are reimplemented and not called from the original libraries, allowing for full reproducibility, support, and easy extension. ATOMMIC is an open-source project under the Apache 2.0 license.
+> **Note:** ATOMMIC is built on top of [NeMo](https://github.com/NVIDIA/NeMo). NeMo is under Apache 2.0 license, so we are allowed to use it. We also assume that we can use the NeMo documentation basis as long as we cite it and always refer to the baselines everywhere in the code and docs. ATOMMIC also includes implementations of reconstruction methods from [fastMRI](https://github.com/facebookresearch/fastMRI) and [DIRECT](https://github.com/NKI-AI/direct), and segmentation methods from [MONAI](https://github.com/Project-MONAI/MONAI), as well as other codebases which are always cited on the corresponding files. All methods in ATOMMIC are reimplemented and not called from the original libraries, allowing for full reproducibility, support, and easy extension. ATOMMIC is an open-source project under the Apache 2.0 license.
```

### Comparing `atommic-1.0.0/atommic.egg-info/SOURCES.txt` & `atommic-1.0.1/atommic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/pyproject.toml` & `atommic-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/setup.cfg` & `atommic-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `atommic-1.0.0/setup.py` & `atommic-1.0.1/setup.py`

 * *Files identical despite different names*

