# Comparing `tmp/sxmp-mule-1.1.0.tar.gz` & `tmp/sxmp_mule-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sxmp-mule-1.1.0.tar", last modified: Tue Jan 31 03:19:21 2023, max compression
+gzip compressed data, was "sxmp_mule-1.1.1.tar", last modified: Wed May  1 23:13:30 2024, max compression
```

## Comparing `sxmp-mule-1.1.0.tar` & `sxmp_mule-1.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.976494 sxmp-mule-1.1.0/
--rw-r--r--   0 mmccallum   (502) staff       (20)    35126 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/LICENSE
--rw-r--r--   0 mmccallum   (502) staff       (20)     2698 2023-01-31 03:19:21.975867 sxmp-mule-1.1.0/PKG-INFO
--rw-r--r--   0 mmccallum   (502) staff       (20)     3771 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/README.md
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.912565 sxmp-mule-1.1.0/mule/
--rw-r--r--   0 mmccallum   (502) staff       (20)      633 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2013 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/mule/analysis.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.915971 sxmp-mule-1.1.0/mule/cli/
--rw-r--r--   0 mmccallum   (502) staff       (20)      625 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/cli/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1188 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/cli/cli.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1599 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/cli/options.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.921406 sxmp-mule-1.1.0/mule/extractors/
--rw-r--r--   0 mmccallum   (502) staff       (20)      724 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/extractors/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1488 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/extractors/block_extractor.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2379 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/extractors/extractor.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     4332 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/extractors/slice_extractor.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.924089 sxmp-mule-1.1.0/mule/features/
--rw-r--r--   0 mmccallum   (502) staff       (20)      814 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/features/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     3477 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/mule/features/feature.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.928309 sxmp-mule-1.1.0/mule/features/source_features/
--rw-r--r--   0 mmccallum   (502) staff       (20)      687 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/features/source_features/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     3009 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/features/source_features/audio_waveform.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2109 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/mule/features/source_features/source_feature.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.938003 sxmp-mule-1.1.0/mule/features/transform_features/
--rw-r--r--   0 mmccallum   (502) staff       (20)      789 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/mule/features/transform_features/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     3026 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/features/transform_features/embedding_feature.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     4949 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/features/transform_features/mel_spectrogram.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2291 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/mule/features/transform_features/timeline_average.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2750 2022-12-15 03:42:39.000000 sxmp-mule-1.1.0/mule/features/transform_features/transform_feature.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.943469 sxmp-mule-1.1.0/mule/models/
--rw-r--r--   0 mmccallum   (502) staff       (20)      682 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/__init__.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.960717 sxmp-mule-1.1.0/mule/models/layers/
--rw-r--r--   0 mmccallum   (502) staff       (20)      741 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/layers/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2801 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/layers/scalar_multiply.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     4219 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/layers/stoch_depth.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     6073 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/layers/weight_standardization.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.963321 sxmp-mule-1.1.0/mule/models/losses/
--rw-r--r--   0 mmccallum   (502) staff       (20)     1147 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/losses/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1476 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/losses/loss.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     6278 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/losses/sim_clr_loss.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.964952 sxmp-mule-1.1.0/mule/models/metrics/
--rw-r--r--   0 mmccallum   (502) staff       (20)     1117 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/metrics/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1049 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/metrics/train_metric.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     3760 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/mlp.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     3876 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/model.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.966318 sxmp-mule-1.1.0/mule/models/optimizers/
--rw-r--r--   0 mmccallum   (502) staff       (20)     1141 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/optimizers/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1707 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/optimizers/optimizer.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.968649 sxmp-mule-1.1.0/mule/models/optimizers/schedules/
--rw-r--r--   0 mmccallum   (502) staff       (20)     1197 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/optimizers/schedules/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1441 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/optimizers/schedules/lr_schedule.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     2662 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/optimizers/schedules/warmup_schedule.py
--rw-r--r--   0 mmccallum   (502) staff       (20)    34248 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/models/sfnfnetf0.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.970704 sxmp-mule-1.1.0/mule/source_files/
--rw-r--r--   0 mmccallum   (502) staff       (20)      673 2022-12-03 06:33:52.000000 sxmp-mule-1.1.0/mule/source_files/__init__.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     7246 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/mule/source_files/audio_file.py
--rw-r--r--   0 mmccallum   (502) staff       (20)     1856 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/mule/source_files/source_file.py
--rw-r--r--   0 mmccallum   (502) staff       (20)       38 2023-01-31 03:19:21.976647 sxmp-mule-1.1.0/setup.cfg
--rw-r--r--   0 mmccallum   (502) staff       (20)     3888 2023-01-31 03:14:51.000000 sxmp-mule-1.1.0/setup.py
-drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2023-01-31 03:19:21.975082 sxmp-mule-1.1.0/sxmp_mule.egg-info/
--rw-r--r--   0 mmccallum   (502) staff       (20)     2698 2023-01-31 03:19:21.000000 sxmp-mule-1.1.0/sxmp_mule.egg-info/PKG-INFO
--rw-r--r--   0 mmccallum   (502) staff       (20)     1600 2023-01-31 03:19:21.000000 sxmp-mule-1.1.0/sxmp_mule.egg-info/SOURCES.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)        1 2023-01-31 03:19:21.000000 sxmp-mule-1.1.0/sxmp_mule.egg-info/dependency_links.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)       39 2023-01-31 03:19:21.000000 sxmp-mule-1.1.0/sxmp_mule.egg-info/entry_points.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)       61 2023-01-31 03:19:21.000000 sxmp-mule-1.1.0/sxmp_mule.egg-info/requires.txt
--rw-r--r--   0 mmccallum   (502) staff       (20)        5 2023-01-31 03:19:21.000000 sxmp-mule-1.1.0/sxmp_mule.egg-info/top_level.txt
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.616347 sxmp_mule-1.1.1/
+-rw-r--r--   0 mmccallum   (502) staff       (20)    35126 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/LICENSE
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2884 2024-05-01 23:13:30.616129 sxmp_mule-1.1.1/PKG-INFO
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3771 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/README.md
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.603614 sxmp_mule-1.1.1/mule/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      633 2024-05-01 23:10:43.000000 sxmp_mule-1.1.1/mule/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2013 2024-05-01 23:10:54.000000 sxmp_mule-1.1.1/mule/analysis.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.604418 sxmp_mule-1.1.1/mule/cli/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      625 2024-05-01 23:10:50.000000 sxmp_mule-1.1.1/mule/cli/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1188 2024-05-01 23:10:58.000000 sxmp_mule-1.1.1/mule/cli/cli.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1599 2024-05-01 23:11:01.000000 sxmp_mule-1.1.1/mule/cli/options.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.605759 sxmp_mule-1.1.1/mule/extractors/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      724 2024-05-01 23:11:05.000000 sxmp_mule-1.1.1/mule/extractors/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1488 2024-05-01 23:11:15.000000 sxmp_mule-1.1.1/mule/extractors/block_extractor.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2379 2024-05-01 23:11:10.000000 sxmp_mule-1.1.1/mule/extractors/extractor.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     4332 2024-05-01 23:11:20.000000 sxmp_mule-1.1.1/mule/extractors/slice_extractor.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.606280 sxmp_mule-1.1.1/mule/features/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      814 2024-05-01 23:10:19.000000 sxmp_mule-1.1.1/mule/features/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3477 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/feature.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.607131 sxmp_mule-1.1.1/mule/features/source_features/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      687 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/source_features/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3009 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/source_features/audio_waveform.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2109 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/source_features/source_feature.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.609105 sxmp_mule-1.1.1/mule/features/transform_features/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      789 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/transform_features/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3026 2024-05-01 23:10:19.000000 sxmp_mule-1.1.1/mule/features/transform_features/embedding_feature.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     4949 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/transform_features/mel_spectrogram.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2291 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/transform_features/timeline_average.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2750 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/features/transform_features/transform_feature.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.609826 sxmp_mule-1.1.1/mule/models/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      682 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/__init__.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.611382 sxmp_mule-1.1.1/mule/models/layers/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      741 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/layers/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2801 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/layers/scalar_multiply.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     4219 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/layers/stoch_depth.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     6073 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/layers/weight_standardization.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.612046 sxmp_mule-1.1.1/mule/models/losses/
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1147 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/losses/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1476 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/losses/loss.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     6278 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/losses/sim_clr_loss.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.612588 sxmp_mule-1.1.1/mule/models/metrics/
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1117 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/metrics/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1049 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/metrics/train_metric.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3760 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/mlp.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     3876 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/model.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.612982 sxmp_mule-1.1.1/mule/models/optimizers/
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1141 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/optimizers/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1707 2024-05-01 23:10:19.000000 sxmp_mule-1.1.1/mule/models/optimizers/optimizer.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.613730 sxmp_mule-1.1.1/mule/models/optimizers/schedules/
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1197 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/optimizers/schedules/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1441 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/optimizers/schedules/lr_schedule.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2662 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/optimizers/schedules/warmup_schedule.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)    34248 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/models/sfnfnetf0.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.614468 sxmp_mule-1.1.1/mule/source_files/
+-rw-r--r--   0 mmccallum   (502) staff       (20)      673 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/source_files/__init__.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     7246 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/source_files/audio_file.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1856 2024-05-01 18:46:32.000000 sxmp_mule-1.1.1/mule/source_files/source_file.py
+-rw-r--r--   0 mmccallum   (502) staff       (20)       38 2024-05-01 23:13:30.616482 sxmp_mule-1.1.1/setup.cfg
+-rw-r--r--   0 mmccallum   (502) staff       (20)     4370 2024-05-01 23:12:08.000000 sxmp_mule-1.1.1/setup.py
+drwxr-xr-x   0 mmccallum   (502) staff       (20)        0 2024-05-01 23:13:30.615756 sxmp_mule-1.1.1/sxmp_mule.egg-info/
+-rw-r--r--   0 mmccallum   (502) staff       (20)     2884 2024-05-01 23:13:30.000000 sxmp_mule-1.1.1/sxmp_mule.egg-info/PKG-INFO
+-rw-r--r--   0 mmccallum   (502) staff       (20)     1600 2024-05-01 23:13:30.000000 sxmp_mule-1.1.1/sxmp_mule.egg-info/SOURCES.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)        1 2024-05-01 23:13:30.000000 sxmp_mule-1.1.1/sxmp_mule.egg-info/dependency_links.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)       39 2024-05-01 23:13:30.000000 sxmp_mule-1.1.1/sxmp_mule.egg-info/entry_points.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)       96 2024-05-01 23:13:30.000000 sxmp_mule-1.1.1/sxmp_mule.egg-info/requires.txt
+-rw-r--r--   0 mmccallum   (502) staff       (20)        5 2024-05-01 23:13:30.000000 sxmp_mule-1.1.1/sxmp_mule.egg-info/top_level.txt
```

### Comparing `sxmp-mule-1.1.0/LICENSE` & `sxmp_mule-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/PKG-INFO` & `sxmp_mule-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sxmp-mule
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/PandoraMedia/music-audio-representations
 Author: Matt C. McCallum
 Author-email: mmccallum@pandora.com
 License: GNU GPL 3.0
 Project-URL: Documentation, https://github.com/PandoraMedia/music-audio-representations
 Project-URL: Bug Reports, https://github.com/PandoraMedia/music-audio-representations/issues
 Project-URL: Source, https://github.com/PandoraMedia/music-audio-representations
@@ -19,14 +19,20 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: librosa==0.9.2
+Requires-Dist: click==8.1.7
+Requires-Dist: scooch>=1.0.4
+Requires-Dist: tensorflow-macos==2.9.1
+Requires-Dist: tensorflow-metal==0.5.0
 
 
 # MULE
 
 The Musicset Unsupervised Large Embedding (MULE) module is your 
 music-audio workhorse!
```

### Comparing `sxmp-mule-1.1.0/README.md` & `sxmp_mule-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/__init__.py` & `sxmp_mule-1.1.1/mule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/analysis.py` & `sxmp_mule-1.1.1/mule/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/cli/__init__.py` & `sxmp_mule-1.1.1/mule/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/cli/cli.py` & `sxmp_mule-1.1.1/mule/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/cli/options.py` & `sxmp_mule-1.1.1/mule/cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/extractors/__init__.py` & `sxmp_mule-1.1.1/mule/extractors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/extractors/block_extractor.py` & `sxmp_mule-1.1.1/mule/extractors/block_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/extractors/extractor.py` & `sxmp_mule-1.1.1/mule/extractors/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/extractors/slice_extractor.py` & `sxmp_mule-1.1.1/mule/extractors/slice_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
```

### Comparing `sxmp-mule-1.1.0/mule/features/__init__.py` & `sxmp_mule-1.1.1/mule/features/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/feature.py` & `sxmp_mule-1.1.1/mule/features/feature.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/source_features/__init__.py` & `sxmp_mule-1.1.1/mule/features/source_features/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/source_features/audio_waveform.py` & `sxmp_mule-1.1.1/mule/features/source_features/audio_waveform.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/source_features/source_feature.py` & `sxmp_mule-1.1.1/mule/features/source_features/source_feature.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/transform_features/__init__.py` & `sxmp_mule-1.1.1/mule/features/transform_features/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/transform_features/embedding_feature.py` & `sxmp_mule-1.1.1/mule/features/transform_features/embedding_feature.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/transform_features/mel_spectrogram.py` & `sxmp_mule-1.1.1/mule/features/transform_features/mel_spectrogram.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/transform_features/timeline_average.py` & `sxmp_mule-1.1.1/mule/features/transform_features/timeline_average.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/features/transform_features/transform_feature.py` & `sxmp_mule-1.1.1/mule/features/transform_features/transform_feature.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/__init__.py` & `sxmp_mule-1.1.1/mule/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/layers/__init__.py` & `sxmp_mule-1.1.1/mule/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/layers/scalar_multiply.py` & `sxmp_mule-1.1.1/mule/models/layers/scalar_multiply.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/layers/stoch_depth.py` & `sxmp_mule-1.1.1/mule/models/layers/stoch_depth.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/layers/weight_standardization.py` & `sxmp_mule-1.1.1/mule/models/layers/weight_standardization.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/losses/__init__.py` & `sxmp_mule-1.1.1/mule/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/losses/loss.py` & `sxmp_mule-1.1.1/mule/models/losses/loss.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/losses/sim_clr_loss.py` & `sxmp_mule-1.1.1/mule/models/losses/sim_clr_loss.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/metrics/__init__.py` & `sxmp_mule-1.1.1/mule/models/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/metrics/train_metric.py` & `sxmp_mule-1.1.1/mule/models/metrics/train_metric.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/mlp.py` & `sxmp_mule-1.1.1/mule/models/mlp.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/model.py` & `sxmp_mule-1.1.1/mule/models/model.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/optimizers/__init__.py` & `sxmp_mule-1.1.1/mule/models/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/optimizers/optimizer.py` & `sxmp_mule-1.1.1/mule/models/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/optimizers/schedules/__init__.py` & `sxmp_mule-1.1.1/mule/models/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/optimizers/schedules/lr_schedule.py` & `sxmp_mule-1.1.1/mule/models/optimizers/schedules/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/optimizers/schedules/warmup_schedule.py` & `sxmp_mule-1.1.1/mule/models/optimizers/schedules/warmup_schedule.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/models/sfnfnetf0.py` & `sxmp_mule-1.1.1/mule/models/sfnfnetf0.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/source_files/__init__.py` & `sxmp_mule-1.1.1/mule/source_files/__init__.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/source_files/audio_file.py` & `sxmp_mule-1.1.1/mule/source_files/audio_file.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/mule/source_files/source_file.py` & `sxmp_mule-1.1.1/mule/source_files/source_file.py`

 * *Files identical despite different names*

### Comparing `sxmp-mule-1.1.0/setup.py` & `sxmp_mule-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2021 Pandora Media, LLC.
+# Copyright 2024 Pandora Media, LLC.
 #
 # Licensed under the GNU GPL License, Version 3.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.gnu.org/licenses/gpl-3.0.en.html
 #
@@ -18,14 +18,15 @@
 # None.
 
 # Third party imports
 # None.
 
 # Python standard library imports
 import setuptools
+import platform
 
 
 long_description = """
 # MULE
 
 The Musicset Unsupervised Large Embedding (MULE) module is your 
 music-audio workhorse!
@@ -55,26 +56,40 @@
 For more information on this module, please check out the publication:
 
 [*Supervised and Unsupervised Learning of Audio Representations for Music Understanding*](https://arxiv.org/abs/2210.03799), **M. C. McCallum**, F. Korzeniowski, S. Oramas, F. Gouyon, A. F. Ehmann.
 
 """
 
 
+# Tensorflow on ARM processors (i.e., macbooks with M1 or M2 or newer processors)
+# need a different compilation of tensorflow.
+# More details on the correct combinations of tensorflow packages below can be 
+# found here:
+#   https://developer.apple.com/metal/tensorflow-plugin/
+REQUIRED_TF = []
+if platform.processor()=='arm':
+    REQUIRED_TF += [
+        'tensorflow-macos==2.9.1',
+        'tensorflow-metal==0.5.0'
+    ]
+else:
+    REQUIRED_TF = ['tensorflow==2.9.1']
+
+
 REQUIRED_PACKAGES = [
     'numpy',
-    'librosa',
-    'click==8.0.0a1',
-    'scooch>=1.0.0',
-    'tensorflow==2.9.1'
-]
+    'librosa==0.9.2',
+    'click==8.1.7',
+    'scooch>=1.0.4'
+] + REQUIRED_TF
 
 
 setuptools.setup(
     name='sxmp-mule',
-    version='1.1.0',
+    version='1.1.1',
     description='',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PandoraMedia/music-audio-representations",
     author="Matt C. McCallum",
     author_email="mmccallum@pandora.com",
     classifiers=[
```

### Comparing `sxmp-mule-1.1.0/sxmp_mule.egg-info/PKG-INFO` & `sxmp_mule-1.1.1/sxmp_mule.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sxmp-mule
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/PandoraMedia/music-audio-representations
 Author: Matt C. McCallum
 Author-email: mmccallum@pandora.com
 License: GNU GPL 3.0
 Project-URL: Documentation, https://github.com/PandoraMedia/music-audio-representations
 Project-URL: Bug Reports, https://github.com/PandoraMedia/music-audio-representations/issues
 Project-URL: Source, https://github.com/PandoraMedia/music-audio-representations
@@ -19,14 +19,20 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: librosa==0.9.2
+Requires-Dist: click==8.1.7
+Requires-Dist: scooch>=1.0.4
+Requires-Dist: tensorflow-macos==2.9.1
+Requires-Dist: tensorflow-metal==0.5.0
 
 
 # MULE
 
 The Musicset Unsupervised Large Embedding (MULE) module is your 
 music-audio workhorse!
```

### Comparing `sxmp-mule-1.1.0/sxmp_mule.egg-info/SOURCES.txt` & `sxmp_mule-1.1.1/sxmp_mule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

