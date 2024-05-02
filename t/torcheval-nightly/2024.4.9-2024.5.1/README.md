# Comparing `tmp/torcheval-nightly-2024.4.9.tar.gz` & `tmp/torcheval-nightly-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcheval-nightly-2024.4.9.tar", last modified: Tue Apr  9 12:09:19 2024, max compression
+gzip compressed data, was "torcheval-nightly-2024.5.1.tar", last modified: Wed May  1 12:08:18 2024, max compression
```

## Comparing `torcheval-nightly-2024.4.9.tar` & `torcheval-nightly-2024.5.1.tar`

### file list

```diff
@@ -1,143 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.531278 torcheval-nightly-2024.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-09 12:09:19.531278 torcheval-nightly-2024.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:09:19.531278 torcheval-nightly-2024.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.511278 torcheval-nightly-2024.4.9/torcheval/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.515278 torcheval-nightly-2024.4.9/torcheval/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.515278 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/max.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/min.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.515278 torcheval-nightly-2024.4.9/torcheval/metrics/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/audio/fad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.519279 torcheval-nightly-2024.4.9/torcheval/metrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/classification/recall_at_fixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.519279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.519279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.519279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    24115 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.523279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/image/psnr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.523279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/num_collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/retrieval_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/retrieval_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.523279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/regression/r2_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.523279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/statistical/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/statistical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/statistical/wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.523279 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/word_information_preserved.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.527279 torcheval-nightly-2024.4.9/torcheval/metrics/image/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.527279 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/retrieval_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/retrieval_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.527279 torcheval-nightly-2024.4.9/torcheval/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/regression/r2_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.527279 torcheval-nightly-2024.4.9/torcheval/metrics/statistical/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/statistical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/statistical/wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/synclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.527279 torcheval-nightly-2024.4.9/torcheval/metrics/text/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/text/word_information_preserved.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.527279 torcheval-nightly-2024.4.9/torcheval/metrics/window/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/window/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/window/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/window/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/window/normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/metrics/window/weighted_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.531278 torcheval-nightly-2024.4.9/torcheval/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/utils/random_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.531278 torcheval-nightly-2024.4.9/torcheval/utils/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/utils/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/utils/test_utils/dummy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/utils/test_utils/metric_class_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 12:02:01.000000 torcheval-nightly-2024.4.9/torcheval/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:09:19.531278 torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-09 12:09:19.000000 torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-09 12:09:19.000000 torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:09:19.000000 torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-09 12:09:19.000000 torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 12:09:19.000000 torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:09:19.000000 torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.978351 torcheval-nightly-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-01 12:08:18.978351 torcheval-nightly-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:08:18.978351 torcheval-nightly-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.962351 torcheval-nightly-2024.5.1/torcheval/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.962351 torcheval-nightly-2024.5.1/torcheval/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.962351 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.962351 torcheval-nightly-2024.5.1/torcheval/metrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/audio/fad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.966351 torcheval-nightly-2024.5.1/torcheval/metrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/classification/recall_at_fixed_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.966351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.966351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.966351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24115 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/frechet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.970351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/image/psnr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.970351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/num_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/retrieval_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/retrieval_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.970351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/regression/r2_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.970351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/statistical/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/statistical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/statistical/wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.970351 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/word_information_preserved.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.970351 torcheval-nightly-2024.5.1/torcheval/metrics/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.974351 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/retrieval_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/retrieval_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.974351 torcheval-nightly-2024.5.1/torcheval/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/regression/r2_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.974351 torcheval-nightly-2024.5.1/torcheval/metrics/statistical/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/statistical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/statistical/wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/synclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.974351 torcheval-nightly-2024.5.1/torcheval/metrics/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/text/word_information_preserved.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.974351 torcheval-nightly-2024.5.1/torcheval/metrics/window/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/window/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/window/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/window/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/window/normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/metrics/window/weighted_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.974351 torcheval-nightly-2024.5.1/torcheval/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/utils/random_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.978351 torcheval-nightly-2024.5.1/torcheval/utils/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/utils/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/utils/test_utils/dummy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/utils/test_utils/metric_class_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-01 12:01:17.000000 torcheval-nightly-2024.5.1/torcheval/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:08:18.978351 torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-01 12:08:18.000000 torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-01 12:08:18.000000 torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:08:18.000000 torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-01 12:08:18.000000 torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 12:08:18.000000 torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:08:18.000000 torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/zip-safe
```

### Comparing `torcheval-nightly-2024.4.9/LICENSE` & `torcheval-nightly-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/PKG-INFO` & `torcheval-nightly-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2024.4.9
+Version: 2024.5.1
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.4.9 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.5.1 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torcheval-nightly-2024.4.9/README.md` & `torcheval-nightly-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/setup.py` & `torcheval-nightly-2024.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/auc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/auc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/cat.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/cat.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/max.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/max.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/mean.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/mean.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/min.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/min.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/sum.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/sum.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/aggregation/throughput.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/audio/fad.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/audio/fad.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,34 +6,20 @@
 
 # pyre-strict
 
 import copy
 from typing import Any, Callable, Iterable, Optional, Union
 
 import torch
-
-try:
-    from torchaudio.functional import frechet_distance
-
-    _TORCHAUDIO_AVAILABLE = True
-except ImportError:
-    _TORCHAUDIO_AVAILABLE = False
-
+from torcheval.metrics.functional.frechet import gaussian_frechet_distance
 from torcheval.metrics.metric import Metric
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 
-def _validate_torchaudio_available() -> None:
-    if not _TORCHAUDIO_AVAILABLE:
-        raise RuntimeError(
-            "TorchAudio is required. Please make sure ``torchaudio`` is installed."
-        )
-
-
 class FrechetAudioDistance(Metric[torch.Tensor]):
     """Computes the Fréchet distance between predicted and target audio waveforms.
 
     Original paper: https://arxiv.org/abs/1812.08466
 
     Args:
         preproc (Callable[[torch.Tensor], torch.Tensor]): Callable for preprocessing waveforms prior to passing to model.
@@ -46,16 +32,14 @@
     def __init__(
         self,
         preproc: Callable[[torch.Tensor], torch.Tensor],
         model: torch.nn.Module,
         embedding_dim: int,
         device: Optional[torch.device] = None,
     ) -> None:
-        _validate_torchaudio_available()
-
         super().__init__(device=device)
 
         self.preproc = preproc
         # pyre-ignore
         self.model = model.to(device)
         self.model.eval()
         self.model.requires_grad_(False)
@@ -116,16 +100,21 @@
         target_cov = self.target_cov_partial / (self.target_n - 1) - target_mean.T @ (
             target_mean
         ) * self.target_n / (self.target_n - 1)
         pred_mean = self.pred_mean_partial / self.pred_n
         pred_cov = self.pred_cov_partial / (self.pred_n - 1) - pred_mean.T @ (
             pred_mean
         ) * self.pred_n / (self.pred_n - 1)
-        return frechet_distance(
-            pred_mean.squeeze(0), pred_cov, target_mean.squeeze(0), target_cov
+        return gaussian_frechet_distance(
+            pred_mean.squeeze(0),
+            # pyre-fixme[6]: For 2nd argument expected `Tensor` but got `float`.
+            pred_cov,
+            target_mean.squeeze(0),
+            # pyre-fixme[6]: For 4th argument expected `Tensor` but got `float`.
+            target_cov,
         )
 
     @torch.inference_mode()
     # pyre-ignore[14]: inconsistent override on *_:Any, **__:Any
     def merge_state(
         self, fads: Iterable["FrechetAudioDistance"]
     ) -> "FrechetAudioDistance":
@@ -161,15 +150,14 @@
         Args:
             device (torch.device or None, optional): Device where computations will be performed.
                 If `None`, the default device will be used. (Default: `None`)
 
         Returns:
             FrechetAudioDistance: Instance of FrechetAudioDistance preloaded with TorchAudio's pretrained VGGish model.
         """
-        _validate_torchaudio_available()
         try:
             from torchaudio.prototype.pipelines import VGGISH
         except ImportError:
             raise RuntimeError(
                 "Using the pretrained VGGish model requires the TorchAudio nightly binary as it is a prototype feature. "
                 "Please install the latest nightly version of ``torchaudio``."
             )
```

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/accuracy.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/auprc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/auroc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/binary_normalized_entropy.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/binary_normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/binned_auprc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/binned_auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/binned_auroc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/binned_auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/binned_precision_recall_curve.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/binned_precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/confusion_matrix.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/f1_score.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/precision.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/precision_recall_curve.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/recall.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/classification/recall_at_fixed_precision.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     multilabel_auprc,
     multilabel_binned_auprc,
     multilabel_binned_precision_recall_curve,
     multilabel_precision_recall_curve,
     multilabel_recall_at_fixed_precision,
     topk_multilabel_accuracy,
 )
+from torcheval.metrics.functional.frechet import gaussian_frechet_distance
 from torcheval.metrics.functional.image import peak_signal_noise_ratio
 from torcheval.metrics.functional.ranking import (
     click_through_rate,
     frequency_at_k,
     hit_rate,
     num_collisions,
     reciprocal_rank,
@@ -74,14 +75,15 @@
     "binary_precision",
     "binary_precision_recall_curve",
     "binary_recall",
     "binary_recall_at_fixed_precision",
     "bleu_score",
     "click_through_rate",
     "frequency_at_k",
+    "gaussian_frechet_distance",
     "hit_rate",
     "mean",
     "mean_squared_error",
     "multiclass_accuracy",
     "multiclass_auprc",
     "multiclass_auroc",
     "multiclass_binned_auprc",
```

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/auc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/auc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/mean.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/mean.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/sum.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/sum.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/aggregation/throughput.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/accuracy.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/auprc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/auroc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binary_normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binned_auprc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binned_auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binned_auroc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binned_auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/binned_precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/confusion_matrix.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/f1_score.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/precision.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/precision_recall_curve.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/recall.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/image/psnr.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/click_through_rate.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/frequency.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/frequency.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/hit_rate.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/num_collisions.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/num_collisions.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/reciprocal_rank.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/retrieval_precision.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/retrieval_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/retrieval_recall.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/retrieval_recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/ranking/weighted_calibration.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/ranking/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/regression/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/regression/mean_squared_error.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/regression/r2_score.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/statistical/wasserstein.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/statistical/wasserstein.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/tensor_utils.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/bleu.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/helper.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/perplexity.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/word_error_rate.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/word_information_lost.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/word_information_lost.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/functional/text/word_information_preserved.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/functional/text/word_information_preserved.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/image/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/image/fid.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/image/fid.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import warnings
 from importlib.util import find_spec
 from typing import Any, Iterable, Optional, TypeVar, Union
 
 import torch
 import torch.nn.functional as F
 from torch import nn, Tensor
+from torcheval.metrics.functional.frechet import gaussian_frechet_distance
 from torcheval.metrics.metric import Metric
 
 if find_spec("torchvision") is not None:
     from torchvision import models
 
     _TORCHVISION_AVAILABLE = True
 else:
@@ -192,59 +193,19 @@
         real_cov = real_cov_num / (self.num_real_images - 1)
         fake_cov_num = self.fake_cov_sum - self.num_fake_images * torch.matmul(
             fake_mean.T, fake_mean
         )
         fake_cov = fake_cov_num / (self.num_fake_images - 1)
 
         # Compute the Frechet Distance between the distributions
-        fid = self._calculate_frechet_distance(
+        fid = gaussian_frechet_distance(
             real_mean.squeeze(), real_cov, fake_mean.squeeze(), fake_cov
         )
         return fid
 
-    def _calculate_frechet_distance(
-        self: TFrechetInceptionDistance,
-        mu1: Tensor,
-        sigma1: Tensor,
-        mu2: Tensor,
-        sigma2: Tensor,
-    ) -> Tensor:
-        """
-        Calculate the Frechet Distance between two multivariate Gaussian distributions.
-
-        Args:
-            mu1 (Tensor): The mean of the first distribution.
-            sigma1 (Tensor): The covariance matrix of the first distribution.
-            mu2 (Tensor): The mean of the second distribution.
-            sigma2 (Tensor): The covariance matrix of the second distribution.
-
-        Returns:
-            tensor: The Frechet Distance between the two distributions.
-        """
-
-        # Compute the squared distance between the means
-        mean_diff = mu1 - mu2
-        mean_diff_squared = mean_diff.square().sum(dim=-1)
-
-        # Calculate the sum of the traces of both covariance matrices
-        trace_sum = sigma1.trace() + sigma2.trace()
-
-        # Compute the eigenvalues of the matrix product of the real and fake covariance matrices
-        sigma_mm = torch.matmul(sigma1, sigma2)
-        eigenvals = torch.linalg.eigvals(sigma_mm)
-
-        # Take the square root of each eigenvalue and take its sum
-        sqrt_eigenvals_sum = eigenvals.sqrt().real.sum(dim=-1)
-
-        # Calculate the FID using the squared distance between the means,
-        # the sum of the traces of the covariance matrices, and the sum of the square roots of the eigenvalues
-        fid = mean_diff_squared + trace_sum - 2 * sqrt_eigenvals_sum
-
-        return fid
-
     def _FID_parameter_check(
         self: TFrechetInceptionDistance,
         model: Optional[nn.Module],
         feature_dim: int,
     ) -> None:
         # Whatever the model, the feature_dim needs to be set
         if feature_dim is None or feature_dim <= 0:
```

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/image/psnr.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/image/psnr.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 TPeakSignalNoiseRatio = TypeVar("TPeakSignalNoiseRatio")
 
 
 class PeakSignalNoiseRatio(Metric[torch.Tensor]):
     """
     Compute the PSNR (Peak Signal to Noise Ratio) between two images.
-    Its functional version is `torcheval.metrics.functional.psnr`
+    Its functional version is `torcheval.metrics.functional.peak_signal_noise_ratio`
 
     Args:
         data_range (float): the range of the input images. Default: None.
             If ``None``, the range computed from the target data ``(target.max() - targert.min())``.
 
     Examples::
```

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/image/ssim.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/metric.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/ranking/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/ranking/click_through_rate.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/ranking/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/ranking/hit_rate.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/ranking/reciprocal_rank.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/ranking/retrieval_precision.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/ranking/retrieval_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/ranking/retrieval_recall.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/ranking/retrieval_recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/ranking/weighted_calibration.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/ranking/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/regression/mean_squared_error.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/regression/r2_score.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/statistical/wasserstein.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/statistical/wasserstein.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/synclib.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/synclib.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,18 @@
     tensors are padded, gathered and then trimmed to secure equal workload
     for all processes.
 
     Return:
         gathered_result: list with size equal to the process group where
             gathered_result[i] corresponds to result tensor from process i
     """
+    # TODO investigate why this stopped working (can cause hangs)
     # if the backend is NCCL, we can gather the differently sized tensors without padding
-    if dist.get_backend(group) == "nccl":
-        return _simple_send_tensors(tensor, world_size, group, rank=rank)
+    # if dist.get_backend(group) == "nccl":
+    #     return _simple_send_tensors(tensor, world_size, group, rank=rank)
 
     # gather sizes of all tensors on all ranks
     local_size = torch.tensor(tensor.shape, device=tensor.device)
     local_sizes = _simple_send_tensors(local_size, world_size, group, rank=None)
     assert local_sizes is not None
 
     # if shapes are all the same, then do a simple gather:
```

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/text/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/text/bleu.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/text/perplexity.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/text/word_error_rate.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/text/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/text/word_information_lost.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/text/word_information_lost.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/text/word_information_preserved.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/text/word_information_preserved.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/toolkit.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/toolkit.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/window/__init__.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/window/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/window/auroc.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/window/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/window/click_through_rate.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/window/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/window/mean_squared_error.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/window/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/window/normalized_entropy.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/window/normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/metrics/window/weighted_calibration.py` & `torcheval-nightly-2024.5.1/torcheval/metrics/window/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/utils/random_data.py` & `torcheval-nightly-2024.5.1/torcheval/utils/random_data.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/utils/test_utils/dummy_metric.py` & `torcheval-nightly-2024.5.1/torcheval/utils/test_utils/dummy_metric.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/utils/test_utils/metric_class_tester.py` & `torcheval-nightly-2024.5.1/torcheval/utils/test_utils/metric_class_tester.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval/version.py` & `torcheval-nightly-2024.5.1/torcheval/version.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/PKG-INFO` & `torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2024.4.9
+Version: 2024.5.1
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.4.9 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.5.1 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torcheval-nightly-2024.4.9/torcheval_nightly.egg-info/SOURCES.txt` & `torcheval-nightly-2024.5.1/torcheval_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 torcheval/metrics/classification/confusion_matrix.py
 torcheval/metrics/classification/f1_score.py
 torcheval/metrics/classification/precision.py
 torcheval/metrics/classification/precision_recall_curve.py
 torcheval/metrics/classification/recall.py
 torcheval/metrics/classification/recall_at_fixed_precision.py
 torcheval/metrics/functional/__init__.py
+torcheval/metrics/functional/frechet.py
 torcheval/metrics/functional/tensor_utils.py
 torcheval/metrics/functional/aggregation/__init__.py
 torcheval/metrics/functional/aggregation/auc.py
 torcheval/metrics/functional/aggregation/mean.py
 torcheval/metrics/functional/aggregation/sum.py
 torcheval/metrics/functional/aggregation/throughput.py
 torcheval/metrics/functional/classification/__init__.py
```

