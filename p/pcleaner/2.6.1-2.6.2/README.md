# Comparing `tmp/pcleaner-2.6.1.tar.gz` & `tmp/pcleaner-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-2.6.1.tar", last modified: Fri Mar 15 19:31:17 2024, max compression
+gzip compressed data, was "pcleaner-2.6.2.tar", last modified: Wed May  1 23:59:31 2024, max compression
```

## Comparing `pcleaner-2.6.1.tar` & `pcleaner-2.6.2.tar`

### file list

```diff
@@ -1,113 +1,117 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.892426 pcleaner-2.6.1/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-03-13 00:41:01.000000 pcleaner-2.6.1/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16232 2024-03-15 19:31:17.892426 pcleaner-2.6.1/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14585 2024-03-10 23:31:03.000000 pcleaner-2.6.1/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.862425 pcleaner-2.6.1/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-03-15 19:28:54.000000 pcleaner-2.6.1/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6986 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.865759 pcleaner-2.6.1/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-10-05 16:27:27.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.865759 pcleaner-2.6.1/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.865759 pcleaner-2.6.1/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.869092 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-03-13 00:41:01.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-10-05 16:27:31.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-10-05 16:27:37.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-09-27 00:34:46.000000 pcleaner-2.6.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    59689 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10442 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.872426 pcleaner-2.6.1/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2023-04-30 23:44:23.000000 pcleaner-2.6.1/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2023-04-30 23:44:23.000000 pcleaner-2.6.1/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-30 23:44:23.000000 pcleaner-2.6.1/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/data/windows_explorer_integration_regedit.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-03-13 01:38:01.000000 pcleaner-2.6.1/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.882426 pcleaner-2.6.1/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.885759 pcleaner-2.6.1/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5671 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CBadgeButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2642 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CColorButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4791 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      682 2023-09-27 00:28:04.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CDropFrame.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2092 2023-09-27 00:33:46.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CElidedLabel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3346 2023-09-27 00:33:46.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1150 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CTextEdit.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1628 2023-09-27 00:28:04.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/CTooltipLabel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-30 23:44:23.000000 pcleaner-2.6.1/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-30 23:44:23.000000 pcleaner-2.6.1/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1381 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/about_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5547 2023-10-05 23:04:30.000000 pcleaner-2.6.1/pcleaner/gui/ctd_interface_gui.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2293 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/error_dialog_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10963 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/gui/file_manager_extension_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27356 2024-03-15 19:28:54.000000 pcleaner-2.6.1/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14388 2024-03-15 19:28:54.000000 pcleaner-2.6.1/pcleaner/gui/gui_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    33067 2024-03-15 19:28:54.000000 pcleaner-2.6.1/pcleaner/gui/image_details_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21465 2024-03-14 00:05:11.000000 pcleaner-2.6.1/pcleaner/gui/image_file.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4374 2024-03-13 23:59:07.000000 pcleaner-2.6.1/pcleaner/gui/image_tab.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7561 2024-03-12 22:16:17.000000 pcleaner-2.6.1/pcleaner/gui/image_viewer.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3591 2024-03-14 01:24:13.000000 pcleaner-2.6.1/pcleaner/gui/issue_reporter_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4989 2024-03-14 02:28:37.000000 pcleaner-2.6.1/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      519 2023-10-05 23:05:26.000000 pcleaner-2.6.1/pcleaner/gui/license_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3563 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/log_parser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4873 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/log_viewer.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    64161 2024-03-14 00:07:45.000000 pcleaner-2.6.1/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19431 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/gui/model_downloader_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4648 2023-10-05 23:05:26.000000 pcleaner-2.6.1/pcleaner/gui/new_profile_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    41984 2024-03-14 00:05:28.000000 pcleaner-2.6.1/pcleaner/gui/processing.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21373 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.885759 pcleaner-2.6.1/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-30 23:44:23.000000 pcleaner-2.6.1/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   105179 2024-03-15 19:31:12.000000 pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   169588 2024-03-15 19:31:12.000000 pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_theme_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4458 2024-03-15 19:31:12.000000 pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_themes.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   348284 2024-03-14 00:29:21.000000 pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_translations.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      956 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/gui/setup_greeter_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      559 2023-10-05 23:05:26.000000 pcleaner-2.6.1/pcleaner/gui/structures.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      701 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/supported_languages.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.889093 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-30 23:44:23.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6619 2024-03-15 19:31:13.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_About.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5576 2024-03-15 19:31:13.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4481 2024-03-15 19:31:13.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13725 2024-03-15 19:31:13.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6367 2024-03-15 19:31:14.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_IssueReporter.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    41024 2024-03-15 19:31:14.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_License.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    49222 2024-03-15 19:31:14.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6958 2024-03-15 19:31:14.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7411 2024-03-15 19:31:14.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12580 2024-03-15 19:31:15.000000 pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5535 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8826 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    32498 2024-03-13 01:39:04.000000 pcleaner-2.6.1/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-03-14 00:29:39.000000 pcleaner-2.6.1/pcleaner/inpainting.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    30621 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     9207 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/preprocessor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-02-22 11:30:27.000000 pcleaner-2.6.1/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22016 2024-03-10 23:31:04.000000 pcleaner-2.6.1/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.892426 pcleaner-2.6.1/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16232 2024-03-15 19:31:17.000000 pcleaner-2.6.1/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3508 2024-03-15 19:31:17.000000 pcleaner-2.6.1/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-03-15 19:31:17.000000 pcleaner-2.6.1/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       90 2024-03-15 19:31:17.000000 pcleaner-2.6.1/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      412 2024-03-15 19:31:17.000000 pcleaner-2.6.1/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-03-15 19:31:17.000000 pcleaner-2.6.1/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-03-13 00:41:01.000000 pcleaner-2.6.1/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1497 2024-03-15 19:31:17.892426 pcleaner-2.6.1/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-03-13 00:41:01.000000 pcleaner-2.6.1/setup.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-03-15 19:31:17.889093 pcleaner-2.6.1/tests/
--rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-22 11:30:27.000000 pcleaner-2.6.1/tests/test_log_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.517274 pcleaner-2.6.2/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-2.6.2/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16416 2024-05-01 23:59:31.517274 pcleaner-2.6.2/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14769 2024-05-01 21:30:08.000000 pcleaner-2.6.2/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.407273 pcleaner-2.6.2/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-05-01 23:58:10.000000 pcleaner-2.6.2/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6986 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.410607 pcleaner-2.6.2/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.410607 pcleaner-2.6.2/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.417273 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.440607 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-2.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    59689 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10442 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.447273 pcleaner-2.6.2/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-2.6.2/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-2.6.2/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-2.6.2/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-04-17 23:18:42.000000 pcleaner-2.6.2/pcleaner/data/windows_explorer_integration_regedit.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.463940 pcleaner-2.6.2/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.483940 pcleaner-2.6.2/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5671 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CBadgeButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2642 2024-01-25 04:44:05.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4791 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      682 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CDropFrame.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2092 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CElidedLabel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3346 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1150 2024-02-15 00:39:49.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CTextEdit.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1628 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/CTooltipLabel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-2.6.2/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-2.6.2/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1381 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/about_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5547 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/ctd_interface_gui.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2293 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/error_dialog_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10963 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/file_manager_extension_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27366 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14479 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/gui_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    33067 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/image_details_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21465 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/image_file.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4315 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/image_tab.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7561 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/image_viewer.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3591 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/issue_reporter_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6685 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      519 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/license_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3563 2024-02-12 16:50:11.000000 pcleaner-2.6.2/pcleaner/gui/log_parser.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4873 2024-02-12 23:21:16.000000 pcleaner-2.6.2/pcleaner/gui/log_viewer.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    64509 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19431 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/model_downloader_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4648 2023-10-07 13:58:30.000000 pcleaner-2.6.2/pcleaner/gui/new_profile_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    41984 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/processing.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21373 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.493940 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   105176 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   169588 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_theme_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4452 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_themes.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   348275 2024-05-01 22:25:41.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_translations.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107395 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   175979 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4675 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_themes.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   843082 2024-05-01 23:54:46.000000 pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_windows_translations.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      956 2024-03-02 00:01:57.000000 pcleaner-2.6.2/pcleaner/gui/setup_greeter_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      559 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/gui/structures.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      701 2024-01-30 21:06:51.000000 pcleaner-2.6.2/pcleaner/gui/supported_languages.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.513940 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-02-12 21:19:18.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6619 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_About.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5576 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4481 2024-05-01 23:59:24.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13725 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6367 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_IssueReporter.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    41024 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_License.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    49222 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6958 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7411 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_NewProfile.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12580 2024-05-01 23:59:25.000000 pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5545 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8826 2024-05-01 21:35:49.000000 pcleaner-2.6.2/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    32498 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/inpainting.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    30621 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     9207 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/preprocessor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-04-14 22:05:44.000000 pcleaner-2.6.2/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    22016 2024-05-01 21:30:08.000000 pcleaner-2.6.2/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.517274 pcleaner-2.6.2/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16416 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3730 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       90 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      412 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-05-01 23:59:31.000000 pcleaner-2.6.2/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2024-01-09 17:47:58.000000 pcleaner-2.6.2/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1497 2024-05-01 23:59:31.517274 pcleaner-2.6.2/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-2.6.2/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-01 23:59:31.513940 pcleaner-2.6.2/tests/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-11 23:18:20.000000 pcleaner-2.6.2/tests/test_log_parser.py
```

### Comparing `pcleaner-2.6.1/LICENSE` & `pcleaner-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/PKG-INFO` & `pcleaner-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 2.6.1
+Version: 2.6.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -93,14 +93,16 @@
 
 ## Features
 
 - Cleans text bubbles without leaving artifacts.
 
 - Avoids painting over parts of the image that aren't text.
 
+- Inpaints bubbles that can't simply be masked out.
+
 - Ignores bubbles containing only symbols or numbers, as those don't need translation.
 
 - Offers a GUI for easy use, dark, light, and system themes are supported.
 
 - No internet connection required after installing the model data.
 
 - Offers a plethora of options to customize the cleaning process and the ability to save multiple presets as profiles.
@@ -318,14 +320,16 @@
 ## Acknowledgements
 
 - [Comic Text Detector](https://github.com/dmMaze/comic-text-detector) for finding text bubbles and generating the initial mask.
 
 - [Manga OCR](https://github.com/kha-white/manga-ocr) for detecting which bubbles only contain symbols or numbers,
   and performing the dedicated OCR command.
 
+- [Simple Lama Inpainting](https://github.com/enesmsahin/simple-lama-inpainting) for inpainting bubbles that can't be masked out.
+
 
 ## License
 
 This project is licensed under the GNU General Public License v3.0 – see
 the [LICENSE](https://raw.githubusercontent.com/VoxelCubes/PanelCleaner/master/LICENSE) file for details.
```

### Comparing `pcleaner-2.6.1/README.md` & `pcleaner-2.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
 ## Features
 
 - Cleans text bubbles without leaving artifacts.
 
 - Avoids painting over parts of the image that aren't text.
 
+- Inpaints bubbles that can't simply be masked out.
+
 - Ignores bubbles containing only symbols or numbers, as those don't need translation.
 
 - Offers a GUI for easy use, dark, light, and system themes are supported.
 
 - No internet connection required after installing the model data.
 
 - Offers a plethora of options to customize the cleaning process and the ability to save multiple presets as profiles.
@@ -270,14 +272,16 @@
 ## Acknowledgements
 
 - [Comic Text Detector](https://github.com/dmMaze/comic-text-detector) for finding text bubbles and generating the initial mask.
 
 - [Manga OCR](https://github.com/kha-white/manga-ocr) for detecting which bubbles only contain symbols or numbers,
   and performing the dedicated OCR command.
 
+- [Simple Lama Inpainting](https://github.com/enesmsahin/simple-lama-inpainting) for inpainting bubbles that can't be masked out.
+
 
 ## License
 
 This project is licensed under the GNU General Public License v3.0 – see
 the [LICENSE](https://raw.githubusercontent.com/VoxelCubes/PanelCleaner/master/LICENSE) file for details.
```

### Comparing `pcleaner-2.6.1/pcleaner/analytics.py` & `pcleaner-2.6.2/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/cli_utils.py` & `pcleaner-2.6.2/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/inference.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-2.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/config.py` & `pcleaner-2.6.2/pcleaner/config.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/ctd_interface.py` & `pcleaner-2.6.2/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner-2.6.2/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner-2.6.2/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/data/windows_explorer_integration_regedit.py` & `pcleaner-2.6.2/pcleaner/data/windows_explorer_integration_regedit.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/denoiser.py` & `pcleaner-2.6.2/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CBadgeButton.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CBadgeButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CColorButton.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CColorButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CDropFrame.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CDropFrame.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CElidedLabel.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CElidedLabel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CTextEdit.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CTextEdit.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/CustomQ/CTooltipLabel.py` & `pcleaner-2.6.2/pcleaner/gui/CustomQ/CTooltipLabel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/about_driver.py` & `pcleaner-2.6.2/pcleaner/gui/about_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/ctd_interface_gui.py` & `pcleaner-2.6.2/pcleaner/gui/ctd_interface_gui.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/error_dialog_driver.py` & `pcleaner-2.6.2/pcleaner/gui/error_dialog_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/file_manager_extension_driver.py` & `pcleaner-2.6.2/pcleaner/gui/file_manager_extension_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/file_table.py` & `pcleaner-2.6.2/pcleaner/gui/file_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
             path_str = path if isinstance(path, str) else ", ".join(path)
             gu.show_warning(
                 self,
                 self.tr("Loading Failed"),
                 self.tr("Failed to discover images: {path}").format(path=path_str) + f"\n\n{e}",
             )
             return
-        except:
+        except Exception:
             path_str = path if isinstance(path, str) else ", ".join(path)
             gu.show_exception(
                 self,
                 self.tr("Loading Failed"),
                 self.tr("Failed to load images: {path}").format(path=path_str),
             )
             return
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/gui_utils.py` & `pcleaner-2.6.2/pcleaner/gui/gui_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     """
     Open any given file with the default application.
     """
     logger.debug(f"Opening file {path}")
     try:
         # Use Qt to open the file, so that it works on all platforms.
         Qg.QDesktopServices.openUrl(Qc.QUrl.fromLocalFile(str(path)))
-    except:
+    except Exception:
         show_exception(None, tr("File Error"), tr("Failed to open file."))
 
 
 class CaptureOutput(Qc.QObject):
     text_written = Qc.Signal(str, str)
 
     def __init__(self, *args, **kwargs) -> None:
@@ -190,29 +190,36 @@
 def clamp_8bit(value: int) -> int:
     """
     Clamp a value to the 0-255 range.
     """
     return max(0, min(value, 255))
 
 
-def apply_color_effect(source: Qg.QColor, effect_base: Qg.QColor, contrast_amount: float) -> Qg.QColor:
+def apply_color_effect(
+    source: Qg.QColor, effect_base: Qg.QColor, contrast_amount: float
+) -> Qg.QColor:
     """
     Apply a color effect to a source color.
 
     :param source: The source color.
     :param effect_base: The base color for the effect.
     :param contrast_amount: The amount of contrast to apply.
     :return: The modified color.
     """
     # Essentially alpha blend, with the effect having the contrast amount as the alpha pasted on top.
     r = clamp_8bit(int(source.red() * (1 - contrast_amount) + effect_base.red() * contrast_amount))
-    g = clamp_8bit(int(source.green() * (1 - contrast_amount) + effect_base.green() * contrast_amount))
-    b = clamp_8bit(int(source.blue() * (1 - contrast_amount) + effect_base.blue() * contrast_amount))
+    g = clamp_8bit(
+        int(source.green() * (1 - contrast_amount) + effect_base.green() * contrast_amount)
+    )
+    b = clamp_8bit(
+        int(source.blue() * (1 - contrast_amount) + effect_base.blue() * contrast_amount)
+    )
     return Qg.QColor(r, g, b)
 
+
 def load_color_palette(theme: str) -> Qg.QPalette:
     """
     Provide a theme name and get a QPalette object.
     The name should match one of the files in the themes folder.
 
     :param theme: The name of the theme.
     :return: A QPalette object.
@@ -259,15 +266,17 @@
                 role_mapping = section_role_mapping.get(section, {})
                 qt_color_role = role_mapping.get(key, None)
                 if qt_color_role is not None:
                     r, g, b = map(int, value.split(","))
                     palette.setColor(Qg.QPalette.Normal, qt_color_role, Qg.QColor(r, g, b))
                     palette.setColor(Qg.QPalette.Inactive, qt_color_role, Qg.QColor(r, g, b))
                     # Calculate the disabled color.
-                    disabled_color = apply_color_effect(Qg.QColor(r, g, b), disabled_color, disabled_contrast_amount)
+                    disabled_color = apply_color_effect(
+                        Qg.QColor(r, g, b), disabled_color, disabled_contrast_amount
+                    )
                     palette.setColor(Qg.QPalette.Disabled, qt_color_role, disabled_color)
     else:
         raise ValueError(f"Could not open theme file: {theme}")
 
     # Fallback calculations
     if not palette.color(Qg.QPalette.Light).isValid():
         base = palette.color(Qg.QPalette.Button)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/image_details_driver.py` & `pcleaner-2.6.2/pcleaner/gui/image_details_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/image_file.py` & `pcleaner-2.6.2/pcleaner/gui/image_file.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/image_tab.py` & `pcleaner-2.6.2/pcleaner/gui/image_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,11 +115,10 @@
     @Slot(imf.Step)
     def update_tabs(self, step: imf.Step = None) -> None:
         """
         Update the thumbnails in the currently active image details tab, if any.
 
         :param step: The step to update the thumbnails for.
         """
-        logger.warning(f"Updating tabs with step {step}.")
         current_tab = self.currentWidget()
         if isinstance(current_tab, idd.ImageDetailsWidget):
             current_tab.load_image_thumbnails(step)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/image_viewer.py` & `pcleaner-2.6.2/pcleaner/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/issue_reporter_driver.py` & `pcleaner-2.6.2/pcleaner/gui/issue_reporter_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/launcher.py` & `pcleaner-2.6.2/pcleaner/gui/launcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,83 @@
 import os
 import platform
 import sys
 from io import StringIO
+from PIL import Image
 
 import PySide6
 import PySide6.QtGui as Qg
 import PySide6.QtWidgets as Qw
 import PySide6.QtCore as Qc
 from loguru import logger
 import torch
 from docopt import docopt
 
 import pcleaner.cli_utils as cu
+import pcleaner.gui.gui_utils as gu
 import pcleaner.config as cfg
 from pcleaner import __display_name__, __version__
 from pcleaner.gui.mainwindow_driver import MainWindow
 
+# TODO Things to copy from deepqt:
+# - the testing
+# - the sys.excepthook
+# - the gather themes (potentially)
 
 # This import is needed to load the icons.
-import pcleaner.gui.rc_generated_files.rc_icons
-import pcleaner.gui.rc_generated_files.rc_theme_icons
-import pcleaner.gui.rc_generated_files.rc_themes
-import pcleaner.gui.rc_generated_files.rc_translations
+if platform.system() == "Windows":
+    import pcleaner.gui.rc_generated_files.rc_windows_icons
+    import pcleaner.gui.rc_generated_files.rc_windows_theme_icons
+    import pcleaner.gui.rc_generated_files.rc_windows_themes
+    import pcleaner.gui.rc_generated_files.rc_windows_translations
+else:
+    import pcleaner.gui.rc_generated_files.rc_icons
+    import pcleaner.gui.rc_generated_files.rc_theme_icons
+    import pcleaner.gui.rc_generated_files.rc_themes
+    import pcleaner.gui.rc_generated_files.rc_translations
 
 
 def launch(files_to_open: list[str], debug: bool = False) -> None:
     """
     Launch the GUI.
 
     :param files_to_open: A list of files to open.
     :param debug: Whether to enable debug mode.
     """
 
+    # Ensure that the resources are loaded.
+    # Due to them not being utilized directly, the import statements may be
+    # removed by an errant code formatter
+    if platform.system() == "Windows":
+        assert pcleaner.gui.rc_generated_files.rc_windows_icons
+        assert pcleaner.gui.rc_generated_files.rc_windows_theme_icons
+        assert pcleaner.gui.rc_generated_files.rc_windows_themes
+        assert pcleaner.gui.rc_generated_files.rc_windows_translations
+    else:
+        assert pcleaner.gui.rc_generated_files.rc_icons
+        assert pcleaner.gui.rc_generated_files.rc_theme_icons
+        assert pcleaner.gui.rc_generated_files.rc_themes
+        assert pcleaner.gui.rc_generated_files.rc_translations
+
     cu.get_log_path().parent.mkdir(parents=True, exist_ok=True)
     # Log up to 1MB to the log file.
     # loguru.logfile(str(cu.get_log_path()), maxBytes=2**30, backupCount=1, loglevel=loguru.DEBUG)
 
     # Set up file logging.
     logger.add(str(cu.get_log_path()), rotation="10 MB", retention="1 week", level="DEBUG")
 
+    # Set up a preliminary exception handler so that this still shows up in the log.
+    # Once the gui is up and running it'll be replaced with a call to the gui's error dialog.
+    def exception_handler(exctype, value, traceback) -> None:
+        logger.opt(depth=1, exception=(exctype, value, traceback)).critical(
+            "An uncaught exception was raised"
+        )
+
+    sys.excepthook = exception_handler
+
     logger.info("\n" + cfg.STARTUP_MESSAGE)
     buffer = StringIO()
     buffer.write("\n- Program Information -\n")
     buffer.write(f"Program: {__display_name__} {__version__}\n")
     buffer.write(f"Executing from: {__file__}\n")
     buffer.write(f"Log file: {cu.get_log_path()}\n")
     buffer.write(f"Config file: {cu.get_config_path()}\n")
@@ -117,15 +152,15 @@
         logger.info(f"Files to open: {input_paths}")
 
     try:
         window = MainWindow(config, files_to_open, debug)
         window.show()
         sys.exit(app.exec())
     except Exception:
-        logger.opt(exception=True).critical("Failed to initialize the main window.")
+        gu.show_exception(None, "Failed to launch", "Failed to initialize the main window.")
     finally:
         logger.info(cfg.SHUTDOWN_MESSAGE + "\n")
 
 
 def main():
     docopt_doc = """Panel Cleaner
 
@@ -136,10 +171,13 @@
         <image_path>          One or multiple files or directories to clean.
                               Leave blank to use the current working directory.
         --debug               Enable debug mode.
     """
     args = docopt(docopt_doc, version=f"Panel Cleaner {__version__}")
     launch(args.image_path, args.debug)
 
+    # Allow loading of large images.
+    Image.MAX_IMAGE_PIXELS = 2**32
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/license_driver.py` & `pcleaner-2.6.2/pcleaner/gui/license_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/log_parser.py` & `pcleaner-2.6.2/pcleaner/gui/log_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/log_viewer.py` & `pcleaner-2.6.2/pcleaner/gui/log_viewer.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/mainwindow_driver.py` & `pcleaner-2.6.2/pcleaner/gui/mainwindow_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import platform
 import time
 import psutil
 from copy import deepcopy
 from functools import partial
 from importlib import resources
 from pathlib import Path
@@ -368,14 +369,25 @@
         self.widget_progress_drawer.setStyleSheet("background-color: palette(alternate-base);")
         self.widget_progress_drawer.update()
 
     def post_init(self) -> None:
         """
         Handle any initialization that must be done after the window is shown.
         """
+
+        def exception_handler(exctype, value, traceback) -> None:
+            gu.show_exception(
+                self,
+                "Uncaught Exception",
+                "An uncaught exception was raised.",
+                exception_information=(exctype, value, traceback),
+            )
+
+        sys.excepthook = exception_handler
+
         # Make the profile groupbox the width of 5 save buttons as a good enough heuristic.
         header_button_width = self.pushButton_save_profile.width()
 
         # Make the output panel just large enough for the analytics.
         font_metrics = Qg.QFontMetrics(self.textEdit_analytics.font())
         char_width = font_metrics.averageCharWidth()
         columns = ANALYTICS_COLUMNS
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/model_downloader_driver.py` & `pcleaner-2.6.2/pcleaner/gui/model_downloader_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/new_profile_driver.py` & `pcleaner-2.6.2/pcleaner/gui/new_profile_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/processing.py` & `pcleaner-2.6.2/pcleaner/gui/processing.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/profile_parser.py` & `pcleaner-2.6.2/pcleaner/gui/profile_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_icons.py` & `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.6.2
+# Created by: The Resource Compiler for Qt version 6.7.0
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x14d\
 \x89\
@@ -3055,45 +3055,45 @@
 \x00v\x00g\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x04\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00>\x00\x00\x00\x00\x00\x01\x00\x00\x14h\
-\x00\x00\x01\x8d\xd0\x94\xc5\xfb\
+\x00\x00\x01\x8d/\x07\x1c\xfd\
 \x00\x00\x00T\x00\x00\x00\x00\x00\x01\x00\x00i\xf6\
-\x00\x00\x01\x8b\x01\xf8*\xb1\
+\x00\x00\x01\x8b\x0an\xba\x80\
 \x00\x00\x00\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x87\xd4\x8d\x9c+\
+\x00\x00\x01\x87\x8c\xdf\x0e\xff\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x05\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00l\x00\x02\x00\x00\x00\x05\x00\x00\x00\x0c\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00z\x00\x02\x00\x00\x00\x05\x00\x00\x00\x07\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x01\x00\x00\x04\x00\x00\x00\x01\x00\x00\x87\xc5\
-\x00\x00\x01\x8e:\x5c\xe2c\
+\x00\x00\x01\x8f6C[\xe0\
 \x00\x00\x00\xb6\x00\x00\x00\x00\x00\x01\x00\x00y\x06\
-\x00\x00\x01\x8e:\x5c\xe2c\
+\x00\x00\x01\x8f6C[\xe0\
 \x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x80$\
-\x00\x00\x01\x8e:\x5c\xe2f\
+\x00\x00\x01\x8f6C[\xe0\
 \x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00\x8c0\
-\x00\x00\x01\x8e:\x5c\xe2c\
+\x00\x00\x01\x8f6C[\xe0\
 \x00\x00\x00\x8a\x00\x00\x00\x00\x00\x01\x00\x00qa\
-\x00\x00\x01\x8e:\x5c\xe2c\
+\x00\x00\x01\x8f6C[\xe0\
 \x00\x00\x01\x00\x00\x04\x00\x00\x00\x01\x00\x00\xab\xd5\
-\x00\x00\x01\x8aW\xa8\xe3\x5c\
+\x00\x00\x01\x8b\x0an\xba\x80\
 \x00\x00\x00\xb6\x00\x00\x00\x00\x00\x01\x00\x00\x9d\x16\
-\x00\x00\x01\x8aN7\xcci\
+\x00\x00\x01\x8b\x0an\xba\x80\
 \x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\xa44\
-\x00\x00\x01\x8aW\xa6\xd4\xbf\
+\x00\x00\x01\x8b\x0an\xba\x80\
 \x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00\xb0A\
-\x00\x00\x01\x8e*\xb4\x9e\xbd\
+\x00\x00\x01\x8e\x10T\x97W\
 \x00\x00\x00\x8a\x00\x00\x00\x00\x00\x01\x00\x00\x95q\
-\x00\x00\x01\x8aN7]g\
+\x00\x00\x01\x8b\x0an\xba\x80\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_theme_icons.py` & `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_theme_icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.6.2
+# Created by: The Resource Compiler for Qt version 6.7.0
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x0e\x00\
 (\
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_themes.py` & `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_themes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.6.2
+# Created by: The Resource Compiler for Qt version 6.7.0
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x02F\
 (\
@@ -101,17 +101,17 @@
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00$\x00\x04\x00\x00\x00\x01\x00\x00\x02J\
-\x00\x00\x01\x8a\x0b\xf6\xcb\xb0\
+\x00\x00\x01\x8b\x0an\xba\x97\
 \x00\x00\x00\x12\x00\x04\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x8a\x0b\xf6\xcb\xb0\
+\x00\x00\x01\x8b\x0an\xba\x97\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/rc_generated_files/rc_translations.py` & `pcleaner-2.6.2/pcleaner/gui/rc_generated_files/rc_translations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.6.2
+# Created by: The Resource Compiler for Qt version 6.7.0
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00W\xc6\
 (\
@@ -7203,23 +7203,23 @@
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x05\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\xde\x00\x04\x00\x00\x00\x01\x00\x01g\x18\
-\x00\x00\x01\x8e:]\x09\xf5\
+\x00\x00\x01\x8f6Ct,\
 \x00\x00\x00\x1e\x00\x04\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x8e:]\x0d0\
+\x00\x00\x01\x8f6CuK\
 \x00\x00\x00\xae\x00\x04\x00\x00\x00\x01\x00\x01\x0c\xe5\
-\x00\x00\x01\x8e:]\x0eK\
+\x00\x00\x01\x8f6Cu\x94\
 \x00\x00\x00N\x00\x04\x00\x00\x00\x01\x00\x00W\xca\
-\x00\x00\x01\x8e:]\x0b(\
+\x00\x00\x01\x8f6Ct\x83\
 \x00\x00\x00~\x00\x04\x00\x00\x00\x01\x00\x00\xb5\x1e\
-\x00\x00\x01\x8e:]\x0c,\
+\x00\x00\x01\x8f6Ct\xfb\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/setup_greeter_driver.py` & `pcleaner-2.6.2/pcleaner/gui/setup_greeter_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/structures.py` & `pcleaner-2.6.2/pcleaner/gui/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/supported_languages.py` & `pcleaner-2.6.2/pcleaner/gui/supported_languages.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_About.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_About.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'About.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'ErrorDialog.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'FileManagerIntegration.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'ImageDetails.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_IssueReporter.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_IssueReporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'IssueReporter.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_License.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_License.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'License.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'Mainwindow.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'ModelDownloader.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_NewProfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'NewProfile.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py` & `pcleaner-2.6.2/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'SetupGreeter.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `pcleaner-2.6.1/pcleaner/gui/worker_thread.py` & `pcleaner-2.6.2/pcleaner/gui/worker_thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         # the instance that the program was closed while the worker was running.
         # Otherwise the Python runtime crashes, which is ok in this state, but it just isn't very nice.
         try:
             try:
                 result = self.fn(*self.args, **self.kwargs)
             except Abort:
                 self.signals.aborted.emit((self.args, self.kwargs))
-            except:
+            except Exception:
                 # traceback.print_exc()  # Disabled because we handle showing the error in whatever
                 # called the worker. This also prevents the runtime errors from getting printed, which
                 # are caught in an outer try block.
                 # Use traceback.format_exc() to get the traceback as a string.
                 # Using the raw traceback instead and letting the logger format that instead though.
                 exception_type, value, traceback = sys.exc_info()
                 self.signals.error.emit(
```

### Comparing `pcleaner-2.6.1/pcleaner/helpers.py` & `pcleaner-2.6.2/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/image_ops.py` & `pcleaner-2.6.2/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/inpainting.py` & `pcleaner-2.6.2/pcleaner/inpainting.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/main.py` & `pcleaner-2.6.2/pcleaner/main.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/masker.py` & `pcleaner-2.6.2/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/model_downloader.py` & `pcleaner-2.6.2/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/preprocessor.py` & `pcleaner-2.6.2/pcleaner/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/profile_cli.py` & `pcleaner-2.6.2/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner/structures.py` & `pcleaner-2.6.2/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/pcleaner.egg-info/PKG-INFO` & `pcleaner-2.6.2/pcleaner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 2.6.1
+Version: 2.6.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -93,14 +93,16 @@
 
 ## Features
 
 - Cleans text bubbles without leaving artifacts.
 
 - Avoids painting over parts of the image that aren't text.
 
+- Inpaints bubbles that can't simply be masked out.
+
 - Ignores bubbles containing only symbols or numbers, as those don't need translation.
 
 - Offers a GUI for easy use, dark, light, and system themes are supported.
 
 - No internet connection required after installing the model data.
 
 - Offers a plethora of options to customize the cleaning process and the ability to save multiple presets as profiles.
@@ -318,14 +320,16 @@
 ## Acknowledgements
 
 - [Comic Text Detector](https://github.com/dmMaze/comic-text-detector) for finding text bubbles and generating the initial mask.
 
 - [Manga OCR](https://github.com/kha-white/manga-ocr) for detecting which bubbles only contain symbols or numbers,
   and performing the dedicated OCR command.
 
+- [Simple Lama Inpainting](https://github.com/enesmsahin/simple-lama-inpainting) for inpainting bubbles that can't be masked out.
+
 
 ## License
 
 This project is licensed under the GNU General Public License v3.0 – see
 the [LICENSE](https://raw.githubusercontent.com/VoxelCubes/PanelCleaner/master/LICENSE) file for details.
```

### Comparing `pcleaner-2.6.1/pcleaner.egg-info/SOURCES.txt` & `pcleaner-2.6.2/pcleaner.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 pcleaner/gui/CustomQ/CTooltipLabel.py
 pcleaner/gui/CustomQ/__init__.py
 pcleaner/gui/rc_generated_files/__init__.py
 pcleaner/gui/rc_generated_files/rc_icons.py
 pcleaner/gui/rc_generated_files/rc_theme_icons.py
 pcleaner/gui/rc_generated_files/rc_themes.py
 pcleaner/gui/rc_generated_files/rc_translations.py
+pcleaner/gui/rc_generated_files/rc_windows_icons.py
+pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py
+pcleaner/gui/rc_generated_files/rc_windows_themes.py
+pcleaner/gui/rc_generated_files/rc_windows_translations.py
 pcleaner/gui/ui_generated_files/__init__.py
 pcleaner/gui/ui_generated_files/ui_About.py
 pcleaner/gui/ui_generated_files/ui_ErrorDialog.py
 pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py
 pcleaner/gui/ui_generated_files/ui_ImageDetails.py
 pcleaner/gui/ui_generated_files/ui_IssueReporter.py
 pcleaner/gui/ui_generated_files/ui_License.py
```

### Comparing `pcleaner-2.6.1/setup.cfg` & `pcleaner-2.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pcleaner-2.6.1/tests/test_log_parser.py` & `pcleaner-2.6.2/tests/test_log_parser.py`

 * *Files identical despite different names*

