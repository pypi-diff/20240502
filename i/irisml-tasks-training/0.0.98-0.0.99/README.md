# Comparing `tmp/irisml-tasks-training-0.0.98.tar.gz` & `tmp/irisml-tasks-training-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-training-0.0.98.tar", last modified: Fri Nov 17 09:36:05 2023, max compression
+gzip compressed data, was "irisml-tasks-training-0.0.99.tar", last modified: Mon Nov 20 17:08:36 2023, max compression
```

## Comparing `irisml-tasks-training-0.0.98.tar` & `irisml-tasks-training-0.0.99.tar`

### file list

```diff
@@ -1,136 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:36:05.653807 irisml-tasks-training-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2023-11-17 09:36:05.653807 irisml-tasks-training-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:36:05.625807 irisml-tasks-training-0.0.98/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:36:05.637807 irisml-tasks-training-0.0.98/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/append_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/benchmark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/benchmark_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/benchmark_model_with_grad_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/build_classification_prompt_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/build_zero_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/concatenate_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/create_classification_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/create_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/evaluate_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/evaluate_detection_average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/evaluate_phrase_grounding_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/evaluate_string_matching_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/exclude_negative_samples_from_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/export_coco_from_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/extract_val_by_key_from_jsonl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/find_incorrect_classification_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/find_incorrect_classification_multilabel_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/get_questions_from_vqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/get_subclass_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/get_targets_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/load_jsonl_vqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/load_simple_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_classification_dataset_from_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_classification_dataset_from_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_detection_dataset_from_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_feature_extractor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_fixed_prompt_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_fixed_text_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_image_text_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_image_text_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_oversampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_prompt_list_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_vqa_collate_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/make_vqa_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/map_classification_predictions_to_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/num_iters_to_epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/remove_empty_images_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/sample_few_shot_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/save_jsonl_vqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/split_image_text_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:36:05.641807 irisml-tasks-training-0.0.98/irisml/tasks/train/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/build_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/build_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/build_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/ddp_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/ddp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugin_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugin_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:36:05.645807 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/clip_grad_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/detect_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/ema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/fp16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/freeze_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/freeze_modules_upto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/log_azureml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/log_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/log_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/mixup.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/nop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/scale_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/step_decay_ema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10111 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/irisml/tasks/train_with_gradient_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:36:05.645807 irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2023-11-17 09:36:05.000000 irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2023-11-17 09:36:05.000000 irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 09:36:05.000000 irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-17 09:36:05.000000 irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-17 09:36:05.000000 irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-11-17 09:36:05.653807 irisml-tasks-training-0.0.98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:36:05.653807 irisml-tasks-training-0.0.98/test/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_append_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_benchmark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_benchmark_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_build_classification_prompt_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_build_zero_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_concatenate_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_create_classification_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_create_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_evaluate_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_evaluate_detection_average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_evaluate_phrase_grounding_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_evaluate_string_matching_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_exclude_negative_samples_from_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_export_coco_from_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_extract_val_by_key_from_jsonl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_find_incorrect_classification_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_find_incorrect_classification_multilabel_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_get_questions_from_vqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_get_subclass_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_get_targets_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_irisml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_load_jsonl_vqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_load_simple_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_classification_dataset_from_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_classification_dataset_from_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_detection_dataset_from_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_feature_extractor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_fixed_prompt_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_fixed_text_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_image_text_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_image_text_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_oversampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_prompt_list_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_vqa_collate_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_make_vqa_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_map_classification_predictions_to_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_num_iters_to_epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_remove_empty_images_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_sample_few_shot_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_save_jsonl_vqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_split_image_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2023-11-17 09:32:31.000000 irisml-tasks-training-0.0.98/test/test_train_with_gradient_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:08:36.342892 irisml-tasks-training-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2023-11-20 17:08:36.342892 irisml-tasks-training-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:08:36.306889 irisml-tasks-training-0.0.99/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:08:36.330891 irisml-tasks-training-0.0.99/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/append_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/benchmark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/benchmark_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/benchmark_model_with_grad_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/build_classification_prompt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/build_zero_shot_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/concatenate_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/create_classification_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/create_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/evaluate_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/evaluate_detection_average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/evaluate_phrase_grounding_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/evaluate_string_matching_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/exclude_negative_samples_from_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/export_coco_from_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/extract_val_by_key_from_jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/find_incorrect_classification_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/find_incorrect_classification_multilabel_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/get_questions_from_vqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/get_subclass_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/get_targets_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/load_jsonl_vqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/load_simple_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_classification_dataset_from_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_classification_dataset_from_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_detection_dataset_from_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_feature_extractor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_fixed_prompt_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_fixed_text_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_image_text_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_image_text_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_oversampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_phrase_grounding_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_prompt_list_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_vqa_collate_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/make_vqa_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/map_classification_predictions_to_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/num_iters_to_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/remove_empty_images_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/sample_few_shot_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/save_jsonl_vqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/split_image_text_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:08:36.334891 irisml-tasks-training-0.0.99/irisml/tasks/train/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/build_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/build_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/build_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/ddp_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/ddp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugin_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugin_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:08:36.334891 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/clip_grad_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/detect_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/fp16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/freeze_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/freeze_modules_upto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/log_azureml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/log_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/log_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/nop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/scale_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/step_decay_ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/irisml/tasks/train_with_gradient_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:08:36.338891 irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2023-11-20 17:08:36.000000 irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2023-11-20 17:08:36.000000 irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 17:08:36.000000 irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-20 17:08:36.000000 irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-20 17:08:36.000000 irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-11-20 17:08:36.346892 irisml-tasks-training-0.0.99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 17:08:36.342892 irisml-tasks-training-0.0.99/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_append_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_benchmark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_benchmark_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_build_classification_prompt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_build_zero_shot_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_concatenate_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_create_classification_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_create_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_evaluate_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_evaluate_detection_average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_evaluate_phrase_grounding_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_evaluate_string_matching_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_exclude_negative_samples_from_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_export_coco_from_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_extract_val_by_key_from_jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_find_incorrect_classification_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_find_incorrect_classification_multilabel_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_get_questions_from_vqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_get_subclass_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_get_targets_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_irisml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_load_jsonl_vqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_load_simple_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_classification_dataset_from_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_classification_dataset_from_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_detection_dataset_from_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_feature_extractor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_fixed_prompt_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_fixed_text_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_image_text_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_image_text_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_oversampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_phrase_grounding_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_prompt_list_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_vqa_collate_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_make_vqa_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_map_classification_predictions_to_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_num_iters_to_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_remove_empty_images_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_sample_few_shot_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_save_jsonl_vqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_split_image_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2023-11-20 17:04:33.000000 irisml-tasks-training-0.0.99/test/test_train_with_gradient_cache.py
```

### Comparing `irisml-tasks-training-0.0.98/LICENSE` & `irisml-tasks-training-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/PKG-INFO` & `irisml-tasks-training-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-training
-Version: 0.0.98
+Version: 0.0.99
 Summary: IrisML tasks for pytorch training
 Home-page: https://github.com/microsoft/irisml-tasks-training
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-training-0.0.98/README.md` & `irisml-tasks-training-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/append_classifier.py` & `irisml-tasks-training-0.0.99/irisml/tasks/append_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/benchmark_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/benchmark_model.py` & `irisml-tasks-training-0.0.99/irisml/tasks/benchmark_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/benchmark_model_with_grad_cache.py` & `irisml-tasks-training-0.0.99/irisml/tasks/benchmark_model_with_grad_cache.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/build_classification_prompt_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/build_classification_prompt_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/build_zero_shot_classifier.py` & `irisml-tasks-training-0.0.99/irisml/tasks/build_zero_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/concatenate_datasets.py` & `irisml-tasks-training-0.0.99/irisml/tasks/concatenate_datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,43 +10,48 @@
 
 class Task(irisml.core.TaskBase):
     """Concatenate the given two datasets together.
 
     If Config.use_same_classspace is False, class_names0 and class_names1 must be provided. The class ids will be mapped so that the new class_names will not have duplicated names.
 
     Config:
-        task_type ('classifictaion_multiclass' or 'object_detection'): The dataset type.
+        task_type ('classifictaion_multiclass', 'object_detection', or 'phrase_grounding'): The dataset type.
         use_same_classspace (bool): If False, the class ids of the dataset1 will be mapped to new class ids.
     """
-    VERSION = '0.1.2'
+    VERSION = '0.2.0'
 
     @dataclasses.dataclass
     class Inputs:
         dataset0: torch.utils.data.Dataset
         dataset1: typing.Optional[torch.utils.data.Dataset] = None
         class_names0: typing.Optional[typing.List[str]] = None
         class_names1: typing.Optional[typing.List[str]] = None
 
     @dataclasses.dataclass
     class Config:
-        task_type: typing.Literal['classification_multiclass', 'object_detection'] = 'classification_multiclass'
+        task_type: typing.Literal['classification_multiclass', 'object_detection', 'phrase_grounding'] = 'classification_multiclass'
         use_same_classspace: bool = True
 
     @dataclasses.dataclass
     class Outputs:
         dataset: torch.utils.data.Dataset
         class_names: typing.Optional[typing.List[str]] = None
         num_classes: typing.Optional[int] = None
 
     def execute(self, inputs):
         if not inputs.dataset1:
             logger.info("dataset1 is None. Returning dataset0 without concatenation.")
             return self.Outputs(inputs.dataset0, inputs.class_names0)
 
-        if not self.config.use_same_classspace:
+        use_same_classspace = self.config.use_same_classspace
+        if self.config.task_type == 'phrase_grounding' and not use_same_classspace:
+            use_same_classspace = True
+            logger.warning("use_same_classspace is ignored for phrase_grounding task.")
+
+        if not use_same_classspace:
             if inputs.class_names0 and inputs.class_names1:
                 class_mappings = [list(range(len(inputs.class_names0))), []]
                 new_class_names = copy.deepcopy(inputs.class_names0)
                 for c in inputs.class_names1:
                     try:
                         existing_class_id = new_class_names.index(c)
                         class_mappings[1].append(existing_class_id)
@@ -59,24 +64,25 @@
             logger.info(f"The number of new classes is {num_classes}")
         else:
             class_mappings = None
             new_class_names = None
             num_classes = None
 
         dataset = ConcatDataset(inputs.dataset0, inputs.dataset1, class_mappings, self.config.task_type)
+        logger.info(f"Concatenated dataset0 ({len(inputs.dataset0)}) and dataset1 ({len(inputs.dataset1)}) into a new dataset ({len(dataset)})")
         return self.Outputs(dataset, new_class_names, num_classes)
 
     def dry_run(self, inputs):
         return self.execute(inputs)
 
 
 class ConcatDataset(torch.utils.data.Dataset):
-    def __init__(self, dataset0, dataset1, class_mappings: typing.List[typing.List[int]], task_type):
+    def __init__(self, dataset0, dataset1, class_mappings: typing.Optional[typing.List[typing.List[int]]], task_type):
         assert class_mappings is None or len(class_mappings) == 2
-        assert task_type in ['classification_multiclass', 'object_detection']
+        assert task_type in ['classification_multiclass', 'object_detection', 'phrase_grounding']
         self._datasets = [dataset0, dataset1]
         self._first_dataset_size = len(dataset0)
         self._class_mappings = class_mappings
         self._task_type = task_type
 
     def __len__(self):
         return len(self._datasets[0]) + len(self._datasets[1])
```

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/create_classification_prompt_generator.py` & `irisml-tasks-training-0.0.99/irisml/tasks/create_classification_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/create_prompt_generator.py` & `irisml-tasks-training-0.0.99/irisml/tasks/create_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/evaluate_accuracy.py` & `irisml-tasks-training-0.0.99/irisml/tasks/evaluate_accuracy.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/evaluate_detection_average_precision.py` & `irisml-tasks-training-0.0.99/irisml/tasks/evaluate_detection_average_precision.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/evaluate_phrase_grounding_recall.py` & `irisml-tasks-training-0.0.99/irisml/tasks/evaluate_phrase_grounding_recall.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/evaluate_string_matching_accuracy.py` & `irisml-tasks-training-0.0.99/irisml/tasks/evaluate_string_matching_accuracy.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/exclude_negative_samples_from_classification_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/exclude_negative_samples_from_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/export_coco_from_torch_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/export_coco_from_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/export_onnx.py` & `irisml-tasks-training-0.0.99/irisml/tasks/export_onnx.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/extract_val_by_key_from_jsonl.py` & `irisml-tasks-training-0.0.99/irisml/tasks/extract_val_by_key_from_jsonl.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/find_incorrect_classification_indices.py` & `irisml-tasks-training-0.0.99/irisml/tasks/find_incorrect_classification_indices.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/find_incorrect_classification_multilabel_indices.py` & `irisml-tasks-training-0.0.99/irisml/tasks/find_incorrect_classification_multilabel_indices.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/get_questions_from_vqa_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/get_questions_from_vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/get_subclass_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/get_subclass_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/get_targets_from_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/get_targets_from_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/load_jsonl_vqa_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/load_jsonl_vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/load_simple_classification_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/load_simple_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_classification_dataset_from_object_detection.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_classification_dataset_from_object_detection.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_classification_dataset_from_predictions.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_classification_dataset_from_predictions.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_detection_dataset_from_predictions.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_detection_dataset_from_predictions.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_feature_extractor_model.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_feature_extractor_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_fixed_prompt_image_transform.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_fixed_prompt_image_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_fixed_text_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_fixed_text_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_image_text_contrastive_model.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_image_text_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_image_text_transform.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_image_text_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_oversampled_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_oversampled_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_prompt_list_image_transform.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_prompt_list_image_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_vqa_collate_function.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_vqa_collate_function.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import dataclasses
 import typing
 import torch
 import irisml.core
 
 
 class Task(irisml.core.TaskBase):
-    """Creates a collate_function for Visual Question Answering (VQA) tasks.
+    """Creates a collate_function for Visual Question Answering (VQA) and Phrase Grounding task.
 
     Config:
         pad_token_id (int): The id of the padding token. Default: 1.
     """
-    VERSION = '0.1.0'
+    VERSION = '0.2.0'
 
     @dataclasses.dataclass
     class Config:
         pad_token_id: int = 1
 
     @dataclasses.dataclass
     class Outputs:
@@ -34,17 +34,19 @@
 
     def __call__(self, batch):
         questions = [b[0][0] for b in batch]
         images = [b[0][1] for b in batch]
         targets = [b[1] for b in batch]
 
         # input_ids, attention_mask. Use 0 for attention_mask padding.
-        questions = (self._padded_stack([q[0] for q in questions], self._pad_token_id), self._padded_stack([q[1] for q in questions]))
-        images = torch.stack(images, 0)
-        if not isinstance(targets[0], str):
+        if isinstance(questions[0][0], torch.Tensor):
+            questions = (self._padded_stack([q[0] for q in questions], self._pad_token_id), self._padded_stack([q[1] for q in questions]))
+        if isinstance(images[0], torch.Tensor):
+            images = torch.stack(images, 0)
+        if isinstance(targets[0][0], torch.Tensor):
             targets = (self._padded_stack([t[0] for t in targets], self._pad_token_id), self._padded_stack([t[1] for t in targets]))
 
         return (questions, images), targets
 
     def _padded_stack(self, tensors, pad_token_id=0):
         """Stacks tensors along the first dimension and pads them to the same length."""
         max_length = max([t.shape[0] for t in tensors])
```

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/make_vqa_image_transform.py` & `irisml-tasks-training-0.0.99/irisml/tasks/make_vqa_image_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/map_classification_predictions_to_detection.py` & `irisml-tasks-training-0.0.99/irisml/tasks/map_classification_predictions_to_detection.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/num_iters_to_epochs.py` & `irisml-tasks-training-0.0.99/irisml/tasks/num_iters_to_epochs.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/predict.py` & `irisml-tasks-training-0.0.99/irisml/tasks/predict.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/remove_empty_images_from_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/remove_empty_images_from_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/sample_few_shot_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/sample_few_shot_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/save_jsonl_vqa_dataset.py` & `irisml-tasks-training-0.0.99/irisml/tasks/save_jsonl_vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/split_image_text_model.py` & `irisml-tasks-training-0.0.99/irisml/tasks/split_image_text_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/build_dataloader.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/build_lr_scheduler.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/build_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/build_optimizer.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/ddp_trainer.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/ddp_trainer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/ddp_utils.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/ddp_utils.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugin_list.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugin_list.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugin_loader.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/amp.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/amp.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/clip_grad_norm.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/clip_grad_norm.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/compile.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/compile.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/debug.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/detect_anomaly.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/detect_anomaly.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/early_stopping.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/early_stopping.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/ema.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/ema.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/fp16.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/fp16.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/freeze_modules.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/freeze_modules.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/freeze_modules_upto.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/freeze_modules_upto.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/heartbeat.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/log_azureml.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/log_azureml.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/log_summary.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/log_summary.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/log_tensorboard.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/log_tensorboard.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/mixup.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/mixup.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/plugin_base.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/progressbar.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/progressbar.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/plugins/step_decay_ema.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/plugins/step_decay_ema.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/task.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/task.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train/trainer.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train/trainer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml/tasks/train_with_gradient_cache.py` & `irisml-tasks-training-0.0.99/irisml/tasks/train_with_gradient_cache.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/PKG-INFO` & `irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-training
-Version: 0.0.98
+Version: 0.0.99
 Summary: IrisML tasks for pytorch training
 Home-page: https://github.com/microsoft/irisml-tasks-training
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-training-0.0.98/irisml_tasks_training.egg-info/SOURCES.txt` & `irisml-tasks-training-0.0.99/irisml_tasks_training.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 irisml/tasks/make_detection_dataset_from_predictions.py
 irisml/tasks/make_feature_extractor_model.py
 irisml/tasks/make_fixed_prompt_image_transform.py
 irisml/tasks/make_fixed_text_dataset.py
 irisml/tasks/make_image_text_contrastive_model.py
 irisml/tasks/make_image_text_transform.py
 irisml/tasks/make_oversampled_dataset.py
+irisml/tasks/make_phrase_grounding_image_transform.py
 irisml/tasks/make_prompt_list_image_transform.py
 irisml/tasks/make_vqa_collate_function.py
 irisml/tasks/make_vqa_image_transform.py
 irisml/tasks/map_classification_predictions_to_detection.py
 irisml/tasks/num_iters_to_epochs.py
 irisml/tasks/predict.py
 irisml/tasks/remove_empty_images_from_dataset.py
@@ -111,14 +112,15 @@
 test/test_make_detection_dataset_from_predictions.py
 test/test_make_feature_extractor_model.py
 test/test_make_fixed_prompt_image_transform.py
 test/test_make_fixed_text_dataset.py
 test/test_make_image_text_contrastive_model.py
 test/test_make_image_text_transform.py
 test/test_make_oversampled_dataset.py
+test/test_make_phrase_grounding_image_transform.py
 test/test_make_prompt_list_image_transform.py
 test/test_make_vqa_collate_function.py
 test/test_make_vqa_image_transform.py
 test/test_map_classification_predictions_to_detection.py
 test/test_num_iters_to_epochs.py
 test/test_predict.py
 test/test_remove_empty_images_from_dataset.py
```

### Comparing `irisml-tasks-training-0.0.98/setup.cfg` & `irisml-tasks-training-0.0.99/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-training
-version = 0.0.98
+version = 0.0.99
 url = https://github.com/microsoft/irisml-tasks-training
 description = IrisML tasks for pytorch training
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-training-0.0.98/test/test_append_classifier.py` & `irisml-tasks-training-0.0.99/test/test_append_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_benchmark_model.py` & `irisml-tasks-training-0.0.99/test/test_benchmark_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_build_classification_prompt_dataset.py` & `irisml-tasks-training-0.0.99/test/test_build_classification_prompt_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_build_zero_shot_classifier.py` & `irisml-tasks-training-0.0.99/test/test_build_zero_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_concatenate_datasets.py` & `irisml-tasks-training-0.0.99/test/test_concatenate_datasets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+import PIL.Image
 import torch
 from irisml.tasks.concatenate_datasets import Task
 
 
 from utils import FakeDataset, FakeDatasetWithGetTargets
 
 
@@ -74,7 +75,23 @@
         self.assertEqual(outputs.dataset.get_targets(1), torch.tensor(2))
         self.assertEqual(outputs.dataset.get_targets(2), torch.tensor(3))
         self.assertEqual(dataset0._counter, 3)
         self.assertEqual(outputs.dataset.get_targets(3), torch.tensor(1))
         self.assertEqual(outputs.dataset.get_targets(4), torch.tensor(2))
         self.assertEqual(outputs.dataset.get_targets(5), torch.tensor(3))
         self.assertEqual(dataset0._counter, 3)
+
+    def test_phrase_grounding_dataset(self):
+        dataset0 = FakeDataset([(('abc', PIL.Image.new('RGB', (10, 10))), [(0, 2), torch.tensor([[0.1, 0.1, 0.2, 0.2]])]),
+                                (('def', PIL.Image.new('RGB', (10, 10))), [(0, 3), torch.tensor([[0.2, 0.2, 0.3, 0.3]])])])
+        dataset1 = FakeDataset([(('abc2', PIL.Image.new('RGB', (10, 10))), [(0, 2), torch.tensor([[0.1, 0.1, 0.2, 0.2]])]),
+                                (('def2', PIL.Image.new('RGB', (10, 10))), [(0, 3), torch.tensor([[0.2, 0.2, 0.3, 0.3]])])])
+        outputs = Task(Task.Config(task_type='phrase_grounding')).execute(Task.Inputs(dataset0, dataset1))
+        self.assertEqual(len(outputs.dataset), 4)
+        self.assertEqual(outputs.dataset[0][0], ('abc', PIL.Image.new('RGB', (10, 10))))
+        self.assertEqual(outputs.dataset[1][0], ('def', PIL.Image.new('RGB', (10, 10))))
+        self.assertEqual(outputs.dataset[2][0], ('abc2', PIL.Image.new('RGB', (10, 10))))
+        self.assertEqual(outputs.dataset[3][0], ('def2', PIL.Image.new('RGB', (10, 10))))
+        self.assertTrue(torch.equal(outputs.dataset[0][1][1], torch.tensor([[0.1, 0.1, 0.2, 0.2]])))
+        self.assertTrue(torch.equal(outputs.dataset[1][1][1], torch.tensor([[0.2, 0.2, 0.3, 0.3]])))
+        self.assertTrue(torch.equal(outputs.dataset[2][1][1], torch.tensor([[0.1, 0.1, 0.2, 0.2]])))
+        self.assertTrue(torch.equal(outputs.dataset[3][1][1], torch.tensor([[0.2, 0.2, 0.3, 0.3]])))
```

### Comparing `irisml-tasks-training-0.0.98/test/test_create_classification_prompt_generator.py` & `irisml-tasks-training-0.0.99/test/test_create_classification_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_evaluate_accuracy.py` & `irisml-tasks-training-0.0.99/test/test_evaluate_accuracy.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_evaluate_detection_average_precision.py` & `irisml-tasks-training-0.0.99/test/test_evaluate_detection_average_precision.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_evaluate_phrase_grounding_recall.py` & `irisml-tasks-training-0.0.99/test/test_evaluate_phrase_grounding_recall.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_evaluate_string_matching_accuracy.py` & `irisml-tasks-training-0.0.99/test/test_evaluate_string_matching_accuracy.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_exclude_negative_samples_from_classification_dataset.py` & `irisml-tasks-training-0.0.99/test/test_exclude_negative_samples_from_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_export_coco_from_torch_dataset.py` & `irisml-tasks-training-0.0.99/test/test_export_coco_from_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_export_onnx.py` & `irisml-tasks-training-0.0.99/test/test_export_onnx.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_extract_val_by_key_from_jsonl.py` & `irisml-tasks-training-0.0.99/test/test_extract_val_by_key_from_jsonl.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_find_incorrect_classification_indices.py` & `irisml-tasks-training-0.0.99/test/test_find_incorrect_classification_indices.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_find_incorrect_classification_multilabel_indices.py` & `irisml-tasks-training-0.0.99/test/test_find_incorrect_classification_multilabel_indices.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_get_questions_from_vqa_dataset.py` & `irisml-tasks-training-0.0.99/test/test_get_questions_from_vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_get_subclass_dataset.py` & `irisml-tasks-training-0.0.99/test/test_get_subclass_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_get_targets_from_dataset.py` & `irisml-tasks-training-0.0.99/test/test_get_targets_from_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_load_jsonl_vqa_dataset.py` & `irisml-tasks-training-0.0.99/test/test_load_jsonl_vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_load_simple_classification_dataset.py` & `irisml-tasks-training-0.0.99/test/test_load_simple_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_classification_dataset_from_object_detection.py` & `irisml-tasks-training-0.0.99/test/test_make_classification_dataset_from_object_detection.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_classification_dataset_from_predictions.py` & `irisml-tasks-training-0.0.99/test/test_make_classification_dataset_from_predictions.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_detection_dataset_from_predictions.py` & `irisml-tasks-training-0.0.99/test/test_make_detection_dataset_from_predictions.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_feature_extractor_model.py` & `irisml-tasks-training-0.0.99/test/test_make_feature_extractor_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_fixed_prompt_image_transform.py` & `irisml-tasks-training-0.0.99/test/test_make_fixed_prompt_image_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_image_text_contrastive_model.py` & `irisml-tasks-training-0.0.99/test/test_make_image_text_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_image_text_transform.py` & `irisml-tasks-training-0.0.99/test/test_make_image_text_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_oversampled_dataset.py` & `irisml-tasks-training-0.0.99/test/test_make_oversampled_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_prompt_list_image_transform.py` & `irisml-tasks-training-0.0.99/test/test_make_prompt_list_image_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_make_vqa_collate_function.py` & `irisml-tasks-training-0.0.99/test/test_make_vqa_collate_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pickle
 import unittest
+import PIL.Image
 import torch
 from irisml.tasks.make_vqa_collate_function import Task
 
 
 class TestMakeVqaCollateFunction(unittest.TestCase):
     def test_collate_function(self):
         outputs = Task(Task.Config()).execute(Task.Inputs())
@@ -42,14 +43,23 @@
         # When targets are strings
         collate_outputs = collate_function([((question, image), 'answer') for _ in range(4)])
         self.assertIsInstance(collate_outputs[1], list)
         self.assertEqual(len(collate_outputs[1]), 4)
         self.assertIsInstance(collate_outputs[1][0], str)
         self.assertEqual(collate_outputs[1], ['answer' for _ in range(4)])
 
+        # Phrase grounding with GPT-V
+        collate_outputs = collate_function([(('caption', PIL.Image.new('RGB', (32, 32))), [((0, 2), torch.tensor([[0.1, 0.1, 0.2, 0.2]]))]) for _ in range(4)])
+        self.assertEqual(collate_outputs[0][0], ['caption'] * 4)
+        self.assertEqual(collate_outputs[0][1], [PIL.Image.new('RGB', (32, 32))] * 4)
+        self.assertIsInstance(collate_outputs[1], list)
+        self.assertEqual(len(collate_outputs[1]), 4)
+
+        self.assertEqual(collate_outputs[1][0][0][0], (0, 2))
+
     def test_collate_function_padding(self):
         outputs = Task(Task.Config(pad_token_id=100)).execute(Task.Inputs())
         collate_function = outputs.collate_function
 
         collate_outputs = collate_function([(((torch.Tensor([i] * i), torch.Tensor([1] * i)), torch.rand(3, 32, 32)), 'answer') for i in range(1, 5)])
 
         self.assertEqual(collate_outputs[0][0][0].tolist(), [[1, 100, 100, 100], [2, 2, 100, 100], [3, 3, 3, 100], [4, 4, 4, 4]])
```

### Comparing `irisml-tasks-training-0.0.98/test/test_make_vqa_image_transform.py` & `irisml-tasks-training-0.0.99/test/test_make_vqa_image_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_map_classification_predictions_to_detection.py` & `irisml-tasks-training-0.0.99/test/test_map_classification_predictions_to_detection.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_num_iters_to_epochs.py` & `irisml-tasks-training-0.0.99/test/test_num_iters_to_epochs.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_predict.py` & `irisml-tasks-training-0.0.99/test/test_predict.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_remove_empty_images_from_dataset.py` & `irisml-tasks-training-0.0.99/test/test_remove_empty_images_from_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_sample_few_shot_dataset.py` & `irisml-tasks-training-0.0.99/test/test_sample_few_shot_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_save_jsonl_vqa_dataset.py` & `irisml-tasks-training-0.0.99/test/test_save_jsonl_vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_split_image_text_model.py` & `irisml-tasks-training-0.0.99/test/test_split_image_text_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.98/test/test_train_with_gradient_cache.py` & `irisml-tasks-training-0.0.99/test/test_train_with_gradient_cache.py`

 * *Files identical despite different names*

