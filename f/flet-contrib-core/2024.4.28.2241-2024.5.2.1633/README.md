# Comparing `tmp/flet_contrib_core-2024.4.28.2241.tar.gz` & `tmp/flet_contrib_core-2024.5.2.1633.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_core-2024.4.28.2241.tar", max compression
+gzip compressed data, was "flet_contrib_core-2024.5.2.1633.tar", max compression
```

## Comparing `flet_contrib_core-2024.4.28.2241.tar` & `flet_contrib_core-2024.5.2.1633.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0      189 2024-04-28 22:41:12.996649 flet_contrib_core-2024.4.28.2241/README.md
--rw-r--r--   0        0        0      673 2024-04-28 22:41:58.736899 flet_contrib_core-2024.4.28.2241/pyproject.toml
--rw-r--r--   0        0        0    10950 2024-04-28 22:41:12.996649 flet_contrib_core-2024.4.28.2241/src/flet_core/__init__.py
--rw-r--r--   0        0        0      434 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/adaptive_control.py
--rw-r--r--   0        0        0    13342 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/alignment.py
--rw-r--r--   0        0        0     6757 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     1955 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/animation.py
--rw-r--r--   0        0        0    11031 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7915 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/audio.py
--rw-r--r--   0        0        0     8439 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/audio_recorder.py
--rw-r--r--   0        0        0     5781 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/badge.py
--rw-r--r--   0        0        0     8099 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/banner.py
--rw-r--r--   0        0        0      326 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/blur.py
--rw-r--r--   0        0        0     1079 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/border.py
--rw-r--r--   0        0        0      958 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     5930 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/bottom_app_bar.py
--rw-r--r--   0        0        0     5830 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2103 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/buttons.py
--rw-r--r--   0        0        0      514 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__init__.py
--rw-r--r--   0        0        0      846 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3524 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc
--rw-r--r--   0        0        0     4799 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc
--rw-r--r--   0        0        0     2352 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc
--rw-r--r--   0        0        0     1800 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/color.cpython-39.pyc
--rw-r--r--   0        0        0     1439 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc
--rw-r--r--   0        0        0     2596 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/line.cpython-39.pyc
--rw-r--r--   0        0        0     2606 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc
--rw-r--r--   0        0        0     4856 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/path.cpython-39.pyc
--rw-r--r--   0        0        0     2490 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/points.cpython-39.pyc
--rw-r--r--   0        0        0     3005 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc
--rw-r--r--   0        0        0     2534 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc
--rw-r--r--   0        0        0      704 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc
--rw-r--r--   0        0        0     4879 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/text.cpython-39.pyc
--rw-r--r--   0        0        0     2910 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/arc.py
--rw-r--r--   0        0        0     4813 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/canvas.py
--rw-r--r--   0        0        0     1646 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/circle.py
--rw-r--r--   0        0        0     1236 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/color.py
--rw-r--r--   0        0        0      844 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/fill.py
--rw-r--r--   0        0        0     1869 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/line.py
--rw-r--r--   0        0        0     1891 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/oval.py
--rw-r--r--   0        0        0     3493 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/path.py
--rw-r--r--   0        0        0     1813 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/points.py
--rw-r--r--   0        0        0     2345 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/rect.py
--rw-r--r--   0        0        0     1951 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/shadow.py
--rw-r--r--   0        0        0      347 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/shape.py
--rw-r--r--   0        0        0     4172 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/text.py
--rw-r--r--   0        0        0     8220 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/card.py
--rw-r--r--   0        0        0     9184 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc
--rw-r--r--   0        0        0     2761 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc
--rw-r--r--   0        0        0     7264 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc
--rw-r--r--   0        0        0     2642 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc
--rw-r--r--   0        0        0     3314 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc
--rw-r--r--   0        0        0     1867 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc
--rw-r--r--   0        0        0      693 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc
--rw-r--r--   0        0        0      654 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc
--rw-r--r--   0        0        0     1541 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc
--rw-r--r--   0        0        0    10717 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc
--rw-r--r--   0        0        0     9157 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc
--rw-r--r--   0        0        0     5936 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc
--rw-r--r--   0        0        0     5564 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc
--rw-r--r--   0        0        0     4511 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc
--rw-r--r--   0        0        0     9932 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2044 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6679 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1932 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2923 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11305 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     9357 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5338 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5965 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3807 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0    12179 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/checkbox.py
--rw-r--r--   0        0        0    14830 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/chip.py
--rw-r--r--   0        0        0     9261 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3097 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/client_storage.py
--rw-r--r--   0        0        0    10869 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/colors.py
--rw-r--r--   0        0        0     6968 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/column.py
--rw-r--r--   0        0        0      877 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/connection.py
--rw-r--r--   0        0        0     7224 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    15069 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/container.py
--rw-r--r--   0        0        0    17732 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/control_event.py
--rw-r--r--   0        0        0     4387 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_action_sheet.py
--rw-r--r--   0        0        0     4507 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_action_sheet_action.py
--rw-r--r--   0        0        0     3102 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_activity_indicator.py
--rw-r--r--   0        0        0     3947 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_alert_dialog.py
--rw-r--r--   0        0        0     5453 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_app_bar.py
--rw-r--r--   0        0        0     3108 2024-04-28 22:41:13.008649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_bottom_sheet.py
--rw-r--r--   0        0        0     7697 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_button.py
--rw-r--r--   0        0        0     6851 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_checkbox.py
--rw-r--r--   0        0        0     2260 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_colors.py
--rw-r--r--   0        0        0     2464 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_context_menu.py
--rw-r--r--   0        0        0     3016 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_context_menu_action.py
--rw-r--r--   0        0        0     8126 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_date_picker.py
--rw-r--r--   0        0        0     3667 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_dialog_action.py
--rw-r--r--   0        0        0     2706 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_filled_button.py
--rw-r--r--   0        0        0    61696 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_icons.py
--rw-r--r--   0        0        0     9207 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_list_tile.py
--rw-r--r--   0        0        0     6378 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_navigation_bar.py
--rw-r--r--   0        0        0     6847 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_picker.py
--rw-r--r--   0        0        0     6833 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_radio.py
--rw-r--r--   0        0        0     5590 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_segmented_button.py
--rw-r--r--   0        0        0     6429 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_slider.py
--rw-r--r--   0        0        0     4722 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_sliding_segmented_button.py
--rw-r--r--   0        0        0     7545 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_switch.py
--rw-r--r--   0        0        0    10254 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_textfield.py
--rw-r--r--   0        0        0     5308 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_timer_picker.py
--rw-r--r--   0        0        0    21708 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/datatable.py
--rw-r--r--   0        0        0    11675 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/date_picker.py
--rw-r--r--   0        0        0    10163 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/dismissible.py
--rw-r--r--   0        0        0     3081 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/divider.py
--rw-r--r--   0        0        0     7147 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6701 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/draggable.py
--rw-r--r--   0        0        0    14762 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/dropdown.py
--rw-r--r--   0        0        0    10571 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     1978 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/event.py
--rw-r--r--   0        0        0     1250 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9795 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/expansion_panel.py
--rw-r--r--   0        0        0    13461 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/expansion_tile.py
--rw-r--r--   0        0        0     9659 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2886 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     3020 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     3608 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/flet_app.py
--rw-r--r--   0        0        0    11149 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    15979 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    27285 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1432 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/gradients.py
--rw-r--r--   0        0        0     8485 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2315 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3849 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/icon.py
--rw-r--r--   0        0        0    13137 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362386 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/icons.py
--rw-r--r--   0        0        0     7812 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/image.py
--rw-r--r--   0        0        0      367 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/inline_span.py
--rw-r--r--   0        0        0    17916 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     8075 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/list_view.py
--rw-r--r--   0        0        0    10049 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      219 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/locks.py
--rw-r--r--   0        0        0     5591 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/lottie.py
--rw-r--r--   0        0        0      583 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/margin.py
--rw-r--r--   0        0        0     5894 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5015 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     4319 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/menu_bar.py
--rw-r--r--   0        0        0     7484 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/menu_item_button.py
--rw-r--r--   0        0        0     1486 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/merge_semantics.py
--rw-r--r--   0        0        0    11864 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0     9992 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/navigation_drawer.py
--rw-r--r--   0        0        0    15476 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     8550 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/padding.py
--rw-r--r--   0        0        0    63608 2024-04-28 22:41:13.012649 flet_contrib_core-2024.4.28.2241/src/flet_core/page.py
--rw-r--r--   0        0        0    10503 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/pagelet.py
--rw-r--r--   0        0        0     2746 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/painting.py
--rw-r--r--   0        0        0     4235 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0    13789 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     5600 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     5663 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4163 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/protocol.py
--rw-r--r--   0        0        0      106 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/__init__.py
--rw-r--r--   0        0        0      310 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4520 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc
--rw-r--r--   0        0        0     5620 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc
--rw-r--r--   0        0        0     3393 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/pubsub_client.py
--rw-r--r--   0        0        0     5873 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/pubsub_hub.py
--rw-r--r--   0        0        0     3419 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/querystring.py
--rw-r--r--   0        0        0     9309 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/radio.py
--rw-r--r--   0        0        0     2350 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/radio_group.py
--rw-r--r--   0        0        0     8133 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/range_slider.py
--rw-r--r--   0        0        0      291 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/ref.py
--rw-r--r--   0        0        0     6438 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     5326 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/rive.py
--rw-r--r--   0        0        0     6989 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/row.py
--rw-r--r--   0        0        0     5151 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/safe_area.py
--rw-r--r--   0        0        0     4513 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/scrollable_control.py
--rw-r--r--   0        0        0    14078 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/search_bar.py
--rw-r--r--   0        0        0     8430 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/segmented_button.py
--rw-r--r--   0        0        0     1690 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/selection_area.py
--rw-r--r--   0        0        0    16317 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/semantics.py
--rw-r--r--   0        0        0     1186 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/semantics_service.py
--rw-r--r--   0        0        0      576 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5260 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2938 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0    10403 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/slider.py
--rw-r--r--   0        0        0     8473 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     5651 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/stack.py
--rw-r--r--   0        0        0     8403 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/submenu_button.py
--rw-r--r--   0        0        0    11516 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/switch.py
--rw-r--r--   0        0        0    14308 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10900 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/text.py
--rw-r--r--   0        0        0     8065 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/text_button.py
--rw-r--r--   0        0        0     3282 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/text_span.py
--rw-r--r--   0        0        0     1375 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/text_style.py
--rw-r--r--   0        0        0    18286 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/textfield.py
--rw-r--r--   0        0        0    32507 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/theme.py
--rw-r--r--   0        0        0     8094 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/time_picker.py
--rw-r--r--   0        0        0     9157 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/transform.py
--rw-r--r--   0        0        0     2847 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     3476 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/two_dimensional_scrollables.py
--rw-r--r--   0        0        0     6265 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/types.py
--rw-r--r--   0        0        0      450 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/user_control.py
--rw-r--r--   0        0        0      311 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__init__.py
--rw-r--r--   0        0        0      567 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      823 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc
--rw-r--r--   0        0        0      562 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1220 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc
--rw-r--r--   0        0        0      692 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc
--rw-r--r--   0        0        0      565 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/strings.cpython-39.pyc
--rw-r--r--   0        0        0     4687 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/vector.cpython-39.pyc
--rw-r--r--   0        0        0      271 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/classproperty.py
--rw-r--r--   0        0        0      243 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/concurrency_utils.py
--rw-r--r--   0        0        0      835 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/deprecated.py
--rw-r--r--   0        0        0      465 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/slugify.py
--rw-r--r--   0        0        0      178 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/strings.py
--rw-r--r--   0        0        0     3207 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/utils/vector.py
--rw-r--r--   0        0        0       90 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/version.py
--rw-r--r--   0        0        0     3123 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0    17853 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/video.py
--rw-r--r--   0        0        0     8864 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/view.py
--rw-r--r--   0        0        0     6042 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/webview.py
--rw-r--r--   0        0        0     4181 2024-04-28 22:41:13.016649 flet_contrib_core-2024.4.28.2241/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 flet_contrib_core-2024.4.28.2241/PKG-INFO
+-rw-r--r--   0        0        0      189 2024-05-02 16:33:07.099091 flet_contrib_core-2024.5.2.1633/README.md
+-rw-r--r--   0        0        0      673 2024-05-02 16:33:54.435516 flet_contrib_core-2024.5.2.1633/pyproject.toml
+-rw-r--r--   0        0        0    10950 2024-05-02 16:33:07.099091 flet_contrib_core-2024.5.2.1633/src/flet_core/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/adaptive_control.py
+-rw-r--r--   0        0        0    13342 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     6757 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     1955 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/animation.py
+-rw-r--r--   0        0        0    11031 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7915 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/audio.py
+-rw-r--r--   0        0        0     8439 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/audio_recorder.py
+-rw-r--r--   0        0        0     5781 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/badge.py
+-rw-r--r--   0        0        0     8099 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/banner.py
+-rw-r--r--   0        0        0      326 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/blur.py
+-rw-r--r--   0        0        0     1079 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/border.py
+-rw-r--r--   0        0        0      958 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     5930 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/bottom_app_bar.py
+-rw-r--r--   0        0        0     5830 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2103 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/buttons.py
+-rw-r--r--   0        0        0      514 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__init__.py
+-rw-r--r--   0        0        0      853 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3531 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc
+-rw-r--r--   0        0        0     4806 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc
+-rw-r--r--   0        0        0     2359 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc
+-rw-r--r--   0        0        0     1807 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/color.cpython-39.pyc
+-rw-r--r--   0        0        0     1446 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc
+-rw-r--r--   0        0        0     2603 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/line.cpython-39.pyc
+-rw-r--r--   0        0        0     2613 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc
+-rw-r--r--   0        0        0     4863 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/path.cpython-39.pyc
+-rw-r--r--   0        0        0     2497 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/points.cpython-39.pyc
+-rw-r--r--   0        0        0     3012 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc
+-rw-r--r--   0        0        0     2541 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc
+-rw-r--r--   0        0        0      711 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc
+-rw-r--r--   0        0        0     4886 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/text.cpython-39.pyc
+-rw-r--r--   0        0        0     2910 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/arc.py
+-rw-r--r--   0        0        0     4813 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/canvas.py
+-rw-r--r--   0        0        0     1646 2024-05-02 16:33:07.107091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/circle.py
+-rw-r--r--   0        0        0     1236 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/color.py
+-rw-r--r--   0        0        0      844 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/fill.py
+-rw-r--r--   0        0        0     1869 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/line.py
+-rw-r--r--   0        0        0     1891 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/oval.py
+-rw-r--r--   0        0        0     3493 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/path.py
+-rw-r--r--   0        0        0     1813 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/points.py
+-rw-r--r--   0        0        0     2345 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/rect.py
+-rw-r--r--   0        0        0     1951 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/shadow.py
+-rw-r--r--   0        0        0      347 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/shape.py
+-rw-r--r--   0        0        0     4172 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/text.py
+-rw-r--r--   0        0        0     8220 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/card.py
+-rw-r--r--   0        0        0     9191 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     2768 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc
+-rw-r--r--   0        0        0     7271 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc
+-rw-r--r--   0        0        0     2649 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc
+-rw-r--r--   0        0        0     3321 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc
+-rw-r--r--   0        0        0      700 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc
+-rw-r--r--   0        0        0      661 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1548 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc
+-rw-r--r--   0        0        0    10724 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     9164 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc
+-rw-r--r--   0        0        0     5943 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc
+-rw-r--r--   0        0        0     5571 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     4518 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc
+-rw-r--r--   0        0        0     9932 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2044 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6679 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1932 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2923 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11305 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     9357 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5338 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5965 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3807 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0    12179 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0    14830 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/chip.py
+-rw-r--r--   0        0        0     9261 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3097 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0    10869 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/colors.py
+-rw-r--r--   0        0        0     6968 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/column.py
+-rw-r--r--   0        0        0      877 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/connection.py
+-rw-r--r--   0        0        0     7224 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    15069 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/container.py
+-rw-r--r--   0        0        0    17732 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/control_event.py
+-rw-r--r--   0        0        0     4387 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_action_sheet.py
+-rw-r--r--   0        0        0     4507 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_action_sheet_action.py
+-rw-r--r--   0        0        0     3102 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_activity_indicator.py
+-rw-r--r--   0        0        0     3947 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_alert_dialog.py
+-rw-r--r--   0        0        0     5453 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_app_bar.py
+-rw-r--r--   0        0        0     3108 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_bottom_sheet.py
+-rw-r--r--   0        0        0     7697 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_button.py
+-rw-r--r--   0        0        0     6851 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_checkbox.py
+-rw-r--r--   0        0        0     2260 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_colors.py
+-rw-r--r--   0        0        0     2464 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_context_menu.py
+-rw-r--r--   0        0        0     3016 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_context_menu_action.py
+-rw-r--r--   0        0        0     8126 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_date_picker.py
+-rw-r--r--   0        0        0     3667 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_dialog_action.py
+-rw-r--r--   0        0        0     2706 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_filled_button.py
+-rw-r--r--   0        0        0    61696 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_icons.py
+-rw-r--r--   0        0        0     9207 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_list_tile.py
+-rw-r--r--   0        0        0     6378 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_navigation_bar.py
+-rw-r--r--   0        0        0     6847 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_picker.py
+-rw-r--r--   0        0        0     6833 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_radio.py
+-rw-r--r--   0        0        0     5590 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_segmented_button.py
+-rw-r--r--   0        0        0     6429 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_slider.py
+-rw-r--r--   0        0        0     4722 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_sliding_segmented_button.py
+-rw-r--r--   0        0        0     7545 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_switch.py
+-rw-r--r--   0        0        0    10254 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_textfield.py
+-rw-r--r--   0        0        0     5308 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_timer_picker.py
+-rw-r--r--   0        0        0    21708 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/datatable.py
+-rw-r--r--   0        0        0    11675 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/date_picker.py
+-rw-r--r--   0        0        0    10163 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/dismissible.py
+-rw-r--r--   0        0        0     3081 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/divider.py
+-rw-r--r--   0        0        0     7147 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6701 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/draggable.py
+-rw-r--r--   0        0        0    14762 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0    10571 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     1978 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/event.py
+-rw-r--r--   0        0        0     1250 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9795 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/expansion_panel.py
+-rw-r--r--   0        0        0    13461 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/expansion_tile.py
+-rw-r--r--   0        0        0     9659 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2886 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     3020 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     3608 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0    11149 2024-05-02 16:33:07.111091 flet_contrib_core-2024.5.2.1633/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    15979 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    27285 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1432 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     8485 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     2315 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3849 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/icon.py
+-rw-r--r--   0        0        0    13137 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362386 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/icons.py
+-rw-r--r--   0        0        0     7812 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/image.py
+-rw-r--r--   0        0        0      367 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/inline_span.py
+-rw-r--r--   0        0        0    17916 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     8075 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/list_view.py
+-rw-r--r--   0        0        0    10049 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      219 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/locks.py
+-rw-r--r--   0        0        0     5591 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/lottie.py
+-rw-r--r--   0        0        0      583 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/margin.py
+-rw-r--r--   0        0        0     5894 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5015 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     4319 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/menu_bar.py
+-rw-r--r--   0        0        0     7484 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/menu_item_button.py
+-rw-r--r--   0        0        0     1486 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/merge_semantics.py
+-rw-r--r--   0        0        0    11864 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0     9992 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/navigation_drawer.py
+-rw-r--r--   0        0        0    15476 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     8550 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/padding.py
+-rw-r--r--   0        0        0    63608 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/page.py
+-rw-r--r--   0        0        0    10503 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/pagelet.py
+-rw-r--r--   0        0        0     2746 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/painting.py
+-rw-r--r--   0        0        0     4235 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0    13789 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     5600 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     5663 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4163 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/protocol.py
+-rw-r--r--   0        0        0      106 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4527 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc
+-rw-r--r--   0        0        0     5627 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc
+-rw-r--r--   0        0        0     3393 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/pubsub_client.py
+-rw-r--r--   0        0        0     5873 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/pubsub_hub.py
+-rw-r--r--   0        0        0     3419 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     9309 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2350 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0     8133 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/range_slider.py
+-rw-r--r--   0        0        0      291 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6438 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     5326 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/rive.py
+-rw-r--r--   0        0        0     6989 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/row.py
+-rw-r--r--   0        0        0     5151 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/safe_area.py
+-rw-r--r--   0        0        0     4513 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/scrollable_control.py
+-rw-r--r--   0        0        0    14078 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/search_bar.py
+-rw-r--r--   0        0        0     8430 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/segmented_button.py
+-rw-r--r--   0        0        0     1690 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/selection_area.py
+-rw-r--r--   0        0        0    16317 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/semantics.py
+-rw-r--r--   0        0        0     1186 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/semantics_service.py
+-rw-r--r--   0        0        0      576 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5260 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2938 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0    10403 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/slider.py
+-rw-r--r--   0        0        0     8473 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     5651 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8403 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/submenu_button.py
+-rw-r--r--   0        0        0    11516 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/switch.py
+-rw-r--r--   0        0        0    14308 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10900 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/text.py
+-rw-r--r--   0        0        0     8065 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/text_button.py
+-rw-r--r--   0        0        0     3282 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/text_span.py
+-rw-r--r--   0        0        0     1375 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    18286 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/textfield.py
+-rw-r--r--   0        0        0    32507 2024-05-02 16:33:07.115091 flet_contrib_core-2024.5.2.1633/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8094 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/time_picker.py
+-rw-r--r--   0        0        0     9157 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2847 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     3476 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/two_dimensional_scrollables.py
+-rw-r--r--   0        0        0     6265 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/types.py
+-rw-r--r--   0        0        0      450 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/user_control.py
+-rw-r--r--   0        0        0      311 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      830 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc
+-rw-r--r--   0        0        0      569 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1227 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc
+-rw-r--r--   0        0        0      699 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc
+-rw-r--r--   0        0        0      572 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/strings.cpython-39.pyc
+-rw-r--r--   0        0        0     4694 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/vector.cpython-39.pyc
+-rw-r--r--   0        0        0      271 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/classproperty.py
+-rw-r--r--   0        0        0      243 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/concurrency_utils.py
+-rw-r--r--   0        0        0      835 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/deprecated.py
+-rw-r--r--   0        0        0      465 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/slugify.py
+-rw-r--r--   0        0        0      178 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/strings.py
+-rw-r--r--   0        0        0     3207 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/utils/vector.py
+-rw-r--r--   0        0        0       96 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/version.py
+-rw-r--r--   0        0        0     3123 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0    17853 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/video.py
+-rw-r--r--   0        0        0     8864 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/view.py
+-rw-r--r--   0        0        0     6042 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/webview.py
+-rw-r--r--   0        0        0     4181 2024-05-02 16:33:07.119091 flet_contrib_core-2024.5.2.1633/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 flet_contrib_core-2024.5.2.1633/PKG-INFO
```

### Comparing `flet_contrib_core-2024.4.28.2241/pyproject.toml` & `flet_contrib_core-2024.5.2.1633/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-core"
-version = "2024.04.28.2241"
+version = "2024.05.02.1633"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/__init__.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/alert_dialog.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/animated_switcher.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/animation.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/app_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/audio.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/audio_recorder.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/audio_recorder.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/badge.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/badge.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/banner.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/border.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/border_radius.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/bottom_app_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/bottom_app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/bottom_sheet.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/buttons.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__init__.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 514 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 0202 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 0202 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
@@ -38,16 +38,17 @@
 00000250: 616e 7661 732e 706f 696e 7473 720b 0000  anvas.pointsr...
 00000260: 0072 0c00 0000 5a15 666c 6574 5f63 6f72  .r....Z.flet_cor
 00000270: 652e 6361 6e76 6173 2e72 6563 7472 0d00  e.canvas.rectr..
 00000280: 0000 5a17 666c 6574 5f63 6f72 652e 6361  ..Z.flet_core.ca
 00000290: 6e76 6173 2e73 6861 646f 7772 0e00 0000  nvas.shadowr....
 000002a0: 5a15 666c 6574 5f63 6f72 652e 6361 6e76  Z.flet_core.canv
 000002b0: 6173 2e74 6578 7472 0f00 0000 a900 7210  as.textr......r.
-000002c0: 0000 0072 1000 0000 fa5b 2f77 6f72 6b73  ...r.....[/works
+000002c0: 0000 0072 1000 0000 fa62 2f77 6f72 6b73  ...r.....b/works
 000002d0: 7061 6365 732f 636f 6e74 7269 6266 6c65  paces/contribfle
-000002e0: 742f 666c 6574 2f73 646b 2f70 7974 686f  t/flet/sdk/pytho
-000002f0: 6e2f 7061 636b 6167 6573 2f66 6c65 742d  n/packages/flet-
-00000300: 636f 7265 2f73 7263 2f66 6c65 745f 636f  core/src/flet_co
-00000310: 7265 2f63 616e 7661 732f 5f5f 696e 6974  re/canvas/__init
-00000320: 5f5f 2e70 79da 083c 6d6f 6475 6c65 3e01  __.py..<module>.
-00000330: 0000 0073 1600 0000 0c01 1001 0c01 0c01  ...s............
-00000340: 0c01 0c01 0c01 0c01 1001 0c01 0c01       ..............
+000002e0: 742f 666c 6574 636f 6e74 7269 622f 7364  t/fletcontrib/sd
+000002f0: 6b2f 7079 7468 6f6e 2f70 6163 6b61 6765  k/python/package
+00000300: 732f 666c 6574 2d63 6f72 652f 7372 632f  s/flet-core/src/
+00000310: 666c 6574 5f63 6f72 652f 6361 6e76 6173  flet_core/canvas
+00000320: 2f5f 5f69 6e69 745f 5f2e 7079 da08 3c6d  /__init__.py..<m
+00000330: 6f64 756c 653e 0100 0000 7316 0000 000c  odule>....s.....
+00000340: 0110 010c 010c 010c 010c 010c 010c 0110  ................
+00000350: 010c 010c 01                             .....
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 2910 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 5e0b 0000  a........:)f^...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 5e0b 0000  a........./f^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
@@ -55,167 +55,167 @@
 00000360: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
 00000370: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
 00000380: 720f 0000 0029 0dda 0473 656c 6672 0800  r....)...selfr..
 00000390: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
 000003a0: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
 000003b0: 720f 0000 0072 1300 0000 7210 0000 0072  r....r....r....r
 000003c0: 1100 0000 7212 0000 00a9 0072 1600 0000  ....r......r....
-000003d0: fa56 2f77 6f72 6b73 7061 6365 732f 636f  .V/workspaces/co
-000003e0: 6e74 7269 6266 6c65 742f 666c 6574 2f73  ntribflet/flet/s
-000003f0: 646b 2f70 7974 686f 6e2f 7061 636b 6167  dk/python/packag
-00000400: 6573 2f66 6c65 742d 636f 7265 2f73 7263  es/flet-core/src
-00000410: 2f66 6c65 745f 636f 7265 2f63 616e 7661  /flet_core/canva
-00000420: 732f 6172 632e 7079 7214 0000 0009 0000  s/arc.pyr.......
-00000430: 0073 1200 0000 0012 1402 0601 0601 0601  .s..............
-00000440: 0601 0601 0601 0601 7a0c 4172 632e 5f5f  ........z.Arc.__
-00000450: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000460: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00000470: 0400 0000 6401 5300 2902 4e5a 0361 7263  ....d.S.).NZ.arc
-00000480: 7216 0000 00a9 0172 1500 0000 7216 0000  r......r....r...
-00000490: 0072 1600 0000 7217 0000 00da 115f 6765  .r....r......_ge
-000004a0: 745f 636f 6e74 726f 6c5f 6e61 6d65 2600  t_control_name&.
-000004b0: 0000 7302 0000 0000 017a 1541 7263 2e5f  ..s......z.Arc._
-000004c0: 6765 745f 636f 6e74 726f 6c5f 6e61 6d65  get_control_name
-000004d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000004e0: 0004 0000 0003 0000 0073 1c00 0000 7400  .........s....t.
-000004f0: 8300 a001 a100 0100 7c00 a002 6401 7c00  ........|...d.|.
-00000500: 6a03 a102 0100 6400 5300 2902 4e72 0f00  j.....d.S.).Nr..
-00000510: 0000 2904 da05 7375 7065 72da 0d62 6566  ..)...super..bef
-00000520: 6f72 655f 7570 6461 7465 da0e 5f73 6574  ore_update.._set
-00000530: 5f61 7474 725f 6a73 6f6e da0b 5f41 7263  _attr_json.._Arc
-00000540: 5f5f 7061 696e 7472 1800 0000 a901 da09  __paintr........
-00000550: 5f5f 636c 6173 735f 5f72 1600 0000 7217  __class__r....r.
-00000560: 0000 0072 1b00 0000 2900 0000 7304 0000  ...r....)...s...
-00000570: 0000 010a 017a 1141 7263 2e62 6566 6f72  .....z.Arc.befor
-00000580: 655f 7570 6461 7465 2901 da06 7265 7475  e_update)...retu
-00000590: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
-000005a0: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
-000005b0: 7c00 a000 6401 a101 5300 a902 4e72 0800  |...d...S...Nr..
-000005c0: 0000 a901 da09 5f67 6574 5f61 7474 7272  ......_get_attrr
-000005d0: 1800 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-000005e0: 0000 0072 0800 0000 2e00 0000 7302 0000  ...r........s...
-000005f0: 0000 027a 0541 7263 2e78 2901 da05 7661  ...z.Arc.x)...va
-00000600: 6c75 6563 0200 0000 0000 0000 0000 0000  luec............
-00000610: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-00000620: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
-00000630: 0072 2100 0000 a901 da09 5f73 6574 5f61  .r!......._set_a
-00000640: 7474 72a9 0272 1500 0000 7224 0000 0072  ttr..r....r$...r
-00000650: 1600 0000 7216 0000 0072 1700 0000 7208  ....r....r....r.
-00000660: 0000 0032 0000 0073 0200 0000 0002 6301  ...2...s......c.
-00000670: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000680: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
-00000690: 6401 a101 5300 a902 4e72 0900 0000 7222  d...S...Nr....r"
-000006a0: 0000 0072 1800 0000 7216 0000 0072 1600  ...r....r....r..
-000006b0: 0000 7217 0000 0072 0900 0000 3700 0000  ..r....r....7...
-000006c0: 7302 0000 0000 027a 0541 7263 2e79 6302  s......z.Arc.yc.
-000006d0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000006e0: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-000006f0: 6401 7c01 a102 0100 6400 5300 7228 0000  d.|.....d.S.r(..
-00000700: 0072 2500 0000 7227 0000 0072 1600 0000  .r%...r'...r....
-00000710: 7216 0000 0072 1700 0000 7209 0000 003b  r....r....r....;
-00000720: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-00000730: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000740: 0000 0073 0a00 0000 7c00 a000 6401 a101  ...s....|...d...
-00000750: 5300 a902 4e72 0a00 0000 7222 0000 0072  S...Nr....r"...r
-00000760: 1800 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-00000770: 0000 0072 0a00 0000 4000 0000 7302 0000  ...r....@...s...
-00000780: 0000 027a 0941 7263 2e77 6964 7468 6302  ...z.Arc.widthc.
-00000790: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000007a0: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-000007b0: 6401 7c01 a102 0100 6400 5300 7229 0000  d.|.....d.S.r)..
-000007c0: 0072 2500 0000 7227 0000 0072 1600 0000  .r%...r'...r....
-000007d0: 7216 0000 0072 1700 0000 720a 0000 0044  r....r....r....D
-000007e0: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-000007f0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000800: 0000 0073 0a00 0000 7c00 a000 6401 a101  ...s....|...d...
-00000810: 5300 a902 4e72 0b00 0000 7222 0000 0072  S...Nr....r"...r
-00000820: 1800 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-00000830: 0000 0072 0b00 0000 4900 0000 7302 0000  ...r....I...s...
-00000840: 0000 027a 0a41 7263 2e68 6569 6768 7463  ...z.Arc.heightc
-00000850: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000860: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
-00000870: 0064 017c 01a1 0201 0064 0053 0072 2a00  .d.|.....d.S.r*.
-00000880: 0000 7225 0000 0072 2700 0000 7216 0000  ..r%...r'...r...
-00000890: 0072 1600 0000 7217 0000 0072 0b00 0000  .r....r....r....
-000008a0: 4d00 0000 7302 0000 0000 0263 0100 0000  M...s......c....
-000008b0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000008c0: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
-000008d0: 0153 00a9 024e 5a0a 7374 6172 7441 6e67  .S...NZ.startAng
-000008e0: 6c65 7222 0000 0072 1800 0000 7216 0000  ler"...r....r...
-000008f0: 0072 1600 0000 7217 0000 0072 0c00 0000  .r....r....r....
-00000900: 5200 0000 7302 0000 0000 027a 0f41 7263  R...s......z.Arc
-00000910: 2e73 7461 7274 5f61 6e67 6c65 6302 0000  .start_anglec...
-00000920: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000930: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-00000940: 7c01 a102 0100 6400 5300 722b 0000 0072  |.....d.S.r+...r
-00000950: 2500 0000 7227 0000 0072 1600 0000 7216  %...r'...r....r.
-00000960: 0000 0072 1700 0000 720c 0000 0056 0000  ...r....r....V..
-00000970: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000980: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000990: 0073 0a00 0000 7c00 a000 6401 a101 5300  .s....|...d...S.
-000009a0: a902 4e5a 0a73 7765 6570 416e 676c 6572  ..NZ.sweepAngler
-000009b0: 2200 0000 7218 0000 0072 1600 0000 7216  "...r....r....r.
-000009c0: 0000 0072 1700 0000 720d 0000 005b 0000  ...r....r....[..
-000009d0: 0073 0200 0000 0002 7a0f 4172 632e 7377  .s......z.Arc.sw
-000009e0: 6565 705f 616e 676c 6563 0200 0000 0000  eep_anglec......
-000009f0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000a00: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-00000a10: 0201 0064 0053 0072 2c00 0000 7225 0000  ...d.S.r,...r%..
-00000a20: 0072 2700 0000 7216 0000 0072 1600 0000  .r'...r....r....
-00000a30: 7217 0000 0072 0d00 0000 5f00 0000 7302  r....r...._...s.
-00000a40: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00000a50: 0000 0100 0000 0500 0000 4300 0000 7310  ..........C...s.
-00000a60: 0000 007c 006a 0064 0164 0264 0364 048d  ...|.j.d.d.d.d..
-00000a70: 0353 0029 054e da09 7573 6543 656e 7465  .S.).N..useCente
-00000a80: 72da 0462 6f6f 6c46 2902 da09 6461 7461  r..boolF)...data
-00000a90: 5f74 7970 65da 0964 6566 5f76 616c 7565  _type..def_value
-00000aa0: 7222 0000 0072 1800 0000 7216 0000 0072  r"...r....r....r
-00000ab0: 1600 0000 7217 0000 0072 0e00 0000 6400  ....r....r....d.
-00000ac0: 0000 7302 0000 0000 027a 0e41 7263 2e75  ..s......z.Arc.u
-00000ad0: 7365 5f63 656e 7465 7263 0200 0000 0000  se_centerc......
-00000ae0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000af0: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-00000b00: 0201 0064 0053 0029 024e 722d 0000 0072  ...d.S.).Nr-...r
-00000b10: 2500 0000 7227 0000 0072 1600 0000 7216  %...r'...r....r.
-00000b20: 0000 0072 1700 0000 720e 0000 0068 0000  ...r....r....h..
-00000b30: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000b40: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000b50: 0073 0600 0000 7c00 6a00 5300 a901 4ea9  .s....|.j.S...N.
-00000b60: 0172 1d00 0000 7218 0000 0072 1600 0000  .r....r....r....
-00000b70: 7216 0000 0072 1700 0000 720f 0000 006d  r....r....r....m
-00000b80: 0000 0073 0200 0000 0002 7a09 4172 632e  ...s......z.Arc.
-00000b90: 7061 696e 7463 0200 0000 0000 0000 0000  paintc..........
-00000ba0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-00000bb0: 0000 007c 017c 005f 0064 0053 0072 3100  ...|.|._.d.S.r1.
-00000bc0: 0000 7232 0000 0072 2700 0000 7216 0000  ..r2...r'...r...
-00000bd0: 0072 1600 0000 7217 0000 0072 0f00 0000  .r....r....r....
-00000be0: 7100 0000 7302 0000 0000 0229 0c4e 4e4e  q...s......).NNN
-00000bf0: 4e4e 4e4e 4e4e 4e4e 4e29 16da 085f 5f6e  NNNNNNNNN)...__n
-00000c00: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000c10: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000c20: 0500 0000 7203 0000 0072 2e00 0000 7206  ....r....r....r.
-00000c30: 0000 0072 0200 0000 7214 0000 0072 1900  ...r....r....r..
-00000c40: 0000 721b 0000 00da 0870 726f 7065 7274  ..r......propert
-00000c50: 7972 0800 0000 da06 7365 7474 6572 7209  yr......setterr.
-00000c60: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000c70: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00000c80: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000c90: 7216 0000 0072 1600 0000 721e 0000 0072  r....r....r....r
-00000ca0: 1700 0000 7207 0000 0008 0000 0073 7600  ....r........sv.
-00000cb0: 0000 0803 0001 0001 0001 0001 0001 0001  ................
-00000cc0: 0001 0004 0001 0001 0001 00f0 0202 0201  ................
-00000cd0: 0201 0201 0201 0201 0201 0601 0605 0601  ................
-00000ce0: 0601 02f0 0c1d 0803 0c05 0201 1003 0401  ................
-00000cf0: 1004 0201 1003 0401 1004 0201 1003 0401  ................
-00000d00: 1004 0201 1003 0401 1004 0201 1003 0401  ................
-00000d10: 1004 0201 1003 0401 1004 0201 1403 0401  ................
-00000d20: 1404 0201 1403 0401 7207 0000 004e 290a  ........r....N).
-00000d30: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000d40: 0000 5a16 666c 6574 5f63 6f72 652e 6361  ..Z.flet_core.ca
-00000d50: 6e76 6173 2e73 6861 7065 7204 0000 00da  nvas.shaper.....
-00000d60: 1166 6c65 745f 636f 7265 2e63 6f6e 7472  .flet_core.contr
-00000d70: 6f6c 7205 0000 00da 1266 6c65 745f 636f  olr......flet_co
-00000d80: 7265 2e70 6169 6e74 696e 6772 0600 0000  re.paintingr....
-00000d90: 7207 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000da0: 1600 0000 7217 0000 00da 083c 6d6f 6475  ....r......<modu
-00000db0: 6c65 3e01 0000 0073 0800 0000 1002 0c01  le>....s........
-00000dc0: 0c01 0c03                                ....
+000003d0: fa5d 2f77 6f72 6b73 7061 6365 732f 636f  .]/workspaces/co
+000003e0: 6e74 7269 6266 6c65 742f 666c 6574 636f  ntribflet/fletco
+000003f0: 6e74 7269 622f 7364 6b2f 7079 7468 6f6e  ntrib/sdk/python
+00000400: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
+00000410: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
+00000420: 652f 6361 6e76 6173 2f61 7263 2e70 7972  e/canvas/arc.pyr
+00000430: 1400 0000 0900 0000 7312 0000 0000 1214  ........s.......
+00000440: 0206 0106 0106 0106 0106 0106 0106 017a  ...............z
+00000450: 0c41 7263 2e5f 5f69 6e69 745f 5f63 0100  .Arc.__init__c..
+00000460: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000470: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
+00000480: 024e 5a03 6172 6372 1600 0000 a901 7215  .NZ.arcr......r.
+00000490: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000004a0: 0000 da11 5f67 6574 5f63 6f6e 7472 6f6c  ...._get_control
+000004b0: 5f6e 616d 6526 0000 0073 0200 0000 0001  _name&...s......
+000004c0: 7a15 4172 632e 5f67 6574 5f63 6f6e 7472  z.Arc._get_contr
+000004d0: 6f6c 5f6e 616d 6563 0100 0000 0000 0000  ol_namec........
+000004e0: 0000 0000 0100 0000 0400 0000 0300 0000  ................
+000004f0: 731c 0000 0074 0083 00a0 01a1 0001 007c  s....t.........|
+00000500: 00a0 0264 017c 006a 03a1 0201 0064 0053  ...d.|.j.....d.S
+00000510: 0029 024e 720f 0000 0029 04da 0573 7570  .).Nr....)...sup
+00000520: 6572 da0d 6265 666f 7265 5f75 7064 6174  er..before_updat
+00000530: 65da 0e5f 7365 745f 6174 7472 5f6a 736f  e.._set_attr_jso
+00000540: 6eda 0b5f 4172 635f 5f70 6169 6e74 7218  n.._Arc__paintr.
+00000550: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+00000560: 7216 0000 0072 1700 0000 721b 0000 0029  r....r....r....)
+00000570: 0000 0073 0400 0000 0001 0a01 7a11 4172  ...s........z.Ar
+00000580: 632e 6265 666f 7265 5f75 7064 6174 6529  c.before_update)
+00000590: 01da 0672 6574 7572 6e63 0100 0000 0000  ...returnc......
+000005a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000005b0: 0000 730a 0000 007c 00a0 0064 01a1 0153  ..s....|...d...S
+000005c0: 00a9 024e 7208 0000 00a9 01da 095f 6765  ...Nr........_ge
+000005d0: 745f 6174 7472 7218 0000 0072 1600 0000  t_attrr....r....
+000005e0: 7216 0000 0072 1700 0000 7208 0000 002e  r....r....r.....
+000005f0: 0000 0073 0200 0000 0002 7a05 4172 632e  ...s......z.Arc.
+00000600: 7829 01da 0576 616c 7565 6302 0000 0000  x)...valuec.....
+00000610: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000620: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
+00000630: a102 0100 6400 5300 7221 0000 00a9 01da  ....d.S.r!......
+00000640: 095f 7365 745f 6174 7472 a902 7215 0000  ._set_attr..r...
+00000650: 0072 2400 0000 7216 0000 0072 1600 0000  .r$...r....r....
+00000660: 7217 0000 0072 0800 0000 3200 0000 7302  r....r....2...s.
+00000670: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00000680: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
+00000690: 0000 007c 00a0 0064 01a1 0153 00a9 024e  ...|...d...S...N
+000006a0: 7209 0000 0072 2200 0000 7218 0000 0072  r....r"...r....r
+000006b0: 1600 0000 7216 0000 0072 1700 0000 7209  ....r....r....r.
+000006c0: 0000 0037 0000 0073 0200 0000 0002 7a05  ...7...s......z.
+000006d0: 4172 632e 7963 0200 0000 0000 0000 0000  Arc.yc..........
+000006e0: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+000006f0: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+00000700: 0053 0072 2800 0000 7225 0000 0072 2700  .S.r(...r%...r'.
+00000710: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000720: 0072 0900 0000 3b00 0000 7302 0000 0000  .r....;...s.....
+00000730: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000740: 0000 0300 0000 4300 0000 730a 0000 007c  ......C...s....|
+00000750: 00a0 0064 01a1 0153 00a9 024e 720a 0000  ...d...S...Nr...
+00000760: 0072 2200 0000 7218 0000 0072 1600 0000  .r"...r....r....
+00000770: 7216 0000 0072 1700 0000 720a 0000 0040  r....r....r....@
+00000780: 0000 0073 0200 0000 0002 7a09 4172 632e  ...s......z.Arc.
+00000790: 7769 6474 6863 0200 0000 0000 0000 0000  widthc..........
+000007a0: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+000007b0: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+000007c0: 0053 0072 2900 0000 7225 0000 0072 2700  .S.r)...r%...r'.
+000007d0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+000007e0: 0072 0a00 0000 4400 0000 7302 0000 0000  .r....D...s.....
+000007f0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000800: 0000 0300 0000 4300 0000 730a 0000 007c  ......C...s....|
+00000810: 00a0 0064 01a1 0153 00a9 024e 720b 0000  ...d...S...Nr...
+00000820: 0072 2200 0000 7218 0000 0072 1600 0000  .r"...r....r....
+00000830: 7216 0000 0072 1700 0000 720b 0000 0049  r....r....r....I
+00000840: 0000 0073 0200 0000 0002 7a0a 4172 632e  ...s......z.Arc.
+00000850: 6865 6967 6874 6302 0000 0000 0000 0000  heightc.........
+00000860: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000870: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
+00000880: 6400 5300 722a 0000 0072 2500 0000 7227  d.S.r*...r%...r'
+00000890: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000008a0: 0000 720b 0000 004d 0000 0073 0200 0000  ..r....M...s....
+000008b0: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
+000008c0: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
+000008d0: 7c00 a000 6401 a101 5300 a902 4e5a 0a73  |...d...S...NZ.s
+000008e0: 7461 7274 416e 676c 6572 2200 0000 7218  tartAngler"...r.
+000008f0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000900: 0000 720c 0000 0052 0000 0073 0200 0000  ..r....R...s....
+00000910: 0002 7a0f 4172 632e 7374 6172 745f 616e  ..z.Arc.start_an
+00000920: 676c 6563 0200 0000 0000 0000 0000 0000  glec............
+00000930: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+00000940: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+00000950: 0072 2b00 0000 7225 0000 0072 2700 0000  .r+...r%...r'...
+00000960: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000970: 0c00 0000 5600 0000 7302 0000 0000 0263  ....V...s......c
+00000980: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000990: 0300 0000 4300 0000 730a 0000 007c 00a0  ....C...s....|..
+000009a0: 0064 01a1 0153 00a9 024e 5a0a 7377 6565  .d...S...NZ.swee
+000009b0: 7041 6e67 6c65 7222 0000 0072 1800 0000  pAngler"...r....
+000009c0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+000009d0: 0d00 0000 5b00 0000 7302 0000 0000 027a  ....[...s......z
+000009e0: 0f41 7263 2e73 7765 6570 5f61 6e67 6c65  .Arc.sweep_angle
+000009f0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000a00: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00000a10: a000 6401 7c01 a102 0100 6400 5300 722c  ..d.|.....d.S.r,
+00000a20: 0000 0072 2500 0000 7227 0000 0072 1600  ...r%...r'...r..
+00000a30: 0000 7216 0000 0072 1700 0000 720d 0000  ..r....r....r...
+00000a40: 005f 0000 0073 0200 0000 0002 6301 0000  ._...s......c...
+00000a50: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00000a60: 0043 0000 0073 1000 0000 7c00 6a00 6401  .C...s....|.j.d.
+00000a70: 6402 6403 6404 8d03 5300 2905 4eda 0975  d.d.d...S.).N..u
+00000a80: 7365 4365 6e74 6572 da04 626f 6f6c 4629  seCenter..boolF)
+00000a90: 02da 0964 6174 615f 7479 7065 da09 6465  ...data_type..de
+00000aa0: 665f 7661 6c75 6572 2200 0000 7218 0000  f_valuer"...r...
+00000ab0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000ac0: 720e 0000 0064 0000 0073 0200 0000 0002  r....d...s......
+00000ad0: 7a0e 4172 632e 7573 655f 6365 6e74 6572  z.Arc.use_center
+00000ae0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000af0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00000b00: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
+00000b10: 4e72 2d00 0000 7225 0000 0072 2700 0000  Nr-...r%...r'...
+00000b20: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000b30: 0e00 0000 6800 0000 7302 0000 0000 0263  ....h...s......c
+00000b40: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000b50: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+00000b60: 0053 00a9 014e a901 721d 0000 0072 1800  .S...N..r....r..
+00000b70: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000b80: 0072 0f00 0000 6d00 0000 7302 0000 0000  .r....m...s.....
+00000b90: 027a 0941 7263 2e70 6169 6e74 6302 0000  .z.Arc.paintc...
+00000ba0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000bb0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000bc0: 6400 5300 7231 0000 0072 3200 0000 7227  d.S.r1...r2...r'
+00000bd0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000be0: 0000 720f 0000 0071 0000 0073 0200 0000  ..r....q...s....
+00000bf0: 0002 290c 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  ..).NNNNNNNNNNNN
+00000c00: 2916 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000c10: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000c20: 6e61 6d65 5f5f 7205 0000 0072 0300 0000  name__r....r....
+00000c30: 722e 0000 0072 0600 0000 7202 0000 0072  r....r....r....r
+00000c40: 1400 0000 7219 0000 0072 1b00 0000 da08  ....r....r......
+00000c50: 7072 6f70 6572 7479 7208 0000 00da 0673  propertyr......s
+00000c60: 6574 7465 7272 0900 0000 720a 0000 0072  etterr....r....r
+00000c70: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
+00000c80: 0000 0072 0f00 0000 da0d 5f5f 636c 6173  ...r......__clas
+00000c90: 7363 656c 6c5f 5f72 1600 0000 7216 0000  scell__r....r...
+00000ca0: 0072 1e00 0000 7217 0000 0072 0700 0000  .r....r....r....
+00000cb0: 0800 0000 7376 0000 0008 0300 0100 0100  ....sv..........
+00000cc0: 0100 0100 0100 0100 0100 0400 0100 0100  ................
+00000cd0: 0100 f002 0202 0102 0102 0102 0102 0102  ................
+00000ce0: 0106 0106 0506 0106 0102 f00c 1d08 030c  ................
+00000cf0: 0502 0110 0304 0110 0402 0110 0304 0110  ................
+00000d00: 0402 0110 0304 0110 0402 0110 0304 0110  ................
+00000d10: 0402 0110 0304 0110 0402 0110 0304 0110  ................
+00000d20: 0402 0114 0304 0114 0402 0114 0304 0172  ...............r
+00000d30: 0700 0000 4e29 0ada 0674 7970 696e 6772  ....N)...typingr
+00000d40: 0200 0000 7203 0000 005a 1666 6c65 745f  ....r....Z.flet_
+00000d50: 636f 7265 2e63 616e 7661 732e 7368 6170  core.canvas.shap
+00000d60: 6572 0400 0000 da11 666c 6574 5f63 6f72  er......flet_cor
+00000d70: 652e 636f 6e74 726f 6c72 0500 0000 da12  e.controlr......
+00000d80: 666c 6574 5f63 6f72 652e 7061 696e 7469  flet_core.painti
+00000d90: 6e67 7206 0000 0072 0700 0000 7216 0000  ngr....r....r...
+00000da0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000db0: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
+00000dc0: 0000 0010 020c 010c 010c 03              ...........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 4813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 cd12 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 cd12 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -89,212 +89,213 @@
 00000580: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00000590: 0400 0000 5300 0000 731a 0000 0074 00a0  ....S...s....t..
 000005a0: 017c 006a 02a1 017d 0174 0366 0069 007c  .|.j...}.t.f.i.|
 000005b0: 01a4 018e 0153 00a9 014e 2904 da04 6a73  .....S...N)...js
 000005c0: 6f6e da05 6c6f 6164 7372 2e00 0000 da11  on..loadsr......
 000005d0: 4361 6e76 6173 5265 7369 7a65 4576 656e  CanvasResizeEven
 000005e0: 7429 02da 0165 da01 64a9 0072 3600 0000  t)...e..d..r6...
-000005f0: fa59 2f77 6f72 6b73 7061 6365 732f 636f  .Y/workspaces/co
-00000600: 6e74 7269 6266 6c65 742f 666c 6574 2f73  ntribflet/flet/s
-00000610: 646b 2f70 7974 686f 6e2f 7061 636b 6167  dk/python/packag
-00000620: 6573 2f66 6c65 742d 636f 7265 2f73 7263  es/flet-core/src
-00000630: 2f66 6c65 745f 636f 7265 2f63 616e 7661  /flet_core/canva
-00000640: 732f 6361 6e76 6173 2e70 79da 2663 6f6e  s/canvas.py.&con
-00000650: 7665 7274 5f63 7573 746f 6d5f 7061 696e  vert_custom_pain
-00000660: 745f 7265 7369 7a65 5f65 7665 6e74 5f64  t_resize_event_d
-00000670: 6174 6155 0000 0073 0400 0000 0001 0c01  ataU...s........
-00000680: 7a3f 4361 6e76 6173 2e5f 5f69 6e69 745f  z?Canvas.__init_
-00000690: 5f2e 3c6c 6f63 616c 733e 2e63 6f6e 7665  _.<locals>.conve
-000006a0: 7274 5f63 7573 746f 6d5f 7061 696e 745f  rt_custom_paint_
-000006b0: 7265 7369 7a65 5f65 7665 6e74 5f64 6174  resize_event_dat
-000006c0: 615a 0672 6573 697a 6529 0a72 0700 0000  aZ.resize).r....
-000006d0: da08 5f5f 696e 6974 5f5f 720b 0000 00da  ..__init__r.....
-000006e0: 125f 4361 6e76 6173 5f5f 6f6e 5f72 6573  ._Canvas__on_res
-000006f0: 697a 65da 125f 6164 645f 6576 656e 745f  ize.._add_event_
-00000700: 6861 6e64 6c65 725a 0b67 6574 5f68 616e  handlerZ.get_han
-00000710: 646c 6572 7214 0000 0072 1500 0000 7216  dlerr....r....r.
-00000720: 0000 00da 096f 6e5f 7265 7369 7a65 291f  .....on_resize).
-00000730: da04 7365 6c66 7214 0000 0072 1500 0000  ..selfr....r....
-00000740: 7216 0000 0072 3c00 0000 7217 0000 0072  r....r<...r....r
-00000750: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00000760: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
-00000770: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00000780: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00000790: 7225 0000 0072 2600 0000 7227 0000 0072  r%...r&...r'...r
-000007a0: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
-000007b0: 0000 0072 2f00 0000 722c 0000 0072 2d00  ...r/...r,...r-.
-000007c0: 0000 722e 0000 0072 3800 0000 7236 0000  ..r....r8...r6..
-000007d0: 0072 3600 0000 7237 0000 0072 3900 0000  .r6...r7...r9...
-000007e0: 1500 0000 7346 0000 0000 2304 0102 0102  ....sF....#.....
-000007f0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000800: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000810: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000820: e606 1d08 040a 0112 0206 0106 0106 017a  ...............z
-00000830: 0f43 616e 7661 732e 5f5f 696e 6974 5f5f  .Canvas.__init__
-00000840: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000850: 0001 0000 0043 0000 0073 0400 0000 6401  .....C...s....d.
-00000860: 5300 2902 4eda 0663 616e 7661 7372 3600  S.).N..canvasr6.
-00000870: 0000 a901 723d 0000 0072 3600 0000 7236  ....r=...r6...r6
-00000880: 0000 0072 3700 0000 da11 5f67 6574 5f63  ...r7....._get_c
-00000890: 6f6e 7472 6f6c 5f6e 616d 6561 0000 0073  ontrol_namea...s
-000008a0: 0200 0000 0001 7a18 4361 6e76 6173 2e5f  ......z.Canvas._
-000008b0: 6765 745f 636f 6e74 726f 6c5f 6e61 6d65  get_control_name
-000008c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000008d0: 0004 0000 0043 0000 0073 3800 0000 6700  .....C...s8...g.
-000008e0: 7d01 7c01 a000 7c00 6a01 a101 0100 7c00  }.|...|.j.....|.
-000008f0: 6a02 6400 7501 7234 7c00 6a02 a003 6401  j.d.u.r4|.j...d.
-00000900: 6402 a102 0100 7c01 a004 7c00 6a02 a101  d.....|...|.j...
-00000910: 0100 7c01 5300 2903 4eda 016e 7215 0000  ..|.S.).N..nr...
-00000920: 0029 05da 0665 7874 656e 64da 0f5f 4361  .)...extend.._Ca
-00000930: 6e76 6173 5f5f 7368 6170 6573 da10 5f43  nvas__shapes.._C
-00000940: 616e 7661 735f 5f63 6f6e 7465 6e74 da12  anvas__content..
-00000950: 5f73 6574 5f61 7474 725f 696e 7465 726e  _set_attr_intern
-00000960: 616c da06 6170 7065 6e64 2902 723d 0000  al..append).r=..
-00000970: 00da 0863 6869 6c64 7265 6e72 3600 0000  ...childrenr6...
-00000980: 7236 0000 0072 3700 0000 da0d 5f67 6574  r6...r7....._get
-00000990: 5f63 6869 6c64 7265 6e64 0000 0073 0c00  _childrend...s..
-000009a0: 0000 0001 0401 0c01 0a01 0e01 0c01 7a14  ..............z.
-000009b0: 4361 6e76 6173 2e5f 6765 745f 6368 696c  Canvas._get_chil
-000009c0: 6472 656e 6301 0000 0000 0000 0000 0000  drenc...........
-000009d0: 0001 0000 0002 0000 0003 0000 0073 1800  .............s..
-000009e0: 0000 7400 8300 a001 a100 0100 7c00 6a02  ..t.........|.j.
-000009f0: a003 a100 0100 6400 5300 7230 0000 0029  ......d.S.r0...)
-00000a00: 04da 0573 7570 6572 da05 636c 6561 6e72  ...super..cleanr
-00000a10: 4300 0000 da05 636c 6561 7272 3f00 0000  C.....clearr?...
-00000a20: a901 da09 5f5f 636c 6173 735f 5f72 3600  ....__class__r6.
-00000a30: 0000 7237 0000 0072 4a00 0000 6c00 0000  ..r7...rJ...l...
-00000a40: 7304 0000 0000 010a 017a 0c43 616e 7661  s........z.Canva
-00000a50: 732e 636c 6561 6e7a 1b55 7365 2063 6c65  s.cleanz.Use cle
-00000a60: 616e 2829 206d 6574 686f 6420 696e 7374  an() method inst
-00000a70: 6561 642e 7a06 302e 3231 2e30 7a03 312e  ead.z.0.21.0z.1.
-00000a80: 3029 03da 0672 6561 736f 6eda 0776 6572  0)...reason..ver
-00000a90: 7369 6f6e da0e 6465 6c65 7465 5f76 6572  sion..delete_ver
-00000aa0: 7369 6f6e 6301 0000 0000 0000 0000 0000  sionc...........
-00000ab0: 0001 0000 0002 0000 00c3 0000 0073 0c00  .............s..
-00000ac0: 0000 7c00 a000 a100 0100 6400 5300 7230  ..|.......d.S.r0
-00000ad0: 0000 0029 0172 4a00 0000 723f 0000 0072  ...).rJ...r?...r
-00000ae0: 3600 0000 7236 0000 0072 3700 0000 da0b  6...r6...r7.....
-00000af0: 636c 6561 6e5f 6173 796e 6370 0000 0073  clean_asyncp...s
-00000b00: 0200 0000 0004 7a12 4361 6e76 6173 2e63  ......z.Canvas.c
-00000b10: 6c65 616e 5f61 7379 6e63 a901 da06 7265  lean_async....re
-00000b20: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
-00000b30: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000b40: 0000 7c00 6a00 5300 7230 0000 00a9 0172  ..|.j.S.r0.....r
-00000b50: 4300 0000 723f 0000 0072 3600 0000 7236  C...r?...r6...r6
-00000b60: 0000 0072 3700 0000 7214 0000 0077 0000  ...r7...r....w..
-00000b70: 0073 0200 0000 0002 7a0d 4361 6e76 6173  .s......z.Canvas
-00000b80: 2e73 6861 7065 7329 01da 0576 616c 7565  .shapes)...value
-00000b90: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000ba0: 0002 0000 0043 0000 0073 1600 0000 7c01  .....C...s....|.
-00000bb0: 6400 7501 720c 7c01 6e02 6700 7c00 5f00  d.u.r.|.n.g.|._.
-00000bc0: 6400 5300 7230 0000 0072 5400 0000 a902  d.S.r0...rT.....
-00000bd0: 723d 0000 0072 5500 0000 7236 0000 0072  r=...rU...r6...r
-00000be0: 3600 0000 7237 0000 0072 1400 0000 7b00  6...r7...r....{.
-00000bf0: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
-00000c00: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00000c10: 0000 7306 0000 007c 006a 0053 0072 3000  ..s....|.j.S.r0.
-00000c20: 0000 a901 7244 0000 0072 3f00 0000 7236  ....rD...r?...r6
-00000c30: 0000 0072 3600 0000 7237 0000 0072 1500  ...r6...r7...r..
-00000c40: 0000 8000 0000 7302 0000 0000 027a 0e43  ......s......z.C
-00000c50: 616e 7661 732e 636f 6e74 656e 7463 0200  anvas.contentc..
-00000c60: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000c70: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-00000c80: 0064 0053 0072 3000 0000 7257 0000 0072  .d.S.r0...rW...r
-00000c90: 5600 0000 7236 0000 0072 3600 0000 7237  V...r6...r6...r7
-00000ca0: 0000 0072 1500 0000 8400 0000 7302 0000  ...r........s...
-00000cb0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-00000cc0: 0100 0000 0300 0000 4300 0000 730a 0000  ........C...s...
-00000cd0: 007c 00a0 0064 01a1 0153 00a9 024e 5a0e  .|...d...S...NZ.
-00000ce0: 7265 7369 7a65 496e 7465 7276 616c 2901  resizeInterval).
-00000cf0: da09 5f67 6574 5f61 7474 7272 3f00 0000  .._get_attrr?...
-00000d00: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00000d10: 1600 0000 8900 0000 7302 0000 0000 027a  ........s......z
-00000d20: 1643 616e 7661 732e 7265 7369 7a65 5f69  .Canvas.resize_i
-00000d30: 6e74 6572 7661 6c63 0200 0000 0000 0000  ntervalc........
-00000d40: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000d50: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00000d60: 0064 0053 0072 5800 0000 2901 da09 5f73  .d.S.rX...)..._s
-00000d70: 6574 5f61 7474 7272 5600 0000 7236 0000  et_attrrV...r6..
-00000d80: 0072 3600 0000 7237 0000 0072 1600 0000  .r6...r7...r....
-00000d90: 8d00 0000 7302 0000 0000 0263 0100 0000  ....s......c....
-00000da0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000db0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
-00000dc0: 3000 0000 2901 723a 0000 0072 3f00 0000  0...).r:...r?...
-00000dd0: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00000de0: 3c00 0000 9200 0000 7302 0000 0000 027a  <.......s......z
-00000df0: 1043 616e 7661 732e 6f6e 5f72 6573 697a  .Canvas.on_resiz
-00000e00: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00000e10: 0000 0400 0000 4300 0000 7332 0000 007c  ......C...s2...|
-00000e20: 006a 00a0 017c 01a1 0101 007c 0164 0075  .j...|.....|.d.u
-00000e30: 0172 227c 00a0 0264 0164 02a1 0201 006e  .r"|...d.d.....n
-00000e40: 0c7c 00a0 0264 0164 00a1 0201 0064 0053  .|...d.d.....d.S
-00000e50: 0029 034e 5a08 6f6e 7265 7369 7a65 5429  .).NZ.onresizeT)
-00000e60: 0372 3a00 0000 5a09 7375 6273 6372 6962  .r:...Z.subscrib
-00000e70: 6572 5a00 0000 2902 723d 0000 00da 0768  erZ...).r=.....h
-00000e80: 616e 646c 6572 7236 0000 0072 3600 0000  andlerr6...r6...
-00000e90: 7237 0000 0072 3c00 0000 9600 0000 7308  r7...r<.......s.
-00000ea0: 0000 0000 020c 0108 010e 0229 1d4e 4e4e  ...........).NNN
-00000eb0: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
-00000ec0: 4e4e 4e4e 4e4e 4e4e 4e4e 291f da08 5f5f  NNNNNNNNNN)...__
-00000ed0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000ee0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000ef0: 7204 0000 0072 0300 0000 7206 0000 0072  r....r....r....r
-00000f00: 0800 0000 7209 0000 0072 0c00 0000 7205  ....r....r....r.
-00000f10: 0000 00da 0462 6f6f 6cda 0369 6e74 720f  .....bool..intr.
-00000f20: 0000 0072 1000 0000 7211 0000 0072 0e00  ...r....r....r..
-00000f30: 0000 720d 0000 0072 0200 0000 7239 0000  ..r....r....r9..
-00000f40: 0072 4000 0000 7248 0000 0072 4a00 0000  .r@...rH...rJ...
-00000f50: 7212 0000 0072 5100 0000 da08 7072 6f70  r....rQ.....prop
-00000f60: 6572 7479 7214 0000 00da 0673 6574 7465  ertyr......sette
-00000f70: 7272 1500 0000 7216 0000 0072 3c00 0000  rr....r....r<...
-00000f80: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00000f90: 3600 0000 7236 0000 0072 4c00 0000 7237  6...r6...rL...r7
-00000fa0: 0000 0072 1300 0000 1400 0000 73a2 0000  ...r........s...
-00000fb0: 0008 0300 0100 0100 0100 0400 0100 0100  ................
-00000fc0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-00000fd0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-00000fe0: 0100 0100 0100 0100 0100 0100 df02 020a  ................
-00000ff0: 0106 0102 0506 0102 0102 0102 0102 0102  ................
-00001000: 0102 010c 0106 0106 0102 0102 0102 0102  ................
-00001010: 0102 0102 0102 0102 0102 0102 0102 0206  ................
-00001020: 0106 0102 df0c 4c08 0308 080c 0402 0106  ......L.........
-00001030: ff04 030a 0402 0114 0304 0118 0402 0114  ................
-00001040: 0304 0114 0402 0110 0304 0110 0402 010a  ................
-00001050: 0304 0172 1300 0000 6300 0000 0000 0000  ...r....c.......
-00001060: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00001070: 0073 1a00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00001080: 6402 9c01 6403 6404 8404 5a03 6401 5300  d...d.d...Z.d.S.
-00001090: 2905 7233 0000 004e 7252 0000 0063 0300  ).r3...NrR...c..
-000010a0: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-000010b0: 0000 4300 0000 7310 0000 007c 017c 005f  ..C...s....|.|._
-000010c0: 007c 027c 005f 0164 0053 0072 3000 0000  .|.|._.d.S.r0...
-000010d0: 2902 7218 0000 0072 1900 0000 2903 723d  ).r....r....).r=
-000010e0: 0000 00da 0177 da01 6872 3600 0000 7236  .....w..hr6...r6
-000010f0: 0000 0072 3700 0000 7239 0000 00a0 0000  ...r7...r9......
-00001100: 0073 0400 0000 0001 0601 7a1a 4361 6e76  .s........z.Canv
-00001110: 6173 5265 7369 7a65 4576 656e 742e 5f5f  asResizeEvent.__
-00001120: 696e 6974 5f5f 2904 725c 0000 0072 5d00  init__).r\...r].
-00001130: 0000 725e 0000 0072 3900 0000 7236 0000  ..r^...r9...r6..
-00001140: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-00001150: 7233 0000 009f 0000 0073 0200 0000 0801  r3.......s......
-00001160: 7233 0000 0029 1d72 3100 0000 da06 7479  r3...).r1.....ty
-00001170: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
-00001180: 0000 0072 0500 0000 da16 666c 6574 5f63  ...r......flet_c
-00001190: 6f72 652e 6361 6e76 6173 2e73 6861 7065  ore.canvas.shape
-000011a0: 7206 0000 005a 1d66 6c65 745f 636f 7265  r....Z.flet_core
-000011b0: 2e63 6f6e 7374 7261 696e 6564 5f63 6f6e  .constrained_con
-000011c0: 7472 6f6c 7207 0000 00da 1166 6c65 745f  trolr......flet_
-000011d0: 636f 7265 2e63 6f6e 7472 6f6c 7208 0000  core.controlr...
-000011e0: 0072 0900 0000 da17 666c 6574 5f63 6f72  .r......flet_cor
-000011f0: 652e 636f 6e74 726f 6c5f 6576 656e 7472  e.control_eventr
-00001200: 0a00 0000 5a17 666c 6574 5f63 6f72 652e  ....Z.flet_core.
-00001210: 6576 656e 745f 6861 6e64 6c65 7272 0b00  event_handlerr..
-00001220: 0000 da0d 666c 6574 5f63 6f72 652e 7265  ....flet_core.re
-00001230: 6672 0c00 0000 da0f 666c 6574 5f63 6f72  fr......flet_cor
-00001240: 652e 7479 7065 7372 0d00 0000 720e 0000  e.typesr....r...
-00001250: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00001260: da0f 666c 6574 5f63 6f72 652e 7574 696c  ..flet_core.util
-00001270: 7372 1200 0000 7213 0000 0072 3300 0000  sr....r....r3...
-00001280: 7236 0000 0072 3600 0000 7236 0000 0072  r6...r6...r6...r
-00001290: 3700 0000 da08 3c6d 6f64 756c 653e 0100  7.....<module>..
-000012a0: 0000 7318 0000 0008 0118 020c 010c 0110  ..s.............
-000012b0: 010c 010c 010c 011c 070c 0310 7f00 0c    ...............
+000005f0: fa60 2f77 6f72 6b73 7061 6365 732f 636f  .`/workspaces/co
+00000600: 6e74 7269 6266 6c65 742f 666c 6574 636f  ntribflet/fletco
+00000610: 6e74 7269 622f 7364 6b2f 7079 7468 6f6e  ntrib/sdk/python
+00000620: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
+00000630: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
+00000640: 652f 6361 6e76 6173 2f63 616e 7661 732e  e/canvas/canvas.
+00000650: 7079 da26 636f 6e76 6572 745f 6375 7374  py.&convert_cust
+00000660: 6f6d 5f70 6169 6e74 5f72 6573 697a 655f  om_paint_resize_
+00000670: 6576 656e 745f 6461 7461 5500 0000 7304  event_dataU...s.
+00000680: 0000 0000 010c 017a 3f43 616e 7661 732e  .......z?Canvas.
+00000690: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+000006a0: 3e2e 636f 6e76 6572 745f 6375 7374 6f6d  >.convert_custom
+000006b0: 5f70 6169 6e74 5f72 6573 697a 655f 6576  _paint_resize_ev
+000006c0: 656e 745f 6461 7461 5a06 7265 7369 7a65  ent_dataZ.resize
+000006d0: 290a 7207 0000 00da 085f 5f69 6e69 745f  ).r......__init_
+000006e0: 5f72 0b00 0000 da12 5f43 616e 7661 735f  _r......_Canvas_
+000006f0: 5f6f 6e5f 7265 7369 7a65 da12 5f61 6464  _on_resize.._add
+00000700: 5f65 7665 6e74 5f68 616e 646c 6572 5a0b  _event_handlerZ.
+00000710: 6765 745f 6861 6e64 6c65 7272 1400 0000  get_handlerr....
+00000720: 7215 0000 0072 1600 0000 da09 6f6e 5f72  r....r......on_r
+00000730: 6573 697a 6529 1fda 0473 656c 6672 1400  esize)...selfr..
+00000740: 0000 7215 0000 0072 1600 0000 723c 0000  ..r....r....r<..
+00000750: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000760: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000770: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+00000780: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+00000790: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+000007a0: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
+000007b0: 722a 0000 0072 2b00 0000 722f 0000 0072  r*...r+...r/...r
+000007c0: 2c00 0000 722d 0000 0072 2e00 0000 7238  ,...r-...r....r8
+000007d0: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+000007e0: 0000 7239 0000 0015 0000 0073 4600 0000  ..r9.......sF...
+000007f0: 0023 0401 0201 0201 0201 0201 0201 0201  .#..............
+00000800: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000810: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000820: 0201 0201 0201 02e6 061d 0804 0a01 1202  ................
+00000830: 0601 0601 0601 7a0f 4361 6e76 6173 2e5f  ......z.Canvas._
+00000840: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000850: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000860: 7304 0000 0064 0153 0029 024e da06 6361  s....d.S.).N..ca
+00000870: 6e76 6173 7236 0000 00a9 0172 3d00 0000  nvasr6.....r=...
+00000880: 7236 0000 0072 3600 0000 7237 0000 00da  r6...r6...r7....
+00000890: 115f 6765 745f 636f 6e74 726f 6c5f 6e61  ._get_control_na
+000008a0: 6d65 6100 0000 7302 0000 0000 017a 1843  mea...s......z.C
+000008b0: 616e 7661 732e 5f67 6574 5f63 6f6e 7472  anvas._get_contr
+000008c0: 6f6c 5f6e 616d 6563 0100 0000 0000 0000  ol_namec........
+000008d0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+000008e0: 7338 0000 0067 007d 017c 01a0 007c 006a  s8...g.}.|...|.j
+000008f0: 01a1 0101 007c 006a 0264 0075 0172 347c  .....|.j.d.u.r4|
+00000900: 006a 02a0 0364 0164 02a1 0201 007c 01a0  .j...d.d.....|..
+00000910: 047c 006a 02a1 0101 007c 0153 0029 034e  .|.j.....|.S.).N
+00000920: da01 6e72 1500 0000 2905 da06 6578 7465  ..nr....)...exte
+00000930: 6e64 da0f 5f43 616e 7661 735f 5f73 6861  nd.._Canvas__sha
+00000940: 7065 73da 105f 4361 6e76 6173 5f5f 636f  pes.._Canvas__co
+00000950: 6e74 656e 74da 125f 7365 745f 6174 7472  ntent.._set_attr
+00000960: 5f69 6e74 6572 6e61 6cda 0661 7070 656e  _internal..appen
+00000970: 6429 0272 3d00 0000 da08 6368 696c 6472  d).r=.....childr
+00000980: 656e 7236 0000 0072 3600 0000 7237 0000  enr6...r6...r7..
+00000990: 00da 0d5f 6765 745f 6368 696c 6472 656e  ..._get_children
+000009a0: 6400 0000 730c 0000 0000 0104 010c 010a  d...s...........
+000009b0: 010e 010c 017a 1443 616e 7661 732e 5f67  .....z.Canvas._g
+000009c0: 6574 5f63 6869 6c64 7265 6e63 0100 0000  et_childrenc....
+000009d0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000009e0: 0300 0000 7318 0000 0074 0083 00a0 01a1  ....s....t......
+000009f0: 0001 007c 006a 02a0 03a1 0001 0064 0053  ...|.j.......d.S
+00000a00: 0072 3000 0000 2904 da05 7375 7065 72da  .r0...)...super.
+00000a10: 0563 6c65 616e 7243 0000 00da 0563 6c65  .cleanrC.....cle
+00000a20: 6172 723f 0000 00a9 01da 095f 5f63 6c61  arr?.......__cla
+00000a30: 7373 5f5f 7236 0000 0072 3700 0000 724a  ss__r6...r7...rJ
+00000a40: 0000 006c 0000 0073 0400 0000 0001 0a01  ...l...s........
+00000a50: 7a0c 4361 6e76 6173 2e63 6c65 616e 7a1b  z.Canvas.cleanz.
+00000a60: 5573 6520 636c 6561 6e28 2920 6d65 7468  Use clean() meth
+00000a70: 6f64 2069 6e73 7465 6164 2e7a 0630 2e32  od instead.z.0.2
+00000a80: 312e 307a 0331 2e30 2903 da06 7265 6173  1.0z.1.0)...reas
+00000a90: 6f6e da07 7665 7273 696f 6eda 0e64 656c  on..version..del
+00000aa0: 6574 655f 7665 7273 696f 6e63 0100 0000  ete_versionc....
+00000ab0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000ac0: c300 0000 730c 0000 007c 00a0 00a1 0001  ....s....|......
+00000ad0: 0064 0053 0072 3000 0000 2901 724a 0000  .d.S.r0...).rJ..
+00000ae0: 0072 3f00 0000 7236 0000 0072 3600 0000  .r?...r6...r6...
+00000af0: 7237 0000 00da 0b63 6c65 616e 5f61 7379  r7.....clean_asy
+00000b00: 6e63 7000 0000 7302 0000 0000 047a 1243  ncp...s......z.C
+00000b10: 616e 7661 732e 636c 6561 6e5f 6173 796e  anvas.clean_asyn
+00000b20: 63a9 01da 0672 6574 7572 6e63 0100 0000  c....returnc....
+00000b30: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000b40: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
+00000b50: 3000 0000 a901 7243 0000 0072 3f00 0000  0.....rC...r?...
+00000b60: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
+00000b70: 1400 0000 7700 0000 7302 0000 0000 027a  ....w...s......z
+00000b80: 0d43 616e 7661 732e 7368 6170 6573 2901  .Canvas.shapes).
+00000b90: da05 7661 6c75 6563 0200 0000 0000 0000  ..valuec........
+00000ba0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000bb0: 7316 0000 007c 0164 0075 0172 0c7c 016e  s....|.d.u.r.|.n
+00000bc0: 0267 007c 005f 0064 0053 0072 3000 0000  .g.|._.d.S.r0...
+00000bd0: 7254 0000 00a9 0272 3d00 0000 7255 0000  rT.....r=...rU..
+00000be0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
+00000bf0: 7214 0000 007b 0000 0073 0200 0000 0002  r....{...s......
+00000c00: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000c10: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+00000c20: 6a00 5300 7230 0000 00a9 0172 4400 0000  j.S.r0.....rD...
+00000c30: 723f 0000 0072 3600 0000 7236 0000 0072  r?...r6...r6...r
+00000c40: 3700 0000 7215 0000 0080 0000 0073 0200  7...r........s..
+00000c50: 0000 0002 7a0e 4361 6e76 6173 2e63 6f6e  ....z.Canvas.con
+00000c60: 7465 6e74 6302 0000 0000 0000 0000 0000  tentc...........
+00000c70: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00000c80: 0000 7c01 7c00 5f00 6400 5300 7230 0000  ..|.|._.d.S.r0..
+00000c90: 0072 5700 0000 7256 0000 0072 3600 0000  .rW...rV...r6...
+00000ca0: 7236 0000 0072 3700 0000 7215 0000 0084  r6...r7...r.....
+00000cb0: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+00000cc0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000cd0: 0000 0073 0a00 0000 7c00 a000 6401 a101  ...s....|...d...
+00000ce0: 5300 a902 4e5a 0e72 6573 697a 6549 6e74  S...NZ.resizeInt
+00000cf0: 6572 7661 6c29 01da 095f 6765 745f 6174  erval)..._get_at
+00000d00: 7472 723f 0000 0072 3600 0000 7236 0000  trr?...r6...r6..
+00000d10: 0072 3700 0000 7216 0000 0089 0000 0073  .r7...r........s
+00000d20: 0200 0000 0002 7a16 4361 6e76 6173 2e72  ......z.Canvas.r
+00000d30: 6573 697a 655f 696e 7465 7276 616c 6302  esize_intervalc.
+00000d40: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000d50: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00000d60: 6401 7c01 a102 0100 6400 5300 7258 0000  d.|.....d.S.rX..
+00000d70: 0029 01da 095f 7365 745f 6174 7472 7256  .)..._set_attrrV
+00000d80: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
+00000d90: 0000 7216 0000 008d 0000 0073 0200 0000  ..r........s....
+00000da0: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000db0: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
+00000dc0: 7c00 6a00 5300 7230 0000 0029 0172 3a00  |.j.S.r0...).r:.
+00000dd0: 0000 723f 0000 0072 3600 0000 7236 0000  ..r?...r6...r6..
+00000de0: 0072 3700 0000 723c 0000 0092 0000 0073  .r7...r<.......s
+00000df0: 0200 0000 0002 7a10 4361 6e76 6173 2e6f  ......z.Canvas.o
+00000e00: 6e5f 7265 7369 7a65 6302 0000 0000 0000  n_resizec.......
+00000e10: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000e20: 0073 3200 0000 7c00 6a00 a001 7c01 a101  .s2...|.j...|...
+00000e30: 0100 7c01 6400 7501 7222 7c00 a002 6401  ..|.d.u.r"|...d.
+00000e40: 6402 a102 0100 6e0c 7c00 a002 6401 6400  d.....n.|...d.d.
+00000e50: a102 0100 6400 5300 2903 4e5a 086f 6e72  ....d.S.).NZ.onr
+00000e60: 6573 697a 6554 2903 723a 0000 005a 0973  esizeT).r:...Z.s
+00000e70: 7562 7363 7269 6265 725a 0000 0029 0272  ubscriberZ...).r
+00000e80: 3d00 0000 da07 6861 6e64 6c65 7272 3600  =.....handlerr6.
+00000e90: 0000 7236 0000 0072 3700 0000 723c 0000  ..r6...r7...r<..
+00000ea0: 0096 0000 0073 0800 0000 0002 0c01 0801  .....s..........
+00000eb0: 0e02 291d 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  ..).NNNNNNNNNNNN
+00000ec0: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
+00000ed0: 4e29 1fda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000ee0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000ef0: 6c6e 616d 655f 5f72 0400 0000 7203 0000  lname__r....r...
+00000f00: 0072 0600 0000 7208 0000 0072 0900 0000  .r....r....r....
+00000f10: 720c 0000 0072 0500 0000 da04 626f 6f6c  r....r......bool
+00000f20: da03 696e 7472 0f00 0000 7210 0000 0072  ..intr....r....r
+00000f30: 1100 0000 720e 0000 0072 0d00 0000 7202  ....r....r....r.
+00000f40: 0000 0072 3900 0000 7240 0000 0072 4800  ...r9...r@...rH.
+00000f50: 0000 724a 0000 0072 1200 0000 7251 0000  ..rJ...r....rQ..
+00000f60: 00da 0870 726f 7065 7274 7972 1400 0000  ...propertyr....
+00000f70: da06 7365 7474 6572 7215 0000 0072 1600  ..setterr....r..
+00000f80: 0000 723c 0000 00da 0d5f 5f63 6c61 7373  ..r<.....__class
+00000f90: 6365 6c6c 5f5f 7236 0000 0072 3600 0000  cell__r6...r6...
+00000fa0: 724c 0000 0072 3700 0000 7213 0000 0014  rL...r7...r.....
+00000fb0: 0000 0073 a200 0000 0803 0001 0001 0001  ...s............
+00000fc0: 0004 0001 0001 0001 0001 0001 0001 0001  ................
+00000fd0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+00000fe0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+00000ff0: 0001 00df 0202 0a01 0601 0205 0601 0201  ................
+00001000: 0201 0201 0201 0201 0201 0c01 0601 0601  ................
+00001010: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001020: 0201 0201 0202 0601 0601 02df 0c4c 0803  .............L..
+00001030: 0808 0c04 0201 06ff 0403 0a04 0201 1403  ................
+00001040: 0401 1804 0201 1403 0401 1404 0201 1003  ................
+00001050: 0401 1004 0201 0a03 0401 7213 0000 0063  ..........r....c
+00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001070: 0300 0000 4000 0000 731a 0000 0065 005a  ....@...s....e.Z
+00001080: 0164 005a 0264 0164 029c 0164 0364 0484  .d.Z.d.d...d.d..
+00001090: 045a 0364 0153 0029 0572 3300 0000 4e72  .Z.d.S.).r3...Nr
+000010a0: 5200 0000 6303 0000 0000 0000 0000 0000  R...c...........
+000010b0: 0003 0000 0002 0000 0043 0000 0073 1000  .........C...s..
+000010c0: 0000 7c01 7c00 5f00 7c02 7c00 5f01 6400  ..|.|._.|.|._.d.
+000010d0: 5300 7230 0000 0029 0272 1800 0000 7219  S.r0...).r....r.
+000010e0: 0000 0029 0372 3d00 0000 da01 77da 0168  ...).r=.....w..h
+000010f0: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
+00001100: 3900 0000 a000 0000 7304 0000 0000 0106  9.......s.......
+00001110: 017a 1a43 616e 7661 7352 6573 697a 6545  .z.CanvasResizeE
+00001120: 7665 6e74 2e5f 5f69 6e69 745f 5f29 0472  vent.__init__).r
+00001130: 5c00 0000 725d 0000 0072 5e00 0000 7239  \...r]...r^...r9
+00001140: 0000 0072 3600 0000 7236 0000 0072 3600  ...r6...r6...r6.
+00001150: 0000 7237 0000 0072 3300 0000 9f00 0000  ..r7...r3.......
+00001160: 7302 0000 0008 0172 3300 0000 291d 7231  s......r3...).r1
+00001170: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
+00001180: 7203 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
+00001190: 1666 6c65 745f 636f 7265 2e63 616e 7661  .flet_core.canva
+000011a0: 732e 7368 6170 6572 0600 0000 5a1d 666c  s.shaper....Z.fl
+000011b0: 6574 5f63 6f72 652e 636f 6e73 7472 6169  et_core.constrai
+000011c0: 6e65 645f 636f 6e74 726f 6c72 0700 0000  ned_controlr....
+000011d0: da11 666c 6574 5f63 6f72 652e 636f 6e74  ..flet_core.cont
+000011e0: 726f 6c72 0800 0000 7209 0000 00da 1766  rolr....r......f
+000011f0: 6c65 745f 636f 7265 2e63 6f6e 7472 6f6c  let_core.control
+00001200: 5f65 7665 6e74 720a 0000 005a 1766 6c65  _eventr....Z.fle
+00001210: 745f 636f 7265 2e65 7665 6e74 5f68 616e  t_core.event_han
+00001220: 646c 6572 720b 0000 00da 0d66 6c65 745f  dlerr......flet_
+00001230: 636f 7265 2e72 6566 720c 0000 00da 0f66  core.refr......f
+00001240: 6c65 745f 636f 7265 2e74 7970 6573 720d  let_core.typesr.
+00001250: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
+00001260: 0000 7211 0000 00da 0f66 6c65 745f 636f  ..r......flet_co
+00001270: 7265 2e75 7469 6c73 7212 0000 0072 1300  re.utilsr....r..
+00001280: 0000 7233 0000 0072 3600 0000 7236 0000  ..r3...r6...r6..
+00001290: 0072 3600 0000 7237 0000 00da 083c 6d6f  .r6...r7.....<mo
+000012a0: 6475 6c65 3e01 0000 0073 1800 0000 0801  dule>....s......
+000012b0: 1802 0c01 0c01 1001 0c01 0c01 0c01 1c07  ................
+000012c0: 0c03 107f 000c                           ......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1646 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 6e06 0000  a........:)fn...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 6e06 0000  a........./fn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
@@ -37,111 +37,112 @@
 00000240: 0564 0053 0029 024e 2904 da03 7265 6672  .d.S.).N)...refr
 00000250: 0c00 0000 720d 0000 0072 0e00 0000 2906  ....r....r....).
 00000260: 7204 0000 00da 085f 5f69 6e69 745f 5f72  r......__init__r
 00000270: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
 00000280: 0000 0029 09da 0473 656c 6672 0800 0000  ...)...selfr....
 00000290: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
 000002a0: 0f00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
-000002b0: 0000 00a9 0072 1200 0000 fa59 2f77 6f72  .....r.....Y/wor
+000002b0: 0000 00a9 0072 1200 0000 fa60 2f77 6f72  .....r.....`/wor
 000002c0: 6b73 7061 6365 732f 636f 6e74 7269 6266  kspaces/contribf
-000002d0: 6c65 742f 666c 6574 2f73 646b 2f70 7974  let/flet/sdk/pyt
-000002e0: 686f 6e2f 7061 636b 6167 6573 2f66 6c65  hon/packages/fle
-000002f0: 742d 636f 7265 2f73 7263 2f66 6c65 745f  t-core/src/flet_
-00000300: 636f 7265 2f63 616e 7661 732f 6369 7263  core/canvas/circ
-00000310: 6c65 2e70 7972 1000 0000 0900 0000 730a  le.pyr........s.
-00000320: 0000 0000 0e14 0206 0106 0106 017a 0f43  .............z.C
-00000330: 6972 636c 652e 5f5f 696e 6974 5f5f 6301  ircle.__init__c.
-00000340: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000350: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
-00000360: 2902 4eda 0663 6972 636c 6572 1200 0000  ).N..circler....
-00000370: a901 7211 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00000380: 0072 1300 0000 da11 5f67 6574 5f63 6f6e  .r......_get_con
-00000390: 7472 6f6c 5f6e 616d 651e 0000 0073 0200  trol_name....s..
-000003a0: 0000 0001 7a18 4369 7263 6c65 2e5f 6765  ....z.Circle._ge
-000003b0: 745f 636f 6e74 726f 6c5f 6e61 6d65 6301  t_control_namec.
-000003c0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000003d0: 0000 0003 0000 0073 1c00 0000 7400 8300  .......s....t...
-000003e0: a001 a100 0100 7c00 a002 6401 7c00 6a03  ......|...d.|.j.
-000003f0: a102 0100 6400 5300 2902 4e72 0b00 0000  ....d.S.).Nr....
-00000400: 2904 da05 7375 7065 72da 0d62 6566 6f72  )...super..befor
-00000410: 655f 7570 6461 7465 da0e 5f73 6574 5f61  e_update.._set_a
-00000420: 7474 725f 6a73 6f6e da0e 5f43 6972 636c  ttr_json.._Circl
-00000430: 655f 5f70 6169 6e74 7215 0000 00a9 01da  e__paintr.......
-00000440: 095f 5f63 6c61 7373 5f5f 7212 0000 0072  .__class__r....r
-00000450: 1300 0000 7218 0000 0021 0000 0073 0400  ....r....!...s..
-00000460: 0000 0001 0a01 7a14 4369 7263 6c65 2e62  ......z.Circle.b
-00000470: 6566 6f72 655f 7570 6461 7465 2901 da06  efore_update)...
-00000480: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-00000490: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000004a0: 0a00 0000 7c00 a000 6401 a101 5300 a902  ....|...d...S...
-000004b0: 4e72 0800 0000 a901 da09 5f67 6574 5f61  Nr........_get_a
-000004c0: 7474 7272 1500 0000 7212 0000 0072 1200  ttrr....r....r..
-000004d0: 0000 7213 0000 0072 0800 0000 2600 0000  ..r....r....&...
-000004e0: 7302 0000 0000 027a 0843 6972 636c 652e  s......z.Circle.
-000004f0: 7829 01da 0576 616c 7565 6302 0000 0000  x)...valuec.....
-00000500: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000510: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
-00000520: a102 0100 6400 5300 721e 0000 00a9 01da  ....d.S.r.......
-00000530: 095f 7365 745f 6174 7472 a902 7211 0000  ._set_attr..r...
-00000540: 0072 2100 0000 7212 0000 0072 1200 0000  .r!...r....r....
-00000550: 7213 0000 0072 0800 0000 2a00 0000 7302  r....r....*...s.
-00000560: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00000570: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
-00000580: 0000 007c 00a0 0064 01a1 0153 00a9 024e  ...|...d...S...N
-00000590: 7209 0000 0072 1f00 0000 7215 0000 0072  r....r....r....r
-000005a0: 1200 0000 7212 0000 0072 1300 0000 7209  ....r....r....r.
-000005b0: 0000 002f 0000 0073 0200 0000 0002 7a08  .../...s......z.
-000005c0: 4369 7263 6c65 2e79 6302 0000 0000 0000  Circle.yc.......
-000005d0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000005e0: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
-000005f0: 0100 6400 5300 7225 0000 0072 2200 0000  ..d.S.r%...r"...
-00000600: 7224 0000 0072 1200 0000 7212 0000 0072  r$...r....r....r
-00000610: 1300 0000 7209 0000 0033 0000 0073 0200  ....r....3...s..
-00000620: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000630: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-00000640: 0000 7c00 a000 6401 a101 5300 a902 4e72  ..|...d...S...Nr
-00000650: 0a00 0000 721f 0000 0072 1500 0000 7212  ....r....r....r.
-00000660: 0000 0072 1200 0000 7213 0000 0072 0a00  ...r....r....r..
-00000670: 0000 3800 0000 7302 0000 0000 027a 0d43  ..8...s......z.C
-00000680: 6972 636c 652e 7261 6469 7573 6302 0000  ircle.radiusc...
-00000690: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000006a0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-000006b0: 7c01 a102 0100 6400 5300 7226 0000 0072  |.....d.S.r&...r
-000006c0: 2200 0000 7224 0000 0072 1200 0000 7212  "...r$...r....r.
-000006d0: 0000 0072 1300 0000 720a 0000 003c 0000  ...r....r....<..
-000006e0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-000006f0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000700: 0073 0600 0000 7c00 6a00 5300 a901 4ea9  .s....|.j.S...N.
-00000710: 0172 1a00 0000 7215 0000 0072 1200 0000  .r....r....r....
-00000720: 7212 0000 0072 1300 0000 720b 0000 0041  r....r....r....A
-00000730: 0000 0073 0200 0000 0002 7a0c 4369 7263  ...s......z.Circ
-00000740: 6c65 2e70 6169 6e74 6302 0000 0000 0000  le.paintc.......
-00000750: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00000760: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
-00000770: 7227 0000 0072 2800 0000 7224 0000 0072  r'...r(...r$...r
-00000780: 1200 0000 7212 0000 0072 1300 0000 720b  ....r....r....r.
-00000790: 0000 0045 0000 0073 0200 0000 0002 2908  ...E...s......).
-000007a0: 4e4e 4e4e 4e4e 4e4e 2912 da08 5f5f 6e61  NNNNNNNN)...__na
-000007b0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000007c0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7205  ..__qualname__r.
-000007d0: 0000 0072 0300 0000 7206 0000 00da 0462  ...r....r......b
-000007e0: 6f6f 6c72 0200 0000 7210 0000 0072 1600  oolr....r....r..
-000007f0: 0000 7218 0000 00da 0870 726f 7065 7274  ..r......propert
-00000800: 7972 0800 0000 da06 7365 7474 6572 7209  yr......setterr.
-00000810: 0000 0072 0a00 0000 720b 0000 00da 0d5f  ...r....r......_
-00000820: 5f63 6c61 7373 6365 6c6c 5f5f 7212 0000  _classcell__r...
-00000830: 0072 1200 0000 721b 0000 0072 1300 0000  .r....r....r....
-00000840: 7207 0000 0008 0000 0073 4600 0000 0803  r........sF.....
-00000850: 0001 0001 0001 0004 0001 0001 0001 00f4  ................
-00000860: 0202 0201 0201 0201 0605 0601 0601 02f4  ................
-00000870: 0c15 0803 0c05 0201 1003 0401 1004 0201  ................
-00000880: 1003 0401 1004 0201 1003 0401 1004 0201  ................
-00000890: 1403 0401 7207 0000 004e 290a da06 7479  ....r....N)...ty
-000008a0: 7069 6e67 7202 0000 0072 0300 0000 da16  pingr....r......
-000008b0: 666c 6574 5f63 6f72 652e 6361 6e76 6173  flet_core.canvas
-000008c0: 2e73 6861 7065 7204 0000 00da 1166 6c65  .shaper......fle
-000008d0: 745f 636f 7265 2e63 6f6e 7472 6f6c 7205  t_core.controlr.
-000008e0: 0000 00da 1266 6c65 745f 636f 7265 2e70  .....flet_core.p
-000008f0: 6169 6e74 696e 6772 0600 0000 7207 0000  aintingr....r...
-00000900: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00000910: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000920: 0000 0073 0800 0000 1002 0c01 0c01 0c03  ...s............
+000002d0: 6c65 742f 666c 6574 636f 6e74 7269 622f  let/fletcontrib/
+000002e0: 7364 6b2f 7079 7468 6f6e 2f70 6163 6b61  sdk/python/packa
+000002f0: 6765 732f 666c 6574 2d63 6f72 652f 7372  ges/flet-core/sr
+00000300: 632f 666c 6574 5f63 6f72 652f 6361 6e76  c/flet_core/canv
+00000310: 6173 2f63 6972 636c 652e 7079 7210 0000  as/circle.pyr...
+00000320: 0009 0000 0073 0a00 0000 000e 1402 0601  .....s..........
+00000330: 0601 0601 7a0f 4369 7263 6c65 2e5f 5f69  ....z.Circle.__i
+00000340: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000350: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
+00000360: 0000 0064 0153 0029 024e da06 6369 7263  ...d.S.).N..circ
+00000370: 6c65 7212 0000 00a9 0172 1100 0000 7212  ler......r....r.
+00000380: 0000 0072 1200 0000 7213 0000 00da 115f  ...r....r......_
+00000390: 6765 745f 636f 6e74 726f 6c5f 6e61 6d65  get_control_name
+000003a0: 1e00 0000 7302 0000 0000 017a 1843 6972  ....s......z.Cir
+000003b0: 636c 652e 5f67 6574 5f63 6f6e 7472 6f6c  cle._get_control
+000003c0: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
+000003d0: 0000 0100 0000 0400 0000 0300 0000 731c  ..............s.
+000003e0: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
+000003f0: 0264 017c 006a 03a1 0201 0064 0053 0029  .d.|.j.....d.S.)
+00000400: 024e 720b 0000 0029 04da 0573 7570 6572  .Nr....)...super
+00000410: da0d 6265 666f 7265 5f75 7064 6174 65da  ..before_update.
+00000420: 0e5f 7365 745f 6174 7472 5f6a 736f 6eda  ._set_attr_json.
+00000430: 0e5f 4369 7263 6c65 5f5f 7061 696e 7472  ._Circle__paintr
+00000440: 1500 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+00000450: 5f72 1200 0000 7213 0000 0072 1800 0000  _r....r....r....
+00000460: 2100 0000 7304 0000 0000 010a 017a 1443  !...s........z.C
+00000470: 6972 636c 652e 6265 666f 7265 5f75 7064  ircle.before_upd
+00000480: 6174 6529 01da 0672 6574 7572 6e63 0100  ate)...returnc..
+00000490: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000004a0: 0000 4300 0000 730a 0000 007c 00a0 0064  ..C...s....|...d
+000004b0: 01a1 0153 00a9 024e 7208 0000 00a9 01da  ...S...Nr.......
+000004c0: 095f 6765 745f 6174 7472 7215 0000 0072  ._get_attrr....r
+000004d0: 1200 0000 7212 0000 0072 1300 0000 7208  ....r....r....r.
+000004e0: 0000 0026 0000 0073 0200 0000 0002 7a08  ...&...s......z.
+000004f0: 4369 7263 6c65 2e78 2901 da05 7661 6c75  Circle.x)...valu
+00000500: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00000510: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
+00000520: 00a0 0064 017c 01a1 0201 0064 0053 0072  ...d.|.....d.S.r
+00000530: 1e00 0000 a901 da09 5f73 6574 5f61 7474  ........_set_att
+00000540: 72a9 0272 1100 0000 7221 0000 0072 1200  r..r....r!...r..
+00000550: 0000 7212 0000 0072 1300 0000 7208 0000  ..r....r....r...
+00000560: 002a 0000 0073 0200 0000 0002 6301 0000  .*...s......c...
+00000570: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000580: 0043 0000 0073 0a00 0000 7c00 a000 6401  .C...s....|...d.
+00000590: a101 5300 a902 4e72 0900 0000 721f 0000  ..S...Nr....r...
+000005a0: 0072 1500 0000 7212 0000 0072 1200 0000  .r....r....r....
+000005b0: 7213 0000 0072 0900 0000 2f00 0000 7302  r....r..../...s.
+000005c0: 0000 0000 027a 0843 6972 636c 652e 7963  .....z.Circle.yc
+000005d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000005e0: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+000005f0: 0064 017c 01a1 0201 0064 0053 0072 2500  .d.|.....d.S.r%.
+00000600: 0000 7222 0000 0072 2400 0000 7212 0000  ..r"...r$...r...
+00000610: 0072 1200 0000 7213 0000 0072 0900 0000  .r....r....r....
+00000620: 3300 0000 7302 0000 0000 0263 0100 0000  3...s......c....
+00000630: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000640: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
+00000650: 0153 00a9 024e 720a 0000 0072 1f00 0000  .S...Nr....r....
+00000660: 7215 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000670: 1300 0000 720a 0000 0038 0000 0073 0200  ....r....8...s..
+00000680: 0000 0002 7a0d 4369 7263 6c65 2e72 6164  ....z.Circle.rad
+00000690: 6975 7363 0200 0000 0000 0000 0000 0000  iusc............
+000006a0: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+000006b0: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+000006c0: 0072 2600 0000 7222 0000 0072 2400 0000  .r&...r"...r$...
+000006d0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000006e0: 0a00 0000 3c00 0000 7302 0000 0000 0263  ....<...s......c
+000006f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000700: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+00000710: 0053 00a9 014e a901 721a 0000 0072 1500  .S...N..r....r..
+00000720: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000730: 0072 0b00 0000 4100 0000 7302 0000 0000  .r....A...s.....
+00000740: 027a 0c43 6972 636c 652e 7061 696e 7463  .z.Circle.paintc
+00000750: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000760: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
+00000770: 005f 0064 0053 0072 2700 0000 7228 0000  ._.d.S.r'...r(..
+00000780: 0072 2400 0000 7212 0000 0072 1200 0000  .r$...r....r....
+00000790: 7213 0000 0072 0b00 0000 4500 0000 7302  r....r....E...s.
+000007a0: 0000 0000 0229 084e 4e4e 4e4e 4e4e 4e29  .....).NNNNNNNN)
+000007b0: 12da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000007c0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000007d0: 616d 655f 5f72 0500 0000 7203 0000 0072  ame__r....r....r
+000007e0: 0600 0000 da04 626f 6f6c 7202 0000 0072  ......boolr....r
+000007f0: 1000 0000 7216 0000 0072 1800 0000 da08  ....r....r......
+00000800: 7072 6f70 6572 7479 7208 0000 00da 0673  propertyr......s
+00000810: 6574 7465 7272 0900 0000 720a 0000 0072  etterr....r....r
+00000820: 0b00 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00000830: 6c5f 5f72 1200 0000 7212 0000 0072 1b00  l__r....r....r..
+00000840: 0000 7213 0000 0072 0700 0000 0800 0000  ..r....r........
+00000850: 7346 0000 0008 0300 0100 0100 0100 0400  sF..............
+00000860: 0100 0100 0100 f402 0202 0102 0102 0106  ................
+00000870: 0506 0106 0102 f40c 1508 030c 0502 0110  ................
+00000880: 0304 0110 0402 0110 0304 0110 0402 0110  ................
+00000890: 0304 0110 0402 0114 0304 0172 0700 0000  ...........r....
+000008a0: 4e29 0ada 0674 7970 696e 6772 0200 0000  N)...typingr....
+000008b0: 7203 0000 00da 1666 6c65 745f 636f 7265  r......flet_core
+000008c0: 2e63 616e 7661 732e 7368 6170 6572 0400  .canvas.shaper..
+000008d0: 0000 da11 666c 6574 5f63 6f72 652e 636f  ....flet_core.co
+000008e0: 6e74 726f 6c72 0500 0000 da12 666c 6574  ntrolr......flet
+000008f0: 5f63 6f72 652e 7061 696e 7469 6e67 7206  _core.paintingr.
+00000900: 0000 0072 0700 0000 7212 0000 0072 1200  ...r....r....r..
+00000910: 0000 7212 0000 0072 1300 0000 da08 3c6d  ..r....r......<m
+00000920: 6f64 756c 653e 0100 0000 7308 0000 0010  odule>....s.....
+00000930: 020c 010c 010c 03                        .......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/color.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/color.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1236 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 d404 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 d404 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6504 8303 5a07 6406 5300 2907 e900 0000  e...Z.d.S.).....
 00000070: 0029 02da 0341 6e79 da08 4f70 7469 6f6e  .)...Any..Option
@@ -29,85 +29,85 @@
 000001c0: 7c06 6401 8d05 0100 7c01 7c00 5f02 7c02  |.d.....|.|._.|.
 000001d0: 7c00 5f03 6400 5300 2902 4e29 04da 0372  |._.d.S.).N)...r
 000001e0: 6566 7209 0000 0072 0a00 0000 720b 0000  efr....r....r...
 000001f0: 0029 0472 0400 0000 da08 5f5f 696e 6974  .).r......__init
 00000200: 5f5f 7207 0000 0072 0800 0000 2907 da04  __r....r....)...
 00000210: 7365 6c66 7207 0000 0072 0800 0000 720c  selfr....r....r.
 00000220: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
-00000230: 0000 a900 720f 0000 00fa 582f 776f 726b  ....r.....X/work
+00000230: 0000 a900 720f 0000 00fa 5f2f 776f 726b  ....r....._/work
 00000240: 7370 6163 6573 2f63 6f6e 7472 6962 666c  spaces/contribfl
-00000250: 6574 2f66 6c65 742f 7364 6b2f 7079 7468  et/flet/sdk/pyth
-00000260: 6f6e 2f70 6163 6b61 6765 732f 666c 6574  on/packages/flet
-00000270: 2d63 6f72 652f 7372 632f 666c 6574 5f63  -core/src/flet_c
-00000280: 6f72 652f 6361 6e76 6173 2f63 6f6c 6f72  ore/canvas/color
-00000290: 2e70 7972 0d00 0000 0800 0000 7306 0000  .pyr........s...
-000002a0: 0000 0c14 0206 017a 0e43 6f6c 6f72 2e5f  .......z.Color._
-000002b0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-000002c0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000002d0: 7304 0000 0064 0153 00a9 024e 7207 0000  s....d.S...Nr...
-000002e0: 0072 0f00 0000 a901 720e 0000 0072 0f00  .r......r....r..
-000002f0: 0000 720f 0000 0072 1000 0000 da11 5f67  ..r....r......_g
-00000300: 6574 5f63 6f6e 7472 6f6c 5f6e 616d 6519  et_control_name.
-00000310: 0000 0073 0200 0000 0001 7a17 436f 6c6f  ...s......z.Colo
-00000320: 722e 5f67 6574 5f63 6f6e 7472 6f6c 5f6e  r._get_control_n
-00000330: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-00000340: 0100 0000 0200 0000 0300 0000 730e 0000  ............s...
-00000350: 0074 0083 00a0 01a1 0001 0064 0053 00a9  .t.........d.S..
-00000360: 014e 2902 da05 7375 7065 72da 0d62 6566  .N)...super..bef
-00000370: 6f72 655f 7570 6461 7465 7212 0000 00a9  ore_updater.....
-00000380: 01da 095f 5f63 6c61 7373 5f5f 720f 0000  ...__class__r...
-00000390: 0072 1000 0000 7216 0000 001c 0000 0073  .r....r........s
-000003a0: 0200 0000 0001 7a13 436f 6c6f 722e 6265  ......z.Color.be
-000003b0: 666f 7265 5f75 7064 6174 6529 01da 0672  fore_update)...r
-000003c0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-000003d0: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
-000003e0: 0000 007c 00a0 0064 01a1 0153 0072 1100  ...|...d...S.r..
-000003f0: 0000 2901 da09 5f67 6574 5f61 7474 7272  ..)..._get_attrr
-00000400: 1200 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00000410: 0000 0072 0700 0000 2000 0000 7302 0000  ...r.... ...s...
-00000420: 0000 027a 0b43 6f6c 6f72 2e63 6f6c 6f72  ...z.Color.color
-00000430: 2901 da05 7661 6c75 6563 0200 0000 0000  )...valuec......
-00000440: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000450: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-00000460: 0201 0064 0053 0072 1100 0000 2901 da09  ...d.S.r....)...
-00000470: 5f73 6574 5f61 7474 72a9 0272 0e00 0000  _set_attr..r....
-00000480: 721b 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000490: 1000 0000 7207 0000 0024 0000 0073 0200  ....r....$...s..
-000004a0: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-000004b0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-000004c0: 0000 7c00 6a00 5300 7214 0000 0029 01da  ..|.j.S.r....)..
-000004d0: 125f 436f 6c6f 725f 5f62 6c65 6e64 5f6d  ._Color__blend_m
-000004e0: 6f64 6572 1200 0000 720f 0000 0072 0f00  oder....r....r..
-000004f0: 0000 7210 0000 0072 0800 0000 2900 0000  ..r....r....)...
-00000500: 7302 0000 0000 027a 1043 6f6c 6f72 2e62  s......z.Color.b
-00000510: 6c65 6e64 5f6d 6f64 6563 0200 0000 0000  lend_modec......
-00000520: 0000 0000 0000 0200 0000 0600 0000 4300  ..............C.
-00000530: 0000 7326 0000 007c 017c 005f 007c 00a0  ..s&...|.|._.|..
-00000540: 0164 0174 027c 0174 0383 0272 1c7c 016a  .d.t.|.t...r.|.j
-00000550: 046e 027c 01a1 0201 0064 0053 0029 024e  .n.|.....d.S.).N
-00000560: 5a09 626c 656e 644d 6f64 6529 0572 1e00  Z.blendMode).r..
-00000570: 0000 721c 0000 00da 0a69 7369 6e73 7461  ..r......isinsta
-00000580: 6e63 6572 0500 0000 721b 0000 0072 1d00  ncer....r....r..
-00000590: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000005a0: 0072 0800 0000 2d00 0000 7308 0000 0000  .r....-...s.....
-000005b0: 0206 0104 0114 ff29 064e 4e4e 4e4e 4e29  .......).NNNNNN)
-000005c0: 10da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000005d0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000005e0: 616d 655f 5f72 0300 0000 da03 7374 7272  ame__r......strr
-000005f0: 0500 0000 da04 626f 6f6c 7202 0000 0072  ......boolr....r
-00000600: 0d00 0000 7213 0000 0072 1600 0000 da08  ....r....r......
-00000610: 7072 6f70 6572 7479 7207 0000 00da 0673  propertyr......s
-00000620: 6574 7465 7272 0800 0000 da0d 5f5f 636c  etterr......__cl
-00000630: 6173 7363 656c 6c5f 5f72 0f00 0000 720f  asscell__r....r.
-00000640: 0000 0072 1700 0000 7210 0000 0072 0600  ...r....r....r..
-00000650: 0000 0700 0000 732e 0000 0008 0300 0100  ......s.........
-00000660: 0400 0100 0100 0100 f602 0206 0106 0506  ................
-00000670: 0106 0102 f60c 1108 030c 0402 0114 0304  ................
-00000680: 0114 0402 0114 0304 0172 0600 0000 4e29  .........r....N)
-00000690: 08da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
-000006a0: 0000 00da 1666 6c65 745f 636f 7265 2e63  .....flet_core.c
-000006b0: 616e 7661 732e 7368 6170 6572 0400 0000  anvas.shaper....
-000006c0: da0f 666c 6574 5f63 6f72 652e 7479 7065  ..flet_core.type
-000006d0: 7372 0500 0000 7206 0000 0072 0f00 0000  sr....r....r....
-000006e0: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-000006f0: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
-00000700: 0000 1002 0c01 0c03                      ........
+00000250: 6574 2f66 6c65 7463 6f6e 7472 6962 2f73  et/fletcontrib/s
+00000260: 646b 2f70 7974 686f 6e2f 7061 636b 6167  dk/python/packag
+00000270: 6573 2f66 6c65 742d 636f 7265 2f73 7263  es/flet-core/src
+00000280: 2f66 6c65 745f 636f 7265 2f63 616e 7661  /flet_core/canva
+00000290: 732f 636f 6c6f 722e 7079 720d 0000 0008  s/color.pyr.....
+000002a0: 0000 0073 0600 0000 000c 1402 0601 7a0e  ...s..........z.
+000002b0: 436f 6c6f 722e 5f5f 696e 6974 5f5f 6301  Color.__init__c.
+000002c0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+000002d0: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
+000002e0: a902 4e72 0700 0000 720f 0000 00a9 0172  ..Nr....r......r
+000002f0: 0e00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00000300: 0000 00da 115f 6765 745f 636f 6e74 726f  ....._get_contro
+00000310: 6c5f 6e61 6d65 1900 0000 7302 0000 0000  l_name....s.....
+00000320: 017a 1743 6f6c 6f72 2e5f 6765 745f 636f  .z.Color._get_co
+00000330: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
+00000340: 0000 0000 0000 0001 0000 0002 0000 0003  ................
+00000350: 0000 0073 0e00 0000 7400 8300 a001 a100  ...s....t.......
+00000360: 0100 6400 5300 a901 4e29 02da 0573 7570  ..d.S...N)...sup
+00000370: 6572 da0d 6265 666f 7265 5f75 7064 6174  er..before_updat
+00000380: 6572 1200 0000 a901 da09 5f5f 636c 6173  er........__clas
+00000390: 735f 5f72 0f00 0000 7210 0000 0072 1600  s__r....r....r..
+000003a0: 0000 1c00 0000 7302 0000 0000 017a 1343  ......s......z.C
+000003b0: 6f6c 6f72 2e62 6566 6f72 655f 7570 6461  olor.before_upda
+000003c0: 7465 2901 da06 7265 7475 726e 6301 0000  te)...returnc...
+000003d0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000003e0: 0043 0000 0073 0a00 0000 7c00 a000 6401  .C...s....|...d.
+000003f0: a101 5300 7211 0000 0029 01da 095f 6765  ..S.r....)..._ge
+00000400: 745f 6174 7472 7212 0000 0072 0f00 0000  t_attrr....r....
+00000410: 720f 0000 0072 1000 0000 7207 0000 0020  r....r....r.... 
+00000420: 0000 0073 0200 0000 0002 7a0b 436f 6c6f  ...s......z.Colo
+00000430: 722e 636f 6c6f 7229 01da 0576 616c 7565  r.color)...value
+00000440: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000450: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00000460: a000 6401 7c01 a102 0100 6400 5300 7211  ..d.|.....d.S.r.
+00000470: 0000 0029 01da 095f 7365 745f 6174 7472  ...)..._set_attr
+00000480: a902 720e 0000 0072 1b00 0000 720f 0000  ..r....r....r...
+00000490: 0072 0f00 0000 7210 0000 0072 0700 0000  .r....r....r....
+000004a0: 2400 0000 7302 0000 0000 0263 0100 0000  $...s......c....
+000004b0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+000004c0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
+000004d0: 1400 0000 2901 da12 5f43 6f6c 6f72 5f5f  ....)..._Color__
+000004e0: 626c 656e 645f 6d6f 6465 7212 0000 0072  blend_moder....r
+000004f0: 0f00 0000 720f 0000 0072 1000 0000 7208  ....r....r....r.
+00000500: 0000 0029 0000 0073 0200 0000 0002 7a10  ...)...s......z.
+00000510: 436f 6c6f 722e 626c 656e 645f 6d6f 6465  Color.blend_mode
+00000520: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000530: 0006 0000 0043 0000 0073 2600 0000 7c01  .....C...s&...|.
+00000540: 7c00 5f00 7c00 a001 6401 7402 7c01 7403  |._.|...d.t.|.t.
+00000550: 8302 721c 7c01 6a04 6e02 7c01 a102 0100  ..r.|.j.n.|.....
+00000560: 6400 5300 2902 4e5a 0962 6c65 6e64 4d6f  d.S.).NZ.blendMo
+00000570: 6465 2905 721e 0000 0072 1c00 0000 da0a  de).r....r......
+00000580: 6973 696e 7374 616e 6365 7205 0000 0072  isinstancer....r
+00000590: 1b00 0000 721d 0000 0072 0f00 0000 720f  ....r....r....r.
+000005a0: 0000 0072 1000 0000 7208 0000 002d 0000  ...r....r....-..
+000005b0: 0073 0800 0000 0002 0601 0401 14ff 2906  .s............).
+000005c0: 4e4e 4e4e 4e4e 2910 da08 5f5f 6e61 6d65  NNNNNN)...__name
+000005d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000005e0: 5f5f 7175 616c 6e61 6d65 5f5f 7203 0000  __qualname__r...
+000005f0: 00da 0373 7472 7205 0000 00da 0462 6f6f  ...strr......boo
+00000600: 6c72 0200 0000 720d 0000 0072 1300 0000  lr....r....r....
+00000610: 7216 0000 00da 0870 726f 7065 7274 7972  r......propertyr
+00000620: 0700 0000 da06 7365 7474 6572 7208 0000  ......setterr...
+00000630: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000640: 720f 0000 0072 0f00 0000 7217 0000 0072  r....r....r....r
+00000650: 1000 0000 7206 0000 0007 0000 0073 2e00  ....r........s..
+00000660: 0000 0803 0001 0004 0001 0001 0001 00f6  ................
+00000670: 0202 0601 0605 0601 0601 02f6 0c11 0803  ................
+00000680: 0c04 0201 1403 0401 1404 0201 1403 0401  ................
+00000690: 7206 0000 004e 2908 da06 7479 7069 6e67  r....N)...typing
+000006a0: 7202 0000 0072 0300 0000 da16 666c 6574  r....r......flet
+000006b0: 5f63 6f72 652e 6361 6e76 6173 2e73 6861  _core.canvas.sha
+000006c0: 7065 7204 0000 00da 0f66 6c65 745f 636f  per......flet_co
+000006d0: 7265 2e74 7970 6573 7205 0000 0072 0600  re.typesr....r..
+000006e0: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+000006f0: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000700: 0100 0000 7306 0000 0010 020c 010c 03    ....s..........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 844 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 4c03 0000  a........:)fL...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 4c03 0000  a........./fL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6504 8303 5a07 6406 5300 2907 e900 0000  e...Z.d.S.).....
 00000070: 0029 02da 0341 6e79 da08 4f70 7469 6f6e  .)...Any..Option
@@ -24,67 +24,68 @@
 00000170: 006a 017c 007c 027c 037c 047c 0564 018d  .j.|.|.|.|.|.d..
 00000180: 0501 007c 017c 005f 0264 0053 0029 024e  ...|.|._.d.S.).N
 00000190: 2904 da03 7265 6672 0800 0000 7209 0000  )...refr....r...
 000001a0: 0072 0a00 0000 2903 7204 0000 00da 085f  .r....).r......_
 000001b0: 5f69 6e69 745f 5f72 0700 0000 2906 da04  _init__r....)...
 000001c0: 7365 6c66 7207 0000 0072 0b00 0000 7208  selfr....r....r.
 000001d0: 0000 0072 0900 0000 720a 0000 00a9 0072  ...r....r......r
-000001e0: 0e00 0000 fa57 2f77 6f72 6b73 7061 6365  .....W/workspace
+000001e0: 0e00 0000 fa5e 2f77 6f72 6b73 7061 6365  .....^/workspace
 000001f0: 732f 636f 6e74 7269 6266 6c65 742f 666c  s/contribflet/fl
-00000200: 6574 2f73 646b 2f70 7974 686f 6e2f 7061  et/sdk/python/pa
-00000210: 636b 6167 6573 2f66 6c65 742d 636f 7265  ckages/flet-core
-00000220: 2f73 7263 2f66 6c65 745f 636f 7265 2f63  /src/flet_core/c
-00000230: 616e 7661 732f 6669 6c6c 2e70 7972 0c00  anvas/fill.pyr..
-00000240: 0000 0800 0000 7304 0000 0000 0b14 027a  ......s........z
-00000250: 0d46 696c 6c2e 5f5f 696e 6974 5f5f 6301  .Fill.__init__c.
-00000260: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000270: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
-00000280: 2902 4eda 0466 696c 6c72 0e00 0000 a901  ).N..fillr......
-00000290: 720d 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-000002a0: 0f00 0000 da11 5f67 6574 5f63 6f6e 7472  ......_get_contr
-000002b0: 6f6c 5f6e 616d 6517 0000 0073 0200 0000  ol_name....s....
-000002c0: 0001 7a16 4669 6c6c 2e5f 6765 745f 636f  ..z.Fill._get_co
-000002d0: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
-000002e0: 0000 0000 0000 0001 0000 0004 0000 0003  ................
-000002f0: 0000 0073 1c00 0000 7400 8300 a001 a100  ...s....t.......
-00000300: 0100 7c00 a002 6401 7c00 6a03 a102 0100  ..|...d.|.j.....
-00000310: 6400 5300 2902 4e72 0700 0000 2904 da05  d.S.).Nr....)...
-00000320: 7375 7065 72da 0d62 6566 6f72 655f 7570  super..before_up
-00000330: 6461 7465 da0e 5f73 6574 5f61 7474 725f  date.._set_attr_
-00000340: 6a73 6f6e da0c 5f46 696c 6c5f 5f70 6169  json.._Fill__pai
-00000350: 6e74 7211 0000 00a9 01da 095f 5f63 6c61  ntr........__cla
-00000360: 7373 5f5f 720e 0000 0072 0f00 0000 7214  ss__r....r....r.
-00000370: 0000 001a 0000 0073 0400 0000 0001 0a01  .......s........
-00000380: 7a12 4669 6c6c 2e62 6566 6f72 655f 7570  z.Fill.before_up
-00000390: 6461 7465 2901 da06 7265 7475 726e 6301  date)...returnc.
-000003a0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000003b0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-000003c0: 5300 a901 4ea9 0172 1600 0000 7211 0000  S...N..r....r...
-000003d0: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000003e0: 7207 0000 001f 0000 0073 0200 0000 0002  r........s......
-000003f0: 7a0a 4669 6c6c 2e70 6169 6e74 2901 da05  z.Fill.paint)...
-00000400: 7661 6c75 6563 0200 0000 0000 0000 0000  valuec..........
-00000410: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-00000420: 0000 007c 017c 005f 0064 0053 0072 1a00  ...|.|._.d.S.r..
-00000430: 0000 721b 0000 0029 0272 0d00 0000 721c  ..r....).r....r.
-00000440: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
-00000450: 0000 7207 0000 0023 0000 0073 0200 0000  ..r....#...s....
-00000460: 0002 2905 4e4e 4e4e 4e29 0eda 085f 5f6e  ..).NNNNN)...__n
-00000470: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000480: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000490: 0300 0000 7205 0000 00da 0462 6f6f 6c72  ....r......boolr
-000004a0: 0200 0000 720c 0000 0072 1200 0000 7214  ....r....r....r.
-000004b0: 0000 00da 0870 726f 7065 7274 7972 0700  .....propertyr..
-000004c0: 0000 da06 7365 7474 6572 da0d 5f5f 636c  ....setter..__cl
-000004d0: 6173 7363 656c 6c5f 5f72 0e00 0000 720e  asscell__r....r.
-000004e0: 0000 0072 1700 0000 720f 0000 0072 0600  ...r....r....r..
-000004f0: 0000 0700 0000 7322 0000 0008 0300 0400  ......s"........
-00000500: 0100 0100 0100 f702 0206 0506 0106 0102  ................
-00000510: f70c 0f08 030c 0502 0114 0304 0172 0600  .............r..
-00000520: 0000 4e29 08da 0674 7970 696e 6772 0200  ..N)...typingr..
-00000530: 0000 7203 0000 00da 1666 6c65 745f 636f  ..r......flet_co
-00000540: 7265 2e63 616e 7661 732e 7368 6170 6572  re.canvas.shaper
-00000550: 0400 0000 da12 666c 6574 5f63 6f72 652e  ......flet_core.
-00000560: 7061 696e 7469 6e67 7205 0000 0072 0600  paintingr....r..
-00000570: 0000 720e 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-00000580: 0072 0f00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000590: 0100 0000 7306 0000 0010 020c 010c 03    ....s..........
+00000200: 6574 636f 6e74 7269 622f 7364 6b2f 7079  etcontrib/sdk/py
+00000210: 7468 6f6e 2f70 6163 6b61 6765 732f 666c  thon/packages/fl
+00000220: 6574 2d63 6f72 652f 7372 632f 666c 6574  et-core/src/flet
+00000230: 5f63 6f72 652f 6361 6e76 6173 2f66 696c  _core/canvas/fil
+00000240: 6c2e 7079 720c 0000 0008 0000 0073 0400  l.pyr........s..
+00000250: 0000 000b 1402 7a0d 4669 6c6c 2e5f 5f69  ......z.Fill.__i
+00000260: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000270: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
+00000280: 0000 0064 0153 0029 024e da04 6669 6c6c  ...d.S.).N..fill
+00000290: 720e 0000 00a9 0172 0d00 0000 720e 0000  r......r....r...
+000002a0: 0072 0e00 0000 720f 0000 00da 115f 6765  .r....r......_ge
+000002b0: 745f 636f 6e74 726f 6c5f 6e61 6d65 1700  t_control_name..
+000002c0: 0000 7302 0000 0000 017a 1646 696c 6c2e  ..s......z.Fill.
+000002d0: 5f67 6574 5f63 6f6e 7472 6f6c 5f6e 616d  _get_control_nam
+000002e0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+000002f0: 0000 0400 0000 0300 0000 731c 0000 0074  ..........s....t
+00000300: 0083 00a0 01a1 0001 007c 00a0 0264 017c  .........|...d.|
+00000310: 006a 03a1 0201 0064 0053 0029 024e 7207  .j.....d.S.).Nr.
+00000320: 0000 0029 04da 0573 7570 6572 da0d 6265  ...)...super..be
+00000330: 666f 7265 5f75 7064 6174 65da 0e5f 7365  fore_update.._se
+00000340: 745f 6174 7472 5f6a 736f 6eda 0c5f 4669  t_attr_json.._Fi
+00000350: 6c6c 5f5f 7061 696e 7472 1100 0000 a901  ll__paintr......
+00000360: da09 5f5f 636c 6173 735f 5f72 0e00 0000  ..__class__r....
+00000370: 720f 0000 0072 1400 0000 1a00 0000 7304  r....r........s.
+00000380: 0000 0000 010a 017a 1246 696c 6c2e 6265  .......z.Fill.be
+00000390: 666f 7265 5f75 7064 6174 6529 01da 0672  fore_update)...r
+000003a0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+000003b0: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+000003c0: 0000 007c 006a 0053 00a9 014e a901 7216  ...|.j.S...N..r.
+000003d0: 0000 0072 1100 0000 720e 0000 0072 0e00  ...r....r....r..
+000003e0: 0000 720f 0000 0072 0700 0000 1f00 0000  ..r....r........
+000003f0: 7302 0000 0000 027a 0a46 696c 6c2e 7061  s......z.Fill.pa
+00000400: 696e 7429 01da 0576 616c 7565 6302 0000  int)...valuec...
+00000410: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000420: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000430: 6400 5300 721a 0000 0072 1b00 0000 2902  d.S.r....r....).
+00000440: 720d 0000 0072 1c00 0000 720e 0000 0072  r....r....r....r
+00000450: 0e00 0000 720f 0000 0072 0700 0000 2300  ....r....r....#.
+00000460: 0000 7302 0000 0000 0229 054e 4e4e 4e4e  ..s......).NNNNN
+00000470: 290e da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000480: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000490: 6e61 6d65 5f5f 7203 0000 0072 0500 0000  name__r....r....
+000004a0: da04 626f 6f6c 7202 0000 0072 0c00 0000  ..boolr....r....
+000004b0: 7212 0000 0072 1400 0000 da08 7072 6f70  r....r......prop
+000004c0: 6572 7479 7207 0000 00da 0673 6574 7465  ertyr......sette
+000004d0: 72da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  r..__classcell__
+000004e0: 720e 0000 0072 0e00 0000 7217 0000 0072  r....r....r....r
+000004f0: 0f00 0000 7206 0000 0007 0000 0073 2200  ....r........s".
+00000500: 0000 0803 0004 0001 0001 0001 00f7 0202  ................
+00000510: 0605 0601 0601 02f7 0c0f 0803 0c05 0201  ................
+00000520: 1403 0401 7206 0000 004e 2908 da06 7479  ....r....N)...ty
+00000530: 7069 6e67 7202 0000 0072 0300 0000 da16  pingr....r......
+00000540: 666c 6574 5f63 6f72 652e 6361 6e76 6173  flet_core.canvas
+00000550: 2e73 6861 7065 7204 0000 00da 1266 6c65  .shaper......fle
+00000560: 745f 636f 7265 2e70 6169 6e74 696e 6772  t_core.paintingr
+00000570: 0500 0000 7206 0000 0072 0e00 0000 720e  ....r....r....r.
+00000580: 0000 0072 0e00 0000 720f 0000 00da 083c  ...r....r......<
+00000590: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
+000005a0: 1002 0c01 0c03                           ......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/line.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/line.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1869 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 4d07 0000  a........:)fM...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 4d07 0000  a........./fM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
@@ -41,123 +41,123 @@
 00000280: 0000 720e 0000 0072 0f00 0000 2907 7204  ..r....r....).r.
 00000290: 0000 00da 085f 5f69 6e69 745f 5f72 0800  .....__init__r..
 000002a0: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
 000002b0: 0072 0c00 0000 290a da04 7365 6c66 7208  .r....)...selfr.
 000002c0: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
 000002d0: 0000 720c 0000 0072 1000 0000 720d 0000  ..r....r....r...
 000002e0: 0072 0e00 0000 720f 0000 00a9 0072 1300  .r....r......r..
-000002f0: 0000 fa57 2f77 6f72 6b73 7061 6365 732f  ...W/workspaces/
+000002f0: 0000 fa5e 2f77 6f72 6b73 7061 6365 732f  ...^/workspaces/
 00000300: 636f 6e74 7269 6266 6c65 742f 666c 6574  contribflet/flet
-00000310: 2f73 646b 2f70 7974 686f 6e2f 7061 636b  /sdk/python/pack
-00000320: 6167 6573 2f66 6c65 742d 636f 7265 2f73  ages/flet-core/s
-00000330: 7263 2f66 6c65 745f 636f 7265 2f63 616e  rc/flet_core/can
-00000340: 7661 732f 6c69 6e65 2e70 7972 1100 0000  vas/line.pyr....
-00000350: 0900 0000 730c 0000 0000 0f14 0206 0106  ....s...........
-00000360: 0106 0106 017a 0d4c 696e 652e 5f5f 696e  .....z.Line.__in
-00000370: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-00000380: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-00000390: 0000 6401 5300 2902 4eda 046c 696e 6572  ..d.S.).N..liner
-000003a0: 1300 0000 a901 7212 0000 0072 1300 0000  ......r....r....
-000003b0: 7213 0000 0072 1400 0000 da11 5f67 6574  r....r......_get
-000003c0: 5f63 6f6e 7472 6f6c 5f6e 616d 6520 0000  _control_name ..
-000003d0: 0073 0200 0000 0001 7a16 4c69 6e65 2e5f  .s......z.Line._
-000003e0: 6765 745f 636f 6e74 726f 6c5f 6e61 6d65  get_control_name
-000003f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000400: 0004 0000 0003 0000 0073 1c00 0000 7400  .........s....t.
-00000410: 8300 a001 a100 0100 7c00 a002 6401 7c00  ........|...d.|.
-00000420: 6a03 a102 0100 6400 5300 2902 4e72 0c00  j.....d.S.).Nr..
-00000430: 0000 2904 da05 7375 7065 72da 0d62 6566  ..)...super..bef
-00000440: 6f72 655f 7570 6461 7465 da0e 5f73 6574  ore_update.._set
-00000450: 5f61 7474 725f 6a73 6f6e da0c 5f4c 696e  _attr_json.._Lin
-00000460: 655f 5f70 6169 6e74 7216 0000 00a9 01da  e__paintr.......
-00000470: 095f 5f63 6c61 7373 5f5f 7213 0000 0072  .__class__r....r
-00000480: 1400 0000 7219 0000 0023 0000 0073 0400  ....r....#...s..
-00000490: 0000 0001 0a01 7a12 4c69 6e65 2e62 6566  ......z.Line.bef
-000004a0: 6f72 655f 7570 6461 7465 2901 da06 7265  ore_update)...re
-000004b0: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
-000004c0: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-000004d0: 0000 7c00 a000 6401 a101 5300 a902 4e72  ..|...d...S...Nr
-000004e0: 0800 0000 a901 da09 5f67 6574 5f61 7474  ........_get_att
-000004f0: 7272 1600 0000 7213 0000 0072 1300 0000  rr....r....r....
-00000500: 7214 0000 0072 0800 0000 2800 0000 7302  r....r....(...s.
-00000510: 0000 0000 027a 074c 696e 652e 7831 2901  .....z.Line.x1).
-00000520: da05 7661 6c75 6563 0200 0000 0000 0000  ..valuec........
-00000530: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000540: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00000550: 0064 0053 0072 1f00 0000 a901 da09 5f73  .d.S.r........_s
-00000560: 6574 5f61 7474 72a9 0272 1200 0000 7222  et_attr..r....r"
-00000570: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000580: 0000 7208 0000 002c 0000 0073 0200 0000  ..r....,...s....
-00000590: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000005a0: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
-000005b0: 7c00 a000 6401 a101 5300 a902 4e72 0900  |...d...S...Nr..
-000005c0: 0000 7220 0000 0072 1600 0000 7213 0000  ..r ...r....r...
-000005d0: 0072 1300 0000 7214 0000 0072 0900 0000  .r....r....r....
-000005e0: 3100 0000 7302 0000 0000 027a 074c 696e  1...s......z.Lin
-000005f0: 652e 7931 6302 0000 0000 0000 0000 0000  e.y1c...........
-00000600: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00000610: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
-00000620: 5300 7226 0000 0072 2300 0000 7225 0000  S.r&...r#...r%..
-00000630: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000640: 7209 0000 0035 0000 0073 0200 0000 0002  r....5...s......
-00000650: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000660: 0003 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
-00000670: a000 6401 a101 5300 a902 4e72 0a00 0000  ..d...S...Nr....
-00000680: 7220 0000 0072 1600 0000 7213 0000 0072  r ...r....r....r
-00000690: 1300 0000 7214 0000 0072 0a00 0000 3a00  ....r....r....:.
-000006a0: 0000 7302 0000 0000 027a 074c 696e 652e  ..s......z.Line.
-000006b0: 7832 6302 0000 0000 0000 0000 0000 0002  x2c.............
-000006c0: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
-000006d0: 7c00 a000 6401 7c01 a102 0100 6400 5300  |...d.|.....d.S.
-000006e0: 7227 0000 0072 2300 0000 7225 0000 0072  r'...r#...r%...r
-000006f0: 1300 0000 7213 0000 0072 1400 0000 720a  ....r....r....r.
-00000700: 0000 003e 0000 0073 0200 0000 0002 6301  ...>...s......c.
-00000710: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000720: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
-00000730: 6401 a101 5300 a902 4e72 0b00 0000 7220  d...S...Nr....r 
-00000740: 0000 0072 1600 0000 7213 0000 0072 1300  ...r....r....r..
-00000750: 0000 7214 0000 0072 0b00 0000 4300 0000  ..r....r....C...
-00000760: 7302 0000 0000 027a 074c 696e 652e 7932  s......z.Line.y2
-00000770: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000780: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00000790: a000 6401 7c01 a102 0100 6400 5300 7228  ..d.|.....d.S.r(
-000007a0: 0000 0072 2300 0000 7225 0000 0072 1300  ...r#...r%...r..
-000007b0: 0000 7213 0000 0072 1400 0000 720b 0000  ..r....r....r...
-000007c0: 0047 0000 0073 0200 0000 0002 6301 0000  .G...s......c...
-000007d0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-000007e0: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-000007f0: a901 4ea9 0172 1b00 0000 7216 0000 0072  ..N..r....r....r
-00000800: 1300 0000 7213 0000 0072 1400 0000 720c  ....r....r....r.
-00000810: 0000 004c 0000 0073 0200 0000 0002 7a0a  ...L...s......z.
-00000820: 4c69 6e65 2e70 6169 6e74 6302 0000 0000  Line.paintc.....
-00000830: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000840: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
-00000850: 5300 7229 0000 0072 2a00 0000 7225 0000  S.r)...r*...r%..
-00000860: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000870: 720c 0000 0050 0000 0073 0200 0000 0002  r....P...s......
-00000880: 2909 4e4e 4e4e 4e4e 4e4e 4e29 13da 085f  ).NNNNNNNNN)..._
-00000890: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000008a0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000008b0: 5f72 0500 0000 7203 0000 0072 0600 0000  _r....r....r....
-000008c0: da04 626f 6f6c 7202 0000 0072 1100 0000  ..boolr....r....
-000008d0: 7217 0000 0072 1900 0000 da08 7072 6f70  r....r......prop
-000008e0: 6572 7479 7208 0000 00da 0673 6574 7465  ertyr......sette
-000008f0: 7272 0900 0000 720a 0000 0072 0b00 0000  rr....r....r....
-00000900: 720c 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-00000910: 6c6c 5f5f 7213 0000 0072 1300 0000 721c  ll__r....r....r.
-00000920: 0000 0072 1400 0000 7207 0000 0008 0000  ...r....r.......
-00000930: 0073 5200 0000 0803 0001 0001 0001 0001  .sR.............
-00000940: 0004 0001 0001 0001 00f3 0202 0201 0201  ................
-00000950: 0201 0201 0605 0601 0601 02f3 0c17 0803  ................
-00000960: 0c05 0201 1003 0401 1004 0201 1003 0401  ................
-00000970: 1004 0201 1003 0401 1004 0201 1003 0401  ................
-00000980: 1004 0201 1403 0401 7207 0000 004e 290a  ........r....N).
-00000990: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-000009a0: 0000 da16 666c 6574 5f63 6f72 652e 6361  ....flet_core.ca
-000009b0: 6e76 6173 2e73 6861 7065 7204 0000 00da  nvas.shaper.....
-000009c0: 1166 6c65 745f 636f 7265 2e63 6f6e 7472  .flet_core.contr
-000009d0: 6f6c 7205 0000 00da 1266 6c65 745f 636f  olr......flet_co
-000009e0: 7265 2e70 6169 6e74 696e 6772 0600 0000  re.paintingr....
-000009f0: 7207 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-00000a00: 1300 0000 7214 0000 00da 083c 6d6f 6475  ....r......<modu
-00000a10: 6c65 3e01 0000 0073 0800 0000 1002 0c01  le>....s........
-00000a20: 0c01 0c03                                ....
+00000310: 636f 6e74 7269 622f 7364 6b2f 7079 7468  contrib/sdk/pyth
+00000320: 6f6e 2f70 6163 6b61 6765 732f 666c 6574  on/packages/flet
+00000330: 2d63 6f72 652f 7372 632f 666c 6574 5f63  -core/src/flet_c
+00000340: 6f72 652f 6361 6e76 6173 2f6c 696e 652e  ore/canvas/line.
+00000350: 7079 7211 0000 0009 0000 0073 0c00 0000  pyr........s....
+00000360: 000f 1402 0601 0601 0601 0601 7a0d 4c69  ............z.Li
+00000370: 6e65 2e5f 5f69 6e69 745f 5f63 0100 0000  ne.__init__c....
+00000380: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000390: 4300 0000 7304 0000 0064 0153 0029 024e  C...s....d.S.).N
+000003a0: da04 6c69 6e65 7213 0000 00a9 0172 1200  ..liner......r..
+000003b0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+000003c0: 00da 115f 6765 745f 636f 6e74 726f 6c5f  ..._get_control_
+000003d0: 6e61 6d65 2000 0000 7302 0000 0000 017a  name ...s......z
+000003e0: 164c 696e 652e 5f67 6574 5f63 6f6e 7472  .Line._get_contr
+000003f0: 6f6c 5f6e 616d 6563 0100 0000 0000 0000  ol_namec........
+00000400: 0000 0000 0100 0000 0400 0000 0300 0000  ................
+00000410: 731c 0000 0074 0083 00a0 01a1 0001 007c  s....t.........|
+00000420: 00a0 0264 017c 006a 03a1 0201 0064 0053  ...d.|.j.....d.S
+00000430: 0029 024e 720c 0000 0029 04da 0573 7570  .).Nr....)...sup
+00000440: 6572 da0d 6265 666f 7265 5f75 7064 6174  er..before_updat
+00000450: 65da 0e5f 7365 745f 6174 7472 5f6a 736f  e.._set_attr_jso
+00000460: 6eda 0c5f 4c69 6e65 5f5f 7061 696e 7472  n.._Line__paintr
+00000470: 1600 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+00000480: 5f72 1300 0000 7214 0000 0072 1900 0000  _r....r....r....
+00000490: 2300 0000 7304 0000 0000 010a 017a 124c  #...s........z.L
+000004a0: 696e 652e 6265 666f 7265 5f75 7064 6174  ine.before_updat
+000004b0: 6529 01da 0672 6574 7572 6e63 0100 0000  e)...returnc....
+000004c0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000004d0: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
+000004e0: 0153 00a9 024e 7208 0000 00a9 01da 095f  .S...Nr........_
+000004f0: 6765 745f 6174 7472 7216 0000 0072 1300  get_attrr....r..
+00000500: 0000 7213 0000 0072 1400 0000 7208 0000  ..r....r....r...
+00000510: 0028 0000 0073 0200 0000 0002 7a07 4c69  .(...s......z.Li
+00000520: 6e65 2e78 3129 01da 0576 616c 7565 6302  ne.x1)...valuec.
+00000530: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000540: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00000550: 6401 7c01 a102 0100 6400 5300 721f 0000  d.|.....d.S.r...
+00000560: 00a9 01da 095f 7365 745f 6174 7472 a902  ....._set_attr..
+00000570: 7212 0000 0072 2200 0000 7213 0000 0072  r....r"...r....r
+00000580: 1300 0000 7214 0000 0072 0800 0000 2c00  ....r....r....,.
+00000590: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
+000005a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000005b0: 0000 730a 0000 007c 00a0 0064 01a1 0153  ..s....|...d...S
+000005c0: 00a9 024e 7209 0000 0072 2000 0000 7216  ...Nr....r ...r.
+000005d0: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+000005e0: 0000 7209 0000 0031 0000 0073 0200 0000  ..r....1...s....
+000005f0: 0002 7a07 4c69 6e65 2e79 3163 0200 0000  ..z.Line.y1c....
+00000600: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000610: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
+00000620: 01a1 0201 0064 0053 0072 2600 0000 7223  .....d.S.r&...r#
+00000630: 0000 0072 2500 0000 7213 0000 0072 1300  ...r%...r....r..
+00000640: 0000 7214 0000 0072 0900 0000 3500 0000  ..r....r....5...
+00000650: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00000660: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00000670: 730a 0000 007c 00a0 0064 01a1 0153 00a9  s....|...d...S..
+00000680: 024e 720a 0000 0072 2000 0000 7216 0000  .Nr....r ...r...
+00000690: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+000006a0: 720a 0000 003a 0000 0073 0200 0000 0002  r....:...s......
+000006b0: 7a07 4c69 6e65 2e78 3263 0200 0000 0000  z.Line.x2c......
+000006c0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+000006d0: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
+000006e0: 0201 0064 0053 0072 2700 0000 7223 0000  ...d.S.r'...r#..
+000006f0: 0072 2500 0000 7213 0000 0072 1300 0000  .r%...r....r....
+00000700: 7214 0000 0072 0a00 0000 3e00 0000 7302  r....r....>...s.
+00000710: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00000720: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
+00000730: 0000 007c 00a0 0064 01a1 0153 00a9 024e  ...|...d...S...N
+00000740: 720b 0000 0072 2000 0000 7216 0000 0072  r....r ...r....r
+00000750: 1300 0000 7213 0000 0072 1400 0000 720b  ....r....r....r.
+00000760: 0000 0043 0000 0073 0200 0000 0002 7a07  ...C...s......z.
+00000770: 4c69 6e65 2e79 3263 0200 0000 0000 0000  Line.y2c........
+00000780: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000790: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
+000007a0: 0064 0053 0072 2800 0000 7223 0000 0072  .d.S.r(...r#...r
+000007b0: 2500 0000 7213 0000 0072 1300 0000 7214  %...r....r....r.
+000007c0: 0000 0072 0b00 0000 4700 0000 7302 0000  ...r....G...s...
+000007d0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+000007e0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+000007f0: 007c 006a 0053 00a9 014e a901 721b 0000  .|.j.S...N..r...
+00000800: 0072 1600 0000 7213 0000 0072 1300 0000  .r....r....r....
+00000810: 7214 0000 0072 0c00 0000 4c00 0000 7302  r....r....L...s.
+00000820: 0000 0000 027a 0a4c 696e 652e 7061 696e  .....z.Line.pain
+00000830: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00000840: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
+00000850: 017c 005f 0064 0053 0072 2900 0000 722a  .|._.d.S.r)...r*
+00000860: 0000 0072 2500 0000 7213 0000 0072 1300  ...r%...r....r..
+00000870: 0000 7214 0000 0072 0c00 0000 5000 0000  ..r....r....P...
+00000880: 7302 0000 0000 0229 094e 4e4e 4e4e 4e4e  s......).NNNNNNN
+00000890: 4e4e 2913 da08 5f5f 6e61 6d65 5f5f da0a  NN)...__name__..
+000008a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000008b0: 616c 6e61 6d65 5f5f 7205 0000 0072 0300  alname__r....r..
+000008c0: 0000 7206 0000 00da 0462 6f6f 6c72 0200  ..r......boolr..
+000008d0: 0000 7211 0000 0072 1700 0000 7219 0000  ..r....r....r...
+000008e0: 00da 0870 726f 7065 7274 7972 0800 0000  ...propertyr....
+000008f0: da06 7365 7474 6572 7209 0000 0072 0a00  ..setterr....r..
+00000900: 0000 720b 0000 0072 0c00 0000 da0d 5f5f  ..r....r......__
+00000910: 636c 6173 7363 656c 6c5f 5f72 1300 0000  classcell__r....
+00000920: 7213 0000 0072 1c00 0000 7214 0000 0072  r....r....r....r
+00000930: 0700 0000 0800 0000 7352 0000 0008 0300  ........sR......
+00000940: 0100 0100 0100 0100 0400 0100 0100 0100  ................
+00000950: f302 0202 0102 0102 0102 0106 0506 0106  ................
+00000960: 0102 f30c 1708 030c 0502 0110 0304 0110  ................
+00000970: 0402 0110 0304 0110 0402 0110 0304 0110  ................
+00000980: 0402 0110 0304 0110 0402 0114 0304 0172  ...............r
+00000990: 0700 0000 4e29 0ada 0674 7970 696e 6772  ....N)...typingr
+000009a0: 0200 0000 7203 0000 00da 1666 6c65 745f  ....r......flet_
+000009b0: 636f 7265 2e63 616e 7661 732e 7368 6170  core.canvas.shap
+000009c0: 6572 0400 0000 da11 666c 6574 5f63 6f72  er......flet_cor
+000009d0: 652e 636f 6e74 726f 6c72 0500 0000 da12  e.controlr......
+000009e0: 666c 6574 5f63 6f72 652e 7061 696e 7469  flet_core.painti
+000009f0: 6e67 7206 0000 0072 0700 0000 7213 0000  ngr....r....r...
+00000a00: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000a10: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
+00000a20: 0000 0010 020c 010c 010c 03              ...........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1891 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 6307 0000  a........:)fc...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 6307 0000  a........./fc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
@@ -41,123 +41,124 @@
 00000280: 6566 720d 0000 0072 0e00 0000 720f 0000  efr....r....r...
 00000290: 0029 0772 0400 0000 da08 5f5f 696e 6974  .).r......__init
 000002a0: 5f5f 7208 0000 0072 0900 0000 720a 0000  __r....r....r...
 000002b0: 0072 0b00 0000 720c 0000 0029 0ada 0473  .r....r....)...s
 000002c0: 656c 6672 0800 0000 7209 0000 0072 0a00  elfr....r....r..
 000002d0: 0000 720b 0000 0072 0c00 0000 7210 0000  ..r....r....r...
 000002e0: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000002f0: a900 7213 0000 00fa 572f 776f 726b 7370  ..r.....W/worksp
+000002f0: a900 7213 0000 00fa 5e2f 776f 726b 7370  ..r.....^/worksp
 00000300: 6163 6573 2f63 6f6e 7472 6962 666c 6574  aces/contribflet
-00000310: 2f66 6c65 742f 7364 6b2f 7079 7468 6f6e  /flet/sdk/python
-00000320: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
-00000330: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
-00000340: 652f 6361 6e76 6173 2f6f 7661 6c2e 7079  e/canvas/oval.py
-00000350: 7211 0000 0009 0000 0073 0c00 0000 000d  r........s......
-00000360: 1402 0601 0601 0601 0601 7a0d 4f76 616c  ..........z.Oval
-00000370: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000380: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00000390: 0000 7304 0000 0064 0153 0029 024e 5a04  ..s....d.S.).NZ.
-000003a0: 6f76 616c 7213 0000 00a9 0172 1200 0000  ovalr......r....
-000003b0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000003c0: 115f 6765 745f 636f 6e74 726f 6c5f 6e61  ._get_control_na
-000003d0: 6d65 1e00 0000 7302 0000 0000 017a 164f  me....s......z.O
-000003e0: 7661 6c2e 5f67 6574 5f63 6f6e 7472 6f6c  val._get_control
-000003f0: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
-00000400: 0000 0100 0000 0400 0000 0300 0000 731c  ..............s.
-00000410: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
-00000420: 0264 017c 006a 03a1 0201 0064 0053 0029  .d.|.j.....d.S.)
-00000430: 024e 720c 0000 0029 04da 0573 7570 6572  .Nr....)...super
-00000440: da0d 6265 666f 7265 5f75 7064 6174 65da  ..before_update.
-00000450: 0e5f 7365 745f 6174 7472 5f6a 736f 6eda  ._set_attr_json.
-00000460: 0c5f 4f76 616c 5f5f 7061 696e 7472 1500  ._Oval__paintr..
-00000470: 0000 a901 da09 5f5f 636c 6173 735f 5f72  ......__class__r
-00000480: 1300 0000 7214 0000 0072 1800 0000 2100  ....r....r....!.
-00000490: 0000 7304 0000 0000 010a 017a 124f 7661  ..s........z.Ova
-000004a0: 6c2e 6265 666f 7265 5f75 7064 6174 6529  l.before_update)
-000004b0: 01da 0672 6574 7572 6e63 0100 0000 0000  ...returnc......
-000004c0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000004d0: 0000 730a 0000 007c 00a0 0064 01a1 0153  ..s....|...d...S
-000004e0: 00a9 024e 7208 0000 00a9 01da 095f 6765  ...Nr........_ge
-000004f0: 745f 6174 7472 7215 0000 0072 1300 0000  t_attrr....r....
-00000500: 7213 0000 0072 1400 0000 7208 0000 0026  r....r....r....&
-00000510: 0000 0073 0200 0000 0002 7a06 4f76 616c  ...s......z.Oval
-00000520: 2e78 2901 da05 7661 6c75 6563 0200 0000  .x)...valuec....
-00000530: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000540: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
-00000550: 01a1 0201 0064 0053 0072 1e00 0000 a901  .....d.S.r......
-00000560: da09 5f73 6574 5f61 7474 72a9 0272 1200  .._set_attr..r..
-00000570: 0000 7221 0000 0072 1300 0000 7213 0000  ..r!...r....r...
-00000580: 0072 1400 0000 7208 0000 002a 0000 0073  .r....r....*...s
-00000590: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-000005a0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000005b0: 0a00 0000 7c00 a000 6401 a101 5300 a902  ....|...d...S...
-000005c0: 4e72 0900 0000 721f 0000 0072 1500 0000  Nr....r....r....
-000005d0: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-000005e0: 0900 0000 2f00 0000 7302 0000 0000 027a  ..../...s......z
-000005f0: 064f 7661 6c2e 7963 0200 0000 0000 0000  .Oval.yc........
-00000600: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000610: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00000620: 0064 0053 0072 2500 0000 7222 0000 0072  .d.S.r%...r"...r
-00000630: 2400 0000 7213 0000 0072 1300 0000 7214  $...r....r....r.
-00000640: 0000 0072 0900 0000 3300 0000 7302 0000  ...r....3...s...
-00000650: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-00000660: 0100 0000 0300 0000 4300 0000 730a 0000  ........C...s...
-00000670: 007c 00a0 0064 01a1 0153 00a9 024e 720a  .|...d...S...Nr.
-00000680: 0000 0072 1f00 0000 7215 0000 0072 1300  ...r....r....r..
-00000690: 0000 7213 0000 0072 1400 0000 720a 0000  ..r....r....r...
-000006a0: 0038 0000 0073 0200 0000 0002 7a0a 4f76  .8...s......z.Ov
-000006b0: 616c 2e77 6964 7468 6302 0000 0000 0000  al.widthc.......
-000006c0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000006d0: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
-000006e0: 0100 6400 5300 7226 0000 0072 2200 0000  ..d.S.r&...r"...
-000006f0: 7224 0000 0072 1300 0000 7213 0000 0072  r$...r....r....r
-00000700: 1400 0000 720a 0000 003c 0000 0073 0200  ....r....<...s..
-00000710: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000720: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-00000730: 0000 7c00 a000 6401 a101 5300 a902 4e72  ..|...d...S...Nr
-00000740: 0b00 0000 721f 0000 0072 1500 0000 7213  ....r....r....r.
-00000750: 0000 0072 1300 0000 7214 0000 0072 0b00  ...r....r....r..
-00000760: 0000 4100 0000 7302 0000 0000 027a 0b4f  ..A...s......z.O
-00000770: 7661 6c2e 6865 6967 6874 6302 0000 0000  val.heightc.....
-00000780: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000790: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
-000007a0: a102 0100 6400 5300 7227 0000 0072 2200  ....d.S.r'...r".
-000007b0: 0000 7224 0000 0072 1300 0000 7213 0000  ..r$...r....r...
-000007c0: 0072 1400 0000 720b 0000 0045 0000 0073  .r....r....E...s
-000007d0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-000007e0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-000007f0: 0600 0000 7c00 6a00 5300 a901 4ea9 0172  ....|.j.S...N..r
-00000800: 1a00 0000 7215 0000 0072 1300 0000 7213  ....r....r....r.
-00000810: 0000 0072 1400 0000 720c 0000 004a 0000  ...r....r....J..
-00000820: 0073 0200 0000 0002 7a0a 4f76 616c 2e70  .s......z.Oval.p
-00000830: 6169 6e74 6302 0000 0000 0000 0000 0000  aintc...........
-00000840: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00000850: 0000 7c01 7c00 5f00 6400 5300 7228 0000  ..|.|._.d.S.r(..
-00000860: 0072 2900 0000 7224 0000 0072 1300 0000  .r)...r$...r....
-00000870: 7213 0000 0072 1400 0000 720c 0000 004e  r....r....r....N
-00000880: 0000 0073 0200 0000 0002 2909 4e4e 4e4e  ...s......).NNNN
-00000890: 4e4e 4e4e 4e29 13da 085f 5f6e 616d 655f  NNNNN)...__name_
-000008a0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000008b0: 5f71 7561 6c6e 616d 655f 5f72 0500 0000  _qualname__r....
-000008c0: 7203 0000 0072 0600 0000 da04 626f 6f6c  r....r......bool
-000008d0: 7202 0000 0072 1100 0000 7216 0000 0072  r....r....r....r
-000008e0: 1800 0000 da08 7072 6f70 6572 7479 7208  ......propertyr.
-000008f0: 0000 00da 0673 6574 7465 7272 0900 0000  .....setterr....
-00000900: 720a 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00000910: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7213  .__classcell__r.
-00000920: 0000 0072 1300 0000 721b 0000 0072 1400  ...r....r....r..
-00000930: 0000 7207 0000 0008 0000 0073 5200 0000  ..r........sR...
-00000940: 0803 0001 0001 0001 0001 0002 0001 0001  ................
-00000950: 0001 00f5 0202 0201 0201 0201 0201 0603  ................
-00000960: 0601 0601 02f5 0c15 0803 0c05 0201 1003  ................
-00000970: 0401 1004 0201 1003 0401 1004 0201 1003  ................
-00000980: 0401 1004 0201 1003 0401 1004 0201 1403  ................
-00000990: 0401 7207 0000 004e 290a da06 7479 7069  ..r....N)...typi
-000009a0: 6e67 7202 0000 0072 0300 0000 da16 666c  ngr....r......fl
-000009b0: 6574 5f63 6f72 652e 6361 6e76 6173 2e73  et_core.canvas.s
-000009c0: 6861 7065 7204 0000 00da 1166 6c65 745f  haper......flet_
-000009d0: 636f 7265 2e63 6f6e 7472 6f6c 7205 0000  core.controlr...
-000009e0: 00da 1266 6c65 745f 636f 7265 2e70 6169  ...flet_core.pai
-000009f0: 6e74 696e 6772 0600 0000 7207 0000 0072  ntingr....r....r
-00000a00: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-00000a10: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000a20: 0073 0800 0000 1002 0c01 0c01 0c03       .s............
+00000310: 2f66 6c65 7463 6f6e 7472 6962 2f73 646b  /fletcontrib/sdk
+00000320: 2f70 7974 686f 6e2f 7061 636b 6167 6573  /python/packages
+00000330: 2f66 6c65 742d 636f 7265 2f73 7263 2f66  /flet-core/src/f
+00000340: 6c65 745f 636f 7265 2f63 616e 7661 732f  let_core/canvas/
+00000350: 6f76 616c 2e70 7972 1100 0000 0900 0000  oval.pyr........
+00000360: 730c 0000 0000 0d14 0206 0106 0106 0106  s...............
+00000370: 017a 0d4f 7661 6c2e 5f5f 696e 6974 5f5f  .z.Oval.__init__
+00000380: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000390: 0001 0000 0043 0000 0073 0400 0000 6401  .....C...s....d.
+000003a0: 5300 2902 4e5a 046f 7661 6c72 1300 0000  S.).NZ.ovalr....
+000003b0: a901 7212 0000 0072 1300 0000 7213 0000  ..r....r....r...
+000003c0: 0072 1400 0000 da11 5f67 6574 5f63 6f6e  .r......_get_con
+000003d0: 7472 6f6c 5f6e 616d 651e 0000 0073 0200  trol_name....s..
+000003e0: 0000 0001 7a16 4f76 616c 2e5f 6765 745f  ....z.Oval._get_
+000003f0: 636f 6e74 726f 6c5f 6e61 6d65 6301 0000  control_namec...
+00000400: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000410: 0003 0000 0073 1c00 0000 7400 8300 a001  .....s....t.....
+00000420: a100 0100 7c00 a002 6401 7c00 6a03 a102  ....|...d.|.j...
+00000430: 0100 6400 5300 2902 4e72 0c00 0000 2904  ..d.S.).Nr....).
+00000440: da05 7375 7065 72da 0d62 6566 6f72 655f  ..super..before_
+00000450: 7570 6461 7465 da0e 5f73 6574 5f61 7474  update.._set_att
+00000460: 725f 6a73 6f6e da0c 5f4f 7661 6c5f 5f70  r_json.._Oval__p
+00000470: 6169 6e74 7215 0000 00a9 01da 095f 5f63  aintr........__c
+00000480: 6c61 7373 5f5f 7213 0000 0072 1400 0000  lass__r....r....
+00000490: 7218 0000 0021 0000 0073 0400 0000 0001  r....!...s......
+000004a0: 0a01 7a12 4f76 616c 2e62 6566 6f72 655f  ..z.Oval.before_
+000004b0: 7570 6461 7465 2901 da06 7265 7475 726e  update)...return
+000004c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000004d0: 0003 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
+000004e0: a000 6401 a101 5300 a902 4e72 0800 0000  ..d...S...Nr....
+000004f0: a901 da09 5f67 6574 5f61 7474 7272 1500  ...._get_attrr..
+00000500: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000510: 0072 0800 0000 2600 0000 7302 0000 0000  .r....&...s.....
+00000520: 027a 064f 7661 6c2e 7829 01da 0576 616c  .z.Oval.x)...val
+00000530: 7565 6302 0000 0000 0000 0000 0000 0002  uec.............
+00000540: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
+00000550: 7c00 a000 6401 7c01 a102 0100 6400 5300  |...d.|.....d.S.
+00000560: 721e 0000 00a9 01da 095f 7365 745f 6174  r........_set_at
+00000570: 7472 a902 7212 0000 0072 2100 0000 7213  tr..r....r!...r.
+00000580: 0000 0072 1300 0000 7214 0000 0072 0800  ...r....r....r..
+00000590: 0000 2a00 0000 7302 0000 0000 0263 0100  ..*...s......c..
+000005a0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000005b0: 0000 4300 0000 730a 0000 007c 00a0 0064  ..C...s....|...d
+000005c0: 01a1 0153 00a9 024e 7209 0000 0072 1f00  ...S...Nr....r..
+000005d0: 0000 7215 0000 0072 1300 0000 7213 0000  ..r....r....r...
+000005e0: 0072 1400 0000 7209 0000 002f 0000 0073  .r....r..../...s
+000005f0: 0200 0000 0002 7a06 4f76 616c 2e79 6302  ......z.Oval.yc.
+00000600: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000610: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00000620: 6401 7c01 a102 0100 6400 5300 7225 0000  d.|.....d.S.r%..
+00000630: 0072 2200 0000 7224 0000 0072 1300 0000  .r"...r$...r....
+00000640: 7213 0000 0072 1400 0000 7209 0000 0033  r....r....r....3
+00000650: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+00000660: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000670: 0000 0073 0a00 0000 7c00 a000 6401 a101  ...s....|...d...
+00000680: 5300 a902 4e72 0a00 0000 721f 0000 0072  S...Nr....r....r
+00000690: 1500 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+000006a0: 0000 0072 0a00 0000 3800 0000 7302 0000  ...r....8...s...
+000006b0: 0000 027a 0a4f 7661 6c2e 7769 6474 6863  ...z.Oval.widthc
+000006c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000006d0: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+000006e0: 0064 017c 01a1 0201 0064 0053 0072 2600  .d.|.....d.S.r&.
+000006f0: 0000 7222 0000 0072 2400 0000 7213 0000  ..r"...r$...r...
+00000700: 0072 1300 0000 7214 0000 0072 0a00 0000  .r....r....r....
+00000710: 3c00 0000 7302 0000 0000 0263 0100 0000  <...s......c....
+00000720: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000730: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
+00000740: 0153 00a9 024e 720b 0000 0072 1f00 0000  .S...Nr....r....
+00000750: 7215 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00000760: 1400 0000 720b 0000 0041 0000 0073 0200  ....r....A...s..
+00000770: 0000 0002 7a0b 4f76 616c 2e68 6569 6768  ....z.Oval.heigh
+00000780: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00000790: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
+000007a0: 00a0 0064 017c 01a1 0201 0064 0053 0072  ...d.|.....d.S.r
+000007b0: 2700 0000 7222 0000 0072 2400 0000 7213  '...r"...r$...r.
+000007c0: 0000 0072 1300 0000 7214 0000 0072 0b00  ...r....r....r..
+000007d0: 0000 4500 0000 7302 0000 0000 0263 0100  ..E...s......c..
+000007e0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000007f0: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00000800: 00a9 014e a901 721a 0000 0072 1500 0000  ...N..r....r....
+00000810: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000820: 0c00 0000 4a00 0000 7302 0000 0000 027a  ....J...s......z
+00000830: 0a4f 7661 6c2e 7061 696e 7463 0200 0000  .Oval.paintc....
+00000840: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000850: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+00000860: 0053 0072 2800 0000 7229 0000 0072 2400  .S.r(...r)...r$.
+00000870: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000880: 0072 0c00 0000 4e00 0000 7302 0000 0000  .r....N...s.....
+00000890: 0229 094e 4e4e 4e4e 4e4e 4e4e 2913 da08  .).NNNNNNNNN)...
+000008a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000008b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000008c0: 5f5f 7205 0000 0072 0300 0000 7206 0000  __r....r....r...
+000008d0: 00da 0462 6f6f 6c72 0200 0000 7211 0000  ...boolr....r...
+000008e0: 0072 1600 0000 7218 0000 00da 0870 726f  .r....r......pro
+000008f0: 7065 7274 7972 0800 0000 da06 7365 7474  pertyr......sett
+00000900: 6572 7209 0000 0072 0a00 0000 720b 0000  err....r....r...
+00000910: 0072 0c00 0000 da0d 5f5f 636c 6173 7363  .r......__classc
+00000920: 656c 6c5f 5f72 1300 0000 7213 0000 0072  ell__r....r....r
+00000930: 1b00 0000 7214 0000 0072 0700 0000 0800  ....r....r......
+00000940: 0000 7352 0000 0008 0300 0100 0100 0100  ..sR............
+00000950: 0100 0200 0100 0100 0100 f502 0202 0102  ................
+00000960: 0102 0102 0106 0306 0106 0102 f50c 1508  ................
+00000970: 030c 0502 0110 0304 0110 0402 0110 0304  ................
+00000980: 0110 0402 0110 0304 0110 0402 0110 0304  ................
+00000990: 0110 0402 0114 0304 0172 0700 0000 4e29  .........r....N)
+000009a0: 0ada 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
+000009b0: 0000 00da 1666 6c65 745f 636f 7265 2e63  .....flet_core.c
+000009c0: 616e 7661 732e 7368 6170 6572 0400 0000  anvas.shaper....
+000009d0: da11 666c 6574 5f63 6f72 652e 636f 6e74  ..flet_core.cont
+000009e0: 726f 6c72 0500 0000 da12 666c 6574 5f63  rolr......flet_c
+000009f0: 6f72 652e 7061 696e 7469 6e67 7206 0000  ore.paintingr...
+00000a00: 0072 0700 0000 7213 0000 0072 1300 0000  .r....r....r....
+00000a10: 7213 0000 0072 1400 0000 da08 3c6d 6f64  r....r......<mod
+00000a20: 756c 653e 0100 0000 7308 0000 0010 020c  ule>....s.......
+00000a30: 010c 010c 03                             .....
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/path.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/path.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 3493 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 a50d 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 a50d 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 6506 8303 5a0b 6401  d.d...d.e...Z.d.
@@ -41,264 +41,264 @@
 00000280: 5061 7468 6300 0000 0000 0000 0000 0000  Pathc...........
 00000290: 0000 0000 0001 0000 0040 0000 0073 0c00  .........@...s..
 000002a0: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
 000002b0: fa10 5061 7468 2e50 6174 6845 6c65 6d65  ..Path.PathEleme
 000002c0: 6e74 4e29 03da 085f 5f6e 616d 655f 5fda  ntN)...__name__.
 000002d0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 000002e0: 7561 6c6e 616d 655f 5fa9 0072 0d00 0000  ualname__..r....
-000002f0: 720d 0000 00fa 572f 776f 726b 7370 6163  r.....W/workspac
+000002f0: 720d 0000 00fa 5e2f 776f 726b 7370 6163  r.....^/workspac
 00000300: 6573 2f63 6f6e 7472 6962 666c 6574 2f66  es/contribflet/f
-00000310: 6c65 742f 7364 6b2f 7079 7468 6f6e 2f70  let/sdk/python/p
-00000320: 6163 6b61 6765 732f 666c 6574 2d63 6f72  ackages/flet-cor
-00000330: 652f 7372 632f 666c 6574 5f63 6f72 652f  e/src/flet_core/
-00000340: 6361 6e76 6173 2f70 6174 682e 7079 da0b  canvas/path.py..
-00000350: 5061 7468 456c 656d 656e 740a 0000 0073  PathElement....s
-00000360: 0200 0000 0802 720f 0000 0063 0000 0000  ......r....c....
-00000370: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000380: 4000 0000 7332 0000 0065 005a 0164 005a  @...s2...e.Z.d.Z
-00000390: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
-000003a0: 023c 0065 056a 0664 0364 048d 015a 0765  .<.e.j.d.d...Z.e
-000003b0: 0865 0464 053c 0064 0653 0029 077a 0b50  .e.d.<.d.S.).z.P
-000003c0: 6174 682e 4d6f 7665 546f da01 78da 0179  ath.MoveTo..x..y
-000003d0: 5a06 6d6f 7665 746f a901 da07 6465 6661  Z.moveto....defa
-000003e0: 756c 74da 0474 7970 654e a909 720a 0000  ult..typeN..r...
-000003f0: 0072 0b00 0000 720c 0000 00da 0566 6c6f  .r....r......flo
-00000400: 6174 da0f 5f5f 616e 6e6f 7461 7469 6f6e  at..__annotation
-00000410: 735f 5fda 0b64 6174 6163 6c61 7373 6573  s__..dataclasses
-00000420: da05 6669 656c 6472 1400 0000 da03 7374  ..fieldr......st
-00000430: 7272 0d00 0000 720d 0000 0072 0d00 0000  rr....r....r....
-00000440: 720e 0000 00da 064d 6f76 6554 6f0e 0000  r......MoveTo...
-00000450: 0073 0600 0000 0a02 0801 0801 721b 0000  .s..........r...
-00000460: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000470: 0000 0300 0000 4000 0000 7332 0000 0065  ......@...s2...e
-00000480: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
-00000490: 0065 0365 0464 023c 0065 056a 0664 0364  .e.e.d.<.e.j.d.d
-000004a0: 048d 015a 0765 0865 0464 053c 0064 0653  ...Z.e.e.d.<.d.S
-000004b0: 0029 077a 0b50 6174 682e 4c69 6e65 546f  .).z.Path.LineTo
-000004c0: 7210 0000 0072 1100 0000 5a06 6c69 6e65  r....r....Z.line
-000004d0: 746f 7212 0000 0072 1400 0000 4e72 1500  tor....r....Nr..
-000004e0: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000004f0: 0072 0e00 0000 da06 4c69 6e65 546f 1400  .r......LineTo..
-00000500: 0000 7306 0000 000a 0208 0108 0172 1c00  ..s..........r..
-00000510: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000520: 0000 0003 0000 0040 0000 0073 5600 0000  .......@...sV...
-00000530: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00000540: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
-00000550: 3c00 6503 6504 6404 3c00 6505 6a06 6405  <.e.e.d.<.e.j.d.
-00000560: 6406 8d01 5a07 6503 6504 6407 3c00 6505  d...Z.e.e.d.<.e.
-00000570: 6a06 6408 6406 8d01 5a08 6509 6504 6409  j.d.d...Z.e.e.d.
-00000580: 3c00 640a 5300 290b 7a10 5061 7468 2e51  <.d.S.).z.Path.Q
-00000590: 7561 6472 6174 6963 546f da04 6370 3178  uadraticTo..cp1x
-000005a0: da04 6370 3179 7210 0000 0072 1100 0000  ..cp1yr....r....
-000005b0: e901 0000 0072 1200 0000 da01 775a 0763  .....r......wZ.c
-000005c0: 6f6e 6963 746f 7214 0000 004e 290a 720a  onictor....N).r.
-000005d0: 0000 0072 0b00 0000 720c 0000 0072 1600  ...r....r....r..
-000005e0: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000005f0: 0072 2000 0000 7214 0000 0072 1a00 0000  .r ...r....r....
-00000600: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000610: 0e00 0000 da0b 5175 6164 7261 7469 6354  ......QuadraticT
-00000620: 6f1a 0000 0073 0c00 0000 0a02 0801 0801  o....s..........
-00000630: 0801 0801 1401 7221 0000 0063 0000 0000  ......r!...c....
-00000640: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000650: 4000 0000 7352 0000 0065 005a 0164 005a  @...sR...e.Z.d.Z
-00000660: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
-00000670: 023c 0065 0365 0464 033c 0065 0365 0464  .<.e.e.d.<.e.e.d
-00000680: 043c 0065 0365 0464 053c 0065 0365 0464  .<.e.e.d.<.e.e.d
-00000690: 063c 0065 056a 0664 0764 088d 015a 0765  .<.e.j.d.d...Z.e
-000006a0: 0865 0464 093c 0064 0a53 0029 0b7a 0c50  .e.d.<.d.S.).z.P
-000006b0: 6174 682e 4375 6269 6354 6f72 1d00 0000  ath.CubicTor....
-000006c0: 721e 0000 005a 0463 7032 785a 0463 7032  r....Z.cp2xZ.cp2
-000006d0: 7972 1000 0000 7211 0000 005a 0763 7562  yr....r....Z.cub
-000006e0: 6963 746f 7212 0000 0072 1400 0000 4e72  ictor....r....Nr
-000006f0: 1500 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
-00000700: 0000 0072 0e00 0000 da07 4375 6269 6354  ...r......CubicT
-00000710: 6f23 0000 0073 0e00 0000 0a02 0801 0801  o#...s..........
-00000720: 0801 0801 0801 0801 7222 0000 0063 0000  ........r"...c..
-00000730: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000740: 0000 4000 0000 733e 0000 0065 005a 0164  ..@...s>...e.Z.d
-00000750: 005a 0255 0065 0364 0119 0065 0464 023c  .Z.U.e.d...e.d.<
-00000760: 0065 0565 0464 033c 0065 0565 0464 043c  .e.e.d.<.e.e.d.<
-00000770: 0065 066a 0764 0564 068d 015a 0865 0965  .e.j.d.d...Z.e.e
-00000780: 0464 073c 0064 0853 0029 097a 0c50 6174  .d.<.d.S.).z.Pat
-00000790: 682e 5375 6250 6174 6872 0900 0000 da08  h.SubPathr......
-000007a0: 656c 656d 656e 7473 7210 0000 0072 1100  elementsr....r..
-000007b0: 0000 5a07 7375 6270 6174 6872 1200 0000  ..Z.subpathr....
-000007c0: 7214 0000 004e 290a 720a 0000 0072 0b00  r....N).r....r..
-000007d0: 0000 720c 0000 0072 0300 0000 7217 0000  ..r....r....r...
-000007e0: 0072 1600 0000 7218 0000 0072 1900 0000  .r....r....r....
-000007f0: 7214 0000 0072 1a00 0000 720d 0000 0072  r....r....r....r
-00000800: 0d00 0000 720d 0000 0072 0e00 0000 da07  ....r....r......
-00000810: 5375 6250 6174 682d 0000 0073 0800 0000  SubPath-...s....
-00000820: 0a02 0c01 0801 0801 7224 0000 0063 0000  ........r$...c..
-00000830: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000840: 0000 4000 0000 7352 0000 0065 005a 0164  ..@...sR...e.Z.d
-00000850: 005a 0255 0065 0365 0464 013c 0065 0365  .Z.U.e.e.d.<.e.e
-00000860: 0464 023c 0065 0365 0464 033c 0065 0365  .d.<.e.e.d.<.e.e
-00000870: 0464 043c 0065 0365 0464 053c 0065 0365  .d.<.e.e.d.<.e.e
-00000880: 0464 063c 0065 056a 0664 0764 088d 015a  .d.<.e.j.d.d...Z
-00000890: 0765 0865 0464 093c 0064 0a53 0029 0b7a  .e.e.d.<.d.S.).z
-000008a0: 0850 6174 682e 4172 6372 1000 0000 7211  .Path.Arcr....r.
-000008b0: 0000 00da 0577 6964 7468 da06 6865 6967  .....width..heig
-000008c0: 6874 da0b 7374 6172 745f 616e 676c 65da  ht..start_angle.
-000008d0: 0b73 7765 6570 5f61 6e67 6c65 da03 6172  .sweep_angle..ar
-000008e0: 6372 1200 0000 7214 0000 004e 7215 0000  cr....r....Nr...
-000008f0: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000900: 720e 0000 00da 0341 7263 3400 0000 730e  r......Arc4...s.
-00000910: 0000 000a 0208 0108 0108 0108 0108 0108  ................
-00000920: 0172 2a00 0000 6300 0000 0000 0000 0000  .r*...c.........
-00000930: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-00000940: 8200 0000 6500 5a01 6400 5a02 5500 6503  ....e.Z.d.Z.U.e.
-00000950: 6504 6401 3c00 6503 6504 6402 3c00 6505  e.d.<.e.e.d.<.e.
-00000960: 6a06 6403 6404 8d01 5a07 6503 6504 6405  j.d.d...Z.e.e.d.
-00000970: 3c00 6505 6a06 6403 6404 8d01 5a08 6503  <.e.j.d.d...Z.e.
-00000980: 6504 6406 3c00 6505 6a06 6407 6404 8d01  e.d.<.e.j.d.d...
-00000990: 5a09 650a 6504 6408 3c00 6505 6a06 6409  Z.e.e.d.<.e.j.d.
-000009a0: 6404 8d01 5a0b 650a 6504 640a 3c00 6505  d...Z.e.e.d.<.e.
-000009b0: 6a06 640b 6404 8d01 5a0c 650d 6504 640c  j.d.d...Z.e.e.d.
-000009c0: 3c00 640d 5300 290e 7a0a 5061 7468 2e41  <.d.S.).z.Path.A
-000009d0: 7263 546f 7210 0000 0072 1100 0000 7201  rcTor....r....r.
-000009e0: 0000 0072 1200 0000 da06 7261 6469 7573  ...r......radius
-000009f0: da08 726f 7461 7469 6f6e 46da 096c 6172  ..rotationF..lar
-00000a00: 6765 5f61 7263 54da 0963 6c6f 636b 7769  ge_arcT..clockwi
-00000a10: 7365 5a05 6172 6374 6f72 1400 0000 4e29  seZ.arctor....N)
-00000a20: 0e72 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000a30: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000a40: 1900 0000 722b 0000 0072 2c00 0000 722d  ....r+...r,...r-
-00000a50: 0000 00da 0462 6f6f 6c72 2e00 0000 7214  .....boolr....r.
-00000a60: 0000 0072 1a00 0000 720d 0000 0072 0d00  ...r....r....r..
-00000a70: 0000 720d 0000 0072 0e00 0000 da05 4172  ..r....r......Ar
-00000a80: 6354 6f3e 0000 0073 0e00 0000 0a02 0801  cTo>...s........
-00000a90: 0801 1401 1401 1401 1401 7230 0000 0063  ..........r0...c
-00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ab0: 0300 0000 4000 0000 7342 0000 0065 005a  ....@...sB...e.Z
-00000ac0: 0164 005a 0255 0065 0365 0464 013c 0065  .d.Z.U.e.e.d.<.e
-00000ad0: 0365 0464 023c 0065 0365 0464 033c 0065  .e.d.<.e.e.d.<.e
-00000ae0: 0365 0464 043c 0065 056a 0664 0564 068d  .e.d.<.e.j.d.d..
-00000af0: 015a 0765 0865 0464 073c 0064 0853 0029  .Z.e.e.d.<.d.S.)
-00000b00: 097a 0950 6174 682e 4f76 616c 7210 0000  .z.Path.Ovalr...
-00000b10: 0072 1100 0000 7225 0000 0072 2600 0000  .r....r%...r&...
-00000b20: da04 6f76 616c 7212 0000 0072 1400 0000  ..ovalr....r....
-00000b30: 4e72 1500 0000 720d 0000 0072 0d00 0000  Nr....r....r....
-00000b40: 720d 0000 0072 0e00 0000 da04 4f76 616c  r....r......Oval
-00000b50: 4800 0000 730a 0000 000a 0208 0108 0108  H...s...........
-00000b60: 0108 0172 3200 0000 6300 0000 0000 0000  ...r2...c.......
-00000b70: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000b80: 0073 5600 0000 6500 5a01 6400 5a02 5500  .sV...e.Z.d.Z.U.
-00000b90: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
-00000ba0: 6503 6504 6403 3c00 6503 6504 6404 3c00  e.e.d.<.e.e.d.<.
-00000bb0: 6505 6a06 6405 6406 8d01 5a07 6508 6504  e.j.d.d...Z.e.e.
-00000bc0: 6407 3c00 6505 6a06 6408 6406 8d01 5a09  d.<.e.j.d.d...Z.
-00000bd0: 650a 6504 6409 3c00 6405 5300 290a 7a09  e.e.d.<.d.S.).z.
-00000be0: 5061 7468 2e52 6563 7472 1000 0000 7211  Path.Rectr....r.
-00000bf0: 0000 0072 2500 0000 7226 0000 004e 7212  ...r%...r&...Nr.
-00000c00: 0000 00da 0d62 6f72 6465 725f 7261 6469  .....border_radi
-00000c10: 7573 5a04 7265 6374 7214 0000 0029 0b72  usZ.rectr....).r
-00000c20: 0a00 0000 720b 0000 0072 0c00 0000 7216  ....r....r....r.
-00000c30: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-00000c40: 0000 7233 0000 0072 0700 0000 7214 0000  ..r3...r....r...
-00000c50: 0072 1a00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000c60: 720d 0000 0072 0e00 0000 da04 5265 6374  r....r......Rect
-00000c70: 5000 0000 730c 0000 000a 0208 0108 0108  P...s...........
-00000c80: 0108 0114 0172 3400 0000 6300 0000 0000  .....r4...c.....
-00000c90: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000ca0: 0000 0073 2200 0000 6500 5a01 6400 5a02  ...s"...e.Z.d.Z.
-00000cb0: 5500 6503 6a04 6401 6402 8d01 5a05 6506  U.e.j.d.d...Z.e.
-00000cc0: 6507 6403 3c00 6404 5300 2905 7a0a 5061  e.d.<.d.S.).z.Pa
-00000cd0: 7468 2e43 6c6f 7365 da05 636c 6f73 6572  th.Close..closer
-00000ce0: 1200 0000 7214 0000 004e 2908 720a 0000  ....r....N).r...
-00000cf0: 0072 0b00 0000 720c 0000 0072 1800 0000  .r....r....r....
-00000d00: 7219 0000 0072 1400 0000 721a 0000 0072  r....r....r....r
-00000d10: 1700 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
-00000d20: 0000 0072 0e00 0000 da05 436c 6f73 6559  ...r......CloseY
-00000d30: 0000 0073 0200 0000 0a02 7236 0000 004e  ...s......r6...N
-00000d40: 2905 7223 0000 00da 0570 6169 6e74 da07  ).r#.....paint..
-00000d50: 7669 7369 626c 65da 0864 6973 6162 6c65  visible..disable
-00000d60: 64da 0464 6174 6163 0700 0000 0000 0000  d..datac........
-00000d70: 0000 0000 0700 0000 0700 0000 4300 0000  ............C...
-00000d80: 7324 0000 0074 006a 017c 007c 037c 047c  s$...t.j.|.|.|.|
-00000d90: 057c 0664 018d 0501 007c 017c 005f 027c  .|.d.....|.|._.|
-00000da0: 027c 005f 0364 0053 0029 024e 2904 da03  .|._.d.S.).N)...
-00000db0: 7265 6672 3800 0000 7239 0000 0072 3a00  refr8...r9...r:.
-00000dc0: 0000 2904 7205 0000 00da 085f 5f69 6e69  ..).r......__ini
-00000dd0: 745f 5f72 2300 0000 7237 0000 0029 07da  t__r#...r7...)..
-00000de0: 0473 656c 6672 2300 0000 7237 0000 0072  .selfr#...r7...r
-00000df0: 3b00 0000 7238 0000 0072 3900 0000 723a  ;...r8...r9...r:
-00000e00: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000e10: 0000 723c 0000 005d 0000 0073 0600 0000  ..r<...]...s....
-00000e20: 000c 1402 0601 7a0d 5061 7468 2e5f 5f69  ......z.Path.__i
-00000e30: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000e40: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
-00000e50: 0000 0064 0153 0029 024e da04 7061 7468  ...d.S.).N..path
-00000e60: 720d 0000 00a9 0172 3d00 0000 720d 0000  r......r=...r...
-00000e70: 0072 0d00 0000 720e 0000 00da 115f 6765  .r....r......_ge
-00000e80: 745f 636f 6e74 726f 6c5f 6e61 6d65 6e00  t_control_namen.
-00000e90: 0000 7302 0000 0000 017a 1650 6174 682e  ..s......z.Path.
-00000ea0: 5f67 6574 5f63 6f6e 7472 6f6c 5f6e 616d  _get_control_nam
-00000eb0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000ec0: 0000 0400 0000 0300 0000 732a 0000 0074  ..........s*...t
-00000ed0: 0083 00a0 01a1 0001 007c 00a0 0264 017c  .........|...d.|
-00000ee0: 006a 03a1 0201 007c 00a0 0264 027c 006a  .j.....|...d.|.j
-00000ef0: 04a1 0201 0064 0053 0029 034e 7223 0000  .....d.S.).Nr#..
-00000f00: 0072 3700 0000 2905 da05 7375 7065 72da  .r7...)...super.
-00000f10: 0d62 6566 6f72 655f 7570 6461 7465 da0e  .before_update..
-00000f20: 5f73 6574 5f61 7474 725f 6a73 6f6e da0f  _set_attr_json..
-00000f30: 5f50 6174 685f 5f65 6c65 6d65 6e74 73da  _Path__elements.
-00000f40: 0c5f 5061 7468 5f5f 7061 696e 7472 3f00  ._Path__paintr?.
-00000f50: 0000 a901 da09 5f5f 636c 6173 735f 5f72  ......__class__r
-00000f60: 0d00 0000 720e 0000 0072 4200 0000 7100  ....r....rB...q.
-00000f70: 0000 7306 0000 0000 010a 010e 017a 1250  ..s..........z.P
-00000f80: 6174 682e 6265 666f 7265 5f75 7064 6174  ath.before_updat
-00000f90: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000fa0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-00000fb0: 006a 0053 00a9 014e a901 7244 0000 0072  .j.S...N..rD...r
-00000fc0: 3f00 0000 720d 0000 0072 0d00 0000 720e  ?...r....r....r.
-00000fd0: 0000 0072 2300 0000 7700 0000 7302 0000  ...r#...w...s...
-00000fe0: 0000 027a 0d50 6174 682e 656c 656d 656e  ...z.Path.elemen
-00000ff0: 7473 2901 da05 7661 6c75 6563 0200 0000  ts)...valuec....
-00001000: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001010: 4300 0000 7316 0000 007c 0164 0075 0172  C...s....|.d.u.r
-00001020: 0c7c 016e 0267 007c 005f 0064 0053 0072  .|.n.g.|._.d.S.r
-00001030: 4800 0000 7249 0000 00a9 0272 3d00 0000  H...rI.....r=...
-00001040: 724a 0000 0072 0d00 0000 720d 0000 0072  rJ...r....r....r
-00001050: 0e00 0000 7223 0000 007b 0000 0073 0200  ....r#...{...s..
-00001060: 0000 0002 2901 da06 7265 7475 726e 6301  ....)...returnc.
-00001070: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00001080: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00001090: 5300 7248 0000 00a9 0172 4500 0000 723f  S.rH.....rE...r?
-000010a0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-000010b0: 0000 7237 0000 0080 0000 0073 0200 0000  ..r7.......s....
-000010c0: 0002 7a0a 5061 7468 2e70 6169 6e74 6302  ..z.Path.paintc.
-000010d0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-000010e0: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
-000010f0: 5f00 6400 5300 7248 0000 0072 4d00 0000  _.d.S.rH...rM...
-00001100: 724b 0000 0072 0d00 0000 720d 0000 0072  rK...r....r....r
-00001110: 0e00 0000 7237 0000 0084 0000 0073 0200  ....r7.......s..
-00001120: 0000 0002 2906 4e4e 4e4e 4e4e 291d 720a  ....).NNNNNN).r.
-00001130: 0000 0072 0b00 0000 720c 0000 0072 1800  ...r....r....r..
-00001140: 0000 da09 6461 7461 636c 6173 7372 0f00  ....dataclassr..
-00001150: 0000 721b 0000 0072 1c00 0000 7221 0000  ..r....r....r!..
-00001160: 0072 2200 0000 7224 0000 0072 2a00 0000  .r"...r$...r*...
-00001170: 7230 0000 0072 3200 0000 7234 0000 0072  r0...r2...r4...r
-00001180: 3600 0000 7204 0000 0072 0300 0000 7206  6...r....r....r.
-00001190: 0000 0072 2f00 0000 7202 0000 0072 3c00  ...r/...r....r<.
-000011a0: 0000 7240 0000 0072 4200 0000 da08 7072  ..r@...rB.....pr
-000011b0: 6f70 6572 7479 7223 0000 00da 0673 6574  opertyr#.....set
-000011c0: 7465 7272 3700 0000 da0d 5f5f 636c 6173  terr7.....__clas
-000011d0: 7363 656c 6c5f 5f72 0d00 0000 720d 0000  scell__r....r...
-000011e0: 0072 4600 0000 720e 0000 0072 0800 0000  .rF...r....r....
-000011f0: 0900 0000 735a 0000 0008 0104 0110 0304  ....sZ..........
-00001200: 0112 0504 0112 0504 0112 0804 0112 0904  ................
-00001210: 0112 0604 0112 0904 0112 0904 0112 0704  ................
-00001220: 0112 0804 0112 0500 0100 0400 0100 0100  ................
-00001230: 0100 f602 020a 0106 0506 0106 0102 f60c  ................
-00001240: 1108 030c 0602 010a 0304 0118 0402 0114  ................
-00001250: 0304 0172 0800 0000 290c 7218 0000 00da  ...r....).r.....
-00001260: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-00001270: 0072 0400 0000 da16 666c 6574 5f63 6f72  .r......flet_cor
-00001280: 652e 6361 6e76 6173 2e73 6861 7065 7205  e.canvas.shaper.
-00001290: 0000 00da 1266 6c65 745f 636f 7265 2e70  .....flet_core.p
-000012a0: 6169 6e74 696e 6772 0600 0000 da0f 666c  aintingr......fl
-000012b0: 6574 5f63 6f72 652e 7479 7065 7372 0700  et_core.typesr..
-000012c0: 0000 7208 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000012d0: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
-000012e0: 6475 6c65 3e01 0000 0073 0a00 0000 0801  dule>....s......
-000012f0: 1402 0c01 0c01 0c03                      ........
+00000310: 6c65 7463 6f6e 7472 6962 2f73 646b 2f70  letcontrib/sdk/p
+00000320: 7974 686f 6e2f 7061 636b 6167 6573 2f66  ython/packages/f
+00000330: 6c65 742d 636f 7265 2f73 7263 2f66 6c65  let-core/src/fle
+00000340: 745f 636f 7265 2f63 616e 7661 732f 7061  t_core/canvas/pa
+00000350: 7468 2e70 79da 0b50 6174 6845 6c65 6d65  th.py..PathEleme
+00000360: 6e74 0a00 0000 7302 0000 0008 0272 0f00  nt....s......r..
+00000370: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000380: 0000 0003 0000 0040 0000 0073 3200 0000  .......@...s2...
+00000390: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
+000003a0: 3c00 6503 6504 6402 3c00 6505 6a06 6403  <.e.e.d.<.e.j.d.
+000003b0: 6404 8d01 5a07 6508 6504 6405 3c00 6406  d...Z.e.e.d.<.d.
+000003c0: 5300 2907 7a0b 5061 7468 2e4d 6f76 6554  S.).z.Path.MoveT
+000003d0: 6fda 0178 da01 795a 066d 6f76 6574 6fa9  o..x..yZ.moveto.
+000003e0: 01da 0764 6566 6175 6c74 da04 7479 7065  ...default..type
+000003f0: 4ea9 0972 0a00 0000 720b 0000 0072 0c00  N..r....r....r..
+00000400: 0000 da05 666c 6f61 74da 0f5f 5f61 6e6e  ....float..__ann
+00000410: 6f74 6174 696f 6e73 5f5f da0b 6461 7461  otations__..data
+00000420: 636c 6173 7365 73da 0566 6965 6c64 7214  classes..fieldr.
+00000430: 0000 00da 0373 7472 720d 0000 0072 0d00  .....strr....r..
+00000440: 0000 720d 0000 0072 0e00 0000 da06 4d6f  ..r....r......Mo
+00000450: 7665 546f 0e00 0000 7306 0000 000a 0208  veTo....s.......
+00000460: 0108 0172 1b00 0000 6300 0000 0000 0000  ...r....c.......
+00000470: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000480: 0073 3200 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
+00000490: 6503 6504 6401 3c00 6503 6504 6402 3c00  e.e.d.<.e.e.d.<.
+000004a0: 6505 6a06 6403 6404 8d01 5a07 6508 6504  e.j.d.d...Z.e.e.
+000004b0: 6405 3c00 6406 5300 2907 7a0b 5061 7468  d.<.d.S.).z.Path
+000004c0: 2e4c 696e 6554 6f72 1000 0000 7211 0000  .LineTor....r...
+000004d0: 005a 066c 696e 6574 6f72 1200 0000 7214  .Z.linetor....r.
+000004e0: 0000 004e 7215 0000 0072 0d00 0000 720d  ...Nr....r....r.
+000004f0: 0000 0072 0d00 0000 720e 0000 00da 064c  ...r....r......L
+00000500: 696e 6554 6f14 0000 0073 0600 0000 0a02  ineTo....s......
+00000510: 0801 0801 721c 0000 0063 0000 0000 0000  ....r....c......
+00000520: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000530: 0000 7356 0000 0065 005a 0164 005a 0255  ..sV...e.Z.d.Z.U
+00000540: 0065 0365 0464 013c 0065 0365 0464 023c  .e.e.d.<.e.e.d.<
+00000550: 0065 0365 0464 033c 0065 0365 0464 043c  .e.e.d.<.e.e.d.<
+00000560: 0065 056a 0664 0564 068d 015a 0765 0365  .e.j.d.d...Z.e.e
+00000570: 0464 073c 0065 056a 0664 0864 068d 015a  .d.<.e.j.d.d...Z
+00000580: 0865 0965 0464 093c 0064 0a53 0029 0b7a  .e.e.d.<.d.S.).z
+00000590: 1050 6174 682e 5175 6164 7261 7469 6354  .Path.QuadraticT
+000005a0: 6fda 0463 7031 78da 0463 7031 7972 1000  o..cp1x..cp1yr..
+000005b0: 0000 7211 0000 00e9 0100 0000 7212 0000  ..r.........r...
+000005c0: 00da 0177 5a07 636f 6e69 6374 6f72 1400  ...wZ.conictor..
+000005d0: 0000 4e29 0a72 0a00 0000 720b 0000 0072  ..N).r....r....r
+000005e0: 0c00 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+000005f0: 0000 0072 1900 0000 7220 0000 0072 1400  ...r....r ...r..
+00000600: 0000 721a 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000610: 0072 0d00 0000 720e 0000 00da 0b51 7561  .r....r......Qua
+00000620: 6472 6174 6963 546f 1a00 0000 730c 0000  draticTo....s...
+00000630: 000a 0208 0108 0108 0108 0114 0172 2100  .............r!.
+00000640: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000650: 0000 0003 0000 0040 0000 0073 5200 0000  .......@...sR...
+00000660: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
+00000670: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
+00000680: 3c00 6503 6504 6404 3c00 6503 6504 6405  <.e.e.d.<.e.e.d.
+00000690: 3c00 6503 6504 6406 3c00 6505 6a06 6407  <.e.e.d.<.e.j.d.
+000006a0: 6408 8d01 5a07 6508 6504 6409 3c00 640a  d...Z.e.e.d.<.d.
+000006b0: 5300 290b 7a0c 5061 7468 2e43 7562 6963  S.).z.Path.Cubic
+000006c0: 546f 721d 0000 0072 1e00 0000 5a04 6370  Tor....r....Z.cp
+000006d0: 3278 5a04 6370 3279 7210 0000 0072 1100  2xZ.cp2yr....r..
+000006e0: 0000 5a07 6375 6269 6374 6f72 1200 0000  ..Z.cubictor....
+000006f0: 7214 0000 004e 7215 0000 0072 0d00 0000  r....Nr....r....
+00000700: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00000710: 0743 7562 6963 546f 2300 0000 730e 0000  .CubicTo#...s...
+00000720: 000a 0208 0108 0108 0108 0108 0108 0172  ...............r
+00000730: 2200 0000 6300 0000 0000 0000 0000 0000  "...c...........
+00000740: 0000 0000 0003 0000 0040 0000 0073 3e00  .........@...s>.
+00000750: 0000 6500 5a01 6400 5a02 5500 6503 6401  ..e.Z.d.Z.U.e.d.
+00000760: 1900 6504 6402 3c00 6505 6504 6403 3c00  ..e.d.<.e.e.d.<.
+00000770: 6505 6504 6404 3c00 6506 6a07 6405 6406  e.e.d.<.e.j.d.d.
+00000780: 8d01 5a08 6509 6504 6407 3c00 6408 5300  ..Z.e.e.d.<.d.S.
+00000790: 2909 7a0c 5061 7468 2e53 7562 5061 7468  ).z.Path.SubPath
+000007a0: 7209 0000 00da 0865 6c65 6d65 6e74 7372  r......elementsr
+000007b0: 1000 0000 7211 0000 005a 0773 7562 7061  ....r....Z.subpa
+000007c0: 7468 7212 0000 0072 1400 0000 4e29 0a72  thr....r....N).r
+000007d0: 0a00 0000 720b 0000 0072 0c00 0000 7203  ....r....r....r.
+000007e0: 0000 0072 1700 0000 7216 0000 0072 1800  ...r....r....r..
+000007f0: 0000 7219 0000 0072 1400 0000 721a 0000  ..r....r....r...
+00000800: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000810: 720e 0000 00da 0753 7562 5061 7468 2d00  r......SubPath-.
+00000820: 0000 7308 0000 000a 020c 0108 0108 0172  ..s............r
+00000830: 2400 0000 6300 0000 0000 0000 0000 0000  $...c...........
+00000840: 0000 0000 0003 0000 0040 0000 0073 5200  .........@...sR.
+00000850: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
+00000860: 6401 3c00 6503 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
+00000870: 6403 3c00 6503 6504 6404 3c00 6503 6504  d.<.e.e.d.<.e.e.
+00000880: 6405 3c00 6503 6504 6406 3c00 6505 6a06  d.<.e.e.d.<.e.j.
+00000890: 6407 6408 8d01 5a07 6508 6504 6409 3c00  d.d...Z.e.e.d.<.
+000008a0: 640a 5300 290b 7a08 5061 7468 2e41 7263  d.S.).z.Path.Arc
+000008b0: 7210 0000 0072 1100 0000 da05 7769 6474  r....r......widt
+000008c0: 68da 0668 6569 6768 74da 0b73 7461 7274  h..height..start
+000008d0: 5f61 6e67 6c65 da0b 7377 6565 705f 616e  _angle..sweep_an
+000008e0: 676c 65da 0361 7263 7212 0000 0072 1400  gle..arcr....r..
+000008f0: 0000 4e72 1500 0000 720d 0000 0072 0d00  ..Nr....r....r..
+00000900: 0000 720d 0000 0072 0e00 0000 da03 4172  ..r....r......Ar
+00000910: 6334 0000 0073 0e00 0000 0a02 0801 0801  c4...s..........
+00000920: 0801 0801 0801 0801 722a 0000 0063 0000  ........r*...c..
+00000930: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000940: 0000 4000 0000 7382 0000 0065 005a 0164  ..@...s....e.Z.d
+00000950: 005a 0255 0065 0365 0464 013c 0065 0365  .Z.U.e.e.d.<.e.e
+00000960: 0464 023c 0065 056a 0664 0364 048d 015a  .d.<.e.j.d.d...Z
+00000970: 0765 0365 0464 053c 0065 056a 0664 0364  .e.e.d.<.e.j.d.d
+00000980: 048d 015a 0865 0365 0464 063c 0065 056a  ...Z.e.e.d.<.e.j
+00000990: 0664 0764 048d 015a 0965 0a65 0464 083c  .d.d...Z.e.e.d.<
+000009a0: 0065 056a 0664 0964 048d 015a 0b65 0a65  .e.j.d.d...Z.e.e
+000009b0: 0464 0a3c 0065 056a 0664 0b64 048d 015a  .d.<.e.j.d.d...Z
+000009c0: 0c65 0d65 0464 0c3c 0064 0d53 0029 0e7a  .e.e.d.<.d.S.).z
+000009d0: 0a50 6174 682e 4172 6354 6f72 1000 0000  .Path.ArcTor....
+000009e0: 7211 0000 0072 0100 0000 7212 0000 00da  r....r....r.....
+000009f0: 0672 6164 6975 73da 0872 6f74 6174 696f  .radius..rotatio
+00000a00: 6e46 da09 6c61 7267 655f 6172 6354 da09  nF..large_arcT..
+00000a10: 636c 6f63 6b77 6973 655a 0561 7263 746f  clockwiseZ.arcto
+00000a20: 7214 0000 004e 290e 720a 0000 0072 0b00  r....N).r....r..
+00000a30: 0000 720c 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000a40: 0072 1800 0000 7219 0000 0072 2b00 0000  .r....r....r+...
+00000a50: 722c 0000 0072 2d00 0000 da04 626f 6f6c  r,...r-.....bool
+00000a60: 722e 0000 0072 1400 0000 721a 0000 0072  r....r....r....r
+00000a70: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00000a80: 0000 00da 0541 7263 546f 3e00 0000 730e  .....ArcTo>...s.
+00000a90: 0000 000a 0208 0108 0114 0114 0114 0114  ................
+00000aa0: 0172 3000 0000 6300 0000 0000 0000 0000  .r0...c.........
+00000ab0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000ac0: 4200 0000 6500 5a01 6400 5a02 5500 6503  B...e.Z.d.Z.U.e.
+00000ad0: 6504 6401 3c00 6503 6504 6402 3c00 6503  e.d.<.e.e.d.<.e.
+00000ae0: 6504 6403 3c00 6503 6504 6404 3c00 6505  e.d.<.e.e.d.<.e.
+00000af0: 6a06 6405 6406 8d01 5a07 6508 6504 6407  j.d.d...Z.e.e.d.
+00000b00: 3c00 6408 5300 2909 7a09 5061 7468 2e4f  <.d.S.).z.Path.O
+00000b10: 7661 6c72 1000 0000 7211 0000 0072 2500  valr....r....r%.
+00000b20: 0000 7226 0000 00da 046f 7661 6c72 1200  ..r&.....ovalr..
+00000b30: 0000 7214 0000 004e 7215 0000 0072 0d00  ..r....Nr....r..
+00000b40: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000b50: 00da 044f 7661 6c48 0000 0073 0a00 0000  ...OvalH...s....
+00000b60: 0a02 0801 0801 0801 0801 7232 0000 0063  ..........r2...c
+00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b80: 0300 0000 4000 0000 7356 0000 0065 005a  ....@...sV...e.Z
+00000b90: 0164 005a 0255 0065 0365 0464 013c 0065  .d.Z.U.e.e.d.<.e
+00000ba0: 0365 0464 023c 0065 0365 0464 033c 0065  .e.d.<.e.e.d.<.e
+00000bb0: 0365 0464 043c 0065 056a 0664 0564 068d  .e.d.<.e.j.d.d..
+00000bc0: 015a 0765 0865 0464 073c 0065 056a 0664  .Z.e.e.d.<.e.j.d
+00000bd0: 0864 068d 015a 0965 0a65 0464 093c 0064  .d...Z.e.e.d.<.d
+00000be0: 0553 0029 0a7a 0950 6174 682e 5265 6374  .S.).z.Path.Rect
+00000bf0: 7210 0000 0072 1100 0000 7225 0000 0072  r....r....r%...r
+00000c00: 2600 0000 4e72 1200 0000 da0d 626f 7264  &...Nr......bord
+00000c10: 6572 5f72 6164 6975 735a 0472 6563 7472  er_radiusZ.rectr
+00000c20: 1400 0000 290b 720a 0000 0072 0b00 0000  ....).r....r....
+00000c30: 720c 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000c40: 1800 0000 7219 0000 0072 3300 0000 7207  ....r....r3...r.
+00000c50: 0000 0072 1400 0000 721a 0000 0072 0d00  ...r....r....r..
+00000c60: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000c70: 00da 0452 6563 7450 0000 0073 0c00 0000  ...RectP...s....
+00000c80: 0a02 0801 0801 0801 0801 1401 7234 0000  ............r4..
+00000c90: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000ca0: 0000 0300 0000 4000 0000 7322 0000 0065  ......@...s"...e
+00000cb0: 005a 0164 005a 0255 0065 036a 0464 0164  .Z.d.Z.U.e.j.d.d
+00000cc0: 028d 015a 0565 0665 0764 033c 0064 0453  ...Z.e.e.d.<.d.S
+00000cd0: 0029 057a 0a50 6174 682e 436c 6f73 65da  .).z.Path.Close.
+00000ce0: 0563 6c6f 7365 7212 0000 0072 1400 0000  .closer....r....
+00000cf0: 4e29 0872 0a00 0000 720b 0000 0072 0c00  N).r....r....r..
+00000d00: 0000 7218 0000 0072 1900 0000 7214 0000  ..r....r....r...
+00000d10: 0072 1a00 0000 7217 0000 0072 0d00 0000  .r....r....r....
+00000d20: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00000d30: 0543 6c6f 7365 5900 0000 7302 0000 000a  .CloseY...s.....
+00000d40: 0272 3600 0000 4e29 0572 2300 0000 da05  .r6...N).r#.....
+00000d50: 7061 696e 74da 0776 6973 6962 6c65 da08  paint..visible..
+00000d60: 6469 7361 626c 6564 da04 6461 7461 6307  disabled..datac.
+00000d70: 0000 0000 0000 0000 0000 0007 0000 0007  ................
+00000d80: 0000 0043 0000 0073 2400 0000 7400 6a01  ...C...s$...t.j.
+00000d90: 7c00 7c03 7c04 7c05 7c06 6401 8d05 0100  |.|.|.|.|.d.....
+00000da0: 7c01 7c00 5f02 7c02 7c00 5f03 6400 5300  |.|._.|.|._.d.S.
+00000db0: 2902 4e29 04da 0372 6566 7238 0000 0072  ).N)...refr8...r
+00000dc0: 3900 0000 723a 0000 0029 0472 0500 0000  9...r:...).r....
+00000dd0: da08 5f5f 696e 6974 5f5f 7223 0000 0072  ..__init__r#...r
+00000de0: 3700 0000 2907 da04 7365 6c66 7223 0000  7...)...selfr#..
+00000df0: 0072 3700 0000 723b 0000 0072 3800 0000  .r7...r;...r8...
+00000e00: 7239 0000 0072 3a00 0000 720d 0000 0072  r9...r:...r....r
+00000e10: 0d00 0000 720e 0000 0072 3c00 0000 5d00  ....r....r<...].
+00000e20: 0000 7306 0000 0000 0c14 0206 017a 0d50  ..s..........z.P
+00000e30: 6174 682e 5f5f 696e 6974 5f5f 6301 0000  ath.__init__c...
+00000e40: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000e50: 0043 0000 0073 0400 0000 6401 5300 2902  .C...s....d.S.).
+00000e60: 4eda 0470 6174 6872 0d00 0000 a901 723d  N..pathr......r=
+00000e70: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000e80: 0000 da11 5f67 6574 5f63 6f6e 7472 6f6c  ...._get_control
+00000e90: 5f6e 616d 656e 0000 0073 0200 0000 0001  _namen...s......
+00000ea0: 7a16 5061 7468 2e5f 6765 745f 636f 6e74  z.Path._get_cont
+00000eb0: 726f 6c5f 6e61 6d65 6301 0000 0000 0000  rol_namec.......
+00000ec0: 0000 0000 0001 0000 0004 0000 0003 0000  ................
+00000ed0: 0073 2a00 0000 7400 8300 a001 a100 0100  .s*...t.........
+00000ee0: 7c00 a002 6401 7c00 6a03 a102 0100 7c00  |...d.|.j.....|.
+00000ef0: a002 6402 7c00 6a04 a102 0100 6400 5300  ..d.|.j.....d.S.
+00000f00: 2903 4e72 2300 0000 7237 0000 0029 05da  ).Nr#...r7...)..
+00000f10: 0573 7570 6572 da0d 6265 666f 7265 5f75  .super..before_u
+00000f20: 7064 6174 65da 0e5f 7365 745f 6174 7472  pdate.._set_attr
+00000f30: 5f6a 736f 6eda 0f5f 5061 7468 5f5f 656c  _json.._Path__el
+00000f40: 656d 656e 7473 da0c 5f50 6174 685f 5f70  ements.._Path__p
+00000f50: 6169 6e74 723f 0000 00a9 01da 095f 5f63  aintr?.......__c
+00000f60: 6c61 7373 5f5f 720d 0000 0072 0e00 0000  lass__r....r....
+00000f70: 7242 0000 0071 0000 0073 0600 0000 0001  rB...q...s......
+00000f80: 0a01 0e01 7a12 5061 7468 2e62 6566 6f72  ....z.Path.befor
+00000f90: 655f 7570 6461 7465 6301 0000 0000 0000  e_updatec.......
+00000fa0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000fb0: 0073 0600 0000 7c00 6a00 5300 a901 4ea9  .s....|.j.S...N.
+00000fc0: 0172 4400 0000 723f 0000 0072 0d00 0000  .rD...r?...r....
+00000fd0: 720d 0000 0072 0e00 0000 7223 0000 0077  r....r....r#...w
+00000fe0: 0000 0073 0200 0000 0002 7a0d 5061 7468  ...s......z.Path
+00000ff0: 2e65 6c65 6d65 6e74 7329 01da 0576 616c  .elements)...val
+00001000: 7565 6302 0000 0000 0000 0000 0000 0002  uec.............
+00001010: 0000 0002 0000 0043 0000 0073 1600 0000  .......C...s....
+00001020: 7c01 6400 7501 720c 7c01 6e02 6700 7c00  |.d.u.r.|.n.g.|.
+00001030: 5f00 6400 5300 7248 0000 0072 4900 0000  _.d.S.rH...rI...
+00001040: a902 723d 0000 0072 4a00 0000 720d 0000  ..r=...rJ...r...
+00001050: 0072 0d00 0000 720e 0000 0072 2300 0000  .r....r....r#...
+00001060: 7b00 0000 7302 0000 0000 0229 01da 0672  {...s......)...r
+00001070: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+00001080: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00001090: 0000 007c 006a 0053 0072 4800 0000 a901  ...|.j.S.rH.....
+000010a0: 7245 0000 0072 3f00 0000 720d 0000 0072  rE...r?...r....r
+000010b0: 0d00 0000 720e 0000 0072 3700 0000 8000  ....r....r7.....
+000010c0: 0000 7302 0000 0000 027a 0a50 6174 682e  ..s......z.Path.
+000010d0: 7061 696e 7463 0200 0000 0000 0000 0000  paintc..........
+000010e0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+000010f0: 0000 007c 017c 005f 0064 0053 0072 4800  ...|.|._.d.S.rH.
+00001100: 0000 724d 0000 0072 4b00 0000 720d 0000  ..rM...rK...r...
+00001110: 0072 0d00 0000 720e 0000 0072 3700 0000  .r....r....r7...
+00001120: 8400 0000 7302 0000 0000 0229 064e 4e4e  ....s......).NNN
+00001130: 4e4e 4e29 1d72 0a00 0000 720b 0000 0072  NNN).r....r....r
+00001140: 0c00 0000 7218 0000 00da 0964 6174 6163  ....r......datac
+00001150: 6c61 7373 720f 0000 0072 1b00 0000 721c  lassr....r....r.
+00001160: 0000 0072 2100 0000 7222 0000 0072 2400  ...r!...r"...r$.
+00001170: 0000 722a 0000 0072 3000 0000 7232 0000  ..r*...r0...r2..
+00001180: 0072 3400 0000 7236 0000 0072 0400 0000  .r4...r6...r....
+00001190: 7203 0000 0072 0600 0000 722f 0000 0072  r....r....r/...r
+000011a0: 0200 0000 723c 0000 0072 4000 0000 7242  ....r<...r@...rB
+000011b0: 0000 00da 0870 726f 7065 7274 7972 2300  .....propertyr#.
+000011c0: 0000 da06 7365 7474 6572 7237 0000 00da  ....setterr7....
+000011d0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720d  .__classcell__r.
+000011e0: 0000 0072 0d00 0000 7246 0000 0072 0e00  ...r....rF...r..
+000011f0: 0000 7208 0000 0009 0000 0073 5a00 0000  ..r........sZ...
+00001200: 0801 0401 1003 0401 1205 0401 1205 0401  ................
+00001210: 1208 0401 1209 0401 1206 0401 1209 0401  ................
+00001220: 1209 0401 1207 0401 1208 0401 1205 0001  ................
+00001230: 0004 0001 0001 0001 00f6 0202 0a01 0605  ................
+00001240: 0601 0601 02f6 0c11 0803 0c06 0201 0a03  ................
+00001250: 0401 1804 0201 1403 0401 7208 0000 0029  ..........r....)
+00001260: 0c72 1800 0000 da06 7479 7069 6e67 7202  .r......typingr.
+00001270: 0000 0072 0300 0000 7204 0000 00da 1666  ...r....r......f
+00001280: 6c65 745f 636f 7265 2e63 616e 7661 732e  let_core.canvas.
+00001290: 7368 6170 6572 0500 0000 da12 666c 6574  shaper......flet
+000012a0: 5f63 6f72 652e 7061 696e 7469 6e67 7206  _core.paintingr.
+000012b0: 0000 00da 0f66 6c65 745f 636f 7265 2e74  .....flet_core.t
+000012c0: 7970 6573 7207 0000 0072 0800 0000 720d  ypesr....r....r.
+000012d0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000012e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000012f0: 730a 0000 0008 0114 020c 010c 010c 03    s..............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/points.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/points.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 1507 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 1507 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 6501 8303  ..G.d.d...d.e...
@@ -18,139 +18,140 @@
 00000110: 0453 0029 05da 0950 6f69 6e74 4d6f 6465  .S.)...PointMode
 00000120: da06 706f 696e 7473 da05 6c69 6e65 735a  ..points..linesZ
 00000130: 0770 6f6c 7967 6f6e 4e29 06da 085f 5f6e  .polygonN)...__n
 00000140: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00000150: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f5a  _..__qualname__Z
 00000160: 0650 4f49 4e54 535a 054c 494e 4553 5a07  .POINTSZ.LINESZ.
 00000170: 504f 4c59 474f 4ea9 0072 0f00 0000 720f  POLYGON..r....r.
-00000180: 0000 00fa 592f 776f 726b 7370 6163 6573  ....Y/workspaces
+00000180: 0000 00fa 602f 776f 726b 7370 6163 6573  ....`/workspaces
 00000190: 2f63 6f6e 7472 6962 666c 6574 2f66 6c65  /contribflet/fle
-000001a0: 742f 7364 6b2f 7079 7468 6f6e 2f70 6163  t/sdk/python/pac
-000001b0: 6b61 6765 732f 666c 6574 2d63 6f72 652f  kages/flet-core/
-000001c0: 7372 632f 666c 6574 5f63 6f72 652f 6361  src/flet_core/ca
-000001d0: 6e76 6173 2f70 6f69 6e74 732e 7079 7209  nvas/points.pyr.
-000001e0: 0000 0009 0000 0073 0600 0000 0801 0401  .......s........
-000001f0: 0401 7209 0000 0063 0000 0000 0000 0000  ..r....c........
-00000200: 0000 0000 0000 0000 0800 0000 0000 0000  ................
-00000210: 73e8 0000 0065 005a 0164 005a 0264 1465  s....e.Z.d.Z.d.e
-00000220: 0365 0465 0519 0019 0065 0365 0619 0065  .e.e.....e.e...e
-00000230: 0365 0719 0065 0365 0819 0065 0365 0819  .e...e.e...e.e..
-00000240: 0065 0964 029c 0664 0364 0484 055a 0a64  .e.d...d.d...Z.d
-00000250: 0564 0684 005a 0b87 0066 0164 0764 0884  .d...Z...f.d.d..
-00000260: 085a 0c65 0d65 0365 0619 0064 099c 0164  .Z.e.e.e...d...d
-00000270: 0a64 0b84 0483 015a 0e65 0e6a 0f65 0365  .d.....Z.e.j.e.e
-00000280: 0619 0064 0c9c 0164 0d64 0b84 0483 015a  ...d...d.d.....Z
-00000290: 0e65 0d65 0365 0465 0519 0019 0064 099c  .e.e.e.e.....d..
-000002a0: 0164 0e64 0f84 0483 015a 1065 106a 0f65  .d.d.....Z.e.j.e
-000002b0: 0365 0465 0519 0019 0064 0c9c 0164 1064  .e.e.....d...d.d
-000002c0: 0f84 0483 015a 1065 0d65 0365 0719 0064  .....Z.e.e.e...d
-000002d0: 099c 0164 1164 1284 0483 015a 1165 116a  ...d.d.....Z.e.j
-000002e0: 0f65 0365 0719 0064 0c9c 0164 1364 1284  .e.e...d...d.d..
-000002f0: 0483 015a 1187 0004 005a 1253 0029 15da  ...Z.....Z.S.)..
-00000300: 0650 6f69 6e74 734e 2906 720a 0000 00da  .PointsN).r.....
-00000310: 0a70 6f69 6e74 5f6d 6f64 65da 0570 6169  .point_mode..pai
-00000320: 6e74 da07 7669 7369 626c 65da 0864 6973  nt..visible..dis
-00000330: 6162 6c65 64da 0464 6174 6163 0800 0000  abled..datac....
-00000340: 0000 0000 0000 0000 0800 0000 0700 0000  ................
-00000350: 4300 0000 732a 0000 0074 006a 017c 007c  C...s*...t.j.|.|
-00000360: 047c 057c 067c 0764 018d 0501 007c 017c  .|.|.|.d.....|.|
-00000370: 005f 027c 027c 005f 037c 037c 005f 0464  ._.|.|._.|.|._.d
-00000380: 0053 0029 024e 2904 da03 7265 6672 1400  .S.).N)...refr..
-00000390: 0000 7215 0000 0072 1600 0000 2905 7206  ..r....r....).r.
-000003a0: 0000 00da 085f 5f69 6e69 745f 5f72 0a00  .....__init__r..
-000003b0: 0000 7212 0000 0072 1300 0000 2908 da04  ..r....r....)...
-000003c0: 7365 6c66 720a 0000 0072 1200 0000 7213  selfr....r....r.
-000003d0: 0000 0072 1700 0000 7214 0000 0072 1500  ...r....r....r..
-000003e0: 0000 7216 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-000003f0: 0072 1000 0000 7218 0000 0010 0000 0073  .r....r........s
-00000400: 0800 0000 000d 1402 0601 0601 7a0f 506f  ............z.Po
-00000410: 696e 7473 2e5f 5f69 6e69 745f 5f63 0100  ints.__init__c..
-00000420: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000430: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
-00000440: 024e 720a 0000 0072 0f00 0000 a901 7219  .Nr....r......r.
-00000450: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00000460: 0000 da11 5f67 6574 5f63 6f6e 7472 6f6c  ...._get_control
-00000470: 5f6e 616d 6523 0000 0073 0200 0000 0001  _name#...s......
-00000480: 7a18 506f 696e 7473 2e5f 6765 745f 636f  z.Points._get_co
-00000490: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
-000004a0: 0000 0000 0000 0001 0000 0004 0000 0003  ................
-000004b0: 0000 0073 2a00 0000 7400 8300 a001 a100  ...s*...t.......
-000004c0: 0100 7c00 a002 6401 7c00 6a03 a102 0100  ..|...d.|.j.....
-000004d0: 7c00 a002 6402 7c00 6a04 a102 0100 6400  |...d.|.j.....d.
-000004e0: 5300 2903 4e72 0a00 0000 7213 0000 0029  S.).Nr....r....)
-000004f0: 05da 0573 7570 6572 da0d 6265 666f 7265  ...super..before
-00000500: 5f75 7064 6174 65da 0e5f 7365 745f 6174  _update.._set_at
-00000510: 7472 5f6a 736f 6eda 0f5f 506f 696e 7473  tr_json.._Points
-00000520: 5f5f 706f 696e 7473 da0e 5f50 6f69 6e74  __points.._Point
-00000530: 735f 5f70 6169 6e74 721a 0000 00a9 01da  s__paintr.......
-00000540: 095f 5f63 6c61 7373 5f5f 720f 0000 0072  .__class__r....r
-00000550: 1000 0000 721d 0000 0026 0000 0073 0600  ....r....&...s..
-00000560: 0000 0001 0a01 0e01 7a14 506f 696e 7473  ........z.Points
-00000570: 2e62 6566 6f72 655f 7570 6461 7465 2901  .before_update).
-00000580: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00000590: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000005a0: 0073 0600 0000 7c00 6a00 5300 a901 4e29  .s....|.j.S...N)
-000005b0: 01da 135f 506f 696e 7473 5f5f 706f 696e  ..._Points__poin
-000005c0: 745f 6d6f 6465 721a 0000 0072 0f00 0000  t_moder....r....
-000005d0: 720f 0000 0072 1000 0000 7212 0000 002c  r....r....r....,
-000005e0: 0000 0073 0200 0000 0002 7a11 506f 696e  ...s......z.Poin
-000005f0: 7473 2e70 6f69 6e74 5f6d 6f64 6529 01da  ts.point_mode)..
-00000600: 0576 616c 7565 6302 0000 0000 0000 0000  .valuec.........
-00000610: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00000620: 2600 0000 7c01 7c00 5f00 7c00 a001 6401  &...|.|._.|...d.
-00000630: 7402 7c01 7403 8302 721c 7c01 6a04 6e02  t.|.t...r.|.j.n.
-00000640: 7c01 a102 0100 6400 5300 2902 4e5a 0970  |.....d.S.).NZ.p
-00000650: 6f69 6e74 4d6f 6465 2905 7225 0000 00da  ointMode).r%....
-00000660: 095f 7365 745f 6174 7472 da0a 6973 696e  ._set_attr..isin
-00000670: 7374 616e 6365 7209 0000 0072 2600 0000  stancer....r&...
-00000680: a902 7219 0000 0072 2600 0000 720f 0000  ..r....r&...r...
-00000690: 0072 0f00 0000 7210 0000 0072 1200 0000  .r....r....r....
-000006a0: 3000 0000 7308 0000 0000 0206 0104 0114  0...s...........
-000006b0: ff63 0100 0000 0000 0000 0000 0000 0100  .c..............
-000006c0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-000006d0: 006a 0053 0072 2400 0000 a901 721f 0000  .j.S.r$.....r...
-000006e0: 0072 1a00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-000006f0: 7210 0000 0072 0a00 0000 3800 0000 7302  r....r....8...s.
-00000700: 0000 0000 027a 0d50 6f69 6e74 732e 706f  .....z.Points.po
-00000710: 696e 7473 6302 0000 0000 0000 0000 0000  intsc...........
-00000720: 0002 0000 0002 0000 0043 0000 0073 1600  .........C...s..
-00000730: 0000 7c01 6400 7501 720c 7c01 6e02 6700  ..|.d.u.r.|.n.g.
-00000740: 7c00 5f00 6400 5300 7224 0000 0072 2a00  |._.d.S.r$...r*.
-00000750: 0000 7229 0000 0072 0f00 0000 720f 0000  ..r)...r....r...
-00000760: 0072 1000 0000 720a 0000 003c 0000 0073  .r....r....<...s
-00000770: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00000780: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00000790: 0600 0000 7c00 6a00 5300 7224 0000 00a9  ....|.j.S.r$....
-000007a0: 0172 2000 0000 721a 0000 0072 0f00 0000  .r ...r....r....
-000007b0: 720f 0000 0072 1000 0000 7213 0000 0041  r....r....r....A
-000007c0: 0000 0073 0200 0000 0002 7a0c 506f 696e  ...s......z.Poin
-000007d0: 7473 2e70 6169 6e74 6302 0000 0000 0000  ts.paintc.......
-000007e0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000007f0: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
-00000800: 7224 0000 0072 2b00 0000 7229 0000 0072  r$...r+...r)...r
-00000810: 0f00 0000 720f 0000 0072 1000 0000 7213  ....r....r....r.
-00000820: 0000 0045 0000 0073 0200 0000 0002 2907  ...E...s......).
-00000830: 4e4e 4e4e 4e4e 4e29 1372 0c00 0000 720d  NNNNNNN).r....r.
-00000840: 0000 0072 0e00 0000 7205 0000 0072 0400  ...r....r....r..
-00000850: 0000 7208 0000 0072 0900 0000 7207 0000  ..r....r....r...
-00000860: 00da 0462 6f6f 6c72 0300 0000 7218 0000  ...boolr....r...
-00000870: 0072 1b00 0000 721d 0000 00da 0870 726f  .r....r......pro
-00000880: 7065 7274 7972 1200 0000 da06 7365 7474  pertyr......sett
-00000890: 6572 720a 0000 0072 1300 0000 da0d 5f5f  err....r......__
-000008a0: 636c 6173 7363 656c 6c5f 5f72 0f00 0000  classcell__r....
-000008b0: 720f 0000 0072 2100 0000 7210 0000 0072  r....r!...r....r
-000008c0: 1100 0000 0f00 0000 733a 0000 0008 0300  ........s:......
-000008d0: 0100 0100 0400 0100 0100 0100 f502 020a  ................
-000008e0: 0106 0106 0506 0106 0102 f50c 1308 030c  ................
-000008f0: 0602 0114 0304 0114 0702 0118 0304 0118  ................
-00000900: 0402 0114 0304 0172 1100 0000 4e29 0eda  .......r....N)..
-00000910: 0465 6e75 6d72 0200 0000 da06 7479 7069  .enumr......typi
-00000920: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
-00000930: 00da 1666 6c65 745f 636f 7265 2e63 616e  ...flet_core.can
-00000940: 7661 732e 7368 6170 6572 0600 0000 da12  vas.shaper......
-00000950: 666c 6574 5f63 6f72 652e 7061 696e 7469  flet_core.painti
-00000960: 6e67 7207 0000 00da 0f66 6c65 745f 636f  ngr......flet_co
-00000970: 7265 2e74 7970 6573 7208 0000 0072 0900  re.typesr....r..
-00000980: 0000 7211 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000990: 0072 0f00 0000 7210 0000 00da 083c 6d6f  .r....r......<mo
-000009a0: 6475 6c65 3e01 0000 0073 0c00 0000 0c01  dule>....s......
-000009b0: 1402 0c01 0c01 0c03 1006                 ..........
+000001a0: 7463 6f6e 7472 6962 2f73 646b 2f70 7974  tcontrib/sdk/pyt
+000001b0: 686f 6e2f 7061 636b 6167 6573 2f66 6c65  hon/packages/fle
+000001c0: 742d 636f 7265 2f73 7263 2f66 6c65 745f  t-core/src/flet_
+000001d0: 636f 7265 2f63 616e 7661 732f 706f 696e  core/canvas/poin
+000001e0: 7473 2e70 7972 0900 0000 0900 0000 7306  ts.pyr........s.
+000001f0: 0000 0008 0104 0104 0172 0900 0000 6300  .........r....c.
+00000200: 0000 0000 0000 0000 0000 0000 0000 0008  ................
+00000210: 0000 0000 0000 0073 e800 0000 6500 5a01  .......s....e.Z.
+00000220: 6400 5a02 6414 6503 6504 6505 1900 1900  d.Z.d.e.e.e.....
+00000230: 6503 6506 1900 6503 6507 1900 6503 6508  e.e...e.e...e.e.
+00000240: 1900 6503 6508 1900 6509 6402 9c06 6403  ..e.e...e.d...d.
+00000250: 6404 8405 5a0a 6405 6406 8400 5a0b 8700  d...Z.d.d...Z...
+00000260: 6601 6407 6408 8408 5a0c 650d 6503 6506  f.d.d...Z.e.e.e.
+00000270: 1900 6409 9c01 640a 640b 8404 8301 5a0e  ..d...d.d.....Z.
+00000280: 650e 6a0f 6503 6506 1900 640c 9c01 640d  e.j.e.e...d...d.
+00000290: 640b 8404 8301 5a0e 650d 6503 6504 6505  d.....Z.e.e.e.e.
+000002a0: 1900 1900 6409 9c01 640e 640f 8404 8301  ....d...d.d.....
+000002b0: 5a10 6510 6a0f 6503 6504 6505 1900 1900  Z.e.j.e.e.e.....
+000002c0: 640c 9c01 6410 640f 8404 8301 5a10 650d  d...d.d.....Z.e.
+000002d0: 6503 6507 1900 6409 9c01 6411 6412 8404  e.e...d...d.d...
+000002e0: 8301 5a11 6511 6a0f 6503 6507 1900 640c  ..Z.e.j.e.e...d.
+000002f0: 9c01 6413 6412 8404 8301 5a11 8700 0400  ..d.d.....Z.....
+00000300: 5a12 5300 2915 da06 506f 696e 7473 4e29  Z.S.)...PointsN)
+00000310: 0672 0a00 0000 da0a 706f 696e 745f 6d6f  .r......point_mo
+00000320: 6465 da05 7061 696e 74da 0776 6973 6962  de..paint..visib
+00000330: 6c65 da08 6469 7361 626c 6564 da04 6461  le..disabled..da
+00000340: 7461 6308 0000 0000 0000 0000 0000 0008  tac.............
+00000350: 0000 0007 0000 0043 0000 0073 2a00 0000  .......C...s*...
+00000360: 7400 6a01 7c00 7c04 7c05 7c06 7c07 6401  t.j.|.|.|.|.|.d.
+00000370: 8d05 0100 7c01 7c00 5f02 7c02 7c00 5f03  ....|.|._.|.|._.
+00000380: 7c03 7c00 5f04 6400 5300 2902 4e29 04da  |.|._.d.S.).N)..
+00000390: 0372 6566 7214 0000 0072 1500 0000 7216  .refr....r....r.
+000003a0: 0000 0029 0572 0600 0000 da08 5f5f 696e  ...).r......__in
+000003b0: 6974 5f5f 720a 0000 0072 1200 0000 7213  it__r....r....r.
+000003c0: 0000 0029 08da 0473 656c 6672 0a00 0000  ...)...selfr....
+000003d0: 7212 0000 0072 1300 0000 7217 0000 0072  r....r....r....r
+000003e0: 1400 0000 7215 0000 0072 1600 0000 720f  ....r....r....r.
+000003f0: 0000 0072 0f00 0000 7210 0000 0072 1800  ...r....r....r..
+00000400: 0000 1000 0000 7308 0000 0000 0d14 0206  ......s.........
+00000410: 0106 017a 0f50 6f69 6e74 732e 5f5f 696e  ...z.Points.__in
+00000420: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00000430: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+00000440: 0000 6401 5300 2902 4e72 0a00 0000 720f  ..d.S.).Nr....r.
+00000450: 0000 00a9 0172 1900 0000 720f 0000 0072  .....r....r....r
+00000460: 0f00 0000 7210 0000 00da 115f 6765 745f  ....r......_get_
+00000470: 636f 6e74 726f 6c5f 6e61 6d65 2300 0000  control_name#...
+00000480: 7302 0000 0000 017a 1850 6f69 6e74 732e  s......z.Points.
+00000490: 5f67 6574 5f63 6f6e 7472 6f6c 5f6e 616d  _get_control_nam
+000004a0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+000004b0: 0000 0400 0000 0300 0000 732a 0000 0074  ..........s*...t
+000004c0: 0083 00a0 01a1 0001 007c 00a0 0264 017c  .........|...d.|
+000004d0: 006a 03a1 0201 007c 00a0 0264 027c 006a  .j.....|...d.|.j
+000004e0: 04a1 0201 0064 0053 0029 034e 720a 0000  .....d.S.).Nr...
+000004f0: 0072 1300 0000 2905 da05 7375 7065 72da  .r....)...super.
+00000500: 0d62 6566 6f72 655f 7570 6461 7465 da0e  .before_update..
+00000510: 5f73 6574 5f61 7474 725f 6a73 6f6e da0f  _set_attr_json..
+00000520: 5f50 6f69 6e74 735f 5f70 6f69 6e74 73da  _Points__points.
+00000530: 0e5f 506f 696e 7473 5f5f 7061 696e 7472  ._Points__paintr
+00000540: 1a00 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+00000550: 5f72 0f00 0000 7210 0000 0072 1d00 0000  _r....r....r....
+00000560: 2600 0000 7306 0000 0000 010a 010e 017a  &...s..........z
+00000570: 1450 6f69 6e74 732e 6265 666f 7265 5f75  .Points.before_u
+00000580: 7064 6174 6529 01da 0672 6574 7572 6e63  pdate)...returnc
+00000590: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000005a0: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+000005b0: 0053 00a9 014e 2901 da13 5f50 6f69 6e74  .S...N)..._Point
+000005c0: 735f 5f70 6f69 6e74 5f6d 6f64 6572 1a00  s__point_moder..
+000005d0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000005e0: 0072 1200 0000 2c00 0000 7302 0000 0000  .r....,...s.....
+000005f0: 027a 1150 6f69 6e74 732e 706f 696e 745f  .z.Points.point_
+00000600: 6d6f 6465 2901 da05 7661 6c75 6563 0200  mode)...valuec..
+00000610: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00000620: 0000 4300 0000 7326 0000 007c 017c 005f  ..C...s&...|.|._
+00000630: 007c 00a0 0164 0174 027c 0174 0383 0272  .|...d.t.|.t...r
+00000640: 1c7c 016a 046e 027c 01a1 0201 0064 0053  .|.j.n.|.....d.S
+00000650: 0029 024e 5a09 706f 696e 744d 6f64 6529  .).NZ.pointMode)
+00000660: 0572 2500 0000 da09 5f73 6574 5f61 7474  .r%....._set_att
+00000670: 72da 0a69 7369 6e73 7461 6e63 6572 0900  r..isinstancer..
+00000680: 0000 7226 0000 00a9 0272 1900 0000 7226  ..r&.....r....r&
+00000690: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000006a0: 0000 7212 0000 0030 0000 0073 0800 0000  ..r....0...s....
+000006b0: 0002 0601 0401 14ff 6301 0000 0000 0000  ........c.......
+000006c0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+000006d0: 0073 0600 0000 7c00 6a00 5300 7224 0000  .s....|.j.S.r$..
+000006e0: 00a9 0172 1f00 0000 721a 0000 0072 0f00  ...r....r....r..
+000006f0: 0000 720f 0000 0072 1000 0000 720a 0000  ..r....r....r...
+00000700: 0038 0000 0073 0200 0000 0002 7a0d 506f  .8...s......z.Po
+00000710: 696e 7473 2e70 6f69 6e74 7363 0200 0000  ints.pointsc....
+00000720: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000730: 4300 0000 7316 0000 007c 0164 0075 0172  C...s....|.d.u.r
+00000740: 0c7c 016e 0267 007c 005f 0064 0053 0072  .|.n.g.|._.d.S.r
+00000750: 2400 0000 722a 0000 0072 2900 0000 720f  $...r*...r)...r.
+00000760: 0000 0072 0f00 0000 7210 0000 0072 0a00  ...r....r....r..
+00000770: 0000 3c00 0000 7302 0000 0000 0263 0100  ..<...s......c..
+00000780: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000790: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+000007a0: 0072 2400 0000 a901 7220 0000 0072 1a00  .r$.....r ...r..
+000007b0: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+000007c0: 0072 1300 0000 4100 0000 7302 0000 0000  .r....A...s.....
+000007d0: 027a 0c50 6f69 6e74 732e 7061 696e 7463  .z.Points.paintc
+000007e0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000007f0: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
+00000800: 005f 0064 0053 0072 2400 0000 722b 0000  ._.d.S.r$...r+..
+00000810: 0072 2900 0000 720f 0000 0072 0f00 0000  .r)...r....r....
+00000820: 7210 0000 0072 1300 0000 4500 0000 7302  r....r....E...s.
+00000830: 0000 0000 0229 074e 4e4e 4e4e 4e4e 2913  .....).NNNNNNN).
+00000840: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000850: 0500 0000 7204 0000 0072 0800 0000 7209  ....r....r....r.
+00000860: 0000 0072 0700 0000 da04 626f 6f6c 7203  ...r......boolr.
+00000870: 0000 0072 1800 0000 721b 0000 0072 1d00  ...r....r....r..
+00000880: 0000 da08 7072 6f70 6572 7479 7212 0000  ....propertyr...
+00000890: 00da 0673 6574 7465 7272 0a00 0000 7213  ...setterr....r.
+000008a0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+000008b0: 5f5f 720f 0000 0072 0f00 0000 7221 0000  __r....r....r!..
+000008c0: 0072 1000 0000 7211 0000 000f 0000 0073  .r....r........s
+000008d0: 3a00 0000 0803 0001 0001 0004 0001 0001  :...............
+000008e0: 0001 00f5 0202 0a01 0601 0605 0601 0601  ................
+000008f0: 02f5 0c13 0803 0c06 0201 1403 0401 1407  ................
+00000900: 0201 1803 0401 1804 0201 1403 0401 7211  ..............r.
+00000910: 0000 004e 290e da04 656e 756d 7202 0000  ...N)...enumr...
+00000920: 00da 0674 7970 696e 6772 0300 0000 7204  ...typingr....r.
+00000930: 0000 0072 0500 0000 da16 666c 6574 5f63  ...r......flet_c
+00000940: 6f72 652e 6361 6e76 6173 2e73 6861 7065  ore.canvas.shape
+00000950: 7206 0000 00da 1266 6c65 745f 636f 7265  r......flet_core
+00000960: 2e70 6169 6e74 696e 6772 0700 0000 da0f  .paintingr......
+00000970: 666c 6574 5f63 6f72 652e 7479 7065 7372  flet_core.typesr
+00000980: 0800 0000 7209 0000 0072 1100 0000 720f  ....r....r....r.
+00000990: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000009a0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000009b0: 730c 0000 000c 0114 020c 010c 010c 0310  s...............
+000009c0: 06                                       .
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 2345 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 2909 0000  a........:)f)...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 2909 0000  a........./f)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 6504 8303 5a0b 6408  d.d...d.e...Z.d.
@@ -48,141 +48,142 @@
 000002f0: 0000 0029 0872 0400 0000 da08 5f5f 696e  ...).r......__in
 00000300: 6974 5f5f 7209 0000 0072 0a00 0000 720b  it__r....r....r.
 00000310: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
 00000320: 0000 290b da04 7365 6c66 7209 0000 0072  ..)...selfr....r
 00000330: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
 00000340: 0000 0072 0e00 0000 7212 0000 0072 0f00  ...r....r....r..
 00000350: 0000 7210 0000 0072 1100 0000 a900 7215  ..r....r......r.
-00000360: 0000 00fa 572f 776f 726b 7370 6163 6573  ....W/workspaces
+00000360: 0000 00fa 5e2f 776f 726b 7370 6163 6573  ....^/workspaces
 00000370: 2f63 6f6e 7472 6962 666c 6574 2f66 6c65  /contribflet/fle
-00000380: 742f 7364 6b2f 7079 7468 6f6e 2f70 6163  t/sdk/python/pac
-00000390: 6b61 6765 732f 666c 6574 2d63 6f72 652f  kages/flet-core/
-000003a0: 7372 632f 666c 6574 5f63 6f72 652f 6361  src/flet_core/ca
-000003b0: 6e76 6173 2f72 6563 742e 7079 7213 0000  nvas/rect.pyr...
-000003c0: 000a 0000 0073 0e00 0000 000e 1402 0601  .....s..........
-000003d0: 0601 0601 0601 0601 7a0d 5265 6374 2e5f  ........z.Rect._
-000003e0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-000003f0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00000400: 7304 0000 0064 0153 0029 024e da04 7265  s....d.S.).N..re
-00000410: 6374 7215 0000 00a9 0172 1400 0000 7215  ctr......r....r.
-00000420: 0000 0072 1500 0000 7216 0000 00da 115f  ...r....r......_
-00000430: 6765 745f 636f 6e74 726f 6c5f 6e61 6d65  get_control_name
-00000440: 2100 0000 7302 0000 0000 017a 1652 6563  !...s......z.Rec
-00000450: 742e 5f67 6574 5f63 6f6e 7472 6f6c 5f6e  t._get_control_n
-00000460: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-00000470: 0100 0000 0400 0000 0300 0000 732a 0000  ............s*..
-00000480: 0074 0083 00a0 01a1 0001 007c 00a0 0264  .t.........|...d
-00000490: 017c 006a 03a1 0201 007c 00a0 0264 027c  .|.j.....|...d.|
-000004a0: 006a 04a1 0201 0064 0053 0029 034e 5a0c  .j.....d.S.).NZ.
-000004b0: 626f 7264 6572 5261 6469 7573 720e 0000  borderRadiusr...
-000004c0: 0029 05da 0573 7570 6572 da0d 6265 666f  .)...super..befo
-000004d0: 7265 5f75 7064 6174 65da 0e5f 7365 745f  re_update.._set_
-000004e0: 6174 7472 5f6a 736f 6eda 145f 5265 6374  attr_json.._Rect
-000004f0: 5f5f 626f 7264 6572 5f72 6164 6975 73da  __border_radius.
-00000500: 0c5f 5265 6374 5f5f 7061 696e 7472 1800  ._Rect__paintr..
-00000510: 0000 a901 da09 5f5f 636c 6173 735f 5f72  ......__class__r
-00000520: 1500 0000 7216 0000 0072 1b00 0000 2400  ....r....r....$.
-00000530: 0000 7306 0000 0000 010a 010e 017a 1252  ..s..........z.R
-00000540: 6563 742e 6265 666f 7265 5f75 7064 6174  ect.before_updat
-00000550: 6529 01da 0672 6574 7572 6e63 0100 0000  e)...returnc....
-00000560: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000570: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
-00000580: 0153 00a9 024e 7209 0000 00a9 01da 095f  .S...Nr........_
-00000590: 6765 745f 6174 7472 7218 0000 0072 1500  get_attrr....r..
-000005a0: 0000 7215 0000 0072 1600 0000 7209 0000  ..r....r....r...
-000005b0: 002a 0000 0073 0200 0000 0002 7a06 5265  .*...s......z.Re
-000005c0: 6374 2e78 2901 da05 7661 6c75 6563 0200  ct.x)...valuec..
-000005d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000005e0: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-000005f0: 017c 01a1 0201 0064 0053 0072 2200 0000  .|.....d.S.r"...
-00000600: a901 da09 5f73 6574 5f61 7474 72a9 0272  ...._set_attr..r
-00000610: 1400 0000 7225 0000 0072 1500 0000 7215  ....r%...r....r.
-00000620: 0000 0072 1600 0000 7209 0000 002e 0000  ...r....r.......
-00000630: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000640: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000650: 0073 0a00 0000 7c00 a000 6401 a101 5300  .s....|...d...S.
-00000660: a902 4e72 0a00 0000 7223 0000 0072 1800  ..Nr....r#...r..
-00000670: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000680: 0072 0a00 0000 3300 0000 7302 0000 0000  .r....3...s.....
-00000690: 027a 0652 6563 742e 7963 0200 0000 0000  .z.Rect.yc......
-000006a0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-000006b0: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-000006c0: 0201 0064 0053 0072 2900 0000 7226 0000  ...d.S.r)...r&..
-000006d0: 0072 2800 0000 7215 0000 0072 1500 0000  .r(...r....r....
-000006e0: 7216 0000 0072 0a00 0000 3700 0000 7302  r....r....7...s.
-000006f0: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00000700: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
-00000710: 0000 007c 00a0 0064 01a1 0153 00a9 024e  ...|...d...S...N
-00000720: 720b 0000 0072 2300 0000 7218 0000 0072  r....r#...r....r
-00000730: 1500 0000 7215 0000 0072 1600 0000 720b  ....r....r....r.
-00000740: 0000 003c 0000 0073 0200 0000 0002 7a0a  ...<...s......z.
-00000750: 5265 6374 2e77 6964 7468 6302 0000 0000  Rect.widthc.....
-00000760: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000770: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
-00000780: a102 0100 6400 5300 722a 0000 0072 2600  ....d.S.r*...r&.
-00000790: 0000 7228 0000 0072 1500 0000 7215 0000  ..r(...r....r...
-000007a0: 0072 1600 0000 720b 0000 0040 0000 0073  .r....r....@...s
-000007b0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-000007c0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000007d0: 0a00 0000 7c00 a000 6401 a101 5300 a902  ....|...d...S...
-000007e0: 4e72 0c00 0000 7223 0000 0072 1800 0000  Nr....r#...r....
-000007f0: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000800: 0c00 0000 4500 0000 7302 0000 0000 027a  ....E...s......z
-00000810: 0b52 6563 742e 6865 6967 6874 6302 0000  .Rect.heightc...
-00000820: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000830: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-00000840: 7c01 a102 0100 6400 5300 722b 0000 0072  |.....d.S.r+...r
-00000850: 2600 0000 7228 0000 0072 1500 0000 7215  &...r(...r....r.
-00000860: 0000 0072 1600 0000 720c 0000 0049 0000  ...r....r....I..
-00000870: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000880: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000890: 0073 0600 0000 7c00 6a00 5300 a901 4ea9  .s....|.j.S...N.
-000008a0: 0172 1d00 0000 7218 0000 0072 1500 0000  .r....r....r....
-000008b0: 7215 0000 0072 1600 0000 720d 0000 004e  r....r....r....N
-000008c0: 0000 0073 0200 0000 0002 7a12 5265 6374  ...s......z.Rect
-000008d0: 2e62 6f72 6465 725f 7261 6469 7573 6302  .border_radiusc.
-000008e0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-000008f0: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
-00000900: 5f00 6400 5300 722c 0000 0072 2d00 0000  _.d.S.r,...r-...
-00000910: 7228 0000 0072 1500 0000 7215 0000 0072  r(...r....r....r
-00000920: 1600 0000 720d 0000 0052 0000 0073 0200  ....r....R...s..
-00000930: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000940: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000950: 0000 7c00 6a00 5300 722c 0000 00a9 0172  ..|.j.S.r,.....r
-00000960: 1e00 0000 7218 0000 0072 1500 0000 7215  ....r....r....r.
-00000970: 0000 0072 1600 0000 720e 0000 0057 0000  ...r....r....W..
-00000980: 0073 0200 0000 0002 7a0a 5265 6374 2e70  .s......z.Rect.p
-00000990: 6169 6e74 6302 0000 0000 0000 0000 0000  aintc...........
-000009a0: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-000009b0: 0000 7c01 7c00 5f00 6400 5300 722c 0000  ..|.|._.d.S.r,..
-000009c0: 0072 2e00 0000 7228 0000 0072 1500 0000  .r....r(...r....
-000009d0: 7215 0000 0072 1600 0000 720e 0000 005b  r....r....r....[
-000009e0: 0000 0073 0200 0000 0002 290a 4e4e 4e4e  ...s......).NNNN
-000009f0: 4e4e 4e4e 4e4e 2915 da08 5f5f 6e61 6d65  NNNNNN)...__name
-00000a00: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000a10: 5f5f 7175 616c 6e61 6d65 5f5f 7205 0000  __qualname__r...
-00000a20: 0072 0300 0000 7207 0000 0072 0600 0000  .r....r....r....
-00000a30: da04 626f 6f6c 7202 0000 0072 1300 0000  ..boolr....r....
-00000a40: 7219 0000 0072 1b00 0000 da08 7072 6f70  r....r......prop
-00000a50: 6572 7479 7209 0000 00da 0673 6574 7465  ertyr......sette
-00000a60: 7272 0a00 0000 720b 0000 0072 0c00 0000  rr....r....r....
-00000a70: 720d 0000 0072 0e00 0000 da0d 5f5f 636c  r....r......__cl
-00000a80: 6173 7363 656c 6c5f 5f72 1500 0000 7215  asscell__r....r.
-00000a90: 0000 0072 1f00 0000 7216 0000 0072 0800  ...r....r....r..
-00000aa0: 0000 0900 0000 735e 0000 0008 0300 0100  ......s^........
-00000ab0: 0100 0100 0100 0100 0200 0100 0100 0100  ................
-00000ac0: f402 0202 0102 0102 0102 0106 0106 0306  ................
-00000ad0: 0106 0102 f40c 1708 030c 0602 0110 0304  ................
-00000ae0: 0110 0402 0110 0304 0110 0402 0110 0304  ................
-00000af0: 0110 0402 0110 0304 0110 0402 0110 0304  ................
-00000b00: 0110 0402 0114 0304 0172 0800 0000 4e29  .........r....N)
-00000b10: 0cda 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
-00000b20: 0000 00da 1666 6c65 745f 636f 7265 2e63  .....flet_core.c
-00000b30: 616e 7661 732e 7368 6170 6572 0400 0000  anvas.shaper....
-00000b40: da11 666c 6574 5f63 6f72 652e 636f 6e74  ..flet_core.cont
-00000b50: 726f 6c72 0500 0000 da12 666c 6574 5f63  rolr......flet_c
-00000b60: 6f72 652e 7061 696e 7469 6e67 7206 0000  ore.paintingr...
-00000b70: 00da 0f66 6c65 745f 636f 7265 2e74 7970  ...flet_core.typ
-00000b80: 6573 7207 0000 0072 0800 0000 7215 0000  esr....r....r...
-00000b90: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000ba0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
-00000bb0: 0000 0010 020c 010c 010c 010c 03         .............
+00000380: 7463 6f6e 7472 6962 2f73 646b 2f70 7974  tcontrib/sdk/pyt
+00000390: 686f 6e2f 7061 636b 6167 6573 2f66 6c65  hon/packages/fle
+000003a0: 742d 636f 7265 2f73 7263 2f66 6c65 745f  t-core/src/flet_
+000003b0: 636f 7265 2f63 616e 7661 732f 7265 6374  core/canvas/rect
+000003c0: 2e70 7972 1300 0000 0a00 0000 730e 0000  .pyr........s...
+000003d0: 0000 0e14 0206 0106 0106 0106 0106 017a  ...............z
+000003e0: 0d52 6563 742e 5f5f 696e 6974 5f5f 6301  .Rect.__init__c.
+000003f0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000400: 0000 0043 0000 0073 0400 0000 6401 5300  ...C...s....d.S.
+00000410: 2902 4eda 0472 6563 7472 1500 0000 a901  ).N..rectr......
+00000420: 7214 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00000430: 1600 0000 da11 5f67 6574 5f63 6f6e 7472  ......_get_contr
+00000440: 6f6c 5f6e 616d 6521 0000 0073 0200 0000  ol_name!...s....
+00000450: 0001 7a16 5265 6374 2e5f 6765 745f 636f  ..z.Rect._get_co
+00000460: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
+00000470: 0000 0000 0000 0001 0000 0004 0000 0003  ................
+00000480: 0000 0073 2a00 0000 7400 8300 a001 a100  ...s*...t.......
+00000490: 0100 7c00 a002 6401 7c00 6a03 a102 0100  ..|...d.|.j.....
+000004a0: 7c00 a002 6402 7c00 6a04 a102 0100 6400  |...d.|.j.....d.
+000004b0: 5300 2903 4e5a 0c62 6f72 6465 7252 6164  S.).NZ.borderRad
+000004c0: 6975 7372 0e00 0000 2905 da05 7375 7065  iusr....)...supe
+000004d0: 72da 0d62 6566 6f72 655f 7570 6461 7465  r..before_update
+000004e0: da0e 5f73 6574 5f61 7474 725f 6a73 6f6e  .._set_attr_json
+000004f0: da14 5f52 6563 745f 5f62 6f72 6465 725f  .._Rect__border_
+00000500: 7261 6469 7573 da0c 5f52 6563 745f 5f70  radius.._Rect__p
+00000510: 6169 6e74 7218 0000 00a9 01da 095f 5f63  aintr........__c
+00000520: 6c61 7373 5f5f 7215 0000 0072 1600 0000  lass__r....r....
+00000530: 721b 0000 0024 0000 0073 0600 0000 0001  r....$...s......
+00000540: 0a01 0e01 7a12 5265 6374 2e62 6566 6f72  ....z.Rect.befor
+00000550: 655f 7570 6461 7465 2901 da06 7265 7475  e_update)...retu
+00000560: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
+00000570: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000580: 7c00 a000 6401 a101 5300 a902 4e72 0900  |...d...S...Nr..
+00000590: 0000 a901 da09 5f67 6574 5f61 7474 7272  ......_get_attrr
+000005a0: 1800 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+000005b0: 0000 0072 0900 0000 2a00 0000 7302 0000  ...r....*...s...
+000005c0: 0000 027a 0652 6563 742e 7829 01da 0576  ...z.Rect.x)...v
+000005d0: 616c 7565 6302 0000 0000 0000 0000 0000  aluec...........
+000005e0: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+000005f0: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+00000600: 5300 7222 0000 00a9 01da 095f 7365 745f  S.r"......._set_
+00000610: 6174 7472 a902 7214 0000 0072 2500 0000  attr..r....r%...
+00000620: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000630: 0900 0000 2e00 0000 7302 0000 0000 0263  ........s......c
+00000640: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000650: 0300 0000 4300 0000 730a 0000 007c 00a0  ....C...s....|..
+00000660: 0064 01a1 0153 00a9 024e 720a 0000 0072  .d...S...Nr....r
+00000670: 2300 0000 7218 0000 0072 1500 0000 7215  #...r....r....r.
+00000680: 0000 0072 1600 0000 720a 0000 0033 0000  ...r....r....3..
+00000690: 0073 0200 0000 0002 7a06 5265 6374 2e79  .s......z.Rect.y
+000006a0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000006b0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+000006c0: a000 6401 7c01 a102 0100 6400 5300 7229  ..d.|.....d.S.r)
+000006d0: 0000 0072 2600 0000 7228 0000 0072 1500  ...r&...r(...r..
+000006e0: 0000 7215 0000 0072 1600 0000 720a 0000  ..r....r....r...
+000006f0: 0037 0000 0073 0200 0000 0002 6301 0000  .7...s......c...
+00000700: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000710: 0043 0000 0073 0a00 0000 7c00 a000 6401  .C...s....|...d.
+00000720: a101 5300 a902 4e72 0b00 0000 7223 0000  ..S...Nr....r#..
+00000730: 0072 1800 0000 7215 0000 0072 1500 0000  .r....r....r....
+00000740: 7216 0000 0072 0b00 0000 3c00 0000 7302  r....r....<...s.
+00000750: 0000 0000 027a 0a52 6563 742e 7769 6474  .....z.Rect.widt
+00000760: 6863 0200 0000 0000 0000 0000 0000 0200  hc..............
+00000770: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
+00000780: 00a0 0064 017c 01a1 0201 0064 0053 0072  ...d.|.....d.S.r
+00000790: 2a00 0000 7226 0000 0072 2800 0000 7215  *...r&...r(...r.
+000007a0: 0000 0072 1500 0000 7216 0000 0072 0b00  ...r....r....r..
+000007b0: 0000 4000 0000 7302 0000 0000 0263 0100  ..@...s......c..
+000007c0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000007d0: 0000 4300 0000 730a 0000 007c 00a0 0064  ..C...s....|...d
+000007e0: 01a1 0153 00a9 024e 720c 0000 0072 2300  ...S...Nr....r#.
+000007f0: 0000 7218 0000 0072 1500 0000 7215 0000  ..r....r....r...
+00000800: 0072 1600 0000 720c 0000 0045 0000 0073  .r....r....E...s
+00000810: 0200 0000 0002 7a0b 5265 6374 2e68 6569  ......z.Rect.hei
+00000820: 6768 7463 0200 0000 0000 0000 0000 0000  ghtc............
+00000830: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+00000840: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+00000850: 0072 2b00 0000 7226 0000 0072 2800 0000  .r+...r&...r(...
+00000860: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000870: 0c00 0000 4900 0000 7302 0000 0000 0263  ....I...s......c
+00000880: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000890: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+000008a0: 0053 00a9 014e a901 721d 0000 0072 1800  .S...N..r....r..
+000008b0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000008c0: 0072 0d00 0000 4e00 0000 7302 0000 0000  .r....N...s.....
+000008d0: 027a 1252 6563 742e 626f 7264 6572 5f72  .z.Rect.border_r
+000008e0: 6164 6975 7363 0200 0000 0000 0000 0000  adiusc..........
+000008f0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000900: 0000 007c 017c 005f 0064 0053 0072 2c00  ...|.|._.d.S.r,.
+00000910: 0000 722d 0000 0072 2800 0000 7215 0000  ..r-...r(...r...
+00000920: 0072 1500 0000 7216 0000 0072 0d00 0000  .r....r....r....
+00000930: 5200 0000 7302 0000 0000 0263 0100 0000  R...s......c....
+00000940: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000950: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
+00000960: 2c00 0000 a901 721e 0000 0072 1800 0000  ,.....r....r....
+00000970: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000980: 0e00 0000 5700 0000 7302 0000 0000 027a  ....W...s......z
+00000990: 0a52 6563 742e 7061 696e 7463 0200 0000  .Rect.paintc....
+000009a0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+000009b0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+000009c0: 0053 0072 2c00 0000 722e 0000 0072 2800  .S.r,...r....r(.
+000009d0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000009e0: 0072 0e00 0000 5b00 0000 7302 0000 0000  .r....[...s.....
+000009f0: 0229 0a4e 4e4e 4e4e 4e4e 4e4e 4e29 15da  .).NNNNNNNNNN)..
+00000a00: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000a10: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000a20: 655f 5f72 0500 0000 7203 0000 0072 0700  e__r....r....r..
+00000a30: 0000 7206 0000 00da 0462 6f6f 6c72 0200  ..r......boolr..
+00000a40: 0000 7213 0000 0072 1900 0000 721b 0000  ..r....r....r...
+00000a50: 00da 0870 726f 7065 7274 7972 0900 0000  ...propertyr....
+00000a60: da06 7365 7474 6572 720a 0000 0072 0b00  ..setterr....r..
+00000a70: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000a80: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000a90: 7215 0000 0072 1500 0000 721f 0000 0072  r....r....r....r
+00000aa0: 1600 0000 7208 0000 0009 0000 0073 5e00  ....r........s^.
+00000ab0: 0000 0803 0001 0001 0001 0001 0001 0002  ................
+00000ac0: 0001 0001 0001 00f4 0202 0201 0201 0201  ................
+00000ad0: 0201 0601 0603 0601 0601 02f4 0c17 0803  ................
+00000ae0: 0c06 0201 1003 0401 1004 0201 1003 0401  ................
+00000af0: 1004 0201 1003 0401 1004 0201 1003 0401  ................
+00000b00: 1004 0201 1003 0401 1004 0201 1403 0401  ................
+00000b10: 7208 0000 004e 290c da06 7479 7069 6e67  r....N)...typing
+00000b20: 7202 0000 0072 0300 0000 da16 666c 6574  r....r......flet
+00000b30: 5f63 6f72 652e 6361 6e76 6173 2e73 6861  _core.canvas.sha
+00000b40: 7065 7204 0000 00da 1166 6c65 745f 636f  per......flet_co
+00000b50: 7265 2e63 6f6e 7472 6f6c 7205 0000 00da  re.controlr.....
+00000b60: 1266 6c65 745f 636f 7265 2e70 6169 6e74  .flet_core.paint
+00000b70: 696e 6772 0600 0000 da0f 666c 6574 5f63  ingr......flet_c
+00000b80: 6f72 652e 7479 7065 7372 0700 0000 7208  ore.typesr....r.
+00000b90: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
+00000ba0: 0000 7216 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000bb0: 3e01 0000 0073 0a00 0000 1002 0c01 0c01  >....s..........
+00000bc0: 0c01 0c03                                ....
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1951 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 9f07 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 9f07 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6507 8303 5a0a 6407 5300 2908 e900 0000  e...Z.d.S.).....
@@ -41,119 +41,119 @@
 00000280: 0029 024e 2904 da03 7265 6672 0d00 0000  .).N)...refr....
 00000290: 720e 0000 0072 0f00 0000 2906 7206 0000  r....r....).r...
 000002a0: 00da 085f 5f69 6e69 745f 5f72 0900 0000  ...__init__r....
 000002b0: 720a 0000 0072 0b00 0000 720c 0000 0029  r....r....r....)
 000002c0: 09da 0473 656c 6672 0900 0000 720a 0000  ...selfr....r...
 000002d0: 0072 0b00 0000 720c 0000 0072 1000 0000  .r....r....r....
 000002e0: 720d 0000 0072 0e00 0000 720f 0000 00a9  r....r....r.....
-000002f0: 0072 1300 0000 fa59 2f77 6f72 6b73 7061  .r.....Y/workspa
+000002f0: 0072 1300 0000 fa60 2f77 6f72 6b73 7061  .r.....`/workspa
 00000300: 6365 732f 636f 6e74 7269 6266 6c65 742f  ces/contribflet/
-00000310: 666c 6574 2f73 646b 2f70 7974 686f 6e2f  flet/sdk/python/
-00000320: 7061 636b 6167 6573 2f66 6c65 742d 636f  packages/flet-co
-00000330: 7265 2f73 7263 2f66 6c65 745f 636f 7265  re/src/flet_core
-00000340: 2f63 616e 7661 732f 7368 6164 6f77 2e70  /canvas/shadow.p
-00000350: 7972 1100 0000 0900 0000 730a 0000 0000  yr........s.....
-00000360: 0e14 0206 0106 0106 017a 0f53 6861 646f  .........z.Shado
-00000370: 772e 5f5f 696e 6974 5f5f 6301 0000 0000  w.__init__c.....
-00000380: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000390: 0000 0073 0400 0000 6401 5300 2902 4e5a  ...s....d.S.).NZ
-000003a0: 0673 6861 646f 7772 1300 0000 a901 7212  .shadowr......r.
-000003b0: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-000003c0: 0000 da11 5f67 6574 5f63 6f6e 7472 6f6c  ...._get_control
-000003d0: 5f6e 616d 651e 0000 0073 0200 0000 0001  _name....s......
-000003e0: 7a18 5368 6164 6f77 2e5f 6765 745f 636f  z.Shadow._get_co
-000003f0: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
-00000400: 0000 0000 0000 0001 0000 0004 0000 0003  ................
-00000410: 0000 0073 1c00 0000 7400 8300 a001 a100  ...s....t.......
-00000420: 0100 7c00 a002 6401 7c00 6a03 a102 0100  ..|...d.|.j.....
-00000430: 6400 5300 2902 4e72 0900 0000 2904 da05  d.S.).Nr....)...
-00000440: 7375 7065 72da 0d62 6566 6f72 655f 7570  super..before_up
-00000450: 6461 7465 da0e 5f73 6574 5f61 7474 725f  date.._set_attr_
-00000460: 6a73 6f6e da0d 5f53 6861 646f 775f 5f70  json.._Shadow__p
-00000470: 6174 6872 1500 0000 a901 da09 5f5f 636c  athr........__cl
-00000480: 6173 735f 5f72 1300 0000 7214 0000 0072  ass__r....r....r
-00000490: 1800 0000 2100 0000 7304 0000 0000 010a  ....!...s.......
-000004a0: 017a 1453 6861 646f 772e 6265 666f 7265  .z.Shadow.before
-000004b0: 5f75 7064 6174 6563 0100 0000 0000 0000  _updatec........
-000004c0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000004d0: 7306 0000 007c 006a 0053 00a9 014e a901  s....|.j.S...N..
-000004e0: 721a 0000 0072 1500 0000 7213 0000 0072  r....r....r....r
-000004f0: 1300 0000 7214 0000 0072 0900 0000 2600  ....r....r....&.
-00000500: 0000 7302 0000 0000 027a 0b53 6861 646f  ..s......z.Shado
-00000510: 772e 7061 7468 2901 da05 7661 6c75 6563  w.path)...valuec
-00000520: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000530: 0200 0000 4300 0000 7316 0000 007c 0164  ....C...s....|.d
-00000540: 0075 0172 0c7c 016e 0267 007c 005f 0064  .u.r.|.n.g.|._.d
-00000550: 0053 0072 1d00 0000 721e 0000 00a9 0272  .S.r....r......r
-00000560: 1200 0000 721f 0000 0072 1300 0000 7213  ....r....r....r.
-00000570: 0000 0072 1400 0000 7209 0000 002a 0000  ...r....r....*..
-00000580: 0073 0200 0000 0002 2901 da06 7265 7475  .s......)...retu
-00000590: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
-000005a0: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
-000005b0: 7c00 a000 6401 a101 5300 a902 4e72 0a00  |...d...S...Nr..
-000005c0: 0000 a901 da09 5f67 6574 5f61 7474 7272  ......_get_attrr
-000005d0: 1500 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-000005e0: 0000 0072 0a00 0000 2f00 0000 7302 0000  ...r..../...s...
-000005f0: 0000 027a 0c53 6861 646f 772e 636f 6c6f  ...z.Shadow.colo
-00000600: 7263 0200 0000 0000 0000 0000 0000 0200  rc..............
-00000610: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
-00000620: 00a0 0064 017c 01a1 0201 0064 0053 0072  ...d.|.....d.S.r
-00000630: 2200 0000 a901 da09 5f73 6574 5f61 7474  "......._set_att
-00000640: 7272 2000 0000 7213 0000 0072 1300 0000  rr ...r....r....
-00000650: 7214 0000 0072 0a00 0000 3300 0000 7302  r....r....3...s.
-00000660: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00000670: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
-00000680: 0000 007c 00a0 0064 01a1 0153 00a9 024e  ...|...d...S...N
-00000690: 720b 0000 0072 2300 0000 7215 0000 0072  r....r#...r....r
-000006a0: 1300 0000 7213 0000 0072 1400 0000 720b  ....r....r....r.
-000006b0: 0000 0038 0000 0073 0200 0000 0002 7a10  ...8...s......z.
-000006c0: 5368 6164 6f77 2e65 6c65 7661 7469 6f6e  Shadow.elevation
-000006d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000006e0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-000006f0: a000 6401 7c01 a102 0100 6400 5300 7227  ..d.|.....d.S.r'
-00000700: 0000 0072 2500 0000 7220 0000 0072 1300  ...r%...r ...r..
-00000710: 0000 7213 0000 0072 1400 0000 720b 0000  ..r....r....r...
-00000720: 003c 0000 0073 0200 0000 0002 6301 0000  .<...s......c...
-00000730: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00000740: 0043 0000 0073 1000 0000 7c00 6a00 6401  .C...s....|.j.d.
-00000750: 6402 6403 6404 8d03 5300 2905 4eda 1374  d.d.d...S.).N..t
-00000760: 7261 6e73 7061 7265 6e74 4f63 636c 7564  ransparentOcclud
-00000770: 6572 da04 626f 6f6c 4629 02da 0964 6174  er..boolF)...dat
-00000780: 615f 7479 7065 da09 6465 665f 7661 6c75  a_type..def_valu
-00000790: 6572 2300 0000 7215 0000 0072 1300 0000  er#...r....r....
-000007a0: 7213 0000 0072 1400 0000 720c 0000 0041  r....r....r....A
-000007b0: 0000 0073 0200 0000 0002 7a1b 5368 6164  ...s......z.Shad
-000007c0: 6f77 2e74 7261 6e73 7061 7265 6e74 5f6f  ow.transparent_o
-000007d0: 6363 6c75 6465 7263 0200 0000 0000 0000  ccluderc........
-000007e0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-000007f0: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00000800: 0064 0053 0029 024e 7228 0000 0072 2500  .d.S.).Nr(...r%.
-00000810: 0000 7220 0000 0072 1300 0000 7213 0000  ..r ...r....r...
-00000820: 0072 1400 0000 720c 0000 0045 0000 0073  .r....r....E...s
-00000830: 0200 0000 0002 2908 4e4e 4e4e 4e4e 4e4e  ......).NNNNNNNN
-00000840: 2915 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000850: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000860: 6e61 6d65 5f5f 7204 0000 0072 0300 0000  name__r....r....
-00000870: 7205 0000 00da 0b50 6174 6845 6c65 6d65  r......PathEleme
-00000880: 6e74 da03 7374 7272 0700 0000 7229 0000  nt..strr....r)..
-00000890: 0072 0200 0000 7211 0000 0072 1600 0000  .r....r....r....
-000008a0: 7218 0000 00da 0870 726f 7065 7274 7972  r......propertyr
-000008b0: 0900 0000 da06 7365 7474 6572 720a 0000  ......setterr...
-000008c0: 0072 0b00 0000 720c 0000 00da 0d5f 5f63  .r....r......__c
-000008d0: 6c61 7373 6365 6c6c 5f5f 7213 0000 0072  lasscell__r....r
-000008e0: 1300 0000 721b 0000 0072 1400 0000 7208  ....r....r....r.
-000008f0: 0000 0008 0000 0073 4600 0000 0803 0001  .......sF.......
-00000900: 0001 0001 0004 0001 0001 0001 00f4 0202  ................
-00000910: 0c01 0601 0201 0605 0601 0601 02f4 0c15  ................
-00000920: 0803 0c05 0201 0a03 0401 1a04 0201 1403  ................
-00000930: 0401 1404 0201 1003 0401 1004 0201 1403  ................
-00000940: 0401 7208 0000 004e 290b da06 7479 7069  ..r....N)...typi
-00000950: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
-00000960: 00da 1566 6c65 745f 636f 7265 2e63 616e  ...flet_core.can
-00000970: 7661 732e 7061 7468 7205 0000 00da 1666  vas.pathr......f
-00000980: 6c65 745f 636f 7265 2e63 616e 7661 732e  let_core.canvas.
-00000990: 7368 6170 6572 0600 0000 da11 666c 6574  shaper......flet
-000009a0: 5f63 6f72 652e 636f 6e74 726f 6c72 0700  _core.controlr..
-000009b0: 0000 7208 0000 0072 1300 0000 7213 0000  ..r....r....r...
-000009c0: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
-000009d0: 6475 6c65 3e01 0000 0073 0800 0000 1402  dule>....s......
-000009e0: 0c01 0c01 0c03                           ......
+00000310: 666c 6574 636f 6e74 7269 622f 7364 6b2f  fletcontrib/sdk/
+00000320: 7079 7468 6f6e 2f70 6163 6b61 6765 732f  python/packages/
+00000330: 666c 6574 2d63 6f72 652f 7372 632f 666c  flet-core/src/fl
+00000340: 6574 5f63 6f72 652f 6361 6e76 6173 2f73  et_core/canvas/s
+00000350: 6861 646f 772e 7079 7211 0000 0009 0000  hadow.pyr.......
+00000360: 0073 0a00 0000 000e 1402 0601 0601 0601  .s..............
+00000370: 7a0f 5368 6164 6f77 2e5f 5f69 6e69 745f  z.Shadow.__init_
+00000380: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000390: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
+000003a0: 0153 0029 024e 5a06 7368 6164 6f77 7213  .S.).NZ.shadowr.
+000003b0: 0000 00a9 0172 1200 0000 7213 0000 0072  .....r....r....r
+000003c0: 1300 0000 7214 0000 00da 115f 6765 745f  ....r......_get_
+000003d0: 636f 6e74 726f 6c5f 6e61 6d65 1e00 0000  control_name....
+000003e0: 7302 0000 0000 017a 1853 6861 646f 772e  s......z.Shadow.
+000003f0: 5f67 6574 5f63 6f6e 7472 6f6c 5f6e 616d  _get_control_nam
+00000400: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+00000410: 0000 0400 0000 0300 0000 731c 0000 0074  ..........s....t
+00000420: 0083 00a0 01a1 0001 007c 00a0 0264 017c  .........|...d.|
+00000430: 006a 03a1 0201 0064 0053 0029 024e 7209  .j.....d.S.).Nr.
+00000440: 0000 0029 04da 0573 7570 6572 da0d 6265  ...)...super..be
+00000450: 666f 7265 5f75 7064 6174 65da 0e5f 7365  fore_update.._se
+00000460: 745f 6174 7472 5f6a 736f 6eda 0d5f 5368  t_attr_json.._Sh
+00000470: 6164 6f77 5f5f 7061 7468 7215 0000 00a9  adow__pathr.....
+00000480: 01da 095f 5f63 6c61 7373 5f5f 7213 0000  ...__class__r...
+00000490: 0072 1400 0000 7218 0000 0021 0000 0073  .r....r....!...s
+000004a0: 0400 0000 0001 0a01 7a14 5368 6164 6f77  ........z.Shadow
+000004b0: 2e62 6566 6f72 655f 7570 6461 7465 6301  .before_updatec.
+000004c0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+000004d0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+000004e0: 5300 a901 4ea9 0172 1a00 0000 7215 0000  S...N..r....r...
+000004f0: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000500: 7209 0000 0026 0000 0073 0200 0000 0002  r....&...s......
+00000510: 7a0b 5368 6164 6f77 2e70 6174 6829 01da  z.Shadow.path)..
+00000520: 0576 616c 7565 6302 0000 0000 0000 0000  .valuec.........
+00000530: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000540: 1600 0000 7c01 6400 7501 720c 7c01 6e02  ....|.d.u.r.|.n.
+00000550: 6700 7c00 5f00 6400 5300 721d 0000 0072  g.|._.d.S.r....r
+00000560: 1e00 0000 a902 7212 0000 0072 1f00 0000  ......r....r....
+00000570: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000580: 0900 0000 2a00 0000 7302 0000 0000 0229  ....*...s......)
+00000590: 01da 0672 6574 7572 6e63 0100 0000 0000  ...returnc......
+000005a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000005b0: 0000 730a 0000 007c 00a0 0064 01a1 0153  ..s....|...d...S
+000005c0: 00a9 024e 720a 0000 00a9 01da 095f 6765  ...Nr........_ge
+000005d0: 745f 6174 7472 7215 0000 0072 1300 0000  t_attrr....r....
+000005e0: 7213 0000 0072 1400 0000 720a 0000 002f  r....r....r..../
+000005f0: 0000 0073 0200 0000 0002 7a0c 5368 6164  ...s......z.Shad
+00000600: 6f77 2e63 6f6c 6f72 6302 0000 0000 0000  ow.colorc.......
+00000610: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000620: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
+00000630: 0100 6400 5300 7222 0000 00a9 01da 095f  ..d.S.r"......._
+00000640: 7365 745f 6174 7472 7220 0000 0072 1300  set_attrr ...r..
+00000650: 0000 7213 0000 0072 1400 0000 720a 0000  ..r....r....r...
+00000660: 0033 0000 0073 0200 0000 0002 6301 0000  .3...s......c...
+00000670: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000680: 0043 0000 0073 0a00 0000 7c00 a000 6401  .C...s....|...d.
+00000690: a101 5300 a902 4e72 0b00 0000 7223 0000  ..S...Nr....r#..
+000006a0: 0072 1500 0000 7213 0000 0072 1300 0000  .r....r....r....
+000006b0: 7214 0000 0072 0b00 0000 3800 0000 7302  r....r....8...s.
+000006c0: 0000 0000 027a 1053 6861 646f 772e 656c  .....z.Shadow.el
+000006d0: 6576 6174 696f 6e63 0200 0000 0000 0000  evationc........
+000006e0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+000006f0: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
+00000700: 0064 0053 0072 2700 0000 7225 0000 0072  .d.S.r'...r%...r
+00000710: 2000 0000 7213 0000 0072 1300 0000 7214   ...r....r....r.
+00000720: 0000 0072 0b00 0000 3c00 0000 7302 0000  ...r....<...s...
+00000730: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00000740: 0100 0000 0500 0000 4300 0000 7310 0000  ........C...s...
+00000750: 007c 006a 0064 0164 0264 0364 048d 0353  .|.j.d.d.d.d...S
+00000760: 0029 054e da13 7472 616e 7370 6172 656e  .).N..transparen
+00000770: 744f 6363 6c75 6465 72da 0462 6f6f 6c46  tOccluder..boolF
+00000780: 2902 da09 6461 7461 5f74 7970 65da 0964  )...data_type..d
+00000790: 6566 5f76 616c 7565 7223 0000 0072 1500  ef_valuer#...r..
+000007a0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+000007b0: 0072 0c00 0000 4100 0000 7302 0000 0000  .r....A...s.....
+000007c0: 027a 1b53 6861 646f 772e 7472 616e 7370  .z.Shadow.transp
+000007d0: 6172 656e 745f 6f63 636c 7564 6572 6302  arent_occluderc.
+000007e0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000007f0: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00000800: 6401 7c01 a102 0100 6400 5300 2902 4e72  d.|.....d.S.).Nr
+00000810: 2800 0000 7225 0000 0072 2000 0000 7213  (...r%...r ...r.
+00000820: 0000 0072 1300 0000 7214 0000 0072 0c00  ...r....r....r..
+00000830: 0000 4500 0000 7302 0000 0000 0229 084e  ..E...s......).N
+00000840: 4e4e 4e4e 4e4e 4e29 15da 085f 5f6e 616d  NNNNNNN)...__nam
+00000850: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000860: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0400  .__qualname__r..
+00000870: 0000 7203 0000 0072 0500 0000 da0b 5061  ..r....r......Pa
+00000880: 7468 456c 656d 656e 74da 0373 7472 7207  thElement..strr.
+00000890: 0000 0072 2900 0000 7202 0000 0072 1100  ...r)...r....r..
+000008a0: 0000 7216 0000 0072 1800 0000 da08 7072  ..r....r......pr
+000008b0: 6f70 6572 7479 7209 0000 00da 0673 6574  opertyr......set
+000008c0: 7465 7272 0a00 0000 720b 0000 0072 0c00  terr....r....r..
+000008d0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+000008e0: 5f72 1300 0000 7213 0000 0072 1b00 0000  _r....r....r....
+000008f0: 7214 0000 0072 0800 0000 0800 0000 7346  r....r........sF
+00000900: 0000 0008 0300 0100 0100 0100 0400 0100  ................
+00000910: 0100 0100 f402 020c 0106 0102 0106 0506  ................
+00000920: 0106 0102 f40c 1508 030c 0502 010a 0304  ................
+00000930: 011a 0402 0114 0304 0114 0402 0110 0304  ................
+00000940: 0110 0402 0114 0304 0172 0800 0000 4e29  .........r....N)
+00000950: 0bda 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
+00000960: 0000 0072 0400 0000 da15 666c 6574 5f63  ...r......flet_c
+00000970: 6f72 652e 6361 6e76 6173 2e70 6174 6872  ore.canvas.pathr
+00000980: 0500 0000 da16 666c 6574 5f63 6f72 652e  ......flet_core.
+00000990: 6361 6e76 6173 2e73 6861 7065 7206 0000  canvas.shaper...
+000009a0: 00da 1166 6c65 745f 636f 7265 2e63 6f6e  ...flet_core.con
+000009b0: 7472 6f6c 7207 0000 0072 0800 0000 7213  trolr....r....r.
+000009c0: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+000009d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000009e0: 7308 0000 0014 020c 010c 010c 03         s............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/__pycache__/text.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/__pycache__/text.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 4172 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 4c10 0000  a........:)fL...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 4c10 0000  a........./fL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
@@ -77,229 +77,230 @@
 000004c0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
 000004d0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
 000004e0: 2910 da04 7365 6c66 720c 0000 0072 0d00  )...selfr....r..
 000004f0: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
 00000500: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
 00000510: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
 00000520: 1a00 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
-00000530: 0000 00a9 0072 1d00 0000 fa57 2f77 6f72  .....r.....W/wor
+00000530: 0000 00a9 0072 1d00 0000 fa5e 2f77 6f72  .....r.....^/wor
 00000540: 6b73 7061 6365 732f 636f 6e74 7269 6266  kspaces/contribf
-00000550: 6c65 742f 666c 6574 2f73 646b 2f70 7974  let/flet/sdk/pyt
-00000560: 686f 6e2f 7061 636b 6167 6573 2f66 6c65  hon/packages/fle
-00000570: 742d 636f 7265 2f73 7263 2f66 6c65 745f  t-core/src/flet_
-00000580: 636f 7265 2f63 616e 7661 732f 7465 7874  core/canvas/text
-00000590: 2e70 7972 1b00 0000 0c00 0000 7318 0000  .pyr........s...
-000005a0: 0000 1514 0206 0106 0106 0106 0106 0106  ................
-000005b0: 0106 0106 0106 0106 017a 0d54 6578 742e  .........z.Text.
-000005c0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-000005d0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000005e0: 0073 0400 0000 6401 5300 a902 4e72 0e00  .s....d.S...Nr..
-000005f0: 0000 721d 0000 00a9 0172 1c00 0000 721d  ..r......r....r.
-00000600: 0000 0072 1d00 0000 721e 0000 00da 115f  ...r....r......_
-00000610: 6765 745f 636f 6e74 726f 6c5f 6e61 6d65  get_control_name
-00000620: 2f00 0000 7302 0000 0000 017a 1654 6578  /...s......z.Tex
-00000630: 742e 5f67 6574 5f63 6f6e 7472 6f6c 5f6e  t._get_control_n
-00000640: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-00000650: 0200 0000 0300 0000 4300 0000 7314 0000  ........C...s...
-00000660: 0067 007d 017c 01a0 007c 006a 01a1 0101  .g.}.|...|.j....
-00000670: 007c 0153 00a9 014e 2902 da06 6578 7465  .|.S...N)...exte
-00000680: 6e64 da0c 5f54 6578 745f 5f73 7061 6e73  nd.._Text__spans
-00000690: 2902 721c 0000 00da 0863 6869 6c64 7265  ).r......childre
-000006a0: 6e72 1d00 0000 721d 0000 0072 1e00 0000  nr....r....r....
-000006b0: da0d 5f67 6574 5f63 6869 6c64 7265 6e32  .._get_children2
-000006c0: 0000 0073 0600 0000 0001 0401 0c01 7a12  ...s..........z.
-000006d0: 5465 7874 2e5f 6765 745f 6368 696c 6472  Text._get_childr
-000006e0: 656e 6301 0000 0000 0000 0000 0000 0001  enc.............
-000006f0: 0000 0004 0000 0003 0000 0073 2a00 0000  ...........s*...
-00000700: 7400 8300 a001 a100 0100 7c00 a002 6401  t.........|...d.
-00000710: 7c00 6a03 a102 0100 7c00 a002 6402 7c00  |.j.....|...d.|.
-00000720: 6a04 a102 0100 6400 5300 2903 4e72 0f00  j.....d.S.).Nr..
-00000730: 0000 7211 0000 0029 05da 0573 7570 6572  ..r....)...super
-00000740: da0d 6265 666f 7265 5f75 7064 6174 65da  ..before_update.
-00000750: 0e5f 7365 745f 6174 7472 5f6a 736f 6eda  ._set_attr_json.
-00000760: 0c5f 5465 7874 5f5f 7374 796c 65da 105f  ._Text__style.._
-00000770: 5465 7874 5f5f 616c 6967 6e6d 656e 7472  Text__alignmentr
-00000780: 2000 0000 a901 da09 5f5f 636c 6173 735f   .......__class_
-00000790: 5f72 1d00 0000 721e 0000 0072 2800 0000  _r....r....r(...
-000007a0: 3700 0000 7306 0000 0000 010a 010e 017a  7...s..........z
-000007b0: 1254 6578 742e 6265 666f 7265 5f75 7064  .Text.before_upd
-000007c0: 6174 6529 01da 0672 6574 7572 6e63 0100  ate)...returnc..
-000007d0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000007e0: 0000 4300 0000 730a 0000 007c 00a0 0064  ..C...s....|...d
-000007f0: 01a1 0153 00a9 024e 720c 0000 00a9 01da  ...S...Nr.......
-00000800: 095f 6765 745f 6174 7472 7220 0000 0072  ._get_attrr ...r
-00000810: 1d00 0000 721d 0000 0072 1e00 0000 720c  ....r....r....r.
-00000820: 0000 003d 0000 0073 0200 0000 0002 7a06  ...=...s......z.
-00000830: 5465 7874 2e78 2901 da05 7661 6c75 6563  Text.x)...valuec
-00000840: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000850: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
-00000860: 0064 017c 01a1 0201 0064 0053 0072 2f00  .d.|.....d.S.r/.
-00000870: 0000 a901 da09 5f73 6574 5f61 7474 72a9  ......_set_attr.
-00000880: 0272 1c00 0000 7232 0000 0072 1d00 0000  .r....r2...r....
-00000890: 721d 0000 0072 1e00 0000 720c 0000 0041  r....r....r....A
-000008a0: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-000008b0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-000008c0: 0000 0073 0a00 0000 7c00 a000 6401 a101  ...s....|...d...
-000008d0: 5300 a902 4e72 0d00 0000 7230 0000 0072  S...Nr....r0...r
-000008e0: 2000 0000 721d 0000 0072 1d00 0000 721e   ...r....r....r.
-000008f0: 0000 0072 0d00 0000 4600 0000 7302 0000  ...r....F...s...
-00000900: 0000 027a 0654 6578 742e 7963 0200 0000  ...z.Text.yc....
-00000910: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000920: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
-00000930: 01a1 0201 0064 0053 0072 3600 0000 7233  .....d.S.r6...r3
-00000940: 0000 0072 3500 0000 721d 0000 0072 1d00  ...r5...r....r..
-00000950: 0000 721e 0000 0072 0d00 0000 4a00 0000  ..r....r....J...
-00000960: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00000970: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00000980: 730a 0000 007c 00a0 0064 01a1 0153 0072  s....|...d...S.r
-00000990: 1f00 0000 7230 0000 0072 2000 0000 721d  ....r0...r ...r.
-000009a0: 0000 0072 1d00 0000 721e 0000 0072 0e00  ...r....r....r..
-000009b0: 0000 4f00 0000 7302 0000 0000 027a 0954  ..O...s......z.T
-000009c0: 6578 742e 7465 7874 6302 0000 0000 0000  ext.textc.......
-000009d0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000009e0: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
-000009f0: 0100 6400 5300 721f 0000 0072 3300 0000  ..d.S.r....r3...
-00000a00: 7235 0000 0072 1d00 0000 721d 0000 0072  r5...r....r....r
-00000a10: 1e00 0000 720e 0000 0053 0000 0073 0200  ....r....S...s..
-00000a20: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000a30: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000a40: 0000 7c00 6a00 5300 7222 0000 00a9 0172  ..|.j.S.r".....r
-00000a50: 2a00 0000 7220 0000 0072 1d00 0000 721d  *...r ...r....r.
-00000a60: 0000 0072 1e00 0000 720f 0000 0058 0000  ...r....r....X..
-00000a70: 0073 0200 0000 0002 7a0a 5465 7874 2e73  .s......z.Text.s
-00000a80: 7479 6c65 6302 0000 0000 0000 0000 0000  tylec...........
-00000a90: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00000aa0: 0000 7c01 7c00 5f00 6400 5300 7222 0000  ..|.|._.d.S.r"..
-00000ab0: 0072 3700 0000 7235 0000 0072 1d00 0000  .r7...r5...r....
-00000ac0: 721d 0000 0072 1e00 0000 720f 0000 005c  r....r....r....\
-00000ad0: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-00000ae0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000af0: 0000 0073 0600 0000 7c00 6a00 5300 7222  ...s....|.j.S.r"
-00000b00: 0000 00a9 0172 2400 0000 7220 0000 0072  .....r$...r ...r
-00000b10: 1d00 0000 721d 0000 0072 1e00 0000 7210  ....r....r....r.
-00000b20: 0000 0061 0000 0073 0200 0000 0002 7a0a  ...a...s......z.
-00000b30: 5465 7874 2e73 7061 6e73 6302 0000 0000  Text.spansc.....
-00000b40: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000b50: 0000 0073 1600 0000 7c01 6400 7501 720c  ...s....|.d.u.r.
-00000b60: 7c01 6e02 6700 7c00 5f00 6400 5300 7222  |.n.g.|._.d.S.r"
-00000b70: 0000 0072 3800 0000 7235 0000 0072 1d00  ...r8...r5...r..
-00000b80: 0000 721d 0000 0072 1e00 0000 7210 0000  ..r....r....r...
-00000b90: 0065 0000 0073 0200 0000 0002 6301 0000  .e...s......c...
-00000ba0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00000bb0: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00000bc0: 7222 0000 00a9 0172 2b00 0000 7220 0000  r".....r+...r ..
-00000bd0: 0072 1d00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000be0: 7211 0000 006a 0000 0073 0200 0000 0002  r....j...s......
-00000bf0: 7a0e 5465 7874 2e61 6c69 676e 6d65 6e74  z.Text.alignment
-00000c00: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000c10: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00000c20: 7c00 5f00 6400 5300 7222 0000 0072 3900  |._.d.S.r"...r9.
-00000c30: 0000 7235 0000 0072 1d00 0000 721d 0000  ..r5...r....r...
-00000c40: 0072 1e00 0000 7211 0000 006e 0000 0073  .r....r....n...s
-00000c50: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00000c60: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00000c70: 0600 0000 7c00 6a00 5300 7222 0000 0029  ....|.j.S.r"...)
-00000c80: 01da 115f 5465 7874 5f5f 7465 7874 5f61  ..._Text__text_a
-00000c90: 6c69 676e 7220 0000 0072 1d00 0000 721d  lignr ...r....r.
-00000ca0: 0000 0072 1e00 0000 7212 0000 0073 0000  ...r....r....s..
-00000cb0: 0073 0200 0000 0002 7a0f 5465 7874 2e74  .s......z.Text.t
-00000cc0: 6578 745f 616c 6967 6e63 0200 0000 0000  ext_alignc......
-00000cd0: 0000 0000 0000 0200 0000 0600 0000 4300  ..............C.
-00000ce0: 0000 7326 0000 007c 017c 005f 007c 00a0  ..s&...|.|._.|..
-00000cf0: 0164 0174 027c 0174 0383 0272 1c7c 016a  .d.t.|.t...r.|.j
-00000d00: 046e 027c 01a1 0201 0064 0053 0029 024e  .n.|.....d.S.).N
-00000d10: 5a09 7465 7874 416c 6967 6e29 0572 3a00  Z.textAlign).r:.
-00000d20: 0000 7234 0000 00da 0a69 7369 6e73 7461  ..r4.....isinsta
-00000d30: 6e63 6572 0a00 0000 7232 0000 0072 3500  ncer....r2...r5.
-00000d40: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000d50: 0072 1200 0000 7700 0000 7308 0000 0000  .r....w...s.....
-00000d60: 0206 0104 0114 ff63 0100 0000 0000 0000  .......c........
-00000d70: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00000d80: 730a 0000 007c 00a0 0064 01a1 0153 00a9  s....|...d...S..
-00000d90: 024e 5a08 6d61 784c 696e 6573 7230 0000  .NZ.maxLinesr0..
-00000da0: 0072 2000 0000 721d 0000 0072 1d00 0000  .r ...r....r....
-00000db0: 721e 0000 0072 1300 0000 7f00 0000 7302  r....r........s.
-00000dc0: 0000 0000 027a 0e54 6578 742e 6d61 785f  .....z.Text.max_
-00000dd0: 6c69 6e65 7363 0200 0000 0000 0000 0000  linesc..........
-00000de0: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
-00000df0: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
-00000e00: 0053 0072 3c00 0000 7233 0000 0072 3500  .S.r<...r3...r5.
-00000e10: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000e20: 0072 1300 0000 8300 0000 7302 0000 0000  .r........s.....
-00000e30: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000e40: 0000 0300 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000e50: 00a0 0064 01a1 0153 00a9 024e 5a08 6d61  ...d...S...NZ.ma
-00000e60: 7857 6964 7468 7230 0000 0072 2000 0000  xWidthr0...r ...
-00000e70: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000e80: 1400 0000 8800 0000 7302 0000 0000 027a  ........s......z
-00000e90: 0e54 6578 742e 6d61 785f 7769 6474 6863  .Text.max_widthc
-00000ea0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000eb0: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
-00000ec0: 0064 017c 01a1 0201 0064 0053 0072 3d00  .d.|.....d.S.r=.
-00000ed0: 0000 7233 0000 0072 3500 0000 721d 0000  ..r3...r5...r...
-00000ee0: 0072 1d00 0000 721e 0000 0072 1400 0000  .r....r....r....
-00000ef0: 8c00 0000 7302 0000 0000 0263 0100 0000  ....s......c....
-00000f00: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000f10: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
-00000f20: 0153 00a9 024e 7215 0000 0072 3000 0000  .S...Nr....r0...
-00000f30: 7220 0000 0072 1d00 0000 721d 0000 0072  r ...r....r....r
-00000f40: 1e00 0000 7215 0000 0091 0000 0073 0200  ....r........s..
-00000f50: 0000 0002 7a0d 5465 7874 2e65 6c6c 6970  ....z.Text.ellip
-00000f60: 7369 7363 0200 0000 0000 0000 0000 0000  sisc............
-00000f70: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-00000f80: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
-00000f90: 0072 3e00 0000 7233 0000 0072 3500 0000  .r>...r3...r5...
-00000fa0: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000fb0: 1500 0000 9500 0000 7302 0000 0000 0263  ........s......c
-00000fc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000fd0: 0300 0000 4300 0000 730a 0000 007c 00a0  ....C...s....|..
-00000fe0: 0064 01a1 0153 00a9 024e 7216 0000 0072  .d...S...Nr....r
-00000ff0: 3000 0000 7220 0000 0072 1d00 0000 721d  0...r ...r....r.
-00001000: 0000 0072 1e00 0000 7216 0000 009a 0000  ...r....r.......
-00001010: 0073 0200 0000 0002 7a0b 5465 7874 2e72  .s......z.Text.r
-00001020: 6f74 6174 6563 0200 0000 0000 0000 0000  otatec..........
-00001030: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
-00001040: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
-00001050: 0053 0072 3f00 0000 7233 0000 0072 3500  .S.r?...r3...r5.
-00001060: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00001070: 0072 1600 0000 9e00 0000 7302 0000 0000  .r........s.....
-00001080: 0229 0f4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  .).NNNNNNNNNNNNN
-00001090: 4e4e 2920 da08 5f5f 6e61 6d65 5f5f da0a  NN) ..__name__..
-000010a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000010b0: 616c 6e61 6d65 5f5f 7207 0000 0072 0400  alname__r....r..
-000010c0: 0000 da03 7374 7272 0900 0000 7203 0000  ....strr....r...
-000010d0: 0072 0800 0000 7205 0000 0072 0a00 0000  .r....r....r....
-000010e0: da03 696e 74da 0462 6f6f 6c72 0200 0000  ..int..boolr....
-000010f0: 721b 0000 0072 2100 0000 7226 0000 0072  r....r!...r&...r
-00001100: 2800 0000 da08 7072 6f70 6572 7479 720c  (.....propertyr.
-00001110: 0000 00da 0673 6574 7465 7272 0d00 0000  .....setterr....
-00001120: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00001130: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00001140: 0000 0072 1500 0000 7216 0000 00da 0d5f  ...r....r......_
-00001150: 5f63 6c61 7373 6365 6c6c 5f5f 721d 0000  _classcell__r...
-00001160: 0072 1d00 0000 722c 0000 0072 1e00 0000  .r....r,...r....
-00001170: 720b 0000 000b 0000 0073 9c00 0000 0803  r........s......
-00001180: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00001190: 0001 0001 0004 0001 0001 0001 00ed 0202  ................
-000011a0: 0201 0201 0601 0601 0a01 0601 0601 0601  ................
-000011b0: 0201 0601 0205 0601 0601 02ed 0c23 0803  .............#..
-000011c0: 0805 0c06 0201 1003 0401 1004 0201 1003  ................
-000011d0: 0401 1004 0201 1403 0401 1404 0201 1403  ................
-000011e0: 0401 1404 0201 1803 0401 1804 0201 1403  ................
-000011f0: 0401 1404 0201 1403 0401 1407 0201 1403  ................
-00001200: 0401 1404 0201 1003 0401 1004 0201 1403  ................
-00001210: 0401 1404 0201 1003 0401 720b 0000 004e  ..........r....N
-00001220: 2911 da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
-00001230: 0300 0000 7204 0000 00da 1366 6c65 745f  ....r......flet_
-00001240: 636f 7265 2e61 6c69 676e 6d65 6e74 7205  core.alignmentr.
-00001250: 0000 00da 1666 6c65 745f 636f 7265 2e63  .....flet_core.c
-00001260: 616e 7661 732e 7368 6170 6572 0600 0000  anvas.shaper....
-00001270: da11 666c 6574 5f63 6f72 652e 636f 6e74  ..flet_core.cont
-00001280: 726f 6c72 0700 0000 5a15 666c 6574 5f63  rolr....Z.flet_c
-00001290: 6f72 652e 696e 6c69 6e65 5f73 7061 6e72  ore.inline_spanr
-000012a0: 0800 0000 da14 666c 6574 5f63 6f72 652e  ......flet_core.
-000012b0: 7465 7874 5f73 7479 6c65 7209 0000 00da  text_styler.....
-000012c0: 0f66 6c65 745f 636f 7265 2e74 7970 6573  .flet_core.types
-000012d0: 720a 0000 0072 0b00 0000 721d 0000 0072  r....r....r....r
-000012e0: 1d00 0000 721d 0000 0072 1e00 0000 da08  ....r....r......
-000012f0: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
-00001300: 0014 020c 010c 010c 010c 010c 010c 03    ...............
+00000550: 6c65 742f 666c 6574 636f 6e74 7269 622f  let/fletcontrib/
+00000560: 7364 6b2f 7079 7468 6f6e 2f70 6163 6b61  sdk/python/packa
+00000570: 6765 732f 666c 6574 2d63 6f72 652f 7372  ges/flet-core/sr
+00000580: 632f 666c 6574 5f63 6f72 652f 6361 6e76  c/flet_core/canv
+00000590: 6173 2f74 6578 742e 7079 721b 0000 000c  as/text.pyr.....
+000005a0: 0000 0073 1800 0000 0015 1402 0601 0601  ...s............
+000005b0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000005c0: 7a0d 5465 7874 2e5f 5f69 6e69 745f 5f63  z.Text.__init__c
+000005d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000005e0: 0100 0000 4300 0000 7304 0000 0064 0153  ....C...s....d.S
+000005f0: 00a9 024e 720e 0000 0072 1d00 0000 a901  ...Nr....r......
+00000600: 721c 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
+00000610: 1e00 0000 da11 5f67 6574 5f63 6f6e 7472  ......_get_contr
+00000620: 6f6c 5f6e 616d 652f 0000 0073 0200 0000  ol_name/...s....
+00000630: 0001 7a16 5465 7874 2e5f 6765 745f 636f  ..z.Text._get_co
+00000640: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
+00000650: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000660: 0000 0073 1400 0000 6700 7d01 7c01 a000  ...s....g.}.|...
+00000670: 7c00 6a01 a101 0100 7c01 5300 a901 4e29  |.j.....|.S...N)
+00000680: 02da 0665 7874 656e 64da 0c5f 5465 7874  ...extend.._Text
+00000690: 5f5f 7370 616e 7329 0272 1c00 0000 da08  __spans).r......
+000006a0: 6368 696c 6472 656e 721d 0000 0072 1d00  childrenr....r..
+000006b0: 0000 721e 0000 00da 0d5f 6765 745f 6368  ..r......_get_ch
+000006c0: 696c 6472 656e 3200 0000 7306 0000 0000  ildren2...s.....
+000006d0: 0104 010c 017a 1254 6578 742e 5f67 6574  .....z.Text._get
+000006e0: 5f63 6869 6c64 7265 6e63 0100 0000 0000  _childrenc......
+000006f0: 0000 0000 0000 0100 0000 0400 0000 0300  ................
+00000700: 0000 732a 0000 0074 0083 00a0 01a1 0001  ..s*...t........
+00000710: 007c 00a0 0264 017c 006a 03a1 0201 007c  .|...d.|.j.....|
+00000720: 00a0 0264 027c 006a 04a1 0201 0064 0053  ...d.|.j.....d.S
+00000730: 0029 034e 720f 0000 0072 1100 0000 2905  .).Nr....r....).
+00000740: da05 7375 7065 72da 0d62 6566 6f72 655f  ..super..before_
+00000750: 7570 6461 7465 da0e 5f73 6574 5f61 7474  update.._set_att
+00000760: 725f 6a73 6f6e da0c 5f54 6578 745f 5f73  r_json.._Text__s
+00000770: 7479 6c65 da10 5f54 6578 745f 5f61 6c69  tyle.._Text__ali
+00000780: 676e 6d65 6e74 7220 0000 00a9 01da 095f  gnmentr ......._
+00000790: 5f63 6c61 7373 5f5f 721d 0000 0072 1e00  _class__r....r..
+000007a0: 0000 7228 0000 0037 0000 0073 0600 0000  ..r(...7...s....
+000007b0: 0001 0a01 0e01 7a12 5465 7874 2e62 6566  ......z.Text.bef
+000007c0: 6f72 655f 7570 6461 7465 2901 da06 7265  ore_update)...re
+000007d0: 7475 726e 6301 0000 0000 0000 0000 0000  turnc...........
+000007e0: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
+000007f0: 0000 7c00 a000 6401 a101 5300 a902 4e72  ..|...d...S...Nr
+00000800: 0c00 0000 a901 da09 5f67 6574 5f61 7474  ........_get_att
+00000810: 7272 2000 0000 721d 0000 0072 1d00 0000  rr ...r....r....
+00000820: 721e 0000 0072 0c00 0000 3d00 0000 7302  r....r....=...s.
+00000830: 0000 0000 027a 0654 6578 742e 7829 01da  .....z.Text.x)..
+00000840: 0576 616c 7565 6302 0000 0000 0000 0000  .valuec.........
+00000850: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000860: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
+00000870: 6400 5300 722f 0000 00a9 01da 095f 7365  d.S.r/......._se
+00000880: 745f 6174 7472 a902 721c 0000 0072 3200  t_attr..r....r2.
+00000890: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000008a0: 0072 0c00 0000 4100 0000 7302 0000 0000  .r....A...s.....
+000008b0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+000008c0: 0000 0300 0000 4300 0000 730a 0000 007c  ......C...s....|
+000008d0: 00a0 0064 01a1 0153 00a9 024e 720d 0000  ...d...S...Nr...
+000008e0: 0072 3000 0000 7220 0000 0072 1d00 0000  .r0...r ...r....
+000008f0: 721d 0000 0072 1e00 0000 720d 0000 0046  r....r....r....F
+00000900: 0000 0073 0200 0000 0002 7a06 5465 7874  ...s......z.Text
+00000910: 2e79 6302 0000 0000 0000 0000 0000 0002  .yc.............
+00000920: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
+00000930: 7c00 a000 6401 7c01 a102 0100 6400 5300  |...d.|.....d.S.
+00000940: 7236 0000 0072 3300 0000 7235 0000 0072  r6...r3...r5...r
+00000950: 1d00 0000 721d 0000 0072 1e00 0000 720d  ....r....r....r.
+00000960: 0000 004a 0000 0073 0200 0000 0002 6301  ...J...s......c.
+00000970: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000980: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
+00000990: 6401 a101 5300 721f 0000 0072 3000 0000  d...S.r....r0...
+000009a0: 7220 0000 0072 1d00 0000 721d 0000 0072  r ...r....r....r
+000009b0: 1e00 0000 720e 0000 004f 0000 0073 0200  ....r....O...s..
+000009c0: 0000 0002 7a09 5465 7874 2e74 6578 7463  ....z.Text.textc
+000009d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000009e0: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+000009f0: 0064 017c 01a1 0201 0064 0053 0072 1f00  .d.|.....d.S.r..
+00000a00: 0000 7233 0000 0072 3500 0000 721d 0000  ..r3...r5...r...
+00000a10: 0072 1d00 0000 721e 0000 0072 0e00 0000  .r....r....r....
+00000a20: 5300 0000 7302 0000 0000 0263 0100 0000  S...s......c....
+00000a30: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000a40: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
+00000a50: 2200 0000 a901 722a 0000 0072 2000 0000  ".....r*...r ...
+00000a60: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00000a70: 0f00 0000 5800 0000 7302 0000 0000 027a  ....X...s......z
+00000a80: 0a54 6578 742e 7374 796c 6563 0200 0000  .Text.stylec....
+00000a90: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000aa0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+00000ab0: 0053 0072 2200 0000 7237 0000 0072 3500  .S.r"...r7...r5.
+00000ac0: 0000 721d 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000ad0: 0072 0f00 0000 5c00 0000 7302 0000 0000  .r....\...s.....
+00000ae0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000af0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00000b00: 006a 0053 0072 2200 0000 a901 7224 0000  .j.S.r".....r$..
+00000b10: 0072 2000 0000 721d 0000 0072 1d00 0000  .r ...r....r....
+00000b20: 721e 0000 0072 1000 0000 6100 0000 7302  r....r....a...s.
+00000b30: 0000 0000 027a 0a54 6578 742e 7370 616e  .....z.Text.span
+00000b40: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+00000b50: 0000 0200 0000 4300 0000 7316 0000 007c  ......C...s....|
+00000b60: 0164 0075 0172 0c7c 016e 0267 007c 005f  .d.u.r.|.n.g.|._
+00000b70: 0064 0053 0072 2200 0000 7238 0000 0072  .d.S.r"...r8...r
+00000b80: 3500 0000 721d 0000 0072 1d00 0000 721e  5...r....r....r.
+00000b90: 0000 0072 1000 0000 6500 0000 7302 0000  ...r....e...s...
+00000ba0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00000bb0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00000bc0: 007c 006a 0053 0072 2200 0000 a901 722b  .|.j.S.r".....r+
+00000bd0: 0000 0072 2000 0000 721d 0000 0072 1d00  ...r ...r....r..
+00000be0: 0000 721e 0000 0072 1100 0000 6a00 0000  ..r....r....j...
+00000bf0: 7302 0000 0000 027a 0e54 6578 742e 616c  s......z.Text.al
+00000c00: 6967 6e6d 656e 7463 0200 0000 0000 0000  ignmentc........
+00000c10: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000c20: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
+00000c30: 2200 0000 7239 0000 0072 3500 0000 721d  "...r9...r5...r.
+00000c40: 0000 0072 1d00 0000 721e 0000 0072 1100  ...r....r....r..
+00000c50: 0000 6e00 0000 7302 0000 0000 0263 0100  ..n...s......c..
+00000c60: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000c70: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00000c80: 0072 2200 0000 2901 da11 5f54 6578 745f  .r"...)..._Text_
+00000c90: 5f74 6578 745f 616c 6967 6e72 2000 0000  _text_alignr ...
+00000ca0: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00000cb0: 1200 0000 7300 0000 7302 0000 0000 027a  ....s...s......z
+00000cc0: 0f54 6578 742e 7465 7874 5f61 6c69 676e  .Text.text_align
+00000cd0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000ce0: 0006 0000 0043 0000 0073 2600 0000 7c01  .....C...s&...|.
+00000cf0: 7c00 5f00 7c00 a001 6401 7402 7c01 7403  |._.|...d.t.|.t.
+00000d00: 8302 721c 7c01 6a04 6e02 7c01 a102 0100  ..r.|.j.n.|.....
+00000d10: 6400 5300 2902 4e5a 0974 6578 7441 6c69  d.S.).NZ.textAli
+00000d20: 676e 2905 723a 0000 0072 3400 0000 da0a  gn).r:...r4.....
+00000d30: 6973 696e 7374 616e 6365 720a 0000 0072  isinstancer....r
+00000d40: 3200 0000 7235 0000 0072 1d00 0000 721d  2...r5...r....r.
+00000d50: 0000 0072 1e00 0000 7212 0000 0077 0000  ...r....r....w..
+00000d60: 0073 0800 0000 0002 0601 0401 14ff 6301  .s............c.
+00000d70: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000d80: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
+00000d90: 6401 a101 5300 a902 4e5a 086d 6178 4c69  d...S...NZ.maxLi
+00000da0: 6e65 7372 3000 0000 7220 0000 0072 1d00  nesr0...r ...r..
+00000db0: 0000 721d 0000 0072 1e00 0000 7213 0000  ..r....r....r...
+00000dc0: 007f 0000 0073 0200 0000 0002 7a0e 5465  .....s......z.Te
+00000dd0: 7874 2e6d 6178 5f6c 696e 6573 6302 0000  xt.max_linesc...
+00000de0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000df0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
+00000e00: 7c01 a102 0100 6400 5300 723c 0000 0072  |.....d.S.r<...r
+00000e10: 3300 0000 7235 0000 0072 1d00 0000 721d  3...r5...r....r.
+00000e20: 0000 0072 1e00 0000 7213 0000 0083 0000  ...r....r.......
+00000e30: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
+00000e40: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000e50: 0073 0a00 0000 7c00 a000 6401 a101 5300  .s....|...d...S.
+00000e60: a902 4e5a 086d 6178 5769 6474 6872 3000  ..NZ.maxWidthr0.
+00000e70: 0000 7220 0000 0072 1d00 0000 721d 0000  ..r ...r....r...
+00000e80: 0072 1e00 0000 7214 0000 0088 0000 0073  .r....r........s
+00000e90: 0200 0000 0002 7a0e 5465 7874 2e6d 6178  ......z.Text.max
+00000ea0: 5f77 6964 7468 6302 0000 0000 0000 0000  _widthc.........
+00000eb0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000ec0: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
+00000ed0: 6400 5300 723d 0000 0072 3300 0000 7235  d.S.r=...r3...r5
+00000ee0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000ef0: 0000 7214 0000 008c 0000 0073 0200 0000  ..r........s....
+00000f00: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000f10: 0000 0003 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000f20: 7c00 a000 6401 a101 5300 a902 4e72 1500  |...d...S...Nr..
+00000f30: 0000 7230 0000 0072 2000 0000 721d 0000  ..r0...r ...r...
+00000f40: 0072 1d00 0000 721e 0000 0072 1500 0000  .r....r....r....
+00000f50: 9100 0000 7302 0000 0000 027a 0d54 6578  ....s......z.Tex
+00000f60: 742e 656c 6c69 7073 6973 6302 0000 0000  t.ellipsisc.....
+00000f70: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000f80: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
+00000f90: a102 0100 6400 5300 723e 0000 0072 3300  ....d.S.r>...r3.
+00000fa0: 0000 7235 0000 0072 1d00 0000 721d 0000  ..r5...r....r...
+00000fb0: 0072 1e00 0000 7215 0000 0095 0000 0073  .r....r........s
+00000fc0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
+00000fd0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000fe0: 0a00 0000 7c00 a000 6401 a101 5300 a902  ....|...d...S...
+00000ff0: 4e72 1600 0000 7230 0000 0072 2000 0000  Nr....r0...r ...
+00001000: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00001010: 1600 0000 9a00 0000 7302 0000 0000 027a  ........s......z
+00001020: 0b54 6578 742e 726f 7461 7465 6302 0000  .Text.rotatec...
+00001030: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00001040: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
+00001050: 7c01 a102 0100 6400 5300 723f 0000 0072  |.....d.S.r?...r
+00001060: 3300 0000 7235 0000 0072 1d00 0000 721d  3...r5...r....r.
+00001070: 0000 0072 1e00 0000 7216 0000 009e 0000  ...r....r.......
+00001080: 0073 0200 0000 0002 290f 4e4e 4e4e 4e4e  .s......).NNNNNN
+00001090: 4e4e 4e4e 4e4e 4e4e 4e29 20da 085f 5f6e  NNNNNNNNN) ..__n
+000010a0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+000010b0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+000010c0: 0700 0000 7204 0000 00da 0373 7472 7209  ....r......strr.
+000010d0: 0000 0072 0300 0000 7208 0000 0072 0500  ...r....r....r..
+000010e0: 0000 720a 0000 00da 0369 6e74 da04 626f  ..r......int..bo
+000010f0: 6f6c 7202 0000 0072 1b00 0000 7221 0000  olr....r....r!..
+00001100: 0072 2600 0000 7228 0000 00da 0870 726f  .r&...r(.....pro
+00001110: 7065 7274 7972 0c00 0000 da06 7365 7474  pertyr......sett
+00001120: 6572 720d 0000 0072 0e00 0000 720f 0000  err....r....r...
+00001130: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+00001140: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00001150: 1600 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00001160: 6c5f 5f72 1d00 0000 721d 0000 0072 2c00  l__r....r....r,.
+00001170: 0000 721e 0000 0072 0b00 0000 0b00 0000  ..r....r........
+00001180: 739c 0000 0008 0300 0100 0100 0100 0100  s...............
+00001190: 0100 0100 0100 0100 0100 0100 0400 0100  ................
+000011a0: 0100 0100 ed02 0202 0102 0106 0106 010a  ................
+000011b0: 0106 0106 0106 0102 0106 0102 0506 0106  ................
+000011c0: 0102 ed0c 2308 0308 050c 0602 0110 0304  ....#...........
+000011d0: 0110 0402 0110 0304 0110 0402 0114 0304  ................
+000011e0: 0114 0402 0114 0304 0114 0402 0118 0304  ................
+000011f0: 0118 0402 0114 0304 0114 0402 0114 0304  ................
+00001200: 0114 0702 0114 0304 0114 0402 0110 0304  ................
+00001210: 0110 0402 0114 0304 0114 0402 0110 0304  ................
+00001220: 0172 0b00 0000 4e29 11da 0674 7970 696e  .r....N)...typin
+00001230: 6772 0200 0000 7203 0000 0072 0400 0000  gr....r....r....
+00001240: da13 666c 6574 5f63 6f72 652e 616c 6967  ..flet_core.alig
+00001250: 6e6d 656e 7472 0500 0000 da16 666c 6574  nmentr......flet
+00001260: 5f63 6f72 652e 6361 6e76 6173 2e73 6861  _core.canvas.sha
+00001270: 7065 7206 0000 00da 1166 6c65 745f 636f  per......flet_co
+00001280: 7265 2e63 6f6e 7472 6f6c 7207 0000 005a  re.controlr....Z
+00001290: 1566 6c65 745f 636f 7265 2e69 6e6c 696e  .flet_core.inlin
+000012a0: 655f 7370 616e 7208 0000 00da 1466 6c65  e_spanr......fle
+000012b0: 745f 636f 7265 2e74 6578 745f 7374 796c  t_core.text_styl
+000012c0: 6572 0900 0000 da0f 666c 6574 5f63 6f72  er......flet_cor
+000012d0: 652e 7479 7065 7372 0a00 0000 720b 0000  e.typesr....r...
+000012e0: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
+000012f0: 721e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001300: 0000 0073 0e00 0000 1402 0c01 0c01 0c01  ...s............
+00001310: 0c01 0c01 0c03                           ......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/arc.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/canvas.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/circle.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/color.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/fill.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/line.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/oval.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/path.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/points.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/rect.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/shadow.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/canvas/text.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/card.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 9932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 cc26 0000  a........:)f.&..
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 cc26 0000  a........./f.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
@@ -144,431 +144,432 @@
 000008f0: 0000 0072 3c00 0000 723d 0000 0063 0100  ...r<...r=...c..
 00000900: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 00000910: 0000 5300 0000 731a 0000 0074 00a0 017c  ..S...s....t...|
 00000920: 006a 02a1 017d 0174 0366 0069 007c 01a4  .j...}.t.f.i.|..
 00000930: 018e 0153 00a9 014e 2904 da04 6a73 6f6e  ...S...N)...json
 00000940: da05 6c6f 6164 7372 3d00 0000 da0d 4261  ..loadsr=.....Ba
 00000950: 7243 6861 7274 4576 656e 7429 02da 0165  rChartEvent)...e
-00000960: da01 64a9 0072 4500 0000 fa5c 2f77 6f72  ..d..rE....\/wor
+00000960: da01 64a9 0072 4500 0000 fa63 2f77 6f72  ..d..rE....c/wor
 00000970: 6b73 7061 6365 732f 636f 6e74 7269 6266  kspaces/contribf
-00000980: 6c65 742f 666c 6574 2f73 646b 2f70 7974  let/flet/sdk/pyt
-00000990: 686f 6e2f 7061 636b 6167 6573 2f66 6c65  hon/packages/fle
-000009a0: 742d 636f 7265 2f73 7263 2f66 6c65 745f  t-core/src/flet_
-000009b0: 636f 7265 2f63 6861 7274 732f 6261 725f  core/charts/bar_
-000009c0: 6368 6172 742e 7079 da1c 636f 6e76 6572  chart.py..conver
-000009d0: 745f 6c69 6e65 6368 6172 745f 6576 656e  t_linechart_even
-000009e0: 745f 6461 7461 6600 0000 7304 0000 0000  t_dataf...s.....
-000009f0: 010c 017a 3742 6172 4368 6172 742e 5f5f  ...z7BarChart.__
-00000a00: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-00000a10: 636f 6e76 6572 745f 6c69 6e65 6368 6172  convert_linechar
-00000a20: 745f 6576 656e 745f 6461 7461 5a0b 6368  t_event_dataZ.ch
-00000a30: 6172 745f 6576 656e 7429 1772 0a00 0000  art_event).r....
-00000a40: da08 5f5f 696e 6974 5f5f 720d 0000 00da  ..__init__r.....
-00000a50: 195f 4261 7243 6861 7274 5f5f 6f6e 5f63  ._BarChart__on_c
-00000a60: 6861 7274 5f65 7665 6e74 da12 5f61 6464  hart_event.._add
-00000a70: 5f65 7665 6e74 5f68 616e 646c 6572 da0b  _event_handler..
-00000a80: 6765 745f 6861 6e64 6c65 7272 1500 0000  get_handlerr....
-00000a90: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000aa0: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
-00000ab0: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
-00000ac0: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-00000ad0: 0072 2300 0000 7224 0000 00da 0e6f 6e5f  .r#...r$.....on_
-00000ae0: 6368 6172 745f 6576 656e 7429 2dda 0473  chart_event)-..s
-00000af0: 656c 6672 1500 0000 7216 0000 0072 1700  elfr....r....r..
-00000b00: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000b10: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000b20: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-00000b30: 2100 0000 7222 0000 0072 2300 0000 7224  !...r"...r#...r$
-00000b40: 0000 0072 4c00 0000 7225 0000 0072 2600  ...rL...r%...r&.
-00000b50: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-00000b60: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000b70: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-00000b80: 3000 0000 7231 0000 0072 3200 0000 7233  0...r1...r2...r3
-00000b90: 0000 0072 3400 0000 7235 0000 0072 3600  ...r4...r5...r6.
-00000ba0: 0000 7237 0000 0072 3800 0000 7239 0000  ..r7...r8...r9..
-00000bb0: 0072 3e00 0000 723a 0000 0072 3b00 0000  .r>...r:...r;...
-00000bc0: 723c 0000 0072 3d00 0000 7247 0000 0072  r<...r=...rG...r
-00000bd0: 4500 0000 7245 0000 0072 4600 0000 7248  E...rE...rF...rH
-00000be0: 0000 0017 0000 0073 6200 0000 0031 0401  .......sb....1..
-00000bf0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000c00: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000c10: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000c20: 0201 0201 02e5 061e 0804 0a01 1202 0601  ................
-00000c30: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00000c40: 0601 0601 0601 0601 0601 0601 0601 7a11  ..............z.
-00000c50: 4261 7243 6861 7274 2e5f 5f69 6e69 745f  BarChart.__init_
-00000c60: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00000c70: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
-00000c80: 0153 0029 024e 5a08 6261 7263 6861 7274  .S.).NZ.barchart
-00000c90: 7245 0000 00a9 0172 4d00 0000 7245 0000  rE.....rM...rE..
-00000ca0: 0072 4500 0000 7246 0000 00da 115f 6765  .rE...rF....._ge
-00000cb0: 745f 636f 6e74 726f 6c5f 6e61 6d65 7f00  t_control_name..
-00000cc0: 0000 7302 0000 0000 017a 1a42 6172 4368  ..s......z.BarCh
-00000cd0: 6172 742e 5f67 6574 5f63 6f6e 7472 6f6c  art._get_control
-00000ce0: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
-00000cf0: 0000 0100 0000 0400 0000 0300 0000 7346  ..............sF
-00000d00: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
-00000d10: 0264 017c 006a 03a1 0201 007c 00a0 0264  .d.|.j.....|...d
-00000d20: 027c 006a 04a1 0201 007c 00a0 0264 037c  .|.j.....|...d.|
-00000d30: 006a 05a1 0201 007c 00a0 0264 047c 006a  .j.....|...d.|.j
-00000d40: 06a1 0201 0064 0053 0029 054e 5a13 686f  .....d.S.).NZ.ho
-00000d50: 7269 7a6f 6e74 616c 4772 6964 4c69 6e65  rizontalGridLine
-00000d60: 735a 1176 6572 7469 6361 6c47 7269 644c  sZ.verticalGridL
-00000d70: 696e 6573 7217 0000 0072 1b00 0000 2907  inesr....r....).
-00000d80: da05 7375 7065 72da 0d62 6566 6f72 655f  ..super..before_
-00000d90: 7570 6461 7465 da0e 5f73 6574 5f61 7474  update.._set_att
-00000da0: 725f 6a73 6f6e da20 5f42 6172 4368 6172  r_json. _BarChar
-00000db0: 745f 5f68 6f72 697a 6f6e 7461 6c5f 6772  t__horizontal_gr
-00000dc0: 6964 5f6c 696e 6573 da1e 5f42 6172 4368  id_lines.._BarCh
-00000dd0: 6172 745f 5f76 6572 7469 6361 6c5f 6772  art__vertical_gr
-00000de0: 6964 5f6c 696e 6573 da12 5f42 6172 4368  id_lines.._BarCh
-00000df0: 6172 745f 5f61 6e69 6d61 7465 da11 5f42  art__animate.._B
-00000e00: 6172 4368 6172 745f 5f62 6f72 6465 7272  arChart__borderr
-00000e10: 4e00 0000 a901 da09 5f5f 636c 6173 735f  N.......__class_
-00000e20: 5f72 4500 0000 7246 0000 0072 5100 0000  _rE...rF...rQ...
-00000e30: 8200 0000 730a 0000 0000 010a 010e 010e  ....s...........
-00000e40: 010e 017a 1642 6172 4368 6172 742e 6265  ...z.BarChart.be
-00000e50: 666f 7265 5f75 7064 6174 6563 0100 0000  fore_updatec....
-00000e60: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000e70: 4300 0000 739e 0000 0067 007d 017c 006a  C...s....g.}.|.j
-00000e80: 0044 005d 0e7d 027c 01a0 017c 02a1 0101  .D.].}.|...|....
-00000e90: 0071 0a7c 006a 0272 3a7c 006a 02a0 0364  .q.|.j.r:|.j...d
-00000ea0: 0164 02a1 0201 007c 01a0 017c 006a 02a1  .d.....|...|.j..
-00000eb0: 0101 007c 006a 0472 5a7c 006a 04a0 0364  ...|.j.rZ|.j...d
-00000ec0: 0164 03a1 0201 007c 01a0 017c 006a 04a1  .d.....|...|.j..
-00000ed0: 0101 007c 006a 0572 7a7c 006a 05a0 0364  ...|.j.rz|.j...d
-00000ee0: 0164 04a1 0201 007c 01a0 017c 006a 05a1  .d.....|...|.j..
-00000ef0: 0101 007c 006a 0672 9a7c 006a 06a0 0364  ...|.j.r.|.j...d
-00000f00: 0164 05a1 0201 007c 01a0 017c 006a 06a1  .d.....|...|.j..
-00000f10: 0101 007c 0153 0029 064e da01 6eda 016c  ...|.S.).N..n..l
-00000f20: da01 74da 0172 da01 6229 07da 155f 4261  ..t..r..b)..._Ba
-00000f30: 7243 6861 7274 5f5f 6261 725f 6772 6f75  rChart__bar_grou
-00000f40: 7073 da06 6170 7065 6e64 da14 5f42 6172  ps..append.._Bar
-00000f50: 4368 6172 745f 5f6c 6566 745f 6178 6973  Chart__left_axis
-00000f60: da12 5f73 6574 5f61 7474 725f 696e 7465  .._set_attr_inte
-00000f70: 726e 616c da13 5f42 6172 4368 6172 745f  rnal.._BarChart_
-00000f80: 5f74 6f70 5f61 7869 73da 155f 4261 7243  _top_axis.._BarC
-00000f90: 6861 7274 5f5f 7269 6768 745f 6178 6973  hart__right_axis
-00000fa0: da16 5f42 6172 4368 6172 745f 5f62 6f74  .._BarChart__bot
-00000fb0: 746f 6d5f 6178 6973 2903 724d 0000 00da  tom_axis).rM....
-00000fc0: 0863 6869 6c64 7265 6e5a 0264 7372 4500  .childrenZ.dsrE.
-00000fd0: 0000 7245 0000 0072 4600 0000 da0d 5f67  ..rE...rF....._g
-00000fe0: 6574 5f63 6869 6c64 7265 6e89 0000 0073  et_children....s
-00000ff0: 2000 0000 0001 0401 0a01 0c01 0601 0e01   ...............
-00001000: 0c01 0601 0e01 0c01 0601 0e01 0c01 0601  ................
-00001010: 0e01 0c01 7a16 4261 7243 6861 7274 2e5f  ....z.BarChart._
-00001020: 6765 745f 6368 696c 6472 656e 6301 0000  get_childrenc...
-00001030: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00001040: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00001050: 723f 0000 00a9 0172 5e00 0000 724e 0000  r?.....r^...rN..
-00001060: 0072 4500 0000 7245 0000 0072 4600 0000  .rE...rE...rF...
-00001070: 7215 0000 009c 0000 0073 0200 0000 0002  r........s......
-00001080: 7a13 4261 7243 6861 7274 2e62 6172 5f67  z.BarChart.bar_g
-00001090: 726f 7570 7363 0200 0000 0000 0000 0000  roupsc..........
-000010a0: 0000 0200 0000 0200 0000 4300 0000 7316  ..........C...s.
-000010b0: 0000 007c 0164 0075 0172 0c7c 016e 0267  ...|.d.u.r.|.n.g
-000010c0: 007c 005f 0064 0053 0072 3f00 0000 7267  .|._.d.S.r?...rg
-000010d0: 0000 00a9 0272 4d00 0000 da05 7661 6c75  .....rM.....valu
-000010e0: 6572 4500 0000 7245 0000 0072 4600 0000  erE...rE...rF...
-000010f0: 7215 0000 00a0 0000 0073 0200 0000 0002  r........s......
-00001100: a901 da06 7265 7475 726e 6301 0000 0000  ....returnc.....
-00001110: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00001120: 0000 0073 0e00 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
-00001130: 6403 8d02 5300 2904 4eda 0b67 726f 7570  d...S.).N..group
-00001140: 7353 7061 6365 da05 666c 6f61 74a9 01da  sSpace..float...
-00001150: 0964 6174 615f 7479 7065 a901 da09 5f67  .data_type...._g
-00001160: 6574 5f61 7474 7272 4e00 0000 7245 0000  et_attrrN...rE..
-00001170: 0072 4500 0000 7246 0000 0072 1600 0000  .rE...rF...r....
-00001180: a500 0000 7302 0000 0000 027a 1542 6172  ....s......z.Bar
-00001190: 4368 6172 742e 6772 6f75 7073 5f73 7061  Chart.groups_spa
-000011a0: 6365 2901 7269 0000 0063 0200 0000 0000  ce).ri...c......
-000011b0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-000011c0: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-000011d0: 0201 0064 0053 0029 024e 726c 0000 00a9  ...d.S.).Nrl....
-000011e0: 01da 095f 7365 745f 6174 7472 7268 0000  ..._set_attrrh..
-000011f0: 0072 4500 0000 7245 0000 0072 4600 0000  .rE...rE...rF...
-00001200: 7216 0000 00a9 0000 0073 0200 0000 0002  r........s......
-00001210: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001220: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00001230: 6a00 5300 723f 0000 00a9 0172 5500 0000  j.S.r?.....rU...
-00001240: 724e 0000 0072 4500 0000 7245 0000 0072  rN...rE...rE...r
-00001250: 4600 0000 7217 0000 00ae 0000 0073 0200  F...r........s..
-00001260: 0000 0002 7a10 4261 7243 6861 7274 2e61  ....z.BarChart.a
-00001270: 6e69 6d61 7465 6302 0000 0000 0000 0000  nimatec.........
-00001280: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00001290: 0a00 0000 7c01 7c00 5f00 6400 5300 723f  ....|.|._.d.S.r?
-000012a0: 0000 0072 7400 0000 7268 0000 0072 4500  ...rt...rh...rE.
-000012b0: 0000 7245 0000 0072 4600 0000 7217 0000  ..rE...rF...r...
-000012c0: 00b2 0000 0073 0200 0000 0002 6301 0000  .....s......c...
-000012d0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-000012e0: 0043 0000 0073 0a00 0000 7c00 a000 6401  .C...s....|...d.
-000012f0: a101 5300 a902 4e72 1900 0000 7270 0000  ..S...Nr....rp..
-00001300: 0072 4e00 0000 7245 0000 0072 4500 0000  .rN...rE...rE...
-00001310: 7246 0000 0072 1900 0000 b700 0000 7302  rF...r........s.
-00001320: 0000 0000 027a 1042 6172 4368 6172 742e  .....z.BarChart.
-00001330: 6267 636f 6c6f 7263 0200 0000 0000 0000  bgcolorc........
-00001340: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001350: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00001360: 0064 0053 0072 7500 0000 7272 0000 0072  .d.S.ru...rr...r
-00001370: 6800 0000 7245 0000 0072 4500 0000 7246  h...rE...rE...rF
-00001380: 0000 0072 1900 0000 bb00 0000 7302 0000  ...r........s...
-00001390: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-000013a0: 0100 0000 0500 0000 4300 0000 7310 0000  ........C...s...
-000013b0: 007c 006a 0064 0164 0264 0364 048d 0353  .|.j.d.d.d.d...S
-000013c0: 0029 054e 7218 0000 00da 0462 6f6f 6c54  .).Nr......boolT
-000013d0: 2902 726f 0000 00da 0964 6566 5f76 616c  ).ro.....def_val
-000013e0: 7565 7270 0000 0072 4e00 0000 7245 0000  uerp...rN...rE..
-000013f0: 0072 4500 0000 7246 0000 0072 1800 0000  .rE...rF...r....
-00001400: c000 0000 7302 0000 0000 027a 1442 6172  ....s......z.Bar
-00001410: 4368 6172 742e 696e 7465 7261 6374 6976  Chart.interactiv
-00001420: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00001430: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
-00001440: 00a0 0064 017c 01a1 0201 0064 0053 0029  ...d.|.....d.S.)
-00001450: 024e 7218 0000 0072 7200 0000 7268 0000  .Nr....rr...rh..
-00001460: 0072 4500 0000 7245 0000 0072 4600 0000  .rE...rE...rF...
-00001470: 7218 0000 00c4 0000 0073 0200 0000 0002  r........s......
-00001480: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001490: 0003 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
-000014a0: a000 6401 a101 5300 a902 4e5a 0e74 6f6f  ..d...S...NZ.too
-000014b0: 6c74 6970 4267 636f 6c6f 7272 7000 0000  ltipBgcolorrp...
-000014c0: 724e 0000 0072 4500 0000 7245 0000 0072  rN...rE...rE...r
-000014d0: 4600 0000 721a 0000 00c9 0000 0073 0200  F...r........s..
-000014e0: 0000 0002 7a18 4261 7243 6861 7274 2e74  ....z.BarChart.t
-000014f0: 6f6f 6c74 6970 5f62 6763 6f6c 6f72 6302  ooltip_bgcolorc.
-00001500: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001510: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-00001520: 6401 7c01 a102 0100 6400 5300 7278 0000  d.|.....d.S.rx..
-00001530: 0072 7200 0000 7268 0000 0072 4500 0000  .rr...rh...rE...
-00001540: 7245 0000 0072 4600 0000 721a 0000 00cd  rE...rF...r.....
-00001550: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-00001560: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001570: 0000 0073 0600 0000 7c00 6a00 5300 723f  ...s....|.j.S.r?
-00001580: 0000 00a9 0172 5600 0000 724e 0000 0072  .....rV...rN...r
-00001590: 4500 0000 7245 0000 0072 4600 0000 721b  E...rE...rF...r.
-000015a0: 0000 00d2 0000 0073 0200 0000 0002 7a0f  .......s......z.
-000015b0: 4261 7243 6861 7274 2e62 6f72 6465 7263  BarChart.borderc
-000015c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000015d0: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
-000015e0: 005f 0064 0053 0072 3f00 0000 7279 0000  ._.d.S.r?...ry..
-000015f0: 0072 6800 0000 7245 0000 0072 4500 0000  .rh...rE...rE...
-00001600: 7246 0000 0072 1b00 0000 d600 0000 7302  rF...r........s.
-00001610: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00001620: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00001630: 0000 007c 006a 0053 0072 3f00 0000 a901  ...|.j.S.r?.....
-00001640: 7253 0000 0072 4e00 0000 7245 0000 0072  rS...rN...rE...r
-00001650: 4500 0000 7246 0000 0072 1c00 0000 db00  E...rF...r......
-00001660: 0000 7302 0000 0000 027a 1e42 6172 4368  ..s......z.BarCh
-00001670: 6172 742e 686f 7269 7a6f 6e74 616c 5f67  art.horizontal_g
-00001680: 7269 645f 6c69 6e65 7363 0200 0000 0000  rid_linesc......
-00001690: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-000016a0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
-000016b0: 0072 3f00 0000 727a 0000 0072 6800 0000  .r?...rz...rh...
-000016c0: 7245 0000 0072 4500 0000 7246 0000 0072  rE...rE...rF...r
-000016d0: 1c00 0000 df00 0000 7302 0000 0000 0263  ........s......c
-000016e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000016f0: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
-00001700: 0053 0072 3f00 0000 a901 7254 0000 0072  .S.r?.....rT...r
-00001710: 4e00 0000 7245 0000 0072 4500 0000 7246  N...rE...rE...rF
-00001720: 0000 0072 1d00 0000 e400 0000 7302 0000  ...r........s...
-00001730: 0000 027a 1c42 6172 4368 6172 742e 7665  ...z.BarChart.ve
-00001740: 7274 6963 616c 5f67 7269 645f 6c69 6e65  rtical_grid_line
-00001750: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00001760: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00001770: 017c 005f 0064 0053 0072 3f00 0000 727b  .|._.d.S.r?...r{
-00001780: 0000 0072 6800 0000 7245 0000 0072 4500  ...rh...rE...rE.
-00001790: 0000 7246 0000 0072 1d00 0000 e800 0000  ..rF...r........
-000017a0: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-000017b0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000017c0: 7306 0000 007c 006a 0053 0072 3f00 0000  s....|.j.S.r?...
-000017d0: a901 7260 0000 0072 4e00 0000 7245 0000  ..r`...rN...rE..
-000017e0: 0072 4500 0000 7246 0000 0072 1e00 0000  .rE...rF...r....
-000017f0: ed00 0000 7302 0000 0000 027a 1242 6172  ....s......z.Bar
-00001800: 4368 6172 742e 6c65 6674 5f61 7869 7363  Chart.left_axisc
-00001810: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001820: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
-00001830: 005f 0064 0053 0072 3f00 0000 727c 0000  ._.d.S.r?...r|..
-00001840: 0072 6800 0000 7245 0000 0072 4500 0000  .rh...rE...rE...
-00001850: 7246 0000 0072 1e00 0000 f100 0000 7302  rF...r........s.
-00001860: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00001870: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00001880: 0000 007c 006a 0053 0072 3f00 0000 a901  ...|.j.S.r?.....
-00001890: 7262 0000 0072 4e00 0000 7245 0000 0072  rb...rN...rE...r
-000018a0: 4500 0000 7246 0000 0072 1f00 0000 f600  E...rF...r......
-000018b0: 0000 7302 0000 0000 027a 1142 6172 4368  ..s......z.BarCh
-000018c0: 6172 742e 746f 705f 6178 6973 6302 0000  art.top_axisc...
-000018d0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-000018e0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
-000018f0: 6400 5300 723f 0000 0072 7d00 0000 7268  d.S.r?...r}...rh
-00001900: 0000 0072 4500 0000 7245 0000 0072 4600  ...rE...rE...rF.
-00001910: 0000 721f 0000 00fa 0000 0073 0200 0000  ..r........s....
-00001920: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00001930: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
-00001940: 7c00 6a00 5300 723f 0000 00a9 0172 6300  |.j.S.r?.....rc.
-00001950: 0000 724e 0000 0072 4500 0000 7245 0000  ..rN...rE...rE..
-00001960: 0072 4600 0000 7220 0000 00ff 0000 0073  .rF...r .......s
-00001970: 0200 0000 0002 7a13 4261 7243 6861 7274  ......z.BarChart
-00001980: 2e72 6967 6874 5f61 7869 7363 0200 0000  .right_axisc....
-00001990: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-000019a0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
-000019b0: 0053 0072 3f00 0000 727e 0000 0072 6800  .S.r?...r~...rh.
-000019c0: 0000 7245 0000 0072 4500 0000 7246 0000  ..rE...rE...rF..
-000019d0: 0072 2000 0000 0301 0000 7302 0000 0000  .r .......s.....
-000019e0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-000019f0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-00001a00: 006a 0053 0072 3f00 0000 a901 7264 0000  .j.S.r?.....rd..
-00001a10: 0072 4e00 0000 7245 0000 0072 4500 0000  .rN...rE...rE...
-00001a20: 7246 0000 0072 2100 0000 0801 0000 7302  rF...r!.......s.
-00001a30: 0000 0000 027a 1442 6172 4368 6172 742e  .....z.BarChart.
-00001a40: 626f 7474 6f6d 5f61 7869 7363 0200 0000  bottom_axisc....
-00001a50: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001a60: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
-00001a70: 0053 0072 3f00 0000 727f 0000 0072 6800  .S.r?...r....rh.
-00001a80: 0000 7245 0000 0072 4500 0000 7246 0000  ..rE...rE...rF..
-00001a90: 0072 2100 0000 0c01 0000 7302 0000 0000  .r!.......s.....
-00001aa0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-00001ab0: 0000 0400 0000 4300 0000 730e 0000 007c  ......C...s....|
-00001ac0: 006a 0064 0164 0264 038d 0253 0029 044e  .j.d.d.d...S.).N
-00001ad0: da09 6261 7365 6c69 6e65 7972 6d00 0000  ..baselineyrm...
-00001ae0: 726e 0000 0072 7000 0000 724e 0000 0072  rn...rp...rN...r
-00001af0: 4500 0000 7245 0000 0072 4600 0000 7222  E...rE...rF...r"
-00001b00: 0000 0011 0100 0073 0200 0000 0002 7a13  .......s......z.
-00001b10: 4261 7243 6861 7274 2e62 6173 656c 696e  BarChart.baselin
-00001b20: 655f 7963 0200 0000 0000 0000 0000 0000  e_yc............
-00001b30: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-00001b40: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
-00001b50: 0029 024e 7280 0000 0072 7200 0000 7268  .).Nr....rr...rh
-00001b60: 0000 0072 4500 0000 7245 0000 0072 4600  ...rE...rE...rF.
-00001b70: 0000 7222 0000 0015 0100 0073 0200 0000  ..r".......s....
-00001b80: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00001b90: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
-00001ba0: 7c00 6a00 6401 6402 6403 8d02 5300 2904  |.j.d.d.d...S.).
-00001bb0: 4eda 046d 696e 7972 6d00 0000 726e 0000  N..minyrm...rn..
-00001bc0: 0072 7000 0000 724e 0000 0072 4500 0000  .rp...rN...rE...
-00001bd0: 7245 0000 0072 4600 0000 7223 0000 001a  rE...rF...r#....
-00001be0: 0100 0073 0200 0000 0002 7a0e 4261 7243  ...s......z.BarC
-00001bf0: 6861 7274 2e6d 696e 5f79 6302 0000 0000  hart.min_yc.....
-00001c00: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00001c10: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
-00001c20: a102 0100 6400 5300 2902 4e72 8100 0000  ....d.S.).Nr....
-00001c30: 7272 0000 0072 6800 0000 7245 0000 0072  rr...rh...rE...r
-00001c40: 4500 0000 7246 0000 0072 2300 0000 1e01  E...rF...r#.....
-00001c50: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
-00001c60: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00001c70: 0000 730e 0000 007c 006a 0064 0164 0264  ..s....|.j.d.d.d
-00001c80: 038d 0253 0029 044e da04 6d61 7879 726d  ...S.).N..maxyrm
-00001c90: 0000 0072 6e00 0000 7270 0000 0072 4e00  ...rn...rp...rN.
-00001ca0: 0000 7245 0000 0072 4500 0000 7246 0000  ..rE...rE...rF..
-00001cb0: 0072 2400 0000 2301 0000 7302 0000 0000  .r$...#...s.....
-00001cc0: 027a 0e42 6172 4368 6172 742e 6d61 785f  .z.BarChart.max_
-00001cd0: 7963 0200 0000 0000 0000 0000 0000 0200  yc..............
-00001ce0: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
-00001cf0: 00a0 0064 017c 01a1 0201 0064 0053 0029  ...d.|.....d.S.)
-00001d00: 024e 7282 0000 0072 7200 0000 7268 0000  .Nr....rr...rh..
-00001d10: 0072 4500 0000 7245 0000 0072 4600 0000  .rE...rE...rF...
-00001d20: 7224 0000 0027 0100 0073 0200 0000 0002  r$...'...s......
-00001d30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001d40: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00001d50: 6a00 5300 723f 0000 0029 0172 4900 0000  j.S.r?...).rI...
-00001d60: 724e 0000 0072 4500 0000 7245 0000 0072  rN...rE...rE...r
-00001d70: 4600 0000 724c 0000 002c 0100 0073 0200  F...rL...,...s..
-00001d80: 0000 0002 7a17 4261 7243 6861 7274 2e6f  ....z.BarChart.o
-00001d90: 6e5f 6368 6172 745f 6576 656e 7463 0200  n_chart_eventc..
-00001da0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001db0: 0000 4300 0000 7332 0000 007c 006a 00a0  ..C...s2...|.j..
-00001dc0: 017c 01a1 0101 007c 0164 0075 0172 227c  .|.....|.d.u.r"|
-00001dd0: 00a0 0264 0164 02a1 0201 006e 0c7c 00a0  ...d.d.....n.|..
-00001de0: 0264 0164 00a1 0201 0064 0053 0029 034e  .d.d.....d.S.).N
-00001df0: 5a0c 6f6e 4368 6172 7445 7665 6e74 5429  Z.onChartEventT)
-00001e00: 0372 4900 0000 da09 7375 6273 6372 6962  .rI.....subscrib
-00001e10: 6572 7300 0000 2902 724d 0000 00da 0768  ers...).rM.....h
-00001e20: 616e 646c 6572 7245 0000 0072 4500 0000  andlerrE...rE...
-00001e30: 7246 0000 0072 4c00 0000 3001 0000 7308  rF...rL...0...s.
-00001e40: 0000 0000 020c 0108 010e 0229 2b4e 4e4e  ...........)+NNN
-00001e50: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
+00000980: 6c65 742f 666c 6574 636f 6e74 7269 622f  let/fletcontrib/
+00000990: 7364 6b2f 7079 7468 6f6e 2f70 6163 6b61  sdk/python/packa
+000009a0: 6765 732f 666c 6574 2d63 6f72 652f 7372  ges/flet-core/sr
+000009b0: 632f 666c 6574 5f63 6f72 652f 6368 6172  c/flet_core/char
+000009c0: 7473 2f62 6172 5f63 6861 7274 2e70 79da  ts/bar_chart.py.
+000009d0: 1c63 6f6e 7665 7274 5f6c 696e 6563 6861  .convert_linecha
+000009e0: 7274 5f65 7665 6e74 5f64 6174 6166 0000  rt_event_dataf..
+000009f0: 0073 0400 0000 0001 0c01 7a37 4261 7243  .s........z7BarC
+00000a00: 6861 7274 2e5f 5f69 6e69 745f 5f2e 3c6c  hart.__init__.<l
+00000a10: 6f63 616c 733e 2e63 6f6e 7665 7274 5f6c  ocals>.convert_l
+00000a20: 696e 6563 6861 7274 5f65 7665 6e74 5f64  inechart_event_d
+00000a30: 6174 615a 0b63 6861 7274 5f65 7665 6e74  ataZ.chart_event
+00000a40: 2917 720a 0000 00da 085f 5f69 6e69 745f  ).r......__init_
+00000a50: 5f72 0d00 0000 da19 5f42 6172 4368 6172  _r......_BarChar
+00000a60: 745f 5f6f 6e5f 6368 6172 745f 6576 656e  t__on_chart_even
+00000a70: 74da 125f 6164 645f 6576 656e 745f 6861  t.._add_event_ha
+00000a80: 6e64 6c65 72da 0b67 6574 5f68 616e 646c  ndler..get_handl
+00000a90: 6572 7215 0000 0072 1600 0000 7217 0000  err....r....r...
+00000aa0: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000ab0: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000ac0: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
+00000ad0: 0000 0072 2200 0000 7223 0000 0072 2400  ...r"...r#...r$.
+00000ae0: 0000 da0e 6f6e 5f63 6861 7274 5f65 7665  ....on_chart_eve
+00000af0: 6e74 292d da04 7365 6c66 7215 0000 0072  nt)-..selfr....r
+00000b00: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+00000b10: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000b20: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000b30: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000b40: 7223 0000 0072 2400 0000 724c 0000 0072  r#...r$...rL...r
+00000b50: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
+00000b60: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00000b70: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+00000b80: 0072 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
+00000b90: 7232 0000 0072 3300 0000 7234 0000 0072  r2...r3...r4...r
+00000ba0: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
+00000bb0: 0000 0072 3900 0000 723e 0000 0072 3a00  ...r9...r>...r:.
+00000bc0: 0000 723b 0000 0072 3c00 0000 723d 0000  ..r;...r<...r=..
+00000bd0: 0072 4700 0000 7245 0000 0072 4500 0000  .rG...rE...rE...
+00000be0: 7246 0000 0072 4800 0000 1700 0000 7362  rF...rH.......sb
+00000bf0: 0000 0000 3104 0102 0102 0102 0102 0102  ....1...........
+00000c00: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000c10: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000c20: 0102 0102 0102 0102 0102 0102 e506 1e08  ................
+00000c30: 040a 0112 0206 0106 0106 0106 0106 0106  ................
+00000c40: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00000c50: 0106 0106 017a 1142 6172 4368 6172 742e  .....z.BarChart.
+00000c60: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000c70: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000c80: 0073 0400 0000 6401 5300 2902 4e5a 0862  .s....d.S.).NZ.b
+00000c90: 6172 6368 6172 7472 4500 0000 a901 724d  archartrE.....rM
+00000ca0: 0000 0072 4500 0000 7245 0000 0072 4600  ...rE...rE...rF.
+00000cb0: 0000 da11 5f67 6574 5f63 6f6e 7472 6f6c  ...._get_control
+00000cc0: 5f6e 616d 657f 0000 0073 0200 0000 0001  _name....s......
+00000cd0: 7a1a 4261 7243 6861 7274 2e5f 6765 745f  z.BarChart._get_
+00000ce0: 636f 6e74 726f 6c5f 6e61 6d65 6301 0000  control_namec...
+00000cf0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000d00: 0003 0000 0073 4600 0000 7400 8300 a001  .....sF...t.....
+00000d10: a100 0100 7c00 a002 6401 7c00 6a03 a102  ....|...d.|.j...
+00000d20: 0100 7c00 a002 6402 7c00 6a04 a102 0100  ..|...d.|.j.....
+00000d30: 7c00 a002 6403 7c00 6a05 a102 0100 7c00  |...d.|.j.....|.
+00000d40: a002 6404 7c00 6a06 a102 0100 6400 5300  ..d.|.j.....d.S.
+00000d50: 2905 4e5a 1368 6f72 697a 6f6e 7461 6c47  ).NZ.horizontalG
+00000d60: 7269 644c 696e 6573 5a11 7665 7274 6963  ridLinesZ.vertic
+00000d70: 616c 4772 6964 4c69 6e65 7372 1700 0000  alGridLinesr....
+00000d80: 721b 0000 0029 07da 0573 7570 6572 da0d  r....)...super..
+00000d90: 6265 666f 7265 5f75 7064 6174 65da 0e5f  before_update.._
+00000da0: 7365 745f 6174 7472 5f6a 736f 6eda 205f  set_attr_json. _
+00000db0: 4261 7243 6861 7274 5f5f 686f 7269 7a6f  BarChart__horizo
+00000dc0: 6e74 616c 5f67 7269 645f 6c69 6e65 73da  ntal_grid_lines.
+00000dd0: 1e5f 4261 7243 6861 7274 5f5f 7665 7274  ._BarChart__vert
+00000de0: 6963 616c 5f67 7269 645f 6c69 6e65 73da  ical_grid_lines.
+00000df0: 125f 4261 7243 6861 7274 5f5f 616e 696d  ._BarChart__anim
+00000e00: 6174 65da 115f 4261 7243 6861 7274 5f5f  ate.._BarChart__
+00000e10: 626f 7264 6572 724e 0000 00a9 01da 095f  borderrN......._
+00000e20: 5f63 6c61 7373 5f5f 7245 0000 0072 4600  _class__rE...rF.
+00000e30: 0000 7251 0000 0082 0000 0073 0a00 0000  ..rQ.......s....
+00000e40: 0001 0a01 0e01 0e01 0e01 7a16 4261 7243  ..........z.BarC
+00000e50: 6861 7274 2e62 6566 6f72 655f 7570 6461  hart.before_upda
+00000e60: 7465 6301 0000 0000 0000 0000 0000 0003  tec.............
+00000e70: 0000 0004 0000 0043 0000 0073 9e00 0000  .......C...s....
+00000e80: 6700 7d01 7c00 6a00 4400 5d0e 7d02 7c01  g.}.|.j.D.].}.|.
+00000e90: a001 7c02 a101 0100 710a 7c00 6a02 723a  ..|.....q.|.j.r:
+00000ea0: 7c00 6a02 a003 6401 6402 a102 0100 7c01  |.j...d.d.....|.
+00000eb0: a001 7c00 6a02 a101 0100 7c00 6a04 725a  ..|.j.....|.j.rZ
+00000ec0: 7c00 6a04 a003 6401 6403 a102 0100 7c01  |.j...d.d.....|.
+00000ed0: a001 7c00 6a04 a101 0100 7c00 6a05 727a  ..|.j.....|.j.rz
+00000ee0: 7c00 6a05 a003 6401 6404 a102 0100 7c01  |.j...d.d.....|.
+00000ef0: a001 7c00 6a05 a101 0100 7c00 6a06 729a  ..|.j.....|.j.r.
+00000f00: 7c00 6a06 a003 6401 6405 a102 0100 7c01  |.j...d.d.....|.
+00000f10: a001 7c00 6a06 a101 0100 7c01 5300 2906  ..|.j.....|.S.).
+00000f20: 4eda 016e da01 6cda 0174 da01 72da 0162  N..n..l..t..r..b
+00000f30: 2907 da15 5f42 6172 4368 6172 745f 5f62  )..._BarChart__b
+00000f40: 6172 5f67 726f 7570 73da 0661 7070 656e  ar_groups..appen
+00000f50: 64da 145f 4261 7243 6861 7274 5f5f 6c65  d.._BarChart__le
+00000f60: 6674 5f61 7869 73da 125f 7365 745f 6174  ft_axis.._set_at
+00000f70: 7472 5f69 6e74 6572 6e61 6cda 135f 4261  tr_internal.._Ba
+00000f80: 7243 6861 7274 5f5f 746f 705f 6178 6973  rChart__top_axis
+00000f90: da15 5f42 6172 4368 6172 745f 5f72 6967  .._BarChart__rig
+00000fa0: 6874 5f61 7869 73da 165f 4261 7243 6861  ht_axis.._BarCha
+00000fb0: 7274 5f5f 626f 7474 6f6d 5f61 7869 7329  rt__bottom_axis)
+00000fc0: 0372 4d00 0000 da08 6368 696c 6472 656e  .rM.....children
+00000fd0: 5a02 6473 7245 0000 0072 4500 0000 7246  Z.dsrE...rE...rF
+00000fe0: 0000 00da 0d5f 6765 745f 6368 696c 6472  ....._get_childr
+00000ff0: 656e 8900 0000 7320 0000 0000 0104 010a  en....s ........
+00001000: 010c 0106 010e 010c 0106 010e 010c 0106  ................
+00001010: 010e 010c 0106 010e 010c 017a 1642 6172  ...........z.Bar
+00001020: 4368 6172 742e 5f67 6574 5f63 6869 6c64  Chart._get_child
+00001030: 7265 6e63 0100 0000 0000 0000 0000 0000  renc............
+00001040: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00001050: 007c 006a 0053 0072 3f00 0000 a901 725e  .|.j.S.r?.....r^
+00001060: 0000 0072 4e00 0000 7245 0000 0072 4500  ...rN...rE...rE.
+00001070: 0000 7246 0000 0072 1500 0000 9c00 0000  ..rF...r........
+00001080: 7302 0000 0000 027a 1342 6172 4368 6172  s......z.BarChar
+00001090: 742e 6261 725f 6772 6f75 7073 6302 0000  t.bar_groupsc...
+000010a0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+000010b0: 0043 0000 0073 1600 0000 7c01 6400 7501  .C...s....|.d.u.
+000010c0: 720c 7c01 6e02 6700 7c00 5f00 6400 5300  r.|.n.g.|._.d.S.
+000010d0: 723f 0000 0072 6700 0000 a902 724d 0000  r?...rg.....rM..
+000010e0: 00da 0576 616c 7565 7245 0000 0072 4500  ...valuerE...rE.
+000010f0: 0000 7246 0000 0072 1500 0000 a000 0000  ..rF...r........
+00001100: 7302 0000 0000 02a9 01da 0672 6574 7572  s..........retur
+00001110: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
+00001120: 0000 0400 0000 4300 0000 730e 0000 007c  ......C...s....|
+00001130: 006a 0064 0164 0264 038d 0253 0029 044e  .j.d.d.d...S.).N
+00001140: da0b 6772 6f75 7073 5370 6163 65da 0566  ..groupsSpace..f
+00001150: 6c6f 6174 a901 da09 6461 7461 5f74 7970  loat....data_typ
+00001160: 65a9 01da 095f 6765 745f 6174 7472 724e  e...._get_attrrN
+00001170: 0000 0072 4500 0000 7245 0000 0072 4600  ...rE...rE...rF.
+00001180: 0000 7216 0000 00a5 0000 0073 0200 0000  ..r........s....
+00001190: 0002 7a15 4261 7243 6861 7274 2e67 726f  ..z.BarChart.gro
+000011a0: 7570 735f 7370 6163 6529 0172 6900 0000  ups_space).ri...
+000011b0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000011c0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+000011d0: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
+000011e0: 4e72 6c00 0000 a901 da09 5f73 6574 5f61  Nrl......._set_a
+000011f0: 7474 7272 6800 0000 7245 0000 0072 4500  ttrrh...rE...rE.
+00001200: 0000 7246 0000 0072 1600 0000 a900 0000  ..rF...r........
+00001210: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00001220: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00001230: 7306 0000 007c 006a 0053 0072 3f00 0000  s....|.j.S.r?...
+00001240: a901 7255 0000 0072 4e00 0000 7245 0000  ..rU...rN...rE..
+00001250: 0072 4500 0000 7246 0000 0072 1700 0000  .rE...rF...r....
+00001260: ae00 0000 7302 0000 0000 027a 1042 6172  ....s......z.Bar
+00001270: 4368 6172 742e 616e 696d 6174 6563 0200  Chart.animatec..
+00001280: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00001290: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
+000012a0: 0064 0053 0072 3f00 0000 7274 0000 0072  .d.S.r?...rt...r
+000012b0: 6800 0000 7245 0000 0072 4500 0000 7246  h...rE...rE...rF
+000012c0: 0000 0072 1700 0000 b200 0000 7302 0000  ...r........s...
+000012d0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+000012e0: 0100 0000 0300 0000 4300 0000 730a 0000  ........C...s...
+000012f0: 007c 00a0 0064 01a1 0153 00a9 024e 7219  .|...d...S...Nr.
+00001300: 0000 0072 7000 0000 724e 0000 0072 4500  ...rp...rN...rE.
+00001310: 0000 7245 0000 0072 4600 0000 7219 0000  ..rE...rF...r...
+00001320: 00b7 0000 0073 0200 0000 0002 7a10 4261  .....s......z.Ba
+00001330: 7243 6861 7274 2e62 6763 6f6c 6f72 6302  rChart.bgcolorc.
+00001340: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001350: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00001360: 6401 7c01 a102 0100 6400 5300 7275 0000  d.|.....d.S.ru..
+00001370: 0072 7200 0000 7268 0000 0072 4500 0000  .rr...rh...rE...
+00001380: 7245 0000 0072 4600 0000 7219 0000 00bb  rE...rF...r.....
+00001390: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+000013a0: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+000013b0: 0000 0073 1000 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
+000013c0: 6403 6404 8d03 5300 2905 4e72 1800 0000  d.d...S.).Nr....
+000013d0: da04 626f 6f6c 5429 0272 6f00 0000 da09  ..boolT).ro.....
+000013e0: 6465 665f 7661 6c75 6572 7000 0000 724e  def_valuerp...rN
+000013f0: 0000 0072 4500 0000 7245 0000 0072 4600  ...rE...rE...rF.
+00001400: 0000 7218 0000 00c0 0000 0073 0200 0000  ..r........s....
+00001410: 0002 7a14 4261 7243 6861 7274 2e69 6e74  ..z.BarChart.int
+00001420: 6572 6163 7469 7665 6302 0000 0000 0000  eractivec.......
+00001430: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00001440: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
+00001450: 0100 6400 5300 2902 4e72 1800 0000 7272  ..d.S.).Nr....rr
+00001460: 0000 0072 6800 0000 7245 0000 0072 4500  ...rh...rE...rE.
+00001470: 0000 7246 0000 0072 1800 0000 c400 0000  ..rF...r........
+00001480: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00001490: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+000014a0: 730a 0000 007c 00a0 0064 01a1 0153 00a9  s....|...d...S..
+000014b0: 024e 5a0e 746f 6f6c 7469 7042 6763 6f6c  .NZ.tooltipBgcol
+000014c0: 6f72 7270 0000 0072 4e00 0000 7245 0000  orrp...rN...rE..
+000014d0: 0072 4500 0000 7246 0000 0072 1a00 0000  .rE...rF...r....
+000014e0: c900 0000 7302 0000 0000 027a 1842 6172  ....s......z.Bar
+000014f0: 4368 6172 742e 746f 6f6c 7469 705f 6267  Chart.tooltip_bg
+00001500: 636f 6c6f 7263 0200 0000 0000 0000 0000  colorc..........
+00001510: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+00001520: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+00001530: 0053 0072 7800 0000 7272 0000 0072 6800  .S.rx...rr...rh.
+00001540: 0000 7245 0000 0072 4500 0000 7246 0000  ..rE...rE...rF..
+00001550: 0072 1a00 0000 cd00 0000 7302 0000 0000  .r........s.....
+00001560: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001570: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00001580: 006a 0053 0072 3f00 0000 a901 7256 0000  .j.S.r?.....rV..
+00001590: 0072 4e00 0000 7245 0000 0072 4500 0000  .rN...rE...rE...
+000015a0: 7246 0000 0072 1b00 0000 d200 0000 7302  rF...r........s.
+000015b0: 0000 0000 027a 0f42 6172 4368 6172 742e  .....z.BarChart.
+000015c0: 626f 7264 6572 6302 0000 0000 0000 0000  borderc.........
+000015d0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000015e0: 0a00 0000 7c01 7c00 5f00 6400 5300 723f  ....|.|._.d.S.r?
+000015f0: 0000 0072 7900 0000 7268 0000 0072 4500  ...ry...rh...rE.
+00001600: 0000 7245 0000 0072 4600 0000 721b 0000  ..rE...rF...r...
+00001610: 00d6 0000 0073 0200 0000 0002 6301 0000  .....s......c...
+00001620: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00001630: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00001640: 723f 0000 00a9 0172 5300 0000 724e 0000  r?.....rS...rN..
+00001650: 0072 4500 0000 7245 0000 0072 4600 0000  .rE...rE...rF...
+00001660: 721c 0000 00db 0000 0073 0200 0000 0002  r........s......
+00001670: 7a1e 4261 7243 6861 7274 2e68 6f72 697a  z.BarChart.horiz
+00001680: 6f6e 7461 6c5f 6772 6964 5f6c 696e 6573  ontal_grid_lines
+00001690: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000016a0: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
+000016b0: 7c00 5f00 6400 5300 723f 0000 0072 7a00  |._.d.S.r?...rz.
+000016c0: 0000 7268 0000 0072 4500 0000 7245 0000  ..rh...rE...rE..
+000016d0: 0072 4600 0000 721c 0000 00df 0000 0073  .rF...r........s
+000016e0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
+000016f0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
+00001700: 0600 0000 7c00 6a00 5300 723f 0000 00a9  ....|.j.S.r?....
+00001710: 0172 5400 0000 724e 0000 0072 4500 0000  .rT...rN...rE...
+00001720: 7245 0000 0072 4600 0000 721d 0000 00e4  rE...rF...r.....
+00001730: 0000 0073 0200 0000 0002 7a1c 4261 7243  ...s......z.BarC
+00001740: 6861 7274 2e76 6572 7469 6361 6c5f 6772  hart.vertical_gr
+00001750: 6964 5f6c 696e 6573 6302 0000 0000 0000  id_linesc.......
+00001760: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00001770: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00001780: 723f 0000 0072 7b00 0000 7268 0000 0072  r?...r{...rh...r
+00001790: 4500 0000 7245 0000 0072 4600 0000 721d  E...rE...rF...r.
+000017a0: 0000 00e8 0000 0073 0200 0000 0002 6301  .......s......c.
+000017b0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+000017c0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+000017d0: 5300 723f 0000 00a9 0172 6000 0000 724e  S.r?.....r`...rN
+000017e0: 0000 0072 4500 0000 7245 0000 0072 4600  ...rE...rE...rF.
+000017f0: 0000 721e 0000 00ed 0000 0073 0200 0000  ..r........s....
+00001800: 0002 7a12 4261 7243 6861 7274 2e6c 6566  ..z.BarChart.lef
+00001810: 745f 6178 6973 6302 0000 0000 0000 0000  t_axisc.........
+00001820: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00001830: 0a00 0000 7c01 7c00 5f00 6400 5300 723f  ....|.|._.d.S.r?
+00001840: 0000 0072 7c00 0000 7268 0000 0072 4500  ...r|...rh...rE.
+00001850: 0000 7245 0000 0072 4600 0000 721e 0000  ..rE...rF...r...
+00001860: 00f1 0000 0073 0200 0000 0002 6301 0000  .....s......c...
+00001870: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00001880: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00001890: 723f 0000 00a9 0172 6200 0000 724e 0000  r?.....rb...rN..
+000018a0: 0072 4500 0000 7245 0000 0072 4600 0000  .rE...rE...rF...
+000018b0: 721f 0000 00f6 0000 0073 0200 0000 0002  r........s......
+000018c0: 7a11 4261 7243 6861 7274 2e74 6f70 5f61  z.BarChart.top_a
+000018d0: 7869 7363 0200 0000 0000 0000 0000 0000  xisc............
+000018e0: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+000018f0: 007c 017c 005f 0064 0053 0072 3f00 0000  .|.|._.d.S.r?...
+00001900: 727d 0000 0072 6800 0000 7245 0000 0072  r}...rh...rE...r
+00001910: 4500 0000 7246 0000 0072 1f00 0000 fa00  E...rF...r......
+00001920: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
+00001930: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00001940: 0000 7306 0000 007c 006a 0053 0072 3f00  ..s....|.j.S.r?.
+00001950: 0000 a901 7263 0000 0072 4e00 0000 7245  ....rc...rN...rE
+00001960: 0000 0072 4500 0000 7246 0000 0072 2000  ...rE...rF...r .
+00001970: 0000 ff00 0000 7302 0000 0000 027a 1342  ......s......z.B
+00001980: 6172 4368 6172 742e 7269 6768 745f 6178  arChart.right_ax
+00001990: 6973 6302 0000 0000 0000 0000 0000 0002  isc.............
+000019a0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+000019b0: 7c01 7c00 5f00 6400 5300 723f 0000 0072  |.|._.d.S.r?...r
+000019c0: 7e00 0000 7268 0000 0072 4500 0000 7245  ~...rh...rE...rE
+000019d0: 0000 0072 4600 0000 7220 0000 0003 0100  ...rF...r ......
+000019e0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
+000019f0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00001a00: 0073 0600 0000 7c00 6a00 5300 723f 0000  .s....|.j.S.r?..
+00001a10: 00a9 0172 6400 0000 724e 0000 0072 4500  ...rd...rN...rE.
+00001a20: 0000 7245 0000 0072 4600 0000 7221 0000  ..rE...rF...r!..
+00001a30: 0008 0100 0073 0200 0000 0002 7a14 4261  .....s......z.Ba
+00001a40: 7243 6861 7274 2e62 6f74 746f 6d5f 6178  rChart.bottom_ax
+00001a50: 6973 6302 0000 0000 0000 0000 0000 0002  isc.............
+00001a60: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00001a70: 7c01 7c00 5f00 6400 5300 723f 0000 0072  |.|._.d.S.r?...r
+00001a80: 7f00 0000 7268 0000 0072 4500 0000 7245  ....rh...rE...rE
+00001a90: 0000 0072 4600 0000 7221 0000 000c 0100  ...rF...r!......
+00001aa0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
+00001ab0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00001ac0: 0073 0e00 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
+00001ad0: 8d02 5300 2904 4eda 0962 6173 656c 696e  ..S.).N..baselin
+00001ae0: 6579 726d 0000 0072 6e00 0000 7270 0000  eyrm...rn...rp..
+00001af0: 0072 4e00 0000 7245 0000 0072 4500 0000  .rN...rE...rE...
+00001b00: 7246 0000 0072 2200 0000 1101 0000 7302  rF...r".......s.
+00001b10: 0000 0000 027a 1342 6172 4368 6172 742e  .....z.BarChart.
+00001b20: 6261 7365 6c69 6e65 5f79 6302 0000 0000  baseline_yc.....
+00001b30: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00001b40: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
+00001b50: a102 0100 6400 5300 2902 4e72 8000 0000  ....d.S.).Nr....
+00001b60: 7272 0000 0072 6800 0000 7245 0000 0072  rr...rh...rE...r
+00001b70: 4500 0000 7246 0000 0072 2200 0000 1501  E...rF...r".....
+00001b80: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
+00001b90: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00001ba0: 0000 730e 0000 007c 006a 0064 0164 0264  ..s....|.j.d.d.d
+00001bb0: 038d 0253 0029 044e da04 6d69 6e79 726d  ...S.).N..minyrm
+00001bc0: 0000 0072 6e00 0000 7270 0000 0072 4e00  ...rn...rp...rN.
+00001bd0: 0000 7245 0000 0072 4500 0000 7246 0000  ..rE...rE...rF..
+00001be0: 0072 2300 0000 1a01 0000 7302 0000 0000  .r#.......s.....
+00001bf0: 027a 0e42 6172 4368 6172 742e 6d69 6e5f  .z.BarChart.min_
+00001c00: 7963 0200 0000 0000 0000 0000 0000 0200  yc..............
+00001c10: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
+00001c20: 00a0 0064 017c 01a1 0201 0064 0053 0029  ...d.|.....d.S.)
+00001c30: 024e 7281 0000 0072 7200 0000 7268 0000  .Nr....rr...rh..
+00001c40: 0072 4500 0000 7245 0000 0072 4600 0000  .rE...rE...rF...
+00001c50: 7223 0000 001e 0100 0073 0200 0000 0002  r#.......s......
+00001c60: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001c70: 0004 0000 0043 0000 0073 0e00 0000 7c00  .....C...s....|.
+00001c80: 6a00 6401 6402 6403 8d02 5300 2904 4eda  j.d.d.d...S.).N.
+00001c90: 046d 6178 7972 6d00 0000 726e 0000 0072  .maxyrm...rn...r
+00001ca0: 7000 0000 724e 0000 0072 4500 0000 7245  p...rN...rE...rE
+00001cb0: 0000 0072 4600 0000 7224 0000 0023 0100  ...rF...r$...#..
+00001cc0: 0073 0200 0000 0002 7a0e 4261 7243 6861  .s......z.BarCha
+00001cd0: 7274 2e6d 6178 5f79 6302 0000 0000 0000  rt.max_yc.......
+00001ce0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00001cf0: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
+00001d00: 0100 6400 5300 2902 4e72 8200 0000 7272  ..d.S.).Nr....rr
+00001d10: 0000 0072 6800 0000 7245 0000 0072 4500  ...rh...rE...rE.
+00001d20: 0000 7246 0000 0072 2400 0000 2701 0000  ..rF...r$...'...
+00001d30: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00001d40: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00001d50: 7306 0000 007c 006a 0053 0072 3f00 0000  s....|.j.S.r?...
+00001d60: 2901 7249 0000 0072 4e00 0000 7245 0000  ).rI...rN...rE..
+00001d70: 0072 4500 0000 7246 0000 0072 4c00 0000  .rE...rF...rL...
+00001d80: 2c01 0000 7302 0000 0000 027a 1742 6172  ,...s......z.Bar
+00001d90: 4368 6172 742e 6f6e 5f63 6861 7274 5f65  Chart.on_chart_e
+00001da0: 7665 6e74 6302 0000 0000 0000 0000 0000  ventc...........
+00001db0: 0002 0000 0004 0000 0043 0000 0073 3200  .........C...s2.
+00001dc0: 0000 7c00 6a00 a001 7c01 a101 0100 7c01  ..|.j...|.....|.
+00001dd0: 6400 7501 7222 7c00 a002 6401 6402 a102  d.u.r"|...d.d...
+00001de0: 0100 6e0c 7c00 a002 6401 6400 a102 0100  ..n.|...d.d.....
+00001df0: 6400 5300 2903 4e5a 0c6f 6e43 6861 7274  d.S.).NZ.onChart
+00001e00: 4576 656e 7454 2903 7249 0000 00da 0973  EventT).rI.....s
+00001e10: 7562 7363 7269 6265 7273 0000 0029 0272  ubscribers...).r
+00001e20: 4d00 0000 da07 6861 6e64 6c65 7272 4500  M.....handlerrE.
+00001e30: 0000 7245 0000 0072 4600 0000 724c 0000  ..rE...rF...rL..
+00001e40: 0030 0100 0073 0800 0000 0002 0c01 0801  .0...s..........
+00001e50: 0e02 292b 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  ..)+NNNNNNNNNNNN
 00001e60: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
-00001e70: 4e4e 4e4e 4e4e 4e4e 292d da08 5f5f 6e61  NNNNNNNN)-..__na
-00001e80: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00001e90: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7204  ..__qualname__r.
-00001ea0: 0000 0072 0300 0000 7207 0000 0072 0b00  ...r....r....r..
-00001eb0: 0000 720f 0000 0072 7600 0000 da03 7374  ..r....rv.....st
-00001ec0: 7272 0600 0000 7209 0000 0072 0800 0000  rr....r....r....
-00001ed0: 720e 0000 0072 0500 0000 da03 696e 7472  r....r......intr
-00001ee0: 1100 0000 7212 0000 0072 1300 0000 7210  ....r....r....r.
-00001ef0: 0000 0072 0200 0000 7248 0000 0072 4f00  ...r....rH...rO.
-00001f00: 0000 7251 0000 0072 6600 0000 da08 7072  ..rQ...rf.....pr
-00001f10: 6f70 6572 7479 7215 0000 00da 0673 6574  opertyr......set
-00001f20: 7465 7272 1600 0000 7217 0000 0072 1900  terr....r....r..
-00001f30: 0000 7218 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00001f40: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00001f50: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00001f60: 2200 0000 7223 0000 0072 2400 0000 724c  "...r#...r$...rL
-00001f70: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00001f80: 5f5f 7245 0000 0072 4500 0000 7257 0000  __rE...rE...rW..
-00001f90: 0072 4600 0000 7214 0000 0016 0000 0073  .rF...r........s
-00001fa0: 3a01 0000 0803 0001 0001 0001 0001 0001  :...............
-00001fb0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00001fc0: 0001 0001 0001 0004 0001 0001 0001 0001  ................
-00001fd0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00001fe0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00001ff0: 0001 0001 0001 0001 0001 00d1 0202 0a01  ................
-00002000: 0201 0201 0601 0601 0601 0601 0601 0601  ................
-00002010: 0601 0601 0601 0601 0201 0201 0205 0601  ................
-00002020: 0201 0201 0201 0201 0201 0201 0c01 0601  ................
-00002030: 0601 0201 0201 0201 0201 0201 0201 0201  ................
-00002040: 0201 0201 0201 0202 0601 0601 0601 02d1  ................
-00002050: 0c68 0803 0c07 0813 0201 0a03 0401 0a04  .h..............
-00002060: 0201 1003 0401 1004 0201 1003 0401 1004  ................
-00002070: 0201 1403 0401 1404 0201 1403 0401 1404  ................
-00002080: 0201 1403 0401 1404 0201 1403 0401 1404  ................
-00002090: 0201 1403 0401 1404 0201 1403 0401 1404  ................
-000020a0: 0201 1403 0401 1404 0201 1403 0401 1404  ................
-000020b0: 0201 1403 0401 1404 0201 1403 0401 1404  ................
-000020c0: 0201 1003 0401 1004 0201 1003 0401 1004  ................
-000020d0: 0201 1003 0401 1004 0201 0a03 0401 7214  ..............r.
-000020e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000020f0: 0000 0000 0300 0000 4000 0000 731a 0000  ........@...s...
-00002100: 0065 005a 0164 005a 0264 0164 029c 0164  .e.Z.d.Z.d.d...d
-00002110: 0364 0484 045a 0364 0153 0029 0572 4200  .d...Z.d.S.).rB.
-00002120: 0000 4e72 6a00 0000 6305 0000 0000 0000  ..Nrj...c.......
-00002130: 0000 0000 0005 0000 0002 0000 0043 0000  .............C..
-00002140: 0073 1c00 0000 7c01 7c00 5f00 7c02 7c00  .s....|.|._.|.|.
-00002150: 5f01 7c03 7c00 5f02 7c04 7c00 5f03 6400  _.|.|._.|.|._.d.
-00002160: 5300 723f 0000 0029 04da 0474 7970 65da  S.r?...)...type.
-00002170: 0b67 726f 7570 5f69 6e64 6578 da09 726f  .group_index..ro
-00002180: 645f 696e 6465 78da 1073 7461 636b 5f69  d_index..stack_i
-00002190: 7465 6d5f 696e 6465 7829 0572 4d00 0000  tem_index).rM...
-000021a0: 728d 0000 0072 8e00 0000 728f 0000 0072  r....r....r....r
-000021b0: 9000 0000 7245 0000 0072 4500 0000 7246  ....rE...rE...rF
-000021c0: 0000 0072 4800 0000 3a01 0000 7308 0000  ...rH...:...s...
-000021d0: 0000 0106 0106 0106 017a 1642 6172 4368  .........z.BarCh
-000021e0: 6172 7445 7665 6e74 2e5f 5f69 6e69 745f  artEvent.__init_
-000021f0: 5f29 0472 8500 0000 7286 0000 0072 8700  _).r....r....r..
-00002200: 0000 7248 0000 0072 4500 0000 7245 0000  ..rH...rE...rE..
-00002210: 0072 4500 0000 7246 0000 0072 4200 0000  .rE...rF...rB...
-00002220: 3901 0000 7302 0000 0008 0172 4200 0000  9...s......rB...
-00002230: 2920 7240 0000 00da 0674 7970 696e 6772  ) r@.....typingr
-00002240: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
-00002250: 0000 00da 1066 6c65 745f 636f 7265 2e62  .....flet_core.b
-00002260: 6f72 6465 7272 0600 0000 da20 666c 6574  orderr..... flet
-00002270: 5f63 6f72 652e 6368 6172 7473 2e62 6172  _core.charts.bar
-00002280: 5f63 6861 7274 5f67 726f 7570 7207 0000  _chart_groupr...
-00002290: 00da 1b66 6c65 745f 636f 7265 2e63 6861  ...flet_core.cha
-000022a0: 7274 732e 6368 6172 745f 6178 6973 7208  rts.chart_axisr.
-000022b0: 0000 00da 2166 6c65 745f 636f 7265 2e63  ....!flet_core.c
-000022c0: 6861 7274 732e 6368 6172 745f 6772 6964  harts.chart_grid
-000022d0: 5f6c 696e 6573 7209 0000 00da 1d66 6c65  _linesr......fle
-000022e0: 745f 636f 7265 2e63 6f6e 7374 7261 696e  t_core.constrain
-000022f0: 6564 5f63 6f6e 7472 6f6c 720a 0000 00da  ed_controlr.....
-00002300: 1166 6c65 745f 636f 7265 2e63 6f6e 7472  .flet_core.contr
-00002310: 6f6c 720b 0000 00da 1766 6c65 745f 636f  olr......flet_co
-00002320: 7265 2e63 6f6e 7472 6f6c 5f65 7665 6e74  re.control_event
-00002330: 720c 0000 00da 1766 6c65 745f 636f 7265  r......flet_core
-00002340: 2e65 7665 6e74 5f68 616e 646c 6572 720d  .event_handlerr.
-00002350: 0000 00da 0d66 6c65 745f 636f 7265 2e72  .....flet_core.r
-00002360: 6566 720e 0000 00da 0f66 6c65 745f 636f  efr......flet_co
-00002370: 7265 2e74 7970 6573 720f 0000 0072 1000  re.typesr....r..
-00002380: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00002390: 0072 1400 0000 7242 0000 0072 4500 0000  .r....rB...rE...
-000023a0: 7245 0000 0072 4500 0000 7246 0000 00da  rE...rE...rF....
-000023b0: 083c 6d6f 6475 6c65 3e01 0000 0073 1e00  .<module>....s..
-000023c0: 0000 0801 1802 0c01 0c01 0c01 0c01 0c01  ................
-000023d0: 0c01 0c01 0c01 0c01 1c09 107f 007f 0025  ...............%
+00001e70: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e29  NNNNNNNNNNNNNNN)
+00001e80: 2dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  -..__name__..__m
+00001e90: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00001ea0: 616d 655f 5f72 0400 0000 7203 0000 0072  ame__r....r....r
+00001eb0: 0700 0000 720b 0000 0072 0f00 0000 7276  ....r....r....rv
+00001ec0: 0000 00da 0373 7472 7206 0000 0072 0900  .....strr....r..
+00001ed0: 0000 7208 0000 0072 0e00 0000 7205 0000  ..r....r....r...
+00001ee0: 00da 0369 6e74 7211 0000 0072 1200 0000  ...intr....r....
+00001ef0: 7213 0000 0072 1000 0000 7202 0000 0072  r....r....r....r
+00001f00: 4800 0000 724f 0000 0072 5100 0000 7266  H...rO...rQ...rf
+00001f10: 0000 00da 0870 726f 7065 7274 7972 1500  .....propertyr..
+00001f20: 0000 da06 7365 7474 6572 7216 0000 0072  ....setterr....r
+00001f30: 1700 0000 7219 0000 0072 1800 0000 721a  ....r....r....r.
+00001f40: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+00001f50: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00001f60: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
+00001f70: 7224 0000 0072 4c00 0000 da0d 5f5f 636c  r$...rL.....__cl
+00001f80: 6173 7363 656c 6c5f 5f72 4500 0000 7245  asscell__rE...rE
+00001f90: 0000 0072 5700 0000 7246 0000 0072 1400  ...rW...rF...r..
+00001fa0: 0000 1600 0000 733a 0100 0008 0300 0100  ......s:........
+00001fb0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+00001fc0: 0100 0100 0100 0100 0100 0100 0100 0400  ................
+00001fd0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+00001fe0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+00001ff0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+00002000: 0100 d102 020a 0102 0102 0106 0106 0106  ................
+00002010: 0106 0106 0106 0106 0106 0106 0106 0102  ................
+00002020: 0102 0102 0506 0102 0102 0102 0102 0102  ................
+00002030: 0102 010c 0106 0106 0102 0102 0102 0102  ................
+00002040: 0102 0102 0102 0102 0102 0102 0102 0206  ................
+00002050: 0106 0106 0102 d10c 6808 030c 0708 1302  ........h.......
+00002060: 010a 0304 010a 0402 0110 0304 0110 0402  ................
+00002070: 0110 0304 0110 0402 0114 0304 0114 0402  ................
+00002080: 0114 0304 0114 0402 0114 0304 0114 0402  ................
+00002090: 0114 0304 0114 0402 0114 0304 0114 0402  ................
+000020a0: 0114 0304 0114 0402 0114 0304 0114 0402  ................
+000020b0: 0114 0304 0114 0402 0114 0304 0114 0402  ................
+000020c0: 0114 0304 0114 0402 0110 0304 0110 0402  ................
+000020d0: 0110 0304 0110 0402 0110 0304 0110 0402  ................
+000020e0: 010a 0304 0172 1400 0000 6300 0000 0000  .....r....c.....
+000020f0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00002100: 0000 0073 1a00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00002110: 6401 6402 9c01 6403 6404 8404 5a03 6401  d.d...d.d...Z.d.
+00002120: 5300 2905 7242 0000 004e 726a 0000 0063  S.).rB...Nrj...c
+00002130: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+00002140: 0200 0000 4300 0000 731c 0000 007c 017c  ....C...s....|.|
+00002150: 005f 007c 027c 005f 017c 037c 005f 027c  ._.|.|._.|.|._.|
+00002160: 047c 005f 0364 0053 0072 3f00 0000 2904  .|._.d.S.r?...).
+00002170: da04 7479 7065 da0b 6772 6f75 705f 696e  ..type..group_in
+00002180: 6465 78da 0972 6f64 5f69 6e64 6578 da10  dex..rod_index..
+00002190: 7374 6163 6b5f 6974 656d 5f69 6e64 6578  stack_item_index
+000021a0: 2905 724d 0000 0072 8d00 0000 728e 0000  ).rM...r....r...
+000021b0: 0072 8f00 0000 7290 0000 0072 4500 0000  .r....r....rE...
+000021c0: 7245 0000 0072 4600 0000 7248 0000 003a  rE...rF...rH...:
+000021d0: 0100 0073 0800 0000 0001 0601 0601 0601  ...s............
+000021e0: 7a16 4261 7243 6861 7274 4576 656e 742e  z.BarChartEvent.
+000021f0: 5f5f 696e 6974 5f5f 2904 7285 0000 0072  __init__).r....r
+00002200: 8600 0000 7287 0000 0072 4800 0000 7245  ....r....rH...rE
+00002210: 0000 0072 4500 0000 7245 0000 0072 4600  ...rE...rE...rF.
+00002220: 0000 7242 0000 0039 0100 0073 0200 0000  ..rB...9...s....
+00002230: 0801 7242 0000 0029 2072 4000 0000 da06  ..rB...) r@.....
+00002240: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
+00002250: 7204 0000 0072 0500 0000 da10 666c 6574  r....r......flet
+00002260: 5f63 6f72 652e 626f 7264 6572 7206 0000  _core.borderr...
+00002270: 00da 2066 6c65 745f 636f 7265 2e63 6861  .. flet_core.cha
+00002280: 7274 732e 6261 725f 6368 6172 745f 6772  rts.bar_chart_gr
+00002290: 6f75 7072 0700 0000 da1b 666c 6574 5f63  oupr......flet_c
+000022a0: 6f72 652e 6368 6172 7473 2e63 6861 7274  ore.charts.chart
+000022b0: 5f61 7869 7372 0800 0000 da21 666c 6574  _axisr.....!flet
+000022c0: 5f63 6f72 652e 6368 6172 7473 2e63 6861  _core.charts.cha
+000022d0: 7274 5f67 7269 645f 6c69 6e65 7372 0900  rt_grid_linesr..
+000022e0: 0000 da1d 666c 6574 5f63 6f72 652e 636f  ....flet_core.co
+000022f0: 6e73 7472 6169 6e65 645f 636f 6e74 726f  nstrained_contro
+00002300: 6c72 0a00 0000 da11 666c 6574 5f63 6f72  lr......flet_cor
+00002310: 652e 636f 6e74 726f 6c72 0b00 0000 da17  e.controlr......
+00002320: 666c 6574 5f63 6f72 652e 636f 6e74 726f  flet_core.contro
+00002330: 6c5f 6576 656e 7472 0c00 0000 da17 666c  l_eventr......fl
+00002340: 6574 5f63 6f72 652e 6576 656e 745f 6861  et_core.event_ha
+00002350: 6e64 6c65 7272 0d00 0000 da0d 666c 6574  ndlerr......flet
+00002360: 5f63 6f72 652e 7265 6672 0e00 0000 da0f  _core.refr......
+00002370: 666c 6574 5f63 6f72 652e 7479 7065 7372  flet_core.typesr
+00002380: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
+00002390: 0000 0072 1300 0000 7214 0000 0072 4200  ...r....r....rB.
+000023a0: 0000 7245 0000 0072 4500 0000 7245 0000  ..rE...rE...rE..
+000023b0: 0072 4600 0000 da08 3c6d 6f64 756c 653e  .rF.....<module>
+000023c0: 0100 0000 731e 0000 0008 0118 020c 010c  ....s...........
+000023d0: 010c 010c 010c 010c 010c 010c 010c 011c  ................
+000023e0: 0910 7f00 7f00 25                        ......%
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 2044 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 fc07 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 fc07 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000070: 8400 6406 6507 8303 5a0b 6407 5300 2908  ..d.e...Z.d.S.).
@@ -42,132 +42,132 @@
 00000290: 7c00 5f05 6400 5300 2902 4e29 0472 0e00  |._.d.S.).N).r..
 000002a0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
 000002b0: 0029 0672 0600 0000 da08 5f5f 696e 6974  .).r......__init
 000002c0: 5f5f 720a 0000 0072 0b00 0000 720c 0000  __r....r....r...
 000002d0: 0072 0d00 0000 2909 da04 7365 6c66 720a  .r....)...selfr.
 000002e0: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
 000002f0: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000300: 0072 1100 0000 a900 7214 0000 00fa 622f  .r......r.....b/
+00000300: 0072 1100 0000 a900 7214 0000 00fa 692f  .r......r.....i/
 00000310: 776f 726b 7370 6163 6573 2f63 6f6e 7472  workspaces/contr
-00000320: 6962 666c 6574 2f66 6c65 742f 7364 6b2f  ibflet/flet/sdk/
-00000330: 7079 7468 6f6e 2f70 6163 6b61 6765 732f  python/packages/
-00000340: 666c 6574 2d63 6f72 652f 7372 632f 666c  flet-core/src/fl
-00000350: 6574 5f63 6f72 652f 6368 6172 7473 2f62  et_core/charts/b
-00000360: 6172 5f63 6861 7274 5f67 726f 7570 2e70  ar_chart_group.p
-00000370: 7972 1200 0000 0900 0000 7316 0000 0000  yr........s.....
-00000380: 0f04 0102 0102 0102 0102 0102 fb06 0806  ................
-00000390: 0106 0106 017a 1642 6172 4368 6172 7447  .....z.BarChartG
-000003a0: 726f 7570 2e5f 5f69 6e69 745f 5f63 0100  roup.__init__c..
-000003b0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000003c0: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
-000003d0: 024e da05 6772 6f75 7072 1400 0000 a901  .N..groupr......
-000003e0: 7213 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-000003f0: 1500 0000 da11 5f67 6574 5f63 6f6e 7472  ......_get_contr
-00000400: 6f6c 5f6e 616d 6525 0000 0073 0200 0000  ol_name%...s....
-00000410: 0001 7a1f 4261 7243 6861 7274 4772 6f75  ..z.BarChartGrou
-00000420: 702e 5f67 6574 5f63 6f6e 7472 6f6c 5f6e  p._get_control_n
-00000430: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-00000440: 0100 0000 0200 0000 0300 0000 730e 0000  ............s...
-00000450: 0074 0083 00a0 01a1 0001 0064 0053 00a9  .t.........d.S..
-00000460: 014e 2902 da05 7375 7065 72da 0d62 6566  .N)...super..bef
-00000470: 6f72 655f 7570 6461 7465 7217 0000 00a9  ore_updater.....
-00000480: 01da 095f 5f63 6c61 7373 5f5f 7214 0000  ...__class__r...
-00000490: 0072 1500 0000 721b 0000 0028 0000 0073  .r....r....(...s
-000004a0: 0200 0000 0001 7a1b 4261 7243 6861 7274  ......z.BarChart
-000004b0: 4772 6f75 702e 6265 666f 7265 5f75 7064  Group.before_upd
-000004c0: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
-000004d0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
-000004e0: 007c 006a 0053 0072 1900 0000 a901 5a18  .|.j.S.r......Z.
-000004f0: 5f42 6172 4368 6172 7447 726f 7570 5f5f  _BarChartGroup__
-00000500: 6261 725f 726f 6473 7217 0000 0072 1400  bar_rodsr....r..
-00000510: 0000 7214 0000 0072 1500 0000 da0d 5f67  ..r....r......_g
-00000520: 6574 5f63 6869 6c64 7265 6e2b 0000 0073  et_children+...s
-00000530: 0200 0000 0001 7a1b 4261 7243 6861 7274  ......z.BarChart
-00000540: 4772 6f75 702e 5f67 6574 5f63 6869 6c64  Group._get_child
-00000550: 7265 6e63 0100 0000 0000 0000 0000 0000  renc............
-00000560: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
-00000570: 007c 006a 0053 0072 1900 0000 721e 0000  .|.j.S.r....r...
-00000580: 0072 1700 0000 7214 0000 0072 1400 0000  .r....r....r....
-00000590: 7215 0000 0072 0b00 0000 2f00 0000 7302  r....r..../...s.
-000005a0: 0000 0000 027a 1642 6172 4368 6172 7447  .....z.BarChartG
-000005b0: 726f 7570 2e62 6172 5f72 6f64 7363 0200  roup.bar_rodsc..
-000005c0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000005d0: 0000 4300 0000 7316 0000 007c 0164 0075  ..C...s....|.d.u
-000005e0: 0172 0c7c 016e 0267 007c 005f 0064 0053  .r.|.n.g.|._.d.S
-000005f0: 0072 1900 0000 721e 0000 00a9 0272 1300  .r....r......r..
-00000600: 0000 da05 7661 6c75 6572 1400 0000 7214  ....valuer....r.
-00000610: 0000 0072 1500 0000 720b 0000 0033 0000  ...r....r....3..
-00000620: 0073 0200 0000 0002 2901 da06 7265 7475  .s......)...retu
-00000630: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
-00000640: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
-00000650: 7c00 6a00 6401 6402 6403 8d02 5300 2904  |.j.d.d.d...S.).
-00000660: 4e72 0a00 0000 da03 696e 74a9 01da 0964  Nr......int....d
-00000670: 6174 615f 7479 7065 a901 da09 5f67 6574  ata_type...._get
-00000680: 5f61 7474 7272 1700 0000 7214 0000 0072  _attrr....r....r
-00000690: 1400 0000 7215 0000 0072 0a00 0000 3800  ....r....r....8.
-000006a0: 0000 7302 0000 0000 027a 0f42 6172 4368  ..s......z.BarCh
-000006b0: 6172 7447 726f 7570 2e78 2901 7221 0000  artGroup.x).r!..
-000006c0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-000006d0: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
-000006e0: 00a0 0064 017c 01a1 0201 0064 0053 0029  ...d.|.....d.S.)
-000006f0: 024e 720a 0000 00a9 01da 095f 7365 745f  .Nr........_set_
-00000700: 6174 7472 7220 0000 0072 1400 0000 7214  attrr ...r....r.
-00000710: 0000 0072 1500 0000 720a 0000 003c 0000  ...r....r....<..
-00000720: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000730: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-00000740: 0073 1000 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
-00000750: 6404 8d03 5300 2905 4eda 0f67 726f 7570  d...S.).N..group
-00000760: 5665 7274 6963 616c 6c79 da04 626f 6f6c  Vertically..bool
-00000770: 4629 0272 2500 0000 da09 6465 665f 7661  F).r%.....def_va
-00000780: 6c75 6572 2600 0000 7217 0000 0072 1400  luer&...r....r..
-00000790: 0000 7214 0000 0072 1500 0000 720c 0000  ..r....r....r...
-000007a0: 0041 0000 0073 0200 0000 0002 7a1e 4261  .A...s......z.Ba
-000007b0: 7243 6861 7274 4772 6f75 702e 6772 6f75  rChartGroup.grou
-000007c0: 705f 7665 7274 6963 616c 6c79 6302 0000  p_verticallyc...
-000007d0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000007e0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-000007f0: 7c01 a102 0100 6400 5300 2902 4e72 2a00  |.....d.S.).Nr*.
-00000800: 0000 7228 0000 0072 2000 0000 7214 0000  ..r(...r ...r...
-00000810: 0072 1400 0000 7215 0000 0072 0c00 0000  .r....r....r....
-00000820: 4500 0000 7302 0000 0000 0263 0100 0000  E...s......c....
-00000830: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00000840: 4300 0000 730e 0000 007c 006a 0064 0164  C...s....|.j.d.d
-00000850: 0264 038d 0253 0029 044e da09 6261 7273  .d...S.).N..bars
-00000860: 5370 6163 65da 0566 6c6f 6174 7224 0000  Space..floatr$..
-00000870: 0072 2600 0000 7217 0000 0072 1400 0000  .r&...r....r....
-00000880: 7214 0000 0072 1500 0000 720d 0000 004a  r....r....r....J
-00000890: 0000 0073 0200 0000 0002 7a18 4261 7243  ...s......z.BarC
-000008a0: 6861 7274 4772 6f75 702e 6261 7273 5f73  hartGroup.bars_s
-000008b0: 7061 6365 6302 0000 0000 0000 0000 0000  pacec...........
-000008c0: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-000008d0: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
-000008e0: 5300 2902 4e72 2d00 0000 7228 0000 0072  S.).Nr-...r(...r
-000008f0: 2000 0000 7214 0000 0072 1400 0000 7215   ...r....r....r.
-00000900: 0000 0072 0d00 0000 4e00 0000 7302 0000  ...r....N...s...
-00000910: 0000 0229 084e 4e4e 4e4e 4e4e 4e29 16da  ...).NNNNNNNN)..
-00000920: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000930: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000940: 655f 5f72 0400 0000 7223 0000 0072 0300  e__r....r#...r..
-00000950: 0000 7205 0000 0072 2b00 0000 7207 0000  ..r....r+...r...
-00000960: 0072 0800 0000 7202 0000 0072 1200 0000  .r....r....r....
-00000970: 7218 0000 0072 1b00 0000 721f 0000 00da  r....r....r.....
-00000980: 0870 726f 7065 7274 7972 0b00 0000 da06  .propertyr......
-00000990: 7365 7474 6572 720a 0000 0072 0c00 0000  setterr....r....
-000009a0: 720d 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-000009b0: 6c6c 5f5f 7214 0000 0072 1400 0000 721c  ll__r....r....r.
-000009c0: 0000 0072 1500 0000 7209 0000 0008 0000  ...r....r.......
-000009d0: 0073 4a00 0000 0803 0001 0001 0001 0004  .sJ.............
-000009e0: 0001 0001 0001 00f4 0202 0601 0a01 0601  ................
-000009f0: 0204 0601 0601 0601 02f4 0c1c 0803 0c03  ................
-00000a00: 0804 0201 0a03 0401 0a04 0201 1403 0401  ................
-00000a10: 1404 0201 1403 0401 1404 0201 1003 0401  ................
-00000a20: 7209 0000 004e 290c da06 7479 7069 6e67  r....N)...typing
-00000a30: 7202 0000 0072 0300 0000 7204 0000 00da  r....r....r.....
-00000a40: 1e66 6c65 745f 636f 7265 2e63 6861 7274  .flet_core.chart
-00000a50: 732e 6261 725f 6368 6172 745f 726f 6472  s.bar_chart_rodr
-00000a60: 0500 0000 da11 666c 6574 5f63 6f72 652e  ......flet_core.
-00000a70: 636f 6e74 726f 6c72 0600 0000 7207 0000  controlr....r...
-00000a80: 00da 0d66 6c65 745f 636f 7265 2e72 6566  ...flet_core.ref
-00000a90: 7208 0000 0072 0900 0000 7214 0000 0072  r....r....r....r
-00000aa0: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
-00000ab0: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000ac0: 0014 020c 0110 010c 03                   .........
+00000320: 6962 666c 6574 2f66 6c65 7463 6f6e 7472  ibflet/fletcontr
+00000330: 6962 2f73 646b 2f70 7974 686f 6e2f 7061  ib/sdk/python/pa
+00000340: 636b 6167 6573 2f66 6c65 742d 636f 7265  ckages/flet-core
+00000350: 2f73 7263 2f66 6c65 745f 636f 7265 2f63  /src/flet_core/c
+00000360: 6861 7274 732f 6261 725f 6368 6172 745f  harts/bar_chart_
+00000370: 6772 6f75 702e 7079 7212 0000 0009 0000  group.pyr.......
+00000380: 0073 1600 0000 000f 0401 0201 0201 0201  .s..............
+00000390: 0201 02fb 0608 0601 0601 0601 7a16 4261  ............z.Ba
+000003a0: 7243 6861 7274 4772 6f75 702e 5f5f 696e  rChartGroup.__in
+000003b0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+000003c0: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+000003d0: 0000 6401 5300 2902 4eda 0567 726f 7570  ..d.S.).N..group
+000003e0: 7214 0000 00a9 0172 1300 0000 7214 0000  r......r....r...
+000003f0: 0072 1400 0000 7215 0000 00da 115f 6765  .r....r......_ge
+00000400: 745f 636f 6e74 726f 6c5f 6e61 6d65 2500  t_control_name%.
+00000410: 0000 7302 0000 0000 017a 1f42 6172 4368  ..s......z.BarCh
+00000420: 6172 7447 726f 7570 2e5f 6765 745f 636f  artGroup._get_co
+00000430: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
+00000440: 0000 0000 0000 0001 0000 0002 0000 0003  ................
+00000450: 0000 0073 0e00 0000 7400 8300 a001 a100  ...s....t.......
+00000460: 0100 6400 5300 a901 4e29 02da 0573 7570  ..d.S...N)...sup
+00000470: 6572 da0d 6265 666f 7265 5f75 7064 6174  er..before_updat
+00000480: 6572 1700 0000 a901 da09 5f5f 636c 6173  er........__clas
+00000490: 735f 5f72 1400 0000 7215 0000 0072 1b00  s__r....r....r..
+000004a0: 0000 2800 0000 7302 0000 0000 017a 1b42  ..(...s......z.B
+000004b0: 6172 4368 6172 7447 726f 7570 2e62 6566  arChartGroup.bef
+000004c0: 6f72 655f 7570 6461 7465 6301 0000 0000  ore_updatec.....
+000004d0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+000004e0: 0000 0073 0600 0000 7c00 6a00 5300 7219  ...s....|.j.S.r.
+000004f0: 0000 00a9 015a 185f 4261 7243 6861 7274  .....Z._BarChart
+00000500: 4772 6f75 705f 5f62 6172 5f72 6f64 7372  Group__bar_rodsr
+00000510: 1700 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+00000520: 0000 00da 0d5f 6765 745f 6368 696c 6472  ....._get_childr
+00000530: 656e 2b00 0000 7302 0000 0000 017a 1b42  en+...s......z.B
+00000540: 6172 4368 6172 7447 726f 7570 2e5f 6765  arChartGroup._ge
+00000550: 745f 6368 696c 6472 656e 6301 0000 0000  t_childrenc.....
+00000560: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000570: 0000 0073 0600 0000 7c00 6a00 5300 7219  ...s....|.j.S.r.
+00000580: 0000 0072 1e00 0000 7217 0000 0072 1400  ...r....r....r..
+00000590: 0000 7214 0000 0072 1500 0000 720b 0000  ..r....r....r...
+000005a0: 002f 0000 0073 0200 0000 0002 7a16 4261  ./...s......z.Ba
+000005b0: 7243 6861 7274 4772 6f75 702e 6261 725f  rChartGroup.bar_
+000005c0: 726f 6473 6302 0000 0000 0000 0000 0000  rodsc...........
+000005d0: 0002 0000 0002 0000 0043 0000 0073 1600  .........C...s..
+000005e0: 0000 7c01 6400 7501 720c 7c01 6e02 6700  ..|.d.u.r.|.n.g.
+000005f0: 7c00 5f00 6400 5300 7219 0000 0072 1e00  |._.d.S.r....r..
+00000600: 0000 a902 7213 0000 00da 0576 616c 7565  ....r......value
+00000610: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000620: 0b00 0000 3300 0000 7302 0000 0000 0229  ....3...s......)
+00000630: 01da 0672 6574 7572 6e63 0100 0000 0000  ...returnc......
+00000640: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000650: 0000 730e 0000 007c 006a 0064 0164 0264  ..s....|.j.d.d.d
+00000660: 038d 0253 0029 044e 720a 0000 00da 0369  ...S.).Nr......i
+00000670: 6e74 a901 da09 6461 7461 5f74 7970 65a9  nt....data_type.
+00000680: 01da 095f 6765 745f 6174 7472 7217 0000  ..._get_attrr...
+00000690: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+000006a0: 720a 0000 0038 0000 0073 0200 0000 0002  r....8...s......
+000006b0: 7a0f 4261 7243 6861 7274 4772 6f75 702e  z.BarChartGroup.
+000006c0: 7829 0172 2100 0000 6302 0000 0000 0000  x).r!...c.......
+000006d0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000006e0: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
+000006f0: 0100 6400 5300 2902 4e72 0a00 0000 a901  ..d.S.).Nr......
+00000700: da09 5f73 6574 5f61 7474 7272 2000 0000  .._set_attrr ...
+00000710: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000720: 0a00 0000 3c00 0000 7302 0000 0000 0263  ....<...s......c
+00000730: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000740: 0500 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
+00000750: 0064 0164 0264 0364 048d 0353 0029 054e  .d.d.d.d...S.).N
+00000760: da0f 6772 6f75 7056 6572 7469 6361 6c6c  ..groupVerticall
+00000770: 79da 0462 6f6f 6c46 2902 7225 0000 00da  y..boolF).r%....
+00000780: 0964 6566 5f76 616c 7565 7226 0000 0072  .def_valuer&...r
+00000790: 1700 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+000007a0: 0000 0072 0c00 0000 4100 0000 7302 0000  ...r....A...s...
+000007b0: 0000 027a 1e42 6172 4368 6172 7447 726f  ...z.BarChartGro
+000007c0: 7570 2e67 726f 7570 5f76 6572 7469 6361  up.group_vertica
+000007d0: 6c6c 7963 0200 0000 0000 0000 0000 0000  llyc............
+000007e0: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+000007f0: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+00000800: 0029 024e 722a 0000 0072 2800 0000 7220  .).Nr*...r(...r 
+00000810: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00000820: 0000 720c 0000 0045 0000 0073 0200 0000  ..r....E...s....
+00000830: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000840: 0000 0004 0000 0043 0000 0073 0e00 0000  .......C...s....
+00000850: 7c00 6a00 6401 6402 6403 8d02 5300 2904  |.j.d.d.d...S.).
+00000860: 4eda 0962 6172 7353 7061 6365 da05 666c  N..barsSpace..fl
+00000870: 6f61 7472 2400 0000 7226 0000 0072 1700  oatr$...r&...r..
+00000880: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000890: 0072 0d00 0000 4a00 0000 7302 0000 0000  .r....J...s.....
+000008a0: 027a 1842 6172 4368 6172 7447 726f 7570  .z.BarChartGroup
+000008b0: 2e62 6172 735f 7370 6163 6563 0200 0000  .bars_spacec....
+000008c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000008d0: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
+000008e0: 01a1 0201 0064 0053 0029 024e 722d 0000  .....d.S.).Nr-..
+000008f0: 0072 2800 0000 7220 0000 0072 1400 0000  .r(...r ...r....
+00000900: 7214 0000 0072 1500 0000 720d 0000 004e  r....r....r....N
+00000910: 0000 0073 0200 0000 0002 2908 4e4e 4e4e  ...s......).NNNN
+00000920: 4e4e 4e4e 2916 da08 5f5f 6e61 6d65 5f5f  NNNN)...__name__
+00000930: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000940: 7175 616c 6e61 6d65 5f5f 7204 0000 0072  qualname__r....r
+00000950: 2300 0000 7203 0000 0072 0500 0000 722b  #...r....r....r+
+00000960: 0000 0072 0700 0000 7208 0000 0072 0200  ...r....r....r..
+00000970: 0000 7212 0000 0072 1800 0000 721b 0000  ..r....r....r...
+00000980: 0072 1f00 0000 da08 7072 6f70 6572 7479  .r......property
+00000990: 720b 0000 00da 0673 6574 7465 7272 0a00  r......setterr..
+000009a0: 0000 720c 0000 0072 0d00 0000 da0d 5f5f  ..r....r......__
+000009b0: 636c 6173 7363 656c 6c5f 5f72 1400 0000  classcell__r....
+000009c0: 7214 0000 0072 1c00 0000 7215 0000 0072  r....r....r....r
+000009d0: 0900 0000 0800 0000 734a 0000 0008 0300  ........sJ......
+000009e0: 0100 0100 0100 0400 0100 0100 0100 f402  ................
+000009f0: 0206 010a 0106 0102 0406 0106 0106 0102  ................
+00000a00: f40c 1c08 030c 0308 0402 010a 0304 010a  ................
+00000a10: 0402 0114 0304 0114 0402 0114 0304 0114  ................
+00000a20: 0402 0110 0304 0172 0900 0000 4e29 0cda  .......r....N)..
+00000a30: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+00000a40: 0072 0400 0000 da1e 666c 6574 5f63 6f72  .r......flet_cor
+00000a50: 652e 6368 6172 7473 2e62 6172 5f63 6861  e.charts.bar_cha
+00000a60: 7274 5f72 6f64 7205 0000 00da 1166 6c65  rt_rodr......fle
+00000a70: 745f 636f 7265 2e63 6f6e 7472 6f6c 7206  t_core.controlr.
+00000a80: 0000 0072 0700 0000 da0d 666c 6574 5f63  ...r......flet_c
+00000a90: 6f72 652e 7265 6672 0800 0000 7209 0000  ore.refr....r...
+00000aa0: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
+00000ab0: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000ac0: 0000 0073 0800 0000 1402 0c01 1001 0c03  ...s............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 6679 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 171a 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 171a 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -111,344 +111,345 @@
 000006e0: 16da 0473 656c 6672 0f00 0000 7210 0000  ...selfr....r...
 000006f0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
 00000700: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
 00000710: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
 00000720: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
 00000730: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
 00000740: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-00000750: a900 7226 0000 00fa 602f 776f 726b 7370  ..r&....`/worksp
+00000750: a900 7226 0000 00fa 672f 776f 726b 7370  ..r&....g/worksp
 00000760: 6163 6573 2f63 6f6e 7472 6962 666c 6574  aces/contribflet
-00000770: 2f66 6c65 742f 7364 6b2f 7079 7468 6f6e  /flet/sdk/python
-00000780: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
-00000790: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
-000007a0: 652f 6368 6172 7473 2f62 6172 5f63 6861  e/charts/bar_cha
-000007b0: 7274 5f72 6f64 2e70 7972 2400 0000 0d00  rt_rod.pyr$.....
-000007c0: 0000 7330 0000 0000 1c04 0102 0102 0102  ..s0............
-000007d0: 0102 0102 fb06 0806 0106 0106 0106 0106  ................
-000007e0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-000007f0: 0106 0106 0106 017a 1442 6172 4368 6172  .......z.BarChar
-00000800: 7452 6f64 2e5f 5f69 6e69 745f 5f63 0100  tRod.__init__c..
-00000810: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000820: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
-00000830: 024e 5a03 726f 6472 2600 0000 a901 7225  .NZ.rodr&.....r%
-00000840: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
-00000850: 0000 da11 5f67 6574 5f63 6f6e 7472 6f6c  ...._get_control
-00000860: 5f6e 616d 6543 0000 0073 0200 0000 0001  _nameC...s......
-00000870: 7a1d 4261 7243 6861 7274 526f 642e 5f67  z.BarChartRod._g
-00000880: 6574 5f63 6f6e 7472 6f6c 5f6e 616d 6563  et_control_namec
-00000890: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000008a0: 0400 0000 0300 0000 7346 0000 0074 0083  ........sF...t..
-000008b0: 00a0 01a1 0001 007c 00a0 0264 017c 006a  .......|...d.|.j
-000008c0: 03a1 0201 007c 00a0 0264 027c 006a 04a1  .....|...d.|.j..
-000008d0: 0201 007c 00a0 0264 037c 006a 05a1 0201  ...|...d.|.j....
-000008e0: 007c 00a0 0264 047c 006a 06a1 0201 0064  .|...d.|.j.....d
-000008f0: 0053 0029 054e 7214 0000 005a 0a62 6f72  .S.).Nr....Z.bor
-00000900: 6465 7253 6964 65da 0c62 6f72 6465 7252  derSide..borderR
-00000910: 6164 6975 735a 0a62 6747 7261 6469 656e  adiusZ.bgGradien
-00000920: 7429 07da 0573 7570 6572 da0d 6265 666f  t)...super..befo
-00000930: 7265 5f75 7064 6174 65da 0e5f 7365 745f  re_update.._set_
-00000940: 6174 7472 5f6a 736f 6eda 165f 4261 7243  attr_json.._BarC
-00000950: 6861 7274 526f 645f 5f67 7261 6469 656e  hartRod__gradien
-00000960: 74da 195f 4261 7243 6861 7274 526f 645f  t.._BarChartRod_
-00000970: 5f62 6f72 6465 725f 7369 6465 da1b 5f42  _border_side.._B
-00000980: 6172 4368 6172 7452 6f64 5f5f 626f 7264  arChartRod__bord
-00000990: 6572 5f72 6164 6975 73da 195f 4261 7243  er_radius.._BarC
-000009a0: 6861 7274 526f 645f 5f62 675f 6772 6164  hartRod__bg_grad
-000009b0: 6965 6e74 7228 0000 00a9 01da 095f 5f63  ientr(.......__c
-000009c0: 6c61 7373 5f5f 7226 0000 0072 2700 0000  lass__r&...r'...
-000009d0: 722c 0000 0046 0000 0073 0a00 0000 0001  r,...F...s......
-000009e0: 0a01 0e01 0e01 0e01 7a19 4261 7243 6861  ........z.BarCha
-000009f0: 7274 526f 642e 6265 666f 7265 5f75 7064  rtRod.before_upd
-00000a00: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
-00000a10: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
-00000a20: 007c 006a 0053 00a9 014e a901 5a1d 5f42  .|.j.S...N..Z._B
-00000a30: 6172 4368 6172 7452 6f64 5f5f 726f 645f  arChartRod__rod_
-00000a40: 7374 6163 6b5f 6974 656d 7372 2800 0000  stack_itemsr(...
-00000a50: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
-00000a60: 0d5f 6765 745f 6368 696c 6472 656e 4d00  ._get_childrenM.
-00000a70: 0000 7302 0000 0000 017a 1942 6172 4368  ..s......z.BarCh
-00000a80: 6172 7452 6f64 2e5f 6765 745f 6368 696c  artRod._get_chil
-00000a90: 6472 656e 6301 0000 0000 0000 0000 0000  drenc...........
-00000aa0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000ab0: 0000 7c00 6a00 5300 7234 0000 0072 3500  ..|.j.S.r4...r5.
-00000ac0: 0000 7228 0000 0072 2600 0000 7226 0000  ..r(...r&...r&..
-00000ad0: 0072 2700 0000 720f 0000 0051 0000 0073  .r'...r....Q...s
-00000ae0: 0200 0000 0002 7a1b 4261 7243 6861 7274  ......z.BarChart
-00000af0: 526f 642e 726f 645f 7374 6163 6b5f 6974  Rod.rod_stack_it
-00000b00: 656d 7363 0200 0000 0000 0000 0000 0000  emsc............
-00000b10: 0200 0000 0200 0000 4300 0000 7316 0000  ........C...s...
-00000b20: 007c 0164 0075 0172 0c7c 016e 0267 007c  .|.d.u.r.|.n.g.|
-00000b30: 005f 0064 0053 0072 3400 0000 7235 0000  ._.d.S.r4...r5..
-00000b40: 00a9 0272 2500 0000 da05 7661 6c75 6572  ...r%.....valuer
-00000b50: 2600 0000 7226 0000 0072 2700 0000 720f  &...r&...r'...r.
-00000b60: 0000 0055 0000 0073 0200 0000 0002 2901  ...U...s......).
-00000b70: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00000b80: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00000b90: 0073 0e00 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
-00000ba0: 8d02 5300 2904 4eda 0566 726f 6d59 da05  ..S.).N..fromY..
-00000bb0: 666c 6f61 74a9 01da 0964 6174 615f 7479  float....data_ty
-00000bc0: 7065 a901 da09 5f67 6574 5f61 7474 7272  pe...._get_attrr
-00000bd0: 2800 0000 7226 0000 0072 2600 0000 7227  (...r&...r&...r'
-00000be0: 0000 0072 1000 0000 5a00 0000 7302 0000  ...r....Z...s...
-00000bf0: 0000 027a 1242 6172 4368 6172 7452 6f64  ...z.BarChartRod
-00000c00: 2e66 726f 6d5f 7929 0172 3800 0000 6302  .from_y).r8...c.
-00000c10: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000c20: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-00000c30: 6401 7c01 a102 0100 6400 5300 2902 4e72  d.|.....d.S.).Nr
-00000c40: 3a00 0000 a901 da09 5f73 6574 5f61 7474  :......._set_att
-00000c50: 7272 3700 0000 7226 0000 0072 2600 0000  rr7...r&...r&...
-00000c60: 7227 0000 0072 1000 0000 5e00 0000 7302  r'...r....^...s.
-00000c70: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00000c80: 0000 0100 0000 0400 0000 4300 0000 730e  ..........C...s.
-00000c90: 0000 007c 006a 0064 0164 0264 038d 0253  ...|.j.d.d.d...S
-00000ca0: 0029 044e da03 746f 5972 3b00 0000 723c  .).N..toYr;...r<
-00000cb0: 0000 0072 3e00 0000 7228 0000 0072 2600  ...r>...r(...r&.
-00000cc0: 0000 7226 0000 0072 2700 0000 7211 0000  ..r&...r'...r...
-00000cd0: 0063 0000 0073 0200 0000 0002 7a10 4261  .c...s......z.Ba
-00000ce0: 7243 6861 7274 526f 642e 746f 5f79 6302  rChartRod.to_yc.
-00000cf0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000d00: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-00000d10: 6401 7c01 a102 0100 6400 5300 2902 4e72  d.|.....d.S.).Nr
-00000d20: 4200 0000 7240 0000 0072 3700 0000 7226  B...r@...r7...r&
-00000d30: 0000 0072 2600 0000 7227 0000 0072 1100  ...r&...r'...r..
-00000d40: 0000 6700 0000 7302 0000 0000 0263 0100  ..g...s......c..
-00000d50: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00000d60: 0000 4300 0000 730e 0000 007c 006a 0064  ..C...s....|.j.d
-00000d70: 0164 0264 038d 0253 0029 044e 7212 0000  .d.d...S.).Nr...
-00000d80: 0072 3b00 0000 723c 0000 0072 3e00 0000  .r;...r<...r>...
-00000d90: 7228 0000 0072 2600 0000 7226 0000 0072  r(...r&...r&...r
-00000da0: 2700 0000 7212 0000 006c 0000 0073 0200  '...r....l...s..
-00000db0: 0000 0002 7a11 4261 7243 6861 7274 526f  ....z.BarChartRo
-00000dc0: 642e 7769 6474 6863 0200 0000 0000 0000  d.widthc........
-00000dd0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000de0: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00000df0: 0064 0053 0029 024e 7212 0000 0072 4000  .d.S.).Nr....r@.
-00000e00: 0000 7237 0000 0072 2600 0000 7226 0000  ..r7...r&...r&..
-00000e10: 0072 2700 0000 7212 0000 0070 0000 0073  .r'...r....p...s
-00000e20: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00000e30: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00000e40: 0a00 0000 7c00 a000 6401 a101 5300 a902  ....|...d...S...
-00000e50: 4e72 1300 0000 723e 0000 0072 2800 0000  Nr....r>...r(...
-00000e60: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
-00000e70: 1300 0000 7500 0000 7302 0000 0000 027a  ....u...s......z
-00000e80: 1142 6172 4368 6172 7452 6f64 2e63 6f6c  .BarChartRod.col
-00000e90: 6f72 6302 0000 0000 0000 0000 0000 0002  orc.............
-00000ea0: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
-00000eb0: 7c00 a000 6401 7c01 a102 0100 6400 5300  |...d.|.....d.S.
-00000ec0: 7243 0000 0072 4000 0000 7237 0000 0072  rC...r@...r7...r
-00000ed0: 2600 0000 7226 0000 0072 2700 0000 7213  &...r&...r'...r.
-00000ee0: 0000 0079 0000 0073 0200 0000 0002 6301  ...y...s......c.
-00000ef0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000f00: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00000f10: 5300 7234 0000 00a9 0172 2f00 0000 7228  S.r4.....r/...r(
-00000f20: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
-00000f30: 0000 7216 0000 007e 0000 0073 0200 0000  ..r....~...s....
-00000f40: 0002 7a17 4261 7243 6861 7274 526f 642e  ..z.BarChartRod.
-00000f50: 626f 7264 6572 5f73 6964 6563 0200 0000  border_sidec....
-00000f60: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000f70: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
-00000f80: 0053 0072 3400 0000 7244 0000 0072 3700  .S.r4...rD...r7.
-00000f90: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
-00000fa0: 0072 1600 0000 8200 0000 7302 0000 0000  .r........s.....
-00000fb0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000fc0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-00000fd0: 006a 0053 0072 3400 0000 a901 7230 0000  .j.S.r4.....r0..
-00000fe0: 0072 2800 0000 7226 0000 0072 2600 0000  .r(...r&...r&...
-00000ff0: 7227 0000 0072 1500 0000 8700 0000 7302  r'...r........s.
-00001000: 0000 0000 027a 1942 6172 4368 6172 7452  .....z.BarChartR
-00001010: 6f64 2e62 6f72 6465 725f 7261 6469 7573  od.border_radius
-00001020: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001030: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00001040: 7c00 5f00 6400 5300 7234 0000 0072 4500  |._.d.S.r4...rE.
-00001050: 0000 7237 0000 0072 2600 0000 7226 0000  ..r7...r&...r&..
-00001060: 0072 2700 0000 7215 0000 008b 0000 0073  .r'...r........s
-00001070: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00001080: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00001090: 0600 0000 7c00 6a00 5300 7234 0000 00a9  ....|.j.S.r4....
-000010a0: 0172 2e00 0000 7228 0000 0072 2600 0000  .r....r(...r&...
-000010b0: 7226 0000 0072 2700 0000 7214 0000 0090  r&...r'...r.....
-000010c0: 0000 0073 0200 0000 0002 7a14 4261 7243  ...s......z.BarC
-000010d0: 6861 7274 526f 642e 6772 6164 6965 6e74  hartRod.gradient
-000010e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000010f0: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00001100: 7c00 5f00 6400 5300 7234 0000 0072 4600  |._.d.S.r4...rF.
-00001110: 0000 7237 0000 0072 2600 0000 7226 0000  ..r7...r&...r&..
-00001120: 0072 2700 0000 7214 0000 0094 0000 0073  .r'...r........s
-00001130: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00001140: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00001150: 0e00 0000 7c00 6a00 6401 6402 6403 8d02  ....|.j.d.d.d...
-00001160: 5300 2904 4eda 0762 6746 726f 6d59 723b  S.).N..bgFromYr;
-00001170: 0000 0072 3c00 0000 723e 0000 0072 2800  ...r<...r>...r(.
-00001180: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
-00001190: 0072 1700 0000 9900 0000 7302 0000 0000  .r........s.....
-000011a0: 027a 1542 6172 4368 6172 7452 6f64 2e62  .z.BarChartRod.b
-000011b0: 675f 6672 6f6d 5f79 6302 0000 0000 0000  g_from_yc.......
-000011c0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000011d0: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
-000011e0: 0100 6400 5300 2902 4e72 4700 0000 7240  ..d.S.).NrG...r@
-000011f0: 0000 0072 3700 0000 7226 0000 0072 2600  ...r7...r&...r&.
-00001200: 0000 7227 0000 0072 1700 0000 9d00 0000  ..r'...r........
-00001210: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00001220: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00001230: 730e 0000 007c 006a 0064 0164 0264 038d  s....|.j.d.d.d..
-00001240: 0253 0029 044e da05 6267 546f 5972 3b00  .S.).N..bgToYr;.
-00001250: 0000 723c 0000 0072 3e00 0000 7228 0000  ..r<...r>...r(..
-00001260: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
-00001270: 7218 0000 00a2 0000 0073 0200 0000 0002  r........s......
-00001280: 7a13 4261 7243 6861 7274 526f 642e 6267  z.BarChartRod.bg
-00001290: 5f74 6f5f 7963 0200 0000 0000 0000 0000  _to_yc..........
-000012a0: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
-000012b0: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
-000012c0: 0053 0029 024e 7248 0000 0072 4000 0000  .S.).NrH...r@...
-000012d0: 7237 0000 0072 2600 0000 7226 0000 0072  r7...r&...r&...r
-000012e0: 2700 0000 7218 0000 00a6 0000 0073 0200  '...r........s..
-000012f0: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00001300: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-00001310: 0000 7c00 a000 6401 a101 5300 a902 4eda  ..|...d...S...N.
-00001320: 0762 6743 6f6c 6f72 723e 0000 0072 2800  .bgColorr>...r(.
-00001330: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
-00001340: 0072 1900 0000 ab00 0000 7302 0000 0000  .r........s.....
-00001350: 027a 1442 6172 4368 6172 7452 6f64 2e62  .z.BarChartRod.b
-00001360: 675f 636f 6c6f 7263 0200 0000 0000 0000  g_colorc........
-00001370: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001380: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00001390: 0064 0053 0072 4900 0000 7240 0000 0072  .d.S.rI...r@...r
-000013a0: 3700 0000 7226 0000 0072 2600 0000 7227  7...r&...r&...r'
-000013b0: 0000 0072 1900 0000 af00 0000 7302 0000  ...r........s...
-000013c0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-000013d0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
-000013e0: 007c 006a 0053 0072 3400 0000 a901 7231  .|.j.S.r4.....r1
-000013f0: 0000 0072 2800 0000 7226 0000 0072 2600  ...r(...r&...r&.
-00001400: 0000 7227 0000 0072 1a00 0000 b400 0000  ..r'...r........
-00001410: 7302 0000 0000 027a 1742 6172 4368 6172  s......z.BarChar
-00001420: 7452 6f64 2e62 675f 6772 6164 6965 6e74  tRod.bg_gradient
-00001430: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001440: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00001450: 7c00 5f00 6400 5300 7234 0000 0072 4b00  |._.d.S.r4...rK.
-00001460: 0000 7237 0000 0072 2600 0000 7226 0000  ..r7...r&...r&..
-00001470: 0072 2700 0000 721a 0000 00b8 0000 0073  .r'...r........s
-00001480: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00001490: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-000014a0: 1000 0000 7c00 6a00 6401 6402 6403 6404  ....|.j.d.d.d.d.
-000014b0: 8d03 5300 2905 4e72 1b00 0000 da04 626f  ..S.).Nr......bo
-000014c0: 6f6c 46a9 0272 3d00 0000 da09 6465 665f  olF..r=.....def_
-000014d0: 7661 6c75 6572 3e00 0000 7228 0000 0072  valuer>...r(...r
-000014e0: 2600 0000 7226 0000 0072 2700 0000 721b  &...r&...r'...r.
-000014f0: 0000 00bd 0000 0073 0200 0000 0002 7a14  .......s......z.
-00001500: 4261 7243 6861 7274 526f 642e 7365 6c65  BarChartRod.sele
-00001510: 6374 6564 6302 0000 0000 0000 0000 0000  ctedc...........
-00001520: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00001530: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
-00001540: 5300 2902 4e72 1b00 0000 7240 0000 0072  S.).Nr....r@...r
-00001550: 3700 0000 7226 0000 0072 2600 0000 7227  7...r&...r&...r'
-00001560: 0000 0072 1b00 0000 c100 0000 7302 0000  ...r........s...
-00001570: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-00001580: 0100 0000 0500 0000 4300 0000 7310 0000  ........C...s...
-00001590: 007c 006a 0064 0164 0264 0364 048d 0353  .|.j.d.d.d.d...S
-000015a0: 0029 054e da0b 7368 6f77 546f 6f6c 7469  .).N..showToolti
-000015b0: 7072 4c00 0000 5472 4d00 0000 723e 0000  prL...TrM...r>..
-000015c0: 0072 2800 0000 7226 0000 0072 2600 0000  .r(...r&...r&...
-000015d0: 7227 0000 0072 1c00 0000 c600 0000 7302  r'...r........s.
-000015e0: 0000 0000 027a 1842 6172 4368 6172 7452  .....z.BarChartR
-000015f0: 6f64 2e73 686f 775f 746f 6f6c 7469 7063  od.show_tooltipc
-00001600: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001610: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
-00001620: 0064 017c 01a1 0201 0064 0053 0029 024e  .d.|.....d.S.).N
-00001630: 724f 0000 0072 4000 0000 7237 0000 0072  rO...r@...r7...r
-00001640: 2600 0000 7226 0000 0072 2700 0000 721c  &...r&...r'...r.
-00001650: 0000 00ca 0000 0073 0200 0000 0002 6301  .......s......c.
-00001660: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001670: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
-00001680: 6401 a101 5300 a902 4e72 1d00 0000 723e  d...S...Nr....r>
-00001690: 0000 0072 2800 0000 7226 0000 0072 2600  ...r(...r&...r&.
-000016a0: 0000 7227 0000 0072 1d00 0000 cf00 0000  ..r'...r........
-000016b0: 7302 0000 0000 027a 1342 6172 4368 6172  s......z.BarChar
-000016c0: 7452 6f64 2e74 6f6f 6c74 6970 6302 0000  tRod.tooltipc...
-000016d0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000016e0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-000016f0: 7c01 a102 0100 6400 5300 7250 0000 0072  |.....d.S.rP...r
-00001700: 4000 0000 7237 0000 0072 2600 0000 7226  @...r7...r&...r&
-00001710: 0000 0072 2700 0000 721d 0000 00d3 0000  ...r'...r.......
-00001720: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00001730: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00001740: 0073 0600 0000 7c00 6a00 5300 7234 0000  .s....|.j.S.r4..
-00001750: 0029 01da 1b5f 4261 7243 6861 7274 526f  .)..._BarChartRo
-00001760: 645f 5f74 6f6f 6c74 6970 5f61 6c69 676e  d__tooltip_align
-00001770: 7228 0000 0072 2600 0000 7226 0000 0072  r(...r&...r&...r
-00001780: 2700 0000 721f 0000 00d8 0000 0073 0200  '...r........s..
-00001790: 0000 0002 7a19 4261 7243 6861 7274 526f  ....z.BarChartRo
-000017a0: 642e 746f 6f6c 7469 705f 616c 6967 6e63  d.tooltip_alignc
-000017b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000017c0: 0600 0000 4300 0000 7326 0000 007c 017c  ....C...s&...|.|
-000017d0: 005f 007c 00a0 0164 0174 027c 0174 0383  ._.|...d.t.|.t..
-000017e0: 0272 1c7c 016a 046e 027c 01a1 0201 0064  .r.|.j.n.|.....d
-000017f0: 0053 0029 024e 5a0c 746f 6f6c 7469 7041  .S.).NZ.tooltipA
-00001800: 6c69 676e 2905 7251 0000 0072 4100 0000  lign).rQ...rA...
-00001810: da0a 6973 696e 7374 616e 6365 720d 0000  ..isinstancer...
-00001820: 0072 3800 0000 7237 0000 0072 2600 0000  .r8...r7...r&...
-00001830: 7226 0000 0072 2700 0000 721f 0000 00dc  r&...r'...r.....
-00001840: 0000 0073 0800 0000 0002 0601 0401 14ff  ...s............
-00001850: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001860: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00001870: 6a00 5300 7234 0000 00a9 015a 1b5f 4261  j.S.r4.....Z._Ba
-00001880: 7243 6861 7274 526f 645f 5f74 6f6f 6c74  rChartRod__toolt
-00001890: 6970 5f73 7479 6c65 7228 0000 0072 2600  ip_styler(...r&.
-000018a0: 0000 7226 0000 0072 2700 0000 721e 0000  ..r&...r'...r...
-000018b0: 00e4 0000 0073 0200 0000 0002 7a19 4261  .....s......z.Ba
-000018c0: 7243 6861 7274 526f 642e 746f 6f6c 7469  rChartRod.toolti
-000018d0: 705f 7374 796c 6563 0200 0000 0000 0000  p_stylec........
-000018e0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-000018f0: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
-00001900: 3400 0000 7253 0000 0072 3700 0000 7226  4...rS...r7...r&
-00001910: 0000 0072 2600 0000 7227 0000 0072 1e00  ...r&...r'...r..
-00001920: 0000 e800 0000 7302 0000 0000 0229 154e  ......s......).N
-00001930: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
-00001940: 4e4e 4e4e 2928 da08 5f5f 6e61 6d65 5f5f  NNNN)(..__name__
-00001950: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00001960: 7175 616c 6e61 6d65 5f5f 7204 0000 0072  qualname__r....r
-00001970: 0300 0000 7206 0000 0072 0800 0000 da03  ....r....r......
-00001980: 7374 7272 0900 0000 720c 0000 0072 0500  strr....r....r..
-00001990: 0000 724c 0000 0072 0b00 0000 720d 0000  ..rL...r....r...
-000019a0: 0072 0a00 0000 7202 0000 0072 2400 0000  .r....r....r$...
-000019b0: 7229 0000 0072 2c00 0000 7236 0000 00da  r)...r,...r6....
-000019c0: 0870 726f 7065 7274 7972 0f00 0000 da06  .propertyr......
-000019d0: 7365 7474 6572 7210 0000 0072 1100 0000  setterr....r....
-000019e0: 7212 0000 0072 1300 0000 7216 0000 0072  r....r....r....r
-000019f0: 1500 0000 7214 0000 0072 1700 0000 7218  ....r....r....r.
-00001a00: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00001a10: 0000 721c 0000 0072 1d00 0000 721f 0000  ..r....r....r...
-00001a20: 0072 1e00 0000 da0d 5f5f 636c 6173 7363  .r......__classc
-00001a30: 656c 6c5f 5f72 2600 0000 7226 0000 0072  ell__r&...r&...r
-00001a40: 3200 0000 7227 0000 0072 0e00 0000 0c00  2...r'...r......
-00001a50: 0000 73e6 0000 0008 0300 0100 0100 0100  ..s.............
-00001a60: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-00001a70: 0100 0100 0100 0100 0100 0400 0100 0100  ................
-00001a80: 0100 e702 020a 0102 0102 0102 0106 0106  ................
-00001a90: 0102 0106 0102 0102 0106 0106 0106 0106  ................
-00001aa0: 0106 0106 0106 0406 0106 0106 0102 e70c  ................
-00001ab0: 3608 030c 0708 0402 010a 0304 010a 0402  6...............
-00001ac0: 0110 0304 0110 0402 0110 0304 0110 0402  ................
-00001ad0: 0110 0304 0110 0402 0114 0304 0114 0402  ................
-00001ae0: 0114 0304 0114 0402 0114 0304 0114 0402  ................
-00001af0: 0114 0304 0114 0402 0110 0304 0110 0402  ................
-00001b00: 0110 0304 0110 0402 0114 0304 0114 0402  ................
-00001b10: 0114 0304 0114 0402 0114 0304 0114 0402  ................
-00001b20: 0114 0304 0114 0402 0114 0304 0114 0402  ................
-00001b30: 0114 0304 0114 0702 010a 0304 0172 0e00  .............r..
-00001b40: 0000 4e29 15da 0674 7970 696e 6772 0200  ..N)...typingr..
-00001b50: 0000 7203 0000 0072 0400 0000 da10 666c  ..r....r......fl
-00001b60: 6574 5f63 6f72 652e 626f 7264 6572 7205  et_core.borderr.
-00001b70: 0000 00da 2966 6c65 745f 636f 7265 2e63  ....)flet_core.c
-00001b80: 6861 7274 732e 6261 725f 6368 6172 745f  harts.bar_chart_
-00001b90: 726f 645f 7374 6163 6b5f 6974 656d 7206  rod_stack_itemr.
-00001ba0: 0000 00da 1166 6c65 745f 636f 7265 2e63  .....flet_core.c
-00001bb0: 6f6e 7472 6f6c 7207 0000 0072 0800 0000  ontrolr....r....
-00001bc0: da13 666c 6574 5f63 6f72 652e 6772 6164  ..flet_core.grad
-00001bd0: 6965 6e74 7372 0900 0000 da0d 666c 6574  ientsr......flet
-00001be0: 5f63 6f72 652e 7265 6672 0a00 0000 da14  _core.refr......
-00001bf0: 666c 6574 5f63 6f72 652e 7465 7874 5f73  flet_core.text_s
-00001c00: 7479 6c65 720b 0000 00da 0f66 6c65 745f  tyler......flet_
-00001c10: 636f 7265 2e74 7970 6573 720c 0000 0072  core.typesr....r
-00001c20: 0d00 0000 720e 0000 0072 2600 0000 7226  ....r....r&...r&
-00001c30: 0000 0072 2600 0000 7227 0000 00da 083c  ...r&...r'.....<
-00001c40: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00001c50: 1402 0c01 0c01 1001 0c01 0c01 0c01 1003  ................
+00000770: 2f66 6c65 7463 6f6e 7472 6962 2f73 646b  /fletcontrib/sdk
+00000780: 2f70 7974 686f 6e2f 7061 636b 6167 6573  /python/packages
+00000790: 2f66 6c65 742d 636f 7265 2f73 7263 2f66  /flet-core/src/f
+000007a0: 6c65 745f 636f 7265 2f63 6861 7274 732f  let_core/charts/
+000007b0: 6261 725f 6368 6172 745f 726f 642e 7079  bar_chart_rod.py
+000007c0: 7224 0000 000d 0000 0073 3000 0000 001c  r$.......s0.....
+000007d0: 0401 0201 0201 0201 0201 02fb 0608 0601  ................
+000007e0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000007f0: 0601 0601 0601 0601 0601 0601 0601 7a14  ..............z.
+00000800: 4261 7243 6861 7274 526f 642e 5f5f 696e  BarChartRod.__in
+00000810: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00000820: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+00000830: 0000 6401 5300 2902 4e5a 0372 6f64 7226  ..d.S.).NZ.rodr&
+00000840: 0000 00a9 0172 2500 0000 7226 0000 0072  .....r%...r&...r
+00000850: 2600 0000 7227 0000 00da 115f 6765 745f  &...r'....._get_
+00000860: 636f 6e74 726f 6c5f 6e61 6d65 4300 0000  control_nameC...
+00000870: 7302 0000 0000 017a 1d42 6172 4368 6172  s......z.BarChar
+00000880: 7452 6f64 2e5f 6765 745f 636f 6e74 726f  tRod._get_contro
+00000890: 6c5f 6e61 6d65 6301 0000 0000 0000 0000  l_namec.........
+000008a0: 0000 0001 0000 0004 0000 0003 0000 0073  ...............s
+000008b0: 4600 0000 7400 8300 a001 a100 0100 7c00  F...t.........|.
+000008c0: a002 6401 7c00 6a03 a102 0100 7c00 a002  ..d.|.j.....|...
+000008d0: 6402 7c00 6a04 a102 0100 7c00 a002 6403  d.|.j.....|...d.
+000008e0: 7c00 6a05 a102 0100 7c00 a002 6404 7c00  |.j.....|...d.|.
+000008f0: 6a06 a102 0100 6400 5300 2905 4e72 1400  j.....d.S.).Nr..
+00000900: 0000 5a0a 626f 7264 6572 5369 6465 da0c  ..Z.borderSide..
+00000910: 626f 7264 6572 5261 6469 7573 5a0a 6267  borderRadiusZ.bg
+00000920: 4772 6164 6965 6e74 2907 da05 7375 7065  Gradient)...supe
+00000930: 72da 0d62 6566 6f72 655f 7570 6461 7465  r..before_update
+00000940: da0e 5f73 6574 5f61 7474 725f 6a73 6f6e  .._set_attr_json
+00000950: da16 5f42 6172 4368 6172 7452 6f64 5f5f  .._BarChartRod__
+00000960: 6772 6164 6965 6e74 da19 5f42 6172 4368  gradient.._BarCh
+00000970: 6172 7452 6f64 5f5f 626f 7264 6572 5f73  artRod__border_s
+00000980: 6964 65da 1b5f 4261 7243 6861 7274 526f  ide.._BarChartRo
+00000990: 645f 5f62 6f72 6465 725f 7261 6469 7573  d__border_radius
+000009a0: da19 5f42 6172 4368 6172 7452 6f64 5f5f  .._BarChartRod__
+000009b0: 6267 5f67 7261 6469 656e 7472 2800 0000  bg_gradientr(...
+000009c0: a901 da09 5f5f 636c 6173 735f 5f72 2600  ....__class__r&.
+000009d0: 0000 7227 0000 0072 2c00 0000 4600 0000  ..r'...r,...F...
+000009e0: 730a 0000 0000 010a 010e 010e 010e 017a  s..............z
+000009f0: 1942 6172 4368 6172 7452 6f64 2e62 6566  .BarChartRod.bef
+00000a00: 6f72 655f 7570 6461 7465 6301 0000 0000  ore_updatec.....
+00000a10: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000a20: 0000 0073 0600 0000 7c00 6a00 5300 a901  ...s....|.j.S...
+00000a30: 4ea9 015a 1d5f 4261 7243 6861 7274 526f  N..Z._BarChartRo
+00000a40: 645f 5f72 6f64 5f73 7461 636b 5f69 7465  d__rod_stack_ite
+00000a50: 6d73 7228 0000 0072 2600 0000 7226 0000  msr(...r&...r&..
+00000a60: 0072 2700 0000 da0d 5f67 6574 5f63 6869  .r'....._get_chi
+00000a70: 6c64 7265 6e4d 0000 0073 0200 0000 0001  ldrenM...s......
+00000a80: 7a19 4261 7243 6861 7274 526f 642e 5f67  z.BarChartRod._g
+00000a90: 6574 5f63 6869 6c64 7265 6e63 0100 0000  et_childrenc....
+00000aa0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000ab0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
+00000ac0: 3400 0000 7235 0000 0072 2800 0000 7226  4...r5...r(...r&
+00000ad0: 0000 0072 2600 0000 7227 0000 0072 0f00  ...r&...r'...r..
+00000ae0: 0000 5100 0000 7302 0000 0000 027a 1b42  ..Q...s......z.B
+00000af0: 6172 4368 6172 7452 6f64 2e72 6f64 5f73  arChartRod.rod_s
+00000b00: 7461 636b 5f69 7465 6d73 6302 0000 0000  tack_itemsc.....
+00000b10: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00000b20: 0000 0073 1600 0000 7c01 6400 7501 720c  ...s....|.d.u.r.
+00000b30: 7c01 6e02 6700 7c00 5f00 6400 5300 7234  |.n.g.|._.d.S.r4
+00000b40: 0000 0072 3500 0000 a902 7225 0000 00da  ...r5.....r%....
+00000b50: 0576 616c 7565 7226 0000 0072 2600 0000  .valuer&...r&...
+00000b60: 7227 0000 0072 0f00 0000 5500 0000 7302  r'...r....U...s.
+00000b70: 0000 0000 0229 01da 0672 6574 7572 6e63  .....)...returnc
+00000b80: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000b90: 0400 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+00000ba0: 0064 0164 0264 038d 0253 0029 044e da05  .d.d.d...S.).N..
+00000bb0: 6672 6f6d 59da 0566 6c6f 6174 a901 da09  fromY..float....
+00000bc0: 6461 7461 5f74 7970 65a9 01da 095f 6765  data_type...._ge
+00000bd0: 745f 6174 7472 7228 0000 0072 2600 0000  t_attrr(...r&...
+00000be0: 7226 0000 0072 2700 0000 7210 0000 005a  r&...r'...r....Z
+00000bf0: 0000 0073 0200 0000 0002 7a12 4261 7243  ...s......z.BarC
+00000c00: 6861 7274 526f 642e 6672 6f6d 5f79 2901  hartRod.from_y).
+00000c10: 7238 0000 0063 0200 0000 0000 0000 0000  r8...c..........
+00000c20: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+00000c30: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+00000c40: 0053 0029 024e 723a 0000 00a9 01da 095f  .S.).Nr:......._
+00000c50: 7365 745f 6174 7472 7237 0000 0072 2600  set_attrr7...r&.
+00000c60: 0000 7226 0000 0072 2700 0000 7210 0000  ..r&...r'...r...
+00000c70: 005e 0000 0073 0200 0000 0002 6301 0000  .^...s......c...
+00000c80: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000c90: 0043 0000 0073 0e00 0000 7c00 6a00 6401  .C...s....|.j.d.
+00000ca0: 6402 6403 8d02 5300 2904 4eda 0374 6f59  d.d...S.).N..toY
+00000cb0: 723b 0000 0072 3c00 0000 723e 0000 0072  r;...r<...r>...r
+00000cc0: 2800 0000 7226 0000 0072 2600 0000 7227  (...r&...r&...r'
+00000cd0: 0000 0072 1100 0000 6300 0000 7302 0000  ...r....c...s...
+00000ce0: 0000 027a 1042 6172 4368 6172 7452 6f64  ...z.BarChartRod
+00000cf0: 2e74 6f5f 7963 0200 0000 0000 0000 0000  .to_yc..........
+00000d00: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+00000d10: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+00000d20: 0053 0029 024e 7242 0000 0072 4000 0000  .S.).NrB...r@...
+00000d30: 7237 0000 0072 2600 0000 7226 0000 0072  r7...r&...r&...r
+00000d40: 2700 0000 7211 0000 0067 0000 0073 0200  '...r....g...s..
+00000d50: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
+00000d60: 0001 0000 0004 0000 0043 0000 0073 0e00  .........C...s..
+00000d70: 0000 7c00 6a00 6401 6402 6403 8d02 5300  ..|.j.d.d.d...S.
+00000d80: 2904 4e72 1200 0000 723b 0000 0072 3c00  ).Nr....r;...r<.
+00000d90: 0000 723e 0000 0072 2800 0000 7226 0000  ..r>...r(...r&..
+00000da0: 0072 2600 0000 7227 0000 0072 1200 0000  .r&...r'...r....
+00000db0: 6c00 0000 7302 0000 0000 027a 1142 6172  l...s......z.Bar
+00000dc0: 4368 6172 7452 6f64 2e77 6964 7468 6302  ChartRod.widthc.
+00000dd0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000de0: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00000df0: 6401 7c01 a102 0100 6400 5300 2902 4e72  d.|.....d.S.).Nr
+00000e00: 1200 0000 7240 0000 0072 3700 0000 7226  ....r@...r7...r&
+00000e10: 0000 0072 2600 0000 7227 0000 0072 1200  ...r&...r'...r..
+00000e20: 0000 7000 0000 7302 0000 0000 0263 0100  ..p...s......c..
+00000e30: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000e40: 0000 4300 0000 730a 0000 007c 00a0 0064  ..C...s....|...d
+00000e50: 01a1 0153 00a9 024e 7213 0000 0072 3e00  ...S...Nr....r>.
+00000e60: 0000 7228 0000 0072 2600 0000 7226 0000  ..r(...r&...r&..
+00000e70: 0072 2700 0000 7213 0000 0075 0000 0073  .r'...r....u...s
+00000e80: 0200 0000 0002 7a11 4261 7243 6861 7274  ......z.BarChart
+00000e90: 526f 642e 636f 6c6f 7263 0200 0000 0000  Rod.colorc......
+00000ea0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00000eb0: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
+00000ec0: 0201 0064 0053 0072 4300 0000 7240 0000  ...d.S.rC...r@..
+00000ed0: 0072 3700 0000 7226 0000 0072 2600 0000  .r7...r&...r&...
+00000ee0: 7227 0000 0072 1300 0000 7900 0000 7302  r'...r....y...s.
+00000ef0: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00000f00: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00000f10: 0000 007c 006a 0053 0072 3400 0000 a901  ...|.j.S.r4.....
+00000f20: 722f 0000 0072 2800 0000 7226 0000 0072  r/...r(...r&...r
+00000f30: 2600 0000 7227 0000 0072 1600 0000 7e00  &...r'...r....~.
+00000f40: 0000 7302 0000 0000 027a 1742 6172 4368  ..s......z.BarCh
+00000f50: 6172 7452 6f64 2e62 6f72 6465 725f 7369  artRod.border_si
+00000f60: 6465 6302 0000 0000 0000 0000 0000 0002  dec.............
+00000f70: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000f80: 7c01 7c00 5f00 6400 5300 7234 0000 0072  |.|._.d.S.r4...r
+00000f90: 4400 0000 7237 0000 0072 2600 0000 7226  D...r7...r&...r&
+00000fa0: 0000 0072 2700 0000 7216 0000 0082 0000  ...r'...r.......
+00000fb0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
+00000fc0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000fd0: 0073 0600 0000 7c00 6a00 5300 7234 0000  .s....|.j.S.r4..
+00000fe0: 00a9 0172 3000 0000 7228 0000 0072 2600  ...r0...r(...r&.
+00000ff0: 0000 7226 0000 0072 2700 0000 7215 0000  ..r&...r'...r...
+00001000: 0087 0000 0073 0200 0000 0002 7a19 4261  .....s......z.Ba
+00001010: 7243 6861 7274 526f 642e 626f 7264 6572  rChartRod.border
+00001020: 5f72 6164 6975 7363 0200 0000 0000 0000  _radiusc........
+00001030: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00001040: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
+00001050: 3400 0000 7245 0000 0072 3700 0000 7226  4...rE...r7...r&
+00001060: 0000 0072 2600 0000 7227 0000 0072 1500  ...r&...r'...r..
+00001070: 0000 8b00 0000 7302 0000 0000 0263 0100  ......s......c..
+00001080: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00001090: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+000010a0: 0072 3400 0000 a901 722e 0000 0072 2800  .r4.....r....r(.
+000010b0: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
+000010c0: 0072 1400 0000 9000 0000 7302 0000 0000  .r........s.....
+000010d0: 027a 1442 6172 4368 6172 7452 6f64 2e67  .z.BarChartRod.g
+000010e0: 7261 6469 656e 7463 0200 0000 0000 0000  radientc........
+000010f0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00001100: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
+00001110: 3400 0000 7246 0000 0072 3700 0000 7226  4...rF...r7...r&
+00001120: 0000 0072 2600 0000 7227 0000 0072 1400  ...r&...r'...r..
+00001130: 0000 9400 0000 7302 0000 0000 0263 0100  ......s......c..
+00001140: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00001150: 0000 4300 0000 730e 0000 007c 006a 0064  ..C...s....|.j.d
+00001160: 0164 0264 038d 0253 0029 044e da07 6267  .d.d...S.).N..bg
+00001170: 4672 6f6d 5972 3b00 0000 723c 0000 0072  FromYr;...r<...r
+00001180: 3e00 0000 7228 0000 0072 2600 0000 7226  >...r(...r&...r&
+00001190: 0000 0072 2700 0000 7217 0000 0099 0000  ...r'...r.......
+000011a0: 0073 0200 0000 0002 7a15 4261 7243 6861  .s......z.BarCha
+000011b0: 7274 526f 642e 6267 5f66 726f 6d5f 7963  rtRod.bg_from_yc
+000011c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000011d0: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+000011e0: 0064 017c 01a1 0201 0064 0053 0029 024e  .d.|.....d.S.).N
+000011f0: 7247 0000 0072 4000 0000 7237 0000 0072  rG...r@...r7...r
+00001200: 2600 0000 7226 0000 0072 2700 0000 7217  &...r&...r'...r.
+00001210: 0000 009d 0000 0073 0200 0000 0002 6301  .......s......c.
+00001220: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00001230: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
+00001240: 6401 6402 6403 8d02 5300 2904 4eda 0562  d.d.d...S.).N..b
+00001250: 6754 6f59 723b 0000 0072 3c00 0000 723e  gToYr;...r<...r>
+00001260: 0000 0072 2800 0000 7226 0000 0072 2600  ...r(...r&...r&.
+00001270: 0000 7227 0000 0072 1800 0000 a200 0000  ..r'...r........
+00001280: 7302 0000 0000 027a 1342 6172 4368 6172  s......z.BarChar
+00001290: 7452 6f64 2e62 675f 746f 5f79 6302 0000  tRod.bg_to_yc...
+000012a0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000012b0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
+000012c0: 7c01 a102 0100 6400 5300 2902 4e72 4800  |.....d.S.).NrH.
+000012d0: 0000 7240 0000 0072 3700 0000 7226 0000  ..r@...r7...r&..
+000012e0: 0072 2600 0000 7227 0000 0072 1800 0000  .r&...r'...r....
+000012f0: a600 0000 7302 0000 0000 0263 0100 0000  ....s......c....
+00001300: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001310: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
+00001320: 0153 00a9 024e da07 6267 436f 6c6f 7272  .S...N..bgColorr
+00001330: 3e00 0000 7228 0000 0072 2600 0000 7226  >...r(...r&...r&
+00001340: 0000 0072 2700 0000 7219 0000 00ab 0000  ...r'...r.......
+00001350: 0073 0200 0000 0002 7a14 4261 7243 6861  .s......z.BarCha
+00001360: 7274 526f 642e 6267 5f63 6f6c 6f72 6302  rtRod.bg_colorc.
+00001370: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001380: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00001390: 6401 7c01 a102 0100 6400 5300 7249 0000  d.|.....d.S.rI..
+000013a0: 0072 4000 0000 7237 0000 0072 2600 0000  .r@...r7...r&...
+000013b0: 7226 0000 0072 2700 0000 7219 0000 00af  r&...r'...r.....
+000013c0: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+000013d0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+000013e0: 0000 0073 0600 0000 7c00 6a00 5300 7234  ...s....|.j.S.r4
+000013f0: 0000 00a9 0172 3100 0000 7228 0000 0072  .....r1...r(...r
+00001400: 2600 0000 7226 0000 0072 2700 0000 721a  &...r&...r'...r.
+00001410: 0000 00b4 0000 0073 0200 0000 0002 7a17  .......s......z.
+00001420: 4261 7243 6861 7274 526f 642e 6267 5f67  BarChartRod.bg_g
+00001430: 7261 6469 656e 7463 0200 0000 0000 0000  radientc........
+00001440: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00001450: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
+00001460: 3400 0000 724b 0000 0072 3700 0000 7226  4...rK...r7...r&
+00001470: 0000 0072 2600 0000 7227 0000 0072 1a00  ...r&...r'...r..
+00001480: 0000 b800 0000 7302 0000 0000 0263 0100  ......s......c..
+00001490: 0000 0000 0000 0000 0000 0100 0000 0500  ................
+000014a0: 0000 4300 0000 7310 0000 007c 006a 0064  ..C...s....|.j.d
+000014b0: 0164 0264 0364 048d 0353 0029 054e 721b  .d.d.d...S.).Nr.
+000014c0: 0000 00da 0462 6f6f 6c46 a902 723d 0000  .....boolF..r=..
+000014d0: 00da 0964 6566 5f76 616c 7565 723e 0000  ...def_valuer>..
+000014e0: 0072 2800 0000 7226 0000 0072 2600 0000  .r(...r&...r&...
+000014f0: 7227 0000 0072 1b00 0000 bd00 0000 7302  r'...r........s.
+00001500: 0000 0000 027a 1442 6172 4368 6172 7452  .....z.BarChartR
+00001510: 6f64 2e73 656c 6563 7465 6463 0200 0000  od.selectedc....
+00001520: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001530: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
+00001540: 01a1 0201 0064 0053 0029 024e 721b 0000  .....d.S.).Nr...
+00001550: 0072 4000 0000 7237 0000 0072 2600 0000  .r@...r7...r&...
+00001560: 7226 0000 0072 2700 0000 721b 0000 00c1  r&...r'...r.....
+00001570: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+00001580: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+00001590: 0000 0073 1000 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
+000015a0: 6403 6404 8d03 5300 2905 4eda 0b73 686f  d.d...S.).N..sho
+000015b0: 7754 6f6f 6c74 6970 724c 0000 0054 724d  wTooltiprL...TrM
+000015c0: 0000 0072 3e00 0000 7228 0000 0072 2600  ...r>...r(...r&.
+000015d0: 0000 7226 0000 0072 2700 0000 721c 0000  ..r&...r'...r...
+000015e0: 00c6 0000 0073 0200 0000 0002 7a18 4261  .....s......z.Ba
+000015f0: 7243 6861 7274 526f 642e 7368 6f77 5f74  rChartRod.show_t
+00001600: 6f6f 6c74 6970 6302 0000 0000 0000 0000  ooltipc.........
+00001610: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00001620: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
+00001630: 6400 5300 2902 4e72 4f00 0000 7240 0000  d.S.).NrO...r@..
+00001640: 0072 3700 0000 7226 0000 0072 2600 0000  .r7...r&...r&...
+00001650: 7227 0000 0072 1c00 0000 ca00 0000 7302  r'...r........s.
+00001660: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00001670: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
+00001680: 0000 007c 00a0 0064 01a1 0153 00a9 024e  ...|...d...S...N
+00001690: 721d 0000 0072 3e00 0000 7228 0000 0072  r....r>...r(...r
+000016a0: 2600 0000 7226 0000 0072 2700 0000 721d  &...r&...r'...r.
+000016b0: 0000 00cf 0000 0073 0200 0000 0002 7a13  .......s......z.
+000016c0: 4261 7243 6861 7274 526f 642e 746f 6f6c  BarChartRod.tool
+000016d0: 7469 7063 0200 0000 0000 0000 0000 0000  tipc............
+000016e0: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+000016f0: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+00001700: 0072 5000 0000 7240 0000 0072 3700 0000  .rP...r@...r7...
+00001710: 7226 0000 0072 2600 0000 7227 0000 0072  r&...r&...r'...r
+00001720: 1d00 0000 d300 0000 7302 0000 0000 0263  ........s......c
+00001730: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001740: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+00001750: 0053 0072 3400 0000 2901 da1b 5f42 6172  .S.r4...)..._Bar
+00001760: 4368 6172 7452 6f64 5f5f 746f 6f6c 7469  ChartRod__toolti
+00001770: 705f 616c 6967 6e72 2800 0000 7226 0000  p_alignr(...r&..
+00001780: 0072 2600 0000 7227 0000 0072 1f00 0000  .r&...r'...r....
+00001790: d800 0000 7302 0000 0000 027a 1942 6172  ....s......z.Bar
+000017a0: 4368 6172 7452 6f64 2e74 6f6f 6c74 6970  ChartRod.tooltip
+000017b0: 5f61 6c69 676e 6302 0000 0000 0000 0000  _alignc.........
+000017c0: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
+000017d0: 2600 0000 7c01 7c00 5f00 7c00 a001 6401  &...|.|._.|...d.
+000017e0: 7402 7c01 7403 8302 721c 7c01 6a04 6e02  t.|.t...r.|.j.n.
+000017f0: 7c01 a102 0100 6400 5300 2902 4e5a 0c74  |.....d.S.).NZ.t
+00001800: 6f6f 6c74 6970 416c 6967 6e29 0572 5100  ooltipAlign).rQ.
+00001810: 0000 7241 0000 00da 0a69 7369 6e73 7461  ..rA.....isinsta
+00001820: 6e63 6572 0d00 0000 7238 0000 0072 3700  ncer....r8...r7.
+00001830: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
+00001840: 0072 1f00 0000 dc00 0000 7308 0000 0000  .r........s.....
+00001850: 0206 0104 0114 ff63 0100 0000 0000 0000  .......c........
+00001860: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00001870: 7306 0000 007c 006a 0053 0072 3400 0000  s....|.j.S.r4...
+00001880: a901 5a1b 5f42 6172 4368 6172 7452 6f64  ..Z._BarChartRod
+00001890: 5f5f 746f 6f6c 7469 705f 7374 796c 6572  __tooltip_styler
+000018a0: 2800 0000 7226 0000 0072 2600 0000 7227  (...r&...r&...r'
+000018b0: 0000 0072 1e00 0000 e400 0000 7302 0000  ...r........s...
+000018c0: 0000 027a 1942 6172 4368 6172 7452 6f64  ...z.BarChartRod
+000018d0: 2e74 6f6f 6c74 6970 5f73 7479 6c65 6302  .tooltip_stylec.
+000018e0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+000018f0: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
+00001900: 5f00 6400 5300 7234 0000 0072 5300 0000  _.d.S.r4...rS...
+00001910: 7237 0000 0072 2600 0000 7226 0000 0072  r7...r&...r&...r
+00001920: 2700 0000 721e 0000 00e8 0000 0073 0200  '...r........s..
+00001930: 0000 0002 2915 4e4e 4e4e 4e4e 4e4e 4e4e  ....).NNNNNNNNNN
+00001940: 4e4e 4e4e 4e4e 4e4e 4e4e 4e29 28da 085f  NNNNNNNNNNN)(.._
+00001950: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00001960: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00001970: 5f72 0400 0000 7203 0000 0072 0600 0000  _r....r....r....
+00001980: 7208 0000 00da 0373 7472 7209 0000 0072  r......strr....r
+00001990: 0c00 0000 7205 0000 0072 4c00 0000 720b  ....r....rL...r.
+000019a0: 0000 0072 0d00 0000 720a 0000 0072 0200  ...r....r....r..
+000019b0: 0000 7224 0000 0072 2900 0000 722c 0000  ..r$...r)...r,..
+000019c0: 0072 3600 0000 da08 7072 6f70 6572 7479  .r6.....property
+000019d0: 720f 0000 00da 0673 6574 7465 7272 1000  r......setterr..
+000019e0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000019f0: 0072 1600 0000 7215 0000 0072 1400 0000  .r....r....r....
+00001a00: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00001a10: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
+00001a20: 0000 0072 1f00 0000 721e 0000 00da 0d5f  ...r....r......_
+00001a30: 5f63 6c61 7373 6365 6c6c 5f5f 7226 0000  _classcell__r&..
+00001a40: 0072 2600 0000 7232 0000 0072 2700 0000  .r&...r2...r'...
+00001a50: 720e 0000 000c 0000 0073 e600 0000 0803  r........s......
+00001a60: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+00001a70: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+00001a80: 0004 0001 0001 0001 00e7 0202 0a01 0201  ................
+00001a90: 0201 0201 0601 0601 0201 0601 0201 0201  ................
+00001aa0: 0601 0601 0601 0601 0601 0601 0604 0601  ................
+00001ab0: 0601 0601 02e7 0c36 0803 0c07 0804 0201  .......6........
+00001ac0: 0a03 0401 0a04 0201 1003 0401 1004 0201  ................
+00001ad0: 1003 0401 1004 0201 1003 0401 1004 0201  ................
+00001ae0: 1403 0401 1404 0201 1403 0401 1404 0201  ................
+00001af0: 1403 0401 1404 0201 1403 0401 1404 0201  ................
+00001b00: 1003 0401 1004 0201 1003 0401 1004 0201  ................
+00001b10: 1403 0401 1404 0201 1403 0401 1404 0201  ................
+00001b20: 1403 0401 1404 0201 1403 0401 1404 0201  ................
+00001b30: 1403 0401 1404 0201 1403 0401 1407 0201  ................
+00001b40: 0a03 0401 720e 0000 004e 2915 da06 7479  ....r....N)...ty
+00001b50: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
+00001b60: 0000 00da 1066 6c65 745f 636f 7265 2e62  .....flet_core.b
+00001b70: 6f72 6465 7272 0500 0000 da29 666c 6574  orderr.....)flet
+00001b80: 5f63 6f72 652e 6368 6172 7473 2e62 6172  _core.charts.bar
+00001b90: 5f63 6861 7274 5f72 6f64 5f73 7461 636b  _chart_rod_stack
+00001ba0: 5f69 7465 6d72 0600 0000 da11 666c 6574  _itemr......flet
+00001bb0: 5f63 6f72 652e 636f 6e74 726f 6c72 0700  _core.controlr..
+00001bc0: 0000 7208 0000 00da 1366 6c65 745f 636f  ..r......flet_co
+00001bd0: 7265 2e67 7261 6469 656e 7473 7209 0000  re.gradientsr...
+00001be0: 00da 0d66 6c65 745f 636f 7265 2e72 6566  ...flet_core.ref
+00001bf0: 720a 0000 00da 1466 6c65 745f 636f 7265  r......flet_core
+00001c00: 2e74 6578 745f 7374 796c 6572 0b00 0000  .text_styler....
+00001c10: da0f 666c 6574 5f63 6f72 652e 7479 7065  ..flet_core.type
+00001c20: 7372 0c00 0000 720d 0000 0072 0e00 0000  sr....r....r....
+00001c30: 7226 0000 0072 2600 0000 7226 0000 0072  r&...r&...r&...r
+00001c40: 2700 0000 da08 3c6d 6f64 756c 653e 0100  '.....<module>..
+00001c50: 0000 7310 0000 0014 020c 010c 0110 010c  ..s.............
+00001c60: 010c 010c 0110 03                        .......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 8c07 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 8c07 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6506 8303 5a0a 6407 5300 2908 e900 0000  e...Z.d.S.).....
@@ -41,126 +41,126 @@
 00000280: 005f 0564 0053 0029 024e 2904 720d 0000  ._.d.S.).N).r...
 00000290: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
 000002a0: 2906 7205 0000 00da 085f 5f69 6e69 745f  ).r......__init_
 000002b0: 5f72 0900 0000 720a 0000 0072 0b00 0000  _r....r....r....
 000002c0: 720c 0000 0029 09da 0473 656c 6672 0900  r....)...selfr..
 000002d0: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
 000002e0: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000002f0: 7210 0000 00a9 0072 1300 0000 fa6b 2f77  r......r.....k/w
+000002f0: 7210 0000 00a9 0072 1300 0000 fa72 2f77  r......r.....r/w
 00000300: 6f72 6b73 7061 6365 732f 636f 6e74 7269  orkspaces/contri
-00000310: 6266 6c65 742f 666c 6574 2f73 646b 2f70  bflet/flet/sdk/p
-00000320: 7974 686f 6e2f 7061 636b 6167 6573 2f66  ython/packages/f
-00000330: 6c65 742d 636f 7265 2f73 7263 2f66 6c65  let-core/src/fle
-00000340: 745f 636f 7265 2f63 6861 7274 732f 6261  t_core/charts/ba
-00000350: 725f 6368 6172 745f 726f 645f 7374 6163  r_chart_rod_stac
-00000360: 6b5f 6974 656d 2e70 7972 1100 0000 0900  k_item.pyr......
-00000370: 0000 7316 0000 0000 0f04 0102 0102 0102  ..s.............
-00000380: 0102 0102 fb06 0806 0106 0106 017a 1d42  .............z.B
-00000390: 6172 4368 6172 7452 6f64 5374 6163 6b49  arChartRodStackI
-000003a0: 7465 6d2e 5f5f 696e 6974 5f5f 6301 0000  tem.__init__c...
-000003b0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-000003c0: 0043 0000 0073 0400 0000 6401 5300 2902  .C...s....d.S.).
-000003d0: 4e5a 0a73 7461 636b 5f69 7465 6d72 1300  NZ.stack_itemr..
-000003e0: 0000 a901 7212 0000 0072 1300 0000 7213  ....r....r....r.
-000003f0: 0000 0072 1400 0000 da11 5f67 6574 5f63  ...r......_get_c
-00000400: 6f6e 7472 6f6c 5f6e 616d 6525 0000 0073  ontrol_name%...s
-00000410: 0200 0000 0001 7a26 4261 7243 6861 7274  ......z&BarChart
-00000420: 526f 6453 7461 636b 4974 656d 2e5f 6765  RodStackItem._ge
-00000430: 745f 636f 6e74 726f 6c5f 6e61 6d65 6301  t_control_namec.
-00000440: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000450: 0000 0003 0000 0073 1c00 0000 7400 8300  .......s....t...
-00000460: a001 a100 0100 7c00 a002 6401 7c00 6a03  ......|...d.|.j.
-00000470: a102 0100 6400 5300 2902 4eda 0a62 6f72  ....d.S.).N..bor
-00000480: 6465 7253 6964 6529 04da 0573 7570 6572  derSide)...super
-00000490: da0d 6265 666f 7265 5f75 7064 6174 65da  ..before_update.
-000004a0: 0e5f 7365 745f 6174 7472 5f6a 736f 6eda  ._set_attr_json.
-000004b0: 225f 4261 7243 6861 7274 526f 6453 7461  "_BarChartRodSta
-000004c0: 636b 4974 656d 5f5f 626f 7264 6572 5f73  ckItem__border_s
-000004d0: 6964 6572 1500 0000 a901 da09 5f5f 636c  ider........__cl
-000004e0: 6173 735f 5f72 1300 0000 7214 0000 0072  ass__r....r....r
-000004f0: 1900 0000 2800 0000 7304 0000 0000 010a  ....(...s.......
-00000500: 017a 2242 6172 4368 6172 7452 6f64 5374  .z"BarChartRodSt
-00000510: 6163 6b49 7465 6d2e 6265 666f 7265 5f75  ackItem.before_u
-00000520: 7064 6174 6529 01da 0672 6574 7572 6e63  pdate)...returnc
-00000530: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000540: 0400 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
-00000550: 0064 0164 0264 038d 0253 0029 044e da05  .d.d.d...S.).N..
-00000560: 6672 6f6d 59da 0566 6c6f 6174 a901 da09  fromY..float....
-00000570: 6461 7461 5f74 7970 65a9 01da 095f 6765  data_type...._ge
-00000580: 745f 6174 7472 7215 0000 0072 1300 0000  t_attrr....r....
-00000590: 7213 0000 0072 1400 0000 7209 0000 002d  r....r....r....-
-000005a0: 0000 0073 0200 0000 0002 7a1b 4261 7243  ...s......z.BarC
-000005b0: 6861 7274 526f 6453 7461 636b 4974 656d  hartRodStackItem
-000005c0: 2e66 726f 6d5f 7929 01da 0576 616c 7565  .from_y)...value
-000005d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000005e0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-000005f0: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
-00000600: 4e72 1f00 0000 a901 da09 5f73 6574 5f61  Nr........_set_a
-00000610: 7474 72a9 0272 1200 0000 7225 0000 0072  ttr..r....r%...r
-00000620: 1300 0000 7213 0000 0072 1400 0000 7209  ....r....r....r.
-00000630: 0000 0031 0000 0073 0200 0000 0002 6301  ...1...s......c.
-00000640: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000650: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
-00000660: 6401 6402 6403 8d02 5300 2904 4eda 0374  d.d.d...S.).N..t
-00000670: 6f59 7220 0000 0072 2100 0000 7223 0000  oYr ...r!...r#..
-00000680: 0072 1500 0000 7213 0000 0072 1300 0000  .r....r....r....
-00000690: 7214 0000 0072 0a00 0000 3600 0000 7302  r....r....6...s.
-000006a0: 0000 0000 027a 1942 6172 4368 6172 7452  .....z.BarChartR
-000006b0: 6f64 5374 6163 6b49 7465 6d2e 746f 5f79  odStackItem.to_y
-000006c0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000006d0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-000006e0: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
-000006f0: 4e72 2900 0000 7226 0000 0072 2800 0000  Nr)...r&...r(...
-00000700: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000710: 0a00 0000 3a00 0000 7302 0000 0000 0263  ....:...s......c
-00000720: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000730: 0300 0000 4300 0000 730a 0000 007c 00a0  ....C...s....|..
-00000740: 0064 01a1 0153 00a9 024e 720b 0000 0072  .d...S...Nr....r
-00000750: 2300 0000 7215 0000 0072 1300 0000 7213  #...r....r....r.
-00000760: 0000 0072 1400 0000 720b 0000 003f 0000  ...r....r....?..
-00000770: 0073 0200 0000 0002 7a1a 4261 7243 6861  .s......z.BarCha
-00000780: 7274 526f 6453 7461 636b 4974 656d 2e63  rtRodStackItem.c
-00000790: 6f6c 6f72 6302 0000 0000 0000 0000 0000  olorc...........
-000007a0: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-000007b0: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
-000007c0: 5300 722a 0000 0072 2600 0000 7228 0000  S.r*...r&...r(..
-000007d0: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-000007e0: 720b 0000 0043 0000 0073 0200 0000 0002  r....C...s......
-000007f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000800: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00000810: 6a00 5300 a901 4ea9 0172 1b00 0000 7215  j.S...N..r....r.
-00000820: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000830: 0000 720c 0000 0048 0000 0073 0200 0000  ..r....H...s....
-00000840: 0002 7a20 4261 7243 6861 7274 526f 6453  ..z BarChartRodS
-00000850: 7461 636b 4974 656d 2e62 6f72 6465 725f  tackItem.border_
-00000860: 7369 6465 6302 0000 0000 0000 0000 0000  sidec...........
-00000870: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00000880: 0000 7c01 7c00 5f00 6400 5300 722b 0000  ..|.|._.d.S.r+..
-00000890: 0072 2c00 0000 7228 0000 0072 1300 0000  .r,...r(...r....
-000008a0: 7213 0000 0072 1400 0000 720c 0000 004c  r....r....r....L
-000008b0: 0000 0073 0200 0000 0002 2908 4e4e 4e4e  ...s......).NNNN
-000008c0: 4e4e 4e4e 2914 da08 5f5f 6e61 6d65 5f5f  NNNN)...__name__
-000008d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000008e0: 7175 616c 6e61 6d65 5f5f 7206 0000 0072  qualname__r....r
-000008f0: 0300 0000 da03 7374 7272 0400 0000 7207  ......strr....r.
-00000900: 0000 00da 0462 6f6f 6c72 0200 0000 7211  .....boolr....r.
-00000910: 0000 0072 1600 0000 7219 0000 00da 0870  ...r....r......p
-00000920: 726f 7065 7274 7972 0900 0000 da06 7365  ropertyr......se
-00000930: 7474 6572 720a 0000 0072 0b00 0000 720c  tterr....r....r.
-00000940: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000950: 5f5f 7213 0000 0072 1300 0000 721c 0000  __r....r....r...
-00000960: 0072 1400 0000 7208 0000 0008 0000 0073  .r....r........s
-00000970: 4800 0000 0803 0001 0001 0001 0004 0001  H...............
-00000980: 0001 0001 00f4 0202 0201 0201 0601 0604  ................
-00000990: 0601 0601 0601 02f4 0c1c 0803 0c05 0201  ................
-000009a0: 1003 0401 1004 0201 1003 0401 1004 0201  ................
-000009b0: 1403 0401 1404 0201 1403 0401 7208 0000  ............r...
-000009c0: 004e 290b da06 7479 7069 6e67 7202 0000  .N)...typingr...
-000009d0: 0072 0300 0000 da10 666c 6574 5f63 6f72  .r......flet_cor
-000009e0: 652e 626f 7264 6572 7204 0000 00da 1166  e.borderr......f
-000009f0: 6c65 745f 636f 7265 2e63 6f6e 7472 6f6c  let_core.control
-00000a00: 7205 0000 0072 0600 0000 da0d 666c 6574  r....r......flet
-00000a10: 5f63 6f72 652e 7265 6672 0700 0000 7208  _core.refr....r.
-00000a20: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
-00000a30: 0000 7214 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000a40: 3e01 0000 0073 0800 0000 1002 0c01 1001  >....s..........
-00000a50: 0c03                                     ..
+00000310: 6266 6c65 742f 666c 6574 636f 6e74 7269  bflet/fletcontri
+00000320: 622f 7364 6b2f 7079 7468 6f6e 2f70 6163  b/sdk/python/pac
+00000330: 6b61 6765 732f 666c 6574 2d63 6f72 652f  kages/flet-core/
+00000340: 7372 632f 666c 6574 5f63 6f72 652f 6368  src/flet_core/ch
+00000350: 6172 7473 2f62 6172 5f63 6861 7274 5f72  arts/bar_chart_r
+00000360: 6f64 5f73 7461 636b 5f69 7465 6d2e 7079  od_stack_item.py
+00000370: 7211 0000 0009 0000 0073 1600 0000 000f  r........s......
+00000380: 0401 0201 0201 0201 0201 02fb 0608 0601  ................
+00000390: 0601 0601 7a1d 4261 7243 6861 7274 526f  ....z.BarChartRo
+000003a0: 6453 7461 636b 4974 656d 2e5f 5f69 6e69  dStackItem.__ini
+000003b0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+000003c0: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+000003d0: 0064 0153 0029 024e 5a0a 7374 6163 6b5f  .d.S.).NZ.stack_
+000003e0: 6974 656d 7213 0000 00a9 0172 1200 0000  itemr......r....
+000003f0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00000400: 115f 6765 745f 636f 6e74 726f 6c5f 6e61  ._get_control_na
+00000410: 6d65 2500 0000 7302 0000 0000 017a 2642  me%...s......z&B
+00000420: 6172 4368 6172 7452 6f64 5374 6163 6b49  arChartRodStackI
+00000430: 7465 6d2e 5f67 6574 5f63 6f6e 7472 6f6c  tem._get_control
+00000440: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
+00000450: 0000 0100 0000 0400 0000 0300 0000 731c  ..............s.
+00000460: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
+00000470: 0264 017c 006a 03a1 0201 0064 0053 0029  .d.|.j.....d.S.)
+00000480: 024e da0a 626f 7264 6572 5369 6465 2904  .N..borderSide).
+00000490: da05 7375 7065 72da 0d62 6566 6f72 655f  ..super..before_
+000004a0: 7570 6461 7465 da0e 5f73 6574 5f61 7474  update.._set_att
+000004b0: 725f 6a73 6f6e da22 5f42 6172 4368 6172  r_json."_BarChar
+000004c0: 7452 6f64 5374 6163 6b49 7465 6d5f 5f62  tRodStackItem__b
+000004d0: 6f72 6465 725f 7369 6465 7215 0000 00a9  order_sider.....
+000004e0: 01da 095f 5f63 6c61 7373 5f5f 7213 0000  ...__class__r...
+000004f0: 0072 1400 0000 7219 0000 0028 0000 0073  .r....r....(...s
+00000500: 0400 0000 0001 0a01 7a22 4261 7243 6861  ........z"BarCha
+00000510: 7274 526f 6453 7461 636b 4974 656d 2e62  rtRodStackItem.b
+00000520: 6566 6f72 655f 7570 6461 7465 2901 da06  efore_update)...
+00000530: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000540: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000550: 0e00 0000 7c00 6a00 6401 6402 6403 8d02  ....|.j.d.d.d...
+00000560: 5300 2904 4eda 0566 726f 6d59 da05 666c  S.).N..fromY..fl
+00000570: 6f61 74a9 01da 0964 6174 615f 7479 7065  oat....data_type
+00000580: a901 da09 5f67 6574 5f61 7474 7272 1500  ...._get_attrr..
+00000590: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+000005a0: 0072 0900 0000 2d00 0000 7302 0000 0000  .r....-...s.....
+000005b0: 027a 1b42 6172 4368 6172 7452 6f64 5374  .z.BarChartRodSt
+000005c0: 6163 6b49 7465 6d2e 6672 6f6d 5f79 2901  ackItem.from_y).
+000005d0: da05 7661 6c75 6563 0200 0000 0000 0000  ..valuec........
+000005e0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+000005f0: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
+00000600: 0064 0053 0029 024e 721f 0000 00a9 01da  .d.S.).Nr.......
+00000610: 095f 7365 745f 6174 7472 a902 7212 0000  ._set_attr..r...
+00000620: 0072 2500 0000 7213 0000 0072 1300 0000  .r%...r....r....
+00000630: 7214 0000 0072 0900 0000 3100 0000 7302  r....r....1...s.
+00000640: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00000650: 0000 0100 0000 0400 0000 4300 0000 730e  ..........C...s.
+00000660: 0000 007c 006a 0064 0164 0264 038d 0253  ...|.j.d.d.d...S
+00000670: 0029 044e da03 746f 5972 2000 0000 7221  .).N..toYr ...r!
+00000680: 0000 0072 2300 0000 7215 0000 0072 1300  ...r#...r....r..
+00000690: 0000 7213 0000 0072 1400 0000 720a 0000  ..r....r....r...
+000006a0: 0036 0000 0073 0200 0000 0002 7a19 4261  .6...s......z.Ba
+000006b0: 7243 6861 7274 526f 6453 7461 636b 4974  rChartRodStackIt
+000006c0: 656d 2e74 6f5f 7963 0200 0000 0000 0000  em.to_yc........
+000006d0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+000006e0: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
+000006f0: 0064 0053 0029 024e 7229 0000 0072 2600  .d.S.).Nr)...r&.
+00000700: 0000 7228 0000 0072 1300 0000 7213 0000  ..r(...r....r...
+00000710: 0072 1400 0000 720a 0000 003a 0000 0073  .r....r....:...s
+00000720: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
+00000730: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000740: 0a00 0000 7c00 a000 6401 a101 5300 a902  ....|...d...S...
+00000750: 4e72 0b00 0000 7223 0000 0072 1500 0000  Nr....r#...r....
+00000760: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000770: 0b00 0000 3f00 0000 7302 0000 0000 027a  ....?...s......z
+00000780: 1a42 6172 4368 6172 7452 6f64 5374 6163  .BarChartRodStac
+00000790: 6b49 7465 6d2e 636f 6c6f 7263 0200 0000  kItem.colorc....
+000007a0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000007b0: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
+000007c0: 01a1 0201 0064 0053 0072 2a00 0000 7226  .....d.S.r*...r&
+000007d0: 0000 0072 2800 0000 7213 0000 0072 1300  ...r(...r....r..
+000007e0: 0000 7214 0000 0072 0b00 0000 4300 0000  ..r....r....C...
+000007f0: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00000800: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000810: 7306 0000 007c 006a 0053 00a9 014e a901  s....|.j.S...N..
+00000820: 721b 0000 0072 1500 0000 7213 0000 0072  r....r....r....r
+00000830: 1300 0000 7214 0000 0072 0c00 0000 4800  ....r....r....H.
+00000840: 0000 7302 0000 0000 027a 2042 6172 4368  ..s......z BarCh
+00000850: 6172 7452 6f64 5374 6163 6b49 7465 6d2e  artRodStackItem.
+00000860: 626f 7264 6572 5f73 6964 6563 0200 0000  border_sidec....
+00000870: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000880: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+00000890: 0053 0072 2b00 0000 722c 0000 0072 2800  .S.r+...r,...r(.
+000008a0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+000008b0: 0072 0c00 0000 4c00 0000 7302 0000 0000  .r....L...s.....
+000008c0: 0229 084e 4e4e 4e4e 4e4e 4e29 14da 085f  .).NNNNNNNN)..._
+000008d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000008e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000008f0: 5f72 0600 0000 7203 0000 00da 0373 7472  _r....r......str
+00000900: 7204 0000 0072 0700 0000 da04 626f 6f6c  r....r......bool
+00000910: 7202 0000 0072 1100 0000 7216 0000 0072  r....r....r....r
+00000920: 1900 0000 da08 7072 6f70 6572 7479 7209  ......propertyr.
+00000930: 0000 00da 0673 6574 7465 7272 0a00 0000  .....setterr....
+00000940: 720b 0000 0072 0c00 0000 da0d 5f5f 636c  r....r......__cl
+00000950: 6173 7363 656c 6c5f 5f72 1300 0000 7213  asscell__r....r.
+00000960: 0000 0072 1c00 0000 7214 0000 0072 0800  ...r....r....r..
+00000970: 0000 0800 0000 7348 0000 0008 0300 0100  ......sH........
+00000980: 0100 0100 0400 0100 0100 0100 f402 0202  ................
+00000990: 0102 0106 0106 0406 0106 0106 0102 f40c  ................
+000009a0: 1c08 030c 0502 0110 0304 0110 0402 0110  ................
+000009b0: 0304 0110 0402 0114 0304 0114 0402 0114  ................
+000009c0: 0304 0172 0800 0000 4e29 0bda 0674 7970  ...r....N)...typ
+000009d0: 696e 6772 0200 0000 7203 0000 00da 1066  ingr....r......f
+000009e0: 6c65 745f 636f 7265 2e62 6f72 6465 7272  let_core.borderr
+000009f0: 0400 0000 da11 666c 6574 5f63 6f72 652e  ......flet_core.
+00000a00: 636f 6e74 726f 6c72 0500 0000 7206 0000  controlr....r...
+00000a10: 00da 0d66 6c65 745f 636f 7265 2e72 6566  ...flet_core.ref
+00000a20: 7207 0000 0072 0800 0000 7213 0000 0072  r....r....r....r
+00000a30: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
+00000a40: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000a50: 0010 020c 0110 010c 03                   .........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 2923 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 6b0b 0000  a........:)fk...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 6b0b 0000  a........./fk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000070: 8400 6406 6507 8303 5a0b 6407 5300 2908  ..d.e...Z.d.S.).
@@ -50,159 +50,159 @@
 00000310: 0000 7213 0000 0029 0872 0600 0000 da08  ..r....).r......
 00000320: 5f5f 696e 6974 5f5f 720a 0000 0072 0b00  __init__r....r..
 00000330: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
 00000340: 0072 0f00 0000 290b da04 7365 6c66 720a  .r....)...selfr.
 00000350: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
 00000360: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
 00000370: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000380: a900 7216 0000 00fa 5d2f 776f 726b 7370  ..r.....]/worksp
+00000380: a900 7216 0000 00fa 642f 776f 726b 7370  ..r.....d/worksp
 00000390: 6163 6573 2f63 6f6e 7472 6962 666c 6574  aces/contribflet
-000003a0: 2f66 6c65 742f 7364 6b2f 7079 7468 6f6e  /flet/sdk/python
-000003b0: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
-000003c0: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
-000003d0: 652f 6368 6172 7473 2f63 6861 7274 5f61  e/charts/chart_a
-000003e0: 7869 732e 7079 7214 0000 0009 0000 0073  xis.pyr........s
-000003f0: 1a00 0000 0011 0401 0201 0201 0201 0201  ................
-00000400: 02fb 0608 0601 0601 0601 0601 0601 7a12  ..............z.
-00000410: 4368 6172 7441 7869 732e 5f5f 696e 6974  ChartAxis.__init
-00000420: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00000430: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-00000440: 6401 5300 2902 4e5a 0461 7869 7372 1600  d.S.).NZ.axisr..
-00000450: 0000 a901 7215 0000 0072 1600 0000 7216  ....r....r....r.
-00000460: 0000 0072 1700 0000 da11 5f67 6574 5f63  ...r......_get_c
-00000470: 6f6e 7472 6f6c 5f6e 616d 6529 0000 0073  ontrol_name)...s
-00000480: 0200 0000 0001 7a1b 4368 6172 7441 7869  ......z.ChartAxi
-00000490: 732e 5f67 6574 5f63 6f6e 7472 6f6c 5f6e  s._get_control_n
-000004a0: 616d 6563 0100 0000 0000 0000 0000 0000  amec............
-000004b0: 0300 0000 0500 0000 4300 0000 734a 0000  ........C...sJ..
-000004c0: 0067 007d 017c 006a 0044 005d 1a7d 027c  .g.}.|.j.D.].}.|
-000004d0: 02a0 0164 0164 02a1 0201 007c 01a0 027c  ...d.d.....|...|
-000004e0: 02a1 0101 0071 0a7c 006a 0372 467c 006a  .....q.|.j.rF|.j
-000004f0: 03a0 0164 0164 03a1 0201 007c 01a0 027c  ...d.d.....|...|
-00000500: 006a 03a1 0101 007c 0153 0029 044e da01  .j.....|.S.).N..
-00000510: 6eda 016c da01 7429 04da 125f 4368 6172  n..l..t)..._Char
-00000520: 7441 7869 735f 5f6c 6162 656c 73da 125f  tAxis__labels.._
-00000530: 7365 745f 6174 7472 5f69 6e74 6572 6e61  set_attr_interna
-00000540: 6cda 0661 7070 656e 64da 115f 4368 6172  l..append.._Char
-00000550: 7441 7869 735f 5f74 6974 6c65 2903 7215  tAxis__title).r.
-00000560: 0000 00da 0863 6869 6c64 7265 6eda 056c  .....children..l
-00000570: 6162 656c 7216 0000 0072 1600 0000 7217  abelr....r....r.
-00000580: 0000 00da 0d5f 6765 745f 6368 696c 6472  ....._get_childr
-00000590: 656e 2c00 0000 7310 0000 0000 0104 010a  en,...s.........
-000005a0: 010c 010c 0106 010e 010c 017a 1743 6861  ...........z.Cha
-000005b0: 7274 4178 6973 2e5f 6765 745f 6368 696c  rtAxis._get_chil
-000005c0: 6472 656e 2901 da06 7265 7475 726e 6301  dren)...returnc.
-000005d0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000005e0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-000005f0: 5300 a901 4ea9 0172 2000 0000 7218 0000  S...N..r ...r...
-00000600: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000610: 720a 0000 0037 0000 0073 0200 0000 0002  r....7...s......
-00000620: 7a0f 4368 6172 7441 7869 732e 7469 746c  z.ChartAxis.titl
-00000630: 6529 01da 0576 616c 7565 6302 0000 0000  e)...valuec.....
-00000640: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000650: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
-00000660: 5300 7225 0000 0072 2600 0000 a902 7215  S.r%...r&.....r.
-00000670: 0000 0072 2700 0000 7216 0000 0072 1600  ...r'...r....r..
-00000680: 0000 7217 0000 0072 0a00 0000 3b00 0000  ..r....r....;...
-00000690: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-000006a0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-000006b0: 730e 0000 007c 006a 0064 0164 0264 038d  s....|.j.d.d.d..
-000006c0: 0253 0029 044e da09 7469 746c 6553 697a  .S.).N..titleSiz
-000006d0: 65da 0566 6c6f 6174 a901 da09 6461 7461  e..float....data
-000006e0: 5f74 7970 65a9 01da 095f 6765 745f 6174  _type...._get_at
-000006f0: 7472 7218 0000 0072 1600 0000 7216 0000  trr....r....r...
-00000700: 0072 1700 0000 720b 0000 0040 0000 0073  .r....r....@...s
-00000710: 0200 0000 0002 7a14 4368 6172 7441 7869  ......z.ChartAxi
-00000720: 732e 7469 746c 655f 7369 7a65 6302 0000  s.title_sizec...
-00000730: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000740: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-00000750: 7c01 a102 0100 6400 5300 2902 4e72 2900  |.....d.S.).Nr).
-00000760: 0000 a901 da09 5f73 6574 5f61 7474 7272  ......_set_attrr
-00000770: 2800 0000 7216 0000 0072 1600 0000 7217  (...r....r....r.
-00000780: 0000 0072 0b00 0000 4400 0000 7302 0000  ...r....D...s...
-00000790: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-000007a0: 0100 0000 0500 0000 4300 0000 7310 0000  ........C...s...
-000007b0: 007c 006a 0064 0164 0264 0364 048d 0353  .|.j.d.d.d.d...S
-000007c0: 0029 054e da0a 7368 6f77 4c61 6265 6c73  .).N..showLabels
-000007d0: da04 626f 6f6c 54a9 0272 2c00 0000 da09  ..boolT..r,.....
-000007e0: 6465 665f 7661 6c75 6572 2d00 0000 7218  def_valuer-...r.
-000007f0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00000800: 0000 720c 0000 0049 0000 0073 0200 0000  ..r....I...s....
-00000810: 0002 7a15 4368 6172 7441 7869 732e 7368  ..z.ChartAxis.sh
-00000820: 6f77 5f6c 6162 656c 7363 0200 0000 0000  ow_labelsc......
-00000830: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000840: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-00000850: 0201 0064 0053 0029 024e 7231 0000 0072  ...d.S.).Nr1...r
-00000860: 2f00 0000 7228 0000 0072 1600 0000 7216  /...r(...r....r.
-00000870: 0000 0072 1700 0000 720c 0000 004d 0000  ...r....r....M..
-00000880: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000890: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000008a0: 0073 0600 0000 7c00 6a00 5300 7225 0000  .s....|.j.S.r%..
-000008b0: 00a9 0172 1d00 0000 7218 0000 0072 1600  ...r....r....r..
-000008c0: 0000 7216 0000 0072 1700 0000 720d 0000  ..r....r....r...
-000008d0: 0052 0000 0073 0200 0000 0002 7a10 4368  .R...s......z.Ch
-000008e0: 6172 7441 7869 732e 6c61 6265 6c73 6302  artAxis.labelsc.
-000008f0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000900: 0000 0043 0000 0073 1600 0000 7c01 6400  ...C...s....|.d.
-00000910: 7501 720c 7c01 6e02 6700 7c00 5f00 6400  u.r.|.n.g.|._.d.
-00000920: 5300 7225 0000 0072 3500 0000 7228 0000  S.r%...r5...r(..
-00000930: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000940: 720d 0000 0056 0000 0073 0200 0000 0002  r....V...s......
-00000950: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000960: 0005 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00000970: 6a00 6401 6402 6403 6404 8d03 5300 2905  j.d.d.d.d...S.).
-00000980: 4eda 0e6c 6162 656c 7349 6e74 6572 7661  N..labelsInterva
-00000990: 6c72 2a00 0000 6700 0000 0000 00f0 3f72  lr*...g.......?r
-000009a0: 3300 0000 722d 0000 0072 1800 0000 7216  3...r-...r....r.
-000009b0: 0000 0072 1600 0000 7217 0000 0072 0e00  ...r....r....r..
-000009c0: 0000 5b00 0000 7302 0000 0000 027a 1943  ..[...s......z.C
-000009d0: 6861 7274 4178 6973 2e6c 6162 656c 735f  hartAxis.labels_
-000009e0: 696e 7465 7276 616c 6302 0000 0000 0000  intervalc.......
-000009f0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000a00: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
-00000a10: 0100 6400 5300 2902 4e72 3600 0000 722f  ..d.S.).Nr6...r/
-00000a20: 0000 0072 2800 0000 7216 0000 0072 1600  ...r(...r....r..
-00000a30: 0000 7217 0000 0072 0e00 0000 5f00 0000  ..r....r...._...
-00000a40: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00000a50: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000a60: 730e 0000 007c 006a 0064 0164 0264 038d  s....|.j.d.d.d..
-00000a70: 0253 0029 044e da0a 6c61 6265 6c73 5369  .S.).N..labelsSi
-00000a80: 7a65 722a 0000 0072 2b00 0000 722d 0000  zer*...r+...r-..
-00000a90: 0072 1800 0000 7216 0000 0072 1600 0000  .r....r....r....
-00000aa0: 7217 0000 0072 0f00 0000 6400 0000 7302  r....r....d...s.
-00000ab0: 0000 0000 027a 1543 6861 7274 4178 6973  .....z.ChartAxis
-00000ac0: 2e6c 6162 656c 735f 7369 7a65 6302 0000  .labels_sizec...
-00000ad0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000ae0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-00000af0: 7c01 a102 0100 6400 5300 2902 4e72 3700  |.....d.S.).Nr7.
-00000b00: 0000 722f 0000 0072 2800 0000 7216 0000  ..r/...r(...r...
-00000b10: 0072 1600 0000 7217 0000 0072 0f00 0000  .r....r....r....
-00000b20: 6800 0000 7302 0000 0000 0229 0a4e 4e4e  h...s......).NNN
-00000b30: 4e4e 4e4e 4e4e 4e29 16da 085f 5f6e 616d  NNNNNNN)...__nam
-00000b40: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000b50: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0400  .__qualname__r..
-00000b60: 0000 7206 0000 0072 0700 0000 7232 0000  ..r....r....r2..
-00000b70: 0072 0300 0000 7205 0000 0072 0800 0000  .r....r....r....
-00000b80: 7202 0000 0072 1400 0000 7219 0000 0072  r....r....r....r
-00000b90: 2300 0000 da08 7072 6f70 6572 7479 720a  #.....propertyr.
-00000ba0: 0000 00da 0673 6574 7465 7272 0b00 0000  .....setterr....
-00000bb0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00000bc0: 0f00 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
-00000bd0: 0000 0072 1700 0000 7209 0000 0008 0000  ...r....r.......
-00000be0: 0073 6000 0000 0803 0001 0001 0001 0001  .s`.............
-00000bf0: 0001 0004 0001 0001 0001 00f2 0202 0601  ................
-00000c00: 0201 0601 0a01 0201 0204 0601 0601 0601  ................
-00000c10: 02f2 0c20 0803 080b 0201 1403 0401 1404  ... ............
-00000c20: 0201 1003 0401 1004 0201 1403 0401 1404  ................
-00000c30: 0201 0a03 0401 0a04 0201 1003 0401 1004  ................
-00000c40: 0201 1003 0401 7209 0000 004e 290c da06  ......r....N)...
-00000c50: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000c60: 7204 0000 00da 2166 6c65 745f 636f 7265  r.....!flet_core
-00000c70: 2e63 6861 7274 732e 6368 6172 745f 6178  .charts.chart_ax
-00000c80: 6973 5f6c 6162 656c 7205 0000 00da 1166  is_labelr......f
-00000c90: 6c65 745f 636f 7265 2e63 6f6e 7472 6f6c  let_core.control
-00000ca0: 7206 0000 0072 0700 0000 da0d 666c 6574  r....r......flet
-00000cb0: 5f63 6f72 652e 7265 6672 0800 0000 7209  _core.refr....r.
-00000cc0: 0000 0072 1600 0000 7216 0000 0072 1600  ...r....r....r..
-00000cd0: 0000 7217 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000ce0: 3e01 0000 0073 0800 0000 1402 0c01 1001  >....s..........
-00000cf0: 0c03                                     ..
+000003a0: 2f66 6c65 7463 6f6e 7472 6962 2f73 646b  /fletcontrib/sdk
+000003b0: 2f70 7974 686f 6e2f 7061 636b 6167 6573  /python/packages
+000003c0: 2f66 6c65 742d 636f 7265 2f73 7263 2f66  /flet-core/src/f
+000003d0: 6c65 745f 636f 7265 2f63 6861 7274 732f  let_core/charts/
+000003e0: 6368 6172 745f 6178 6973 2e70 7972 1400  chart_axis.pyr..
+000003f0: 0000 0900 0000 731a 0000 0000 1104 0102  ......s.........
+00000400: 0102 0102 0102 0102 fb06 0806 0106 0106  ................
+00000410: 0106 0106 017a 1243 6861 7274 4178 6973  .....z.ChartAxis
+00000420: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000430: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000440: 0000 7304 0000 0064 0153 0029 024e 5a04  ..s....d.S.).NZ.
+00000450: 6178 6973 7216 0000 00a9 0172 1500 0000  axisr......r....
+00000460: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00000470: 115f 6765 745f 636f 6e74 726f 6c5f 6e61  ._get_control_na
+00000480: 6d65 2900 0000 7302 0000 0000 017a 1b43  me)...s......z.C
+00000490: 6861 7274 4178 6973 2e5f 6765 745f 636f  hartAxis._get_co
+000004a0: 6e74 726f 6c5f 6e61 6d65 6301 0000 0000  ntrol_namec.....
+000004b0: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+000004c0: 0000 0073 4a00 0000 6700 7d01 7c00 6a00  ...sJ...g.}.|.j.
+000004d0: 4400 5d1a 7d02 7c02 a001 6401 6402 a102  D.].}.|...d.d...
+000004e0: 0100 7c01 a002 7c02 a101 0100 710a 7c00  ..|...|.....q.|.
+000004f0: 6a03 7246 7c00 6a03 a001 6401 6403 a102  j.rF|.j...d.d...
+00000500: 0100 7c01 a002 7c00 6a03 a101 0100 7c01  ..|...|.j.....|.
+00000510: 5300 2904 4eda 016e da01 6cda 0174 2904  S.).N..n..l..t).
+00000520: da12 5f43 6861 7274 4178 6973 5f5f 6c61  .._ChartAxis__la
+00000530: 6265 6c73 da12 5f73 6574 5f61 7474 725f  bels.._set_attr_
+00000540: 696e 7465 726e 616c da06 6170 7065 6e64  internal..append
+00000550: da11 5f43 6861 7274 4178 6973 5f5f 7469  .._ChartAxis__ti
+00000560: 746c 6529 0372 1500 0000 da08 6368 696c  tle).r......chil
+00000570: 6472 656e da05 6c61 6265 6c72 1600 0000  dren..labelr....
+00000580: 7216 0000 0072 1700 0000 da0d 5f67 6574  r....r......_get
+00000590: 5f63 6869 6c64 7265 6e2c 0000 0073 1000  _children,...s..
+000005a0: 0000 0001 0401 0a01 0c01 0c01 0601 0e01  ................
+000005b0: 0c01 7a17 4368 6172 7441 7869 732e 5f67  ..z.ChartAxis._g
+000005c0: 6574 5f63 6869 6c64 7265 6e29 01da 0672  et_children)...r
+000005d0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+000005e0: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+000005f0: 0000 007c 006a 0053 00a9 014e a901 7220  ...|.j.S...N..r 
+00000600: 0000 0072 1800 0000 7216 0000 0072 1600  ...r....r....r..
+00000610: 0000 7217 0000 0072 0a00 0000 3700 0000  ..r....r....7...
+00000620: 7302 0000 0000 027a 0f43 6861 7274 4178  s......z.ChartAx
+00000630: 6973 2e74 6974 6c65 2901 da05 7661 6c75  is.title)...valu
+00000640: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00000650: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
+00000660: 017c 005f 0064 0053 0072 2500 0000 7226  .|._.d.S.r%...r&
+00000670: 0000 00a9 0272 1500 0000 7227 0000 0072  .....r....r'...r
+00000680: 1600 0000 7216 0000 0072 1700 0000 720a  ....r....r....r.
+00000690: 0000 003b 0000 0073 0200 0000 0002 6301  ...;...s......c.
+000006a0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000006b0: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
+000006c0: 6401 6402 6403 8d02 5300 2904 4eda 0974  d.d.d...S.).N..t
+000006d0: 6974 6c65 5369 7a65 da05 666c 6f61 74a9  itleSize..float.
+000006e0: 01da 0964 6174 615f 7479 7065 a901 da09  ...data_type....
+000006f0: 5f67 6574 5f61 7474 7272 1800 0000 7216  _get_attrr....r.
+00000700: 0000 0072 1600 0000 7217 0000 0072 0b00  ...r....r....r..
+00000710: 0000 4000 0000 7302 0000 0000 027a 1443  ..@...s......z.C
+00000720: 6861 7274 4178 6973 2e74 6974 6c65 5f73  hartAxis.title_s
+00000730: 697a 6563 0200 0000 0000 0000 0000 0000  izec............
+00000740: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+00000750: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+00000760: 0029 024e 7229 0000 00a9 01da 095f 7365  .).Nr)......._se
+00000770: 745f 6174 7472 7228 0000 0072 1600 0000  t_attrr(...r....
+00000780: 7216 0000 0072 1700 0000 720b 0000 0044  r....r....r....D
+00000790: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+000007a0: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+000007b0: 0000 0073 1000 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
+000007c0: 6403 6404 8d03 5300 2905 4eda 0a73 686f  d.d...S.).N..sho
+000007d0: 774c 6162 656c 73da 0462 6f6f 6c54 a902  wLabels..boolT..
+000007e0: 722c 0000 00da 0964 6566 5f76 616c 7565  r,.....def_value
+000007f0: 722d 0000 0072 1800 0000 7216 0000 0072  r-...r....r....r
+00000800: 1600 0000 7217 0000 0072 0c00 0000 4900  ....r....r....I.
+00000810: 0000 7302 0000 0000 027a 1543 6861 7274  ..s......z.Chart
+00000820: 4178 6973 2e73 686f 775f 6c61 6265 6c73  Axis.show_labels
+00000830: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000840: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00000850: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
+00000860: 4e72 3100 0000 722f 0000 0072 2800 0000  Nr1...r/...r(...
+00000870: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000880: 0c00 0000 4d00 0000 7302 0000 0000 0263  ....M...s......c
+00000890: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000008a0: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+000008b0: 0053 0072 2500 0000 a901 721d 0000 0072  .S.r%.....r....r
+000008c0: 1800 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+000008d0: 0000 0072 0d00 0000 5200 0000 7302 0000  ...r....R...s...
+000008e0: 0000 027a 1043 6861 7274 4178 6973 2e6c  ...z.ChartAxis.l
+000008f0: 6162 656c 7363 0200 0000 0000 0000 0000  abelsc..........
+00000900: 0000 0200 0000 0200 0000 4300 0000 7316  ..........C...s.
+00000910: 0000 007c 0164 0075 0172 0c7c 016e 0267  ...|.d.u.r.|.n.g
+00000920: 007c 005f 0064 0053 0072 2500 0000 7235  .|._.d.S.r%...r5
+00000930: 0000 0072 2800 0000 7216 0000 0072 1600  ...r(...r....r..
+00000940: 0000 7217 0000 0072 0d00 0000 5600 0000  ..r....r....V...
+00000950: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00000960: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+00000970: 7310 0000 007c 006a 0064 0164 0264 0364  s....|.j.d.d.d.d
+00000980: 048d 0353 0029 054e da0e 6c61 6265 6c73  ...S.).N..labels
+00000990: 496e 7465 7276 616c 722a 0000 0067 0000  Intervalr*...g..
+000009a0: 0000 0000 f03f 7233 0000 0072 2d00 0000  .....?r3...r-...
+000009b0: 7218 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
+000009c0: 1700 0000 720e 0000 005b 0000 0073 0200  ....r....[...s..
+000009d0: 0000 0002 7a19 4368 6172 7441 7869 732e  ....z.ChartAxis.
+000009e0: 6c61 6265 6c73 5f69 6e74 6572 7661 6c63  labels_intervalc
+000009f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000a00: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+00000a10: 0064 017c 01a1 0201 0064 0053 0029 024e  .d.|.....d.S.).N
+00000a20: 7236 0000 0072 2f00 0000 7228 0000 0072  r6...r/...r(...r
+00000a30: 1600 0000 7216 0000 0072 1700 0000 720e  ....r....r....r.
+00000a40: 0000 005f 0000 0073 0200 0000 0002 6301  ..._...s......c.
+00000a50: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000a60: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
+00000a70: 6401 6402 6403 8d02 5300 2904 4eda 0a6c  d.d.d...S.).N..l
+00000a80: 6162 656c 7353 697a 6572 2a00 0000 722b  abelsSizer*...r+
+00000a90: 0000 0072 2d00 0000 7218 0000 0072 1600  ...r-...r....r..
+00000aa0: 0000 7216 0000 0072 1700 0000 720f 0000  ..r....r....r...
+00000ab0: 0064 0000 0073 0200 0000 0002 7a15 4368  .d...s......z.Ch
+00000ac0: 6172 7441 7869 732e 6c61 6265 6c73 5f73  artAxis.labels_s
+00000ad0: 697a 6563 0200 0000 0000 0000 0000 0000  izec............
+00000ae0: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+00000af0: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+00000b00: 0029 024e 7237 0000 0072 2f00 0000 7228  .).Nr7...r/...r(
+00000b10: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000b20: 0000 720f 0000 0068 0000 0073 0200 0000  ..r....h...s....
+00000b30: 0002 290a 4e4e 4e4e 4e4e 4e4e 4e4e 2916  ..).NNNNNNNNNN).
+00000b40: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000b50: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000b60: 6d65 5f5f 7204 0000 0072 0600 0000 7207  me__r....r....r.
+00000b70: 0000 0072 3200 0000 7203 0000 0072 0500  ...r2...r....r..
+00000b80: 0000 7208 0000 0072 0200 0000 7214 0000  ..r....r....r...
+00000b90: 0072 1900 0000 7223 0000 00da 0870 726f  .r....r#.....pro
+00000ba0: 7065 7274 7972 0a00 0000 da06 7365 7474  pertyr......sett
+00000bb0: 6572 720b 0000 0072 0c00 0000 720d 0000  err....r....r...
+00000bc0: 0072 0e00 0000 720f 0000 0072 1600 0000  .r....r....r....
+00000bd0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000be0: 0900 0000 0800 0000 7360 0000 0008 0300  ........s`......
+00000bf0: 0100 0100 0100 0100 0100 0400 0100 0100  ................
+00000c00: 0100 f202 0206 0102 0106 010a 0102 0102  ................
+00000c10: 0406 0106 0106 0102 f20c 2008 0308 0b02  .......... .....
+00000c20: 0114 0304 0114 0402 0110 0304 0110 0402  ................
+00000c30: 0114 0304 0114 0402 010a 0304 010a 0402  ................
+00000c40: 0110 0304 0110 0402 0110 0304 0172 0900  .............r..
+00000c50: 0000 4e29 0cda 0674 7970 696e 6772 0200  ..N)...typingr..
+00000c60: 0000 7203 0000 0072 0400 0000 da21 666c  ..r....r.....!fl
+00000c70: 6574 5f63 6f72 652e 6368 6172 7473 2e63  et_core.charts.c
+00000c80: 6861 7274 5f61 7869 735f 6c61 6265 6c72  hart_axis_labelr
+00000c90: 0500 0000 da11 666c 6574 5f63 6f72 652e  ......flet_core.
+00000ca0: 636f 6e74 726f 6c72 0600 0000 7207 0000  controlr....r...
+00000cb0: 00da 0d66 6c65 745f 636f 7265 2e72 6566  ...flet_core.ref
+00000cc0: 7208 0000 0072 0900 0000 7216 0000 0072  r....r....r....r
+00000cd0: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
+00000ce0: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000cf0: 0014 020c 0110 010c 03                   .........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1293 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 0d05 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 0d05 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000060: 8400 6405 6504 8303 5a08 6406 5300 2907  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 02da 0341 6e79 da08 4f70  .....)...Any..Op
@@ -30,88 +30,89 @@
 000001d0: 0501 007c 017c 005f 027c 027c 005f 0364  ...|.|._.|.|._.d
 000001e0: 0053 0029 024e 2904 720a 0000 0072 0b00  .S.).N).r....r..
 000001f0: 0000 720c 0000 0072 0d00 0000 2904 7204  ..r....r....).r.
 00000200: 0000 00da 085f 5f69 6e69 745f 5f72 0800  .....__init__r..
 00000210: 0000 7209 0000 0029 07da 0473 656c 6672  ..r....)...selfr
 00000220: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
 00000230: 0000 0072 0c00 0000 720d 0000 00a9 0072  ...r....r......r
-00000240: 1000 0000 fa63 2f77 6f72 6b73 7061 6365  .....c/workspace
+00000240: 1000 0000 fa6a 2f77 6f72 6b73 7061 6365  .....j/workspace
 00000250: 732f 636f 6e74 7269 6266 6c65 742f 666c  s/contribflet/fl
-00000260: 6574 2f73 646b 2f70 7974 686f 6e2f 7061  et/sdk/python/pa
-00000270: 636b 6167 6573 2f66 6c65 742d 636f 7265  ckages/flet-core
-00000280: 2f73 7263 2f66 6c65 745f 636f 7265 2f63  /src/flet_core/c
-00000290: 6861 7274 732f 6368 6172 745f 6178 6973  harts/chart_axis
-000002a0: 5f6c 6162 656c 2e70 7972 0e00 0000 0800  _label.pyr......
-000002b0: 0000 7312 0000 0000 0d04 0102 0102 0102  ..s.............
-000002c0: 0102 0102 fb06 0806 017a 1743 6861 7274  .........z.Chart
-000002d0: 4178 6973 4c61 6265 6c2e 5f5f 696e 6974  AxisLabel.__init
-000002e0: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-000002f0: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-00000300: 6401 5300 2902 4eda 016c 7210 0000 00a9  d.S.).N..lr.....
-00000310: 0172 0f00 0000 7210 0000 0072 1000 0000  .r....r....r....
-00000320: 7211 0000 00da 115f 6765 745f 636f 6e74  r......_get_cont
-00000330: 726f 6c5f 6e61 6d65 2000 0000 7302 0000  rol_name ...s...
-00000340: 0000 017a 2043 6861 7274 4178 6973 4c61  ...z ChartAxisLa
-00000350: 6265 6c2e 5f67 6574 5f63 6f6e 7472 6f6c  bel._get_control
-00000360: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
-00000370: 0000 0200 0000 0300 0000 4300 0000 731a  ..........C...s.
-00000380: 0000 0067 007d 017c 006a 0072 167c 01a0  ...g.}.|.j.r.|..
-00000390: 017c 006a 00a1 0101 007c 0153 00a9 014e  .|.j.....|.S...N
-000003a0: 2902 da16 5f43 6861 7274 4178 6973 4c61  )..._ChartAxisLa
-000003b0: 6265 6c5f 5f6c 6162 656c da06 6170 7065  bel__label..appe
-000003c0: 6e64 2902 720f 0000 00da 0863 6869 6c64  nd).r......child
-000003d0: 7265 6e72 1000 0000 7210 0000 0072 1100  renr....r....r..
-000003e0: 0000 da0d 5f67 6574 5f63 6869 6c64 7265  ...._get_childre
-000003f0: 6e23 0000 0073 0800 0000 0001 0401 0601  n#...s..........
-00000400: 0c01 7a1c 4368 6172 7441 7869 734c 6162  ..z.ChartAxisLab
-00000410: 656c 2e5f 6765 745f 6368 696c 6472 656e  el._get_children
-00000420: 2901 da06 7265 7475 726e 6301 0000 0000  )...returnc.....
-00000430: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-00000440: 0000 0073 1000 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
-00000450: 6403 6404 8d03 5300 2905 4e72 0800 0000  d.d...S.).Nr....
-00000460: da05 666c 6f61 7467 0000 0000 0000 f03f  ..floatg.......?
-00000470: 2902 da09 6461 7461 5f74 7970 65da 0964  )...data_type..d
-00000480: 6566 5f76 616c 7565 2901 da09 5f67 6574  ef_value)..._get
-00000490: 5f61 7474 7272 1300 0000 7210 0000 0072  _attrr....r....r
-000004a0: 1000 0000 7211 0000 0072 0800 0000 2a00  ....r....r....*.
-000004b0: 0000 7302 0000 0000 027a 1443 6861 7274  ..s......z.Chart
-000004c0: 4178 6973 4c61 6265 6c2e 7661 6c75 6529  AxisLabel.value)
-000004d0: 0172 0800 0000 6302 0000 0000 0000 0000  .r....c.........
-000004e0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-000004f0: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
-00000500: 6400 5300 2902 4e72 0800 0000 2901 da09  d.S.).Nr....)...
-00000510: 5f73 6574 5f61 7474 72a9 0272 0f00 0000  _set_attr..r....
-00000520: 7208 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000530: 1100 0000 7208 0000 002e 0000 0073 0200  ....r........s..
-00000540: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000550: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00000560: 0000 7c00 6a00 5300 7215 0000 00a9 0172  ..|.j.S.r......r
-00000570: 1600 0000 7213 0000 0072 1000 0000 7210  ....r....r....r.
-00000580: 0000 0072 1100 0000 7209 0000 0033 0000  ...r....r....3..
-00000590: 0073 0200 0000 0002 7a14 4368 6172 7441  .s......z.ChartA
-000005a0: 7869 734c 6162 656c 2e6c 6162 656c 6302  xisLabel.labelc.
-000005b0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-000005c0: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
-000005d0: 5f00 6400 5300 7215 0000 0072 2100 0000  _.d.S.r....r!...
-000005e0: 7220 0000 0072 1000 0000 7210 0000 0072  r ...r....r....r
-000005f0: 1100 0000 7209 0000 0037 0000 0073 0200  ....r....7...s..
-00000600: 0000 0002 2906 4e4e 4e4e 4e4e 2910 da08  ....).NNNNNN)...
-00000610: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000620: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000630: 5f5f 7205 0000 0072 0300 0000 7204 0000  __r....r....r...
-00000640: 0072 0600 0000 da04 626f 6f6c 7202 0000  .r......boolr...
-00000650: 0072 0e00 0000 7214 0000 0072 1900 0000  .r....r....r....
-00000660: da08 7072 6f70 6572 7479 7208 0000 00da  ..propertyr.....
-00000670: 0673 6574 7465 7272 0900 0000 7210 0000  .setterr....r...
-00000680: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000690: 7207 0000 0007 0000 0073 3000 0000 0803  r........s0.....
-000006a0: 0001 0004 0001 0001 0001 00f6 0202 0201  ................
-000006b0: 0604 0601 0601 0601 02f6 0c18 0803 0807  ................
-000006c0: 0201 1003 0401 1004 0201 1403 0401 7207  ..............r.
-000006d0: 0000 004e 2909 da06 7479 7069 6e67 7202  ...N)...typingr.
-000006e0: 0000 0072 0300 0000 da11 666c 6574 5f63  ...r......flet_c
-000006f0: 6f72 652e 636f 6e74 726f 6c72 0400 0000  ore.controlr....
-00000700: 7205 0000 00da 0d66 6c65 745f 636f 7265  r......flet_core
-00000710: 2e72 6566 7206 0000 0072 0700 0000 7210  .refr....r....r.
-00000720: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-00000730: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000740: 7306 0000 0010 0210 010c 03              s..........
+00000260: 6574 636f 6e74 7269 622f 7364 6b2f 7079  etcontrib/sdk/py
+00000270: 7468 6f6e 2f70 6163 6b61 6765 732f 666c  thon/packages/fl
+00000280: 6574 2d63 6f72 652f 7372 632f 666c 6574  et-core/src/flet
+00000290: 5f63 6f72 652f 6368 6172 7473 2f63 6861  _core/charts/cha
+000002a0: 7274 5f61 7869 735f 6c61 6265 6c2e 7079  rt_axis_label.py
+000002b0: 720e 0000 0008 0000 0073 1200 0000 000d  r........s......
+000002c0: 0401 0201 0201 0201 0201 02fb 0608 0601  ................
+000002d0: 7a17 4368 6172 7441 7869 734c 6162 656c  z.ChartAxisLabel
+000002e0: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+000002f0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000300: 0000 7304 0000 0064 0153 0029 024e da01  ..s....d.S.).N..
+00000310: 6c72 1000 0000 a901 720f 0000 0072 1000  lr......r....r..
+00000320: 0000 7210 0000 0072 1100 0000 da11 5f67  ..r....r......_g
+00000330: 6574 5f63 6f6e 7472 6f6c 5f6e 616d 6520  et_control_name 
+00000340: 0000 0073 0200 0000 0001 7a20 4368 6172  ...s......z Char
+00000350: 7441 7869 734c 6162 656c 2e5f 6765 745f  tAxisLabel._get_
+00000360: 636f 6e74 726f 6c5f 6e61 6d65 6301 0000  control_namec...
+00000370: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00000380: 0043 0000 0073 1a00 0000 6700 7d01 7c00  .C...s....g.}.|.
+00000390: 6a00 7216 7c01 a001 7c00 6a00 a101 0100  j.r.|...|.j.....
+000003a0: 7c01 5300 a901 4e29 02da 165f 4368 6172  |.S...N)..._Char
+000003b0: 7441 7869 734c 6162 656c 5f5f 6c61 6265  tAxisLabel__labe
+000003c0: 6cda 0661 7070 656e 6429 0272 0f00 0000  l..append).r....
+000003d0: da08 6368 696c 6472 656e 7210 0000 0072  ..childrenr....r
+000003e0: 1000 0000 7211 0000 00da 0d5f 6765 745f  ....r......_get_
+000003f0: 6368 696c 6472 656e 2300 0000 7308 0000  children#...s...
+00000400: 0000 0104 0106 010c 017a 1c43 6861 7274  .........z.Chart
+00000410: 4178 6973 4c61 6265 6c2e 5f67 6574 5f63  AxisLabel._get_c
+00000420: 6869 6c64 7265 6e29 01da 0672 6574 7572  hildren)...retur
+00000430: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
+00000440: 0000 0500 0000 4300 0000 7310 0000 007c  ......C...s....|
+00000450: 006a 0064 0164 0264 0364 048d 0353 0029  .j.d.d.d.d...S.)
+00000460: 054e 7208 0000 00da 0566 6c6f 6174 6700  .Nr......floatg.
+00000470: 0000 0000 00f0 3f29 02da 0964 6174 615f  ......?)...data_
+00000480: 7479 7065 da09 6465 665f 7661 6c75 6529  type..def_value)
+00000490: 01da 095f 6765 745f 6174 7472 7213 0000  ..._get_attrr...
+000004a0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+000004b0: 7208 0000 002a 0000 0073 0200 0000 0002  r....*...s......
+000004c0: 7a14 4368 6172 7441 7869 734c 6162 656c  z.ChartAxisLabel
+000004d0: 2e76 616c 7565 2901 7208 0000 0063 0200  .value).r....c..
+000004e0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000004f0: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
+00000500: 017c 01a1 0201 0064 0053 0029 024e 7208  .|.....d.S.).Nr.
+00000510: 0000 0029 01da 095f 7365 745f 6174 7472  ...)..._set_attr
+00000520: a902 720f 0000 0072 0800 0000 7210 0000  ..r....r....r...
+00000530: 0072 1000 0000 7211 0000 0072 0800 0000  .r....r....r....
+00000540: 2e00 0000 7302 0000 0000 0263 0100 0000  ....s......c....
+00000550: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00000560: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
+00000570: 1500 0000 a901 7216 0000 0072 1300 0000  ......r....r....
+00000580: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000590: 0900 0000 3300 0000 7302 0000 0000 027a  ....3...s......z
+000005a0: 1443 6861 7274 4178 6973 4c61 6265 6c2e  .ChartAxisLabel.
+000005b0: 6c61 6265 6c63 0200 0000 0000 0000 0000  labelc..........
+000005c0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+000005d0: 0000 007c 017c 005f 0064 0053 0072 1500  ...|.|._.d.S.r..
+000005e0: 0000 7221 0000 0072 2000 0000 7210 0000  ..r!...r ...r...
+000005f0: 0072 1000 0000 7211 0000 0072 0900 0000  .r....r....r....
+00000600: 3700 0000 7302 0000 0000 0229 064e 4e4e  7...s......).NNN
+00000610: 4e4e 4e29 10da 085f 5f6e 616d 655f 5fda  NNN)...__name__.
+00000620: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000630: 7561 6c6e 616d 655f 5f72 0500 0000 7203  ualname__r....r.
+00000640: 0000 0072 0400 0000 7206 0000 00da 0462  ...r....r......b
+00000650: 6f6f 6c72 0200 0000 720e 0000 0072 1400  oolr....r....r..
+00000660: 0000 7219 0000 00da 0870 726f 7065 7274  ..r......propert
+00000670: 7972 0800 0000 da06 7365 7474 6572 7209  yr......setterr.
+00000680: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
+00000690: 0000 7211 0000 0072 0700 0000 0700 0000  ..r....r........
+000006a0: 7330 0000 0008 0300 0100 0400 0100 0100  s0..............
+000006b0: 0100 f602 0202 0106 0406 0106 0106 0102  ................
+000006c0: f60c 1808 0308 0702 0110 0304 0110 0402  ................
+000006d0: 0114 0304 0172 0700 0000 4e29 09da 0674  .....r....N)...t
+000006e0: 7970 696e 6772 0200 0000 7203 0000 00da  ypingr....r.....
+000006f0: 1166 6c65 745f 636f 7265 2e63 6f6e 7472  .flet_core.contr
+00000700: 6f6c 7204 0000 0072 0500 0000 da0d 666c  olr....r......fl
+00000710: 6574 5f63 6f72 652e 7265 6672 0600 0000  et_core.refr....
+00000720: 7207 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00000730: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
+00000740: 6c65 3e01 0000 0073 0600 0000 1002 1001  le>....s........
+00000750: 0c03                                     ..
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 5201 0000  a........:)fR...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 5201 0000  a........./fR...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6500 6a05 4700 6404 6405 8400 6405  ..e.j.G.d.d...d.
 00000060: 8302 8301 5a06 6401 5300 2906 e900 0000  ....Z.d.S.).....
 00000070: 004e 2901 da05 6669 656c 6429 02da 044c  .N)...field)...L
@@ -23,22 +23,22 @@
 00000160: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00000170: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
 00000180: 0200 0000 7207 0000 0072 0400 0000 da05  ....r....r......
 00000190: 666c 6f61 74da 0f5f 5f61 6e6e 6f74 6174  float..__annotat
 000001a0: 696f 6e73 5f5f 7208 0000 00da 0373 7472  ions__r......str
 000001b0: 7209 0000 0072 0a00 0000 7203 0000 00da  r....r....r.....
 000001c0: 0369 6e74 a900 7212 0000 0072 1200 0000  .int..r....r....
-000001d0: fa63 2f77 6f72 6b73 7061 6365 732f 636f  .c/workspaces/co
-000001e0: 6e74 7269 6266 6c65 742f 666c 6574 2f73  ntribflet/flet/s
-000001f0: 646b 2f70 7974 686f 6e2f 7061 636b 6167  dk/python/packag
-00000200: 6573 2f66 6c65 742d 636f 7265 2f73 7263  es/flet-core/src
-00000210: 2f66 6c65 745f 636f 7265 2f63 6861 7274  /flet_core/chart
-00000220: 732f 6368 6172 745f 6772 6964 5f6c 696e  s/chart_grid_lin
-00000230: 6573 2e70 7972 0500 0000 0600 0000 7308  es.pyr........s.
-00000240: 0000 000a 0216 0116 0116 0172 0500 0000  ...........r....
-00000250: 2907 da0b 6461 7461 636c 6173 7365 7372  )...dataclassesr
-00000260: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-00000270: 0072 0400 0000 da09 6461 7461 636c 6173  .r......dataclas
-00000280: 7372 0500 0000 7212 0000 0072 1200 0000  sr....r....r....
-00000290: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
-000002a0: 756c 653e 0100 0000 7308 0000 0008 010c  ule>....s.......
-000002b0: 0110 0304 01                             .....
+000001d0: fa6a 2f77 6f72 6b73 7061 6365 732f 636f  .j/workspaces/co
+000001e0: 6e74 7269 6266 6c65 742f 666c 6574 636f  ntribflet/fletco
+000001f0: 6e74 7269 622f 7364 6b2f 7079 7468 6f6e  ntrib/sdk/python
+00000200: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
+00000210: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
+00000220: 652f 6368 6172 7473 2f63 6861 7274 5f67  e/charts/chart_g
+00000230: 7269 645f 6c69 6e65 732e 7079 7205 0000  rid_lines.pyr...
+00000240: 0006 0000 0073 0800 0000 0a02 1601 1601  .....s..........
+00000250: 1601 7205 0000 0029 07da 0b64 6174 6163  ..r....)...datac
+00000260: 6c61 7373 6573 7202 0000 00da 0674 7970  lassesr......typ
+00000270: 696e 6772 0300 0000 7204 0000 00da 0964  ingr....r......d
+00000280: 6174 6163 6c61 7373 7205 0000 0072 1200  ataclassr....r..
+00000290: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000002a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000002b0: 0800 0000 0801 0c01 1003 0401            ............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 286 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 1e01 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 1e01 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6500 6a05 4700 6404 6405 8400 6405  ..e.j.G.d.d...d.
 00000060: 8302 8301 5a06 6401 5300 2906 e900 0000  ....Z.d.S.).....
 00000070: 004e 2901 da05 6669 656c 6429 02da 044c  .N)...field)...L
@@ -20,22 +20,23 @@
 00000130: 685f 7061 7474 6572 6e29 0dda 085f 5f6e  h_pattern)...__n
 00000140: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00000150: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
 00000160: 0200 0000 7207 0000 0072 0400 0000 da03  ....r....r......
 00000170: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
 00000180: 6e73 5f5f 7208 0000 00da 0566 6c6f 6174  ns__r......float
 00000190: 7209 0000 0072 0300 0000 da03 696e 74a9  r....r......int.
-000001a0: 0072 1100 0000 7211 0000 00fa 632f 776f  .r....r.....c/wo
+000001a0: 0072 1100 0000 7211 0000 00fa 6a2f 776f  .r....r.....j/wo
 000001b0: 726b 7370 6163 6573 2f63 6f6e 7472 6962  rkspaces/contrib
-000001c0: 666c 6574 2f66 6c65 742f 7364 6b2f 7079  flet/flet/sdk/py
-000001d0: 7468 6f6e 2f70 6163 6b61 6765 732f 666c  thon/packages/fl
-000001e0: 6574 2d63 6f72 652f 7372 632f 666c 6574  et-core/src/flet
-000001f0: 5f63 6f72 652f 6368 6172 7473 2f63 6861  _core/charts/cha
-00000200: 7274 5f70 6f69 6e74 5f6c 696e 652e 7079  rt_point_line.py
-00000210: 7205 0000 0006 0000 0073 0600 0000 0a02  r........s......
-00000220: 1601 1601 7205 0000 0029 07da 0b64 6174  ....r....)...dat
-00000230: 6163 6c61 7373 6573 7202 0000 00da 0674  aclassesr......t
-00000240: 7970 696e 6772 0300 0000 7204 0000 00da  ypingr....r.....
-00000250: 0964 6174 6163 6c61 7373 7205 0000 0072  .dataclassr....r
-00000260: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000270: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000280: 0073 0800 0000 0801 0c01 1003 0401       .s............
+000001c0: 666c 6574 2f66 6c65 7463 6f6e 7472 6962  flet/fletcontrib
+000001d0: 2f73 646b 2f70 7974 686f 6e2f 7061 636b  /sdk/python/pack
+000001e0: 6167 6573 2f66 6c65 742d 636f 7265 2f73  ages/flet-core/s
+000001f0: 7263 2f66 6c65 745f 636f 7265 2f63 6861  rc/flet_core/cha
+00000200: 7274 732f 6368 6172 745f 706f 696e 745f  rts/chart_point_
+00000210: 6c69 6e65 2e70 7972 0500 0000 0600 0000  line.pyr........
+00000220: 7306 0000 000a 0216 0116 0172 0500 0000  s..........r....
+00000230: 2907 da0b 6461 7461 636c 6173 7365 7372  )...dataclassesr
+00000240: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00000250: 0072 0400 0000 da09 6461 7461 636c 6173  .r......dataclas
+00000260: 7372 0500 0000 7211 0000 0072 1100 0000  sr....r....r....
+00000270: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
+00000280: 756c 653e 0100 0000 7308 0000 0008 010c  ule>....s.......
+00000290: 0110 0304 01                             .....
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 1006 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 ee03 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 ee03 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6500  ..d.d.l.m.Z...e.
 00000050: 6a04 4700 6404 6405 8400 6405 8302 8301  j.G.d.d...d.....
 00000060: 5a05 6500 6a04 4700 6406 6407 8400 6407  Z.e.j.G.d.d...d.
 00000070: 6505 8303 8301 5a06 6500 6a04 4700 6408  e.....Z.e.j.G.d.
@@ -13,85 +13,85 @@
 000000c0: 696f 6e61 6c63 0000 0000 0000 0000 0000  ionalc..........
 000000d0: 0000 0000 0000 0100 0000 4000 0000 730c  ..........@...s.
 000000e0: 0000 0065 005a 0164 005a 0264 0153 0029  ...e.Z.d.Z.d.S.)
 000000f0: 02da 0f43 6861 7274 506f 696e 7453 6861  ...ChartPointSha
 00000100: 7065 4e29 03da 085f 5f6e 616d 655f 5fda  peN)...__name__.
 00000110: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 00000120: 7561 6c6e 616d 655f 5fa9 0072 0800 0000  ualname__..r....
-00000130: 7208 0000 00fa 642f 776f 726b 7370 6163  r.....d/workspac
+00000130: 7208 0000 00fa 6b2f 776f 726b 7370 6163  r.....k/workspac
 00000140: 6573 2f63 6f6e 7472 6962 666c 6574 2f66  es/contribflet/f
-00000150: 6c65 742f 7364 6b2f 7079 7468 6f6e 2f70  let/sdk/python/p
-00000160: 6163 6b61 6765 732f 666c 6574 2d63 6f72  ackages/flet-cor
-00000170: 652f 7372 632f 666c 6574 5f63 6f72 652f  e/src/flet_core/
-00000180: 6368 6172 7473 2f63 6861 7274 5f70 6f69  charts/chart_poi
-00000190: 6e74 5f73 6861 7065 2e70 7972 0400 0000  nt_shape.pyr....
-000001a0: 0600 0000 7302 0000 0008 0272 0400 0000  ....s......r....
-000001b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000001c0: 0003 0000 0040 0000 0073 7800 0000 6500  .....@...sx...e.
-000001d0: 5a01 6400 5a02 5500 6503 6401 6402 8d01  Z.d.Z.U.e.d.d...
-000001e0: 5a04 6505 6506 6403 3c00 6503 6404 6402  Z.e.e.d.<.e.d.d.
-000001f0: 8d01 5a07 6508 6505 1900 6506 6405 3c00  ..Z.e.e...e.d.<.
-00000200: 6503 6404 6402 8d01 5a09 6508 650a 1900  e.d.d...Z.e.e...
-00000210: 6506 6406 3c00 6503 6404 6402 8d01 5a0b  e.d.<.e.d.d...Z.
-00000220: 6508 6505 1900 6506 6407 3c00 6503 6404  e.e...e.d.<.e.d.
-00000230: 6402 8d01 5a0c 6508 650a 1900 6506 6408  d...Z.e.e...e.d.
-00000240: 3c00 6404 5300 2909 da10 4368 6172 7443  <.d.S.)...ChartC
-00000250: 6972 636c 6550 6f69 6e74 da06 6369 7263  irclePoint..circ
-00000260: 6c65 a901 da07 6465 6661 756c 74da 0474  le....default..t
-00000270: 7970 654e da05 636f 6c6f 72da 0672 6164  ypeN..color..rad
-00000280: 6975 73da 0c73 7472 6f6b 655f 636f 6c6f  ius..stroke_colo
-00000290: 72da 0c73 7472 6f6b 655f 7769 6474 6829  r..stroke_width)
-000002a0: 0d72 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-000002b0: 7202 0000 0072 0e00 0000 da03 7374 72da  r....r......str.
-000002c0: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-000002d0: 720f 0000 0072 0300 0000 7210 0000 00da  r....r....r.....
-000002e0: 0566 6c6f 6174 7211 0000 0072 1200 0000  .floatr....r....
-000002f0: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00000300: 0900 0000 720a 0000 000b 0000 0073 0a00  ....r........s..
-00000310: 0000 0a02 1201 1601 1601 1601 720a 0000  ............r...
-00000320: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000330: 0000 0300 0000 4000 0000 7378 0000 0065  ......@...sx...e
-00000340: 005a 0164 005a 0255 0065 0364 0164 028d  .Z.d.Z.U.e.d.d..
-00000350: 015a 0465 0565 0664 033c 0065 0364 0464  .Z.e.e.d.<.e.d.d
-00000360: 028d 015a 0765 0865 0519 0065 0664 053c  ...Z.e.e...e.d.<
-00000370: 0065 0364 0464 028d 015a 0965 0865 0a19  .e.d.d...Z.e.e..
-00000380: 0065 0664 063c 0065 0364 0464 028d 015a  .e.d.<.e.d.d...Z
-00000390: 0b65 0865 0519 0065 0664 073c 0065 0364  .e.e...e.d.<.e.d
-000003a0: 0464 028d 015a 0c65 0865 0a19 0065 0664  .d...Z.e.e...e.d
-000003b0: 083c 0064 0453 0029 09da 1043 6861 7274  .<.d.S.)...Chart
-000003c0: 5371 7561 7265 506f 696e 74da 0673 7175  SquarePoint..squ
-000003d0: 6172 6572 0c00 0000 720e 0000 004e 720f  arer....r....Nr.
-000003e0: 0000 00da 0473 697a 6572 1100 0000 7212  .....sizer....r.
-000003f0: 0000 0029 0d72 0500 0000 7206 0000 0072  ...).r....r....r
-00000400: 0700 0000 7202 0000 0072 0e00 0000 7213  ....r....r....r.
-00000410: 0000 0072 1400 0000 720f 0000 0072 0300  ...r....r....r..
-00000420: 0000 7218 0000 0072 1500 0000 7211 0000  ..r....r....r...
-00000430: 0072 1200 0000 7208 0000 0072 0800 0000  .r....r....r....
-00000440: 7208 0000 0072 0900 0000 7216 0000 0014  r....r....r.....
-00000450: 0000 0073 0a00 0000 0a02 1201 1601 1601  ...s............
-00000460: 1601 7216 0000 0063 0000 0000 0000 0000  ..r....c........
-00000470: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000480: 7362 0000 0065 005a 0164 005a 0255 0065  sb...e.Z.d.Z.U.e
-00000490: 0364 0164 028d 015a 0465 0565 0664 033c  .d.d...Z.e.e.d.<
-000004a0: 0065 0364 0464 028d 015a 0765 0865 0519  .e.d.d...Z.e.e..
-000004b0: 0065 0664 053c 0065 0364 0464 028d 015a  .e.d.<.e.d.d...Z
-000004c0: 0965 0865 0a19 0065 0664 063c 0065 0364  .e.e...e.d.<.e.d
-000004d0: 0464 028d 015a 0b65 0865 0a19 0065 0664  .d...Z.e.e...e.d
-000004e0: 073c 0064 0453 0029 08da 0f43 6861 7274  .<.d.S.)...Chart
-000004f0: 4372 6f73 7350 6f69 6e74 5a05 6372 6f73  CrossPointZ.cros
-00000500: 7372 0c00 0000 720e 0000 004e 720f 0000  sr....r....Nr...
-00000510: 0072 1800 0000 da05 7769 6474 6829 0c72  .r......width).r
-00000520: 0500 0000 7206 0000 0072 0700 0000 7202  ....r....r....r.
-00000530: 0000 0072 0e00 0000 7213 0000 0072 1400  ...r....r....r..
-00000540: 0000 720f 0000 0072 0300 0000 7218 0000  ..r....r....r...
-00000550: 0072 1500 0000 721a 0000 0072 0800 0000  .r....r....r....
-00000560: 7208 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-00000570: 1900 0000 1d00 0000 7308 0000 000a 0212  ........s.......
-00000580: 0116 0116 0172 1900 0000 2909 da0b 6461  .....r....)...da
-00000590: 7461 636c 6173 7365 7372 0200 0000 da06  taclassesr......
-000005a0: 7479 7069 6e67 7203 0000 00da 0964 6174  typingr......dat
-000005b0: 6163 6c61 7373 7204 0000 0072 0a00 0000  aclassr....r....
-000005c0: 7216 0000 0072 1900 0000 7208 0000 0072  r....r....r....r
-000005d0: 0800 0000 7208 0000 0072 0900 0000 da08  ....r....r......
-000005e0: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
-000005f0: 0008 010c 010c 0304 0110 0404 0112 0804  ................
-00000600: 0112 0804 01                             .....
+00000150: 6c65 7463 6f6e 7472 6962 2f73 646b 2f70  letcontrib/sdk/p
+00000160: 7974 686f 6e2f 7061 636b 6167 6573 2f66  ython/packages/f
+00000170: 6c65 742d 636f 7265 2f73 7263 2f66 6c65  let-core/src/fle
+00000180: 745f 636f 7265 2f63 6861 7274 732f 6368  t_core/charts/ch
+00000190: 6172 745f 706f 696e 745f 7368 6170 652e  art_point_shape.
+000001a0: 7079 7204 0000 0006 0000 0073 0200 0000  pyr........s....
+000001b0: 0802 7204 0000 0063 0000 0000 0000 0000  ..r....c........
+000001c0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+000001d0: 7378 0000 0065 005a 0164 005a 0255 0065  sx...e.Z.d.Z.U.e
+000001e0: 0364 0164 028d 015a 0465 0565 0664 033c  .d.d...Z.e.e.d.<
+000001f0: 0065 0364 0464 028d 015a 0765 0865 0519  .e.d.d...Z.e.e..
+00000200: 0065 0664 053c 0065 0364 0464 028d 015a  .e.d.<.e.d.d...Z
+00000210: 0965 0865 0a19 0065 0664 063c 0065 0364  .e.e...e.d.<.e.d
+00000220: 0464 028d 015a 0b65 0865 0519 0065 0664  .d...Z.e.e...e.d
+00000230: 073c 0065 0364 0464 028d 015a 0c65 0865  .<.e.d.d...Z.e.e
+00000240: 0a19 0065 0664 083c 0064 0453 0029 09da  ...e.d.<.d.S.)..
+00000250: 1043 6861 7274 4369 7263 6c65 506f 696e  .ChartCirclePoin
+00000260: 74da 0663 6972 636c 65a9 01da 0764 6566  t..circle....def
+00000270: 6175 6c74 da04 7479 7065 4eda 0563 6f6c  ault..typeN..col
+00000280: 6f72 da06 7261 6469 7573 da0c 7374 726f  or..radius..stro
+00000290: 6b65 5f63 6f6c 6f72 da0c 7374 726f 6b65  ke_color..stroke
+000002a0: 5f77 6964 7468 290d 7205 0000 0072 0600  _width).r....r..
+000002b0: 0000 7207 0000 0072 0200 0000 720e 0000  ..r....r....r...
+000002c0: 00da 0373 7472 da0f 5f5f 616e 6e6f 7461  ...str..__annota
+000002d0: 7469 6f6e 735f 5f72 0f00 0000 7203 0000  tions__r....r...
+000002e0: 0072 1000 0000 da05 666c 6f61 7472 1100  .r......floatr..
+000002f0: 0000 7212 0000 0072 0800 0000 7208 0000  ..r....r....r...
+00000300: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000310: 0b00 0000 730a 0000 000a 0212 0116 0116  ....s...........
+00000320: 0116 0172 0a00 0000 6300 0000 0000 0000  ...r....c.......
+00000330: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000340: 0073 7800 0000 6500 5a01 6400 5a02 5500  .sx...e.Z.d.Z.U.
+00000350: 6503 6401 6402 8d01 5a04 6505 6506 6403  e.d.d...Z.e.e.d.
+00000360: 3c00 6503 6404 6402 8d01 5a07 6508 6505  <.e.d.d...Z.e.e.
+00000370: 1900 6506 6405 3c00 6503 6404 6402 8d01  ..e.d.<.e.d.d...
+00000380: 5a09 6508 650a 1900 6506 6406 3c00 6503  Z.e.e...e.d.<.e.
+00000390: 6404 6402 8d01 5a0b 6508 6505 1900 6506  d.d...Z.e.e...e.
+000003a0: 6407 3c00 6503 6404 6402 8d01 5a0c 6508  d.<.e.d.d...Z.e.
+000003b0: 650a 1900 6506 6408 3c00 6404 5300 2909  e...e.d.<.d.S.).
+000003c0: da10 4368 6172 7453 7175 6172 6550 6f69  ..ChartSquarePoi
+000003d0: 6e74 da06 7371 7561 7265 720c 0000 0072  nt..squarer....r
+000003e0: 0e00 0000 4e72 0f00 0000 da04 7369 7a65  ....Nr......size
+000003f0: 7211 0000 0072 1200 0000 290d 7205 0000  r....r....).r...
+00000400: 0072 0600 0000 7207 0000 0072 0200 0000  .r....r....r....
+00000410: 720e 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000420: 0f00 0000 7203 0000 0072 1800 0000 7215  ....r....r....r.
+00000430: 0000 0072 1100 0000 7212 0000 0072 0800  ...r....r....r..
+00000440: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00000450: 0072 1600 0000 1400 0000 730a 0000 000a  .r........s.....
+00000460: 0212 0116 0116 0116 0172 1600 0000 6300  .........r....c.
+00000470: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000480: 0000 0040 0000 0073 6200 0000 6500 5a01  ...@...sb...e.Z.
+00000490: 6400 5a02 5500 6503 6401 6402 8d01 5a04  d.Z.U.e.d.d...Z.
+000004a0: 6505 6506 6403 3c00 6503 6404 6402 8d01  e.e.d.<.e.d.d...
+000004b0: 5a07 6508 6505 1900 6506 6405 3c00 6503  Z.e.e...e.d.<.e.
+000004c0: 6404 6402 8d01 5a09 6508 650a 1900 6506  d.d...Z.e.e...e.
+000004d0: 6406 3c00 6503 6404 6402 8d01 5a0b 6508  d.<.e.d.d...Z.e.
+000004e0: 650a 1900 6506 6407 3c00 6404 5300 2908  e...e.d.<.d.S.).
+000004f0: da0f 4368 6172 7443 726f 7373 506f 696e  ..ChartCrossPoin
+00000500: 745a 0563 726f 7373 720c 0000 0072 0e00  tZ.crossr....r..
+00000510: 0000 4e72 0f00 0000 7218 0000 00da 0577  ..Nr....r......w
+00000520: 6964 7468 290c 7205 0000 0072 0600 0000  idth).r....r....
+00000530: 7207 0000 0072 0200 0000 720e 0000 0072  r....r....r....r
+00000540: 1300 0000 7214 0000 0072 0f00 0000 7203  ....r....r....r.
+00000550: 0000 0072 1800 0000 7215 0000 0072 1a00  ...r....r....r..
+00000560: 0000 7208 0000 0072 0800 0000 7208 0000  ..r....r....r...
+00000570: 0072 0900 0000 7219 0000 001d 0000 0073  .r....r........s
+00000580: 0800 0000 0a02 1201 1601 1601 7219 0000  ............r...
+00000590: 0029 09da 0b64 6174 6163 6c61 7373 6573  .)...dataclasses
+000005a0: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
+000005b0: 0000 da09 6461 7461 636c 6173 7372 0400  ....dataclassr..
+000005c0: 0000 720a 0000 0072 1600 0000 7219 0000  ..r....r....r...
+000005d0: 0072 0800 0000 7208 0000 0072 0800 0000  .r....r....r....
+000005e0: 7209 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000005f0: 0000 0073 1400 0000 0801 0c01 0c03 0401  ...s............
+00000600: 1004 0401 1208 0401 1208 0401            ............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 11305 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 292c 0000  a........:)f),..
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 292c 0000  a........./f),..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
@@ -160,511 +160,512 @@
 000009f0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
 00000a00: 0200 0000 0400 0000 5300 0000 731a 0000  ........S...s...
 00000a10: 0074 00a0 017c 006a 02a1 017d 0174 0366  .t...|.j...}.t.f
 00000a20: 0069 007c 01a4 018e 0153 00a9 014e 2904  .i.|.....S...N).
 00000a30: da04 6a73 6f6e da05 6c6f 6164 7372 4100  ..json..loadsrA.
 00000a40: 0000 da0e 4c69 6e65 4368 6172 7445 7665  ....LineChartEve
 00000a50: 6e74 2902 da01 65da 0164 a900 7249 0000  nt)...e..d..rI..
-00000a60: 00fa 5d2f 776f 726b 7370 6163 6573 2f63  ..]/workspaces/c
-00000a70: 6f6e 7472 6962 666c 6574 2f66 6c65 742f  ontribflet/flet/
-00000a80: 7364 6b2f 7079 7468 6f6e 2f70 6163 6b61  sdk/python/packa
-00000a90: 6765 732f 666c 6574 2d63 6f72 652f 7372  ges/flet-core/sr
-00000aa0: 632f 666c 6574 5f63 6f72 652f 6368 6172  c/flet_core/char
-00000ab0: 7473 2f6c 696e 655f 6368 6172 742e 7079  ts/line_chart.py
-00000ac0: da1c 636f 6e76 6572 745f 6c69 6e65 6368  ..convert_linech
-00000ad0: 6172 745f 6576 656e 745f 6461 7461 6a00  art_event_dataj.
-00000ae0: 0000 7304 0000 0000 010c 017a 384c 696e  ..s........z8Lin
-00000af0: 6543 6861 7274 2e5f 5f69 6e69 745f 5f2e  eChart.__init__.
-00000b00: 3c6c 6f63 616c 733e 2e63 6f6e 7665 7274  <locals>.convert
-00000b10: 5f6c 696e 6563 6861 7274 5f65 7665 6e74  _linechart_event
-00000b20: 5f64 6174 61da 0b63 6861 7274 5f65 7665  _data..chart_eve
-00000b30: 6e74 291b 720a 0000 00da 085f 5f69 6e69  nt).r......__ini
-00000b40: 745f 5f72 0d00 0000 da1a 5f4c 696e 6543  t__r......_LineC
-00000b50: 6861 7274 5f5f 6f6e 5f63 6861 7274 5f65  hart__on_chart_e
-00000b60: 7665 6e74 da12 5f61 6464 5f65 7665 6e74  vent.._add_event
-00000b70: 5f68 616e 646c 6572 da0b 6765 745f 6861  _handler..get_ha
-00000b80: 6e64 6c65 7272 1500 0000 7216 0000 0072  ndlerr....r....r
-00000b90: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00000ba0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000bb0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000bc0: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-00000bd0: 7226 0000 0072 2400 0000 7225 0000 0072  r&...r$...r%...r
-00000be0: 2700 0000 7228 0000 00da 0e6f 6e5f 6368  '...r(.....on_ch
-00000bf0: 6172 745f 6576 656e 7429 31da 0473 656c  art_event)1..sel
-00000c00: 6672 1500 0000 7216 0000 0072 1700 0000  fr....r....r....
-00000c10: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000c20: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
-00000c30: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
-00000c40: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-00000c50: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00000c60: 7228 0000 0072 5100 0000 7229 0000 0072  r(...rQ...r)...r
-00000c70: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
-00000c80: 0000 0072 2e00 0000 722f 0000 0072 3000  ...r....r/...r0.
-00000c90: 0000 7231 0000 0072 3200 0000 7233 0000  ..r1...r2...r3..
-00000ca0: 0072 3400 0000 7235 0000 0072 3600 0000  .r4...r5...r6...
-00000cb0: 7237 0000 0072 3800 0000 7239 0000 0072  r7...r8...r9...r
-00000cc0: 3a00 0000 723b 0000 0072 3c00 0000 723d  :...r;...r<...r=
-00000cd0: 0000 0072 4200 0000 723e 0000 0072 3f00  ...rB...r>...r?.
-00000ce0: 0000 7240 0000 0072 4100 0000 724b 0000  ..r@...rA...rK..
-00000cf0: 0072 4900 0000 7249 0000 0072 4a00 0000  .rI...rI...rJ...
-00000d00: 724d 0000 0017 0000 0073 6a00 0000 0035  rM.......sj....5
-00000d10: 0401 0201 0201 0201 0201 0201 0201 0201  ................
-00000d20: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000d30: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000d40: 0201 0201 0201 02e5 061e 0804 0a01 1202  ................
-00000d50: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00000d60: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00000d70: 0601 0601 0601 0601 7a12 4c69 6e65 4368  ........z.LineCh
-00000d80: 6172 742e 5f5f 696e 6974 5f5f 6301 0000  art.__init__c...
-00000d90: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00000da0: 0043 0000 0073 0400 0000 6401 5300 2902  .C...s....d.S.).
-00000db0: 4e5a 096c 696e 6563 6861 7274 7249 0000  NZ.linechartrI..
-00000dc0: 00a9 0172 5200 0000 7249 0000 0072 4900  ...rR...rI...rI.
-00000dd0: 0000 724a 0000 00da 115f 6765 745f 636f  ..rJ....._get_co
-00000de0: 6e74 726f 6c5f 6e61 6d65 8700 0000 7302  ntrol_name....s.
-00000df0: 0000 0000 017a 1b4c 696e 6543 6861 7274  .....z.LineChart
-00000e00: 2e5f 6765 745f 636f 6e74 726f 6c5f 6e61  ._get_control_na
-00000e10: 6d65 6301 0000 0000 0000 0000 0000 0001  mec.............
-00000e20: 0000 0004 0000 0003 0000 0073 4600 0000  ...........sF...
-00000e30: 7400 8300 a001 a100 0100 7c00 a002 6401  t.........|...d.
-00000e40: 7c00 6a03 a102 0100 7c00 a002 6402 7c00  |.j.....|...d.|.
-00000e50: 6a04 a102 0100 7c00 a002 6403 7c00 6a05  j.....|...d.|.j.
-00000e60: a102 0100 7c00 a002 6404 7c00 6a06 a102  ....|...d.|.j...
-00000e70: 0100 6400 5300 2905 4eda 1368 6f72 697a  ..d.S.).N..horiz
-00000e80: 6f6e 7461 6c47 7269 644c 696e 6573 da11  ontalGridLines..
-00000e90: 7665 7274 6963 616c 4772 6964 4c69 6e65  verticalGridLine
-00000ea0: 7372 1600 0000 721c 0000 0029 07da 0573  sr....r....)...s
-00000eb0: 7570 6572 da0d 6265 666f 7265 5f75 7064  uper..before_upd
-00000ec0: 6174 65da 0e5f 7365 745f 6174 7472 5f6a  ate.._set_attr_j
-00000ed0: 736f 6eda 215f 4c69 6e65 4368 6172 745f  son.!_LineChart_
-00000ee0: 5f68 6f72 697a 6f6e 7461 6c5f 6772 6964  _horizontal_grid
-00000ef0: 5f6c 696e 6573 da1f 5f4c 696e 6543 6861  _lines.._LineCha
-00000f00: 7274 5f5f 7665 7274 6963 616c 5f67 7269  rt__vertical_gri
-00000f10: 645f 6c69 6e65 73da 135f 4c69 6e65 4368  d_lines.._LineCh
-00000f20: 6172 745f 5f61 6e69 6d61 7465 da12 5f4c  art__animate.._L
-00000f30: 696e 6543 6861 7274 5f5f 626f 7264 6572  ineChart__border
-00000f40: 7253 0000 00a9 01da 095f 5f63 6c61 7373  rS.......__class
-00000f50: 5f5f 7249 0000 0072 4a00 0000 7258 0000  __rI...rJ...rX..
-00000f60: 008a 0000 0073 0a00 0000 0001 0a01 0e01  .....s..........
-00000f70: 0e01 0e01 7a17 4c69 6e65 4368 6172 742e  ....z.LineChart.
-00000f80: 6265 666f 7265 5f75 7064 6174 6563 0100  before_updatec..
-00000f90: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000fa0: 0000 4300 0000 739e 0000 0067 007d 017c  ..C...s....g.}.|
-00000fb0: 006a 0044 005d 0e7d 027c 01a0 017c 02a1  .j.D.].}.|...|..
-00000fc0: 0101 0071 0a7c 006a 0272 3a7c 006a 02a0  ...q.|.j.r:|.j..
-00000fd0: 0364 0164 02a1 0201 007c 01a0 017c 006a  .d.d.....|...|.j
-00000fe0: 02a1 0101 007c 006a 0472 5a7c 006a 04a0  .....|.j.rZ|.j..
-00000ff0: 0364 0164 03a1 0201 007c 01a0 017c 006a  .d.d.....|...|.j
-00001000: 04a1 0101 007c 006a 0572 7a7c 006a 05a0  .....|.j.rz|.j..
-00001010: 0364 0164 04a1 0201 007c 01a0 017c 006a  .d.d.....|...|.j
-00001020: 05a1 0101 007c 006a 0672 9a7c 006a 06a0  .....|.j.r.|.j..
-00001030: 0364 0164 05a1 0201 007c 01a0 017c 006a  .d.d.....|...|.j
-00001040: 06a1 0101 007c 0153 0029 064e da01 6eda  .....|.S.).N..n.
-00001050: 016c da01 74da 0172 da01 6229 07da 175f  .l..t..r..b)..._
-00001060: 4c69 6e65 4368 6172 745f 5f64 6174 615f  LineChart__data_
-00001070: 7365 7269 6573 da06 6170 7065 6e64 da15  series..append..
-00001080: 5f4c 696e 6543 6861 7274 5f5f 6c65 6674  _LineChart__left
-00001090: 5f61 7869 73da 125f 7365 745f 6174 7472  _axis.._set_attr
-000010a0: 5f69 6e74 6572 6e61 6cda 145f 4c69 6e65  _internal.._Line
-000010b0: 4368 6172 745f 5f74 6f70 5f61 7869 73da  Chart__top_axis.
-000010c0: 165f 4c69 6e65 4368 6172 745f 5f72 6967  ._LineChart__rig
-000010d0: 6874 5f61 7869 73da 175f 4c69 6e65 4368  ht_axis.._LineCh
-000010e0: 6172 745f 5f62 6f74 746f 6d5f 6178 6973  art__bottom_axis
-000010f0: 2903 7252 0000 00da 0863 6869 6c64 7265  ).rR.....childre
-00001100: 6eda 0264 7372 4900 0000 7249 0000 0072  n..dsrI...rI...r
-00001110: 4a00 0000 da0d 5f67 6574 5f63 6869 6c64  J....._get_child
-00001120: 7265 6e91 0000 0073 2000 0000 0001 0401  ren....s .......
-00001130: 0a01 0c01 0601 0e01 0c01 0601 0e01 0c01  ................
-00001140: 0601 0e01 0c01 0601 0e01 0c01 7a17 4c69  ............z.Li
-00001150: 6e65 4368 6172 742e 5f67 6574 5f63 6869  neChart._get_chi
-00001160: 6c64 7265 6e63 0100 0000 0000 0000 0000  ldrenc..........
-00001170: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00001180: 0000 007c 006a 0053 0072 4300 0000 a901  ...|.j.S.rC.....
-00001190: 7265 0000 0072 5300 0000 7249 0000 0072  re...rS...rI...r
-000011a0: 4900 0000 724a 0000 0072 1500 0000 a400  I...rJ...r......
-000011b0: 0000 7302 0000 0000 027a 154c 696e 6543  ..s......z.LineC
-000011c0: 6861 7274 2e64 6174 615f 7365 7269 6573  hart.data_series
-000011d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000011e0: 0002 0000 0043 0000 0073 1600 0000 7c01  .....C...s....|.
-000011f0: 6400 7501 720c 7c01 6e02 6700 7c00 5f00  d.u.r.|.n.g.|._.
-00001200: 6400 5300 7243 0000 0072 6f00 0000 a902  d.S.rC...ro.....
-00001210: 7252 0000 00da 0576 616c 7565 7249 0000  rR.....valuerI..
-00001220: 0072 4900 0000 724a 0000 0072 1500 0000  .rI...rJ...r....
-00001230: a800 0000 7302 0000 0000 02a9 01da 0672  ....s..........r
-00001240: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-00001250: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00001260: 0000 007c 006a 0053 0072 4300 0000 a901  ...|.j.S.rC.....
-00001270: 725c 0000 0072 5300 0000 7249 0000 0072  r\...rS...rI...r
-00001280: 4900 0000 724a 0000 0072 1600 0000 ad00  I...rJ...r......
-00001290: 0000 7302 0000 0000 027a 114c 696e 6543  ..s......z.LineC
-000012a0: 6861 7274 2e61 6e69 6d61 7465 2901 7271  hart.animate).rq
-000012b0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000012c0: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-000012d0: 007c 017c 005f 0064 0053 0072 4300 0000  .|.|._.d.S.rC...
-000012e0: 7274 0000 0072 7000 0000 7249 0000 0072  rt...rp...rI...r
-000012f0: 4900 0000 724a 0000 0072 1600 0000 b100  I...rJ...r......
-00001300: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
-00001310: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001320: 0000 730a 0000 007c 00a0 0064 01a1 0153  ..s....|...d...S
-00001330: 00a9 024e 721a 0000 00a9 01da 095f 6765  ...Nr........_ge
-00001340: 745f 6174 7472 7253 0000 0072 4900 0000  t_attrrS...rI...
-00001350: 7249 0000 0072 4a00 0000 721a 0000 00b6  rI...rJ...r.....
-00001360: 0000 0073 0200 0000 0002 7a11 4c69 6e65  ...s......z.Line
-00001370: 4368 6172 742e 6267 636f 6c6f 7263 0200  Chart.bgcolorc..
-00001380: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001390: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-000013a0: 017c 01a1 0201 0064 0053 0072 7500 0000  .|.....d.S.ru...
-000013b0: a901 da09 5f73 6574 5f61 7474 7272 7000  ...._set_attrrp.
-000013c0: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
-000013d0: 0072 1a00 0000 ba00 0000 7302 0000 0000  .r........s.....
-000013e0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-000013f0: 0000 0500 0000 4300 0000 7310 0000 007c  ......C...s....|
-00001400: 006a 0064 0164 0264 0364 048d 0353 0029  .j.d.d.d.d...S.)
-00001410: 054e 7217 0000 00da 0462 6f6f 6c54 2902  .Nr......boolT).
-00001420: da09 6461 7461 5f74 7970 65da 0964 6566  ..data_type..def
-00001430: 5f76 616c 7565 7276 0000 0072 5300 0000  _valuerv...rS...
-00001440: 7249 0000 0072 4900 0000 724a 0000 0072  rI...rI...rJ...r
-00001450: 1700 0000 bf00 0000 7302 0000 0000 027a  ........s......z
-00001460: 154c 696e 6543 6861 7274 2e69 6e74 6572  .LineChart.inter
-00001470: 6163 7469 7665 6302 0000 0000 0000 0000  activec.........
-00001480: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-00001490: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
-000014a0: 6400 5300 2902 4e72 1700 0000 7278 0000  d.S.).Nr....rx..
-000014b0: 0072 7000 0000 7249 0000 0072 4900 0000  .rp...rI...rI...
-000014c0: 724a 0000 0072 1700 0000 c300 0000 7302  rJ...r........s.
-000014d0: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-000014e0: 0000 0100 0000 0400 0000 4300 0000 730e  ..........C...s.
-000014f0: 0000 007c 006a 0064 0164 0264 038d 0253  ...|.j.d.d.d...S
-00001500: 0029 044e da0e 706f 696e 744c 696e 6553  .).N..pointLineS
-00001510: 7461 7274 da05 666c 6f61 74a9 0172 7b00  tart..float..r{.
-00001520: 0000 7276 0000 0072 5300 0000 7249 0000  ..rv...rS...rI..
-00001530: 0072 4900 0000 724a 0000 0072 1800 0000  .rI...rJ...r....
-00001540: c800 0000 7302 0000 0000 027a 1a4c 696e  ....s......z.Lin
-00001550: 6543 6861 7274 2e70 6f69 6e74 5f6c 696e  eChart.point_lin
-00001560: 655f 7374 6172 7463 0200 0000 0000 0000  e_startc........
-00001570: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001580: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00001590: 0064 0053 0029 024e 727d 0000 0072 7800  .d.S.).Nr}...rx.
-000015a0: 0000 7270 0000 0072 4900 0000 7249 0000  ..rp...rI...rI..
-000015b0: 0072 4a00 0000 7218 0000 00cc 0000 0073  .rJ...r........s
-000015c0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-000015d0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-000015e0: 0e00 0000 7c00 6a00 6401 6402 6403 8d02  ....|.j.d.d.d...
-000015f0: 5300 2904 4eda 0c70 6f69 6e74 4c69 6e65  S.).N..pointLine
-00001600: 456e 6472 7e00 0000 727f 0000 0072 7600  Endr~...r....rv.
-00001610: 0000 7253 0000 0072 4900 0000 7249 0000  ..rS...rI...rI..
-00001620: 0072 4a00 0000 7219 0000 00d1 0000 0073  .rJ...r........s
-00001630: 0200 0000 0002 7a18 4c69 6e65 4368 6172  ......z.LineChar
-00001640: 742e 706f 696e 745f 6c69 6e65 5f65 6e64  t.point_line_end
-00001650: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001660: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00001670: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
-00001680: 4e72 8000 0000 7278 0000 0072 7000 0000  Nr....rx...rp...
-00001690: 7249 0000 0072 4900 0000 724a 0000 0072  rI...rI...rJ...r
-000016a0: 1900 0000 d500 0000 7302 0000 0000 0263  ........s......c
-000016b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000016c0: 0300 0000 4300 0000 730a 0000 007c 00a0  ....C...s....|..
-000016d0: 0064 01a1 0153 00a9 024e da0e 746f 6f6c  .d...S...N..tool
-000016e0: 7469 7042 6763 6f6c 6f72 7276 0000 0072  tipBgcolorrv...r
-000016f0: 5300 0000 7249 0000 0072 4900 0000 724a  S...rI...rI...rJ
-00001700: 0000 0072 1b00 0000 da00 0000 7302 0000  ...r........s...
-00001710: 0000 027a 194c 696e 6543 6861 7274 2e74  ...z.LineChart.t
-00001720: 6f6f 6c74 6970 5f62 6763 6f6c 6f72 6302  ooltip_bgcolorc.
-00001730: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001740: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-00001750: 6401 7c01 a102 0100 6400 5300 7281 0000  d.|.....d.S.r...
-00001760: 0072 7800 0000 7270 0000 0072 4900 0000  .rx...rp...rI...
-00001770: 7249 0000 0072 4a00 0000 721b 0000 00de  rI...rJ...r.....
-00001780: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-00001790: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000017a0: 0000 0073 0600 0000 7c00 6a00 5300 7243  ...s....|.j.S.rC
-000017b0: 0000 00a9 0172 5d00 0000 7253 0000 0072  .....r]...rS...r
-000017c0: 4900 0000 7249 0000 0072 4a00 0000 721c  I...rI...rJ...r.
-000017d0: 0000 00e3 0000 0073 0200 0000 0002 7a10  .......s......z.
-000017e0: 4c69 6e65 4368 6172 742e 626f 7264 6572  LineChart.border
-000017f0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001800: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00001810: 7c00 5f00 6400 5300 7243 0000 0072 8300  |._.d.S.rC...r..
-00001820: 0000 7270 0000 0072 4900 0000 7249 0000  ..rp...rI...rI..
-00001830: 0072 4a00 0000 721c 0000 00e7 0000 0073  .rJ...r........s
-00001840: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00001850: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-00001860: 0600 0000 7c00 6a00 5300 7243 0000 00a9  ....|.j.S.rC....
-00001870: 0172 5a00 0000 7253 0000 0072 4900 0000  .rZ...rS...rI...
-00001880: 7249 0000 0072 4a00 0000 721d 0000 00ec  rI...rJ...r.....
-00001890: 0000 0073 0200 0000 0002 7a1f 4c69 6e65  ...s......z.Line
-000018a0: 4368 6172 742e 686f 7269 7a6f 6e74 616c  Chart.horizontal
-000018b0: 5f67 7269 645f 6c69 6e65 7363 0200 0000  _grid_linesc....
-000018c0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-000018d0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
-000018e0: 0053 0072 4300 0000 7284 0000 0072 7000  .S.rC...r....rp.
-000018f0: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
-00001900: 0072 1d00 0000 f000 0000 7302 0000 0000  .r........s.....
-00001910: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-00001920: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-00001930: 006a 0053 0072 4300 0000 a901 725b 0000  .j.S.rC.....r[..
-00001940: 0072 5300 0000 7249 0000 0072 4900 0000  .rS...rI...rI...
-00001950: 724a 0000 0072 1e00 0000 f500 0000 7302  rJ...r........s.
-00001960: 0000 0000 027a 1d4c 696e 6543 6861 7274  .....z.LineChart
-00001970: 2e76 6572 7469 6361 6c5f 6772 6964 5f6c  .vertical_grid_l
-00001980: 696e 6573 6302 0000 0000 0000 0000 0000  inesc...........
-00001990: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-000019a0: 0000 7c01 7c00 5f00 6400 5300 7243 0000  ..|.|._.d.S.rC..
-000019b0: 0072 8500 0000 7270 0000 0072 4900 0000  .r....rp...rI...
-000019c0: 7249 0000 0072 4a00 0000 721e 0000 00f9  rI...rJ...r.....
-000019d0: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-000019e0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000019f0: 0000 0073 0600 0000 7c00 6a00 5300 7243  ...s....|.j.S.rC
-00001a00: 0000 00a9 0172 6700 0000 7253 0000 0072  .....rg...rS...r
-00001a10: 4900 0000 7249 0000 0072 4a00 0000 721f  I...rI...rJ...r.
-00001a20: 0000 00fe 0000 0073 0200 0000 0002 7a13  .......s......z.
-00001a30: 4c69 6e65 4368 6172 742e 6c65 6674 5f61  LineChart.left_a
-00001a40: 7869 7363 0200 0000 0000 0000 0000 0000  xisc............
-00001a50: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-00001a60: 007c 017c 005f 0064 0053 0072 4300 0000  .|.|._.d.S.rC...
-00001a70: 7286 0000 0072 7000 0000 7249 0000 0072  r....rp...rI...r
-00001a80: 4900 0000 724a 0000 0072 1f00 0000 0201  I...rJ...r......
-00001a90: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
-00001aa0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00001ab0: 0000 7306 0000 007c 006a 0053 0072 4300  ..s....|.j.S.rC.
-00001ac0: 0000 a901 7269 0000 0072 5300 0000 7249  ....ri...rS...rI
-00001ad0: 0000 0072 4900 0000 724a 0000 0072 2000  ...rI...rJ...r .
-00001ae0: 0000 0701 0000 7302 0000 0000 027a 124c  ......s......z.L
-00001af0: 696e 6543 6861 7274 2e74 6f70 5f61 7869  ineChart.top_axi
-00001b00: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00001b10: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00001b20: 017c 005f 0064 0053 0072 4300 0000 7287  .|._.d.S.rC...r.
-00001b30: 0000 0072 7000 0000 7249 0000 0072 4900  ...rp...rI...rI.
-00001b40: 0000 724a 0000 0072 2000 0000 0b01 0000  ..rJ...r .......
-00001b50: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00001b60: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00001b70: 7306 0000 007c 006a 0053 0072 4300 0000  s....|.j.S.rC...
-00001b80: a901 726a 0000 0072 5300 0000 7249 0000  ..rj...rS...rI..
-00001b90: 0072 4900 0000 724a 0000 0072 2100 0000  .rI...rJ...r!...
-00001ba0: 1001 0000 7302 0000 0000 027a 144c 696e  ....s......z.Lin
-00001bb0: 6543 6861 7274 2e72 6967 6874 5f61 7869  eChart.right_axi
-00001bc0: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00001bd0: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00001be0: 017c 005f 0064 0053 0072 4300 0000 7288  .|._.d.S.rC...r.
-00001bf0: 0000 0072 7000 0000 7249 0000 0072 4900  ...rp...rI...rI.
-00001c00: 0000 724a 0000 0072 2100 0000 1401 0000  ..rJ...r!.......
-00001c10: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00001c20: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00001c30: 7306 0000 007c 006a 0053 0072 4300 0000  s....|.j.S.rC...
-00001c40: a901 726b 0000 0072 5300 0000 7249 0000  ..rk...rS...rI..
-00001c50: 0072 4900 0000 724a 0000 0072 2200 0000  .rI...rJ...r"...
-00001c60: 1901 0000 7302 0000 0000 027a 154c 696e  ....s......z.Lin
-00001c70: 6543 6861 7274 2e62 6f74 746f 6d5f 6178  eChart.bottom_ax
-00001c80: 6973 6302 0000 0000 0000 0000 0000 0002  isc.............
-00001c90: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00001ca0: 7c01 7c00 5f00 6400 5300 7243 0000 0072  |.|._.d.S.rC...r
-00001cb0: 8900 0000 7270 0000 0072 4900 0000 7249  ....rp...rI...rI
-00001cc0: 0000 0072 4a00 0000 7222 0000 001d 0100  ...rJ...r"......
-00001cd0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00001ce0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00001cf0: 0073 0e00 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
-00001d00: 8d02 5300 2904 4eda 0962 6173 656c 696e  ..S.).N..baselin
-00001d10: 6578 727e 0000 0072 7f00 0000 7276 0000  exr~...r....rv..
-00001d20: 0072 5300 0000 7249 0000 0072 4900 0000  .rS...rI...rI...
-00001d30: 724a 0000 0072 2300 0000 2201 0000 7302  rJ...r#..."...s.
-00001d40: 0000 0000 027a 144c 696e 6543 6861 7274  .....z.LineChart
-00001d50: 2e62 6173 656c 696e 655f 7863 0200 0000  .baseline_xc....
-00001d60: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001d70: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
-00001d80: 01a1 0201 0064 0053 0029 024e 728a 0000  .....d.S.).Nr...
-00001d90: 0072 7800 0000 7270 0000 0072 4900 0000  .rx...rp...rI...
-00001da0: 7249 0000 0072 4a00 0000 7223 0000 0026  rI...rJ...r#...&
-00001db0: 0100 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-00001dc0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00001dd0: 0000 0073 0e00 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
-00001de0: 6403 8d02 5300 2904 4eda 0962 6173 656c  d...S.).N..basel
-00001df0: 696e 6579 727e 0000 0072 7f00 0000 7276  ineyr~...r....rv
-00001e00: 0000 0072 5300 0000 7249 0000 0072 4900  ...rS...rI...rI.
-00001e10: 0000 724a 0000 0072 2600 0000 2b01 0000  ..rJ...r&...+...
-00001e20: 7302 0000 0000 027a 144c 696e 6543 6861  s......z.LineCha
-00001e30: 7274 2e62 6173 656c 696e 655f 7963 0200  rt.baseline_yc..
-00001e40: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001e50: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-00001e60: 017c 01a1 0201 0064 0053 0029 024e 728b  .|.....d.S.).Nr.
-00001e70: 0000 0072 7800 0000 7270 0000 0072 4900  ...rx...rp...rI.
-00001e80: 0000 7249 0000 0072 4a00 0000 7226 0000  ..rI...rJ...r&..
-00001e90: 002f 0100 0073 0200 0000 0002 6301 0000  ./...s......c...
-00001ea0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00001eb0: 0043 0000 0073 0e00 0000 7c00 6a00 6401  .C...s....|.j.d.
-00001ec0: 6402 6403 8d02 5300 2904 4eda 046d 696e  d.d...S.).N..min
-00001ed0: 7872 7e00 0000 727f 0000 0072 7600 0000  xr~...r....rv...
-00001ee0: 7253 0000 0072 4900 0000 7249 0000 0072  rS...rI...rI...r
-00001ef0: 4a00 0000 7224 0000 0034 0100 0073 0200  J...r$...4...s..
-00001f00: 0000 0002 7a0f 4c69 6e65 4368 6172 742e  ....z.LineChart.
-00001f10: 6d69 6e5f 7863 0200 0000 0000 0000 0000  min_xc..........
-00001f20: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
-00001f30: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
-00001f40: 0053 0029 024e 728c 0000 0072 7800 0000  .S.).Nr....rx...
-00001f50: 7270 0000 0072 4900 0000 7249 0000 0072  rp...rI...rI...r
-00001f60: 4a00 0000 7224 0000 0038 0100 0073 0200  J...r$...8...s..
-00001f70: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00001f80: 0001 0000 0004 0000 0043 0000 0073 0e00  .........C...s..
-00001f90: 0000 7c00 6a00 6401 6402 6403 8d02 5300  ..|.j.d.d.d...S.
-00001fa0: 2904 4eda 046d 6178 7872 7e00 0000 727f  ).N..maxxr~...r.
-00001fb0: 0000 0072 7600 0000 7253 0000 0072 4900  ...rv...rS...rI.
-00001fc0: 0000 7249 0000 0072 4a00 0000 7225 0000  ..rI...rJ...r%..
-00001fd0: 003d 0100 0073 0200 0000 0002 7a0f 4c69  .=...s......z.Li
-00001fe0: 6e65 4368 6172 742e 6d61 785f 7863 0200  neChart.max_xc..
-00001ff0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00002000: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-00002010: 017c 01a1 0201 0064 0053 0029 024e 728d  .|.....d.S.).Nr.
-00002020: 0000 0072 7800 0000 7270 0000 0072 4900  ...rx...rp...rI.
-00002030: 0000 7249 0000 0072 4a00 0000 7225 0000  ..rI...rJ...r%..
-00002040: 0041 0100 0073 0200 0000 0002 6301 0000  .A...s......c...
-00002050: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00002060: 0043 0000 0073 0e00 0000 7c00 6a00 6401  .C...s....|.j.d.
-00002070: 6402 6403 8d02 5300 2904 4eda 046d 696e  d.d...S.).N..min
-00002080: 7972 7e00 0000 727f 0000 0072 7600 0000  yr~...r....rv...
-00002090: 7253 0000 0072 4900 0000 7249 0000 0072  rS...rI...rI...r
-000020a0: 4a00 0000 7227 0000 0046 0100 0073 0200  J...r'...F...s..
-000020b0: 0000 0002 7a0f 4c69 6e65 4368 6172 742e  ....z.LineChart.
-000020c0: 6d69 6e5f 7963 0200 0000 0000 0000 0000  min_yc..........
-000020d0: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
-000020e0: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
-000020f0: 0053 0029 024e 728e 0000 0072 7800 0000  .S.).Nr....rx...
-00002100: 7270 0000 0072 4900 0000 7249 0000 0072  rp...rI...rI...r
-00002110: 4a00 0000 7227 0000 004a 0100 0073 0200  J...r'...J...s..
-00002120: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00002130: 0001 0000 0004 0000 0043 0000 0073 0e00  .........C...s..
-00002140: 0000 7c00 6a00 6401 6402 6403 8d02 5300  ..|.j.d.d.d...S.
-00002150: 2904 4eda 046d 6178 7972 7e00 0000 727f  ).N..maxyr~...r.
-00002160: 0000 0072 7600 0000 7253 0000 0072 4900  ...rv...rS...rI.
-00002170: 0000 7249 0000 0072 4a00 0000 7228 0000  ..rI...rJ...r(..
-00002180: 004f 0100 0073 0200 0000 0002 7a0f 4c69  .O...s......z.Li
-00002190: 6e65 4368 6172 742e 6d61 785f 7963 0200  neChart.max_yc..
-000021a0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000021b0: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-000021c0: 017c 01a1 0201 0064 0053 0029 024e 728f  .|.....d.S.).Nr.
-000021d0: 0000 0072 7800 0000 7270 0000 0072 4900  ...rx...rp...rI.
-000021e0: 0000 7249 0000 0072 4a00 0000 7228 0000  ..rI...rJ...r(..
-000021f0: 0053 0100 0073 0200 0000 0002 6301 0000  .S...s......c...
-00002200: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00002210: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00002220: 7243 0000 0029 0172 4e00 0000 7253 0000  rC...).rN...rS..
-00002230: 0072 4900 0000 7249 0000 0072 4a00 0000  .rI...rI...rJ...
-00002240: 7251 0000 0058 0100 0073 0200 0000 0002  rQ...X...s......
-00002250: 7a18 4c69 6e65 4368 6172 742e 6f6e 5f63  z.LineChart.on_c
-00002260: 6861 7274 5f65 7665 6e74 6302 0000 0000  hart_eventc.....
-00002270: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00002280: 0000 0073 3200 0000 7c00 6a00 a001 7c01  ...s2...|.j...|.
-00002290: a101 0100 7c01 6400 7501 7222 7c00 a002  ....|.d.u.r"|...
-000022a0: 6401 6402 a102 0100 6e0c 7c00 a002 6401  d.d.....n.|...d.
-000022b0: 6400 a102 0100 6400 5300 2903 4eda 0c6f  d.....d.S.).N..o
-000022c0: 6e43 6861 7274 4576 656e 7454 2903 724e  nChartEventT).rN
-000022d0: 0000 00da 0973 7562 7363 7269 6265 7279  .....subscribery
-000022e0: 0000 0029 0272 5200 0000 da07 6861 6e64  ...).rR.....hand
-000022f0: 6c65 7272 4900 0000 7249 0000 0072 4a00  lerrI...rI...rJ.
-00002300: 0000 7251 0000 005c 0100 0073 0800 0000  ..rQ...\...s....
-00002310: 0002 0c01 0801 0e02 292f 4e4e 4e4e 4e4e  ........)/NNNNNN
-00002320: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
+00000a60: 00fa 642f 776f 726b 7370 6163 6573 2f63  ..d/workspaces/c
+00000a70: 6f6e 7472 6962 666c 6574 2f66 6c65 7463  ontribflet/fletc
+00000a80: 6f6e 7472 6962 2f73 646b 2f70 7974 686f  ontrib/sdk/pytho
+00000a90: 6e2f 7061 636b 6167 6573 2f66 6c65 742d  n/packages/flet-
+00000aa0: 636f 7265 2f73 7263 2f66 6c65 745f 636f  core/src/flet_co
+00000ab0: 7265 2f63 6861 7274 732f 6c69 6e65 5f63  re/charts/line_c
+00000ac0: 6861 7274 2e70 79da 1c63 6f6e 7665 7274  hart.py..convert
+00000ad0: 5f6c 696e 6563 6861 7274 5f65 7665 6e74  _linechart_event
+00000ae0: 5f64 6174 616a 0000 0073 0400 0000 0001  _dataj...s......
+00000af0: 0c01 7a38 4c69 6e65 4368 6172 742e 5f5f  ..z8LineChart.__
+00000b00: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00000b10: 636f 6e76 6572 745f 6c69 6e65 6368 6172  convert_linechar
+00000b20: 745f 6576 656e 745f 6461 7461 da0b 6368  t_event_data..ch
+00000b30: 6172 745f 6576 656e 7429 1b72 0a00 0000  art_event).r....
+00000b40: da08 5f5f 696e 6974 5f5f 720d 0000 00da  ..__init__r.....
+00000b50: 1a5f 4c69 6e65 4368 6172 745f 5f6f 6e5f  ._LineChart__on_
+00000b60: 6368 6172 745f 6576 656e 74da 125f 6164  chart_event.._ad
+00000b70: 645f 6576 656e 745f 6861 6e64 6c65 72da  d_event_handler.
+00000b80: 0b67 6574 5f68 616e 646c 6572 7215 0000  .get_handlerr...
+00000b90: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000ba0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000bb0: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
+00000bc0: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
+00000bd0: 0000 7223 0000 0072 2600 0000 7224 0000  ..r#...r&...r$..
+00000be0: 0072 2500 0000 7227 0000 0072 2800 0000  .r%...r'...r(...
+00000bf0: da0e 6f6e 5f63 6861 7274 5f65 7665 6e74  ..on_chart_event
+00000c00: 2931 da04 7365 6c66 7215 0000 0072 1600  )1..selfr....r..
+00000c10: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000c20: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000c30: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000c40: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
+00000c50: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
+00000c60: 0000 7227 0000 0072 2800 0000 7251 0000  ..r'...r(...rQ..
+00000c70: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
+00000c80: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
+00000c90: 2f00 0000 7230 0000 0072 3100 0000 7232  /...r0...r1...r2
+00000ca0: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
+00000cb0: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
+00000cc0: 0072 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
+00000cd0: 723c 0000 0072 3d00 0000 7242 0000 0072  r<...r=...rB...r
+00000ce0: 3e00 0000 723f 0000 0072 4000 0000 7241  >...r?...r@...rA
+00000cf0: 0000 0072 4b00 0000 7249 0000 0072 4900  ...rK...rI...rI.
+00000d00: 0000 724a 0000 0072 4d00 0000 1700 0000  ..rJ...rM.......
+00000d10: 736a 0000 0000 3504 0102 0102 0102 0102  sj....5.........
+00000d20: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000d30: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000d40: 0102 0102 0102 0102 0102 0102 0102 e506  ................
+00000d50: 1e08 040a 0112 0206 0106 0106 0106 0106  ................
+00000d60: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00000d70: 0106 0106 0106 0106 0106 0106 0106 017a  ...............z
+00000d80: 124c 696e 6543 6861 7274 2e5f 5f69 6e69  .LineChart.__ini
+00000d90: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00000da0: 0100 0000 0100 0000 4300 0000 7304 0000  ........C...s...
+00000db0: 0064 0153 0029 024e 5a09 6c69 6e65 6368  .d.S.).NZ.linech
+00000dc0: 6172 7472 4900 0000 a901 7252 0000 0072  artrI.....rR...r
+00000dd0: 4900 0000 7249 0000 0072 4a00 0000 da11  I...rI...rJ.....
+00000de0: 5f67 6574 5f63 6f6e 7472 6f6c 5f6e 616d  _get_control_nam
+00000df0: 6587 0000 0073 0200 0000 0001 7a1b 4c69  e....s......z.Li
+00000e00: 6e65 4368 6172 742e 5f67 6574 5f63 6f6e  neChart._get_con
+00000e10: 7472 6f6c 5f6e 616d 6563 0100 0000 0000  trol_namec......
+00000e20: 0000 0000 0000 0100 0000 0400 0000 0300  ................
+00000e30: 0000 7346 0000 0074 0083 00a0 01a1 0001  ..sF...t........
+00000e40: 007c 00a0 0264 017c 006a 03a1 0201 007c  .|...d.|.j.....|
+00000e50: 00a0 0264 027c 006a 04a1 0201 007c 00a0  ...d.|.j.....|..
+00000e60: 0264 037c 006a 05a1 0201 007c 00a0 0264  .d.|.j.....|...d
+00000e70: 047c 006a 06a1 0201 0064 0053 0029 054e  .|.j.....d.S.).N
+00000e80: da13 686f 7269 7a6f 6e74 616c 4772 6964  ..horizontalGrid
+00000e90: 4c69 6e65 73da 1176 6572 7469 6361 6c47  Lines..verticalG
+00000ea0: 7269 644c 696e 6573 7216 0000 0072 1c00  ridLinesr....r..
+00000eb0: 0000 2907 da05 7375 7065 72da 0d62 6566  ..)...super..bef
+00000ec0: 6f72 655f 7570 6461 7465 da0e 5f73 6574  ore_update.._set
+00000ed0: 5f61 7474 725f 6a73 6f6e da21 5f4c 696e  _attr_json.!_Lin
+00000ee0: 6543 6861 7274 5f5f 686f 7269 7a6f 6e74  eChart__horizont
+00000ef0: 616c 5f67 7269 645f 6c69 6e65 73da 1f5f  al_grid_lines.._
+00000f00: 4c69 6e65 4368 6172 745f 5f76 6572 7469  LineChart__verti
+00000f10: 6361 6c5f 6772 6964 5f6c 696e 6573 da13  cal_grid_lines..
+00000f20: 5f4c 696e 6543 6861 7274 5f5f 616e 696d  _LineChart__anim
+00000f30: 6174 65da 125f 4c69 6e65 4368 6172 745f  ate.._LineChart_
+00000f40: 5f62 6f72 6465 7272 5300 0000 a901 da09  _borderrS.......
+00000f50: 5f5f 636c 6173 735f 5f72 4900 0000 724a  __class__rI...rJ
+00000f60: 0000 0072 5800 0000 8a00 0000 730a 0000  ...rX.......s...
+00000f70: 0000 010a 010e 010e 010e 017a 174c 696e  ...........z.Lin
+00000f80: 6543 6861 7274 2e62 6566 6f72 655f 7570  eChart.before_up
+00000f90: 6461 7465 6301 0000 0000 0000 0000 0000  datec...........
+00000fa0: 0003 0000 0004 0000 0043 0000 0073 9e00  .........C...s..
+00000fb0: 0000 6700 7d01 7c00 6a00 4400 5d0e 7d02  ..g.}.|.j.D.].}.
+00000fc0: 7c01 a001 7c02 a101 0100 710a 7c00 6a02  |...|.....q.|.j.
+00000fd0: 723a 7c00 6a02 a003 6401 6402 a102 0100  r:|.j...d.d.....
+00000fe0: 7c01 a001 7c00 6a02 a101 0100 7c00 6a04  |...|.j.....|.j.
+00000ff0: 725a 7c00 6a04 a003 6401 6403 a102 0100  rZ|.j...d.d.....
+00001000: 7c01 a001 7c00 6a04 a101 0100 7c00 6a05  |...|.j.....|.j.
+00001010: 727a 7c00 6a05 a003 6401 6404 a102 0100  rz|.j...d.d.....
+00001020: 7c01 a001 7c00 6a05 a101 0100 7c00 6a06  |...|.j.....|.j.
+00001030: 729a 7c00 6a06 a003 6401 6405 a102 0100  r.|.j...d.d.....
+00001040: 7c01 a001 7c00 6a06 a101 0100 7c01 5300  |...|.j.....|.S.
+00001050: 2906 4eda 016e da01 6cda 0174 da01 72da  ).N..n..l..t..r.
+00001060: 0162 2907 da17 5f4c 696e 6543 6861 7274  .b)..._LineChart
+00001070: 5f5f 6461 7461 5f73 6572 6965 73da 0661  __data_series..a
+00001080: 7070 656e 64da 155f 4c69 6e65 4368 6172  ppend.._LineChar
+00001090: 745f 5f6c 6566 745f 6178 6973 da12 5f73  t__left_axis.._s
+000010a0: 6574 5f61 7474 725f 696e 7465 726e 616c  et_attr_internal
+000010b0: da14 5f4c 696e 6543 6861 7274 5f5f 746f  .._LineChart__to
+000010c0: 705f 6178 6973 da16 5f4c 696e 6543 6861  p_axis.._LineCha
+000010d0: 7274 5f5f 7269 6768 745f 6178 6973 da17  rt__right_axis..
+000010e0: 5f4c 696e 6543 6861 7274 5f5f 626f 7474  _LineChart__bott
+000010f0: 6f6d 5f61 7869 7329 0372 5200 0000 da08  om_axis).rR.....
+00001100: 6368 696c 6472 656e da02 6473 7249 0000  children..dsrI..
+00001110: 0072 4900 0000 724a 0000 00da 0d5f 6765  .rI...rJ....._ge
+00001120: 745f 6368 696c 6472 656e 9100 0000 7320  t_children....s 
+00001130: 0000 0000 0104 010a 010c 0106 010e 010c  ................
+00001140: 0106 010e 010c 0106 010e 010c 0106 010e  ................
+00001150: 010c 017a 174c 696e 6543 6861 7274 2e5f  ...z.LineChart._
+00001160: 6765 745f 6368 696c 6472 656e 6301 0000  get_childrenc...
+00001170: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00001180: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00001190: 7243 0000 00a9 0172 6500 0000 7253 0000  rC.....re...rS..
+000011a0: 0072 4900 0000 7249 0000 0072 4a00 0000  .rI...rI...rJ...
+000011b0: 7215 0000 00a4 0000 0073 0200 0000 0002  r........s......
+000011c0: 7a15 4c69 6e65 4368 6172 742e 6461 7461  z.LineChart.data
+000011d0: 5f73 6572 6965 7363 0200 0000 0000 0000  _seriesc........
+000011e0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+000011f0: 7316 0000 007c 0164 0075 0172 0c7c 016e  s....|.d.u.r.|.n
+00001200: 0267 007c 005f 0064 0053 0072 4300 0000  .g.|._.d.S.rC...
+00001210: 726f 0000 00a9 0272 5200 0000 da05 7661  ro.....rR.....va
+00001220: 6c75 6572 4900 0000 7249 0000 0072 4a00  luerI...rI...rJ.
+00001230: 0000 7215 0000 00a8 0000 0073 0200 0000  ..r........s....
+00001240: 0002 a901 da06 7265 7475 726e 6301 0000  ......returnc...
+00001250: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00001260: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00001270: 7243 0000 00a9 0172 5c00 0000 7253 0000  rC.....r\...rS..
+00001280: 0072 4900 0000 7249 0000 0072 4a00 0000  .rI...rI...rJ...
+00001290: 7216 0000 00ad 0000 0073 0200 0000 0002  r........s......
+000012a0: 7a11 4c69 6e65 4368 6172 742e 616e 696d  z.LineChart.anim
+000012b0: 6174 6529 0172 7100 0000 6302 0000 0000  ate).rq...c.....
+000012c0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+000012d0: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
+000012e0: 5300 7243 0000 0072 7400 0000 7270 0000  S.rC...rt...rp..
+000012f0: 0072 4900 0000 7249 0000 0072 4a00 0000  .rI...rI...rJ...
+00001300: 7216 0000 00b1 0000 0073 0200 0000 0002  r........s......
+00001310: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001320: 0003 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
+00001330: a000 6401 a101 5300 a902 4e72 1a00 0000  ..d...S...Nr....
+00001340: a901 da09 5f67 6574 5f61 7474 7272 5300  ...._get_attrrS.
+00001350: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
+00001360: 0072 1a00 0000 b600 0000 7302 0000 0000  .r........s.....
+00001370: 027a 114c 696e 6543 6861 7274 2e62 6763  .z.LineChart.bgc
+00001380: 6f6c 6f72 6302 0000 0000 0000 0000 0000  olorc...........
+00001390: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+000013a0: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+000013b0: 5300 7275 0000 00a9 01da 095f 7365 745f  S.ru......._set_
+000013c0: 6174 7472 7270 0000 0072 4900 0000 7249  attrrp...rI...rI
+000013d0: 0000 0072 4a00 0000 721a 0000 00ba 0000  ...rJ...r.......
+000013e0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
+000013f0: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00001400: 0073 1000 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
+00001410: 6404 8d03 5300 2905 4e72 1700 0000 da04  d...S.).Nr......
+00001420: 626f 6f6c 5429 02da 0964 6174 615f 7479  boolT)...data_ty
+00001430: 7065 da09 6465 665f 7661 6c75 6572 7600  pe..def_valuerv.
+00001440: 0000 7253 0000 0072 4900 0000 7249 0000  ..rS...rI...rI..
+00001450: 0072 4a00 0000 7217 0000 00bf 0000 0073  .rJ...r........s
+00001460: 0200 0000 0002 7a15 4c69 6e65 4368 6172  ......z.LineChar
+00001470: 742e 696e 7465 7261 6374 6976 6563 0200  t.interactivec..
+00001480: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001490: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
+000014a0: 017c 01a1 0201 0064 0053 0029 024e 7217  .|.....d.S.).Nr.
+000014b0: 0000 0072 7800 0000 7270 0000 0072 4900  ...rx...rp...rI.
+000014c0: 0000 7249 0000 0072 4a00 0000 7217 0000  ..rI...rJ...r...
+000014d0: 00c3 0000 0073 0200 0000 0002 6301 0000  .....s......c...
+000014e0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+000014f0: 0043 0000 0073 0e00 0000 7c00 6a00 6401  .C...s....|.j.d.
+00001500: 6402 6403 8d02 5300 2904 4eda 0e70 6f69  d.d...S.).N..poi
+00001510: 6e74 4c69 6e65 5374 6172 74da 0566 6c6f  ntLineStart..flo
+00001520: 6174 a901 727b 0000 0072 7600 0000 7253  at..r{...rv...rS
+00001530: 0000 0072 4900 0000 7249 0000 0072 4a00  ...rI...rI...rJ.
+00001540: 0000 7218 0000 00c8 0000 0073 0200 0000  ..r........s....
+00001550: 0002 7a1a 4c69 6e65 4368 6172 742e 706f  ..z.LineChart.po
+00001560: 696e 745f 6c69 6e65 5f73 7461 7274 6302  int_line_startc.
+00001570: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001580: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00001590: 6401 7c01 a102 0100 6400 5300 2902 4e72  d.|.....d.S.).Nr
+000015a0: 7d00 0000 7278 0000 0072 7000 0000 7249  }...rx...rp...rI
+000015b0: 0000 0072 4900 0000 724a 0000 0072 1800  ...rI...rJ...r..
+000015c0: 0000 cc00 0000 7302 0000 0000 0263 0100  ......s......c..
+000015d0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+000015e0: 0000 4300 0000 730e 0000 007c 006a 0064  ..C...s....|.j.d
+000015f0: 0164 0264 038d 0253 0029 044e da0c 706f  .d.d...S.).N..po
+00001600: 696e 744c 696e 6545 6e64 727e 0000 0072  intLineEndr~...r
+00001610: 7f00 0000 7276 0000 0072 5300 0000 7249  ....rv...rS...rI
+00001620: 0000 0072 4900 0000 724a 0000 0072 1900  ...rI...rJ...r..
+00001630: 0000 d100 0000 7302 0000 0000 027a 184c  ......s......z.L
+00001640: 696e 6543 6861 7274 2e70 6f69 6e74 5f6c  ineChart.point_l
+00001650: 696e 655f 656e 6463 0200 0000 0000 0000  ine_endc........
+00001660: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00001670: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
+00001680: 0064 0053 0029 024e 7280 0000 0072 7800  .d.S.).Nr....rx.
+00001690: 0000 7270 0000 0072 4900 0000 7249 0000  ..rp...rI...rI..
+000016a0: 0072 4a00 0000 7219 0000 00d5 0000 0073  .rJ...r........s
+000016b0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
+000016c0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+000016d0: 0a00 0000 7c00 a000 6401 a101 5300 a902  ....|...d...S...
+000016e0: 4eda 0e74 6f6f 6c74 6970 4267 636f 6c6f  N..tooltipBgcolo
+000016f0: 7272 7600 0000 7253 0000 0072 4900 0000  rrv...rS...rI...
+00001700: 7249 0000 0072 4a00 0000 721b 0000 00da  rI...rJ...r.....
+00001710: 0000 0073 0200 0000 0002 7a19 4c69 6e65  ...s......z.Line
+00001720: 4368 6172 742e 746f 6f6c 7469 705f 6267  Chart.tooltip_bg
+00001730: 636f 6c6f 7263 0200 0000 0000 0000 0000  colorc..........
+00001740: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+00001750: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+00001760: 0053 0072 8100 0000 7278 0000 0072 7000  .S.r....rx...rp.
+00001770: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
+00001780: 0072 1b00 0000 de00 0000 7302 0000 0000  .r........s.....
+00001790: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+000017a0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+000017b0: 006a 0053 0072 4300 0000 a901 725d 0000  .j.S.rC.....r]..
+000017c0: 0072 5300 0000 7249 0000 0072 4900 0000  .rS...rI...rI...
+000017d0: 724a 0000 0072 1c00 0000 e300 0000 7302  rJ...r........s.
+000017e0: 0000 0000 027a 104c 696e 6543 6861 7274  .....z.LineChart
+000017f0: 2e62 6f72 6465 7263 0200 0000 0000 0000  .borderc........
+00001800: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00001810: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
+00001820: 4300 0000 7283 0000 0072 7000 0000 7249  C...r....rp...rI
+00001830: 0000 0072 4900 0000 724a 0000 0072 1c00  ...rI...rJ...r..
+00001840: 0000 e700 0000 7302 0000 0000 0263 0100  ......s......c..
+00001850: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00001860: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00001870: 0072 4300 0000 a901 725a 0000 0072 5300  .rC.....rZ...rS.
+00001880: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
+00001890: 0072 1d00 0000 ec00 0000 7302 0000 0000  .r........s.....
+000018a0: 027a 1f4c 696e 6543 6861 7274 2e68 6f72  .z.LineChart.hor
+000018b0: 697a 6f6e 7461 6c5f 6772 6964 5f6c 696e  izontal_grid_lin
+000018c0: 6573 6302 0000 0000 0000 0000 0000 0002  esc.............
+000018d0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+000018e0: 7c01 7c00 5f00 6400 5300 7243 0000 0072  |.|._.d.S.rC...r
+000018f0: 8400 0000 7270 0000 0072 4900 0000 7249  ....rp...rI...rI
+00001900: 0000 0072 4a00 0000 721d 0000 00f0 0000  ...rJ...r.......
+00001910: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
+00001920: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00001930: 0073 0600 0000 7c00 6a00 5300 7243 0000  .s....|.j.S.rC..
+00001940: 00a9 0172 5b00 0000 7253 0000 0072 4900  ...r[...rS...rI.
+00001950: 0000 7249 0000 0072 4a00 0000 721e 0000  ..rI...rJ...r...
+00001960: 00f5 0000 0073 0200 0000 0002 7a1d 4c69  .....s......z.Li
+00001970: 6e65 4368 6172 742e 7665 7274 6963 616c  neChart.vertical
+00001980: 5f67 7269 645f 6c69 6e65 7363 0200 0000  _grid_linesc....
+00001990: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+000019a0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+000019b0: 0053 0072 4300 0000 7285 0000 0072 7000  .S.rC...r....rp.
+000019c0: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
+000019d0: 0072 1e00 0000 f900 0000 7302 0000 0000  .r........s.....
+000019e0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+000019f0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00001a00: 006a 0053 0072 4300 0000 a901 7267 0000  .j.S.rC.....rg..
+00001a10: 0072 5300 0000 7249 0000 0072 4900 0000  .rS...rI...rI...
+00001a20: 724a 0000 0072 1f00 0000 fe00 0000 7302  rJ...r........s.
+00001a30: 0000 0000 027a 134c 696e 6543 6861 7274  .....z.LineChart
+00001a40: 2e6c 6566 745f 6178 6973 6302 0000 0000  .left_axisc.....
+00001a50: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00001a60: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
+00001a70: 5300 7243 0000 0072 8600 0000 7270 0000  S.rC...r....rp..
+00001a80: 0072 4900 0000 7249 0000 0072 4a00 0000  .rI...rI...rJ...
+00001a90: 721f 0000 0002 0100 0073 0200 0000 0002  r........s......
+00001aa0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001ab0: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+00001ac0: 6a00 5300 7243 0000 00a9 0172 6900 0000  j.S.rC.....ri...
+00001ad0: 7253 0000 0072 4900 0000 7249 0000 0072  rS...rI...rI...r
+00001ae0: 4a00 0000 7220 0000 0007 0100 0073 0200  J...r .......s..
+00001af0: 0000 0002 7a12 4c69 6e65 4368 6172 742e  ....z.LineChart.
+00001b00: 746f 705f 6178 6973 6302 0000 0000 0000  top_axisc.......
+00001b10: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00001b20: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00001b30: 7243 0000 0072 8700 0000 7270 0000 0072  rC...r....rp...r
+00001b40: 4900 0000 7249 0000 0072 4a00 0000 7220  I...rI...rJ...r 
+00001b50: 0000 000b 0100 0073 0200 0000 0002 6301  .......s......c.
+00001b60: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00001b70: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+00001b80: 5300 7243 0000 00a9 0172 6a00 0000 7253  S.rC.....rj...rS
+00001b90: 0000 0072 4900 0000 7249 0000 0072 4a00  ...rI...rI...rJ.
+00001ba0: 0000 7221 0000 0010 0100 0073 0200 0000  ..r!.......s....
+00001bb0: 0002 7a14 4c69 6e65 4368 6172 742e 7269  ..z.LineChart.ri
+00001bc0: 6768 745f 6178 6973 6302 0000 0000 0000  ght_axisc.......
+00001bd0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00001be0: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00001bf0: 7243 0000 0072 8800 0000 7270 0000 0072  rC...r....rp...r
+00001c00: 4900 0000 7249 0000 0072 4a00 0000 7221  I...rI...rJ...r!
+00001c10: 0000 0014 0100 0073 0200 0000 0002 6301  .......s......c.
+00001c20: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00001c30: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+00001c40: 5300 7243 0000 00a9 0172 6b00 0000 7253  S.rC.....rk...rS
+00001c50: 0000 0072 4900 0000 7249 0000 0072 4a00  ...rI...rI...rJ.
+00001c60: 0000 7222 0000 0019 0100 0073 0200 0000  ..r".......s....
+00001c70: 0002 7a15 4c69 6e65 4368 6172 742e 626f  ..z.LineChart.bo
+00001c80: 7474 6f6d 5f61 7869 7363 0200 0000 0000  ttom_axisc......
+00001c90: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00001ca0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+00001cb0: 0072 4300 0000 7289 0000 0072 7000 0000  .rC...r....rp...
+00001cc0: 7249 0000 0072 4900 0000 724a 0000 0072  rI...rI...rJ...r
+00001cd0: 2200 0000 1d01 0000 7302 0000 0000 0263  ".......s......c
+00001ce0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001cf0: 0400 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+00001d00: 0064 0164 0264 038d 0253 0029 044e da09  .d.d.d...S.).N..
+00001d10: 6261 7365 6c69 6e65 7872 7e00 0000 727f  baselinexr~...r.
+00001d20: 0000 0072 7600 0000 7253 0000 0072 4900  ...rv...rS...rI.
+00001d30: 0000 7249 0000 0072 4a00 0000 7223 0000  ..rI...rJ...r#..
+00001d40: 0022 0100 0073 0200 0000 0002 7a14 4c69  ."...s......z.Li
+00001d50: 6e65 4368 6172 742e 6261 7365 6c69 6e65  neChart.baseline
+00001d60: 5f78 6302 0000 0000 0000 0000 0000 0002  _xc.............
+00001d70: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
+00001d80: 7c00 a000 6401 7c01 a102 0100 6400 5300  |...d.|.....d.S.
+00001d90: 2902 4e72 8a00 0000 7278 0000 0072 7000  ).Nr....rx...rp.
+00001da0: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
+00001db0: 0072 2300 0000 2601 0000 7302 0000 0000  .r#...&...s.....
+00001dc0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001dd0: 0000 0400 0000 4300 0000 730e 0000 007c  ......C...s....|
+00001de0: 006a 0064 0164 0264 038d 0253 0029 044e  .j.d.d.d...S.).N
+00001df0: da09 6261 7365 6c69 6e65 7972 7e00 0000  ..baselineyr~...
+00001e00: 727f 0000 0072 7600 0000 7253 0000 0072  r....rv...rS...r
+00001e10: 4900 0000 7249 0000 0072 4a00 0000 7226  I...rI...rJ...r&
+00001e20: 0000 002b 0100 0073 0200 0000 0002 7a14  ...+...s......z.
+00001e30: 4c69 6e65 4368 6172 742e 6261 7365 6c69  LineChart.baseli
+00001e40: 6e65 5f79 6302 0000 0000 0000 0000 0000  ne_yc...........
+00001e50: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+00001e60: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+00001e70: 5300 2902 4e72 8b00 0000 7278 0000 0072  S.).Nr....rx...r
+00001e80: 7000 0000 7249 0000 0072 4900 0000 724a  p...rI...rI...rJ
+00001e90: 0000 0072 2600 0000 2f01 0000 7302 0000  ...r&.../...s...
+00001ea0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00001eb0: 0100 0000 0400 0000 4300 0000 730e 0000  ........C...s...
+00001ec0: 007c 006a 0064 0164 0264 038d 0253 0029  .|.j.d.d.d...S.)
+00001ed0: 044e da04 6d69 6e78 727e 0000 0072 7f00  .N..minxr~...r..
+00001ee0: 0000 7276 0000 0072 5300 0000 7249 0000  ..rv...rS...rI..
+00001ef0: 0072 4900 0000 724a 0000 0072 2400 0000  .rI...rJ...r$...
+00001f00: 3401 0000 7302 0000 0000 027a 0f4c 696e  4...s......z.Lin
+00001f10: 6543 6861 7274 2e6d 696e 5f78 6302 0000  eChart.min_xc...
+00001f20: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00001f30: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
+00001f40: 7c01 a102 0100 6400 5300 2902 4e72 8c00  |.....d.S.).Nr..
+00001f50: 0000 7278 0000 0072 7000 0000 7249 0000  ..rx...rp...rI..
+00001f60: 0072 4900 0000 724a 0000 0072 2400 0000  .rI...rJ...r$...
+00001f70: 3801 0000 7302 0000 0000 0263 0100 0000  8...s......c....
+00001f80: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00001f90: 4300 0000 730e 0000 007c 006a 0064 0164  C...s....|.j.d.d
+00001fa0: 0264 038d 0253 0029 044e da04 6d61 7878  .d...S.).N..maxx
+00001fb0: 727e 0000 0072 7f00 0000 7276 0000 0072  r~...r....rv...r
+00001fc0: 5300 0000 7249 0000 0072 4900 0000 724a  S...rI...rI...rJ
+00001fd0: 0000 0072 2500 0000 3d01 0000 7302 0000  ...r%...=...s...
+00001fe0: 0000 027a 0f4c 696e 6543 6861 7274 2e6d  ...z.LineChart.m
+00001ff0: 6178 5f78 6302 0000 0000 0000 0000 0000  ax_xc...........
+00002000: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+00002010: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+00002020: 5300 2902 4e72 8d00 0000 7278 0000 0072  S.).Nr....rx...r
+00002030: 7000 0000 7249 0000 0072 4900 0000 724a  p...rI...rI...rJ
+00002040: 0000 0072 2500 0000 4101 0000 7302 0000  ...r%...A...s...
+00002050: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00002060: 0100 0000 0400 0000 4300 0000 730e 0000  ........C...s...
+00002070: 007c 006a 0064 0164 0264 038d 0253 0029  .|.j.d.d.d...S.)
+00002080: 044e da04 6d69 6e79 727e 0000 0072 7f00  .N..minyr~...r..
+00002090: 0000 7276 0000 0072 5300 0000 7249 0000  ..rv...rS...rI..
+000020a0: 0072 4900 0000 724a 0000 0072 2700 0000  .rI...rJ...r'...
+000020b0: 4601 0000 7302 0000 0000 027a 0f4c 696e  F...s......z.Lin
+000020c0: 6543 6861 7274 2e6d 696e 5f79 6302 0000  eChart.min_yc...
+000020d0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000020e0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
+000020f0: 7c01 a102 0100 6400 5300 2902 4e72 8e00  |.....d.S.).Nr..
+00002100: 0000 7278 0000 0072 7000 0000 7249 0000  ..rx...rp...rI..
+00002110: 0072 4900 0000 724a 0000 0072 2700 0000  .rI...rJ...r'...
+00002120: 4a01 0000 7302 0000 0000 0263 0100 0000  J...s......c....
+00002130: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00002140: 4300 0000 730e 0000 007c 006a 0064 0164  C...s....|.j.d.d
+00002150: 0264 038d 0253 0029 044e da04 6d61 7879  .d...S.).N..maxy
+00002160: 727e 0000 0072 7f00 0000 7276 0000 0072  r~...r....rv...r
+00002170: 5300 0000 7249 0000 0072 4900 0000 724a  S...rI...rI...rJ
+00002180: 0000 0072 2800 0000 4f01 0000 7302 0000  ...r(...O...s...
+00002190: 0000 027a 0f4c 696e 6543 6861 7274 2e6d  ...z.LineChart.m
+000021a0: 6178 5f79 6302 0000 0000 0000 0000 0000  ax_yc...........
+000021b0: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+000021c0: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+000021d0: 5300 2902 4e72 8f00 0000 7278 0000 0072  S.).Nr....rx...r
+000021e0: 7000 0000 7249 0000 0072 4900 0000 724a  p...rI...rI...rJ
+000021f0: 0000 0072 2800 0000 5301 0000 7302 0000  ...r(...S...s...
+00002200: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00002210: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00002220: 007c 006a 0053 0072 4300 0000 2901 724e  .|.j.S.rC...).rN
+00002230: 0000 0072 5300 0000 7249 0000 0072 4900  ...rS...rI...rI.
+00002240: 0000 724a 0000 0072 5100 0000 5801 0000  ..rJ...rQ...X...
+00002250: 7302 0000 0000 027a 184c 696e 6543 6861  s......z.LineCha
+00002260: 7274 2e6f 6e5f 6368 6172 745f 6576 656e  rt.on_chart_even
+00002270: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00002280: 0000 0400 0000 4300 0000 7332 0000 007c  ......C...s2...|
+00002290: 006a 00a0 017c 01a1 0101 007c 0164 0075  .j...|.....|.d.u
+000022a0: 0172 227c 00a0 0264 0164 02a1 0201 006e  .r"|...d.d.....n
+000022b0: 0c7c 00a0 0264 0164 00a1 0201 0064 0053  .|...d.d.....d.S
+000022c0: 0029 034e da0c 6f6e 4368 6172 7445 7665  .).N..onChartEve
+000022d0: 6e74 5429 0372 4e00 0000 da09 7375 6273  ntT).rN.....subs
+000022e0: 6372 6962 6572 7900 0000 2902 7252 0000  cribery...).rR..
+000022f0: 00da 0768 616e 646c 6572 7249 0000 0072  ...handlerrI...r
+00002300: 4900 0000 724a 0000 0072 5100 0000 5c01  I...rJ...rQ...\.
+00002310: 0000 7308 0000 0000 020c 0108 010e 0229  ..s............)
+00002320: 2f4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  /NNNNNNNNNNNNNNN
 00002330: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
-00002340: 4e4e 4e4e 4e4e 4e4e 4e29 31da 085f 5f6e  NNNNNNNNN)1..__n
-00002350: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00002360: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00002370: 0300 0000 7202 0000 0072 0900 0000 720f  ....r....r....r.
-00002380: 0000 0072 7a00 0000 720b 0000 00da 0373  ...rz...r......s
-00002390: 7472 7206 0000 0072 0800 0000 7207 0000  trr....r....r...
-000023a0: 0072 0e00 0000 7204 0000 00da 0369 6e74  .r....r......int
-000023b0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000023c0: 1000 0000 7205 0000 0072 4d00 0000 7254  ....r....rM...rT
-000023d0: 0000 0072 5800 0000 726e 0000 00da 0870  ...rX...rn.....p
-000023e0: 726f 7065 7274 7972 1500 0000 da06 7365  ropertyr......se
-000023f0: 7474 6572 7216 0000 0072 1a00 0000 7217  tterr....r....r.
-00002400: 0000 0072 1800 0000 7219 0000 0072 1b00  ...r....r....r..
-00002410: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00002420: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00002430: 7222 0000 0072 2300 0000 7226 0000 0072  r"...r#...r&...r
-00002440: 2400 0000 7225 0000 0072 2700 0000 7228  $...r%...r'...r(
-00002450: 0000 0072 5100 0000 da0d 5f5f 636c 6173  ...rQ.....__clas
-00002460: 7363 656c 6c5f 5f72 4900 0000 7249 0000  scell__rI...rI..
-00002470: 0072 5e00 0000 724a 0000 0072 1400 0000  .r^...rJ...r....
-00002480: 1600 0000 736a 0100 0008 0300 0100 0100  ....sj..........
-00002490: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-000024a0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-000024b0: 0100 0100 0400 0100 0100 0100 0100 0100  ................
-000024c0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-000024d0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-000024e0: 0100 0100 0100 0100 cd02 020a 0102 0106  ................
-000024f0: 0102 0102 0106 0106 0106 0106 0106 0106  ................
-00002500: 0106 0106 0106 0102 0102 0102 0102 0102  ................
-00002510: 0102 0506 0102 0102 0102 0102 0102 0102  ................
-00002520: 010c 0106 0106 0102 0102 0102 0102 0102  ................
-00002530: 0102 0102 0102 0102 0102 0102 0206 0106  ................
-00002540: 0106 0102 cd0c 7008 030c 0708 1302 010a  ......p.........
-00002550: 0304 010a 0402 0110 0304 0110 0402 0114  ................
-00002560: 0304 0114 0402 0114 0304 0114 0402 0110  ................
-00002570: 0304 0110 0402 0110 0304 0110 0402 0114  ................
-00002580: 0304 0114 0402 0114 0304 0114 0402 0114  ................
-00002590: 0304 0114 0402 0114 0304 0114 0402 0114  ................
-000025a0: 0304 0114 0402 0114 0304 0114 0402 0114  ................
-000025b0: 0304 0114 0402 0114 0304 0114 0402 0110  ................
-000025c0: 0304 0110 0402 0110 0304 0110 0402 0110  ................
-000025d0: 0304 0110 0402 0110 0304 0110 0402 0110  ................
-000025e0: 0304 0110 0402 0110 0304 0110 0402 010a  ................
-000025f0: 0304 0172 1400 0000 6300 0000 0000 0000  ...r....c.......
-00002600: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00002610: 0073 1a00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00002620: 6402 9c01 6403 6404 8404 5a03 6401 5300  d...d.d...Z.d.S.
-00002630: 2905 7246 0000 004e 7272 0000 0063 0300  ).rF...Nrr...c..
-00002640: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-00002650: 0000 4300 0000 7310 0000 007c 017c 005f  ..C...s....|.|._
-00002660: 007c 027c 005f 0164 0053 0072 4300 0000  .|.|._.d.S.rC...
-00002670: 2902 da04 7479 7065 da05 7370 6f74 7329  )...type..spots)
-00002680: 0372 5200 0000 729b 0000 0072 9c00 0000  .rR...r....r....
-00002690: 7249 0000 0072 4900 0000 724a 0000 0072  rI...rI...rJ...r
-000026a0: 4d00 0000 6601 0000 7304 0000 0000 0106  M...f...s.......
-000026b0: 017a 174c 696e 6543 6861 7274 4576 656e  .z.LineChartEven
-000026c0: 742e 5f5f 696e 6974 5f5f a904 7293 0000  t.__init__..r...
-000026d0: 0072 9400 0000 7295 0000 0072 4d00 0000  .r....r....rM...
-000026e0: 7249 0000 0072 4900 0000 7249 0000 0072  rI...rI...rI...r
-000026f0: 4a00 0000 7246 0000 0065 0100 0073 0200  J...rF...e...s..
-00002700: 0000 0801 7246 0000 0063 0000 0000 0000  ....rF...c......
-00002710: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00002720: 0000 731a 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00002730: 0164 029c 0164 0364 0484 045a 0364 0153  .d...d.d...Z.d.S
-00002740: 0029 05da 124c 696e 6543 6861 7274 4576  .)...LineChartEv
-00002750: 656e 7453 706f 744e 7272 0000 0063 0300  entSpotNrr...c..
-00002760: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-00002770: 0000 4300 0000 7310 0000 007c 017c 005f  ..C...s....|.|._
-00002780: 007c 027c 005f 0164 0053 0072 4300 0000  .|.|._.d.S.rC...
-00002790: 2902 da09 6261 725f 696e 6465 78da 0a73  )...bar_index..s
-000027a0: 706f 745f 696e 6465 7829 0372 5200 0000  pot_index).rR...
-000027b0: 729f 0000 0072 a000 0000 7249 0000 0072  r....r....rI...r
-000027c0: 4900 0000 724a 0000 0072 4d00 0000 6c01  I...rJ...rM...l.
-000027d0: 0000 7304 0000 0000 0106 017a 1b4c 696e  ..s........z.Lin
-000027e0: 6543 6861 7274 4576 656e 7453 706f 742e  eChartEventSpot.
-000027f0: 5f5f 696e 6974 5f5f 729d 0000 0072 4900  __init__r....rI.
-00002800: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
-00002810: 0072 9e00 0000 6b01 0000 7302 0000 0008  .r....k...s.....
-00002820: 0172 9e00 0000 2921 7244 0000 00da 0674  .r....)!rD.....t
-00002830: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-00002840: 0400 0000 7205 0000 00da 1066 6c65 745f  ....r......flet_
-00002850: 636f 7265 2e62 6f72 6465 7272 0600 0000  core.borderr....
-00002860: da1b 666c 6574 5f63 6f72 652e 6368 6172  ..flet_core.char
-00002870: 7473 2e63 6861 7274 5f61 7869 7372 0700  ts.chart_axisr..
-00002880: 0000 da21 666c 6574 5f63 6f72 652e 6368  ...!flet_core.ch
-00002890: 6172 7473 2e63 6861 7274 5f67 7269 645f  arts.chart_grid_
-000028a0: 6c69 6e65 7372 0800 0000 da20 666c 6574  linesr..... flet
-000028b0: 5f63 6f72 652e 6368 6172 7473 2e6c 696e  _core.charts.lin
-000028c0: 655f 6368 6172 745f 6461 7461 7209 0000  e_chart_datar...
-000028d0: 00da 1d66 6c65 745f 636f 7265 2e63 6f6e  ...flet_core.con
-000028e0: 7374 7261 696e 6564 5f63 6f6e 7472 6f6c  strained_control
-000028f0: 720a 0000 00da 1166 6c65 745f 636f 7265  r......flet_core
-00002900: 2e63 6f6e 7472 6f6c 720b 0000 00da 1766  .controlr......f
-00002910: 6c65 745f 636f 7265 2e63 6f6e 7472 6f6c  let_core.control
-00002920: 5f65 7665 6e74 720c 0000 00da 1766 6c65  _eventr......fle
-00002930: 745f 636f 7265 2e65 7665 6e74 5f68 616e  t_core.event_han
-00002940: 646c 6572 720d 0000 00da 0d66 6c65 745f  dlerr......flet_
-00002950: 636f 7265 2e72 6566 720e 0000 00da 0f66  core.refr......f
-00002960: 6c65 745f 636f 7265 2e74 7970 6573 720f  let_core.typesr.
-00002970: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-00002980: 0000 7213 0000 0072 1400 0000 7246 0000  ..r....r....rF..
-00002990: 0072 9e00 0000 7249 0000 0072 4900 0000  .r....rI...rI...
-000029a0: 7249 0000 0072 4a00 0000 da08 3c6d 6f64  rI...rJ.....<mod
-000029b0: 756c 653e 0100 0000 7320 0000 0008 0118  ule>....s ......
-000029c0: 020c 010c 010c 010c 010c 010c 010c 010c  ................
-000029d0: 010c 011c 0910 7f00 7f00 5110 06         ..........Q..
+00002340: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
+00002350: 2931 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )1..__name__..__
+00002360: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00002370: 6e61 6d65 5f5f 7203 0000 0072 0200 0000  name__r....r....
+00002380: 7209 0000 0072 0f00 0000 727a 0000 0072  r....r....rz...r
+00002390: 0b00 0000 da03 7374 7272 0600 0000 7208  ......strr....r.
+000023a0: 0000 0072 0700 0000 720e 0000 0072 0400  ...r....r....r..
+000023b0: 0000 da03 696e 7472 1100 0000 7212 0000  ....intr....r...
+000023c0: 0072 1300 0000 7210 0000 0072 0500 0000  .r....r....r....
+000023d0: 724d 0000 0072 5400 0000 7258 0000 0072  rM...rT...rX...r
+000023e0: 6e00 0000 da08 7072 6f70 6572 7479 7215  n.....propertyr.
+000023f0: 0000 00da 0673 6574 7465 7272 1600 0000  .....setterr....
+00002400: 721a 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00002410: 1900 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
+00002420: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+00002430: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00002440: 0072 2600 0000 7224 0000 0072 2500 0000  .r&...r$...r%...
+00002450: 7227 0000 0072 2800 0000 7251 0000 00da  r'...r(...rQ....
+00002460: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7249  .__classcell__rI
+00002470: 0000 0072 4900 0000 725e 0000 0072 4a00  ...rI...r^...rJ.
+00002480: 0000 7214 0000 0016 0000 0073 6a01 0000  ..r........sj...
+00002490: 0803 0001 0001 0001 0001 0001 0001 0001  ................
+000024a0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+000024b0: 0001 0001 0001 0001 0001 0004 0001 0001  ................
+000024c0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+000024d0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+000024e0: 0001 0001 0001 0001 0001 0001 0001 00cd  ................
+000024f0: 0202 0a01 0201 0601 0201 0201 0601 0601  ................
+00002500: 0601 0601 0601 0601 0601 0601 0601 0201  ................
+00002510: 0201 0201 0201 0201 0205 0601 0201 0201  ................
+00002520: 0201 0201 0201 0201 0c01 0601 0601 0201  ................
+00002530: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00002540: 0201 0202 0601 0601 0601 02cd 0c70 0803  .............p..
+00002550: 0c07 0813 0201 0a03 0401 0a04 0201 1003  ................
+00002560: 0401 1004 0201 1403 0401 1404 0201 1403  ................
+00002570: 0401 1404 0201 1003 0401 1004 0201 1003  ................
+00002580: 0401 1004 0201 1403 0401 1404 0201 1403  ................
+00002590: 0401 1404 0201 1403 0401 1404 0201 1403  ................
+000025a0: 0401 1404 0201 1403 0401 1404 0201 1403  ................
+000025b0: 0401 1404 0201 1403 0401 1404 0201 1403  ................
+000025c0: 0401 1404 0201 1003 0401 1004 0201 1003  ................
+000025d0: 0401 1004 0201 1003 0401 1004 0201 1003  ................
+000025e0: 0401 1004 0201 1003 0401 1004 0201 1003  ................
+000025f0: 0401 1004 0201 0a03 0401 7214 0000 0063  ..........r....c
+00002600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002610: 0300 0000 4000 0000 731a 0000 0065 005a  ....@...s....e.Z
+00002620: 0164 005a 0264 0164 029c 0164 0364 0484  .d.Z.d.d...d.d..
+00002630: 045a 0364 0153 0029 0572 4600 0000 4e72  .Z.d.S.).rF...Nr
+00002640: 7200 0000 6303 0000 0000 0000 0000 0000  r...c...........
+00002650: 0003 0000 0002 0000 0043 0000 0073 1000  .........C...s..
+00002660: 0000 7c01 7c00 5f00 7c02 7c00 5f01 6400  ..|.|._.|.|._.d.
+00002670: 5300 7243 0000 0029 02da 0474 7970 65da  S.rC...)...type.
+00002680: 0573 706f 7473 2903 7252 0000 0072 9b00  .spots).rR...r..
+00002690: 0000 729c 0000 0072 4900 0000 7249 0000  ..r....rI...rI..
+000026a0: 0072 4a00 0000 724d 0000 0066 0100 0073  .rJ...rM...f...s
+000026b0: 0400 0000 0001 0601 7a17 4c69 6e65 4368  ........z.LineCh
+000026c0: 6172 7445 7665 6e74 2e5f 5f69 6e69 745f  artEvent.__init_
+000026d0: 5fa9 0472 9300 0000 7294 0000 0072 9500  _..r....r....r..
+000026e0: 0000 724d 0000 0072 4900 0000 7249 0000  ..rM...rI...rI..
+000026f0: 0072 4900 0000 724a 0000 0072 4600 0000  .rI...rJ...rF...
+00002700: 6501 0000 7302 0000 0008 0172 4600 0000  e...s......rF...
+00002710: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00002720: 0003 0000 0040 0000 0073 1a00 0000 6500  .....@...s....e.
+00002730: 5a01 6400 5a02 6401 6402 9c01 6403 6404  Z.d.Z.d.d...d.d.
+00002740: 8404 5a03 6401 5300 2905 da12 4c69 6e65  ..Z.d.S.)...Line
+00002750: 4368 6172 7445 7665 6e74 5370 6f74 4e72  ChartEventSpotNr
+00002760: 7200 0000 6303 0000 0000 0000 0000 0000  r...c...........
+00002770: 0003 0000 0002 0000 0043 0000 0073 1000  .........C...s..
+00002780: 0000 7c01 7c00 5f00 7c02 7c00 5f01 6400  ..|.|._.|.|._.d.
+00002790: 5300 7243 0000 0029 02da 0962 6172 5f69  S.rC...)...bar_i
+000027a0: 6e64 6578 da0a 7370 6f74 5f69 6e64 6578  ndex..spot_index
+000027b0: 2903 7252 0000 0072 9f00 0000 72a0 0000  ).rR...r....r...
+000027c0: 0072 4900 0000 7249 0000 0072 4a00 0000  .rI...rI...rJ...
+000027d0: 724d 0000 006c 0100 0073 0400 0000 0001  rM...l...s......
+000027e0: 0601 7a1b 4c69 6e65 4368 6172 7445 7665  ..z.LineChartEve
+000027f0: 6e74 5370 6f74 2e5f 5f69 6e69 745f 5f72  ntSpot.__init__r
+00002800: 9d00 0000 7249 0000 0072 4900 0000 7249  ....rI...rI...rI
+00002810: 0000 0072 4a00 0000 729e 0000 006b 0100  ...rJ...r....k..
+00002820: 0073 0200 0000 0801 729e 0000 0029 2172  .s......r....)!r
+00002830: 4400 0000 da06 7479 7069 6e67 7202 0000  D.....typingr...
+00002840: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
+00002850: da10 666c 6574 5f63 6f72 652e 626f 7264  ..flet_core.bord
+00002860: 6572 7206 0000 00da 1b66 6c65 745f 636f  err......flet_co
+00002870: 7265 2e63 6861 7274 732e 6368 6172 745f  re.charts.chart_
+00002880: 6178 6973 7207 0000 00da 2166 6c65 745f  axisr.....!flet_
+00002890: 636f 7265 2e63 6861 7274 732e 6368 6172  core.charts.char
+000028a0: 745f 6772 6964 5f6c 696e 6573 7208 0000  t_grid_linesr...
+000028b0: 00da 2066 6c65 745f 636f 7265 2e63 6861  .. flet_core.cha
+000028c0: 7274 732e 6c69 6e65 5f63 6861 7274 5f64  rts.line_chart_d
+000028d0: 6174 6172 0900 0000 da1d 666c 6574 5f63  atar......flet_c
+000028e0: 6f72 652e 636f 6e73 7472 6169 6e65 645f  ore.constrained_
+000028f0: 636f 6e74 726f 6c72 0a00 0000 da11 666c  controlr......fl
+00002900: 6574 5f63 6f72 652e 636f 6e74 726f 6c72  et_core.controlr
+00002910: 0b00 0000 da17 666c 6574 5f63 6f72 652e  ......flet_core.
+00002920: 636f 6e74 726f 6c5f 6576 656e 7472 0c00  control_eventr..
+00002930: 0000 da17 666c 6574 5f63 6f72 652e 6576  ....flet_core.ev
+00002940: 656e 745f 6861 6e64 6c65 7272 0d00 0000  ent_handlerr....
+00002950: da0d 666c 6574 5f63 6f72 652e 7265 6672  ..flet_core.refr
+00002960: 0e00 0000 da0f 666c 6574 5f63 6f72 652e  ......flet_core.
+00002970: 7479 7065 7372 0f00 0000 7210 0000 0072  typesr....r....r
+00002980: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00002990: 0000 0072 4600 0000 729e 0000 0072 4900  ...rF...r....rI.
+000029a0: 0000 7249 0000 0072 4900 0000 724a 0000  ..rI...rI...rJ..
+000029b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000029c0: 2000 0000 0801 1802 0c01 0c01 0c01 0c01   ...............
+000029d0: 0c01 0c01 0c01 0c01 0c01 1c09 107f 007f  ................
+000029e0: 0051 1006                                .Q..
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 9357 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 8d24 0000  a........:)f.$..
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 8d24 0000  a........./f.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6406 6c0e  m.Z.m.Z...d.d.l.
@@ -140,434 +140,434 @@
 000008b0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
 000008c0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
 000008d0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
 000008e0: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
 000008f0: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
 00000900: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
 00000910: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
-00000920: 7227 0000 00a9 0072 2a00 0000 fa62 2f77  r'.....r*....b/w
+00000920: 7227 0000 00a9 0072 2a00 0000 fa69 2f77  r'.....r*....i/w
 00000930: 6f72 6b73 7061 6365 732f 636f 6e74 7269  orkspaces/contri
-00000940: 6266 6c65 742f 666c 6574 2f73 646b 2f70  bflet/flet/sdk/p
-00000950: 7974 686f 6e2f 7061 636b 6167 6573 2f66  ython/packages/f
-00000960: 6c65 742d 636f 7265 2f73 7263 2f66 6c65  let-core/src/fle
-00000970: 745f 636f 7265 2f63 6861 7274 732f 6c69  t_core/charts/li
-00000980: 6e65 5f63 6861 7274 5f64 6174 612e 7079  ne_chart_data.py
-00000990: 7228 0000 000d 0000 0073 3a00 0000 0020  r(.......s:.... 
-000009a0: 0401 0201 0201 0201 0201 02fb 0608 0601  ................
-000009b0: 0601 0601 0601 0601 0601 0602 02ff 0403  ................
-000009c0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-000009d0: 0601 0601 0601 0601 7a16 4c69 6e65 4368  ........z.LineCh
-000009e0: 6172 7444 6174 612e 5f5f 696e 6974 5f5f  artData.__init__
-000009f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000a00: 0001 0000 0043 0000 0073 0400 0000 6401  .....C...s....d.
-00000a10: 5300 2902 4e72 2700 0000 722a 0000 00a9  S.).Nr'...r*....
-00000a20: 0172 2900 0000 722a 0000 0072 2a00 0000  .r)...r*...r*...
-00000a30: 722b 0000 00da 115f 6765 745f 636f 6e74  r+....._get_cont
-00000a40: 726f 6c5f 6e61 6d65 4d00 0000 7302 0000  rol_nameM...s...
-00000a50: 0000 017a 1f4c 696e 6543 6861 7274 4461  ...z.LineChartDa
-00000a60: 7461 2e5f 6765 745f 636f 6e74 726f 6c5f  ta._get_control_
-00000a70: 6e61 6d65 6301 0000 0000 0000 0000 0000  namec...........
-00000a80: 0001 0000 0004 0000 0003 0000 0073 9a00  .............s..
-00000a90: 0000 7400 8300 a001 a100 0100 7c00 a002  ..t.........|...
-00000aa0: 6401 7c00 6a03 a102 0100 7c00 a002 6402  d.|.j.....|...d.
-00000ab0: 7c00 6a04 a102 0100 7c00 a002 6403 7c00  |.j.....|...d.|.
-00000ac0: 6a05 a102 0100 7c00 a002 6404 7c00 6a06  j.....|...d.|.j.
-00000ad0: a102 0100 7c00 a002 6405 7c00 6a07 a102  ....|...d.|.j...
-00000ae0: 0100 7c00 a002 6406 7c00 6a08 a102 0100  ..|...d.|.j.....
-00000af0: 7c00 a002 6407 7c00 6a09 a102 0100 7c00  |...d.|.j.....|.
-00000b00: a002 6408 7c00 6a0a a102 0100 7c00 a002  ..d.|.j.....|...
-00000b10: 6409 7c00 6a0b a102 0100 7c00 a002 640a  d.|.j.....|...d.
-00000b20: 7c00 6a0c a102 0100 6400 5300 290b 4e72  |.j.....d.S.).Nr
-00000b30: 1200 0000 7218 0000 0072 2200 0000 5a0d  ....r....r"...Z.
-00000b40: 7365 6c65 6374 6564 506f 696e 745a 0b64  selectedPointZ.d
-00000b50: 6173 6850 6174 7465 726e 5a11 6162 6f76  ashPatternZ.abov
-00000b60: 654c 696e 6547 7261 6469 656e 745a 1162  eLineGradientZ.b
-00000b70: 656c 6f77 4c69 6e65 4772 6164 6965 6e74  elowLineGradient
-00000b80: 5a09 6162 6f76 654c 696e 655a 0962 656c  Z.aboveLineZ.bel
-00000b90: 6f77 4c69 6e65 5a11 7365 6c65 6374 6564  owLineZ.selected
-00000ba0: 4265 6c6f 774c 696e 6529 0dda 0573 7570  BelowLine)...sup
-00000bb0: 6572 da0d 6265 666f 7265 5f75 7064 6174  er..before_updat
-00000bc0: 65da 0e5f 7365 745f 6174 7472 5f6a 736f  e.._set_attr_jso
-00000bd0: 6eda 185f 4c69 6e65 4368 6172 7444 6174  n.._LineChartDat
-00000be0: 615f 5f67 7261 6469 656e 74da 165f 4c69  a__gradient.._Li
-00000bf0: 6e65 4368 6172 7444 6174 615f 5f73 6861  neChartData__sha
-00000c00: 646f 77da 155f 4c69 6e65 4368 6172 7444  dow.._LineChartD
-00000c10: 6174 615f 5f70 6f69 6e74 da1e 5f4c 696e  ata__point.._Lin
-00000c20: 6543 6861 7274 4461 7461 5f5f 7365 6c65  eChartData__sele
-00000c30: 6374 6564 5f70 6f69 6e74 da1c 5f4c 696e  cted_point.._Lin
-00000c40: 6543 6861 7274 4461 7461 5f5f 6461 7368  eChartData__dash
-00000c50: 5f70 6174 7465 726e da23 5f4c 696e 6543  _pattern.#_LineC
-00000c60: 6861 7274 4461 7461 5f5f 6162 6f76 655f  hartData__above_
-00000c70: 6c69 6e65 5f67 7261 6469 656e 74da 235f  line_gradient.#_
-00000c80: 4c69 6e65 4368 6172 7444 6174 615f 5f62  LineChartData__b
-00000c90: 656c 6f77 5f6c 696e 655f 6772 6164 6965  elow_line_gradie
-00000ca0: 6e74 da1a 5f4c 696e 6543 6861 7274 4461  nt.._LineChartDa
-00000cb0: 7461 5f5f 6162 6f76 655f 6c69 6e65 da1a  ta__above_line..
-00000cc0: 5f4c 696e 6543 6861 7274 4461 7461 5f5f  _LineChartData__
-00000cd0: 6265 6c6f 775f 6c69 6e65 da23 5f4c 696e  below_line.#_Lin
-00000ce0: 6543 6861 7274 4461 7461 5f5f 7365 6c65  eChartData__sele
-00000cf0: 6374 6564 5f62 656c 6f77 5f6c 696e 6572  cted_below_liner
-00000d00: 2c00 0000 a901 da09 5f5f 636c 6173 735f  ,.......__class_
-00000d10: 5f72 2a00 0000 722b 0000 0072 2f00 0000  _r*...r+...r/...
-00000d20: 5000 0000 7316 0000 0000 010a 010e 010e  P...s...........
-00000d30: 010e 010e 010e 010e 010e 010e 010e 017a  ...............z
-00000d40: 1b4c 696e 6543 6861 7274 4461 7461 2e62  .LineChartData.b
-00000d50: 6566 6f72 655f 7570 6461 7465 6301 0000  efore_updatec...
-00000d60: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00000d70: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00000d80: a901 4ea9 015a 1b5f 4c69 6e65 4368 6172  ..N..Z._LineChar
-00000d90: 7444 6174 615f 5f64 6174 615f 706f 696e  tData__data_poin
-00000da0: 7473 722c 0000 0072 2a00 0000 722a 0000  tsr,...r*...r*..
-00000db0: 0072 2b00 0000 da0d 5f67 6574 5f63 6869  .r+....._get_chi
-00000dc0: 6c64 7265 6e5d 0000 0073 0200 0000 0001  ldren]...s......
-00000dd0: 7a1b 4c69 6e65 4368 6172 7444 6174 612e  z.LineChartData.
-00000de0: 5f67 6574 5f63 6869 6c64 7265 6e63 0100  _get_childrenc..
-00000df0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000e00: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
-00000e10: 0072 3d00 0000 723e 0000 0072 2c00 0000  .r=...r>...r,...
-00000e20: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
-00000e30: 0f00 0000 6100 0000 7302 0000 0000 027a  ....a...s......z
-00000e40: 194c 696e 6543 6861 7274 4461 7461 2e64  .LineChartData.d
-00000e50: 6174 615f 706f 696e 7473 6302 0000 0000  ata_pointsc.....
-00000e60: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000e70: 0000 0073 1600 0000 7c01 6400 7501 720c  ...s....|.d.u.r.
-00000e80: 7c01 6e02 6700 7c00 5f00 6400 5300 723d  |.n.g.|._.d.S.r=
-00000e90: 0000 0072 3e00 0000 a902 7229 0000 00da  ...r>.....r)....
-00000ea0: 0576 616c 7565 722a 0000 0072 2a00 0000  .valuer*...r*...
-00000eb0: 722b 0000 0072 0f00 0000 6500 0000 7302  r+...r....e...s.
-00000ec0: 0000 0000 0229 01da 0672 6574 7572 6e63  .....)...returnc
-00000ed0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000ee0: 0500 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
-00000ef0: 0064 0164 0264 0364 048d 0353 0029 054e  .d.d.d.d...S.).N
-00000f00: da0b 7374 726f 6b65 5769 6474 68da 0566  ..strokeWidth..f
-00000f10: 6c6f 6174 6700 0000 0000 00f0 3fa9 02da  loatg.......?...
-00000f20: 0964 6174 615f 7479 7065 da09 6465 665f  .data_type..def_
-00000f30: 7661 6c75 65a9 01da 095f 6765 745f 6174  value...._get_at
-00000f40: 7472 722c 0000 0072 2a00 0000 722a 0000  trr,...r*...r*..
-00000f50: 0072 2b00 0000 7213 0000 006a 0000 0073  .r+...r....j...s
-00000f60: 0200 0000 0002 7a1a 4c69 6e65 4368 6172  ......z.LineChar
-00000f70: 7444 6174 612e 7374 726f 6b65 5f77 6964  tData.stroke_wid
-00000f80: 7468 2901 7241 0000 0063 0200 0000 0000  th).rA...c......
-00000f90: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000fa0: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-00000fb0: 0201 0064 0053 0029 024e 7243 0000 00a9  ...d.S.).NrC....
-00000fc0: 01da 095f 7365 745f 6174 7472 7240 0000  ..._set_attrr@..
-00000fd0: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
-00000fe0: 7213 0000 006e 0000 0073 0200 0000 0002  r....n...s......
-00000ff0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001000: 0005 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00001010: 6a00 6401 6402 6403 6404 8d03 5300 2905  j.d.d.d.d...S.).
-00001020: 4e72 1000 0000 da04 626f 6f6c 4672 4500  Nr......boolFrE.
-00001030: 0000 7248 0000 0072 2c00 0000 722a 0000  ..rH...r,...r*..
-00001040: 0072 2a00 0000 722b 0000 0072 1000 0000  .r*...r+...r....
-00001050: 7300 0000 7302 0000 0000 027a 144c 696e  s...s......z.Lin
-00001060: 6543 6861 7274 4461 7461 2e63 7572 7665  eChartData.curve
-00001070: 6463 0200 0000 0000 0000 0000 0000 0200  dc..............
-00001080: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
-00001090: 00a0 0064 017c 01a1 0201 0064 0053 0029  ...d.|.....d.S.)
-000010a0: 024e 7210 0000 0072 4a00 0000 7240 0000  .Nr....rJ...r@..
-000010b0: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
-000010c0: 7210 0000 0077 0000 0073 0200 0000 0002  r....w...s......
-000010d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000010e0: 0003 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
-000010f0: a000 6401 a101 5300 a902 4e72 1100 0000  ..d...S...Nr....
-00001100: 7248 0000 0072 2c00 0000 722a 0000 0072  rH...r,...r*...r
-00001110: 2a00 0000 722b 0000 0072 1100 0000 7c00  *...r+...r....|.
-00001120: 0000 7302 0000 0000 027a 134c 696e 6543  ..s......z.LineC
-00001130: 6861 7274 4461 7461 2e63 6f6c 6f72 6302  hartData.colorc.
-00001140: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001150: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-00001160: 6401 7c01 a102 0100 6400 5300 724d 0000  d.|.....d.S.rM..
-00001170: 0072 4a00 0000 7240 0000 0072 2a00 0000  .rJ...r@...r*...
-00001180: 722a 0000 0072 2b00 0000 7211 0000 0080  r*...r+...r.....
-00001190: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-000011a0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000011b0: 0000 0073 0600 0000 7c00 6a00 5300 723d  ...s....|.j.S.r=
-000011c0: 0000 00a9 0172 3100 0000 722c 0000 0072  .....r1...r,...r
-000011d0: 2a00 0000 722a 0000 0072 2b00 0000 7212  *...r*...r+...r.
-000011e0: 0000 0085 0000 0073 0200 0000 0002 7a16  .......s......z.
-000011f0: 4c69 6e65 4368 6172 7444 6174 612e 6772  LineChartData.gr
-00001200: 6164 6965 6e74 6302 0000 0000 0000 0000  adientc.........
-00001210: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00001220: 0a00 0000 7c01 7c00 5f00 6400 5300 723d  ....|.|._.d.S.r=
-00001230: 0000 0072 4e00 0000 7240 0000 0072 2a00  ...rN...r@...r*.
-00001240: 0000 722a 0000 0072 2b00 0000 7212 0000  ..r*...r+...r...
-00001250: 0089 0000 0073 0200 0000 0002 6301 0000  .....s......c...
-00001260: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00001270: 0043 0000 0073 1000 0000 7c00 6a00 6401  .C...s....|.j.d.
-00001280: 6402 6403 6404 8d03 5300 2905 4eda 0e73  d.d.d...S.).N..s
-00001290: 7472 6f6b 6543 6170 526f 756e 6472 4c00  trokeCapRoundrL.
-000012a0: 0000 4672 4500 0000 7248 0000 0072 2c00  ..FrE...rH...r,.
-000012b0: 0000 722a 0000 0072 2a00 0000 722b 0000  ..r*...r*...r+..
-000012c0: 0072 1400 0000 8e00 0000 7302 0000 0000  .r........s.....
-000012d0: 027a 1e4c 696e 6543 6861 7274 4461 7461  .z.LineChartData
-000012e0: 2e73 7472 6f6b 655f 6361 705f 726f 756e  .stroke_cap_roun
-000012f0: 6463 0200 0000 0000 0000 0000 0000 0200  dc..............
-00001300: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
-00001310: 00a0 0064 017c 01a1 0201 0064 0053 0029  ...d.|.....d.S.)
-00001320: 024e 724f 0000 0072 4a00 0000 7240 0000  .NrO...rJ...r@..
-00001330: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
-00001340: 7214 0000 0092 0000 0073 0200 0000 0002  r........s......
-00001350: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001360: 0005 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00001370: 6a00 6401 6402 6403 6404 8d03 5300 2905  j.d.d.d.d...S.).
-00001380: 4eda 1870 7265 7665 6e74 4375 7276 654f  N..preventCurveO
-00001390: 7665 7253 686f 6f74 696e 6772 4c00 0000  verShootingrL...
-000013a0: 4672 4500 0000 7248 0000 0072 2c00 0000  FrE...rH...r,...
-000013b0: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
-000013c0: 1500 0000 9700 0000 7306 0000 0000 0204  ........s.......
-000013d0: 0106 ff7a 294c 696e 6543 6861 7274 4461  ...z)LineChartDa
-000013e0: 7461 2e70 7265 7665 6e74 5f63 7572 7665  ta.prevent_curve
-000013f0: 5f6f 7665 725f 7368 6f6f 7469 6e67 6302  _over_shootingc.
-00001400: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001410: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
-00001420: 6401 7c01 a102 0100 6400 5300 2902 4e72  d.|.....d.S.).Nr
-00001430: 5000 0000 724a 0000 0072 4000 0000 722a  P...rJ...r@...r*
-00001440: 0000 0072 2a00 0000 722b 0000 0072 1500  ...r*...r+...r..
-00001450: 0000 9d00 0000 7302 0000 0000 0263 0100  ......s......c..
-00001460: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00001470: 0000 4300 0000 730e 0000 007c 006a 0064  ..C...s....|.j.d
-00001480: 0164 0264 038d 0253 0029 044e da21 7072  .d.d...S.).N.!pr
-00001490: 6576 656e 7443 7572 7665 4f76 6572 5368  eventCurveOverSh
-000014a0: 6f6f 7469 6e67 5468 7265 7368 6f6c 6472  ootingThresholdr
-000014b0: 4400 0000 a901 7246 0000 0072 4800 0000  D.....rF...rH...
-000014c0: 722c 0000 0072 2a00 0000 722a 0000 0072  r,...r*...r*...r
-000014d0: 2b00 0000 7216 0000 00a2 0000 0073 0200  +...r........s..
-000014e0: 0000 0002 7a33 4c69 6e65 4368 6172 7444  ....z3LineChartD
-000014f0: 6174 612e 7072 6576 656e 745f 6375 7276  ata.prevent_curv
-00001500: 655f 6f76 6572 5f73 686f 6f74 696e 675f  e_over_shooting_
-00001510: 7468 7265 7368 6f6c 6463 0200 0000 0000  thresholdc......
-00001520: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00001530: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-00001540: 0201 0064 0053 0029 024e 7251 0000 0072  ...d.S.).NrQ...r
-00001550: 4a00 0000 7240 0000 0072 2a00 0000 722a  J...r@...r*...r*
-00001560: 0000 0072 2b00 0000 7216 0000 00a6 0000  ...r+...r.......
-00001570: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00001580: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00001590: 0073 0600 0000 7c00 6a00 5300 723d 0000  .s....|.j.S.r=..
-000015a0: 00a9 0172 3500 0000 722c 0000 0072 2a00  ...r5...r,...r*.
-000015b0: 0000 722a 0000 0072 2b00 0000 7217 0000  ..r*...r+...r...
-000015c0: 00ab 0000 0073 0200 0000 0002 7a1a 4c69  .....s......z.Li
-000015d0: 6e65 4368 6172 7444 6174 612e 6461 7368  neChartData.dash
-000015e0: 5f70 6174 7465 726e 6302 0000 0000 0000  _patternc.......
-000015f0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00001600: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
-00001610: 723d 0000 0072 5300 0000 7240 0000 0072  r=...rS...r@...r
-00001620: 2a00 0000 722a 0000 0072 2b00 0000 7217  *...r*...r+...r.
-00001630: 0000 00af 0000 0073 0200 0000 0002 6301  .......s......c.
-00001640: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00001650: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00001660: 5300 723d 0000 00a9 0172 3200 0000 722c  S.r=.....r2...r,
-00001670: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
-00001680: 0000 7218 0000 00b4 0000 0073 0200 0000  ..r........s....
-00001690: 0002 7a14 4c69 6e65 4368 6172 7444 6174  ..z.LineChartDat
-000016a0: 612e 7368 6164 6f77 6302 0000 0000 0000  a.shadowc.......
-000016b0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000016c0: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
-000016d0: 723d 0000 0072 5400 0000 7240 0000 0072  r=...rT...r@...r
-000016e0: 2a00 0000 722a 0000 0072 2b00 0000 7218  *...r*...r+...r.
-000016f0: 0000 00b8 0000 0073 0200 0000 0002 6301  .......s......c.
-00001700: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00001710: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00001720: 5300 723d 0000 00a9 0172 3300 0000 722c  S.r=.....r3...r,
-00001730: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
-00001740: 0000 7222 0000 00bd 0000 0073 0200 0000  ..r".......s....
-00001750: 0002 7a13 4c69 6e65 4368 6172 7444 6174  ..z.LineChartDat
-00001760: 612e 706f 696e 7463 0200 0000 0000 0000  a.pointc........
-00001770: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00001780: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
-00001790: 3d00 0000 7255 0000 0072 4000 0000 722a  =...rU...r@...r*
-000017a0: 0000 0072 2a00 0000 722b 0000 0072 2200  ...r*...r+...r".
-000017b0: 0000 c100 0000 7302 0000 0000 0263 0100  ......s......c..
-000017c0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000017d0: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
-000017e0: 0072 3d00 0000 a901 7234 0000 0072 2c00  .r=.....r4...r,.
-000017f0: 0000 722a 0000 0072 2a00 0000 722b 0000  ..r*...r*...r+..
-00001800: 0072 2300 0000 c600 0000 7302 0000 0000  .r#.......s.....
-00001810: 027a 1c4c 696e 6543 6861 7274 4461 7461  .z.LineChartData
-00001820: 2e73 656c 6563 7465 645f 706f 696e 7463  .selected_pointc
-00001830: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001840: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
-00001850: 005f 0064 0053 0072 3d00 0000 7256 0000  ._.d.S.r=...rV..
-00001860: 0072 4000 0000 722a 0000 0072 2a00 0000  .r@...r*...r*...
-00001870: 722b 0000 0072 2300 0000 ca00 0000 7302  r+...r#.......s.
-00001880: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00001890: 0000 0100 0000 0300 0000 4300 0000 730a  ..........C...s.
-000018a0: 0000 007c 00a0 0064 01a1 0153 00a9 024e  ...|...d...S...N
-000018b0: 5a10 6162 6f76 654c 696e 6542 6763 6f6c  Z.aboveLineBgcol
-000018c0: 6f72 7248 0000 0072 2c00 0000 722a 0000  orrH...r,...r*..
-000018d0: 0072 2a00 0000 722b 0000 0072 1900 0000  .r*...r+...r....
-000018e0: cf00 0000 7302 0000 0000 027a 204c 696e  ....s......z Lin
-000018f0: 6543 6861 7274 4461 7461 2e61 626f 7665  eChartData.above
-00001900: 5f6c 696e 655f 6267 636f 6c6f 7263 0200  _line_bgcolorc..
-00001910: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001920: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-00001930: 017c 01a1 0201 0064 0053 0072 5700 0000  .|.....d.S.rW...
-00001940: 724a 0000 0072 4000 0000 722a 0000 0072  rJ...r@...r*...r
-00001950: 2a00 0000 722b 0000 0072 1900 0000 d300  *...r+...r......
-00001960: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
-00001970: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00001980: 0000 7306 0000 007c 006a 0053 0072 3d00  ..s....|.j.S.r=.
-00001990: 0000 a901 7236 0000 0072 2c00 0000 722a  ....r6...r,...r*
-000019a0: 0000 0072 2a00 0000 722b 0000 0072 1a00  ...r*...r+...r..
-000019b0: 0000 d800 0000 7302 0000 0000 027a 214c  ......s......z!L
-000019c0: 696e 6543 6861 7274 4461 7461 2e61 626f  ineChartData.abo
-000019d0: 7665 5f6c 696e 655f 6772 6164 6965 6e74  ve_line_gradient
-000019e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000019f0: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00001a00: 7c00 5f00 6400 5300 723d 0000 0072 5800  |._.d.S.r=...rX.
-00001a10: 0000 7240 0000 0072 2a00 0000 722a 0000  ..r@...r*...r*..
-00001a20: 0072 2b00 0000 721a 0000 00dc 0000 0073  .r+...r........s
-00001a30: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-00001a40: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00001a50: 0e00 0000 7c00 6a00 6401 6402 6403 8d02  ....|.j.d.d.d...
-00001a60: 5300 2904 4eda 1061 626f 7665 4c69 6e65  S.).N..aboveLine
-00001a70: 4375 746f 6666 5972 4400 0000 7252 0000  CutoffYrD...rR..
-00001a80: 0072 4800 0000 722c 0000 0072 2a00 0000  .rH...r,...r*...
-00001a90: 722a 0000 0072 2b00 0000 721b 0000 00e1  r*...r+...r.....
-00001aa0: 0000 0073 0200 0000 0002 7a21 4c69 6e65  ...s......z!Line
-00001ab0: 4368 6172 7444 6174 612e 6162 6f76 655f  ChartData.above_
-00001ac0: 6c69 6e65 5f63 7574 6f66 665f 7963 0200  line_cutoff_yc..
-00001ad0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001ae0: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-00001af0: 017c 01a1 0201 0064 0053 0029 024e 7259  .|.....d.S.).NrY
-00001b00: 0000 0072 4a00 0000 7240 0000 0072 2a00  ...rJ...r@...r*.
-00001b10: 0000 722a 0000 0072 2b00 0000 721b 0000  ..r*...r+...r...
-00001b20: 00e5 0000 0073 0200 0000 0002 6301 0000  .....s......c...
-00001b30: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00001b40: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00001b50: 723d 0000 00a9 0172 3800 0000 722c 0000  r=.....r8...r,..
-00001b60: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
-00001b70: 721c 0000 00ea 0000 0073 0200 0000 0002  r........s......
-00001b80: 7a18 4c69 6e65 4368 6172 7444 6174 612e  z.LineChartData.
-00001b90: 6162 6f76 655f 6c69 6e65 6302 0000 0000  above_linec.....
-00001ba0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00001bb0: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
-00001bc0: 5300 723d 0000 0072 5a00 0000 7240 0000  S.r=...rZ...r@..
-00001bd0: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
-00001be0: 721c 0000 00ee 0000 0073 0200 0000 0002  r........s......
-00001bf0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001c00: 0003 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
-00001c10: a000 6401 a101 5300 a902 4e5a 1062 656c  ..d...S...NZ.bel
-00001c20: 6f77 4c69 6e65 4267 636f 6c6f 7272 4800  owLineBgcolorrH.
-00001c30: 0000 722c 0000 0072 2a00 0000 722a 0000  ..r,...r*...r*..
-00001c40: 0072 2b00 0000 721d 0000 00f3 0000 0073  .r+...r........s
-00001c50: 0200 0000 0002 7a20 4c69 6e65 4368 6172  ......z LineChar
-00001c60: 7444 6174 612e 6265 6c6f 775f 6c69 6e65  tData.below_line
-00001c70: 5f62 6763 6f6c 6f72 6302 0000 0000 0000  _bgcolorc.......
-00001c80: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00001c90: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
-00001ca0: 0100 6400 5300 725b 0000 0072 4a00 0000  ..d.S.r[...rJ...
-00001cb0: 7240 0000 0072 2a00 0000 722a 0000 0072  r@...r*...r*...r
-00001cc0: 2b00 0000 721d 0000 00f7 0000 0073 0200  +...r........s..
-00001cd0: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00001ce0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00001cf0: 0000 7c00 6a00 5300 723d 0000 00a9 0172  ..|.j.S.r=.....r
-00001d00: 3700 0000 722c 0000 0072 2a00 0000 722a  7...r,...r*...r*
-00001d10: 0000 0072 2b00 0000 721e 0000 00fc 0000  ...r+...r.......
-00001d20: 0073 0200 0000 0002 7a21 4c69 6e65 4368  .s......z!LineCh
-00001d30: 6172 7444 6174 612e 6265 6c6f 775f 6c69  artData.below_li
-00001d40: 6e65 5f67 7261 6469 656e 7463 0200 0000  ne_gradientc....
-00001d50: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001d60: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
-00001d70: 0053 0072 3d00 0000 725c 0000 0072 4000  .S.r=...r\...r@.
-00001d80: 0000 722a 0000 0072 2a00 0000 722b 0000  ..r*...r*...r+..
-00001d90: 0072 1e00 0000 0001 0000 7302 0000 0000  .r........s.....
-00001da0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-00001db0: 0000 0400 0000 4300 0000 730e 0000 007c  ......C...s....|
-00001dc0: 006a 0064 0164 0264 038d 0253 0029 044e  .j.d.d.d...S.).N
-00001dd0: da10 6265 6c6f 774c 696e 6543 7574 6f66  ..belowLineCutof
-00001de0: 6659 7244 0000 0072 5200 0000 7248 0000  fYrD...rR...rH..
-00001df0: 0072 2c00 0000 722a 0000 0072 2a00 0000  .r,...r*...r*...
-00001e00: 722b 0000 0072 1f00 0000 0501 0000 7302  r+...r........s.
-00001e10: 0000 0000 027a 214c 696e 6543 6861 7274  .....z!LineChart
-00001e20: 4461 7461 2e62 656c 6f77 5f6c 696e 655f  Data.below_line_
-00001e30: 6375 746f 6666 5f79 6302 0000 0000 0000  cutoff_yc.......
-00001e40: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00001e50: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
-00001e60: 0100 6400 5300 2902 4e72 5d00 0000 724a  ..d.S.).Nr]...rJ
-00001e70: 0000 0072 4000 0000 722a 0000 0072 2a00  ...r@...r*...r*.
-00001e80: 0000 722b 0000 0072 1f00 0000 0901 0000  ..r+...r........
-00001e90: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00001ea0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00001eb0: 7306 0000 007c 006a 0053 0072 3d00 0000  s....|.j.S.r=...
-00001ec0: a901 7239 0000 0072 2c00 0000 722a 0000  ..r9...r,...r*..
-00001ed0: 0072 2a00 0000 722b 0000 0072 2000 0000  .r*...r+...r ...
-00001ee0: 0e01 0000 7302 0000 0000 027a 184c 696e  ....s......z.Lin
-00001ef0: 6543 6861 7274 4461 7461 2e62 656c 6f77  eChartData.below
-00001f00: 5f6c 696e 6563 0200 0000 0000 0000 0000  _linec..........
-00001f10: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-00001f20: 0000 007c 017c 005f 0064 0053 0072 3d00  ...|.|._.d.S.r=.
-00001f30: 0000 725e 0000 0072 4000 0000 722a 0000  ..r^...r@...r*..
-00001f40: 0072 2a00 0000 722b 0000 0072 2000 0000  .r*...r+...r ...
-00001f50: 1201 0000 7302 0000 0000 0263 0100 0000  ....s......c....
-00001f60: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00001f70: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
-00001f80: 3d00 0000 a901 723a 0000 0072 2c00 0000  =.....r:...r,...
-00001f90: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
-00001fa0: 2100 0000 1701 0000 7302 0000 0000 027a  !.......s......z
-00001fb0: 214c 696e 6543 6861 7274 4461 7461 2e73  !LineChartData.s
-00001fc0: 656c 6563 7465 645f 6265 6c6f 775f 6c69  elected_below_li
-00001fd0: 6e65 6302 0000 0000 0000 0000 0000 0002  nec.............
-00001fe0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00001ff0: 7c01 7c00 5f00 6400 5300 723d 0000 0072  |.|._.d.S.r=...r
-00002000: 5f00 0000 7240 0000 0072 2a00 0000 722a  _...r@...r*...r*
-00002010: 0000 0072 2b00 0000 7221 0000 001b 0100  ...r+...r!......
-00002020: 0073 0200 0000 0002 2919 4e4e 4e4e 4e4e  .s......).NNNNNN
-00002030: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
-00002040: 4e4e 4e29 2dda 085f 5f6e 616d 655f 5fda  NNN)-..__name__.
-00002050: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00002060: 7561 6c6e 616d 655f 5f72 0400 0000 7203  ualname__r....r.
-00002070: 0000 0072 0800 0000 724c 0000 00da 0373  ...r....rL.....s
-00002080: 7472 720b 0000 0072 0a00 0000 da03 696e  trr....r......in
-00002090: 7472 0d00 0000 7206 0000 0072 0500 0000  tr....r....r....
-000020a0: 7207 0000 0072 0c00 0000 7202 0000 0072  r....r....r....r
-000020b0: 2800 0000 722d 0000 0072 2f00 0000 723f  (...r-...r/...r?
-000020c0: 0000 00da 0870 726f 7065 7274 7972 0f00  .....propertyr..
-000020d0: 0000 da06 7365 7474 6572 7213 0000 0072  ....setterr....r
-000020e0: 1000 0000 7211 0000 0072 1200 0000 7214  ....r....r....r.
-000020f0: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-00002100: 0000 7218 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
-00002110: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00002120: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00002130: 1f00 0000 7220 0000 0072 2100 0000 da0d  ....r ...r!.....
-00002140: 5f5f 636c 6173 7363 656c 6c5f 5f72 2a00  __classcell__r*.
-00002150: 0000 722a 0000 0072 3b00 0000 722b 0000  ..r*...r;...r+..
-00002160: 0072 0e00 0000 0c00 0000 7316 0100 0008  .r........s.....
-00002170: 0300 0100 0100 0100 0100 0100 0100 0100  ................
-00002180: 0100 0100 0100 0100 0100 0100 0100 0100  ................
-00002190: 0100 0100 0100 0100 0100 0400 0100 0100  ................
-000021a0: 0100 e302 020a 0106 0106 0106 0102 0106  ................
-000021b0: 0106 0102 010a 0106 0106 0106 0102 0106  ................
-000021c0: 0106 0106 0102 0106 010c 010c 010c 0406  ................
-000021d0: 0106 0106 0102 e30c 4008 030c 0d08 0402  ........@.......
-000021e0: 010a 0304 010a 0402 0110 0304 0110 0402  ................
-000021f0: 0114 0304 0114 0402 0114 0304 0114 0402  ................
-00002200: 0114 0304 0114 0402 0114 0304 0114 0402  ................
-00002210: 0114 0504 0114 0402 0110 0304 0110 0402  ................
-00002220: 010a 0304 0118 0402 010a 0304 0114 0402  ................
-00002230: 010a 0304 011a 0402 010a 0304 011a 0402  ................
-00002240: 0114 0304 0114 0402 0114 0304 0114 0402  ................
-00002250: 0110 0304 0110 0402 0114 0304 0114 0402  ................
-00002260: 0114 0304 0114 0402 0114 0304 0114 0402  ................
-00002270: 0110 0304 0110 0402 0114 0304 0114 0402  ................
-00002280: 011a 0304 0172 0e00 0000 4e29 15da 0674  .....r....N)...t
-00002290: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-000022a0: 0400 0000 7205 0000 00da 2166 6c65 745f  ....r.....!flet_
-000022b0: 636f 7265 2e63 6861 7274 732e 6368 6172  core.charts.char
-000022c0: 745f 706f 696e 745f 6c69 6e65 7206 0000  t_point_liner...
-000022d0: 00da 2266 6c65 745f 636f 7265 2e63 6861  .."flet_core.cha
-000022e0: 7274 732e 6368 6172 745f 706f 696e 745f  rts.chart_point_
-000022f0: 7368 6170 6572 0700 0000 da26 666c 6574  shaper.....&flet
-00002300: 5f63 6f72 652e 6368 6172 7473 2e6c 696e  _core.charts.lin
-00002310: 655f 6368 6172 745f 6461 7461 5f70 6f69  e_chart_data_poi
-00002320: 6e74 7208 0000 00da 1166 6c65 745f 636f  ntr......flet_co
-00002330: 7265 2e63 6f6e 7472 6f6c 7209 0000 0072  re.controlr....r
-00002340: 0a00 0000 da13 666c 6574 5f63 6f72 652e  ......flet_core.
-00002350: 6772 6164 6965 6e74 7372 0b00 0000 da0d  gradientsr......
-00002360: 666c 6574 5f63 6f72 652e 7265 6672 0c00  flet_core.refr..
-00002370: 0000 da10 666c 6574 5f63 6f72 652e 7368  ....flet_core.sh
-00002380: 6164 6f77 720d 0000 0072 0e00 0000 722a  adowr....r....r*
-00002390: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
-000023a0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000023b0: 7310 0000 0018 020c 010c 010c 0110 010c  s...............
-000023c0: 010c 010c 03                             .....
+00000940: 6266 6c65 742f 666c 6574 636f 6e74 7269  bflet/fletcontri
+00000950: 622f 7364 6b2f 7079 7468 6f6e 2f70 6163  b/sdk/python/pac
+00000960: 6b61 6765 732f 666c 6574 2d63 6f72 652f  kages/flet-core/
+00000970: 7372 632f 666c 6574 5f63 6f72 652f 6368  src/flet_core/ch
+00000980: 6172 7473 2f6c 696e 655f 6368 6172 745f  arts/line_chart_
+00000990: 6461 7461 2e70 7972 2800 0000 0d00 0000  data.pyr(.......
+000009a0: 733a 0000 0000 2004 0102 0102 0102 0102  s:.... .........
+000009b0: 0102 fb06 0806 0106 0106 0106 0106 0106  ................
+000009c0: 0106 0202 ff04 0306 0106 0106 0106 0106  ................
+000009d0: 0106 0106 0106 0106 0106 0106 0106 017a  ...............z
+000009e0: 164c 696e 6543 6861 7274 4461 7461 2e5f  .LineChartData._
+000009f0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000a00: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000a10: 7304 0000 0064 0153 0029 024e 7227 0000  s....d.S.).Nr'..
+00000a20: 0072 2a00 0000 a901 7229 0000 0072 2a00  .r*.....r)...r*.
+00000a30: 0000 722a 0000 0072 2b00 0000 da11 5f67  ..r*...r+....._g
+00000a40: 6574 5f63 6f6e 7472 6f6c 5f6e 616d 654d  et_control_nameM
+00000a50: 0000 0073 0200 0000 0001 7a1f 4c69 6e65  ...s......z.Line
+00000a60: 4368 6172 7444 6174 612e 5f67 6574 5f63  ChartData._get_c
+00000a70: 6f6e 7472 6f6c 5f6e 616d 6563 0100 0000  ontrol_namec....
+00000a80: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000a90: 0300 0000 739a 0000 0074 0083 00a0 01a1  ....s....t......
+00000aa0: 0001 007c 00a0 0264 017c 006a 03a1 0201  ...|...d.|.j....
+00000ab0: 007c 00a0 0264 027c 006a 04a1 0201 007c  .|...d.|.j.....|
+00000ac0: 00a0 0264 037c 006a 05a1 0201 007c 00a0  ...d.|.j.....|..
+00000ad0: 0264 047c 006a 06a1 0201 007c 00a0 0264  .d.|.j.....|...d
+00000ae0: 057c 006a 07a1 0201 007c 00a0 0264 067c  .|.j.....|...d.|
+00000af0: 006a 08a1 0201 007c 00a0 0264 077c 006a  .j.....|...d.|.j
+00000b00: 09a1 0201 007c 00a0 0264 087c 006a 0aa1  .....|...d.|.j..
+00000b10: 0201 007c 00a0 0264 097c 006a 0ba1 0201  ...|...d.|.j....
+00000b20: 007c 00a0 0264 0a7c 006a 0ca1 0201 0064  .|...d.|.j.....d
+00000b30: 0053 0029 0b4e 7212 0000 0072 1800 0000  .S.).Nr....r....
+00000b40: 7222 0000 005a 0d73 656c 6563 7465 6450  r"...Z.selectedP
+00000b50: 6f69 6e74 5a0b 6461 7368 5061 7474 6572  ointZ.dashPatter
+00000b60: 6e5a 1161 626f 7665 4c69 6e65 4772 6164  nZ.aboveLineGrad
+00000b70: 6965 6e74 5a11 6265 6c6f 774c 696e 6547  ientZ.belowLineG
+00000b80: 7261 6469 656e 745a 0961 626f 7665 4c69  radientZ.aboveLi
+00000b90: 6e65 5a09 6265 6c6f 774c 696e 655a 1173  neZ.belowLineZ.s
+00000ba0: 656c 6563 7465 6442 656c 6f77 4c69 6e65  electedBelowLine
+00000bb0: 290d da05 7375 7065 72da 0d62 6566 6f72  )...super..befor
+00000bc0: 655f 7570 6461 7465 da0e 5f73 6574 5f61  e_update.._set_a
+00000bd0: 7474 725f 6a73 6f6e da18 5f4c 696e 6543  ttr_json.._LineC
+00000be0: 6861 7274 4461 7461 5f5f 6772 6164 6965  hartData__gradie
+00000bf0: 6e74 da16 5f4c 696e 6543 6861 7274 4461  nt.._LineChartDa
+00000c00: 7461 5f5f 7368 6164 6f77 da15 5f4c 696e  ta__shadow.._Lin
+00000c10: 6543 6861 7274 4461 7461 5f5f 706f 696e  eChartData__poin
+00000c20: 74da 1e5f 4c69 6e65 4368 6172 7444 6174  t.._LineChartDat
+00000c30: 615f 5f73 656c 6563 7465 645f 706f 696e  a__selected_poin
+00000c40: 74da 1c5f 4c69 6e65 4368 6172 7444 6174  t.._LineChartDat
+00000c50: 615f 5f64 6173 685f 7061 7474 6572 6eda  a__dash_pattern.
+00000c60: 235f 4c69 6e65 4368 6172 7444 6174 615f  #_LineChartData_
+00000c70: 5f61 626f 7665 5f6c 696e 655f 6772 6164  _above_line_grad
+00000c80: 6965 6e74 da23 5f4c 696e 6543 6861 7274  ient.#_LineChart
+00000c90: 4461 7461 5f5f 6265 6c6f 775f 6c69 6e65  Data__below_line
+00000ca0: 5f67 7261 6469 656e 74da 1a5f 4c69 6e65  _gradient.._Line
+00000cb0: 4368 6172 7444 6174 615f 5f61 626f 7665  ChartData__above
+00000cc0: 5f6c 696e 65da 1a5f 4c69 6e65 4368 6172  _line.._LineChar
+00000cd0: 7444 6174 615f 5f62 656c 6f77 5f6c 696e  tData__below_lin
+00000ce0: 65da 235f 4c69 6e65 4368 6172 7444 6174  e.#_LineChartDat
+00000cf0: 615f 5f73 656c 6563 7465 645f 6265 6c6f  a__selected_belo
+00000d00: 775f 6c69 6e65 722c 0000 00a9 01da 095f  w_liner,......._
+00000d10: 5f63 6c61 7373 5f5f 722a 0000 0072 2b00  _class__r*...r+.
+00000d20: 0000 722f 0000 0050 0000 0073 1600 0000  ..r/...P...s....
+00000d30: 0001 0a01 0e01 0e01 0e01 0e01 0e01 0e01  ................
+00000d40: 0e01 0e01 0e01 7a1b 4c69 6e65 4368 6172  ......z.LineChar
+00000d50: 7444 6174 612e 6265 666f 7265 5f75 7064  tData.before_upd
+00000d60: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
+00000d70: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00000d80: 007c 006a 0053 00a9 014e a901 5a1b 5f4c  .|.j.S...N..Z._L
+00000d90: 696e 6543 6861 7274 4461 7461 5f5f 6461  ineChartData__da
+00000da0: 7461 5f70 6f69 6e74 7372 2c00 0000 722a  ta_pointsr,...r*
+00000db0: 0000 0072 2a00 0000 722b 0000 00da 0d5f  ...r*...r+....._
+00000dc0: 6765 745f 6368 696c 6472 656e 5d00 0000  get_children]...
+00000dd0: 7302 0000 0000 017a 1b4c 696e 6543 6861  s......z.LineCha
+00000de0: 7274 4461 7461 2e5f 6765 745f 6368 696c  rtData._get_chil
+00000df0: 6472 656e 6301 0000 0000 0000 0000 0000  drenc...........
+00000e00: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+00000e10: 0000 7c00 6a00 5300 723d 0000 0072 3e00  ..|.j.S.r=...r>.
+00000e20: 0000 722c 0000 0072 2a00 0000 722a 0000  ..r,...r*...r*..
+00000e30: 0072 2b00 0000 720f 0000 0061 0000 0073  .r+...r....a...s
+00000e40: 0200 0000 0002 7a19 4c69 6e65 4368 6172  ......z.LineChar
+00000e50: 7444 6174 612e 6461 7461 5f70 6f69 6e74  tData.data_point
+00000e60: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+00000e70: 0000 0200 0000 4300 0000 7316 0000 007c  ......C...s....|
+00000e80: 0164 0075 0172 0c7c 016e 0267 007c 005f  .d.u.r.|.n.g.|._
+00000e90: 0064 0053 0072 3d00 0000 723e 0000 00a9  .d.S.r=...r>....
+00000ea0: 0272 2900 0000 da05 7661 6c75 6572 2a00  .r).....valuer*.
+00000eb0: 0000 722a 0000 0072 2b00 0000 720f 0000  ..r*...r+...r...
+00000ec0: 0065 0000 0073 0200 0000 0002 2901 da06  .e...s......)...
+00000ed0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000ee0: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
+00000ef0: 1000 0000 7c00 6a00 6401 6402 6403 6404  ....|.j.d.d.d.d.
+00000f00: 8d03 5300 2905 4eda 0b73 7472 6f6b 6557  ..S.).N..strokeW
+00000f10: 6964 7468 da05 666c 6f61 7467 0000 0000  idth..floatg....
+00000f20: 0000 f03f a902 da09 6461 7461 5f74 7970  ...?....data_typ
+00000f30: 65da 0964 6566 5f76 616c 7565 a901 da09  e..def_value....
+00000f40: 5f67 6574 5f61 7474 7272 2c00 0000 722a  _get_attrr,...r*
+00000f50: 0000 0072 2a00 0000 722b 0000 0072 1300  ...r*...r+...r..
+00000f60: 0000 6a00 0000 7302 0000 0000 027a 1a4c  ..j...s......z.L
+00000f70: 696e 6543 6861 7274 4461 7461 2e73 7472  ineChartData.str
+00000f80: 6f6b 655f 7769 6474 6829 0172 4100 0000  oke_width).rA...
+00000f90: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000fa0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00000fb0: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
+00000fc0: 4e72 4300 0000 a901 da09 5f73 6574 5f61  NrC......._set_a
+00000fd0: 7474 7272 4000 0000 722a 0000 0072 2a00  ttrr@...r*...r*.
+00000fe0: 0000 722b 0000 0072 1300 0000 6e00 0000  ..r+...r....n...
+00000ff0: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00001000: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+00001010: 7310 0000 007c 006a 0064 0164 0264 0364  s....|.j.d.d.d.d
+00001020: 048d 0353 0029 054e 7210 0000 00da 0462  ...S.).Nr......b
+00001030: 6f6f 6c46 7245 0000 0072 4800 0000 722c  oolFrE...rH...r,
+00001040: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
+00001050: 0000 7210 0000 0073 0000 0073 0200 0000  ..r....s...s....
+00001060: 0002 7a14 4c69 6e65 4368 6172 7444 6174  ..z.LineChartDat
+00001070: 612e 6375 7276 6564 6302 0000 0000 0000  a.curvedc.......
+00001080: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00001090: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
+000010a0: 0100 6400 5300 2902 4e72 1000 0000 724a  ..d.S.).Nr....rJ
+000010b0: 0000 0072 4000 0000 722a 0000 0072 2a00  ...r@...r*...r*.
+000010c0: 0000 722b 0000 0072 1000 0000 7700 0000  ..r+...r....w...
+000010d0: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+000010e0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+000010f0: 730a 0000 007c 00a0 0064 01a1 0153 00a9  s....|...d...S..
+00001100: 024e 7211 0000 0072 4800 0000 722c 0000  .Nr....rH...r,..
+00001110: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
+00001120: 7211 0000 007c 0000 0073 0200 0000 0002  r....|...s......
+00001130: 7a13 4c69 6e65 4368 6172 7444 6174 612e  z.LineChartData.
+00001140: 636f 6c6f 7263 0200 0000 0000 0000 0000  colorc..........
+00001150: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+00001160: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+00001170: 0053 0072 4d00 0000 724a 0000 0072 4000  .S.rM...rJ...r@.
+00001180: 0000 722a 0000 0072 2a00 0000 722b 0000  ..r*...r*...r+..
+00001190: 0072 1100 0000 8000 0000 7302 0000 0000  .r........s.....
+000011a0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+000011b0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+000011c0: 006a 0053 0072 3d00 0000 a901 7231 0000  .j.S.r=.....r1..
+000011d0: 0072 2c00 0000 722a 0000 0072 2a00 0000  .r,...r*...r*...
+000011e0: 722b 0000 0072 1200 0000 8500 0000 7302  r+...r........s.
+000011f0: 0000 0000 027a 164c 696e 6543 6861 7274  .....z.LineChart
+00001200: 4461 7461 2e67 7261 6469 656e 7463 0200  Data.gradientc..
+00001210: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00001220: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
+00001230: 0064 0053 0072 3d00 0000 724e 0000 0072  .d.S.r=...rN...r
+00001240: 4000 0000 722a 0000 0072 2a00 0000 722b  @...r*...r*...r+
+00001250: 0000 0072 1200 0000 8900 0000 7302 0000  ...r........s...
+00001260: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00001270: 0100 0000 0500 0000 4300 0000 7310 0000  ........C...s...
+00001280: 007c 006a 0064 0164 0264 0364 048d 0353  .|.j.d.d.d.d...S
+00001290: 0029 054e da0e 7374 726f 6b65 4361 7052  .).N..strokeCapR
+000012a0: 6f75 6e64 724c 0000 0046 7245 0000 0072  oundrL...FrE...r
+000012b0: 4800 0000 722c 0000 0072 2a00 0000 722a  H...r,...r*...r*
+000012c0: 0000 0072 2b00 0000 7214 0000 008e 0000  ...r+...r.......
+000012d0: 0073 0200 0000 0002 7a1e 4c69 6e65 4368  .s......z.LineCh
+000012e0: 6172 7444 6174 612e 7374 726f 6b65 5f63  artData.stroke_c
+000012f0: 6170 5f72 6f75 6e64 6302 0000 0000 0000  ap_roundc.......
+00001300: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00001310: 0073 1000 0000 7c00 a000 6401 7c01 a102  .s....|...d.|...
+00001320: 0100 6400 5300 2902 4e72 4f00 0000 724a  ..d.S.).NrO...rJ
+00001330: 0000 0072 4000 0000 722a 0000 0072 2a00  ...r@...r*...r*.
+00001340: 0000 722b 0000 0072 1400 0000 9200 0000  ..r+...r........
+00001350: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00001360: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+00001370: 7310 0000 007c 006a 0064 0164 0264 0364  s....|.j.d.d.d.d
+00001380: 048d 0353 0029 054e da18 7072 6576 656e  ...S.).N..preven
+00001390: 7443 7572 7665 4f76 6572 5368 6f6f 7469  tCurveOverShooti
+000013a0: 6e67 724c 0000 0046 7245 0000 0072 4800  ngrL...FrE...rH.
+000013b0: 0000 722c 0000 0072 2a00 0000 722a 0000  ..r,...r*...r*..
+000013c0: 0072 2b00 0000 7215 0000 0097 0000 0073  .r+...r........s
+000013d0: 0600 0000 0002 0401 06ff 7a29 4c69 6e65  ..........z)Line
+000013e0: 4368 6172 7444 6174 612e 7072 6576 656e  ChartData.preven
+000013f0: 745f 6375 7276 655f 6f76 6572 5f73 686f  t_curve_over_sho
+00001400: 6f74 696e 6763 0200 0000 0000 0000 0000  otingc..........
+00001410: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
+00001420: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
+00001430: 0053 0029 024e 7250 0000 0072 4a00 0000  .S.).NrP...rJ...
+00001440: 7240 0000 0072 2a00 0000 722a 0000 0072  r@...r*...r*...r
+00001450: 2b00 0000 7215 0000 009d 0000 0073 0200  +...r........s..
+00001460: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
+00001470: 0001 0000 0004 0000 0043 0000 0073 0e00  .........C...s..
+00001480: 0000 7c00 6a00 6401 6402 6403 8d02 5300  ..|.j.d.d.d...S.
+00001490: 2904 4eda 2170 7265 7665 6e74 4375 7276  ).N.!preventCurv
+000014a0: 654f 7665 7253 686f 6f74 696e 6754 6872  eOverShootingThr
+000014b0: 6573 686f 6c64 7244 0000 00a9 0172 4600  esholdrD.....rF.
+000014c0: 0000 7248 0000 0072 2c00 0000 722a 0000  ..rH...r,...r*..
+000014d0: 0072 2a00 0000 722b 0000 0072 1600 0000  .r*...r+...r....
+000014e0: a200 0000 7302 0000 0000 027a 334c 696e  ....s......z3Lin
+000014f0: 6543 6861 7274 4461 7461 2e70 7265 7665  eChartData.preve
+00001500: 6e74 5f63 7572 7665 5f6f 7665 725f 7368  nt_curve_over_sh
+00001510: 6f6f 7469 6e67 5f74 6872 6573 686f 6c64  ooting_threshold
+00001520: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001530: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00001540: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
+00001550: 4e72 5100 0000 724a 0000 0072 4000 0000  NrQ...rJ...r@...
+00001560: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
+00001570: 1600 0000 a600 0000 7302 0000 0000 0263  ........s......c
+00001580: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001590: 0100 0000 4300 0000 7306 0000 007c 006a  ....C...s....|.j
+000015a0: 0053 0072 3d00 0000 a901 7235 0000 0072  .S.r=.....r5...r
+000015b0: 2c00 0000 722a 0000 0072 2a00 0000 722b  ,...r*...r*...r+
+000015c0: 0000 0072 1700 0000 ab00 0000 7302 0000  ...r........s...
+000015d0: 0000 027a 1a4c 696e 6543 6861 7274 4461  ...z.LineChartDa
+000015e0: 7461 2e64 6173 685f 7061 7474 6572 6e63  ta.dash_patternc
+000015f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001600: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
+00001610: 005f 0064 0053 0072 3d00 0000 7253 0000  ._.d.S.r=...rS..
+00001620: 0072 4000 0000 722a 0000 0072 2a00 0000  .r@...r*...r*...
+00001630: 722b 0000 0072 1700 0000 af00 0000 7302  r+...r........s.
+00001640: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00001650: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00001660: 0000 007c 006a 0053 0072 3d00 0000 a901  ...|.j.S.r=.....
+00001670: 7232 0000 0072 2c00 0000 722a 0000 0072  r2...r,...r*...r
+00001680: 2a00 0000 722b 0000 0072 1800 0000 b400  *...r+...r......
+00001690: 0000 7302 0000 0000 027a 144c 696e 6543  ..s......z.LineC
+000016a0: 6861 7274 4461 7461 2e73 6861 646f 7763  hartData.shadowc
+000016b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000016c0: 0200 0000 4300 0000 730a 0000 007c 017c  ....C...s....|.|
+000016d0: 005f 0064 0053 0072 3d00 0000 7254 0000  ._.d.S.r=...rT..
+000016e0: 0072 4000 0000 722a 0000 0072 2a00 0000  .r@...r*...r*...
+000016f0: 722b 0000 0072 1800 0000 b800 0000 7302  r+...r........s.
+00001700: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00001710: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00001720: 0000 007c 006a 0053 0072 3d00 0000 a901  ...|.j.S.r=.....
+00001730: 7233 0000 0072 2c00 0000 722a 0000 0072  r3...r,...r*...r
+00001740: 2a00 0000 722b 0000 0072 2200 0000 bd00  *...r+...r".....
+00001750: 0000 7302 0000 0000 027a 134c 696e 6543  ..s......z.LineC
+00001760: 6861 7274 4461 7461 2e70 6f69 6e74 6302  hartData.pointc.
+00001770: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00001780: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
+00001790: 5f00 6400 5300 723d 0000 0072 5500 0000  _.d.S.r=...rU...
+000017a0: 7240 0000 0072 2a00 0000 722a 0000 0072  r@...r*...r*...r
+000017b0: 2b00 0000 7222 0000 00c1 0000 0073 0200  +...r".......s..
+000017c0: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
+000017d0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+000017e0: 0000 7c00 6a00 5300 723d 0000 00a9 0172  ..|.j.S.r=.....r
+000017f0: 3400 0000 722c 0000 0072 2a00 0000 722a  4...r,...r*...r*
+00001800: 0000 0072 2b00 0000 7223 0000 00c6 0000  ...r+...r#......
+00001810: 0073 0200 0000 0002 7a1c 4c69 6e65 4368  .s......z.LineCh
+00001820: 6172 7444 6174 612e 7365 6c65 6374 6564  artData.selected
+00001830: 5f70 6f69 6e74 6302 0000 0000 0000 0000  _pointc.........
+00001840: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00001850: 0a00 0000 7c01 7c00 5f00 6400 5300 723d  ....|.|._.d.S.r=
+00001860: 0000 0072 5600 0000 7240 0000 0072 2a00  ...rV...r@...r*.
+00001870: 0000 722a 0000 0072 2b00 0000 7223 0000  ..r*...r+...r#..
+00001880: 00ca 0000 0073 0200 0000 0002 6301 0000  .....s......c...
+00001890: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000018a0: 0043 0000 0073 0a00 0000 7c00 a000 6401  .C...s....|...d.
+000018b0: a101 5300 a902 4e5a 1061 626f 7665 4c69  ..S...NZ.aboveLi
+000018c0: 6e65 4267 636f 6c6f 7272 4800 0000 722c  neBgcolorrH...r,
+000018d0: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
+000018e0: 0000 7219 0000 00cf 0000 0073 0200 0000  ..r........s....
+000018f0: 0002 7a20 4c69 6e65 4368 6172 7444 6174  ..z LineChartDat
+00001900: 612e 6162 6f76 655f 6c69 6e65 5f62 6763  a.above_line_bgc
+00001910: 6f6c 6f72 6302 0000 0000 0000 0000 0000  olorc...........
+00001920: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+00001930: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+00001940: 5300 7257 0000 0072 4a00 0000 7240 0000  S.rW...rJ...r@..
+00001950: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
+00001960: 7219 0000 00d3 0000 0073 0200 0000 0002  r........s......
+00001970: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001980: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+00001990: 6a00 5300 723d 0000 00a9 0172 3600 0000  j.S.r=.....r6...
+000019a0: 722c 0000 0072 2a00 0000 722a 0000 0072  r,...r*...r*...r
+000019b0: 2b00 0000 721a 0000 00d8 0000 0073 0200  +...r........s..
+000019c0: 0000 0002 7a21 4c69 6e65 4368 6172 7444  ....z!LineChartD
+000019d0: 6174 612e 6162 6f76 655f 6c69 6e65 5f67  ata.above_line_g
+000019e0: 7261 6469 656e 7463 0200 0000 0000 0000  radientc........
+000019f0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00001a00: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
+00001a10: 3d00 0000 7258 0000 0072 4000 0000 722a  =...rX...r@...r*
+00001a20: 0000 0072 2a00 0000 722b 0000 0072 1a00  ...r*...r+...r..
+00001a30: 0000 dc00 0000 7302 0000 0000 0263 0100  ......s......c..
+00001a40: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00001a50: 0000 4300 0000 730e 0000 007c 006a 0064  ..C...s....|.j.d
+00001a60: 0164 0264 038d 0253 0029 044e da10 6162  .d.d...S.).N..ab
+00001a70: 6f76 654c 696e 6543 7574 6f66 6659 7244  oveLineCutoffYrD
+00001a80: 0000 0072 5200 0000 7248 0000 0072 2c00  ...rR...rH...r,.
+00001a90: 0000 722a 0000 0072 2a00 0000 722b 0000  ..r*...r*...r+..
+00001aa0: 0072 1b00 0000 e100 0000 7302 0000 0000  .r........s.....
+00001ab0: 027a 214c 696e 6543 6861 7274 4461 7461  .z!LineChartData
+00001ac0: 2e61 626f 7665 5f6c 696e 655f 6375 746f  .above_line_cuto
+00001ad0: 6666 5f79 6302 0000 0000 0000 0000 0000  ff_yc...........
+00001ae0: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+00001af0: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+00001b00: 5300 2902 4e72 5900 0000 724a 0000 0072  S.).NrY...rJ...r
+00001b10: 4000 0000 722a 0000 0072 2a00 0000 722b  @...r*...r*...r+
+00001b20: 0000 0072 1b00 0000 e500 0000 7302 0000  ...r........s...
+00001b30: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00001b40: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00001b50: 007c 006a 0053 0072 3d00 0000 a901 7238  .|.j.S.r=.....r8
+00001b60: 0000 0072 2c00 0000 722a 0000 0072 2a00  ...r,...r*...r*.
+00001b70: 0000 722b 0000 0072 1c00 0000 ea00 0000  ..r+...r........
+00001b80: 7302 0000 0000 027a 184c 696e 6543 6861  s......z.LineCha
+00001b90: 7274 4461 7461 2e61 626f 7665 5f6c 696e  rtData.above_lin
+00001ba0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00001bb0: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
+00001bc0: 017c 005f 0064 0053 0072 3d00 0000 725a  .|._.d.S.r=...rZ
+00001bd0: 0000 0072 4000 0000 722a 0000 0072 2a00  ...r@...r*...r*.
+00001be0: 0000 722b 0000 0072 1c00 0000 ee00 0000  ..r+...r........
+00001bf0: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00001c00: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00001c10: 730a 0000 007c 00a0 0064 01a1 0153 00a9  s....|...d...S..
+00001c20: 024e 5a10 6265 6c6f 774c 696e 6542 6763  .NZ.belowLineBgc
+00001c30: 6f6c 6f72 7248 0000 0072 2c00 0000 722a  olorrH...r,...r*
+00001c40: 0000 0072 2a00 0000 722b 0000 0072 1d00  ...r*...r+...r..
+00001c50: 0000 f300 0000 7302 0000 0000 027a 204c  ......s......z L
+00001c60: 696e 6543 6861 7274 4461 7461 2e62 656c  ineChartData.bel
+00001c70: 6f77 5f6c 696e 655f 6267 636f 6c6f 7263  ow_line_bgcolorc
+00001c80: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001c90: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+00001ca0: 0064 017c 01a1 0201 0064 0053 0072 5b00  .d.|.....d.S.r[.
+00001cb0: 0000 724a 0000 0072 4000 0000 722a 0000  ..rJ...r@...r*..
+00001cc0: 0072 2a00 0000 722b 0000 0072 1d00 0000  .r*...r+...r....
+00001cd0: f700 0000 7302 0000 0000 0263 0100 0000  ....s......c....
+00001ce0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00001cf0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
+00001d00: 3d00 0000 a901 7237 0000 0072 2c00 0000  =.....r7...r,...
+00001d10: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
+00001d20: 1e00 0000 fc00 0000 7302 0000 0000 027a  ........s......z
+00001d30: 214c 696e 6543 6861 7274 4461 7461 2e62  !LineChartData.b
+00001d40: 656c 6f77 5f6c 696e 655f 6772 6164 6965  elow_line_gradie
+00001d50: 6e74 6302 0000 0000 0000 0000 0000 0002  ntc.............
+00001d60: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00001d70: 7c01 7c00 5f00 6400 5300 723d 0000 0072  |.|._.d.S.r=...r
+00001d80: 5c00 0000 7240 0000 0072 2a00 0000 722a  \...r@...r*...r*
+00001d90: 0000 0072 2b00 0000 721e 0000 0000 0100  ...r+...r.......
+00001da0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
+00001db0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00001dc0: 0073 0e00 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
+00001dd0: 8d02 5300 2904 4eda 1062 656c 6f77 4c69  ..S.).N..belowLi
+00001de0: 6e65 4375 746f 6666 5972 4400 0000 7252  neCutoffYrD...rR
+00001df0: 0000 0072 4800 0000 722c 0000 0072 2a00  ...rH...r,...r*.
+00001e00: 0000 722a 0000 0072 2b00 0000 721f 0000  ..r*...r+...r...
+00001e10: 0005 0100 0073 0200 0000 0002 7a21 4c69  .....s......z!Li
+00001e20: 6e65 4368 6172 7444 6174 612e 6265 6c6f  neChartData.belo
+00001e30: 775f 6c69 6e65 5f63 7574 6f66 665f 7963  w_line_cutoff_yc
+00001e40: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001e50: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
+00001e60: 0064 017c 01a1 0201 0064 0053 0029 024e  .d.|.....d.S.).N
+00001e70: 725d 0000 0072 4a00 0000 7240 0000 0072  r]...rJ...r@...r
+00001e80: 2a00 0000 722a 0000 0072 2b00 0000 721f  *...r*...r+...r.
+00001e90: 0000 0009 0100 0073 0200 0000 0002 6301  .......s......c.
+00001ea0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00001eb0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+00001ec0: 5300 723d 0000 00a9 0172 3900 0000 722c  S.r=.....r9...r,
+00001ed0: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
+00001ee0: 0000 7220 0000 000e 0100 0073 0200 0000  ..r .......s....
+00001ef0: 0002 7a18 4c69 6e65 4368 6172 7444 6174  ..z.LineChartDat
+00001f00: 612e 6265 6c6f 775f 6c69 6e65 6302 0000  a.below_linec...
+00001f10: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00001f20: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00001f30: 6400 5300 723d 0000 0072 5e00 0000 7240  d.S.r=...r^...r@
+00001f40: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
+00001f50: 0000 7220 0000 0012 0100 0073 0200 0000  ..r .......s....
+00001f60: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00001f70: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
+00001f80: 7c00 6a00 5300 723d 0000 00a9 0172 3a00  |.j.S.r=.....r:.
+00001f90: 0000 722c 0000 0072 2a00 0000 722a 0000  ..r,...r*...r*..
+00001fa0: 0072 2b00 0000 7221 0000 0017 0100 0073  .r+...r!.......s
+00001fb0: 0200 0000 0002 7a21 4c69 6e65 4368 6172  ......z!LineChar
+00001fc0: 7444 6174 612e 7365 6c65 6374 6564 5f62  tData.selected_b
+00001fd0: 656c 6f77 5f6c 696e 6563 0200 0000 0000  elow_linec......
+00001fe0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00001ff0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+00002000: 0072 3d00 0000 725f 0000 0072 4000 0000  .r=...r_...r@...
+00002010: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
+00002020: 2100 0000 1b01 0000 7302 0000 0000 0229  !.......s......)
+00002030: 194e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  .NNNNNNNNNNNNNNN
+00002040: 4e4e 4e4e 4e4e 4e4e 4e4e 292d da08 5f5f  NNNNNNNNNN)-..__
+00002050: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00002060: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00002070: 7204 0000 0072 0300 0000 7208 0000 0072  r....r....r....r
+00002080: 4c00 0000 da03 7374 7272 0b00 0000 720a  L.....strr....r.
+00002090: 0000 00da 0369 6e74 720d 0000 0072 0600  .....intr....r..
+000020a0: 0000 7205 0000 0072 0700 0000 720c 0000  ..r....r....r...
+000020b0: 0072 0200 0000 7228 0000 0072 2d00 0000  .r....r(...r-...
+000020c0: 722f 0000 0072 3f00 0000 da08 7072 6f70  r/...r?.....prop
+000020d0: 6572 7479 720f 0000 00da 0673 6574 7465  ertyr......sette
+000020e0: 7272 1300 0000 7210 0000 0072 1100 0000  rr....r....r....
+000020f0: 7212 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00002100: 1600 0000 7217 0000 0072 1800 0000 7222  ....r....r....r"
+00002110: 0000 0072 2300 0000 7219 0000 0072 1a00  ...r#...r....r..
+00002120: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00002130: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00002140: 7221 0000 00da 0d5f 5f63 6c61 7373 6365  r!.....__classce
+00002150: 6c6c 5f5f 722a 0000 0072 2a00 0000 723b  ll__r*...r*...r;
+00002160: 0000 0072 2b00 0000 720e 0000 000c 0000  ...r+...r.......
+00002170: 0073 1601 0000 0803 0001 0001 0001 0001  .s..............
+00002180: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+00002190: 0001 0001 0001 0001 0001 0001 0001 0001  ................
+000021a0: 0004 0001 0001 0001 00e3 0202 0a01 0601  ................
+000021b0: 0601 0601 0201 0601 0601 0201 0a01 0601  ................
+000021c0: 0601 0601 0201 0601 0601 0601 0201 0601  ................
+000021d0: 0c01 0c01 0c04 0601 0601 0601 02e3 0c40  ...............@
+000021e0: 0803 0c0d 0804 0201 0a03 0401 0a04 0201  ................
+000021f0: 1003 0401 1004 0201 1403 0401 1404 0201  ................
+00002200: 1403 0401 1404 0201 1403 0401 1404 0201  ................
+00002210: 1403 0401 1404 0201 1405 0401 1404 0201  ................
+00002220: 1003 0401 1004 0201 0a03 0401 1804 0201  ................
+00002230: 0a03 0401 1404 0201 0a03 0401 1a04 0201  ................
+00002240: 0a03 0401 1a04 0201 1403 0401 1404 0201  ................
+00002250: 1403 0401 1404 0201 1003 0401 1004 0201  ................
+00002260: 1403 0401 1404 0201 1403 0401 1404 0201  ................
+00002270: 1403 0401 1404 0201 1003 0401 1004 0201  ................
+00002280: 1403 0401 1404 0201 1a03 0401 720e 0000  ............r...
+00002290: 004e 2915 da06 7479 7069 6e67 7202 0000  .N)...typingr...
+000022a0: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
+000022b0: da21 666c 6574 5f63 6f72 652e 6368 6172  .!flet_core.char
+000022c0: 7473 2e63 6861 7274 5f70 6f69 6e74 5f6c  ts.chart_point_l
+000022d0: 696e 6572 0600 0000 da22 666c 6574 5f63  iner....."flet_c
+000022e0: 6f72 652e 6368 6172 7473 2e63 6861 7274  ore.charts.chart
+000022f0: 5f70 6f69 6e74 5f73 6861 7065 7207 0000  _point_shaper...
+00002300: 00da 2666 6c65 745f 636f 7265 2e63 6861  ..&flet_core.cha
+00002310: 7274 732e 6c69 6e65 5f63 6861 7274 5f64  rts.line_chart_d
+00002320: 6174 615f 706f 696e 7472 0800 0000 da11  ata_pointr......
+00002330: 666c 6574 5f63 6f72 652e 636f 6e74 726f  flet_core.contro
+00002340: 6c72 0900 0000 720a 0000 00da 1366 6c65  lr....r......fle
+00002350: 745f 636f 7265 2e67 7261 6469 656e 7473  t_core.gradients
+00002360: 720b 0000 00da 0d66 6c65 745f 636f 7265  r......flet_core
+00002370: 2e72 6566 720c 0000 00da 1066 6c65 745f  .refr......flet_
+00002380: 636f 7265 2e73 6861 646f 7772 0d00 0000  core.shadowr....
+00002390: 720e 0000 0072 2a00 0000 722a 0000 0072  r....r*...r*...r
+000023a0: 2a00 0000 722b 0000 00da 083c 6d6f 6475  *...r+.....<modu
+000023b0: 6c65 3e01 0000 0073 1000 0000 1802 0c01  le>....s........
+000023c0: 0c01 0c01 1001 0c01 0c01 0c03            ............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 5338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 da14 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 da14 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -90,282 +90,283 @@
 00000590: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
 000005a0: 2911 da04 7365 6c66 720d 0000 0072 0e00  )...selfr....r..
 000005b0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
 000005c0: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
 000005d0: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
 000005e0: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
 000005f0: 0000 0072 1c00 0000 a900 721f 0000 00fa  ...r......r.....
-00000600: 682f 776f 726b 7370 6163 6573 2f63 6f6e  h/workspaces/con
-00000610: 7472 6962 666c 6574 2f66 6c65 742f 7364  tribflet/flet/sd
-00000620: 6b2f 7079 7468 6f6e 2f70 6163 6b61 6765  k/python/package
-00000630: 732f 666c 6574 2d63 6f72 652f 7372 632f  s/flet-core/src/
-00000640: 666c 6574 5f63 6f72 652f 6368 6172 7473  flet_core/charts
-00000650: 2f6c 696e 655f 6368 6172 745f 6461 7461  /line_chart_data
-00000660: 5f70 6f69 6e74 2e70 7972 1d00 0000 0c00  _point.pyr......
-00000670: 0000 7326 0000 0000 1704 0102 0102 0102  ..s&............
-00000680: 0102 0102 fb06 0806 0106 0106 0106 0106  ................
-00000690: 0106 0106 0106 0106 0106 0106 017a 1b4c  .............z.L
-000006a0: 696e 6543 6861 7274 4461 7461 506f 696e  ineChartDataPoin
-000006b0: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
-000006c0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-000006d0: 0000 0073 0400 0000 6401 5300 2902 4eda  ...s....d.S.).N.
-000006e0: 0170 721f 0000 00a9 0172 1e00 0000 721f  .pr......r....r.
-000006f0: 0000 0072 1f00 0000 7220 0000 00da 115f  ...r....r ....._
-00000700: 6765 745f 636f 6e74 726f 6c5f 6e61 6d65  get_control_name
-00000710: 3800 0000 7302 0000 0000 017a 244c 696e  8...s......z$Lin
-00000720: 6543 6861 7274 4461 7461 506f 696e 742e  eChartDataPoint.
-00000730: 5f67 6574 5f63 6f6e 7472 6f6c 5f6e 616d  _get_control_nam
-00000740: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000750: 0000 0400 0000 0300 0000 7346 0000 0074  ..........sF...t
-00000760: 0083 00a0 01a1 0001 007c 00a0 0264 017c  .........|...d.|
-00000770: 006a 03a1 0201 007c 00a0 0264 027c 006a  .j.....|...d.|.j
-00000780: 04a1 0201 007c 00a0 0264 037c 006a 05a1  .....|...d.|.j..
-00000790: 0201 007c 00a0 0264 047c 006a 06a1 0201  ...|...d.|.j....
-000007a0: 0064 0053 0029 054e 5a0c 746f 6f6c 7469  .d.S.).NZ.toolti
-000007b0: 7053 7479 6c65 7214 0000 00da 0d73 656c  pStyler......sel
-000007c0: 6563 7465 6450 6f69 6e74 da11 7365 6c65  ectedPoint..sele
-000007d0: 6374 6564 4265 6c6f 774c 696e 6529 07da  ctedBelowLine)..
-000007e0: 0573 7570 6572 da0d 6265 666f 7265 5f75  .super..before_u
-000007f0: 7064 6174 65da 0e5f 7365 745f 6174 7472  pdate.._set_attr
-00000800: 5f6a 736f 6eda 225f 4c69 6e65 4368 6172  _json."_LineChar
-00000810: 7444 6174 6150 6f69 6e74 5f5f 746f 6f6c  tDataPoint__tool
-00000820: 7469 705f 7374 796c 65da 1a5f 4c69 6e65  tip_style.._Line
-00000830: 4368 6172 7444 6174 6150 6f69 6e74 5f5f  ChartDataPoint__
-00000840: 706f 696e 74da 235f 4c69 6e65 4368 6172  point.#_LineChar
-00000850: 7444 6174 6150 6f69 6e74 5f5f 7365 6c65  tDataPoint__sele
-00000860: 6374 6564 5f70 6f69 6e74 da28 5f4c 696e  cted_point.(_Lin
-00000870: 6543 6861 7274 4461 7461 506f 696e 745f  eChartDataPoint_
-00000880: 5f73 656c 6563 7465 645f 6265 6c6f 775f  _selected_below_
-00000890: 6c69 6e65 7222 0000 00a9 01da 095f 5f63  liner".......__c
-000008a0: 6c61 7373 5f5f 721f 0000 0072 2000 0000  lass__r....r ...
-000008b0: 7227 0000 003b 0000 0073 0a00 0000 0001  r'...;...s......
-000008c0: 0a01 0e01 0e01 0e01 7a20 4c69 6e65 4368  ........z LineCh
-000008d0: 6172 7444 6174 6150 6f69 6e74 2e62 6566  artDataPoint.bef
-000008e0: 6f72 655f 7570 6461 7465 6301 0000 0000  ore_updatec.....
-000008f0: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
-00000900: 0000 0073 0800 0000 6700 7d01 7c01 5300  ...s....g.}.|.S.
-00000910: a901 4e72 1f00 0000 2902 721e 0000 00da  ..Nr....).r.....
-00000920: 0863 6869 6c64 7265 6e72 1f00 0000 721f  .childrenr....r.
-00000930: 0000 0072 2000 0000 da0d 5f67 6574 5f63  ...r ....._get_c
-00000940: 6869 6c64 7265 6e42 0000 0073 0400 0000  hildrenB...s....
-00000950: 0001 0401 7a20 4c69 6e65 4368 6172 7444  ....z LineChartD
-00000960: 6174 6150 6f69 6e74 2e5f 6765 745f 6368  ataPoint._get_ch
-00000970: 696c 6472 656e 2901 da06 7265 7475 726e  ildren)...return
-00000980: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000990: 0005 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-000009a0: 6a00 6401 6402 6403 6404 8d03 5300 2905  j.d.d.d.d...S.).
-000009b0: 4e72 0d00 0000 da05 666c 6f61 7472 0100  Nr......floatr..
-000009c0: 0000 a902 da09 6461 7461 5f74 7970 65da  ......data_type.
-000009d0: 0964 6566 5f76 616c 7565 a901 da09 5f67  .def_value...._g
-000009e0: 6574 5f61 7474 7272 2200 0000 721f 0000  et_attrr"...r...
-000009f0: 0072 1f00 0000 7220 0000 0072 0d00 0000  .r....r ...r....
-00000a00: 4700 0000 7302 0000 0000 027a 144c 696e  G...s......z.Lin
-00000a10: 6543 6861 7274 4461 7461 506f 696e 742e  eChartDataPoint.
-00000a20: 7829 01da 0576 616c 7565 6302 0000 0000  x)...valuec.....
-00000a30: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000a40: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
-00000a50: a102 0100 6400 5300 2902 4e72 0d00 0000  ....d.S.).Nr....
-00000a60: a901 da09 5f73 6574 5f61 7474 72a9 0272  ...._set_attr..r
-00000a70: 1e00 0000 7239 0000 0072 1f00 0000 721f  ....r9...r....r.
-00000a80: 0000 0072 2000 0000 720d 0000 004b 0000  ...r ...r....K..
-00000a90: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00000aa0: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-00000ab0: 0073 1000 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
-00000ac0: 6404 8d03 5300 2905 4e72 0e00 0000 7233  d...S.).Nr....r3
-00000ad0: 0000 0072 0100 0000 7234 0000 0072 3700  ...r....r4...r7.
-00000ae0: 0000 7222 0000 0072 1f00 0000 721f 0000  ..r"...r....r...
-00000af0: 0072 2000 0000 720e 0000 0050 0000 0073  .r ...r....P...s
-00000b00: 0200 0000 0002 7a14 4c69 6e65 4368 6172  ......z.LineChar
-00000b10: 7444 6174 6150 6f69 6e74 2e79 6302 0000  tDataPoint.yc...
-00000b20: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000b30: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
-00000b40: 7c01 a102 0100 6400 5300 2902 4e72 0e00  |.....d.S.).Nr..
-00000b50: 0000 723a 0000 0072 3c00 0000 721f 0000  ..r:...r<...r...
-00000b60: 0072 1f00 0000 7220 0000 0072 0e00 0000  .r....r ...r....
-00000b70: 5400 0000 7302 0000 0000 0263 0100 0000  T...s......c....
-00000b80: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-00000b90: 4300 0000 7310 0000 007c 006a 0064 0164  C...s....|.j.d.d
-00000ba0: 0264 0364 048d 0353 0029 054e 720f 0000  .d.d...S.).Nr...
-00000bb0: 00da 0462 6f6f 6c46 7234 0000 0072 3700  ...boolFr4...r7.
-00000bc0: 0000 7222 0000 0072 1f00 0000 721f 0000  ..r"...r....r...
-00000bd0: 0072 2000 0000 720f 0000 0059 0000 0073  .r ...r....Y...s
-00000be0: 0200 0000 0002 7a1b 4c69 6e65 4368 6172  ......z.LineChar
-00000bf0: 7444 6174 6150 6f69 6e74 2e73 656c 6563  tDataPoint.selec
-00000c00: 7465 6463 0200 0000 0000 0000 0000 0000  tedc............
-00000c10: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-00000c20: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
-00000c30: 0029 024e 720f 0000 0072 3a00 0000 723c  .).Nr....r:...r<
-00000c40: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
-00000c50: 0000 720f 0000 005d 0000 0073 0200 0000  ..r....]...s....
-00000c60: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00000c70: 0000 0005 0000 0043 0000 0073 1000 0000  .......C...s....
-00000c80: 7c00 6a00 6401 6402 6403 6404 8d03 5300  |.j.d.d.d.d...S.
-00000c90: 2905 4eda 0b73 686f 7754 6f6f 6c74 6970  ).N..showTooltip
-00000ca0: 723d 0000 0054 7234 0000 0072 3700 0000  r=...Tr4...r7...
-00000cb0: 7222 0000 0072 1f00 0000 721f 0000 0072  r"...r....r....r
-00000cc0: 2000 0000 7210 0000 0062 0000 0073 0200   ...r....b...s..
-00000cd0: 0000 0002 7a1f 4c69 6e65 4368 6172 7444  ....z.LineChartD
-00000ce0: 6174 6150 6f69 6e74 2e73 686f 775f 746f  ataPoint.show_to
-00000cf0: 6f6c 7469 7063 0200 0000 0000 0000 0000  oltipc..........
-00000d00: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
-00000d10: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
-00000d20: 0053 0029 024e 723e 0000 0072 3a00 0000  .S.).Nr>...r:...
-00000d30: 723c 0000 0072 1f00 0000 721f 0000 0072  r<...r....r....r
-00000d40: 2000 0000 7210 0000 0066 0000 0073 0200   ...r....f...s..
-00000d50: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000d60: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-00000d70: 0000 7c00 a000 6401 a101 5300 a902 4e72  ..|...d...S...Nr
-00000d80: 1100 0000 7237 0000 0072 2200 0000 721f  ....r7...r"...r.
-00000d90: 0000 0072 1f00 0000 7220 0000 0072 1100  ...r....r ...r..
-00000da0: 0000 6b00 0000 7302 0000 0000 027a 1a4c  ..k...s......z.L
-00000db0: 696e 6543 6861 7274 4461 7461 506f 696e  ineChartDataPoin
-00000dc0: 742e 746f 6f6c 7469 7063 0200 0000 0000  t.tooltipc......
-00000dd0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000de0: 0000 7310 0000 007c 00a0 0064 017c 01a1  ..s....|...d.|..
-00000df0: 0201 0064 0053 0072 3f00 0000 723a 0000  ...d.S.r?...r:..
-00000e00: 0072 3c00 0000 721f 0000 0072 1f00 0000  .r<...r....r....
-00000e10: 7220 0000 0072 1100 0000 6f00 0000 7302  r ...r....o...s.
-00000e20: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
-00000e30: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00000e40: 0000 007c 006a 0053 0072 2f00 0000 2901  ...|.j.S.r/...).
-00000e50: da22 5f4c 696e 6543 6861 7274 4461 7461  ."_LineChartData
-00000e60: 506f 696e 745f 5f74 6f6f 6c74 6970 5f61  Point__tooltip_a
-00000e70: 6c69 676e 7222 0000 0072 1f00 0000 721f  lignr"...r....r.
-00000e80: 0000 0072 2000 0000 7213 0000 0074 0000  ...r ...r....t..
-00000e90: 0073 0200 0000 0002 7a20 4c69 6e65 4368  .s......z LineCh
-00000ea0: 6172 7444 6174 6150 6f69 6e74 2e74 6f6f  artDataPoint.too
-00000eb0: 6c74 6970 5f61 6c69 676e 6302 0000 0000  ltip_alignc.....
-00000ec0: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
-00000ed0: 0000 0073 2600 0000 7c01 7c00 5f00 7c00  ...s&...|.|._.|.
-00000ee0: a001 6401 7402 7c01 7403 8302 721c 7c01  ..d.t.|.t...r.|.
-00000ef0: 6a04 6e02 7c01 a102 0100 6400 5300 2902  j.n.|.....d.S.).
-00000f00: 4eda 0c74 6f6f 6c74 6970 416c 6967 6e29  N..tooltipAlign)
-00000f10: 0572 4000 0000 723b 0000 00da 0a69 7369  .r@...r;.....isi
-00000f20: 6e73 7461 6e63 6572 0b00 0000 7239 0000  nstancer....r9..
-00000f30: 0072 3c00 0000 721f 0000 0072 1f00 0000  .r<...r....r....
-00000f40: 7220 0000 0072 1300 0000 7800 0000 7308  r ...r....x...s.
-00000f50: 0000 0000 0206 0104 0114 ff63 0100 0000  ...........c....
-00000f60: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000f70: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
-00000f80: 2f00 0000 a901 7229 0000 0072 2200 0000  /.....r)...r"...
-00000f90: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-00000fa0: 1200 0000 8000 0000 7302 0000 0000 027a  ........s......z
-00000fb0: 204c 696e 6543 6861 7274 4461 7461 506f   LineChartDataPo
-00000fc0: 696e 742e 746f 6f6c 7469 705f 7374 796c  int.tooltip_styl
-00000fd0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00000fe0: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000ff0: 017c 005f 0064 0053 0072 2f00 0000 7243  .|._.d.S.r/...rC
-00001000: 0000 0072 3c00 0000 721f 0000 0072 1f00  ...r<...r....r..
-00001010: 0000 7220 0000 0072 1200 0000 8400 0000  ..r ...r........
-00001020: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00001030: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00001040: 7306 0000 007c 006a 0053 0072 2f00 0000  s....|.j.S.r/...
-00001050: a901 722a 0000 0072 2200 0000 721f 0000  ..r*...r"...r...
-00001060: 0072 1f00 0000 7220 0000 0072 1400 0000  .r....r ...r....
-00001070: 8900 0000 7302 0000 0000 027a 184c 696e  ....s......z.Lin
-00001080: 6543 6861 7274 4461 7461 506f 696e 742e  eChartDataPoint.
-00001090: 706f 696e 7463 0200 0000 0000 0000 0000  pointc..........
-000010a0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-000010b0: 0000 007c 017c 005f 0064 0053 0072 2f00  ...|.|._.d.S.r/.
-000010c0: 0000 7244 0000 0072 3c00 0000 721f 0000  ..rD...r<...r...
-000010d0: 0072 1f00 0000 7220 0000 0072 1400 0000  .r....r ...r....
-000010e0: 8d00 0000 7302 0000 0000 0263 0100 0000  ....s......c....
-000010f0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00001100: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
-00001110: 2f00 0000 a901 722b 0000 0072 2200 0000  /.....r+...r"...
-00001120: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-00001130: 1500 0000 9200 0000 7302 0000 0000 027a  ........s......z
-00001140: 214c 696e 6543 6861 7274 4461 7461 506f  !LineChartDataPo
-00001150: 696e 742e 7365 6c65 6374 6564 5f70 6f69  int.selected_poi
-00001160: 6e74 6302 0000 0000 0000 0000 0000 0002  ntc.............
-00001170: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00001180: 7c01 7c00 5f00 6400 5300 722f 0000 0072  |.|._.d.S.r/...r
-00001190: 4500 0000 723c 0000 0072 1f00 0000 721f  E...r<...r....r.
-000011a0: 0000 0072 2000 0000 7215 0000 0096 0000  ...r ...r.......
-000011b0: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-000011c0: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-000011d0: 0073 1000 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
-000011e0: 6404 8d03 5300 2905 4eda 0d73 686f 7741  d...S.).N..showA
-000011f0: 626f 7665 4c69 6e65 723d 0000 0054 7234  boveLiner=...Tr4
-00001200: 0000 0072 3700 0000 7222 0000 0072 1f00  ...r7...r"...r..
-00001210: 0000 721f 0000 0072 2000 0000 7216 0000  ..r....r ...r...
-00001220: 009b 0000 0073 0200 0000 0002 7a22 4c69  .....s......z"Li
-00001230: 6e65 4368 6172 7444 6174 6150 6f69 6e74  neChartDataPoint
-00001240: 2e73 686f 775f 6162 6f76 655f 6c69 6e65  .show_above_line
-00001250: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001260: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00001270: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
-00001280: 4e72 4600 0000 723a 0000 0072 3c00 0000  NrF...r:...r<...
-00001290: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-000012a0: 1600 0000 9f00 0000 7302 0000 0000 0263  ........s......c
-000012b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000012c0: 0500 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
-000012d0: 0064 0164 0264 0364 048d 0353 0029 054e  .d.d.d.d...S.).N
-000012e0: da0d 7368 6f77 4265 6c6f 774c 696e 6572  ..showBelowLiner
-000012f0: 3d00 0000 5472 3400 0000 7237 0000 0072  =...Tr4...r7...r
-00001300: 2200 0000 721f 0000 0072 1f00 0000 7220  "...r....r....r 
-00001310: 0000 0072 1700 0000 a400 0000 7302 0000  ...r........s...
-00001320: 0000 027a 224c 696e 6543 6861 7274 4461  ...z"LineChartDa
-00001330: 7461 506f 696e 742e 7368 6f77 5f62 656c  taPoint.show_bel
-00001340: 6f77 5f6c 696e 6563 0200 0000 0000 0000  ow_linec........
-00001350: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001360: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00001370: 0064 0053 0029 024e 7247 0000 0072 3a00  .d.S.).NrG...r:.
-00001380: 0000 723c 0000 0072 1f00 0000 721f 0000  ..r<...r....r...
-00001390: 0072 2000 0000 7217 0000 00a8 0000 0073  .r ...r........s
-000013a0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
-000013b0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-000013c0: 0600 0000 7c00 6a00 5300 722f 0000 00a9  ....|.j.S.r/....
-000013d0: 0172 2c00 0000 7222 0000 0072 1f00 0000  .r,...r"...r....
-000013e0: 721f 0000 0072 2000 0000 7218 0000 00ad  r....r ...r.....
-000013f0: 0000 0073 0200 0000 0002 7a26 4c69 6e65  ...s......z&Line
-00001400: 4368 6172 7444 6174 6150 6f69 6e74 2e73  ChartDataPoint.s
-00001410: 656c 6563 7465 645f 6265 6c6f 775f 6c69  elected_below_li
-00001420: 6e65 6302 0000 0000 0000 0000 0000 0002  nec.............
-00001430: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00001440: 7c01 7c00 5f00 6400 5300 722f 0000 0072  |.|._.d.S.r/...r
-00001450: 4800 0000 723c 0000 0072 1f00 0000 721f  H...r<...r....r.
-00001460: 0000 0072 2000 0000 7218 0000 00b1 0000  ...r ...r.......
-00001470: 0073 0200 0000 0002 2910 4e4e 4e4e 4e4e  .s......).NNNNNN
-00001480: 4e4e 4e4e 4e4e 4e4e 4e4e 2921 da08 5f5f  NNNNNNNNNN)!..__
-00001490: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000014a0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000014b0: 7208 0000 0072 0300 0000 723d 0000 00da  r....r....r=....
-000014c0: 0373 7472 720a 0000 0072 0b00 0000 7204  .strr....r....r.
-000014d0: 0000 0072 0600 0000 7205 0000 0072 0900  ...r....r....r..
-000014e0: 0000 7202 0000 0072 1d00 0000 7223 0000  ..r....r....r#..
-000014f0: 0072 2700 0000 7231 0000 00da 0870 726f  .r'...r1.....pro
-00001500: 7065 7274 7972 0d00 0000 da06 7365 7474  pertyr......sett
-00001510: 6572 720e 0000 0072 0f00 0000 7210 0000  err....r....r...
-00001520: 0072 1100 0000 7213 0000 0072 1200 0000  .r....r....r....
-00001530: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001540: 1700 0000 7218 0000 00da 0d5f 5f63 6c61  ....r......__cla
-00001550: 7373 6365 6c6c 5f5f 721f 0000 0072 1f00  sscell__r....r..
-00001560: 0000 722d 0000 0072 2000 0000 720c 0000  ..r-...r ...r...
-00001570: 000b 0000 0073 aa00 0000 0803 0001 0001  .....s..........
-00001580: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00001590: 0001 0004 0001 0001 0001 00ec 0202 0201  ................
-000015a0: 0201 0601 0601 0601 0601 0601 0c01 0c01  ................
-000015b0: 0601 0601 0c04 0601 0601 0601 02ec 0c2c  ...............,
-000015c0: 0803 0c07 0805 0201 1003 0401 1004 0201  ................
-000015d0: 1003 0401 1004 0201 1403 0401 1404 0201  ................
-000015e0: 1403 0401 1404 0201 1403 0401 1404 0201  ................
-000015f0: 1403 0401 1407 0201 0a03 0401 1404 0201  ................
-00001600: 0a03 0401 1a04 0201 0a03 0401 1a04 0201  ................
-00001610: 1403 0401 1404 0201 1403 0401 1404 0201  ................
-00001620: 1a03 0401 720c 0000 004e 2912 da06 7479  ....r....N)...ty
-00001630: 7069 6e67 7202 0000 0072 0300 0000 7204  pingr....r....r.
-00001640: 0000 00da 2166 6c65 745f 636f 7265 2e63  ....!flet_core.c
-00001650: 6861 7274 732e 6368 6172 745f 706f 696e  harts.chart_poin
-00001660: 745f 6c69 6e65 7205 0000 00da 2266 6c65  t_liner....."fle
-00001670: 745f 636f 7265 2e63 6861 7274 732e 6368  t_core.charts.ch
-00001680: 6172 745f 706f 696e 745f 7368 6170 6572  art_point_shaper
-00001690: 0600 0000 da11 666c 6574 5f63 6f72 652e  ......flet_core.
-000016a0: 636f 6e74 726f 6c72 0700 0000 7208 0000  controlr....r...
-000016b0: 00da 0d66 6c65 745f 636f 7265 2e72 6566  ...flet_core.ref
-000016c0: 7209 0000 00da 1466 6c65 745f 636f 7265  r......flet_core
-000016d0: 2e74 6578 745f 7374 796c 6572 0a00 0000  .text_styler....
-000016e0: da0f 666c 6574 5f63 6f72 652e 7479 7065  ..flet_core.type
-000016f0: 7372 0b00 0000 720c 0000 0072 1f00 0000  sr....r....r....
-00001700: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-00001710: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
-00001720: 0000 1402 0c01 0c01 1001 0c01 0c01 0c03  ................
+00000600: 6f2f 776f 726b 7370 6163 6573 2f63 6f6e  o/workspaces/con
+00000610: 7472 6962 666c 6574 2f66 6c65 7463 6f6e  tribflet/fletcon
+00000620: 7472 6962 2f73 646b 2f70 7974 686f 6e2f  trib/sdk/python/
+00000630: 7061 636b 6167 6573 2f66 6c65 742d 636f  packages/flet-co
+00000640: 7265 2f73 7263 2f66 6c65 745f 636f 7265  re/src/flet_core
+00000650: 2f63 6861 7274 732f 6c69 6e65 5f63 6861  /charts/line_cha
+00000660: 7274 5f64 6174 615f 706f 696e 742e 7079  rt_data_point.py
+00000670: 721d 0000 000c 0000 0073 2600 0000 0017  r........s&.....
+00000680: 0401 0201 0201 0201 0201 02fb 0608 0601  ................
+00000690: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000006a0: 0601 0601 7a1b 4c69 6e65 4368 6172 7444  ....z.LineChartD
+000006b0: 6174 6150 6f69 6e74 2e5f 5f69 6e69 745f  ataPoint.__init_
+000006c0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+000006d0: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
+000006e0: 0153 0029 024e da01 7072 1f00 0000 a901  .S.).N..pr......
+000006f0: 721e 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00000700: 2000 0000 da11 5f67 6574 5f63 6f6e 7472   ....._get_contr
+00000710: 6f6c 5f6e 616d 6538 0000 0073 0200 0000  ol_name8...s....
+00000720: 0001 7a24 4c69 6e65 4368 6172 7444 6174  ..z$LineChartDat
+00000730: 6150 6f69 6e74 2e5f 6765 745f 636f 6e74  aPoint._get_cont
+00000740: 726f 6c5f 6e61 6d65 6301 0000 0000 0000  rol_namec.......
+00000750: 0000 0000 0001 0000 0004 0000 0003 0000  ................
+00000760: 0073 4600 0000 7400 8300 a001 a100 0100  .sF...t.........
+00000770: 7c00 a002 6401 7c00 6a03 a102 0100 7c00  |...d.|.j.....|.
+00000780: a002 6402 7c00 6a04 a102 0100 7c00 a002  ..d.|.j.....|...
+00000790: 6403 7c00 6a05 a102 0100 7c00 a002 6404  d.|.j.....|...d.
+000007a0: 7c00 6a06 a102 0100 6400 5300 2905 4e5a  |.j.....d.S.).NZ
+000007b0: 0c74 6f6f 6c74 6970 5374 796c 6572 1400  .tooltipStyler..
+000007c0: 0000 da0d 7365 6c65 6374 6564 506f 696e  ....selectedPoin
+000007d0: 74da 1173 656c 6563 7465 6442 656c 6f77  t..selectedBelow
+000007e0: 4c69 6e65 2907 da05 7375 7065 72da 0d62  Line)...super..b
+000007f0: 6566 6f72 655f 7570 6461 7465 da0e 5f73  efore_update.._s
+00000800: 6574 5f61 7474 725f 6a73 6f6e da22 5f4c  et_attr_json."_L
+00000810: 696e 6543 6861 7274 4461 7461 506f 696e  ineChartDataPoin
+00000820: 745f 5f74 6f6f 6c74 6970 5f73 7479 6c65  t__tooltip_style
+00000830: da1a 5f4c 696e 6543 6861 7274 4461 7461  .._LineChartData
+00000840: 506f 696e 745f 5f70 6f69 6e74 da23 5f4c  Point__point.#_L
+00000850: 696e 6543 6861 7274 4461 7461 506f 696e  ineChartDataPoin
+00000860: 745f 5f73 656c 6563 7465 645f 706f 696e  t__selected_poin
+00000870: 74da 285f 4c69 6e65 4368 6172 7444 6174  t.(_LineChartDat
+00000880: 6150 6f69 6e74 5f5f 7365 6c65 6374 6564  aPoint__selected
+00000890: 5f62 656c 6f77 5f6c 696e 6572 2200 0000  _below_liner"...
+000008a0: a901 da09 5f5f 636c 6173 735f 5f72 1f00  ....__class__r..
+000008b0: 0000 7220 0000 0072 2700 0000 3b00 0000  ..r ...r'...;...
+000008c0: 730a 0000 0000 010a 010e 010e 010e 017a  s..............z
+000008d0: 204c 696e 6543 6861 7274 4461 7461 506f   LineChartDataPo
+000008e0: 696e 742e 6265 666f 7265 5f75 7064 6174  int.before_updat
+000008f0: 6563 0100 0000 0000 0000 0000 0000 0200  ec..............
+00000900: 0000 0100 0000 4300 0000 7308 0000 0067  ......C...s....g
+00000910: 007d 017c 0153 00a9 014e 721f 0000 0029  .}.|.S...Nr....)
+00000920: 0272 1e00 0000 da08 6368 696c 6472 656e  .r......children
+00000930: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00000940: 0d5f 6765 745f 6368 696c 6472 656e 4200  ._get_childrenB.
+00000950: 0000 7304 0000 0000 0104 017a 204c 696e  ..s........z Lin
+00000960: 6543 6861 7274 4461 7461 506f 696e 742e  eChartDataPoint.
+00000970: 5f67 6574 5f63 6869 6c64 7265 6e29 01da  _get_children)..
+00000980: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
+00000990: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+000009a0: 7310 0000 007c 006a 0064 0164 0264 0364  s....|.j.d.d.d.d
+000009b0: 048d 0353 0029 054e 720d 0000 00da 0566  ...S.).Nr......f
+000009c0: 6c6f 6174 7201 0000 00a9 02da 0964 6174  loatr........dat
+000009d0: 615f 7479 7065 da09 6465 665f 7661 6c75  a_type..def_valu
+000009e0: 65a9 01da 095f 6765 745f 6174 7472 7222  e...._get_attrr"
+000009f0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+00000a00: 0000 720d 0000 0047 0000 0073 0200 0000  ..r....G...s....
+00000a10: 0002 7a14 4c69 6e65 4368 6172 7444 6174  ..z.LineChartDat
+00000a20: 6150 6f69 6e74 2e78 2901 da05 7661 6c75  aPoint.x)...valu
+00000a30: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00000a40: 0000 0400 0000 4300 0000 7310 0000 007c  ......C...s....|
+00000a50: 00a0 0064 017c 01a1 0201 0064 0053 0029  ...d.|.....d.S.)
+00000a60: 024e 720d 0000 00a9 01da 095f 7365 745f  .Nr........_set_
+00000a70: 6174 7472 a902 721e 0000 0072 3900 0000  attr..r....r9...
+00000a80: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00000a90: 0d00 0000 4b00 0000 7302 0000 0000 0263  ....K...s......c
+00000aa0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000ab0: 0500 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
+00000ac0: 0064 0164 0264 0364 048d 0353 0029 054e  .d.d.d.d...S.).N
+00000ad0: 720e 0000 0072 3300 0000 7201 0000 0072  r....r3...r....r
+00000ae0: 3400 0000 7237 0000 0072 2200 0000 721f  4...r7...r"...r.
+00000af0: 0000 0072 1f00 0000 7220 0000 0072 0e00  ...r....r ...r..
+00000b00: 0000 5000 0000 7302 0000 0000 027a 144c  ..P...s......z.L
+00000b10: 696e 6543 6861 7274 4461 7461 506f 696e  ineChartDataPoin
+00000b20: 742e 7963 0200 0000 0000 0000 0000 0000  t.yc............
+00000b30: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+00000b40: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
+00000b50: 0029 024e 720e 0000 0072 3a00 0000 723c  .).Nr....r:...r<
+00000b60: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+00000b70: 0000 720e 0000 0054 0000 0073 0200 0000  ..r....T...s....
+00000b80: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000b90: 0000 0005 0000 0043 0000 0073 1000 0000  .......C...s....
+00000ba0: 7c00 6a00 6401 6402 6403 6404 8d03 5300  |.j.d.d.d.d...S.
+00000bb0: 2905 4e72 0f00 0000 da04 626f 6f6c 4672  ).Nr......boolFr
+00000bc0: 3400 0000 7237 0000 0072 2200 0000 721f  4...r7...r"...r.
+00000bd0: 0000 0072 1f00 0000 7220 0000 0072 0f00  ...r....r ...r..
+00000be0: 0000 5900 0000 7302 0000 0000 027a 1b4c  ..Y...s......z.L
+00000bf0: 696e 6543 6861 7274 4461 7461 506f 696e  ineChartDataPoin
+00000c00: 742e 7365 6c65 6374 6564 6302 0000 0000  t.selectedc.....
+00000c10: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000c20: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
+00000c30: a102 0100 6400 5300 2902 4e72 0f00 0000  ....d.S.).Nr....
+00000c40: 723a 0000 0072 3c00 0000 721f 0000 0072  r:...r<...r....r
+00000c50: 1f00 0000 7220 0000 0072 0f00 0000 5d00  ....r ...r....].
+00000c60: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
+00000c70: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00000c80: 0000 7310 0000 007c 006a 0064 0164 0264  ..s....|.j.d.d.d
+00000c90: 0364 048d 0353 0029 054e da0b 7368 6f77  .d...S.).N..show
+00000ca0: 546f 6f6c 7469 7072 3d00 0000 5472 3400  Tooltipr=...Tr4.
+00000cb0: 0000 7237 0000 0072 2200 0000 721f 0000  ..r7...r"...r...
+00000cc0: 0072 1f00 0000 7220 0000 0072 1000 0000  .r....r ...r....
+00000cd0: 6200 0000 7302 0000 0000 027a 1f4c 696e  b...s......z.Lin
+00000ce0: 6543 6861 7274 4461 7461 506f 696e 742e  eChartDataPoint.
+00000cf0: 7368 6f77 5f74 6f6f 6c74 6970 6302 0000  show_tooltipc...
+00000d00: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000d10: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
+00000d20: 7c01 a102 0100 6400 5300 2902 4e72 3e00  |.....d.S.).Nr>.
+00000d30: 0000 723a 0000 0072 3c00 0000 721f 0000  ..r:...r<...r...
+00000d40: 0072 1f00 0000 7220 0000 0072 1000 0000  .r....r ...r....
+00000d50: 6600 0000 7302 0000 0000 0263 0100 0000  f...s......c....
+00000d60: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000d70: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
+00000d80: 0153 00a9 024e 7211 0000 0072 3700 0000  .S...Nr....r7...
+00000d90: 7222 0000 0072 1f00 0000 721f 0000 0072  r"...r....r....r
+00000da0: 2000 0000 7211 0000 006b 0000 0073 0200   ...r....k...s..
+00000db0: 0000 0002 7a1a 4c69 6e65 4368 6172 7444  ....z.LineChartD
+00000dc0: 6174 6150 6f69 6e74 2e74 6f6f 6c74 6970  ataPoint.tooltip
+00000dd0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000de0: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
+00000df0: a000 6401 7c01 a102 0100 6400 5300 723f  ..d.|.....d.S.r?
+00000e00: 0000 0072 3a00 0000 723c 0000 0072 1f00  ...r:...r<...r..
+00000e10: 0000 721f 0000 0072 2000 0000 7211 0000  ..r....r ...r...
+00000e20: 006f 0000 0073 0200 0000 0002 6301 0000  .o...s......c...
+00000e30: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000e40: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00000e50: 722f 0000 0029 01da 225f 4c69 6e65 4368  r/...).."_LineCh
+00000e60: 6172 7444 6174 6150 6f69 6e74 5f5f 746f  artDataPoint__to
+00000e70: 6f6c 7469 705f 616c 6967 6e72 2200 0000  oltip_alignr"...
+00000e80: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00000e90: 1300 0000 7400 0000 7302 0000 0000 027a  ....t...s......z
+00000ea0: 204c 696e 6543 6861 7274 4461 7461 506f   LineChartDataPo
+00000eb0: 696e 742e 746f 6f6c 7469 705f 616c 6967  int.tooltip_alig
+00000ec0: 6e63 0200 0000 0000 0000 0000 0000 0200  nc..............
+00000ed0: 0000 0600 0000 4300 0000 7326 0000 007c  ......C...s&...|
+00000ee0: 017c 005f 007c 00a0 0164 0174 027c 0174  .|._.|...d.t.|.t
+00000ef0: 0383 0272 1c7c 016a 046e 027c 01a1 0201  ...r.|.j.n.|....
+00000f00: 0064 0053 0029 024e da0c 746f 6f6c 7469  .d.S.).N..toolti
+00000f10: 7041 6c69 676e 2905 7240 0000 0072 3b00  pAlign).r@...r;.
+00000f20: 0000 da0a 6973 696e 7374 616e 6365 720b  ....isinstancer.
+00000f30: 0000 0072 3900 0000 723c 0000 0072 1f00  ...r9...r<...r..
+00000f40: 0000 721f 0000 0072 2000 0000 7213 0000  ..r....r ...r...
+00000f50: 0078 0000 0073 0800 0000 0002 0601 0401  .x...s..........
+00000f60: 14ff 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000f70: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
+00000f80: 7c00 6a00 5300 722f 0000 00a9 0172 2900  |.j.S.r/.....r).
+00000f90: 0000 7222 0000 0072 1f00 0000 721f 0000  ..r"...r....r...
+00000fa0: 0072 2000 0000 7212 0000 0080 0000 0073  .r ...r........s
+00000fb0: 0200 0000 0002 7a20 4c69 6e65 4368 6172  ......z LineChar
+00000fc0: 7444 6174 6150 6f69 6e74 2e74 6f6f 6c74  tDataPoint.toolt
+00000fd0: 6970 5f73 7479 6c65 6302 0000 0000 0000  ip_stylec.......
+00000fe0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00000ff0: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00001000: 722f 0000 0072 4300 0000 723c 0000 0072  r/...rC...r<...r
+00001010: 1f00 0000 721f 0000 0072 2000 0000 7212  ....r....r ...r.
+00001020: 0000 0084 0000 0073 0200 0000 0002 6301  .......s......c.
+00001030: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00001040: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+00001050: 5300 722f 0000 00a9 0172 2a00 0000 7222  S.r/.....r*...r"
+00001060: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+00001070: 0000 7214 0000 0089 0000 0073 0200 0000  ..r........s....
+00001080: 0002 7a18 4c69 6e65 4368 6172 7444 6174  ..z.LineChartDat
+00001090: 6150 6f69 6e74 2e70 6f69 6e74 6302 0000  aPoint.pointc...
+000010a0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+000010b0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+000010c0: 6400 5300 722f 0000 0072 4400 0000 723c  d.S.r/...rD...r<
+000010d0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+000010e0: 0000 7214 0000 008d 0000 0073 0200 0000  ..r........s....
+000010f0: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00001100: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
+00001110: 7c00 6a00 5300 722f 0000 00a9 0172 2b00  |.j.S.r/.....r+.
+00001120: 0000 7222 0000 0072 1f00 0000 721f 0000  ..r"...r....r...
+00001130: 0072 2000 0000 7215 0000 0092 0000 0073  .r ...r........s
+00001140: 0200 0000 0002 7a21 4c69 6e65 4368 6172  ......z!LineChar
+00001150: 7444 6174 6150 6f69 6e74 2e73 656c 6563  tDataPoint.selec
+00001160: 7465 645f 706f 696e 7463 0200 0000 0000  ted_pointc......
+00001170: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00001180: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+00001190: 0072 2f00 0000 7245 0000 0072 3c00 0000  .r/...rE...r<...
+000011a0: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+000011b0: 1500 0000 9600 0000 7302 0000 0000 0263  ........s......c
+000011c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000011d0: 0500 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
+000011e0: 0064 0164 0264 0364 048d 0353 0029 054e  .d.d.d.d...S.).N
+000011f0: da0d 7368 6f77 4162 6f76 654c 696e 6572  ..showAboveLiner
+00001200: 3d00 0000 5472 3400 0000 7237 0000 0072  =...Tr4...r7...r
+00001210: 2200 0000 721f 0000 0072 1f00 0000 7220  "...r....r....r 
+00001220: 0000 0072 1600 0000 9b00 0000 7302 0000  ...r........s...
+00001230: 0000 027a 224c 696e 6543 6861 7274 4461  ...z"LineChartDa
+00001240: 7461 506f 696e 742e 7368 6f77 5f61 626f  taPoint.show_abo
+00001250: 7665 5f6c 696e 6563 0200 0000 0000 0000  ve_linec........
+00001260: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00001270: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
+00001280: 0064 0053 0029 024e 7246 0000 0072 3a00  .d.S.).NrF...r:.
+00001290: 0000 723c 0000 0072 1f00 0000 721f 0000  ..r<...r....r...
+000012a0: 0072 2000 0000 7216 0000 009f 0000 0073  .r ...r........s
+000012b0: 0200 0000 0002 6301 0000 0000 0000 0000  ......c.........
+000012c0: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
+000012d0: 1000 0000 7c00 6a00 6401 6402 6403 6404  ....|.j.d.d.d.d.
+000012e0: 8d03 5300 2905 4eda 0d73 686f 7742 656c  ..S.).N..showBel
+000012f0: 6f77 4c69 6e65 723d 0000 0054 7234 0000  owLiner=...Tr4..
+00001300: 0072 3700 0000 7222 0000 0072 1f00 0000  .r7...r"...r....
+00001310: 721f 0000 0072 2000 0000 7217 0000 00a4  r....r ...r.....
+00001320: 0000 0073 0200 0000 0002 7a22 4c69 6e65  ...s......z"Line
+00001330: 4368 6172 7444 6174 6150 6f69 6e74 2e73  ChartDataPoint.s
+00001340: 686f 775f 6265 6c6f 775f 6c69 6e65 6302  how_below_linec.
+00001350: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001360: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00001370: 6401 7c01 a102 0100 6400 5300 2902 4e72  d.|.....d.S.).Nr
+00001380: 4700 0000 723a 0000 0072 3c00 0000 721f  G...r:...r<...r.
+00001390: 0000 0072 1f00 0000 7220 0000 0072 1700  ...r....r ...r..
+000013a0: 0000 a800 0000 7302 0000 0000 0263 0100  ......s......c..
+000013b0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000013c0: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+000013d0: 0072 2f00 0000 a901 722c 0000 0072 2200  .r/.....r,...r".
+000013e0: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+000013f0: 0072 1800 0000 ad00 0000 7302 0000 0000  .r........s.....
+00001400: 027a 264c 696e 6543 6861 7274 4461 7461  .z&LineChartData
+00001410: 506f 696e 742e 7365 6c65 6374 6564 5f62  Point.selected_b
+00001420: 656c 6f77 5f6c 696e 6563 0200 0000 0000  elow_linec......
+00001430: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00001440: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+00001450: 0072 2f00 0000 7248 0000 0072 3c00 0000  .r/...rH...r<...
+00001460: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00001470: 1800 0000 b100 0000 7302 0000 0000 0229  ........s......)
+00001480: 104e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  .NNNNNNNNNNNNNNN
+00001490: 4e29 21da 085f 5f6e 616d 655f 5fda 0a5f  N)!..__name__.._
+000014a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000014b0: 6c6e 616d 655f 5f72 0800 0000 7203 0000  lname__r....r...
+000014c0: 0072 3d00 0000 da03 7374 7272 0a00 0000  .r=.....strr....
+000014d0: 720b 0000 0072 0400 0000 7206 0000 0072  r....r....r....r
+000014e0: 0500 0000 7209 0000 0072 0200 0000 721d  ....r....r....r.
+000014f0: 0000 0072 2300 0000 7227 0000 0072 3100  ...r#...r'...r1.
+00001500: 0000 da08 7072 6f70 6572 7479 720d 0000  ....propertyr...
+00001510: 00da 0673 6574 7465 7272 0e00 0000 720f  ...setterr....r.
+00001520: 0000 0072 1000 0000 7211 0000 0072 1300  ...r....r....r..
+00001530: 0000 7212 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00001540: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
+00001550: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00001560: 1f00 0000 721f 0000 0072 2d00 0000 7220  ....r....r-...r 
+00001570: 0000 0072 0c00 0000 0b00 0000 73aa 0000  ...r........s...
+00001580: 0008 0300 0100 0100 0100 0100 0100 0100  ................
+00001590: 0100 0100 0100 0100 0100 0400 0100 0100  ................
+000015a0: 0100 ec02 0202 0102 0106 0106 0106 0106  ................
+000015b0: 0106 010c 010c 0106 0106 010c 0406 0106  ................
+000015c0: 0106 0102 ec0c 2c08 030c 0708 0502 0110  ......,.........
+000015d0: 0304 0110 0402 0110 0304 0110 0402 0114  ................
+000015e0: 0304 0114 0402 0114 0304 0114 0402 0114  ................
+000015f0: 0304 0114 0402 0114 0304 0114 0702 010a  ................
+00001600: 0304 0114 0402 010a 0304 011a 0402 010a  ................
+00001610: 0304 011a 0402 0114 0304 0114 0402 0114  ................
+00001620: 0304 0114 0402 011a 0304 0172 0c00 0000  ...........r....
+00001630: 4e29 12da 0674 7970 696e 6772 0200 0000  N)...typingr....
+00001640: 7203 0000 0072 0400 0000 da21 666c 6574  r....r.....!flet
+00001650: 5f63 6f72 652e 6368 6172 7473 2e63 6861  _core.charts.cha
+00001660: 7274 5f70 6f69 6e74 5f6c 696e 6572 0500  rt_point_liner..
+00001670: 0000 da22 666c 6574 5f63 6f72 652e 6368  ..."flet_core.ch
+00001680: 6172 7473 2e63 6861 7274 5f70 6f69 6e74  arts.chart_point
+00001690: 5f73 6861 7065 7206 0000 00da 1166 6c65  _shaper......fle
+000016a0: 745f 636f 7265 2e63 6f6e 7472 6f6c 7207  t_core.controlr.
+000016b0: 0000 0072 0800 0000 da0d 666c 6574 5f63  ...r......flet_c
+000016c0: 6f72 652e 7265 6672 0900 0000 da14 666c  ore.refr......fl
+000016d0: 6574 5f63 6f72 652e 7465 7874 5f73 7479  et_core.text_sty
+000016e0: 6c65 720a 0000 00da 0f66 6c65 745f 636f  ler......flet_co
+000016f0: 7265 2e74 7970 6573 720b 0000 0072 0c00  re.typesr....r..
+00001700: 0000 721f 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00001710: 0072 2000 0000 da08 3c6d 6f64 756c 653e  .r .....<module>
+00001720: 0100 0000 730e 0000 0014 020c 010c 0110  ....s...........
+00001730: 010c 010c 010c 03                        .......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 5965 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 4d17 0000  a........:)fM...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 4d17 0000  a........./fM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
@@ -98,251 +98,252 @@
 00000610: 7230 0000 0063 0100 0000 0000 0000 0000  r0...c..........
 00000620: 0000 0200 0000 0400 0000 5300 0000 731a  ..........S...s.
 00000630: 0000 0074 00a0 017c 006a 02a1 017d 0174  ...t...|.j...}.t
 00000640: 0366 0069 007c 01a4 018e 0153 00a9 014e  .f.i.|.....S...N
 00000650: 2904 da04 6a73 6f6e da05 6c6f 6164 7372  )...json..loadsr
 00000660: 3000 0000 da0d 5069 6543 6861 7274 4576  0.....PieChartEv
 00000670: 656e 7429 02da 0165 da01 64a9 0072 3800  ent)...e..d..r8.
-00000680: 0000 fa5c 2f77 6f72 6b73 7061 6365 732f  ...\/workspaces/
+00000680: 0000 fa63 2f77 6f72 6b73 7061 6365 732f  ...c/workspaces/
 00000690: 636f 6e74 7269 6266 6c65 742f 666c 6574  contribflet/flet
-000006a0: 2f73 646b 2f70 7974 686f 6e2f 7061 636b  /sdk/python/pack
-000006b0: 6167 6573 2f66 6c65 742d 636f 7265 2f73  ages/flet-core/s
-000006c0: 7263 2f66 6c65 745f 636f 7265 2f63 6861  rc/flet_core/cha
-000006d0: 7274 732f 7069 655f 6368 6172 742e 7079  rts/pie_chart.py
-000006e0: da1c 636f 6e76 6572 745f 6c69 6e65 6368  ..convert_linech
-000006f0: 6172 745f 6576 656e 745f 6461 7461 5900  art_event_dataY.
-00000700: 0000 7304 0000 0000 010c 017a 3750 6965  ..s........z7Pie
-00000710: 4368 6172 742e 5f5f 696e 6974 5f5f 2e3c  Chart.__init__.<
-00000720: 6c6f 6361 6c73 3e2e 636f 6e76 6572 745f  locals>.convert_
-00000730: 6c69 6e65 6368 6172 745f 6576 656e 745f  linechart_event_
-00000740: 6461 7461 da0b 6368 6172 745f 6576 656e  data..chart_even
-00000750: 7429 0d72 0700 0000 da08 5f5f 696e 6974  t).r......__init
-00000760: 5f5f 720a 0000 00da 195f 5069 6543 6861  __r......_PieCha
-00000770: 7274 5f5f 6f6e 5f63 6861 7274 5f65 7665  rt__on_chart_eve
-00000780: 6e74 da12 5f61 6464 5f65 7665 6e74 5f68  nt.._add_event_h
-00000790: 616e 646c 6572 da0b 6765 745f 6861 6e64  andler..get_hand
-000007a0: 6c65 7272 1200 0000 7213 0000 0072 1400  lerr....r....r..
-000007b0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000007c0: 00da 0e6f 6e5f 6368 6172 745f 6576 656e  ...on_chart_even
-000007d0: 7429 23da 0473 656c 6672 1200 0000 7213  t)#..selfr....r.
-000007e0: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
-000007f0: 0000 7217 0000 0072 4000 0000 7218 0000  ..r....r@...r...
-00000800: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000810: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000820: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
-00000830: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
-00000840: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-00000850: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
-00000860: 722c 0000 0072 3100 0000 722d 0000 0072  r,...r1...r-...r
-00000870: 2e00 0000 722f 0000 0072 3000 0000 723a  ....r/...r0...r:
-00000880: 0000 0072 3800 0000 7238 0000 0072 3900  ...r8...r8...r9.
-00000890: 0000 723c 0000 0014 0000 0073 4e00 0000  ..r<.......sN...
-000008a0: 0027 0401 0201 0201 0201 0201 0201 0201  .'..............
-000008b0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000008c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000008d0: 0201 0201 0201 0201 02e5 061e 0804 0a01  ................
-000008e0: 1202 0601 0601 0601 0601 0601 0601 7a11  ..............z.
-000008f0: 5069 6543 6861 7274 2e5f 5f69 6e69 745f  PieChart.__init_
-00000900: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00000910: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
-00000920: 0153 0029 024e 5a08 7069 6563 6861 7274  .S.).NZ.piechart
-00000930: 7238 0000 00a9 0172 4100 0000 7238 0000  r8.....rA...r8..
-00000940: 0072 3800 0000 7239 0000 00da 115f 6765  .r8...r9....._ge
-00000950: 745f 636f 6e74 726f 6c5f 6e61 6d65 6800  t_control_nameh.
-00000960: 0000 7302 0000 0000 017a 1a50 6965 4368  ..s......z.PieCh
-00000970: 6172 742e 5f67 6574 5f63 6f6e 7472 6f6c  art._get_control
-00000980: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
-00000990: 0000 0100 0000 0400 0000 0300 0000 731c  ..............s.
-000009a0: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
-000009b0: 0264 017c 006a 03a1 0201 0064 0053 0029  .d.|.j.....d.S.)
-000009c0: 024e 7217 0000 0029 04da 0573 7570 6572  .Nr....)...super
-000009d0: da0d 6265 666f 7265 5f75 7064 6174 65da  ..before_update.
-000009e0: 0e5f 7365 745f 6174 7472 5f6a 736f 6eda  ._set_attr_json.
-000009f0: 125f 5069 6543 6861 7274 5f5f 616e 696d  ._PieChart__anim
-00000a00: 6174 6572 4200 0000 a901 da09 5f5f 636c  aterB.......__cl
-00000a10: 6173 735f 5f72 3800 0000 7239 0000 0072  ass__r8...r9...r
-00000a20: 4500 0000 6b00 0000 7304 0000 0000 010a  E...k...s.......
-00000a30: 017a 1650 6965 4368 6172 742e 6265 666f  .z.PieChart.befo
-00000a40: 7265 5f75 7064 6174 6563 0100 0000 0000  re_updatec......
-00000a50: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00000a60: 0000 731e 0000 0067 007d 017c 006a 0044  ..s....g.}.|.j.D
-00000a70: 005d 0e7d 027c 01a0 017c 02a1 0101 0071  .].}.|...|.....q
-00000a80: 0a7c 0153 0072 3200 0000 2902 da13 5f50  .|.S.r2...)..._P
-00000a90: 6965 4368 6172 745f 5f73 6563 7469 6f6e  ieChart__section
-00000aa0: 73da 0661 7070 656e 6429 0372 4100 0000  s..append).rA...
-00000ab0: da08 6368 696c 6472 656e da02 6473 7238  ..children..dsr8
-00000ac0: 0000 0072 3800 0000 7239 0000 00da 0d5f  ...r8...r9....._
-00000ad0: 6765 745f 6368 696c 6472 656e 6f00 0000  get_childreno...
-00000ae0: 7308 0000 0000 0104 010a 010c 017a 1650  s............z.P
-00000af0: 6965 4368 6172 742e 5f67 6574 5f63 6869  ieChart._get_chi
-00000b00: 6c64 7265 6e63 0100 0000 0000 0000 0000  ldrenc..........
-00000b10: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
-00000b20: 0000 007c 006a 0053 0072 3200 0000 a901  ...|.j.S.r2.....
-00000b30: 724a 0000 0072 4200 0000 7238 0000 0072  rJ...rB...r8...r
-00000b40: 3800 0000 7239 0000 0072 1200 0000 7600  8...r9...r....v.
-00000b50: 0000 7302 0000 0000 027a 1150 6965 4368  ..s......z.PieCh
-00000b60: 6172 742e 7365 6374 696f 6e73 6302 0000  art.sectionsc...
-00000b70: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000b80: 0043 0000 0073 1600 0000 7c01 6400 7501  .C...s....|.d.u.
-00000b90: 720c 7c01 6e02 6700 7c00 5f00 6400 5300  r.|.n.g.|._.d.S.
-00000ba0: 7232 0000 0072 4f00 0000 a902 7241 0000  r2...rO.....rA..
-00000bb0: 00da 0576 616c 7565 7238 0000 0072 3800  ...valuer8...r8.
-00000bc0: 0000 7239 0000 0072 1200 0000 7a00 0000  ..r9...r....z...
-00000bd0: 7302 0000 0000 02a9 01da 0672 6574 7572  s..........retur
-00000be0: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00000bf0: 0000 0300 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000c00: 00a0 0064 01a1 0153 00a9 024e 5a10 6365  ...d...S...NZ.ce
-00000c10: 6e74 6572 5370 6163 6543 6f6c 6f72 a901  nterSpaceColor..
-00000c20: da09 5f67 6574 5f61 7474 7272 4200 0000  .._get_attrrB...
-00000c30: 7238 0000 0072 3800 0000 7239 0000 0072  r8...r8...r9...r
-00000c40: 1300 0000 7f00 0000 7302 0000 0000 027a  ........s......z
-00000c50: 1b50 6965 4368 6172 742e 6365 6e74 6572  .PieChart.center
-00000c60: 5f73 7061 6365 5f63 6f6c 6f72 2901 7251  _space_color).rQ
-00000c70: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000c80: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-00000c90: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
-00000ca0: 0072 5400 0000 a901 da09 5f73 6574 5f61  .rT......._set_a
-00000cb0: 7474 7272 5000 0000 7238 0000 0072 3800  ttrrP...r8...r8.
-00000cc0: 0000 7239 0000 0072 1300 0000 8300 0000  ..r9...r........
-00000cd0: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00000ce0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000cf0: 730e 0000 007c 006a 0064 0164 0264 038d  s....|.j.d.d.d..
-00000d00: 0253 0029 044e da11 6365 6e74 6572 5370  .S.).N..centerSp
-00000d10: 6163 6552 6164 6975 73da 0566 6c6f 6174  aceRadius..float
-00000d20: a901 da09 6461 7461 5f74 7970 6572 5500  ....data_typerU.
-00000d30: 0000 7242 0000 0072 3800 0000 7238 0000  ..rB...r8...r8..
-00000d40: 0072 3900 0000 7214 0000 0088 0000 0073  .r9...r........s
-00000d50: 0200 0000 0002 7a1c 5069 6543 6861 7274  ......z.PieChart
-00000d60: 2e63 656e 7465 725f 7370 6163 655f 7261  .center_space_ra
-00000d70: 6469 7573 6302 0000 0000 0000 0000 0000  diusc...........
-00000d80: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00000d90: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
-00000da0: 5300 2902 4e72 5900 0000 7257 0000 0072  S.).NrY...rW...r
-00000db0: 5000 0000 7238 0000 0072 3800 0000 7239  P...r8...r8...r9
-00000dc0: 0000 0072 1400 0000 8c00 0000 7302 0000  ...r........s...
-00000dd0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-00000de0: 0100 0000 0400 0000 4300 0000 730e 0000  ........C...s...
-00000df0: 007c 006a 0064 0164 0264 038d 0253 0029  .|.j.d.d.d...S.)
-00000e00: 044e da0d 7365 6374 696f 6e73 5370 6163  .N..sectionsSpac
-00000e10: 6572 5a00 0000 725b 0000 0072 5500 0000  erZ...r[...rU...
-00000e20: 7242 0000 0072 3800 0000 7238 0000 0072  rB...r8...r8...r
-00000e30: 3900 0000 7215 0000 0091 0000 0073 0200  9...r........s..
-00000e40: 0000 0002 7a17 5069 6543 6861 7274 2e73  ....z.PieChart.s
-00000e50: 6563 7469 6f6e 735f 7370 6163 6563 0200  ections_spacec..
-00000e60: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000e70: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
-00000e80: 017c 01a1 0201 0064 0053 0029 024e 725d  .|.....d.S.).Nr]
-00000e90: 0000 0072 5700 0000 7250 0000 0072 3800  ...rW...rP...r8.
-00000ea0: 0000 7238 0000 0072 3900 0000 7215 0000  ..r8...r9...r...
-00000eb0: 0095 0000 0073 0200 0000 0002 6301 0000  .....s......c...
-00000ec0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000ed0: 0043 0000 0073 0e00 0000 7c00 6a00 6401  .C...s....|.j.d.
-00000ee0: 6402 6403 8d02 5300 2904 4eda 1173 7461  d.d...S.).N..sta
-00000ef0: 7274 4465 6772 6565 4f66 6673 6574 725a  rtDegreeOffsetrZ
-00000f00: 0000 0072 5b00 0000 7255 0000 0072 4200  ...r[...rU...rB.
-00000f10: 0000 7238 0000 0072 3800 0000 7239 0000  ..r8...r8...r9..
-00000f20: 0072 1600 0000 9a00 0000 7302 0000 0000  .r........s.....
-00000f30: 027a 1c50 6965 4368 6172 742e 7374 6172  .z.PieChart.star
-00000f40: 745f 6465 6772 6565 5f6f 6666 7365 7463  t_degree_offsetc
-00000f50: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000f60: 0400 0000 4300 0000 7310 0000 007c 00a0  ....C...s....|..
-00000f70: 0064 017c 01a1 0201 0064 0053 0029 024e  .d.|.....d.S.).N
-00000f80: 725e 0000 0072 5700 0000 7250 0000 0072  r^...rW...rP...r
-00000f90: 3800 0000 7238 0000 0072 3900 0000 7216  8...r8...r9...r.
-00000fa0: 0000 009e 0000 0073 0200 0000 0002 6301  .......s......c.
-00000fb0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00000fc0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00000fd0: 5300 7232 0000 00a9 0172 4700 0000 7242  S.r2.....rG...rB
-00000fe0: 0000 0072 3800 0000 7238 0000 0072 3900  ...r8...r8...r9.
-00000ff0: 0000 7217 0000 00a3 0000 0073 0200 0000  ..r........s....
-00001000: 0002 7a10 5069 6543 6861 7274 2e61 6e69  ..z.PieChart.ani
-00001010: 6d61 7465 6302 0000 0000 0000 0000 0000  matec...........
-00001020: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00001030: 0000 7c01 7c00 5f00 6400 5300 7232 0000  ..|.|._.d.S.r2..
-00001040: 0072 5f00 0000 7250 0000 0072 3800 0000  .r_...rP...r8...
-00001050: 7238 0000 0072 3900 0000 7217 0000 00a7  r8...r9...r.....
-00001060: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
-00001070: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001080: 0000 0073 0600 0000 7c00 6a00 5300 7232  ...s....|.j.S.r2
-00001090: 0000 0029 0172 3d00 0000 7242 0000 0072  ...).r=...rB...r
-000010a0: 3800 0000 7238 0000 0072 3900 0000 7240  8...r8...r9...r@
-000010b0: 0000 00ac 0000 0073 0200 0000 0002 7a17  .......s......z.
-000010c0: 5069 6543 6861 7274 2e6f 6e5f 6368 6172  PieChart.on_char
-000010d0: 745f 6576 656e 7463 0200 0000 0000 0000  t_eventc........
-000010e0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-000010f0: 7332 0000 007c 006a 00a0 017c 01a1 0101  s2...|.j...|....
-00001100: 007c 0164 0075 0172 227c 00a0 0264 0164  .|.d.u.r"|...d.d
-00001110: 02a1 0201 006e 0c7c 00a0 0264 0164 00a1  .....n.|...d.d..
-00001120: 0201 0064 0053 0029 034e da0c 6f6e 4368  ...d.S.).N..onCh
-00001130: 6172 7445 7665 6e74 5429 0372 3d00 0000  artEventT).r=...
-00001140: da09 7375 6273 6372 6962 6572 5800 0000  ..subscriberX...
-00001150: 2902 7241 0000 00da 0768 616e 646c 6572  ).rA.....handler
-00001160: 7238 0000 0072 3800 0000 7239 0000 0072  r8...r8...r9...r
-00001170: 4000 0000 b000 0000 7308 0000 0000 020c  @.......s.......
-00001180: 0108 010e 0229 214e 4e4e 4e4e 4e4e 4e4e  .....)!NNNNNNNNN
+000006a0: 636f 6e74 7269 622f 7364 6b2f 7079 7468  contrib/sdk/pyth
+000006b0: 6f6e 2f70 6163 6b61 6765 732f 666c 6574  on/packages/flet
+000006c0: 2d63 6f72 652f 7372 632f 666c 6574 5f63  -core/src/flet_c
+000006d0: 6f72 652f 6368 6172 7473 2f70 6965 5f63  ore/charts/pie_c
+000006e0: 6861 7274 2e70 79da 1c63 6f6e 7665 7274  hart.py..convert
+000006f0: 5f6c 696e 6563 6861 7274 5f65 7665 6e74  _linechart_event
+00000700: 5f64 6174 6159 0000 0073 0400 0000 0001  _dataY...s......
+00000710: 0c01 7a37 5069 6543 6861 7274 2e5f 5f69  ..z7PieChart.__i
+00000720: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e63  nit__.<locals>.c
+00000730: 6f6e 7665 7274 5f6c 696e 6563 6861 7274  onvert_linechart
+00000740: 5f65 7665 6e74 5f64 6174 61da 0b63 6861  _event_data..cha
+00000750: 7274 5f65 7665 6e74 290d 7207 0000 00da  rt_event).r.....
+00000760: 085f 5f69 6e69 745f 5f72 0a00 0000 da19  .__init__r......
+00000770: 5f50 6965 4368 6172 745f 5f6f 6e5f 6368  _PieChart__on_ch
+00000780: 6172 745f 6576 656e 74da 125f 6164 645f  art_event.._add_
+00000790: 6576 656e 745f 6861 6e64 6c65 72da 0b67  event_handler..g
+000007a0: 6574 5f68 616e 646c 6572 7212 0000 0072  et_handlerr....r
+000007b0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
+000007c0: 0000 0072 1700 0000 da0e 6f6e 5f63 6861  ...r......on_cha
+000007d0: 7274 5f65 7665 6e74 2923 da04 7365 6c66  rt_event)#..self
+000007e0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000007f0: 1500 0000 7216 0000 0072 1700 0000 7240  ....r....r....r@
+00000800: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
+00000810: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000820: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00000830: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
+00000840: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
+00000850: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+00000860: 0000 722b 0000 0072 2c00 0000 7231 0000  ..r+...r,...r1..
+00000870: 0072 2d00 0000 722e 0000 0072 2f00 0000  .r-...r....r/...
+00000880: 7230 0000 0072 3a00 0000 7238 0000 0072  r0...r:...r8...r
+00000890: 3800 0000 7239 0000 0072 3c00 0000 1400  8...r9...r<.....
+000008a0: 0000 734e 0000 0000 2704 0102 0102 0102  ..sN....'.......
+000008b0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000008c0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000008d0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000008e0: e506 1e08 040a 0112 0206 0106 0106 0106  ................
+000008f0: 0106 0106 017a 1150 6965 4368 6172 742e  .....z.PieChart.
+00000900: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000910: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000920: 0073 0400 0000 6401 5300 2902 4e5a 0870  .s....d.S.).NZ.p
+00000930: 6965 6368 6172 7472 3800 0000 a901 7241  iechartr8.....rA
+00000940: 0000 0072 3800 0000 7238 0000 0072 3900  ...r8...r8...r9.
+00000950: 0000 da11 5f67 6574 5f63 6f6e 7472 6f6c  ...._get_control
+00000960: 5f6e 616d 6568 0000 0073 0200 0000 0001  _nameh...s......
+00000970: 7a1a 5069 6543 6861 7274 2e5f 6765 745f  z.PieChart._get_
+00000980: 636f 6e74 726f 6c5f 6e61 6d65 6301 0000  control_namec...
+00000990: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+000009a0: 0003 0000 0073 1c00 0000 7400 8300 a001  .....s....t.....
+000009b0: a100 0100 7c00 a002 6401 7c00 6a03 a102  ....|...d.|.j...
+000009c0: 0100 6400 5300 2902 4e72 1700 0000 2904  ..d.S.).Nr....).
+000009d0: da05 7375 7065 72da 0d62 6566 6f72 655f  ..super..before_
+000009e0: 7570 6461 7465 da0e 5f73 6574 5f61 7474  update.._set_att
+000009f0: 725f 6a73 6f6e da12 5f50 6965 4368 6172  r_json.._PieChar
+00000a00: 745f 5f61 6e69 6d61 7465 7242 0000 00a9  t__animaterB....
+00000a10: 01da 095f 5f63 6c61 7373 5f5f 7238 0000  ...__class__r8..
+00000a20: 0072 3900 0000 7245 0000 006b 0000 0073  .r9...rE...k...s
+00000a30: 0400 0000 0001 0a01 7a16 5069 6543 6861  ........z.PieCha
+00000a40: 7274 2e62 6566 6f72 655f 7570 6461 7465  rt.before_update
+00000a50: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000a60: 0004 0000 0043 0000 0073 1e00 0000 6700  .....C...s....g.
+00000a70: 7d01 7c00 6a00 4400 5d0e 7d02 7c01 a001  }.|.j.D.].}.|...
+00000a80: 7c02 a101 0100 710a 7c01 5300 7232 0000  |.....q.|.S.r2..
+00000a90: 0029 02da 135f 5069 6543 6861 7274 5f5f  .)..._PieChart__
+00000aa0: 7365 6374 696f 6e73 da06 6170 7065 6e64  sections..append
+00000ab0: 2903 7241 0000 00da 0863 6869 6c64 7265  ).rA.....childre
+00000ac0: 6eda 0264 7372 3800 0000 7238 0000 0072  n..dsr8...r8...r
+00000ad0: 3900 0000 da0d 5f67 6574 5f63 6869 6c64  9....._get_child
+00000ae0: 7265 6e6f 0000 0073 0800 0000 0001 0401  reno...s........
+00000af0: 0a01 0c01 7a16 5069 6543 6861 7274 2e5f  ....z.PieChart._
+00000b00: 6765 745f 6368 696c 6472 656e 6301 0000  get_childrenc...
+00000b10: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000b20: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
+00000b30: 7232 0000 00a9 0172 4a00 0000 7242 0000  r2.....rJ...rB..
+00000b40: 0072 3800 0000 7238 0000 0072 3900 0000  .r8...r8...r9...
+00000b50: 7212 0000 0076 0000 0073 0200 0000 0002  r....v...s......
+00000b60: 7a11 5069 6543 6861 7274 2e73 6563 7469  z.PieChart.secti
+00000b70: 6f6e 7363 0200 0000 0000 0000 0000 0000  onsc............
+00000b80: 0200 0000 0200 0000 4300 0000 7316 0000  ........C...s...
+00000b90: 007c 0164 0075 0172 0c7c 016e 0267 007c  .|.d.u.r.|.n.g.|
+00000ba0: 005f 0064 0053 0072 3200 0000 724f 0000  ._.d.S.r2...rO..
+00000bb0: 00a9 0272 4100 0000 da05 7661 6c75 6572  ...rA.....valuer
+00000bc0: 3800 0000 7238 0000 0072 3900 0000 7212  8...r8...r9...r.
+00000bd0: 0000 007a 0000 0073 0200 0000 0002 a901  ...z...s........
+00000be0: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
+00000bf0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000c00: 0073 0a00 0000 7c00 a000 6401 a101 5300  .s....|...d...S.
+00000c10: a902 4e5a 1063 656e 7465 7253 7061 6365  ..NZ.centerSpace
+00000c20: 436f 6c6f 72a9 01da 095f 6765 745f 6174  Color...._get_at
+00000c30: 7472 7242 0000 0072 3800 0000 7238 0000  trrB...r8...r8..
+00000c40: 0072 3900 0000 7213 0000 007f 0000 0073  .r9...r........s
+00000c50: 0200 0000 0002 7a1b 5069 6543 6861 7274  ......z.PieChart
+00000c60: 2e63 656e 7465 725f 7370 6163 655f 636f  .center_space_co
+00000c70: 6c6f 7229 0172 5100 0000 6302 0000 0000  lor).rQ...c.....
+00000c80: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000c90: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
+00000ca0: a102 0100 6400 5300 7254 0000 00a9 01da  ....d.S.rT......
+00000cb0: 095f 7365 745f 6174 7472 7250 0000 0072  ._set_attrrP...r
+00000cc0: 3800 0000 7238 0000 0072 3900 0000 7213  8...r8...r9...r.
+00000cd0: 0000 0083 0000 0073 0200 0000 0002 6301  .......s......c.
+00000ce0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000cf0: 0000 0043 0000 0073 0e00 0000 7c00 6a00  ...C...s....|.j.
+00000d00: 6401 6402 6403 8d02 5300 2904 4eda 1163  d.d.d...S.).N..c
+00000d10: 656e 7465 7253 7061 6365 5261 6469 7573  enterSpaceRadius
+00000d20: da05 666c 6f61 74a9 01da 0964 6174 615f  ..float....data_
+00000d30: 7479 7065 7255 0000 0072 4200 0000 7238  typerU...rB...r8
+00000d40: 0000 0072 3800 0000 7239 0000 0072 1400  ...r8...r9...r..
+00000d50: 0000 8800 0000 7302 0000 0000 027a 1c50  ......s......z.P
+00000d60: 6965 4368 6172 742e 6365 6e74 6572 5f73  ieChart.center_s
+00000d70: 7061 6365 5f72 6164 6975 7363 0200 0000  pace_radiusc....
+00000d80: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000d90: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
+00000da0: 01a1 0201 0064 0053 0029 024e 7259 0000  .....d.S.).NrY..
+00000db0: 0072 5700 0000 7250 0000 0072 3800 0000  .rW...rP...r8...
+00000dc0: 7238 0000 0072 3900 0000 7214 0000 008c  r8...r9...r.....
+00000dd0: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+00000de0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00000df0: 0000 0073 0e00 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
+00000e00: 6403 8d02 5300 2904 4eda 0d73 6563 7469  d...S.).N..secti
+00000e10: 6f6e 7353 7061 6365 725a 0000 0072 5b00  onsSpacerZ...r[.
+00000e20: 0000 7255 0000 0072 4200 0000 7238 0000  ..rU...rB...r8..
+00000e30: 0072 3800 0000 7239 0000 0072 1500 0000  .r8...r9...r....
+00000e40: 9100 0000 7302 0000 0000 027a 1750 6965  ....s......z.Pie
+00000e50: 4368 6172 742e 7365 6374 696f 6e73 5f73  Chart.sections_s
+00000e60: 7061 6365 6302 0000 0000 0000 0000 0000  pacec...........
+00000e70: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
+00000e80: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
+00000e90: 5300 2902 4e72 5d00 0000 7257 0000 0072  S.).Nr]...rW...r
+00000ea0: 5000 0000 7238 0000 0072 3800 0000 7239  P...r8...r8...r9
+00000eb0: 0000 0072 1500 0000 9500 0000 7302 0000  ...r........s...
+00000ec0: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
+00000ed0: 0100 0000 0400 0000 4300 0000 730e 0000  ........C...s...
+00000ee0: 007c 006a 0064 0164 0264 038d 0253 0029  .|.j.d.d.d...S.)
+00000ef0: 044e da11 7374 6172 7444 6567 7265 654f  .N..startDegreeO
+00000f00: 6666 7365 7472 5a00 0000 725b 0000 0072  ffsetrZ...r[...r
+00000f10: 5500 0000 7242 0000 0072 3800 0000 7238  U...rB...r8...r8
+00000f20: 0000 0072 3900 0000 7216 0000 009a 0000  ...r9...r.......
+00000f30: 0073 0200 0000 0002 7a1c 5069 6543 6861  .s......z.PieCha
+00000f40: 7274 2e73 7461 7274 5f64 6567 7265 655f  rt.start_degree_
+00000f50: 6f66 6673 6574 6302 0000 0000 0000 0000  offsetc.........
+00000f60: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00000f70: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
+00000f80: 6400 5300 2902 4e72 5e00 0000 7257 0000  d.S.).Nr^...rW..
+00000f90: 0072 5000 0000 7238 0000 0072 3800 0000  .rP...r8...r8...
+00000fa0: 7239 0000 0072 1600 0000 9e00 0000 7302  r9...r........s.
+00000fb0: 0000 0000 0263 0100 0000 0000 0000 0000  .....c..........
+00000fc0: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00000fd0: 0000 007c 006a 0053 0072 3200 0000 a901  ...|.j.S.r2.....
+00000fe0: 7247 0000 0072 4200 0000 7238 0000 0072  rG...rB...r8...r
+00000ff0: 3800 0000 7239 0000 0072 1700 0000 a300  8...r9...r......
+00001000: 0000 7302 0000 0000 027a 1050 6965 4368  ..s......z.PieCh
+00001010: 6172 742e 616e 696d 6174 6563 0200 0000  art.animatec....
+00001020: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00001030: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+00001040: 0053 0072 3200 0000 725f 0000 0072 5000  .S.r2...r_...rP.
+00001050: 0000 7238 0000 0072 3800 0000 7239 0000  ..r8...r8...r9..
+00001060: 0072 1700 0000 a700 0000 7302 0000 0000  .r........s.....
+00001070: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001080: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00001090: 006a 0053 0072 3200 0000 2901 723d 0000  .j.S.r2...).r=..
+000010a0: 0072 4200 0000 7238 0000 0072 3800 0000  .rB...r8...r8...
+000010b0: 7239 0000 0072 4000 0000 ac00 0000 7302  r9...r@.......s.
+000010c0: 0000 0000 027a 1750 6965 4368 6172 742e  .....z.PieChart.
+000010d0: 6f6e 5f63 6861 7274 5f65 7665 6e74 6302  on_chart_eventc.
+000010e0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000010f0: 0000 0043 0000 0073 3200 0000 7c00 6a00  ...C...s2...|.j.
+00001100: a001 7c01 a101 0100 7c01 6400 7501 7222  ..|.....|.d.u.r"
+00001110: 7c00 a002 6401 6402 a102 0100 6e0c 7c00  |...d.d.....n.|.
+00001120: a002 6401 6400 a102 0100 6400 5300 2903  ..d.d.....d.S.).
+00001130: 4eda 0c6f 6e43 6861 7274 4576 656e 7454  N..onChartEventT
+00001140: 2903 723d 0000 00da 0973 7562 7363 7269  ).r=.....subscri
+00001150: 6265 7258 0000 0029 0272 4100 0000 da07  berX...).rA.....
+00001160: 6861 6e64 6c65 7272 3800 0000 7238 0000  handlerr8...r8..
+00001170: 0072 3900 0000 7240 0000 00b0 0000 0073  .r9...r@.......s
+00001180: 0800 0000 0002 0c01 0801 0e02 2921 4e4e  ............)!NN
 00001190: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e  NNNNNNNNNNNNNNNN
-000011a0: 4e4e 4e4e 4e4e 4e4e 2920 da08 5f5f 6e61  NNNNNNNN) ..__na
-000011b0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000011c0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7204  ..__qualname__r.
-000011d0: 0000 0072 0300 0000 7206 0000 00da 0373  ...r....r......s
-000011e0: 7472 7208 0000 0072 0c00 0000 720b 0000  trr....r....r...
-000011f0: 0072 0500 0000 da04 626f 6f6c da03 696e  .r......bool..in
-00001200: 7472 0e00 0000 720f 0000 0072 1000 0000  tr....r....r....
-00001210: 720d 0000 0072 0200 0000 723c 0000 0072  r....r....r<...r
-00001220: 4300 0000 7245 0000 0072 4e00 0000 da08  C...rE...rN.....
-00001230: 7072 6f70 6572 7479 7212 0000 00da 0673  propertyr......s
-00001240: 6574 7465 7272 1300 0000 7214 0000 0072  etterr....r....r
-00001250: 1500 0000 7216 0000 0072 1700 0000 7240  ....r....r....r@
-00001260: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00001270: 5f5f 7238 0000 0072 3800 0000 7248 0000  __r8...r8...rH..
-00001280: 0072 3900 0000 7211 0000 0013 0000 0073  .r9...r........s
-00001290: c200 0000 0803 0001 0001 0001 0001 0001  ................
-000012a0: 0001 0004 0001 0001 0001 0001 0001 0001  ................
-000012b0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-000012c0: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-000012d0: 0001 0001 0001 00db 0202 0a01 0601 0201  ................
-000012e0: 0201 0201 0205 0601 0201 0201 0201 0201  ................
-000012f0: 0201 0201 0c01 0601 0601 0201 0201 0201  ................
-00001300: 0201 0201 0201 0201 0201 0201 0201 0202  ................
-00001310: 0601 0601 0601 02db 0c54 0803 0c04 0807  .........T......
-00001320: 0201 0a03 0401 0a04 0201 1403 0401 1404  ................
-00001330: 0201 1003 0401 1004 0201 1003 0401 1004  ................
-00001340: 0201 1003 0401 1004 0201 1003 0401 1004  ................
-00001350: 0201 0a03 0401 7211 0000 0063 0000 0000  ......r....c....
-00001360: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00001370: 4000 0000 731a 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00001380: 0264 0164 029c 0164 0364 0484 045a 0364  .d.d...d.d...Z.d
-00001390: 0153 0029 0572 3500 0000 4e72 5200 0000  .S.).r5...NrR...
-000013a0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-000013b0: 0002 0000 0043 0000 0073 1000 0000 7c01  .....C...s....|.
-000013c0: 7c00 5f00 7c02 7c00 5f01 6400 5300 7232  |._.|.|._.d.S.r2
-000013d0: 0000 0029 02da 0474 7970 65da 0d73 6563  ...)...type..sec
-000013e0: 7469 6f6e 5f69 6e64 6578 2903 7241 0000  tion_index).rA..
-000013f0: 0072 6c00 0000 726d 0000 0072 3800 0000  .rl...rm...r8...
-00001400: 7238 0000 0072 3900 0000 723c 0000 00ba  r8...r9...r<....
-00001410: 0000 0073 0400 0000 0001 0601 7a16 5069  ...s........z.Pi
-00001420: 6543 6861 7274 4576 656e 742e 5f5f 696e  eChartEvent.__in
-00001430: 6974 5f5f 2904 7263 0000 0072 6400 0000  it__).rc...rd...
-00001440: 7265 0000 0072 3c00 0000 7238 0000 0072  re...r<...r8...r
-00001450: 3800 0000 7238 0000 0072 3900 0000 7235  8...r8...r9...r5
-00001460: 0000 00b9 0000 0073 0200 0000 0801 7235  .......s......r5
-00001470: 0000 0029 1a72 3300 0000 da06 7479 7069  ...).r3.....typi
-00001480: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
-00001490: 0072 0500 0000 da22 666c 6574 5f63 6f72  .r....."flet_cor
-000014a0: 652e 6368 6172 7473 2e70 6965 5f63 6861  e.charts.pie_cha
-000014b0: 7274 5f73 6563 7469 6f6e 7206 0000 00da  rt_sectionr.....
-000014c0: 1d66 6c65 745f 636f 7265 2e63 6f6e 7374  .flet_core.const
-000014d0: 7261 696e 6564 5f63 6f6e 7472 6f6c 7207  rained_controlr.
-000014e0: 0000 00da 1166 6c65 745f 636f 7265 2e63  .....flet_core.c
-000014f0: 6f6e 7472 6f6c 7208 0000 00da 1766 6c65  ontrolr......fle
-00001500: 745f 636f 7265 2e63 6f6e 7472 6f6c 5f65  t_core.control_e
-00001510: 7665 6e74 7209 0000 00da 1766 6c65 745f  ventr......flet_
-00001520: 636f 7265 2e65 7665 6e74 5f68 616e 646c  core.event_handl
-00001530: 6572 720a 0000 00da 0d66 6c65 745f 636f  err......flet_co
-00001540: 7265 2e72 6566 720b 0000 00da 0f66 6c65  re.refr......fle
-00001550: 745f 636f 7265 2e74 7970 6573 720c 0000  t_core.typesr...
-00001560: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00001570: 7210 0000 0072 1100 0000 7235 0000 0072  r....r....r5...r
-00001580: 3800 0000 7238 0000 0072 3800 0000 7239  8...r8...r8...r9
-00001590: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000015a0: 0073 1600 0000 0801 1802 0c01 0c01 0c01  .s..............
-000015b0: 0c01 0c01 0c01 1c09 107f 0027            ...........'
+000011a0: 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e29  NNNNNNNNNNNNNNN)
+000011b0: 20da 085f 5f6e 616d 655f 5fda 0a5f 5f6d   ..__name__..__m
+000011c0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000011d0: 616d 655f 5f72 0400 0000 7203 0000 0072  ame__r....r....r
+000011e0: 0600 0000 da03 7374 7272 0800 0000 720c  ......strr....r.
+000011f0: 0000 0072 0b00 0000 7205 0000 00da 0462  ...r....r......b
+00001200: 6f6f 6cda 0369 6e74 720e 0000 0072 0f00  ool..intr....r..
+00001210: 0000 7210 0000 0072 0d00 0000 7202 0000  ..r....r....r...
+00001220: 0072 3c00 0000 7243 0000 0072 4500 0000  .r<...rC...rE...
+00001230: 724e 0000 00da 0870 726f 7065 7274 7972  rN.....propertyr
+00001240: 1200 0000 da06 7365 7474 6572 7213 0000  ......setterr...
+00001250: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001260: 7217 0000 0072 4000 0000 da0d 5f5f 636c  r....r@.....__cl
+00001270: 6173 7363 656c 6c5f 5f72 3800 0000 7238  asscell__r8...r8
+00001280: 0000 0072 4800 0000 7239 0000 0072 1100  ...rH...r9...r..
+00001290: 0000 1300 0000 73c2 0000 0008 0300 0100  ......s.........
+000012a0: 0100 0100 0100 0100 0100 0400 0100 0100  ................
+000012b0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+000012c0: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+000012d0: 0100 0100 0100 0100 0100 0100 0100 db02  ................
+000012e0: 020a 0106 0102 0102 0102 0102 0506 0102  ................
+000012f0: 0102 0102 0102 0102 0102 010c 0106 0106  ................
+00001300: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00001310: 0102 0102 0102 0206 0106 0106 0102 db0c  ................
+00001320: 5408 030c 0408 0702 010a 0304 010a 0402  T...............
+00001330: 0114 0304 0114 0402 0110 0304 0110 0402  ................
+00001340: 0110 0304 0110 0402 0110 0304 0110 0402  ................
+00001350: 0110 0304 0110 0402 010a 0304 0172 1100  .............r..
+00001360: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001370: 0000 0003 0000 0040 0000 0073 1a00 0000  .......@...s....
+00001380: 6500 5a01 6400 5a02 6401 6402 9c01 6403  e.Z.d.Z.d.d...d.
+00001390: 6404 8404 5a03 6401 5300 2905 7235 0000  d...Z.d.S.).r5..
+000013a0: 004e 7252 0000 0063 0300 0000 0000 0000  .NrR...c........
+000013b0: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+000013c0: 7310 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
+000013d0: 0164 0053 0072 3200 0000 2902 da04 7479  .d.S.r2...)...ty
+000013e0: 7065 da0d 7365 6374 696f 6e5f 696e 6465  pe..section_inde
+000013f0: 7829 0372 4100 0000 726c 0000 0072 6d00  x).rA...rl...rm.
+00001400: 0000 7238 0000 0072 3800 0000 7239 0000  ..r8...r8...r9..
+00001410: 0072 3c00 0000 ba00 0000 7304 0000 0000  .r<.......s.....
+00001420: 0106 017a 1650 6965 4368 6172 7445 7665  ...z.PieChartEve
+00001430: 6e74 2e5f 5f69 6e69 745f 5f29 0472 6300  nt.__init__).rc.
+00001440: 0000 7264 0000 0072 6500 0000 723c 0000  ..rd...re...r<..
+00001450: 0072 3800 0000 7238 0000 0072 3800 0000  .r8...r8...r8...
+00001460: 7239 0000 0072 3500 0000 b900 0000 7302  r9...r5.......s.
+00001470: 0000 0008 0172 3500 0000 291a 7233 0000  .....r5...).r3..
+00001480: 00da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
+00001490: 0000 0072 0400 0000 7205 0000 00da 2266  ...r....r....."f
+000014a0: 6c65 745f 636f 7265 2e63 6861 7274 732e  let_core.charts.
+000014b0: 7069 655f 6368 6172 745f 7365 6374 696f  pie_chart_sectio
+000014c0: 6e72 0600 0000 da1d 666c 6574 5f63 6f72  nr......flet_cor
+000014d0: 652e 636f 6e73 7472 6169 6e65 645f 636f  e.constrained_co
+000014e0: 6e74 726f 6c72 0700 0000 da11 666c 6574  ntrolr......flet
+000014f0: 5f63 6f72 652e 636f 6e74 726f 6c72 0800  _core.controlr..
+00001500: 0000 da17 666c 6574 5f63 6f72 652e 636f  ....flet_core.co
+00001510: 6e74 726f 6c5f 6576 656e 7472 0900 0000  ntrol_eventr....
+00001520: da17 666c 6574 5f63 6f72 652e 6576 656e  ..flet_core.even
+00001530: 745f 6861 6e64 6c65 7272 0a00 0000 da0d  t_handlerr......
+00001540: 666c 6574 5f63 6f72 652e 7265 6672 0b00  flet_core.refr..
+00001550: 0000 da0f 666c 6574 5f63 6f72 652e 7479  ....flet_core.ty
+00001560: 7065 7372 0c00 0000 720d 0000 0072 0e00  pesr....r....r..
+00001570: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00001580: 0072 3500 0000 7238 0000 0072 3800 0000  .r5...r8...r8...
+00001590: 7238 0000 0072 3900 0000 da08 3c6d 6f64  r8...r9.....<mod
+000015a0: 756c 653e 0100 0000 7316 0000 0008 0118  ule>....s.......
+000015b0: 020c 010c 010c 010c 010c 010c 011c 0910  ................
+000015c0: 7f00 27                                  ..'
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 3807 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 df0e 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 df0e 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 6506 8303  ..G.d.d...d.e...
@@ -65,218 +65,219 @@
 00000400: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
 00000410: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
 00000420: 0000 7211 0000 0072 1200 0000 290e da04  ..r....r....)...
 00000430: 7365 6c66 720a 0000 0072 0b00 0000 720c  selfr....r....r.
 00000440: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
 00000450: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
 00000460: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000470: 7216 0000 00a9 0072 1900 0000 fa64 2f77  r......r.....d/w
+00000470: 7216 0000 00a9 0072 1900 0000 fa6b 2f77  r......r.....k/w
 00000480: 6f72 6b73 7061 6365 732f 636f 6e74 7269  orkspaces/contri
-00000490: 6266 6c65 742f 666c 6574 2f73 646b 2f70  bflet/flet/sdk/p
-000004a0: 7974 686f 6e2f 7061 636b 6167 6573 2f66  ython/packages/f
-000004b0: 6c65 742d 636f 7265 2f73 7263 2f66 6c65  let-core/src/fle
-000004c0: 745f 636f 7265 2f63 6861 7274 732f 7069  t_core/charts/pi
-000004d0: 655f 6368 6172 745f 7365 6374 696f 6e2e  e_chart_section.
-000004e0: 7079 7217 0000 000a 0000 0073 2000 0000  pyr........s ...
-000004f0: 0014 0401 0201 0201 0201 0201 02fb 0608  ................
-00000500: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00000510: 7a18 5069 6543 6861 7274 5365 6374 696f  z.PieChartSectio
-00000520: 6e2e 5f5f 696e 6974 5f5f 6301 0000 0000  n.__init__c.....
-00000530: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000540: 0000 0073 0400 0000 6401 5300 2902 4e5a  ...s....d.S.).NZ
-00000550: 0773 6563 7469 6f6e 7219 0000 00a9 0172  .sectionr......r
-00000560: 1800 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00000570: 0000 00da 115f 6765 745f 636f 6e74 726f  ....._get_contro
-00000580: 6c5f 6e61 6d65 3000 0000 7302 0000 0000  l_name0...s.....
-00000590: 017a 2150 6965 4368 6172 7453 6563 7469  .z!PieChartSecti
-000005a0: 6f6e 2e5f 6765 745f 636f 6e74 726f 6c5f  on._get_control_
-000005b0: 6e61 6d65 6301 0000 0000 0000 0000 0000  namec...........
-000005c0: 0001 0000 0004 0000 0003 0000 0073 2a00  .............s*.
-000005d0: 0000 7400 8300 a001 a100 0100 7c00 a002  ..t.........|...
-000005e0: 6401 7c00 6a03 a102 0100 7c00 a002 6402  d.|.j.....|...d.
-000005f0: 7c00 6a04 a102 0100 6400 5300 2903 4eda  |.j.....d.S.).N.
-00000600: 0a62 6f72 6465 7253 6964 655a 0a74 6974  .borderSideZ.tit
-00000610: 6c65 5374 796c 6529 05da 0573 7570 6572  leStyle)...super
-00000620: da0d 6265 666f 7265 5f75 7064 6174 65da  ..before_update.
-00000630: 0e5f 7365 745f 6174 7472 5f6a 736f 6eda  ._set_attr_json.
-00000640: 1d5f 5069 6543 6861 7274 5365 6374 696f  ._PieChartSectio
-00000650: 6e5f 5f62 6f72 6465 725f 7369 6465 da1d  n__border_side..
-00000660: 5f50 6965 4368 6172 7453 6563 7469 6f6e  _PieChartSection
-00000670: 5f5f 7469 746c 655f 7374 796c 6572 1b00  __title_styler..
-00000680: 0000 a901 da09 5f5f 636c 6173 735f 5f72  ......__class__r
-00000690: 1900 0000 721a 0000 0072 1f00 0000 3300  ....r....r....3.
-000006a0: 0000 7306 0000 0000 010a 010e 017a 1d50  ..s..........z.P
-000006b0: 6965 4368 6172 7453 6563 7469 6f6e 2e62  ieChartSection.b
-000006c0: 6566 6f72 655f 7570 6461 7465 6301 0000  efore_updatec...
-000006d0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000006e0: 0043 0000 0073 2800 0000 6700 7d01 7c00  .C...s(...g.}.|.
-000006f0: 6a00 7224 7c00 6a00 a001 6401 6402 a102  j.r$|.j...d.d...
-00000700: 0100 7c01 a002 7c00 6a00 a101 0100 7c01  ..|...|.j.....|.
-00000710: 5300 2903 4eda 016e 7211 0000 0029 03da  S.).N..nr....)..
-00000720: 175f 5069 6543 6861 7274 5365 6374 696f  ._PieChartSectio
-00000730: 6e5f 5f62 6164 6765 da12 5f73 6574 5f61  n__badge.._set_a
-00000740: 7474 725f 696e 7465 726e 616c da06 6170  ttr_internal..ap
-00000750: 7065 6e64 2902 7218 0000 00da 0863 6869  pend).r......chi
-00000760: 6c64 7265 6e72 1900 0000 7219 0000 0072  ldrenr....r....r
-00000770: 1a00 0000 da0d 5f67 6574 5f63 6869 6c64  ......_get_child
-00000780: 7265 6e38 0000 0073 0a00 0000 0001 0401  ren8...s........
-00000790: 0601 0e01 0c01 7a1d 5069 6543 6861 7274  ......z.PieChart
-000007a0: 5365 6374 696f 6e2e 5f67 6574 5f63 6869  Section._get_chi
-000007b0: 6c64 7265 6e29 01da 0672 6574 7572 6e63  ldren)...returnc
-000007c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000007d0: 0400 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
-000007e0: 0064 0164 0264 038d 0253 0029 044e 720a  .d.d.d...S.).Nr.
-000007f0: 0000 00da 0566 6c6f 6174 a901 da09 6461  .....float....da
-00000800: 7461 5f74 7970 65a9 01da 095f 6765 745f  ta_type...._get_
-00000810: 6174 7472 721b 0000 0072 1900 0000 7219  attrr....r....r.
-00000820: 0000 0072 1a00 0000 720a 0000 0040 0000  ...r....r....@..
-00000830: 0073 0200 0000 0002 7a15 5069 6543 6861  .s......z.PieCha
-00000840: 7274 5365 6374 696f 6e2e 7661 6c75 6529  rtSection.value)
-00000850: 0172 0a00 0000 6302 0000 0000 0000 0000  .r....c.........
-00000860: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-00000870: 1000 0000 7c00 a000 6401 7c01 a102 0100  ....|...d.|.....
-00000880: 6400 5300 2902 4e72 0a00 0000 a901 da09  d.S.).Nr........
-00000890: 5f73 6574 5f61 7474 72a9 0272 1800 0000  _set_attr..r....
-000008a0: 720a 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000008b0: 1a00 0000 720a 0000 0044 0000 0073 0200  ....r....D...s..
-000008c0: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-000008d0: 0001 0000 0004 0000 0043 0000 0073 0e00  .........C...s..
-000008e0: 0000 7c00 6a00 6401 6402 6403 8d02 5300  ..|.j.d.d.d...S.
-000008f0: 2904 4e72 0b00 0000 722c 0000 0072 2d00  ).Nr....r,...r-.
-00000900: 0000 722f 0000 0072 1b00 0000 7219 0000  ..r/...r....r...
-00000910: 0072 1900 0000 721a 0000 0072 0b00 0000  .r....r....r....
-00000920: 4900 0000 7302 0000 0000 027a 1650 6965  I...s......z.Pie
-00000930: 4368 6172 7453 6563 7469 6f6e 2e72 6164  ChartSection.rad
-00000940: 6975 7363 0200 0000 0000 0000 0000 0000  iusc............
-00000950: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
-00000960: 007c 00a0 0064 017c 01a1 0201 0064 0053  .|...d.|.....d.S
-00000970: 0029 024e 720b 0000 0072 3100 0000 7233  .).Nr....r1...r3
-00000980: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00000990: 0000 720b 0000 004d 0000 0073 0200 0000  ..r....M...s....
-000009a0: 0002 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000009b0: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
-000009c0: 7c00 6a00 5300 a901 4ea9 0172 2100 0000  |.j.S...N..r!...
-000009d0: 721b 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000009e0: 1a00 0000 720d 0000 0052 0000 0073 0200  ....r....R...s..
-000009f0: 0000 0002 7a1b 5069 6543 6861 7274 5365  ....z.PieChartSe
-00000a00: 6374 696f 6e2e 626f 7264 6572 5f73 6964  ction.border_sid
-00000a10: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00000a20: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000a30: 017c 005f 0064 0053 0072 3400 0000 7235  .|._.d.S.r4...r5
-00000a40: 0000 0072 3300 0000 7219 0000 0072 1900  ...r3...r....r..
-00000a50: 0000 721a 0000 0072 0d00 0000 5600 0000  ..r....r....V...
-00000a60: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00000a70: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00000a80: 730a 0000 007c 00a0 0064 01a1 0153 00a9  s....|...d...S..
-00000a90: 024e 720c 0000 0072 2f00 0000 721b 0000  .Nr....r/...r...
-00000aa0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000ab0: 720c 0000 005b 0000 0073 0200 0000 0002  r....[...s......
-00000ac0: 7a15 5069 6543 6861 7274 5365 6374 696f  z.PieChartSectio
-00000ad0: 6e2e 636f 6c6f 7263 0200 0000 0000 0000  n.colorc........
-00000ae0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000af0: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
-00000b00: 0064 0053 0072 3600 0000 7231 0000 0072  .d.S.r6...r1...r
-00000b10: 3300 0000 7219 0000 0072 1900 0000 721a  3...r....r....r.
-00000b20: 0000 0072 0c00 0000 5f00 0000 7302 0000  ...r...._...s...
-00000b30: 0000 0263 0100 0000 0000 0000 0000 0000  ...c............
-00000b40: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
-00000b50: 007c 006a 0053 0072 3400 0000 a901 7226  .|.j.S.r4.....r&
-00000b60: 0000 0072 1b00 0000 7219 0000 0072 1900  ...r....r....r..
-00000b70: 0000 721a 0000 0072 1100 0000 6400 0000  ..r....r....d...
-00000b80: 7302 0000 0000 027a 1550 6965 4368 6172  s......z.PieChar
-00000b90: 7453 6563 7469 6f6e 2e62 6164 6765 6302  tSection.badgec.
-00000ba0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000bb0: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
-00000bc0: 5f00 6400 5300 7234 0000 0072 3700 0000  _.d.S.r4...r7...
-00000bd0: 7233 0000 0072 1900 0000 7219 0000 0072  r3...r....r....r
-00000be0: 1a00 0000 7211 0000 0068 0000 0073 0200  ....r....h...s..
-00000bf0: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000c00: 0001 0000 0004 0000 0043 0000 0073 0e00  .........C...s..
-00000c10: 0000 7c00 6a00 6401 6402 6403 8d02 5300  ..|.j.d.d.d...S.
-00000c20: 2904 4eda 0d62 6164 6765 506f 7369 7469  ).N..badgePositi
-00000c30: 6f6e 722c 0000 0072 2d00 0000 722f 0000  onr,...r-...r/..
-00000c40: 0072 1b00 0000 7219 0000 0072 1900 0000  .r....r....r....
-00000c50: 721a 0000 0072 1200 0000 6d00 0000 7302  r....r....m...s.
-00000c60: 0000 0000 027a 1e50 6965 4368 6172 7453  .....z.PieChartS
-00000c70: 6563 7469 6f6e 2e62 6164 6765 5f70 6f73  ection.badge_pos
-00000c80: 6974 696f 6e63 0200 0000 0000 0000 0000  itionc..........
-00000c90: 0000 0200 0000 0400 0000 4300 0000 7310  ..........C...s.
-00000ca0: 0000 007c 00a0 0064 017c 01a1 0201 0064  ...|...d.|.....d
-00000cb0: 0053 0029 024e 7238 0000 0072 3100 0000  .S.).Nr8...r1...
-00000cc0: 7233 0000 0072 1900 0000 7219 0000 0072  r3...r....r....r
-00000cd0: 1a00 0000 7212 0000 0071 0000 0073 0200  ....r....q...s..
-00000ce0: 0000 0002 6301 0000 0000 0000 0000 0000  ....c...........
-00000cf0: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-00000d00: 0000 7c00 a000 6401 a101 5300 a902 4e72  ..|...d...S...Nr
-00000d10: 0e00 0000 722f 0000 0072 1b00 0000 7219  ....r/...r....r.
-00000d20: 0000 0072 1900 0000 721a 0000 0072 0e00  ...r....r....r..
-00000d30: 0000 7600 0000 7302 0000 0000 027a 1550  ..v...s......z.P
-00000d40: 6965 4368 6172 7453 6563 7469 6f6e 2e74  ieChartSection.t
-00000d50: 6974 6c65 6302 0000 0000 0000 0000 0000  itlec...........
-00000d60: 0002 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00000d70: 0000 7c00 a000 6401 7c01 a102 0100 6400  ..|...d.|.....d.
-00000d80: 5300 7239 0000 0072 3100 0000 7233 0000  S.r9...r1...r3..
-00000d90: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000da0: 720e 0000 007a 0000 0073 0200 0000 0002  r....z...s......
-00000db0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000dc0: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00000dd0: 6a00 5300 7234 0000 00a9 0172 2200 0000  j.S.r4.....r"...
-00000de0: 721b 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000df0: 1a00 0000 720f 0000 007f 0000 0073 0200  ....r........s..
-00000e00: 0000 0002 7a1b 5069 6543 6861 7274 5365  ....z.PieChartSe
-00000e10: 6374 696f 6e2e 7469 746c 655f 7374 796c  ction.title_styl
-00000e20: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00000e30: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000e40: 017c 005f 0064 0053 0072 3400 0000 723a  .|._.d.S.r4...r:
-00000e50: 0000 0072 3300 0000 7219 0000 0072 1900  ...r3...r....r..
-00000e60: 0000 721a 0000 0072 0f00 0000 8300 0000  ..r....r........
-00000e70: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
-00000e80: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00000e90: 7310 0000 007c 006a 0064 0164 0264 0364  s....|.j.d.d.d.d
-00000ea0: 048d 0353 0029 054e da0d 7469 746c 6550  ...S.).N..titleP
-00000eb0: 6f73 6974 696f 6e72 2c00 0000 6700 0000  ositionr,...g...
-00000ec0: 0000 00f0 3f29 0272 2e00 0000 da09 6465  ....?).r......de
-00000ed0: 665f 7661 6c75 6572 2f00 0000 721b 0000  f_valuer/...r...
-00000ee0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000ef0: 7210 0000 0088 0000 0073 0200 0000 0002  r........s......
-00000f00: 7a1e 5069 6543 6861 7274 5365 6374 696f  z.PieChartSectio
-00000f10: 6e2e 7469 746c 655f 706f 7369 7469 6f6e  n.title_position
-00000f20: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000f30: 0004 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00000f40: a000 6401 7c01 a102 0100 6400 5300 2902  ..d.|.....d.S.).
-00000f50: 4e72 3b00 0000 7231 0000 0072 3300 0000  Nr;...r1...r3...
-00000f60: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000f70: 1000 0000 8c00 0000 7302 0000 0000 0229  ........s......)
-00000f80: 0d4e 4e4e 4e4e 4e4e 4e4e 4e4e 4e4e 291c  .NNNNNNNNNNNNN).
-00000f90: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000fa0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000fb0: 6d65 5f5f 7206 0000 0072 0300 0000 da03  me__r....r......
-00000fc0: 7374 7272 0400 0000 7208 0000 0072 0500  strr....r....r..
-00000fd0: 0000 7207 0000 00da 0462 6f6f 6c72 0200  ..r......boolr..
-00000fe0: 0000 7217 0000 0072 1c00 0000 721f 0000  ..r....r....r...
-00000ff0: 0072 2a00 0000 da08 7072 6f70 6572 7479  .r*.....property
-00001000: 720a 0000 00da 0673 6574 7465 7272 0b00  r......setterr..
-00001010: 0000 720d 0000 0072 0c00 0000 7211 0000  ..r....r....r...
-00001020: 0072 1200 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00001030: 7210 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-00001040: 6c6c 5f5f 7219 0000 0072 1900 0000 7223  ll__r....r....r#
-00001050: 0000 0072 1a00 0000 7209 0000 0009 0000  ...r....r.......
-00001060: 0073 8600 0000 0803 0001 0001 0001 0001  .s..............
-00001070: 0001 0001 0001 0001 0004 0001 0001 0001  ................
-00001080: 00ef 0202 0201 0201 0601 0601 0601 0601  ................
-00001090: 0201 0601 0204 0601 0601 0601 02ef 0c26  ...............&
-000010a0: 0803 0c05 0808 0201 1003 0401 1004 0201  ................
-000010b0: 1003 0401 1004 0201 1403 0401 1404 0201  ................
-000010c0: 1403 0401 1404 0201 1403 0401 1404 0201  ................
-000010d0: 1003 0401 1004 0201 0a03 0401 1404 0201  ................
-000010e0: 0a03 0401 1404 0201 1003 0401 7209 0000  ............r...
-000010f0: 004e 290d da06 7479 7069 6e67 7202 0000  .N)...typingr...
-00001100: 0072 0300 0000 da10 666c 6574 5f63 6f72  .r......flet_cor
-00001110: 652e 626f 7264 6572 7204 0000 00da 1166  e.borderr......f
-00001120: 6c65 745f 636f 7265 2e63 6f6e 7472 6f6c  let_core.control
-00001130: 7205 0000 0072 0600 0000 da0d 666c 6574  r....r......flet
-00001140: 5f63 6f72 652e 7265 6672 0700 0000 da14  _core.refr......
-00001150: 666c 6574 5f63 6f72 652e 7465 7874 5f73  flet_core.text_s
-00001160: 7479 6c65 7208 0000 0072 0900 0000 7219  tyler....r....r.
-00001170: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00001180: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001190: 730a 0000 0010 020c 0110 010c 010c 03    s..............
+00000490: 6266 6c65 742f 666c 6574 636f 6e74 7269  bflet/fletcontri
+000004a0: 622f 7364 6b2f 7079 7468 6f6e 2f70 6163  b/sdk/python/pac
+000004b0: 6b61 6765 732f 666c 6574 2d63 6f72 652f  kages/flet-core/
+000004c0: 7372 632f 666c 6574 5f63 6f72 652f 6368  src/flet_core/ch
+000004d0: 6172 7473 2f70 6965 5f63 6861 7274 5f73  arts/pie_chart_s
+000004e0: 6563 7469 6f6e 2e70 7972 1700 0000 0a00  ection.pyr......
+000004f0: 0000 7320 0000 0000 1404 0102 0102 0102  ..s ............
+00000500: 0102 0102 fb06 0806 0106 0106 0106 0106  ................
+00000510: 0106 0106 0106 017a 1850 6965 4368 6172  .......z.PieChar
+00000520: 7453 6563 7469 6f6e 2e5f 5f69 6e69 745f  tSection.__init_
+00000530: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000540: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
+00000550: 0153 0029 024e 5a07 7365 6374 696f 6e72  .S.).NZ.sectionr
+00000560: 1900 0000 a901 7218 0000 0072 1900 0000  ......r....r....
+00000570: 7219 0000 0072 1a00 0000 da11 5f67 6574  r....r......_get
+00000580: 5f63 6f6e 7472 6f6c 5f6e 616d 6530 0000  _control_name0..
+00000590: 0073 0200 0000 0001 7a21 5069 6543 6861  .s......z!PieCha
+000005a0: 7274 5365 6374 696f 6e2e 5f67 6574 5f63  rtSection._get_c
+000005b0: 6f6e 7472 6f6c 5f6e 616d 6563 0100 0000  ontrol_namec....
+000005c0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000005d0: 0300 0000 732a 0000 0074 0083 00a0 01a1  ....s*...t......
+000005e0: 0001 007c 00a0 0264 017c 006a 03a1 0201  ...|...d.|.j....
+000005f0: 007c 00a0 0264 027c 006a 04a1 0201 0064  .|...d.|.j.....d
+00000600: 0053 0029 034e da0a 626f 7264 6572 5369  .S.).N..borderSi
+00000610: 6465 5a0a 7469 746c 6553 7479 6c65 2905  deZ.titleStyle).
+00000620: da05 7375 7065 72da 0d62 6566 6f72 655f  ..super..before_
+00000630: 7570 6461 7465 da0e 5f73 6574 5f61 7474  update.._set_att
+00000640: 725f 6a73 6f6e da1d 5f50 6965 4368 6172  r_json.._PieChar
+00000650: 7453 6563 7469 6f6e 5f5f 626f 7264 6572  tSection__border
+00000660: 5f73 6964 65da 1d5f 5069 6543 6861 7274  _side.._PieChart
+00000670: 5365 6374 696f 6e5f 5f74 6974 6c65 5f73  Section__title_s
+00000680: 7479 6c65 721b 0000 00a9 01da 095f 5f63  tyler........__c
+00000690: 6c61 7373 5f5f 7219 0000 0072 1a00 0000  lass__r....r....
+000006a0: 721f 0000 0033 0000 0073 0600 0000 0001  r....3...s......
+000006b0: 0a01 0e01 7a1d 5069 6543 6861 7274 5365  ....z.PieChartSe
+000006c0: 6374 696f 6e2e 6265 666f 7265 5f75 7064  ction.before_upd
+000006d0: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
+000006e0: 0200 0000 0400 0000 4300 0000 7328 0000  ........C...s(..
+000006f0: 0067 007d 017c 006a 0072 247c 006a 00a0  .g.}.|.j.r$|.j..
+00000700: 0164 0164 02a1 0201 007c 01a0 027c 006a  .d.d.....|...|.j
+00000710: 00a1 0101 007c 0153 0029 034e da01 6e72  .....|.S.).N..nr
+00000720: 1100 0000 2903 da17 5f50 6965 4368 6172  ....)..._PieChar
+00000730: 7453 6563 7469 6f6e 5f5f 6261 6467 65da  tSection__badge.
+00000740: 125f 7365 745f 6174 7472 5f69 6e74 6572  ._set_attr_inter
+00000750: 6e61 6cda 0661 7070 656e 6429 0272 1800  nal..append).r..
+00000760: 0000 da08 6368 696c 6472 656e 7219 0000  ....childrenr...
+00000770: 0072 1900 0000 721a 0000 00da 0d5f 6765  .r....r......_ge
+00000780: 745f 6368 696c 6472 656e 3800 0000 730a  t_children8...s.
+00000790: 0000 0000 0104 0106 010e 010c 017a 1d50  .............z.P
+000007a0: 6965 4368 6172 7453 6563 7469 6f6e 2e5f  ieChartSection._
+000007b0: 6765 745f 6368 696c 6472 656e 2901 da06  get_children)...
+000007c0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+000007d0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+000007e0: 0e00 0000 7c00 6a00 6401 6402 6403 8d02  ....|.j.d.d.d...
+000007f0: 5300 2904 4e72 0a00 0000 da05 666c 6f61  S.).Nr......floa
+00000800: 74a9 01da 0964 6174 615f 7479 7065 a901  t....data_type..
+00000810: da09 5f67 6574 5f61 7474 7272 1b00 0000  .._get_attrr....
+00000820: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000830: 0a00 0000 4000 0000 7302 0000 0000 027a  ....@...s......z
+00000840: 1550 6965 4368 6172 7453 6563 7469 6f6e  .PieChartSection
+00000850: 2e76 616c 7565 2901 720a 0000 0063 0200  .value).r....c..
+00000860: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000870: 0000 4300 0000 7310 0000 007c 00a0 0064  ..C...s....|...d
+00000880: 017c 01a1 0201 0064 0053 0029 024e 720a  .|.....d.S.).Nr.
+00000890: 0000 00a9 01da 095f 7365 745f 6174 7472  ......._set_attr
+000008a0: a902 7218 0000 0072 0a00 0000 7219 0000  ..r....r....r...
+000008b0: 0072 1900 0000 721a 0000 0072 0a00 0000  .r....r....r....
+000008c0: 4400 0000 7302 0000 0000 0263 0100 0000  D...s......c....
+000008d0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+000008e0: 4300 0000 730e 0000 007c 006a 0064 0164  C...s....|.j.d.d
+000008f0: 0264 038d 0253 0029 044e 720b 0000 0072  .d...S.).Nr....r
+00000900: 2c00 0000 722d 0000 0072 2f00 0000 721b  ,...r-...r/...r.
+00000910: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00000920: 0000 720b 0000 0049 0000 0073 0200 0000  ..r....I...s....
+00000930: 0002 7a16 5069 6543 6861 7274 5365 6374  ..z.PieChartSect
+00000940: 696f 6e2e 7261 6469 7573 6302 0000 0000  ion.radiusc.....
+00000950: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000960: 0000 0073 1000 0000 7c00 a000 6401 7c01  ...s....|...d.|.
+00000970: a102 0100 6400 5300 2902 4e72 0b00 0000  ....d.S.).Nr....
+00000980: 7231 0000 0072 3300 0000 7219 0000 0072  r1...r3...r....r
+00000990: 1900 0000 721a 0000 0072 0b00 0000 4d00  ....r....r....M.
+000009a0: 0000 7302 0000 0000 0263 0100 0000 0000  ..s......c......
+000009b0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+000009c0: 0000 7306 0000 007c 006a 0053 00a9 014e  ..s....|.j.S...N
+000009d0: a901 7221 0000 0072 1b00 0000 7219 0000  ..r!...r....r...
+000009e0: 0072 1900 0000 721a 0000 0072 0d00 0000  .r....r....r....
+000009f0: 5200 0000 7302 0000 0000 027a 1b50 6965  R...s......z.Pie
+00000a00: 4368 6172 7453 6563 7469 6f6e 2e62 6f72  ChartSection.bor
+00000a10: 6465 725f 7369 6465 6302 0000 0000 0000  der_sidec.......
+00000a20: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00000a30: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00000a40: 7234 0000 0072 3500 0000 7233 0000 0072  r4...r5...r3...r
+00000a50: 1900 0000 7219 0000 0072 1a00 0000 720d  ....r....r....r.
+00000a60: 0000 0056 0000 0073 0200 0000 0002 6301  ...V...s......c.
+00000a70: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000a80: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
+00000a90: 6401 a101 5300 a902 4e72 0c00 0000 722f  d...S...Nr....r/
+00000aa0: 0000 0072 1b00 0000 7219 0000 0072 1900  ...r....r....r..
+00000ab0: 0000 721a 0000 0072 0c00 0000 5b00 0000  ..r....r....[...
+00000ac0: 7302 0000 0000 027a 1550 6965 4368 6172  s......z.PieChar
+00000ad0: 7453 6563 7469 6f6e 2e63 6f6c 6f72 6302  tSection.colorc.
+00000ae0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000af0: 0000 0043 0000 0073 1000 0000 7c00 a000  ...C...s....|...
+00000b00: 6401 7c01 a102 0100 6400 5300 7236 0000  d.|.....d.S.r6..
+00000b10: 0072 3100 0000 7233 0000 0072 1900 0000  .r1...r3...r....
+00000b20: 7219 0000 0072 1a00 0000 720c 0000 005f  r....r....r...._
+00000b30: 0000 0073 0200 0000 0002 6301 0000 0000  ...s......c.....
+00000b40: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000b50: 0000 0073 0600 0000 7c00 6a00 5300 7234  ...s....|.j.S.r4
+00000b60: 0000 00a9 0172 2600 0000 721b 0000 0072  .....r&...r....r
+00000b70: 1900 0000 7219 0000 0072 1a00 0000 7211  ....r....r....r.
+00000b80: 0000 0064 0000 0073 0200 0000 0002 7a15  ...d...s......z.
+00000b90: 5069 6543 6861 7274 5365 6374 696f 6e2e  PieChartSection.
+00000ba0: 6261 6467 6563 0200 0000 0000 0000 0000  badgec..........
+00000bb0: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000bc0: 0000 007c 017c 005f 0064 0053 0072 3400  ...|.|._.d.S.r4.
+00000bd0: 0000 7237 0000 0072 3300 0000 7219 0000  ..r7...r3...r...
+00000be0: 0072 1900 0000 721a 0000 0072 1100 0000  .r....r....r....
+00000bf0: 6800 0000 7302 0000 0000 0263 0100 0000  h...s......c....
+00000c00: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000c10: 4300 0000 730e 0000 007c 006a 0064 0164  C...s....|.j.d.d
+00000c20: 0264 038d 0253 0029 044e da0d 6261 6467  .d...S.).N..badg
+00000c30: 6550 6f73 6974 696f 6e72 2c00 0000 722d  ePositionr,...r-
+00000c40: 0000 0072 2f00 0000 721b 0000 0072 1900  ...r/...r....r..
+00000c50: 0000 7219 0000 0072 1a00 0000 7212 0000  ..r....r....r...
+00000c60: 006d 0000 0073 0200 0000 0002 7a1e 5069  .m...s......z.Pi
+00000c70: 6543 6861 7274 5365 6374 696f 6e2e 6261  eChartSection.ba
+00000c80: 6467 655f 706f 7369 7469 6f6e 6302 0000  dge_positionc...
+00000c90: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000ca0: 0043 0000 0073 1000 0000 7c00 a000 6401  .C...s....|...d.
+00000cb0: 7c01 a102 0100 6400 5300 2902 4e72 3800  |.....d.S.).Nr8.
+00000cc0: 0000 7231 0000 0072 3300 0000 7219 0000  ..r1...r3...r...
+00000cd0: 0072 1900 0000 721a 0000 0072 1200 0000  .r....r....r....
+00000ce0: 7100 0000 7302 0000 0000 0263 0100 0000  q...s......c....
+00000cf0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000d00: 4300 0000 730a 0000 007c 00a0 0064 01a1  C...s....|...d..
+00000d10: 0153 00a9 024e 720e 0000 0072 2f00 0000  .S...Nr....r/...
+00000d20: 721b 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000d30: 1a00 0000 720e 0000 0076 0000 0073 0200  ....r....v...s..
+00000d40: 0000 0002 7a15 5069 6543 6861 7274 5365  ....z.PieChartSe
+00000d50: 6374 696f 6e2e 7469 746c 6563 0200 0000  ction.titlec....
+00000d60: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000d70: 4300 0000 7310 0000 007c 00a0 0064 017c  C...s....|...d.|
+00000d80: 01a1 0201 0064 0053 0072 3900 0000 7231  .....d.S.r9...r1
+00000d90: 0000 0072 3300 0000 7219 0000 0072 1900  ...r3...r....r..
+00000da0: 0000 721a 0000 0072 0e00 0000 7a00 0000  ..r....r....z...
+00000db0: 7302 0000 0000 0263 0100 0000 0000 0000  s......c........
+00000dc0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000dd0: 7306 0000 007c 006a 0053 0072 3400 0000  s....|.j.S.r4...
+00000de0: a901 7222 0000 0072 1b00 0000 7219 0000  ..r"...r....r...
+00000df0: 0072 1900 0000 721a 0000 0072 0f00 0000  .r....r....r....
+00000e00: 7f00 0000 7302 0000 0000 027a 1b50 6965  ....s......z.Pie
+00000e10: 4368 6172 7453 6563 7469 6f6e 2e74 6974  ChartSection.tit
+00000e20: 6c65 5f73 7479 6c65 6302 0000 0000 0000  le_stylec.......
+00000e30: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00000e40: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00000e50: 7234 0000 0072 3a00 0000 7233 0000 0072  r4...r:...r3...r
+00000e60: 1900 0000 7219 0000 0072 1a00 0000 720f  ....r....r....r.
+00000e70: 0000 0083 0000 0073 0200 0000 0002 6301  .......s......c.
+00000e80: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+00000e90: 0000 0043 0000 0073 1000 0000 7c00 6a00  ...C...s....|.j.
+00000ea0: 6401 6402 6403 6404 8d03 5300 2905 4eda  d.d.d.d...S.).N.
+00000eb0: 0d74 6974 6c65 506f 7369 7469 6f6e 722c  .titlePositionr,
+00000ec0: 0000 0067 0000 0000 0000 f03f 2902 722e  ...g.......?).r.
+00000ed0: 0000 00da 0964 6566 5f76 616c 7565 722f  .....def_valuer/
+00000ee0: 0000 0072 1b00 0000 7219 0000 0072 1900  ...r....r....r..
+00000ef0: 0000 721a 0000 0072 1000 0000 8800 0000  ..r....r........
+00000f00: 7302 0000 0000 027a 1e50 6965 4368 6172  s......z.PieChar
+00000f10: 7453 6563 7469 6f6e 2e74 6974 6c65 5f70  tSection.title_p
+00000f20: 6f73 6974 696f 6e63 0200 0000 0000 0000  ositionc........
+00000f30: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000f40: 7310 0000 007c 00a0 0064 017c 01a1 0201  s....|...d.|....
+00000f50: 0064 0053 0029 024e 723b 0000 0072 3100  .d.S.).Nr;...r1.
+00000f60: 0000 7233 0000 0072 1900 0000 7219 0000  ..r3...r....r...
+00000f70: 0072 1a00 0000 7210 0000 008c 0000 0073  .r....r........s
+00000f80: 0200 0000 0002 290d 4e4e 4e4e 4e4e 4e4e  ......).NNNNNNNN
+00000f90: 4e4e 4e4e 4e29 1cda 085f 5f6e 616d 655f  NNNNN)...__name_
+00000fa0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000fb0: 5f71 7561 6c6e 616d 655f 5f72 0600 0000  _qualname__r....
+00000fc0: 7203 0000 00da 0373 7472 7204 0000 0072  r......strr....r
+00000fd0: 0800 0000 7205 0000 0072 0700 0000 da04  ....r....r......
+00000fe0: 626f 6f6c 7202 0000 0072 1700 0000 721c  boolr....r....r.
+00000ff0: 0000 0072 1f00 0000 722a 0000 00da 0870  ...r....r*.....p
+00001000: 726f 7065 7274 7972 0a00 0000 da06 7365  ropertyr......se
+00001010: 7474 6572 720b 0000 0072 0d00 0000 720c  tterr....r....r.
+00001020: 0000 0072 1100 0000 7212 0000 0072 0e00  ...r....r....r..
+00001030: 0000 720f 0000 0072 1000 0000 da0d 5f5f  ..r....r......__
+00001040: 636c 6173 7363 656c 6c5f 5f72 1900 0000  classcell__r....
+00001050: 7219 0000 0072 2300 0000 721a 0000 0072  r....r#...r....r
+00001060: 0900 0000 0900 0000 7386 0000 0008 0300  ........s.......
+00001070: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+00001080: 0400 0100 0100 0100 ef02 0202 0102 0106  ................
+00001090: 0106 0106 0106 0102 0106 0102 0406 0106  ................
+000010a0: 0106 0102 ef0c 2608 030c 0508 0802 0110  ......&.........
+000010b0: 0304 0110 0402 0110 0304 0110 0402 0114  ................
+000010c0: 0304 0114 0402 0114 0304 0114 0402 0114  ................
+000010d0: 0304 0114 0402 0110 0304 0110 0402 010a  ................
+000010e0: 0304 0114 0402 010a 0304 0114 0402 0110  ................
+000010f0: 0304 0172 0900 0000 4e29 0dda 0674 7970  ...r....N)...typ
+00001100: 696e 6772 0200 0000 7203 0000 00da 1066  ingr....r......f
+00001110: 6c65 745f 636f 7265 2e62 6f72 6465 7272  let_core.borderr
+00001120: 0400 0000 da11 666c 6574 5f63 6f72 652e  ......flet_core.
+00001130: 636f 6e74 726f 6c72 0500 0000 7206 0000  controlr....r...
+00001140: 00da 0d66 6c65 745f 636f 7265 2e72 6566  ...flet_core.ref
+00001150: 7207 0000 00da 1466 6c65 745f 636f 7265  r......flet_core
+00001160: 2e74 6578 745f 7374 796c 6572 0800 0000  .text_styler....
+00001170: 7209 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00001180: 1900 0000 721a 0000 00da 083c 6d6f 6475  ....r......<modu
+00001190: 6c65 3e01 0000 0073 0a00 0000 1002 0c01  le>....s........
+000011a0: 1001 0c01 0c03                           ......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart_group.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart_rod.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_axis.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_axis_label.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/chart_point_shape.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/line_chart.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/line_chart_data.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/line_chart_data_point.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/pie_chart.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/charts/pie_chart_section.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/checkbox.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/chip.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/chip.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/circle_avatar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/client_storage.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/colors.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/column.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/connection.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/constrained_control.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/container.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/control.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_action_sheet.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_action_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_action_sheet_action.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_action_sheet_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_activity_indicator.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_activity_indicator.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_alert_dialog.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_app_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_bottom_sheet.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_checkbox.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_colors.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_colors.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_context_menu.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_context_menu.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_context_menu_action.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_context_menu_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_date_picker.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_date_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_dialog_action.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_dialog_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_filled_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_icons.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_icons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_list_tile.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_navigation_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_picker.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_radio.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_radio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_segmented_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_slider.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_sliding_segmented_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_sliding_segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_switch.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_switch.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_textfield.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_textfield.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/cupertino_timer_picker.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/cupertino_timer_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/datatable.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/date_picker.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/date_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/dismissible.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/dismissible.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/divider.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/drag_target.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/draggable.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/dropdown.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/elevated_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/embed_json_encoder.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/event_handler.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/expansion_panel.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/expansion_panel.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/expansion_tile.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/expansion_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/file_picker.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/filled_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/filled_tonal_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/flet_app.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/floating_action_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/form_field_control.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/gesture_detector.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/gradients.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/grid_view.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/haptic_feedback.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/icon.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/icon_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/icons.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/image.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/list_tile.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/list_view.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/local_connection.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/lottie.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/lottie.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/margin.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/markdown.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/matplotlib_chart.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/menu_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/menu_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/menu_item_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/menu_item_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/merge_semantics.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/merge_semantics.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/navigation_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/navigation_drawer.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/navigation_drawer.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/navigation_rail.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/outlined_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/padding.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/page.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/pagelet.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/pagelet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/painting.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/plotly_chart.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/popup_menu_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/progress_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/progress_ring.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/protocol.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 3393 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 410d 0000  a........:)fA...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 410d 0000  a........./fA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6500 a009 6504 6a0a a101  m.Z...e...e.j...
 00000070: 5a0b 4700 6405 6406 8400 6406 8302 5a0c  Z.G.d.d...d...Z.
@@ -42,242 +42,242 @@
 00000290: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
 000002a0: 1000 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
 000002b0: 6400 5300 a901 4e29 02da 155f 5075 6253  d.S...N)..._PubS
 000002c0: 7562 436c 6965 6e74 5f5f 7075 6273 7562  ubClient__pubsub
 000002d0: da19 5f50 7562 5375 6243 6c69 656e 745f  .._PubSubClient_
 000002e0: 5f73 6573 7369 6f6e 5f69 6429 03da 0473  _session_id)...s
 000002f0: 656c 6672 0700 0000 7208 0000 00a9 0072  elfr....r......r
-00000300: 0d00 0000 fa60 2f77 6f72 6b73 7061 6365  .....`/workspace
+00000300: 0d00 0000 fa67 2f77 6f72 6b73 7061 6365  .....g/workspace
 00000310: 732f 636f 6e74 7269 6266 6c65 742f 666c  s/contribflet/fl
-00000320: 6574 2f73 646b 2f70 7974 686f 6e2f 7061  et/sdk/python/pa
-00000330: 636b 6167 6573 2f66 6c65 742d 636f 7265  ckages/flet-core
-00000340: 2f73 7263 2f66 6c65 745f 636f 7265 2f70  /src/flet_core/p
-00000350: 7562 7375 622f 7075 6273 7562 5f63 6c69  ubsub/pubsub_cli
-00000360: 656e 742e 7079 da08 5f5f 696e 6974 5f5f  ent.py..__init__
-00000370: 0c00 0000 7304 0000 0000 0106 017a 1550  ....s........z.P
-00000380: 7562 5375 6243 6c69 656e 742e 5f5f 696e  ubSubClient.__in
-00000390: 6974 5f5f 2901 da07 6d65 7373 6167 6563  it__)...messagec
-000003a0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000003b0: 0300 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
-000003c0: 00a0 017c 01a1 0101 0064 0053 0072 0900  ...|.....d.S.r..
-000003d0: 0000 2902 720a 0000 00da 0873 656e 645f  ..).r......send_
-000003e0: 616c 6ca9 0272 0c00 0000 7210 0000 0072  all..r....r....r
-000003f0: 0d00 0000 720d 0000 0072 0e00 0000 7211  ....r....r....r.
-00000400: 0000 0010 0000 0073 0200 0000 0001 7a15  .......s......z.
-00000410: 5075 6253 7562 436c 6965 6e74 2e73 656e  PubSubClient.sen
-00000420: 645f 616c 6c7a 1e55 7365 2073 656e 645f  d_allz.Use send_
-00000430: 616c 6c28 2920 6d65 7468 6f64 2069 6e73  all() method ins
-00000440: 7465 6164 2e7a 0630 2e32 312e 307a 0331  tead.z.0.21.0z.1
-00000450: 2e30 2903 da06 7265 6173 6f6e da07 7665  .0)...reason..ve
-00000460: 7273 696f 6eda 0e64 656c 6574 655f 7665  rsion..delete_ve
-00000470: 7273 696f 6e63 0200 0000 0000 0000 0000  rsionc..........
-00000480: 0000 0200 0000 0300 0000 c300 0000 730e  ..............s.
-00000490: 0000 007c 00a0 007c 01a1 0101 0064 0053  ...|...|.....d.S
-000004a0: 0072 0900 0000 2901 7211 0000 0072 1200  .r....).r....r..
-000004b0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-000004c0: 00da 0e73 656e 645f 616c 6c5f 6173 796e  ...send_all_asyn
-000004d0: 6313 0000 0073 0200 0000 0006 7a1b 5075  c....s......z.Pu
-000004e0: 6253 7562 436c 6965 6e74 2e73 656e 645f  bSubClient.send_
-000004f0: 616c 6c5f 6173 796e 6329 02da 0574 6f70  all_async)...top
-00000500: 6963 7210 0000 0063 0300 0000 0000 0000  icr....c........
-00000510: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000520: 7312 0000 007c 006a 00a0 017c 017c 02a1  s....|.j...|.|..
-00000530: 0201 0064 0053 0072 0900 0000 2902 720a  ...d.S.r....).r.
-00000540: 0000 00da 1173 656e 645f 616c 6c5f 6f6e  .....send_all_on
-00000550: 5f74 6f70 6963 a903 720c 0000 0072 1700  _topic..r....r..
-00000560: 0000 7210 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000570: 0072 0e00 0000 7218 0000 001b 0000 0073  .r....r........s
-00000580: 0200 0000 0001 7a1e 5075 6253 7562 436c  ......z.PubSubCl
-00000590: 6965 6e74 2e73 656e 645f 616c 6c5f 6f6e  ient.send_all_on
-000005a0: 5f74 6f70 6963 7a27 5573 6520 7365 6e64  _topicz'Use send
-000005b0: 5f61 6c6c 5f6f 6e5f 746f 7069 6328 2920  _all_on_topic() 
-000005c0: 6d65 7468 6f64 2069 6e73 7465 6164 2e63  method instead.c
-000005d0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-000005e0: 0400 0000 c300 0000 7310 0000 007c 00a0  ........s....|..
-000005f0: 007c 017c 02a1 0201 0064 0053 0072 0900  .|.|.....d.S.r..
-00000600: 0000 2901 7218 0000 0072 1900 0000 720d  ..).r....r....r.
-00000610: 0000 0072 0d00 0000 720e 0000 00da 1773  ...r....r......s
-00000620: 656e 645f 616c 6c5f 6f6e 5f74 6f70 6963  end_all_on_topic
-00000630: 5f61 7379 6e63 1e00 0000 7302 0000 0000  _async....s.....
-00000640: 067a 2450 7562 5375 6243 6c69 656e 742e  .z$PubSubClient.
-00000650: 7365 6e64 5f61 6c6c 5f6f 6e5f 746f 7069  send_all_on_topi
-00000660: 635f 6173 796e 6363 0200 0000 0000 0000  c_asyncc........
-00000670: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000680: 7314 0000 007c 006a 00a0 017c 006a 027c  s....|.j...|.j.|
-00000690: 01a1 0201 0064 0053 0072 0900 0000 2903  .....d.S.r....).
-000006a0: 720a 0000 00da 0b73 656e 645f 6f74 6865  r......send_othe
-000006b0: 7273 720b 0000 0072 1200 0000 720d 0000  rsr....r....r...
-000006c0: 0072 0d00 0000 720e 0000 0072 1b00 0000  .r....r....r....
-000006d0: 2600 0000 7302 0000 0000 017a 1850 7562  &...s......z.Pub
-000006e0: 5375 6243 6c69 656e 742e 7365 6e64 5f6f  SubClient.send_o
-000006f0: 7468 6572 737a 2155 7365 2073 656e 645f  thersz!Use send_
-00000700: 6f74 6865 7273 2829 206d 6574 686f 6420  others() method 
-00000710: 696e 7374 6561 642e 6302 0000 0000 0000  instead.c.......
-00000720: 0000 0000 0002 0000 0003 0000 00c3 0000  ................
-00000730: 0073 0e00 0000 7c00 a000 7c01 a101 0100  .s....|...|.....
-00000740: 6400 5300 7209 0000 0029 0172 1b00 0000  d.S.r....).r....
-00000750: 7212 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000760: 0e00 0000 da11 7365 6e64 5f6f 7468 6572  ......send_other
-00000770: 735f 6173 796e 6329 0000 0073 0200 0000  s_async)...s....
-00000780: 0006 7a1e 5075 6253 7562 436c 6965 6e74  ..z.PubSubClient
-00000790: 2e73 656e 645f 6f74 6865 7273 5f61 7379  .send_others_asy
-000007a0: 6e63 6303 0000 0000 0000 0000 0000 0003  ncc.............
-000007b0: 0000 0005 0000 0043 0000 0073 1600 0000  .......C...s....
-000007c0: 7c00 6a00 a001 7c00 6a02 7c01 7c02 a103  |.j...|.j.|.|...
-000007d0: 0100 6400 5300 7209 0000 0029 0372 0a00  ..d.S.r....).r..
-000007e0: 0000 da14 7365 6e64 5f6f 7468 6572 735f  ....send_others_
-000007f0: 6f6e 5f74 6f70 6963 720b 0000 0072 1900  on_topicr....r..
-00000800: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000810: 0072 1d00 0000 3100 0000 7302 0000 0000  .r....1...s.....
-00000820: 017a 2150 7562 5375 6243 6c69 656e 742e  .z!PubSubClient.
-00000830: 7365 6e64 5f6f 7468 6572 735f 6f6e 5f74  send_others_on_t
-00000840: 6f70 6963 7a2a 5573 6520 7365 6e64 5f6f  opicz*Use send_o
-00000850: 7468 6572 735f 6f6e 5f74 6f70 6963 2829  thers_on_topic()
-00000860: 206d 6574 686f 6420 696e 7374 6561 642e   method instead.
-00000870: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000880: 0004 0000 00c3 0000 0073 1000 0000 7c00  .........s....|.
-00000890: a000 7c01 7c02 a102 0100 6400 5300 7209  ..|.|.....d.S.r.
-000008a0: 0000 0029 0172 1d00 0000 7219 0000 0072  ...).r....r....r
-000008b0: 0d00 0000 720d 0000 0072 0e00 0000 da1a  ....r....r......
-000008c0: 7365 6e64 5f6f 7468 6572 735f 6f6e 5f74  send_others_on_t
-000008d0: 6f70 6963 5f61 7379 6e63 3400 0000 7302  opic_async4...s.
-000008e0: 0000 0000 067a 2750 7562 5375 6243 6c69  .....z'PubSubCli
-000008f0: 656e 742e 7365 6e64 5f6f 7468 6572 735f  ent.send_others_
-00000900: 6f6e 5f74 6f70 6963 5f61 7379 6e63 2901  on_topic_async).
-00000910: da07 6861 6e64 6c65 7263 0200 0000 0000  ..handlerc......
-00000920: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000930: 0000 7314 0000 007c 006a 00a0 017c 006a  ..s....|.j...|.j
-00000940: 027c 01a1 0201 0064 0053 0072 0900 0000  .|.....d.S.r....
-00000950: 2903 720a 0000 00da 0973 7562 7363 7269  ).r......subscri
-00000960: 6265 720b 0000 00a9 0272 0c00 0000 721f  ber......r....r.
-00000970: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000980: 0000 7220 0000 003c 0000 0073 0200 0000  ..r ...<...s....
-00000990: 0001 7a16 5075 6253 7562 436c 6965 6e74  ..z.PubSubClient
-000009a0: 2e73 7562 7363 7269 6265 7a1f 5573 6520  .subscribez.Use 
-000009b0: 7375 6273 6372 6962 6528 2920 6d65 7468  subscribe() meth
-000009c0: 6f64 2069 6e73 7465 6164 2e63 0200 0000  od instead.c....
-000009d0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000009e0: c300 0000 730e 0000 007c 00a0 007c 01a1  ....s....|...|..
-000009f0: 0101 0064 0053 0072 0900 0000 2901 7220  ...d.S.r....).r 
-00000a00: 0000 0072 2100 0000 720d 0000 0072 0d00  ...r!...r....r..
-00000a10: 0000 720e 0000 00da 0f73 7562 7363 7269  ..r......subscri
-00000a20: 6265 5f61 7379 6e63 3f00 0000 7302 0000  be_async?...s...
-00000a30: 0000 067a 1c50 7562 5375 6243 6c69 656e  ...z.PubSubClien
-00000a40: 742e 7375 6273 6372 6962 655f 6173 796e  t.subscribe_asyn
-00000a50: 6329 0272 1700 0000 721f 0000 0063 0300  c).r....r....c..
-00000a60: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00000a70: 0000 4300 0000 7316 0000 007c 006a 00a0  ..C...s....|.j..
-00000a80: 017c 006a 027c 017c 02a1 0301 0064 0053  .|.j.|.|.....d.S
-00000a90: 0072 0900 0000 2903 720a 0000 00da 0f73  .r....).r......s
-00000aa0: 7562 7363 7269 6265 5f74 6f70 6963 720b  ubscribe_topicr.
-00000ab0: 0000 00a9 0372 0c00 0000 7217 0000 0072  .....r....r....r
-00000ac0: 1f00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000ad0: 0000 0072 2300 0000 4700 0000 7302 0000  ...r#...G...s...
-00000ae0: 0000 017a 1c50 7562 5375 6243 6c69 656e  ...z.PubSubClien
-00000af0: 742e 7375 6273 6372 6962 655f 746f 7069  t.subscribe_topi
-00000b00: 637a 2555 7365 2073 7562 7363 7269 6265  cz%Use subscribe
-00000b10: 5f74 6f70 6963 2829 206d 6574 686f 6420  _topic() method 
-00000b20: 696e 7374 6561 642e 6303 0000 0000 0000  instead.c.......
-00000b30: 0000 0000 0003 0000 0004 0000 00c3 0000  ................
-00000b40: 0073 1000 0000 7c00 a000 7c01 7c02 a102  .s....|...|.|...
-00000b50: 0100 6400 5300 7209 0000 0029 0172 2300  ..d.S.r....).r#.
-00000b60: 0000 7224 0000 0072 0d00 0000 720d 0000  ..r$...r....r...
-00000b70: 0072 0e00 0000 da15 7375 6273 6372 6962  .r......subscrib
-00000b80: 655f 746f 7069 635f 6173 796e 634a 0000  e_topic_asyncJ..
-00000b90: 0073 0200 0000 0006 7a22 5075 6253 7562  .s......z"PubSub
-00000ba0: 436c 6965 6e74 2e73 7562 7363 7269 6265  Client.subscribe
-00000bb0: 5f74 6f70 6963 5f61 7379 6e63 6301 0000  _topic_asyncc...
-00000bc0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000bd0: 0043 0000 0073 1200 0000 7c00 6a00 a001  .C...s....|.j...
-00000be0: 7c00 6a02 a101 0100 6400 5300 7209 0000  |.j.....d.S.r...
-00000bf0: 0029 0372 0a00 0000 da0b 756e 7375 6273  .).r......unsubs
-00000c00: 6372 6962 6572 0b00 0000 a901 720c 0000  criber......r...
-00000c10: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00000c20: 7226 0000 0052 0000 0073 0200 0000 0001  r&...R...s......
-00000c30: 7a18 5075 6253 7562 436c 6965 6e74 2e75  z.PubSubClient.u
-00000c40: 6e73 7562 7363 7269 6265 7a21 5573 6520  nsubscribez!Use 
-00000c50: 756e 7375 6273 6372 6962 6528 2920 6d65  unsubscribe() me
-00000c60: 7468 6f64 2069 6e73 7465 6164 2e63 0100  thod instead.c..
-00000c70: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000c80: 0000 c300 0000 730c 0000 007c 00a0 00a1  ......s....|....
-00000c90: 0001 0064 0053 0072 0900 0000 2901 7226  ...d.S.r....).r&
-00000ca0: 0000 0072 2700 0000 720d 0000 0072 0d00  ...r'...r....r..
-00000cb0: 0000 720e 0000 00da 1175 6e73 7562 7363  ..r......unsubsc
-00000cc0: 7269 6265 5f61 7379 6e63 5500 0000 7302  ribe_asyncU...s.
-00000cd0: 0000 0000 067a 1e50 7562 5375 6243 6c69  .....z.PubSubCli
-00000ce0: 656e 742e 756e 7375 6273 6372 6962 655f  ent.unsubscribe_
-00000cf0: 6173 796e 6329 0172 1700 0000 6302 0000  async).r....c...
-00000d00: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000d10: 0043 0000 0073 1400 0000 7c00 6a00 a001  .C...s....|.j...
-00000d20: 7c00 6a02 7c01 a102 0100 6400 5300 7209  |.j.|.....d.S.r.
-00000d30: 0000 0029 0372 0a00 0000 da11 756e 7375  ...).r......unsu
-00000d40: 6273 6372 6962 655f 746f 7069 6372 0b00  bscribe_topicr..
-00000d50: 0000 a902 720c 0000 0072 1700 0000 720d  ....r....r....r.
-00000d60: 0000 0072 0d00 0000 720e 0000 0072 2900  ...r....r....r).
-00000d70: 0000 5d00 0000 7302 0000 0000 017a 1e50  ..]...s......z.P
-00000d80: 7562 5375 6243 6c69 656e 742e 756e 7375  ubSubClient.unsu
-00000d90: 6273 6372 6962 655f 746f 7069 637a 2755  bscribe_topicz'U
-00000da0: 7365 2075 6e73 7562 7363 7269 6265 5f74  se unsubscribe_t
-00000db0: 6f70 6963 2829 206d 6574 686f 6420 696e  opic() method in
-00000dc0: 7374 6561 642e 6302 0000 0000 0000 0000  stead.c.........
-00000dd0: 0000 0002 0000 0003 0000 00c3 0000 0073  ...............s
-00000de0: 0e00 0000 7c00 a000 7c01 a101 0100 6400  ....|...|.....d.
-00000df0: 5300 7209 0000 0029 0172 2900 0000 722a  S.r....).r)...r*
-00000e00: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000e10: 0000 da17 756e 7375 6273 6372 6962 655f  ....unsubscribe_
-00000e20: 746f 7069 635f 6173 796e 6360 0000 0073  topic_async`...s
-00000e30: 0200 0000 0006 7a24 5075 6253 7562 436c  ......z$PubSubCl
-00000e40: 6965 6e74 2e75 6e73 7562 7363 7269 6265  ient.unsubscribe
-00000e50: 5f74 6f70 6963 5f61 7379 6e63 6301 0000  _topic_asyncc...
-00000e60: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000e70: 0043 0000 0073 1200 0000 7c00 6a00 a001  .C...s....|.j...
-00000e80: 7c00 6a02 a101 0100 6400 5300 7209 0000  |.j.....d.S.r...
-00000e90: 0029 0372 0a00 0000 da0f 756e 7375 6273  .).r......unsubs
-00000ea0: 6372 6962 655f 616c 6c72 0b00 0000 7227  cribe_allr....r'
-00000eb0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000ec0: 0000 722c 0000 0068 0000 0073 0200 0000  ..r,...h...s....
-00000ed0: 0001 7a1c 5075 6253 7562 436c 6965 6e74  ..z.PubSubClient
-00000ee0: 2e75 6e73 7562 7363 7269 6265 5f61 6c6c  .unsubscribe_all
-00000ef0: 7a25 5573 6520 756e 7375 6273 6372 6962  z%Use unsubscrib
-00000f00: 655f 616c 6c28 2920 6d65 7468 6f64 2069  e_all() method i
-00000f10: 6e73 7465 6164 2e63 0100 0000 0000 0000  nstead.c........
-00000f20: 0000 0000 0100 0000 0200 0000 c300 0000  ................
-00000f30: 730c 0000 007c 00a0 00a1 0001 0064 0053  s....|.......d.S
-00000f40: 0072 0900 0000 2901 722c 0000 0072 2700  .r....).r,...r'.
-00000f50: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-00000f60: 00da 1575 6e73 7562 7363 7269 6265 5f61  ...unsubscribe_a
-00000f70: 6c6c 5f61 7379 6e63 6b00 0000 7302 0000  ll_asynck...s...
-00000f80: 0000 067a 2250 7562 5375 6243 6c69 656e  ...z"PubSubClien
-00000f90: 742e 756e 7375 6273 6372 6962 655f 616c  t.unsubscribe_al
-00000fa0: 6c5f 6173 796e 634e 291b da08 5f5f 6e61  l_asyncN)...__na
-00000fb0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000fc0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7204  ..__qualname__r.
-00000fd0: 0000 00da 0373 7472 720f 0000 0072 0200  .....strr....r..
-00000fe0: 0000 7211 0000 0072 0500 0000 7216 0000  ..r....r....r...
-00000ff0: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001000: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00001010: 0300 0000 7220 0000 0072 2200 0000 7223  ....r ...r"...r#
-00001020: 0000 0072 2500 0000 7226 0000 0072 2800  ...r%...r&...r(.
-00001030: 0000 7229 0000 0072 2b00 0000 722c 0000  ..r)...r+...r,..
-00001040: 0072 2d00 0000 720d 0000 0072 0d00 0000  .r-...r....r....
-00001050: 720d 0000 0072 0e00 0000 7206 0000 000b  r....r....r.....
-00001060: 0000 0073 8000 0000 0801 1004 0e03 0201  ...s............
-00001070: 0201 0201 02fd 0405 1003 1003 0201 0201  ................
-00001080: 0201 02fd 0405 1203 0e03 0201 0201 0201  ................
-00001090: 02fd 0405 1003 1003 0201 0201 0201 02fd  ................
-000010a0: 0405 1203 0e03 0201 0201 0201 02fd 0405  ................
-000010b0: 1003 1003 0201 0201 0201 02fd 0405 1203  ................
-000010c0: 0803 0201 0201 0201 02fd 0405 0a03 0e03  ................
-000010d0: 0201 0201 0201 02fd 0405 1003 0803 0201  ................
-000010e0: 0201 0201 02fd 0405 7206 0000 0029 0dda  ........r....)..
-000010f0: 076c 6f67 6769 6e67 da06 7479 7069 6e67  .logging..typing
-00001100: 7202 0000 0072 0300 0000 da09 666c 6574  r....r......flet
-00001110: 5f63 6f72 65da 1b66 6c65 745f 636f 7265  _core..flet_core
-00001120: 2e70 7562 7375 622e 7075 6273 7562 5f68  .pubsub.pubsub_h
-00001130: 7562 7204 0000 00da 1a66 6c65 745f 636f  ubr......flet_co
-00001140: 7265 2e75 7469 6c73 2e64 6570 7265 6361  re.utils.depreca
-00001150: 7465 6472 0500 0000 da09 6765 744c 6f67  tedr......getLog
-00001160: 6765 7272 2e00 0000 da06 6c6f 6767 6572  gerr......logger
-00001170: 7206 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00001180: 0d00 0000 720e 0000 00da 083c 6d6f 6475  ....r......<modu
-00001190: 6c65 3e01 0000 0073 0c00 0000 0801 1002  le>....s........
-000011a0: 0801 0c01 0c02 0c03                      ........
+00000320: 6574 636f 6e74 7269 622f 7364 6b2f 7079  etcontrib/sdk/py
+00000330: 7468 6f6e 2f70 6163 6b61 6765 732f 666c  thon/packages/fl
+00000340: 6574 2d63 6f72 652f 7372 632f 666c 6574  et-core/src/flet
+00000350: 5f63 6f72 652f 7075 6273 7562 2f70 7562  _core/pubsub/pub
+00000360: 7375 625f 636c 6965 6e74 2e70 79da 085f  sub_client.py.._
+00000370: 5f69 6e69 745f 5f0c 0000 0073 0400 0000  _init__....s....
+00000380: 0001 0601 7a15 5075 6253 7562 436c 6965  ....z.PubSubClie
+00000390: 6e74 2e5f 5f69 6e69 745f 5f29 01da 076d  nt.__init__)...m
+000003a0: 6573 7361 6765 6302 0000 0000 0000 0000  essagec.........
+000003b0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000003c0: 1000 0000 7c00 6a00 a001 7c01 a101 0100  ....|.j...|.....
+000003d0: 6400 5300 7209 0000 0029 0272 0a00 0000  d.S.r....).r....
+000003e0: da08 7365 6e64 5f61 6c6c a902 720c 0000  ..send_all..r...
+000003f0: 0072 1000 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000400: 720e 0000 0072 1100 0000 1000 0000 7302  r....r........s.
+00000410: 0000 0000 017a 1550 7562 5375 6243 6c69  .....z.PubSubCli
+00000420: 656e 742e 7365 6e64 5f61 6c6c 7a1e 5573  ent.send_allz.Us
+00000430: 6520 7365 6e64 5f61 6c6c 2829 206d 6574  e send_all() met
+00000440: 686f 6420 696e 7374 6561 642e 7a06 302e  hod instead.z.0.
+00000450: 3231 2e30 7a03 312e 3029 03da 0672 6561  21.0z.1.0)...rea
+00000460: 736f 6eda 0776 6572 7369 6f6e da0e 6465  son..version..de
+00000470: 6c65 7465 5f76 6572 7369 6f6e 6302 0000  lete_versionc...
+00000480: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00000490: 00c3 0000 0073 0e00 0000 7c00 a000 7c01  .....s....|...|.
+000004a0: a101 0100 6400 5300 7209 0000 0029 0172  ....d.S.r....).r
+000004b0: 1100 0000 7212 0000 0072 0d00 0000 720d  ....r....r....r.
+000004c0: 0000 0072 0e00 0000 da0e 7365 6e64 5f61  ...r......send_a
+000004d0: 6c6c 5f61 7379 6e63 1300 0000 7302 0000  ll_async....s...
+000004e0: 0000 067a 1b50 7562 5375 6243 6c69 656e  ...z.PubSubClien
+000004f0: 742e 7365 6e64 5f61 6c6c 5f61 7379 6e63  t.send_all_async
+00000500: 2902 da05 746f 7069 6372 1000 0000 6303  )...topicr....c.
+00000510: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000520: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
+00000530: a001 7c01 7c02 a102 0100 6400 5300 7209  ..|.|.....d.S.r.
+00000540: 0000 0029 0272 0a00 0000 da11 7365 6e64  ...).r......send
+00000550: 5f61 6c6c 5f6f 6e5f 746f 7069 63a9 0372  _all_on_topic..r
+00000560: 0c00 0000 7217 0000 0072 1000 0000 720d  ....r....r....r.
+00000570: 0000 0072 0d00 0000 720e 0000 0072 1800  ...r....r....r..
+00000580: 0000 1b00 0000 7302 0000 0000 017a 1e50  ......s......z.P
+00000590: 7562 5375 6243 6c69 656e 742e 7365 6e64  ubSubClient.send
+000005a0: 5f61 6c6c 5f6f 6e5f 746f 7069 637a 2755  _all_on_topicz'U
+000005b0: 7365 2073 656e 645f 616c 6c5f 6f6e 5f74  se send_all_on_t
+000005c0: 6f70 6963 2829 206d 6574 686f 6420 696e  opic() method in
+000005d0: 7374 6561 642e 6303 0000 0000 0000 0000  stead.c.........
+000005e0: 0000 0003 0000 0004 0000 00c3 0000 0073  ...............s
+000005f0: 1000 0000 7c00 a000 7c01 7c02 a102 0100  ....|...|.|.....
+00000600: 6400 5300 7209 0000 0029 0172 1800 0000  d.S.r....).r....
+00000610: 7219 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000620: 0e00 0000 da17 7365 6e64 5f61 6c6c 5f6f  ......send_all_o
+00000630: 6e5f 746f 7069 635f 6173 796e 631e 0000  n_topic_async...
+00000640: 0073 0200 0000 0006 7a24 5075 6253 7562  .s......z$PubSub
+00000650: 436c 6965 6e74 2e73 656e 645f 616c 6c5f  Client.send_all_
+00000660: 6f6e 5f74 6f70 6963 5f61 7379 6e63 6302  on_topic_asyncc.
+00000670: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000680: 0000 0043 0000 0073 1400 0000 7c00 6a00  ...C...s....|.j.
+00000690: a001 7c00 6a02 7c01 a102 0100 6400 5300  ..|.j.|.....d.S.
+000006a0: 7209 0000 0029 0372 0a00 0000 da0b 7365  r....).r......se
+000006b0: 6e64 5f6f 7468 6572 7372 0b00 0000 7212  nd_othersr....r.
+000006c0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000006d0: 0000 721b 0000 0026 0000 0073 0200 0000  ..r....&...s....
+000006e0: 0001 7a18 5075 6253 7562 436c 6965 6e74  ..z.PubSubClient
+000006f0: 2e73 656e 645f 6f74 6865 7273 7a21 5573  .send_othersz!Us
+00000700: 6520 7365 6e64 5f6f 7468 6572 7328 2920  e send_others() 
+00000710: 6d65 7468 6f64 2069 6e73 7465 6164 2e63  method instead.c
+00000720: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000730: 0300 0000 c300 0000 730e 0000 007c 00a0  ........s....|..
+00000740: 007c 01a1 0101 0064 0053 0072 0900 0000  .|.....d.S.r....
+00000750: 2901 721b 0000 0072 1200 0000 720d 0000  ).r....r....r...
+00000760: 0072 0d00 0000 720e 0000 00da 1173 656e  .r....r......sen
+00000770: 645f 6f74 6865 7273 5f61 7379 6e63 2900  d_others_async).
+00000780: 0000 7302 0000 0000 067a 1e50 7562 5375  ..s......z.PubSu
+00000790: 6243 6c69 656e 742e 7365 6e64 5f6f 7468  bClient.send_oth
+000007a0: 6572 735f 6173 796e 6363 0300 0000 0000  ers_asyncc......
+000007b0: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
+000007c0: 0000 7316 0000 007c 006a 00a0 017c 006a  ..s....|.j...|.j
+000007d0: 027c 017c 02a1 0301 0064 0053 0072 0900  .|.|.....d.S.r..
+000007e0: 0000 2903 720a 0000 00da 1473 656e 645f  ..).r......send_
+000007f0: 6f74 6865 7273 5f6f 6e5f 746f 7069 6372  others_on_topicr
+00000800: 0b00 0000 7219 0000 0072 0d00 0000 720d  ....r....r....r.
+00000810: 0000 0072 0e00 0000 721d 0000 0031 0000  ...r....r....1..
+00000820: 0073 0200 0000 0001 7a21 5075 6253 7562  .s......z!PubSub
+00000830: 436c 6965 6e74 2e73 656e 645f 6f74 6865  Client.send_othe
+00000840: 7273 5f6f 6e5f 746f 7069 637a 2a55 7365  rs_on_topicz*Use
+00000850: 2073 656e 645f 6f74 6865 7273 5f6f 6e5f   send_others_on_
+00000860: 746f 7069 6328 2920 6d65 7468 6f64 2069  topic() method i
+00000870: 6e73 7465 6164 2e63 0300 0000 0000 0000  nstead.c........
+00000880: 0000 0000 0300 0000 0400 0000 c300 0000  ................
+00000890: 7310 0000 007c 00a0 007c 017c 02a1 0201  s....|...|.|....
+000008a0: 0064 0053 0072 0900 0000 2901 721d 0000  .d.S.r....).r...
+000008b0: 0072 1900 0000 720d 0000 0072 0d00 0000  .r....r....r....
+000008c0: 720e 0000 00da 1a73 656e 645f 6f74 6865  r......send_othe
+000008d0: 7273 5f6f 6e5f 746f 7069 635f 6173 796e  rs_on_topic_asyn
+000008e0: 6334 0000 0073 0200 0000 0006 7a27 5075  c4...s......z'Pu
+000008f0: 6253 7562 436c 6965 6e74 2e73 656e 645f  bSubClient.send_
+00000900: 6f74 6865 7273 5f6f 6e5f 746f 7069 635f  others_on_topic_
+00000910: 6173 796e 6329 01da 0768 616e 646c 6572  async)...handler
+00000920: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000930: 0004 0000 0043 0000 0073 1400 0000 7c00  .....C...s....|.
+00000940: 6a00 a001 7c00 6a02 7c01 a102 0100 6400  j...|.j.|.....d.
+00000950: 5300 7209 0000 0029 0372 0a00 0000 da09  S.r....).r......
+00000960: 7375 6273 6372 6962 6572 0b00 0000 a902  subscriber......
+00000970: 720c 0000 0072 1f00 0000 720d 0000 0072  r....r....r....r
+00000980: 0d00 0000 720e 0000 0072 2000 0000 3c00  ....r....r ...<.
+00000990: 0000 7302 0000 0000 017a 1650 7562 5375  ..s......z.PubSu
+000009a0: 6243 6c69 656e 742e 7375 6273 6372 6962  bClient.subscrib
+000009b0: 657a 1f55 7365 2073 7562 7363 7269 6265  ez.Use subscribe
+000009c0: 2829 206d 6574 686f 6420 696e 7374 6561  () method instea
+000009d0: 642e 6302 0000 0000 0000 0000 0000 0002  d.c.............
+000009e0: 0000 0003 0000 00c3 0000 0073 0e00 0000  ...........s....
+000009f0: 7c00 a000 7c01 a101 0100 6400 5300 7209  |...|.....d.S.r.
+00000a00: 0000 0029 0172 2000 0000 7221 0000 0072  ...).r ...r!...r
+00000a10: 0d00 0000 720d 0000 0072 0e00 0000 da0f  ....r....r......
+00000a20: 7375 6273 6372 6962 655f 6173 796e 633f  subscribe_async?
+00000a30: 0000 0073 0200 0000 0006 7a1c 5075 6253  ...s......z.PubS
+00000a40: 7562 436c 6965 6e74 2e73 7562 7363 7269  ubClient.subscri
+00000a50: 6265 5f61 7379 6e63 2902 7217 0000 0072  be_async).r....r
+00000a60: 1f00 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00000a70: 0003 0000 0005 0000 0043 0000 0073 1600  .........C...s..
+00000a80: 0000 7c00 6a00 a001 7c00 6a02 7c01 7c02  ..|.j...|.j.|.|.
+00000a90: a103 0100 6400 5300 7209 0000 0029 0372  ....d.S.r....).r
+00000aa0: 0a00 0000 da0f 7375 6273 6372 6962 655f  ......subscribe_
+00000ab0: 746f 7069 6372 0b00 0000 a903 720c 0000  topicr......r...
+00000ac0: 0072 1700 0000 721f 0000 0072 0d00 0000  .r....r....r....
+00000ad0: 720d 0000 0072 0e00 0000 7223 0000 0047  r....r....r#...G
+00000ae0: 0000 0073 0200 0000 0001 7a1c 5075 6253  ...s......z.PubS
+00000af0: 7562 436c 6965 6e74 2e73 7562 7363 7269  ubClient.subscri
+00000b00: 6265 5f74 6f70 6963 7a25 5573 6520 7375  be_topicz%Use su
+00000b10: 6273 6372 6962 655f 746f 7069 6328 2920  bscribe_topic() 
+00000b20: 6d65 7468 6f64 2069 6e73 7465 6164 2e63  method instead.c
+00000b30: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000b40: 0400 0000 c300 0000 7310 0000 007c 00a0  ........s....|..
+00000b50: 007c 017c 02a1 0201 0064 0053 0072 0900  .|.|.....d.S.r..
+00000b60: 0000 2901 7223 0000 0072 2400 0000 720d  ..).r#...r$...r.
+00000b70: 0000 0072 0d00 0000 720e 0000 00da 1573  ...r....r......s
+00000b80: 7562 7363 7269 6265 5f74 6f70 6963 5f61  ubscribe_topic_a
+00000b90: 7379 6e63 4a00 0000 7302 0000 0000 067a  syncJ...s......z
+00000ba0: 2250 7562 5375 6243 6c69 656e 742e 7375  "PubSubClient.su
+00000bb0: 6273 6372 6962 655f 746f 7069 635f 6173  bscribe_topic_as
+00000bc0: 796e 6363 0100 0000 0000 0000 0000 0000  yncc............
+00000bd0: 0100 0000 0300 0000 4300 0000 7312 0000  ........C...s...
+00000be0: 007c 006a 00a0 017c 006a 02a1 0101 0064  .|.j...|.j.....d
+00000bf0: 0053 0072 0900 0000 2903 720a 0000 00da  .S.r....).r.....
+00000c00: 0b75 6e73 7562 7363 7269 6265 720b 0000  .unsubscriber...
+00000c10: 00a9 0172 0c00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000c20: 0000 720e 0000 0072 2600 0000 5200 0000  ..r....r&...R...
+00000c30: 7302 0000 0000 017a 1850 7562 5375 6243  s......z.PubSubC
+00000c40: 6c69 656e 742e 756e 7375 6273 6372 6962  lient.unsubscrib
+00000c50: 657a 2155 7365 2075 6e73 7562 7363 7269  ez!Use unsubscri
+00000c60: 6265 2829 206d 6574 686f 6420 696e 7374  be() method inst
+00000c70: 6561 642e 6301 0000 0000 0000 0000 0000  ead.c...........
+00000c80: 0001 0000 0002 0000 00c3 0000 0073 0c00  .............s..
+00000c90: 0000 7c00 a000 a100 0100 6400 5300 7209  ..|.......d.S.r.
+00000ca0: 0000 0029 0172 2600 0000 7227 0000 0072  ...).r&...r'...r
+00000cb0: 0d00 0000 720d 0000 0072 0e00 0000 da11  ....r....r......
+00000cc0: 756e 7375 6273 6372 6962 655f 6173 796e  unsubscribe_asyn
+00000cd0: 6355 0000 0073 0200 0000 0006 7a1e 5075  cU...s......z.Pu
+00000ce0: 6253 7562 436c 6965 6e74 2e75 6e73 7562  bSubClient.unsub
+00000cf0: 7363 7269 6265 5f61 7379 6e63 2901 7217  scribe_async).r.
+00000d00: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000d10: 0200 0000 0400 0000 4300 0000 7314 0000  ........C...s...
+00000d20: 007c 006a 00a0 017c 006a 027c 01a1 0201  .|.j...|.j.|....
+00000d30: 0064 0053 0072 0900 0000 2903 720a 0000  .d.S.r....).r...
+00000d40: 00da 1175 6e73 7562 7363 7269 6265 5f74  ...unsubscribe_t
+00000d50: 6f70 6963 720b 0000 00a9 0272 0c00 0000  opicr......r....
+00000d60: 7217 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000d70: 0e00 0000 7229 0000 005d 0000 0073 0200  ....r)...]...s..
+00000d80: 0000 0001 7a1e 5075 6253 7562 436c 6965  ....z.PubSubClie
+00000d90: 6e74 2e75 6e73 7562 7363 7269 6265 5f74  nt.unsubscribe_t
+00000da0: 6f70 6963 7a27 5573 6520 756e 7375 6273  opicz'Use unsubs
+00000db0: 6372 6962 655f 746f 7069 6328 2920 6d65  cribe_topic() me
+00000dc0: 7468 6f64 2069 6e73 7465 6164 2e63 0200  thod instead.c..
+00000dd0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000de0: 0000 c300 0000 730e 0000 007c 00a0 007c  ......s....|...|
+00000df0: 01a1 0101 0064 0053 0072 0900 0000 2901  .....d.S.r....).
+00000e00: 7229 0000 0072 2a00 0000 720d 0000 0072  r)...r*...r....r
+00000e10: 0d00 0000 720e 0000 00da 1775 6e73 7562  ....r......unsub
+00000e20: 7363 7269 6265 5f74 6f70 6963 5f61 7379  scribe_topic_asy
+00000e30: 6e63 6000 0000 7302 0000 0000 067a 2450  nc`...s......z$P
+00000e40: 7562 5375 6243 6c69 656e 742e 756e 7375  ubSubClient.unsu
+00000e50: 6273 6372 6962 655f 746f 7069 635f 6173  bscribe_topic_as
+00000e60: 796e 6363 0100 0000 0000 0000 0000 0000  yncc............
+00000e70: 0100 0000 0300 0000 4300 0000 7312 0000  ........C...s...
+00000e80: 007c 006a 00a0 017c 006a 02a1 0101 0064  .|.j...|.j.....d
+00000e90: 0053 0072 0900 0000 2903 720a 0000 00da  .S.r....).r.....
+00000ea0: 0f75 6e73 7562 7363 7269 6265 5f61 6c6c  .unsubscribe_all
+00000eb0: 720b 0000 0072 2700 0000 720d 0000 0072  r....r'...r....r
+00000ec0: 0d00 0000 720e 0000 0072 2c00 0000 6800  ....r....r,...h.
+00000ed0: 0000 7302 0000 0000 017a 1c50 7562 5375  ..s......z.PubSu
+00000ee0: 6243 6c69 656e 742e 756e 7375 6273 6372  bClient.unsubscr
+00000ef0: 6962 655f 616c 6c7a 2555 7365 2075 6e73  ibe_allz%Use uns
+00000f00: 7562 7363 7269 6265 5f61 6c6c 2829 206d  ubscribe_all() m
+00000f10: 6574 686f 6420 696e 7374 6561 642e 6301  ethod instead.c.
+00000f20: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000f30: 0000 00c3 0000 0073 0c00 0000 7c00 a000  .......s....|...
+00000f40: a100 0100 6400 5300 7209 0000 0029 0172  ....d.S.r....).r
+00000f50: 2c00 0000 7227 0000 0072 0d00 0000 720d  ,...r'...r....r.
+00000f60: 0000 0072 0e00 0000 da15 756e 7375 6273  ...r......unsubs
+00000f70: 6372 6962 655f 616c 6c5f 6173 796e 636b  cribe_all_asynck
+00000f80: 0000 0073 0200 0000 0006 7a22 5075 6253  ...s......z"PubS
+00000f90: 7562 436c 6965 6e74 2e75 6e73 7562 7363  ubClient.unsubsc
+00000fa0: 7269 6265 5f61 6c6c 5f61 7379 6e63 4e29  ribe_all_asyncN)
+00000fb0: 1bda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000fc0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000fd0: 616d 655f 5f72 0400 0000 da03 7374 7272  ame__r......strr
+00000fe0: 0f00 0000 7202 0000 0072 1100 0000 7205  ....r....r....r.
+00000ff0: 0000 0072 1600 0000 7218 0000 0072 1a00  ...r....r....r..
+00001000: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00001010: 0072 1e00 0000 7203 0000 0072 2000 0000  .r....r....r ...
+00001020: 7222 0000 0072 2300 0000 7225 0000 0072  r"...r#...r%...r
+00001030: 2600 0000 7228 0000 0072 2900 0000 722b  &...r(...r)...r+
+00001040: 0000 0072 2c00 0000 722d 0000 0072 0d00  ...r,...r-...r..
+00001050: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00001060: 0072 0600 0000 0b00 0000 7380 0000 0008  .r........s.....
+00001070: 0110 040e 0302 0102 0102 0102 fd04 0510  ................
+00001080: 0310 0302 0102 0102 0102 fd04 0512 030e  ................
+00001090: 0302 0102 0102 0102 fd04 0510 0310 0302  ................
+000010a0: 0102 0102 0102 fd04 0512 030e 0302 0102  ................
+000010b0: 0102 0102 fd04 0510 0310 0302 0102 0102  ................
+000010c0: 0102 fd04 0512 0308 0302 0102 0102 0102  ................
+000010d0: fd04 050a 030e 0302 0102 0102 0102 fd04  ................
+000010e0: 0510 0308 0302 0102 0102 0102 fd04 0572  ...............r
+000010f0: 0600 0000 290d da07 6c6f 6767 696e 67da  ....)...logging.
+00001100: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
+00001110: 00da 0966 6c65 745f 636f 7265 da1b 666c  ...flet_core..fl
+00001120: 6574 5f63 6f72 652e 7075 6273 7562 2e70  et_core.pubsub.p
+00001130: 7562 7375 625f 6875 6272 0400 0000 da1a  ubsub_hubr......
+00001140: 666c 6574 5f63 6f72 652e 7574 696c 732e  flet_core.utils.
+00001150: 6465 7072 6563 6174 6564 7205 0000 00da  deprecatedr.....
+00001160: 0967 6574 4c6f 6767 6572 722e 0000 00da  .getLoggerr.....
+00001170: 066c 6f67 6765 7272 0600 0000 720d 0000  .loggerr....r...
+00001180: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00001190: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
+000011a0: 0000 0008 0110 0208 010c 010c 020c 03    ...............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 5873 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 f116 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 f116 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6400 6401 6c0d 5a0d 6400  m.Z...d.d.l.Z.d.
@@ -57,296 +57,296 @@
 00000380: 6f63 6bda 175f 5075 6253 7562 4875 625f  ock.._PubSubHub_
 00000390: 5f73 7562 7363 7269 6265 7273 da1d 5f50  _subscribers.._P
 000003a0: 7562 5375 6248 7562 5f5f 746f 7069 635f  ubSubHub__topic_
 000003b0: 7375 6273 6372 6962 6572 73da 1d5f 5075  subscribers.._Pu
 000003c0: 6253 7562 4875 625f 5f73 7562 7363 7269  bSubHub__subscri
 000003d0: 6265 725f 746f 7069 6373 2903 da04 7365  ber_topics)...se
 000003e0: 6c66 720d 0000 0072 0e00 0000 a900 721a  lfr....r......r.
-000003f0: 0000 00fa 5d2f 776f 726b 7370 6163 6573  ....]/workspaces
+000003f0: 0000 00fa 642f 776f 726b 7370 6163 6573  ....d/workspaces
 00000400: 2f63 6f6e 7472 6962 666c 6574 2f66 6c65  /contribflet/fle
-00000410: 742f 7364 6b2f 7079 7468 6f6e 2f70 6163  t/sdk/python/pac
-00000420: 6b61 6765 732f 666c 6574 2d63 6f72 652f  kages/flet-core/
-00000430: 7372 632f 666c 6574 5f63 6f72 652f 7075  src/flet_core/pu
-00000440: 6273 7562 2f70 7562 7375 625f 6875 622e  bsub/pubsub_hub.
-00000450: 7079 da08 5f5f 696e 6974 5f5f 0f00 0000  py..__init__....
-00000460: 7314 0000 0000 050a 0106 0106 0116 0302  s...............
-00000470: fe04 0502 fe04 0502 fe7a 1250 7562 5375  .........z.PubSu
-00000480: 6248 7562 2e5f 5f69 6e69 745f 5f29 01da  bHub.__init__)..
-00000490: 076d 6573 7361 6765 6302 0000 0000 0000  .messagec.......
-000004a0: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-000004b0: 0073 5a00 0000 7400 a001 6401 7c01 9b00  .sZ...t...d.|...
-000004c0: 6402 9d03 a101 0100 7c00 6a02 8f2e 0100  d.......|.j.....
-000004d0: 7c00 6a03 a004 a100 4400 5d12 7d02 7c00  |.j.....D.].}.|.
-000004e0: a005 7c02 7c01 6701 a102 0100 7124 5700  ..|.|.g.....q$W.
-000004f0: 6400 0400 0400 8303 0100 6e10 3100 734c  d.........n.1.sL
-00000500: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
-00000510: 2903 4e7a 1070 7562 7375 622e 7365 6e64  ).Nz.pubsub.send
-00000520: 5f61 6c6c 28fa 0129 2906 720f 0000 0072  _all(..)).r....r
-00000530: 1000 0000 7215 0000 0072 1600 0000 da06  ....r....r......
-00000540: 7661 6c75 6573 da10 5f50 7562 5375 6248  values.._PubSubH
-00000550: 7562 5f5f 7365 6e64 2903 7219 0000 0072  ub__send).r....r
-00000560: 1d00 0000 da07 6861 6e64 6c65 7272 1a00  ......handlerr..
-00000570: 0000 721a 0000 0072 1b00 0000 da08 7365  ..r....r......se
-00000580: 6e64 5f61 6c6c 2200 0000 7308 0000 0000  nd_all"...s.....
-00000590: 0112 0108 010e 017a 1250 7562 5375 6248  .......z.PubSubH
-000005a0: 7562 2e73 656e 645f 616c 6c29 02da 0574  ub.send_all)...t
-000005b0: 6f70 6963 721d 0000 0063 0300 0000 0000  opicr....c......
-000005c0: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-000005d0: 0000 7370 0000 0074 00a0 0164 017c 019b  ..sp...t...d.|..
-000005e0: 0064 027c 029b 0064 039d 05a1 0101 007c  .d.|...d.......|
-000005f0: 006a 028f 3e01 007c 017c 006a 0376 0072  .j..>..|.|.j.v.r
-00000600: 4e7c 006a 037c 0119 00a0 04a1 0044 005d  N|.j.|.......D.]
-00000610: 147d 037c 00a0 057c 037c 017c 0267 02a1  .}.|...|.|.|.g..
-00000620: 0201 0071 3857 0064 0004 0004 0083 0301  ...q8W.d........
-00000630: 006e 1031 0073 6230 0001 0001 0001 0059  .n.1.sb0.......Y
-00000640: 0001 0064 0053 0029 044e 7a19 7075 6273  ...d.S.).Nz.pubs
-00000650: 7562 2e73 656e 645f 616c 6c5f 6f6e 5f74  ub.send_all_on_t
-00000660: 6f70 6963 28fa 022c 2072 1e00 0000 2906  opic(.., r....).
-00000670: 720f 0000 0072 1000 0000 7215 0000 0072  r....r....r....r
-00000680: 1700 0000 721f 0000 0072 2000 0000 2904  ....r....r ...).
-00000690: 7219 0000 0072 2300 0000 721d 0000 0072  r....r#...r....r
-000006a0: 2100 0000 721a 0000 0072 1a00 0000 721b  !...r....r....r.
-000006b0: 0000 00da 1173 656e 645f 616c 6c5f 6f6e  .....send_all_on
-000006c0: 5f74 6f70 6963 2800 0000 730a 0000 0000  _topic(...s.....
-000006d0: 0118 0108 010a 0112 017a 1b50 7562 5375  .........z.PubSu
-000006e0: 6248 7562 2e73 656e 645f 616c 6c5f 6f6e  bHub.send_all_on
-000006f0: 5f74 6f70 6963 2902 da11 6578 6365 7074  _topic)...except
-00000700: 5f73 6573 7369 6f6e 5f69 6472 1d00 0000  _session_idr....
-00000710: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
-00000720: 0008 0000 0043 0000 0073 6c00 0000 7400  .....C...sl...t.
-00000730: a001 6401 7c01 9b00 6402 7c02 9b00 6403  ..d.|...d.|...d.
-00000740: 9d05 a101 0100 7c00 6a02 8f3a 0100 7c00  ......|.j..:..|.
-00000750: 6a03 a004 a100 4400 5d1e 5c02 7d03 7d04  j.....D.].\.}.}.
-00000760: 7c01 7c03 6b03 722a 7c00 a005 7c04 7c02  |.|.k.r*|...|.|.
-00000770: 6701 a102 0100 712a 5700 6400 0400 0400  g.....q*W.d.....
-00000780: 8303 0100 6e10 3100 735e 3000 0100 0100  ....n.1.s^0.....
-00000790: 0100 5900 0100 6400 5300 2904 4e7a 1370  ..Y...d.S.).Nz.p
-000007a0: 7562 7375 622e 7365 6e64 5f6f 7468 6572  ubsub.send_other
-000007b0: 7328 7224 0000 0072 1e00 0000 2906 720f  s(r$...r....).r.
-000007c0: 0000 0072 1000 0000 7215 0000 0072 1600  ...r....r....r..
-000007d0: 0000 da05 6974 656d 7372 2000 0000 2905  ....itemsr ...).
-000007e0: 7219 0000 0072 2600 0000 721d 0000 00da  r....r&...r.....
-000007f0: 0a73 6573 7369 6f6e 5f69 6472 2100 0000  .session_idr!...
-00000800: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00000810: 0b73 656e 645f 6f74 6865 7273 2f00 0000  .send_others/...
-00000820: 730a 0000 0000 0118 0108 0112 0108 017a  s..............z
-00000830: 1550 7562 5375 6248 7562 2e73 656e 645f  .PubSubHub.send_
-00000840: 6f74 6865 7273 2903 7226 0000 0072 2300  others).r&...r#.
-00000850: 0000 721d 0000 0063 0400 0000 0000 0000  ..r....c........
-00000860: 0000 0000 0600 0000 0900 0000 4300 0000  ............C...
-00000870: 7382 0000 0074 00a0 0164 017c 019b 0064  s....t...d.|...d
-00000880: 027c 029b 0064 027c 039b 0064 039d 07a1  .|...d.|...d....
-00000890: 0101 007c 006a 028f 4a01 007c 027c 006a  ...|.j..J..|.|.j
-000008a0: 0376 0072 607c 006a 037c 0219 00a0 04a1  .v.r`|.j.|......
-000008b0: 0044 005d 205c 027d 047d 057c 017c 046b  .D.] \.}.}.|.|.k
-000008c0: 0372 3e7c 00a0 057c 057c 027c 0367 02a1  .r>|...|.|.|.g..
-000008d0: 0201 0071 3e57 0064 0004 0004 0083 0301  ...q>W.d........
-000008e0: 006e 1031 0073 7430 0001 0001 0001 0059  .n.1.st0.......Y
-000008f0: 0001 0064 0053 0029 044e 7a1c 7075 6273  ...d.S.).Nz.pubs
-00000900: 7562 2e73 656e 645f 6f74 6865 7273 5f6f  ub.send_others_o
-00000910: 6e5f 746f 7069 6328 7224 0000 0072 1e00  n_topic(r$...r..
-00000920: 0000 2906 720f 0000 0072 1000 0000 7215  ..).r....r....r.
-00000930: 0000 0072 1700 0000 7227 0000 0072 2000  ...r....r'...r .
-00000940: 0000 2906 7219 0000 0072 2600 0000 7223  ..).r....r&...r#
-00000950: 0000 0072 1d00 0000 7228 0000 0072 2100  ...r....r(...r!.
-00000960: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000970: 00da 1473 656e 645f 6f74 6865 7273 5f6f  ...send_others_o
-00000980: 6e5f 746f 7069 6336 0000 0073 1000 0000  n_topic6...s....
-00000990: 0001 0401 16ff 0403 0801 0a01 1601 0801  ................
-000009a0: 7a1e 5075 6253 7562 4875 622e 7365 6e64  z.PubSubHub.send
-000009b0: 5f6f 7468 6572 735f 6f6e 5f74 6f70 6963  _others_on_topic
-000009c0: 2902 7228 0000 0072 2100 0000 6303 0000  ).r(...r!...c...
-000009d0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-000009e0: 0043 0000 0073 4600 0000 7400 a001 6401  .C...sF...t...d.
-000009f0: 7c01 9b00 6402 9d03 a101 0100 7c00 6a02  |...d.......|.j.
-00000a00: 8f1a 0100 7c02 7c00 6a03 7c01 3c00 5700  ....|.|.j.|.<.W.
-00000a10: 6400 0400 0400 8303 0100 6e10 3100 7338  d.........n.1.s8
-00000a20: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
-00000a30: 2903 4e7a 1170 7562 7375 622e 7375 6273  ).Nz.pubsub.subs
-00000a40: 6372 6962 6528 721e 0000 0029 0472 0f00  cribe(r....).r..
-00000a50: 0000 7210 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000a60: 0029 0372 1900 0000 7228 0000 0072 2100  .).r....r(...r!.
-00000a70: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000a80: 00da 0973 7562 7363 7269 6265 4000 0000  ...subscribe@...
-00000a90: 7306 0000 0000 0112 0108 017a 1350 7562  s..........z.Pub
-00000aa0: 5375 6248 7562 2e73 7562 7363 7269 6265  SubHub.subscribe
-00000ab0: 2e29 0372 2800 0000 7223 0000 0072 2100  .).r(...r#...r!.
-00000ac0: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
-00000ad0: 0000 0008 0000 0043 0000 0073 5000 0000  .......C...sP...
-00000ae0: 7400 a001 6401 7c01 9b00 6402 7c02 9b00  t...d.|...d.|...
-00000af0: 6403 9d05 a101 0100 7c00 6a02 8f1e 0100  d.......|.j.....
-00000b00: 7c00 a003 7c01 7c02 7c03 a103 0100 5700  |...|.|.|.....W.
-00000b10: 6400 0400 0400 8303 0100 6e10 3100 7342  d.........n.1.sB
-00000b20: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
-00000b30: 2904 4e7a 1770 7562 7375 622e 7375 6273  ).Nz.pubsub.subs
-00000b40: 6372 6962 655f 746f 7069 6328 7224 0000  cribe_topic(r$..
-00000b50: 0072 1e00 0000 2904 720f 0000 0072 1000  .r....).r....r..
-00000b60: 0000 7215 0000 00da 1b5f 5075 6253 7562  ..r......_PubSub
-00000b70: 4875 625f 5f73 7562 7363 7269 6265 5f74  Hub__subscribe_t
-00000b80: 6f70 6963 2904 7219 0000 0072 2800 0000  opic).r....r(...
-00000b90: 7223 0000 0072 2100 0000 721a 0000 0072  r#...r!...r....r
-00000ba0: 1a00 0000 721b 0000 00da 0f73 7562 7363  ....r......subsc
-00000bb0: 7269 6265 5f74 6f70 6963 4500 0000 7306  ribe_topicE...s.
-00000bc0: 0000 0000 0618 0108 017a 1950 7562 5375  .........z.PubSu
-00000bd0: 6248 7562 2e73 7562 7363 7269 6265 5f74  bHub.subscribe_t
-00000be0: 6f70 6963 6304 0000 0000 0000 0000 0000  opicc...........
-00000bf0: 0006 0000 0003 0000 0043 0000 0073 5800  .........C...sX.
-00000c00: 0000 7c00 6a00 a001 7c02 a101 7d04 7c04  ..|.j...|...}.|.
-00000c10: 6400 7500 7222 6900 7d04 7c04 7c00 6a00  d.u.r"i.}.|.|.j.
-00000c20: 7c02 3c00 7c03 7c04 7c01 3c00 7c00 6a02  |.<.|.|.|.<.|.j.
-00000c30: a001 7c01 a101 7d05 7c05 6400 7500 724c  ..|...}.|.d.u.rL
-00000c40: 6900 7d05 7c05 7c00 6a02 7c01 3c00 7c03  i.}.|.|.j.|.<.|.
-00000c50: 7c05 7c02 3c00 6400 5300 2901 4e29 0372  |.|.<.d.S.).N).r
-00000c60: 1700 0000 da03 6765 7472 1800 0000 2906  ......getr....).
-00000c70: 7219 0000 0072 2800 0000 7223 0000 0072  r....r(...r#...r
-00000c80: 2100 0000 da11 746f 7069 635f 7375 6273  !.....topic_subs
-00000c90: 6372 6962 6572 73da 1173 7562 7363 7269  cribers..subscri
-00000ca0: 6265 725f 746f 7069 6373 721a 0000 0072  ber_topicsr....r
-00000cb0: 1a00 0000 721b 0000 005a 115f 5f73 7562  ....r....Z.__sub
-00000cc0: 7363 7269 6265 5f74 6f70 6963 4f00 0000  scribe_topicO...
-00000cd0: 7314 0000 0000 060c 0108 0104 010a 0108  s...............
-00000ce0: 010c 0108 0104 010a 017a 1b50 7562 5375  .........z.PubSu
-00000cf0: 6248 7562 2e5f 5f73 7562 7363 7269 6265  bHub.__subscribe
-00000d00: 5f74 6f70 6963 2901 7228 0000 0063 0200  _topic).r(...c..
-00000d10: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-00000d20: 0000 4300 0000 7346 0000 0074 00a0 0164  ..C...sF...t...d
-00000d30: 017c 019b 0064 029d 03a1 0101 007c 006a  .|...d.......|.j
-00000d40: 028f 1a01 007c 00a0 037c 01a1 0101 0057  .....|...|.....W
-00000d50: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-00000d60: 3830 0001 0001 0001 0059 0001 0064 0053  80.......Y...d.S
-00000d70: 0029 034e fa13 7075 6273 7562 2e75 6e73  .).N..pubsub.uns
-00000d80: 7562 7363 7269 6265 2872 1e00 0000 2904  ubscribe(r....).
-00000d90: 720f 0000 0072 1000 0000 7215 0000 00da  r....r....r.....
-00000da0: 175f 5075 6253 7562 4875 625f 5f75 6e73  ._PubSubHub__uns
-00000db0: 7562 7363 7269 6265 a902 7219 0000 0072  ubscribe..r....r
-00000dc0: 2800 0000 721a 0000 0072 1a00 0000 721b  (...r....r....r.
-00000dd0: 0000 00da 0b75 6e73 7562 7363 7269 6265  .....unsubscribe
-00000de0: 6000 0000 7306 0000 0000 0112 0108 017a  `...s..........z
-00000df0: 1550 7562 5375 6248 7562 2e75 6e73 7562  .PubSubHub.unsub
-00000e00: 7363 7269 6265 2902 7228 0000 0072 2300  scribe).r(...r#.
-00000e10: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00000e20: 0000 0008 0000 0043 0000 0073 4e00 0000  .......C...sN...
-00000e30: 7400 a001 6401 7c01 9b00 6402 7c02 9b00  t...d.|...d.|...
-00000e40: 6403 9d05 a101 0100 7c00 6a02 8f1c 0100  d.......|.j.....
-00000e50: 7c00 a003 7c01 7c02 a102 0100 5700 6400  |...|.|.....W.d.
-00000e60: 0400 0400 8303 0100 6e10 3100 7340 3000  ........n.1.s@0.
-00000e70: 0100 0100 0100 5900 0100 6400 5300 2904  ......Y...d.S.).
-00000e80: 4e72 3100 0000 7224 0000 0072 1e00 0000  Nr1...r$...r....
-00000e90: 2904 720f 0000 0072 1000 0000 7215 0000  ).r....r....r...
-00000ea0: 00da 1d5f 5075 6253 7562 4875 625f 5f75  ..._PubSubHub__u
-00000eb0: 6e73 7562 7363 7269 6265 5f74 6f70 6963  nsubscribe_topic
-00000ec0: a903 7219 0000 0072 2800 0000 7223 0000  ..r....r(...r#..
-00000ed0: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000ee0: da11 756e 7375 6273 6372 6962 655f 746f  ..unsubscribe_to
-00000ef0: 7069 6365 0000 0073 0600 0000 0001 1801  pice...s........
-00000f00: 0801 7a1b 5075 6253 7562 4875 622e 756e  ..z.PubSubHub.un
-00000f10: 7375 6273 6372 6962 655f 746f 7069 6363  subscribe_topicc
-00000f20: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000f30: 0800 0000 4300 0000 7370 0000 0074 00a0  ....C...sp...t..
-00000f40: 0164 017c 019b 0064 029d 03a1 0101 007c  .d.|...d.......|
-00000f50: 006a 028f 4401 007c 00a0 037c 01a1 0101  .j..D..|...|....
-00000f60: 007c 017c 006a 0476 0072 4e7c 006a 047c  .|.|.j.v.rN|.j.|
-00000f70: 0119 00a0 05a1 0044 005d 107d 027c 00a0  .......D.].}.|..
-00000f80: 067c 017c 02a1 0201 0071 3c57 0064 0004  .|.|.....q<W.d..
-00000f90: 0004 0083 0301 006e 1031 0073 6230 0001  .......n.1.sb0..
-00000fa0: 0001 0001 0059 0001 0064 0053 0029 034e  .....Y...d.S.).N
-00000fb0: 7a17 7075 6273 7562 2e75 6e73 7562 7363  z.pubsub.unsubsc
-00000fc0: 7269 6265 5f61 6c6c 2872 1e00 0000 2907  ribe_all(r....).
-00000fd0: 720f 0000 0072 1000 0000 7215 0000 0072  r....r....r....r
-00000fe0: 3200 0000 7218 0000 00da 046b 6579 7372  2...r......keysr
-00000ff0: 3500 0000 7236 0000 0072 1a00 0000 721a  5...r6...r....r.
-00001000: 0000 0072 1b00 0000 da0f 756e 7375 6273  ...r......unsubs
-00001010: 6372 6962 655f 616c 6c6a 0000 0073 0c00  cribe_allj...s..
-00001020: 0000 0001 1201 0801 0a01 0a01 1201 7a19  ..............z.
-00001030: 5075 6253 7562 4875 622e 756e 7375 6273  PubSubHub.unsubs
-00001040: 6372 6962 655f 616c 6c63 0200 0000 0000  cribe_allc......
-00001050: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-00001060: 0000 7324 0000 0074 00a0 0164 017c 019b  ..s$...t...d.|..
-00001070: 0064 029d 03a1 0101 007c 006a 02a0 037c  .d.......|.j...|
-00001080: 0164 00a1 0201 0064 0053 0029 034e 7a15  .d.....d.S.).Nz.
-00001090: 7075 6273 7562 2e5f 5f75 6e73 7562 7363  pubsub.__unsubsc
-000010a0: 7269 6265 2872 1e00 0000 2904 720f 0000  ribe(r....).r...
-000010b0: 0072 1000 0000 7216 0000 00da 0370 6f70  .r....r......pop
-000010c0: 7233 0000 0072 1a00 0000 721a 0000 0072  r3...r....r....r
-000010d0: 1b00 0000 5a0d 5f5f 756e 7375 6273 6372  ....Z.__unsubscr
-000010e0: 6962 6572 0000 0073 0400 0000 0001 1201  iber...s........
-000010f0: 7a17 5075 6253 7562 4875 622e 5f5f 756e  z.PubSubHub.__un
-00001100: 7375 6273 6372 6962 6563 0300 0000 0000  subscribec......
-00001110: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
-00001120: 0000 7390 0000 0074 00a0 0164 017c 019b  ..s....t...d.|..
-00001130: 0064 027c 029b 0064 039d 05a1 0101 007c  .d.|...d.......|
-00001140: 006a 02a0 037c 02a1 017d 037c 0364 0075  .j...|...}.|.d.u
-00001150: 0172 527c 03a0 047c 0164 00a1 0201 0074  .rR|...|.d.....t
-00001160: 057c 0383 0164 046b 0272 527c 006a 02a0  .|...d.k.rR|.j..
-00001170: 047c 0264 00a1 0201 007c 006a 06a0 037c  .|.d.....|.j...|
-00001180: 01a1 017d 047c 0464 0075 0172 8c7c 04a0  ...}.|.d.u.r.|..
-00001190: 047c 0264 00a1 0201 0074 057c 0483 0164  .|.d.....t.|...d
-000011a0: 046b 0272 8c7c 006a 06a0 047c 0164 00a1  .k.r.|.j...|.d..
-000011b0: 0201 0064 0053 0029 054e 7a1b 7075 6273  ...d.S.).Nz.pubs
-000011c0: 7562 2e5f 5f75 6e73 7562 7363 7269 6265  ub.__unsubscribe
-000011d0: 5f74 6f70 6963 2872 2400 0000 721e 0000  _topic(r$...r...
-000011e0: 0072 0100 0000 2907 720f 0000 0072 1000  .r....).r....r..
-000011f0: 0000 7217 0000 0072 2e00 0000 723a 0000  ..r....r....r:..
-00001200: 00da 036c 656e 7218 0000 0029 0572 1900  ...lenr....).r..
-00001210: 0000 7228 0000 0072 2300 0000 722f 0000  ..r(...r#...r/..
-00001220: 0072 3000 0000 721a 0000 0072 1a00 0000  .r0...r....r....
-00001230: 721b 0000 005a 135f 5f75 6e73 7562 7363  r....Z.__unsubsc
-00001240: 7269 6265 5f74 6f70 6963 7600 0000 7316  ribe_topicv...s.
-00001250: 0000 0000 0118 010c 0108 010c 010c 010e  ................
-00001260: 010c 0108 010c 010c 017a 1d50 7562 5375  .........z.PubSu
-00001270: 6248 7562 2e5f 5f75 6e73 7562 7363 7269  bHub.__unsubscri
-00001280: 6265 5f74 6f70 6963 2902 7221 0000 00da  be_topic).r!....
-00001290: 0461 7267 7363 0300 0000 0000 0000 0000  .argsc..........
-000012a0: 0000 0300 0000 0400 0000 4300 0000 735e  ..........C...s^
-000012b0: 0000 007c 006a 0073 0e4a 0064 0183 0182  ...|.j.s.J.d....
-000012c0: 0174 01a0 027c 01a1 0172 2c74 01a0 037c  .t...|...r,t...|
-000012d0: 017c 028e 007c 006a 00a1 0201 006e 2e7c  .|...|.j.....n.|
-000012e0: 006a 0472 527c 006a 006a 057c 006a 006a  .j.rR|.j.j.|.j.j
-000012f0: 067c 006a 047c 0167 037c 02a2 0152 008e  .|.j.|.g.|...R..
-00001300: 0001 006e 087c 017c 028e 0001 0064 0053  ...n.|.|.....d.S
-00001310: 0029 024e 7a1c 5075 6253 7562 2065 7665  .).Nz.PubSub eve
-00001320: 6e74 206c 6f6f 7020 6973 206e 6f74 2073  nt loop is not s
-00001330: 6574 2907 7211 0000 00da 0761 7379 6e63  et).r......async
-00001340: 696f da13 6973 636f 726f 7574 696e 6566  io..iscoroutinef
-00001350: 756e 6374 696f 6eda 1872 756e 5f63 6f72  unction..run_cor
-00001360: 6f75 7469 6e65 5f74 6872 6561 6473 6166  outine_threadsaf
-00001370: 6572 1200 0000 da14 6361 6c6c 5f73 6f6f  er......call_soo
-00001380: 6e5f 7468 7265 6164 7361 6665 da0f 7275  n_threadsafe..ru
-00001390: 6e5f 696e 5f65 7865 6375 746f 7229 0372  n_in_executor).r
-000013a0: 1900 0000 7221 0000 0072 3c00 0000 721a  ....r!...r<...r.
-000013b0: 0000 0072 1a00 0000 721b 0000 005a 065f  ...r....r....Z._
-000013c0: 5f73 656e 6483 0000 0073 1400 0000 0003  _send....s......
-000013d0: 0e02 0a01 1402 0601 0601 0cff 0201 02ff  ................
-000013e0: 0a04 7a10 5075 6253 7562 4875 622e 5f5f  ..z.PubSubHub.__
-000013f0: 7365 6e64 2902 4e4e 291b da08 5f5f 6e61  send).NN)...__na
-00001400: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00001410: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7208  ..__qualname__r.
-00001420: 0000 0072 3d00 0000 da11 4162 7374 7261  ...r=.....Abstra
-00001430: 6374 4576 656e 744c 6f6f 7072 0200 0000  ctEventLoopr....
-00001440: 721c 0000 0072 0300 0000 7222 0000 00da  r....r....r"....
-00001450: 0373 7472 7225 0000 0072 2900 0000 722a  .strr%...r)...r*
-00001460: 0000 0072 0500 0000 722b 0000 0072 0900  ...r....r+...r..
-00001470: 0000 7204 0000 0072 2d00 0000 722c 0000  ..r....r-...r,..
-00001480: 0072 3400 0000 7237 0000 0072 3900 0000  .r4...r7...r9...
-00001490: 7232 0000 0072 3500 0000 7207 0000 0072  r2...r5...r....r
-000014a0: 2000 0000 721a 0000 0072 1a00 0000 721a   ...r....r....r.
-000014b0: 0000 0072 1b00 0000 720c 0000 000e 0000  ...r....r.......
-000014c0: 0073 3400 0000 0803 0001 00fd 0202 0801  .s4.............
-000014d0: 06fd 0c13 0e06 1007 1007 120a 1007 0201  ................
-000014e0: 0201 16fc 0c0c 0201 0201 16fc 0c11 0e05  ................
-000014f0: 1005 0e08 0e04 100e 18ff 720c 0000 0029  ..........r....)
-00001500: 1672 3d00 0000 da07 6c6f 6767 696e 6772  .r=.....loggingr
-00001510: 1300 0000 da12 636f 6e63 7572 7265 6e74  ......concurrent
-00001520: 2e66 7574 7572 6573 7202 0000 00da 0674  .futuresr......t
-00001530: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
-00001540: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
-00001550: 0000 0072 0900 0000 da09 666c 6574 5f63  ...r......flet_c
-00001560: 6f72 65da 0f66 6c65 745f 636f 7265 2e6c  ore..flet_core.l
-00001570: 6f63 6b73 720a 0000 00da 2166 6c65 745f  ocksr.....!flet_
-00001580: 636f 7265 2e75 7469 6c73 2e63 6f6e 6375  core.utils.concu
-00001590: 7272 656e 6379 5f75 7469 6c73 720b 0000  rrency_utilsr...
-000015a0: 00da 0967 6574 4c6f 6767 6572 7242 0000  ...getLoggerrB..
-000015b0: 0072 0f00 0000 720c 0000 0072 1a00 0000  .r....r....r....
-000015c0: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-000015d0: 083c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
-000015e0: 0000 0801 0801 0801 0c01 2402 0801 0c01  ..........$.....
-000015f0: 0c02 0c03                                ....
+00000410: 7463 6f6e 7472 6962 2f73 646b 2f70 7974  tcontrib/sdk/pyt
+00000420: 686f 6e2f 7061 636b 6167 6573 2f66 6c65  hon/packages/fle
+00000430: 742d 636f 7265 2f73 7263 2f66 6c65 745f  t-core/src/flet_
+00000440: 636f 7265 2f70 7562 7375 622f 7075 6273  core/pubsub/pubs
+00000450: 7562 5f68 7562 2e70 79da 085f 5f69 6e69  ub_hub.py..__ini
+00000460: 745f 5f0f 0000 0073 1400 0000 0005 0a01  t__....s........
+00000470: 0601 0601 1603 02fe 0405 02fe 0405 02fe  ................
+00000480: 7a12 5075 6253 7562 4875 622e 5f5f 696e  z.PubSubHub.__in
+00000490: 6974 5f5f 2901 da07 6d65 7373 6167 6563  it__)...messagec
+000004a0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+000004b0: 0800 0000 4300 0000 735a 0000 0074 00a0  ....C...sZ...t..
+000004c0: 0164 017c 019b 0064 029d 03a1 0101 007c  .d.|...d.......|
+000004d0: 006a 028f 2e01 007c 006a 03a0 04a1 0044  .j.....|.j.....D
+000004e0: 005d 127d 027c 00a0 057c 027c 0167 01a1  .].}.|...|.|.g..
+000004f0: 0201 0071 2457 0064 0004 0004 0083 0301  ...q$W.d........
+00000500: 006e 1031 0073 4c30 0001 0001 0001 0059  .n.1.sL0.......Y
+00000510: 0001 0064 0053 0029 034e 7a10 7075 6273  ...d.S.).Nz.pubs
+00000520: 7562 2e73 656e 645f 616c 6c28 fa01 2929  ub.send_all(..))
+00000530: 0672 0f00 0000 7210 0000 0072 1500 0000  .r....r....r....
+00000540: 7216 0000 00da 0676 616c 7565 73da 105f  r......values.._
+00000550: 5075 6253 7562 4875 625f 5f73 656e 6429  PubSubHub__send)
+00000560: 0372 1900 0000 721d 0000 00da 0768 616e  .r....r......han
+00000570: 646c 6572 721a 0000 0072 1a00 0000 721b  dlerr....r....r.
+00000580: 0000 00da 0873 656e 645f 616c 6c22 0000  .....send_all"..
+00000590: 0073 0800 0000 0001 1201 0801 0e01 7a12  .s............z.
+000005a0: 5075 6253 7562 4875 622e 7365 6e64 5f61  PubSubHub.send_a
+000005b0: 6c6c 2902 da05 746f 7069 6372 1d00 0000  ll)...topicr....
+000005c0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+000005d0: 0008 0000 0043 0000 0073 7000 0000 7400  .....C...sp...t.
+000005e0: a001 6401 7c01 9b00 6402 7c02 9b00 6403  ..d.|...d.|...d.
+000005f0: 9d05 a101 0100 7c00 6a02 8f3e 0100 7c01  ......|.j..>..|.
+00000600: 7c00 6a03 7600 724e 7c00 6a03 7c01 1900  |.j.v.rN|.j.|...
+00000610: a004 a100 4400 5d14 7d03 7c00 a005 7c03  ....D.].}.|...|.
+00000620: 7c01 7c02 6702 a102 0100 7138 5700 6400  |.|.g.....q8W.d.
+00000630: 0400 0400 8303 0100 6e10 3100 7362 3000  ........n.1.sb0.
+00000640: 0100 0100 0100 5900 0100 6400 5300 2904  ......Y...d.S.).
+00000650: 4e7a 1970 7562 7375 622e 7365 6e64 5f61  Nz.pubsub.send_a
+00000660: 6c6c 5f6f 6e5f 746f 7069 6328 fa02 2c20  ll_on_topic(.., 
+00000670: 721e 0000 0029 0672 0f00 0000 7210 0000  r....).r....r...
+00000680: 0072 1500 0000 7217 0000 0072 1f00 0000  .r....r....r....
+00000690: 7220 0000 0029 0472 1900 0000 7223 0000  r ...).r....r#..
+000006a0: 0072 1d00 0000 7221 0000 0072 1a00 0000  .r....r!...r....
+000006b0: 721a 0000 0072 1b00 0000 da11 7365 6e64  r....r......send
+000006c0: 5f61 6c6c 5f6f 6e5f 746f 7069 6328 0000  _all_on_topic(..
+000006d0: 0073 0a00 0000 0001 1801 0801 0a01 1201  .s..............
+000006e0: 7a1b 5075 6253 7562 4875 622e 7365 6e64  z.PubSubHub.send
+000006f0: 5f61 6c6c 5f6f 6e5f 746f 7069 6329 02da  _all_on_topic)..
+00000700: 1165 7863 6570 745f 7365 7373 696f 6e5f  .except_session_
+00000710: 6964 721d 0000 0063 0300 0000 0000 0000  idr....c........
+00000720: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
+00000730: 736c 0000 0074 00a0 0164 017c 019b 0064  sl...t...d.|...d
+00000740: 027c 029b 0064 039d 05a1 0101 007c 006a  .|...d.......|.j
+00000750: 028f 3a01 007c 006a 03a0 04a1 0044 005d  ..:..|.j.....D.]
+00000760: 1e5c 027d 037d 047c 017c 036b 0372 2a7c  .\.}.}.|.|.k.r*|
+00000770: 00a0 057c 047c 0267 01a1 0201 0071 2a57  ...|.|.g.....q*W
+00000780: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+00000790: 5e30 0001 0001 0001 0059 0001 0064 0053  ^0.......Y...d.S
+000007a0: 0029 044e 7a13 7075 6273 7562 2e73 656e  .).Nz.pubsub.sen
+000007b0: 645f 6f74 6865 7273 2872 2400 0000 721e  d_others(r$...r.
+000007c0: 0000 0029 0672 0f00 0000 7210 0000 0072  ...).r....r....r
+000007d0: 1500 0000 7216 0000 00da 0569 7465 6d73  ....r......items
+000007e0: 7220 0000 0029 0572 1900 0000 7226 0000  r ...).r....r&..
+000007f0: 0072 1d00 0000 da0a 7365 7373 696f 6e5f  .r......session_
+00000800: 6964 7221 0000 0072 1a00 0000 721a 0000  idr!...r....r...
+00000810: 0072 1b00 0000 da0b 7365 6e64 5f6f 7468  .r......send_oth
+00000820: 6572 732f 0000 0073 0a00 0000 0001 1801  ers/...s........
+00000830: 0801 1201 0801 7a15 5075 6253 7562 4875  ......z.PubSubHu
+00000840: 622e 7365 6e64 5f6f 7468 6572 7329 0372  b.send_others).r
+00000850: 2600 0000 7223 0000 0072 1d00 0000 6304  &...r#...r....c.
+00000860: 0000 0000 0000 0000 0000 0006 0000 0009  ................
+00000870: 0000 0043 0000 0073 8200 0000 7400 a001  ...C...s....t...
+00000880: 6401 7c01 9b00 6402 7c02 9b00 6402 7c03  d.|...d.|...d.|.
+00000890: 9b00 6403 9d07 a101 0100 7c00 6a02 8f4a  ..d.......|.j..J
+000008a0: 0100 7c02 7c00 6a03 7600 7260 7c00 6a03  ..|.|.j.v.r`|.j.
+000008b0: 7c02 1900 a004 a100 4400 5d20 5c02 7d04  |.......D.] \.}.
+000008c0: 7d05 7c01 7c04 6b03 723e 7c00 a005 7c05  }.|.|.k.r>|...|.
+000008d0: 7c02 7c03 6702 a102 0100 713e 5700 6400  |.|.g.....q>W.d.
+000008e0: 0400 0400 8303 0100 6e10 3100 7374 3000  ........n.1.st0.
+000008f0: 0100 0100 0100 5900 0100 6400 5300 2904  ......Y...d.S.).
+00000900: 4e7a 1c70 7562 7375 622e 7365 6e64 5f6f  Nz.pubsub.send_o
+00000910: 7468 6572 735f 6f6e 5f74 6f70 6963 2872  thers_on_topic(r
+00000920: 2400 0000 721e 0000 0029 0672 0f00 0000  $...r....).r....
+00000930: 7210 0000 0072 1500 0000 7217 0000 0072  r....r....r....r
+00000940: 2700 0000 7220 0000 0029 0672 1900 0000  '...r ...).r....
+00000950: 7226 0000 0072 2300 0000 721d 0000 0072  r&...r#...r....r
+00000960: 2800 0000 7221 0000 0072 1a00 0000 721a  (...r!...r....r.
+00000970: 0000 0072 1b00 0000 da14 7365 6e64 5f6f  ...r......send_o
+00000980: 7468 6572 735f 6f6e 5f74 6f70 6963 3600  thers_on_topic6.
+00000990: 0000 7310 0000 0000 0104 0116 ff04 0308  ..s.............
+000009a0: 010a 0116 0108 017a 1e50 7562 5375 6248  .......z.PubSubH
+000009b0: 7562 2e73 656e 645f 6f74 6865 7273 5f6f  ub.send_others_o
+000009c0: 6e5f 746f 7069 6329 0272 2800 0000 7221  n_topic).r(...r!
+000009d0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+000009e0: 0300 0000 0800 0000 4300 0000 7346 0000  ........C...sF..
+000009f0: 0074 00a0 0164 017c 019b 0064 029d 03a1  .t...d.|...d....
+00000a00: 0101 007c 006a 028f 1a01 007c 027c 006a  ...|.j.....|.|.j
+00000a10: 037c 013c 0057 0064 0004 0004 0083 0301  .|.<.W.d........
+00000a20: 006e 1031 0073 3830 0001 0001 0001 0059  .n.1.s80.......Y
+00000a30: 0001 0064 0053 0029 034e 7a11 7075 6273  ...d.S.).Nz.pubs
+00000a40: 7562 2e73 7562 7363 7269 6265 2872 1e00  ub.subscribe(r..
+00000a50: 0000 2904 720f 0000 0072 1000 0000 7215  ..).r....r....r.
+00000a60: 0000 0072 1600 0000 2903 7219 0000 0072  ...r....).r....r
+00000a70: 2800 0000 7221 0000 0072 1a00 0000 721a  (...r!...r....r.
+00000a80: 0000 0072 1b00 0000 da09 7375 6273 6372  ...r......subscr
+00000a90: 6962 6540 0000 0073 0600 0000 0001 1201  ibe@...s........
+00000aa0: 0801 7a13 5075 6253 7562 4875 622e 7375  ..z.PubSubHub.su
+00000ab0: 6273 6372 6962 652e 2903 7228 0000 0072  bscribe.).r(...r
+00000ac0: 2300 0000 7221 0000 0063 0400 0000 0000  #...r!...c......
+00000ad0: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
+00000ae0: 0000 7350 0000 0074 00a0 0164 017c 019b  ..sP...t...d.|..
+00000af0: 0064 027c 029b 0064 039d 05a1 0101 007c  .d.|...d.......|
+00000b00: 006a 028f 1e01 007c 00a0 037c 017c 027c  .j.....|...|.|.|
+00000b10: 03a1 0301 0057 0064 0004 0004 0083 0301  .....W.d........
+00000b20: 006e 1031 0073 4230 0001 0001 0001 0059  .n.1.sB0.......Y
+00000b30: 0001 0064 0053 0029 044e 7a17 7075 6273  ...d.S.).Nz.pubs
+00000b40: 7562 2e73 7562 7363 7269 6265 5f74 6f70  ub.subscribe_top
+00000b50: 6963 2872 2400 0000 721e 0000 0029 0472  ic(r$...r....).r
+00000b60: 0f00 0000 7210 0000 0072 1500 0000 da1b  ....r....r......
+00000b70: 5f50 7562 5375 6248 7562 5f5f 7375 6273  _PubSubHub__subs
+00000b80: 6372 6962 655f 746f 7069 6329 0472 1900  cribe_topic).r..
+00000b90: 0000 7228 0000 0072 2300 0000 7221 0000  ..r(...r#...r!..
+00000ba0: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000bb0: da0f 7375 6273 6372 6962 655f 746f 7069  ..subscribe_topi
+00000bc0: 6345 0000 0073 0600 0000 0006 1801 0801  cE...s..........
+00000bd0: 7a19 5075 6253 7562 4875 622e 7375 6273  z.PubSubHub.subs
+00000be0: 6372 6962 655f 746f 7069 6363 0400 0000  cribe_topicc....
+00000bf0: 0000 0000 0000 0000 0600 0000 0300 0000  ................
+00000c00: 4300 0000 7358 0000 007c 006a 00a0 017c  C...sX...|.j...|
+00000c10: 02a1 017d 047c 0464 0075 0072 2269 007d  ...}.|.d.u.r"i.}
+00000c20: 047c 047c 006a 007c 023c 007c 037c 047c  .|.|.j.|.<.|.|.|
+00000c30: 013c 007c 006a 02a0 017c 01a1 017d 057c  .<.|.j...|...}.|
+00000c40: 0564 0075 0072 4c69 007d 057c 057c 006a  .d.u.rLi.}.|.|.j
+00000c50: 027c 013c 007c 037c 057c 023c 0064 0053  .|.<.|.|.|.<.d.S
+00000c60: 0029 014e 2903 7217 0000 00da 0367 6574  .).N).r......get
+00000c70: 7218 0000 0029 0672 1900 0000 7228 0000  r....).r....r(..
+00000c80: 0072 2300 0000 7221 0000 00da 1174 6f70  .r#...r!.....top
+00000c90: 6963 5f73 7562 7363 7269 6265 7273 da11  ic_subscribers..
+00000ca0: 7375 6273 6372 6962 6572 5f74 6f70 6963  subscriber_topic
+00000cb0: 7372 1a00 0000 721a 0000 0072 1b00 0000  sr....r....r....
+00000cc0: 5a11 5f5f 7375 6273 6372 6962 655f 746f  Z.__subscribe_to
+00000cd0: 7069 634f 0000 0073 1400 0000 0006 0c01  picO...s........
+00000ce0: 0801 0401 0a01 0801 0c01 0801 0401 0a01  ................
+00000cf0: 7a1b 5075 6253 7562 4875 622e 5f5f 7375  z.PubSubHub.__su
+00000d00: 6273 6372 6962 655f 746f 7069 6329 0172  bscribe_topic).r
+00000d10: 2800 0000 6302 0000 0000 0000 0000 0000  (...c...........
+00000d20: 0002 0000 0008 0000 0043 0000 0073 4600  .........C...sF.
+00000d30: 0000 7400 a001 6401 7c01 9b00 6402 9d03  ..t...d.|...d...
+00000d40: a101 0100 7c00 6a02 8f1a 0100 7c00 a003  ....|.j.....|...
+00000d50: 7c01 a101 0100 5700 6400 0400 0400 8303  |.....W.d.......
+00000d60: 0100 6e10 3100 7338 3000 0100 0100 0100  ..n.1.s80.......
+00000d70: 5900 0100 6400 5300 2903 4efa 1370 7562  Y...d.S.).N..pub
+00000d80: 7375 622e 756e 7375 6273 6372 6962 6528  sub.unsubscribe(
+00000d90: 721e 0000 0029 0472 0f00 0000 7210 0000  r....).r....r...
+00000da0: 0072 1500 0000 da17 5f50 7562 5375 6248  .r......_PubSubH
+00000db0: 7562 5f5f 756e 7375 6273 6372 6962 65a9  ub__unsubscribe.
+00000dc0: 0272 1900 0000 7228 0000 0072 1a00 0000  .r....r(...r....
+00000dd0: 721a 0000 0072 1b00 0000 da0b 756e 7375  r....r......unsu
+00000de0: 6273 6372 6962 6560 0000 0073 0600 0000  bscribe`...s....
+00000df0: 0001 1201 0801 7a15 5075 6253 7562 4875  ......z.PubSubHu
+00000e00: 622e 756e 7375 6273 6372 6962 6529 0272  b.unsubscribe).r
+00000e10: 2800 0000 7223 0000 0063 0300 0000 0000  (...r#...c......
+00000e20: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
+00000e30: 0000 734e 0000 0074 00a0 0164 017c 019b  ..sN...t...d.|..
+00000e40: 0064 027c 029b 0064 039d 05a1 0101 007c  .d.|...d.......|
+00000e50: 006a 028f 1c01 007c 00a0 037c 017c 02a1  .j.....|...|.|..
+00000e60: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+00000e70: 1031 0073 4030 0001 0001 0001 0059 0001  .1.s@0.......Y..
+00000e80: 0064 0053 0029 044e 7231 0000 0072 2400  .d.S.).Nr1...r$.
+00000e90: 0000 721e 0000 0029 0472 0f00 0000 7210  ..r....).r....r.
+00000ea0: 0000 0072 1500 0000 da1d 5f50 7562 5375  ...r......_PubSu
+00000eb0: 6248 7562 5f5f 756e 7375 6273 6372 6962  bHub__unsubscrib
+00000ec0: 655f 746f 7069 63a9 0372 1900 0000 7228  e_topic..r....r(
+00000ed0: 0000 0072 2300 0000 721a 0000 0072 1a00  ...r#...r....r..
+00000ee0: 0000 721b 0000 00da 1175 6e73 7562 7363  ..r......unsubsc
+00000ef0: 7269 6265 5f74 6f70 6963 6500 0000 7306  ribe_topice...s.
+00000f00: 0000 0000 0118 0108 017a 1b50 7562 5375  .........z.PubSu
+00000f10: 6248 7562 2e75 6e73 7562 7363 7269 6265  bHub.unsubscribe
+00000f20: 5f74 6f70 6963 6302 0000 0000 0000 0000  _topicc.........
+00000f30: 0000 0003 0000 0008 0000 0043 0000 0073  ...........C...s
+00000f40: 7000 0000 7400 a001 6401 7c01 9b00 6402  p...t...d.|...d.
+00000f50: 9d03 a101 0100 7c00 6a02 8f44 0100 7c00  ......|.j..D..|.
+00000f60: a003 7c01 a101 0100 7c01 7c00 6a04 7600  ..|.....|.|.j.v.
+00000f70: 724e 7c00 6a04 7c01 1900 a005 a100 4400  rN|.j.|.......D.
+00000f80: 5d10 7d02 7c00 a006 7c01 7c02 a102 0100  ].}.|...|.|.....
+00000f90: 713c 5700 6400 0400 0400 8303 0100 6e10  q<W.d.........n.
+00000fa0: 3100 7362 3000 0100 0100 0100 5900 0100  1.sb0.......Y...
+00000fb0: 6400 5300 2903 4e7a 1770 7562 7375 622e  d.S.).Nz.pubsub.
+00000fc0: 756e 7375 6273 6372 6962 655f 616c 6c28  unsubscribe_all(
+00000fd0: 721e 0000 0029 0772 0f00 0000 7210 0000  r....).r....r...
+00000fe0: 0072 1500 0000 7232 0000 0072 1800 0000  .r....r2...r....
+00000ff0: da04 6b65 7973 7235 0000 0072 3600 0000  ..keysr5...r6...
+00001000: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+00001010: 0f75 6e73 7562 7363 7269 6265 5f61 6c6c  .unsubscribe_all
+00001020: 6a00 0000 730c 0000 0000 0112 0108 010a  j...s...........
+00001030: 010a 0112 017a 1950 7562 5375 6248 7562  .....z.PubSubHub
+00001040: 2e75 6e73 7562 7363 7269 6265 5f61 6c6c  .unsubscribe_all
+00001050: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001060: 0005 0000 0043 0000 0073 2400 0000 7400  .....C...s$...t.
+00001070: a001 6401 7c01 9b00 6402 9d03 a101 0100  ..d.|...d.......
+00001080: 7c00 6a02 a003 7c01 6400 a102 0100 6400  |.j...|.d.....d.
+00001090: 5300 2903 4e7a 1570 7562 7375 622e 5f5f  S.).Nz.pubsub.__
+000010a0: 756e 7375 6273 6372 6962 6528 721e 0000  unsubscribe(r...
+000010b0: 0029 0472 0f00 0000 7210 0000 0072 1600  .).r....r....r..
+000010c0: 0000 da03 706f 7072 3300 0000 721a 0000  ....popr3...r...
+000010d0: 0072 1a00 0000 721b 0000 005a 0d5f 5f75  .r....r....Z.__u
+000010e0: 6e73 7562 7363 7269 6265 7200 0000 7304  nsubscriber...s.
+000010f0: 0000 0000 0112 017a 1750 7562 5375 6248  .......z.PubSubH
+00001100: 7562 2e5f 5f75 6e73 7562 7363 7269 6265  ub.__unsubscribe
+00001110: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
+00001120: 0007 0000 0043 0000 0073 9000 0000 7400  .....C...s....t.
+00001130: a001 6401 7c01 9b00 6402 7c02 9b00 6403  ..d.|...d.|...d.
+00001140: 9d05 a101 0100 7c00 6a02 a003 7c02 a101  ......|.j...|...
+00001150: 7d03 7c03 6400 7501 7252 7c03 a004 7c01  }.|.d.u.rR|...|.
+00001160: 6400 a102 0100 7405 7c03 8301 6404 6b02  d.....t.|...d.k.
+00001170: 7252 7c00 6a02 a004 7c02 6400 a102 0100  rR|.j...|.d.....
+00001180: 7c00 6a06 a003 7c01 a101 7d04 7c04 6400  |.j...|...}.|.d.
+00001190: 7501 728c 7c04 a004 7c02 6400 a102 0100  u.r.|...|.d.....
+000011a0: 7405 7c04 8301 6404 6b02 728c 7c00 6a06  t.|...d.k.r.|.j.
+000011b0: a004 7c01 6400 a102 0100 6400 5300 2905  ..|.d.....d.S.).
+000011c0: 4e7a 1b70 7562 7375 622e 5f5f 756e 7375  Nz.pubsub.__unsu
+000011d0: 6273 6372 6962 655f 746f 7069 6328 7224  bscribe_topic(r$
+000011e0: 0000 0072 1e00 0000 7201 0000 0029 0772  ...r....r....).r
+000011f0: 0f00 0000 7210 0000 0072 1700 0000 722e  ....r....r....r.
+00001200: 0000 0072 3a00 0000 da03 6c65 6e72 1800  ...r:.....lenr..
+00001210: 0000 2905 7219 0000 0072 2800 0000 7223  ..).r....r(...r#
+00001220: 0000 0072 2f00 0000 7230 0000 0072 1a00  ...r/...r0...r..
+00001230: 0000 721a 0000 0072 1b00 0000 5a13 5f5f  ..r....r....Z.__
+00001240: 756e 7375 6273 6372 6962 655f 746f 7069  unsubscribe_topi
+00001250: 6376 0000 0073 1600 0000 0001 1801 0c01  cv...s..........
+00001260: 0801 0c01 0c01 0e01 0c01 0801 0c01 0c01  ................
+00001270: 7a1d 5075 6253 7562 4875 622e 5f5f 756e  z.PubSubHub.__un
+00001280: 7375 6273 6372 6962 655f 746f 7069 6329  subscribe_topic)
+00001290: 0272 2100 0000 da04 6172 6773 6303 0000  .r!.....argsc...
+000012a0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+000012b0: 0043 0000 0073 5e00 0000 7c00 6a00 730e  .C...s^...|.j.s.
+000012c0: 4a00 6401 8301 8201 7401 a002 7c01 a101  J.d.....t...|...
+000012d0: 722c 7401 a003 7c01 7c02 8e00 7c00 6a00  r,t...|.|...|.j.
+000012e0: a102 0100 6e2e 7c00 6a04 7252 7c00 6a00  ....n.|.j.rR|.j.
+000012f0: 6a05 7c00 6a00 6a06 7c00 6a04 7c01 6703  j.|.j.j.|.j.|.g.
+00001300: 7c02 a201 5200 8e00 0100 6e08 7c01 7c02  |...R.....n.|.|.
+00001310: 8e00 0100 6400 5300 2902 4e7a 1c50 7562  ....d.S.).Nz.Pub
+00001320: 5375 6220 6576 656e 7420 6c6f 6f70 2069  Sub event loop i
+00001330: 7320 6e6f 7420 7365 7429 0772 1100 0000  s not set).r....
+00001340: da07 6173 796e 6369 6fda 1369 7363 6f72  ..asyncio..iscor
+00001350: 6f75 7469 6e65 6675 6e63 7469 6f6e da18  outinefunction..
+00001360: 7275 6e5f 636f 726f 7574 696e 655f 7468  run_coroutine_th
+00001370: 7265 6164 7361 6665 7212 0000 00da 1463  readsafer......c
+00001380: 616c 6c5f 736f 6f6e 5f74 6872 6561 6473  all_soon_threads
+00001390: 6166 65da 0f72 756e 5f69 6e5f 6578 6563  afe..run_in_exec
+000013a0: 7574 6f72 2903 7219 0000 0072 2100 0000  utor).r....r!...
+000013b0: 723c 0000 0072 1a00 0000 721a 0000 0072  r<...r....r....r
+000013c0: 1b00 0000 5a06 5f5f 7365 6e64 8300 0000  ....Z.__send....
+000013d0: 7314 0000 0000 030e 020a 0114 0206 0106  s...............
+000013e0: 010c ff02 0102 ff0a 047a 1050 7562 5375  .........z.PubSu
+000013f0: 6248 7562 2e5f 5f73 656e 6429 024e 4e29  bHub.__send).NN)
+00001400: 1bda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00001410: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00001420: 616d 655f 5f72 0800 0000 723d 0000 00da  ame__r....r=....
+00001430: 1141 6273 7472 6163 7445 7665 6e74 4c6f  .AbstractEventLo
+00001440: 6f70 7202 0000 0072 1c00 0000 7203 0000  opr....r....r...
+00001450: 0072 2200 0000 da03 7374 7272 2500 0000  .r".....strr%...
+00001460: 7229 0000 0072 2a00 0000 7205 0000 0072  r)...r*...r....r
+00001470: 2b00 0000 7209 0000 0072 0400 0000 722d  +...r....r....r-
+00001480: 0000 0072 2c00 0000 7234 0000 0072 3700  ...r,...r4...r7.
+00001490: 0000 7239 0000 0072 3200 0000 7235 0000  ..r9...r2...r5..
+000014a0: 0072 0700 0000 7220 0000 0072 1a00 0000  .r....r ...r....
+000014b0: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+000014c0: 0c00 0000 0e00 0000 7334 0000 0008 0300  ........s4......
+000014d0: 0100 fd02 0208 0106 fd0c 130e 0610 0710  ................
+000014e0: 0712 0a10 0702 0102 0116 fc0c 0c02 0102  ................
+000014f0: 0116 fc0c 110e 0510 050e 080e 0410 0e18  ................
+00001500: ff72 0c00 0000 2916 723d 0000 00da 076c  .r....).r=.....l
+00001510: 6f67 6769 6e67 7213 0000 00da 1263 6f6e  oggingr......con
+00001520: 6375 7272 656e 742e 6675 7475 7265 7372  current.futuresr
+00001530: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00001540: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00001550: 7207 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
+00001560: 0966 6c65 745f 636f 7265 da0f 666c 6574  .flet_core..flet
+00001570: 5f63 6f72 652e 6c6f 636b 7372 0a00 0000  _core.locksr....
+00001580: da21 666c 6574 5f63 6f72 652e 7574 696c  .!flet_core.util
+00001590: 732e 636f 6e63 7572 7265 6e63 795f 7574  s.concurrency_ut
+000015a0: 696c 7372 0b00 0000 da09 6765 744c 6f67  ilsr......getLog
+000015b0: 6765 7272 4200 0000 720f 0000 0072 0c00  gerrB...r....r..
+000015c0: 0000 721a 0000 0072 1a00 0000 721a 0000  ..r....r....r...
+000015d0: 0072 1b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000015e0: 0100 0000 7312 0000 0008 0108 0108 010c  ....s...........
+000015f0: 0124 0208 010c 010c 020c 03              .$.........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/pubsub_client.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/pubsub_client.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/pubsub/pubsub_hub.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/pubsub/pubsub_hub.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/querystring.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/radio.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/radio_group.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/range_slider.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/range_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/responsive_row.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/rive.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/rive.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/row.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/safe_area.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/safe_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/scrollable_control.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/search_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/search_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/segmented_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/selection_area.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/selection_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/semantics.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/semantics_service.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/semantics_service.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/session_storage.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/shader_mask.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/shadow.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/shake_detector.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/slider.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/snack_bar.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/stack.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/submenu_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/submenu_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/switch.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/tabs.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/template_route.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/text.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/text_button.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/text_span.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/text_style.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/textfield.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/theme.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/time_picker.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/time_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/tooltip.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/transform.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/transparent_pointer.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/two_dimensional_scrollables.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/two_dimensional_scrollables.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/types.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 311 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 3701 0000  a........:)f7...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 3701 0000  a........./f7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6407 5300 2908  d.l.m.Z...d.S.).
@@ -21,16 +21,16 @@
 00000140: 2e75 7469 6c73 2e73 6c75 6769 6679 7205  .utils.slugifyr.
 00000150: 0000 005a 1766 6c65 745f 636f 7265 2e75  ...Z.flet_core.u
 00000160: 7469 6c73 2e73 7472 696e 6773 7206 0000  tils.stringsr...
 00000170: 005a 1666 6c65 745f 636f 7265 2e75 7469  .Z.flet_core.uti
 00000180: 6c73 2e76 6563 746f 7272 0700 0000 5a1d  ls.vectorr....Z.
 00000190: 666c 6574 5f63 6f72 652e 7574 696c 732e  flet_core.utils.
 000001a0: 636c 6173 7370 726f 7065 7274 7972 0800  classpropertyr..
-000001b0: 0000 a900 7209 0000 0072 0900 0000 fa5a  ....r....r.....Z
+000001b0: 0000 a900 7209 0000 0072 0900 0000 fa61  ....r....r.....a
 000001c0: 2f77 6f72 6b73 7061 6365 732f 636f 6e74  /workspaces/cont
-000001d0: 7269 6266 6c65 742f 666c 6574 2f73 646b  ribflet/flet/sdk
-000001e0: 2f70 7974 686f 6e2f 7061 636b 6167 6573  /python/packages
-000001f0: 2f66 6c65 742d 636f 7265 2f73 7263 2f66  /flet-core/src/f
-00000200: 6c65 745f 636f 7265 2f75 7469 6c73 2f5f  let_core/utils/_
-00000210: 5f69 6e69 745f 5f2e 7079 da08 3c6d 6f64  _init__.py..<mod
-00000220: 756c 653e 0100 0000 730a 0000 0010 010c  ule>....s.......
-00000230: 010c 010c 010c 01                        .......
+000001d0: 7269 6266 6c65 742f 666c 6574 636f 6e74  ribflet/fletcont
+000001e0: 7269 622f 7364 6b2f 7079 7468 6f6e 2f70  rib/sdk/python/p
+000001f0: 6163 6b61 6765 732f 666c 6574 2d63 6f72  ackages/flet-cor
+00000200: 652f 7372 632f 666c 6574 5f63 6f72 652f  e/src/flet_core/
+00000210: 7574 696c 732f 5f5f 696e 6974 5f5f 2e70  utils/__init__.p
+00000220: 79da 083c 6d6f 6475 6c65 3e01 0000 0073  y..<module>....s
+00000230: 0a00 0000 1001 0c01 0c01 0c01 0c01       ..............
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 0f01 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 0f01 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6501 6402 8301 5a05 4700  m.Z...e.d...Z.G.
 00000050: 6403 6404 8400 6404 8302 5a06 6405 5300  d.d...d...Z.d.S.
 00000060: 2906 e900 0000 0029 04da 0754 7970 6556  )......)...TypeV
 00000070: 6172 da04 5479 7065 da03 416e 79da 0843  ar..Type..Any..C
@@ -15,38 +15,38 @@
 000000e0: 8404 5a08 6401 5300 2908 da0d 636c 6173  ..Z.d.S.)...clas
 000000f0: 7370 726f 7065 7274 794e 2902 da04 6675  spropertyN)...fu
 00000100: 6e63 da06 7265 7475 726e 6302 0000 0000  nc..returnc.....
 00000110: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
 00000120: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
 00000130: 5300 a901 4ea9 01da 0466 6765 7429 02da  S...N....fget)..
 00000140: 0473 656c 6672 0800 0000 a900 720e 0000  .selfr......r...
-00000150: 00fa 5f2f 776f 726b 7370 6163 6573 2f63  .._/workspaces/c
-00000160: 6f6e 7472 6962 666c 6574 2f66 6c65 742f  ontribflet/flet/
-00000170: 7364 6b2f 7079 7468 6f6e 2f70 6163 6b61  sdk/python/packa
-00000180: 6765 732f 666c 6574 2d63 6f72 652f 7372  ges/flet-core/sr
-00000190: 632f 666c 6574 5f63 6f72 652f 7574 696c  c/flet_core/util
-000001a0: 732f 636c 6173 7370 726f 7065 7274 792e  s/classproperty.
-000001b0: 7079 da08 5f5f 696e 6974 5f5f 0800 0000  py..__init__....
-000001c0: 7302 0000 0000 017a 1663 6c61 7373 7072  s......z.classpr
-000001d0: 6f70 6572 7479 2e5f 5f69 6e69 745f 5f29  operty.__init__)
-000001e0: 03da 0869 6e73 7461 6e63 65da 056f 776e  ...instance..own
-000001f0: 6572 7209 0000 0063 0300 0000 0000 0000  err....c........
-00000200: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-00000210: 730a 0000 007c 00a0 007c 02a1 0153 0072  s....|...|...S.r
-00000220: 0a00 0000 720b 0000 0029 0372 0d00 0000  ....r....).r....
-00000230: 7211 0000 0072 1200 0000 720e 0000 0072  r....r....r....r
-00000240: 0e00 0000 720f 0000 00da 075f 5f67 6574  ....r......__get
-00000250: 5f5f 0b00 0000 7302 0000 0000 017a 1563  __....s......z.c
-00000260: 6c61 7373 7072 6f70 6572 7479 2e5f 5f67  lassproperty.__g
-00000270: 6574 5f5f 2909 da08 5f5f 6e61 6d65 5f5f  et__)...__name__
-00000280: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000290: 7175 616c 6e61 6d65 5f5f 7205 0000 0072  qualname__r....r
-000002a0: 0300 0000 7206 0000 0072 0400 0000 7210  ....r....r....r.
-000002b0: 0000 0072 1300 0000 720e 0000 0072 0e00  ...r....r....r..
-000002c0: 0000 720e 0000 0072 0f00 0000 7207 0000  ..r....r....r...
-000002d0: 0007 0000 0073 0400 0000 0801 1e03 7207  .....s........r.
-000002e0: 0000 004e 2907 da06 7479 7069 6e67 7202  ...N)...typingr.
-000002f0: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-00000300: 0000 7206 0000 0072 0700 0000 720e 0000  ..r....r....r...
-00000310: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000320: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
-00000330: 0000 0018 0308 03                        .......
+00000150: 00fa 662f 776f 726b 7370 6163 6573 2f63  ..f/workspaces/c
+00000160: 6f6e 7472 6962 666c 6574 2f66 6c65 7463  ontribflet/fletc
+00000170: 6f6e 7472 6962 2f73 646b 2f70 7974 686f  ontrib/sdk/pytho
+00000180: 6e2f 7061 636b 6167 6573 2f66 6c65 742d  n/packages/flet-
+00000190: 636f 7265 2f73 7263 2f66 6c65 745f 636f  core/src/flet_co
+000001a0: 7265 2f75 7469 6c73 2f63 6c61 7373 7072  re/utils/classpr
+000001b0: 6f70 6572 7479 2e70 79da 085f 5f69 6e69  operty.py..__ini
+000001c0: 745f 5f08 0000 0073 0200 0000 0001 7a16  t__....s......z.
+000001d0: 636c 6173 7370 726f 7065 7274 792e 5f5f  classproperty.__
+000001e0: 696e 6974 5f5f 2903 da08 696e 7374 616e  init__)...instan
+000001f0: 6365 da05 6f77 6e65 7272 0900 0000 6303  ce..ownerr....c.
+00000200: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00000210: 0000 0043 0000 0073 0a00 0000 7c00 a000  ...C...s....|...
+00000220: 7c02 a101 5300 720a 0000 0072 0b00 0000  |...S.r....r....
+00000230: 2903 720d 0000 0072 1100 0000 7212 0000  ).r....r....r...
+00000240: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000250: da07 5f5f 6765 745f 5f0b 0000 0073 0200  ..__get__....s..
+00000260: 0000 0001 7a15 636c 6173 7370 726f 7065  ....z.classprope
+00000270: 7274 792e 5f5f 6765 745f 5f29 09da 085f  rty.__get__)..._
+00000280: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000290: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000002a0: 5f72 0500 0000 7203 0000 0072 0600 0000  _r....r....r....
+000002b0: 7204 0000 0072 1000 0000 7213 0000 0072  r....r....r....r
+000002c0: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+000002d0: 0000 0072 0700 0000 0700 0000 7304 0000  ...r........s...
+000002e0: 0008 011e 0372 0700 0000 4e29 07da 0674  .....r....N)...t
+000002f0: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
+00000300: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00000310: 0000 0072 0e00 0000 720e 0000 0072 0e00  ...r....r....r..
+00000320: 0000 720f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000330: 3e01 0000 0073 0400 0000 1803 0803       >....s........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 243 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 f300 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 f300 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6404 6405 8400 5a03 6401  d...Z.d.d...Z.d.
 00000050: 5300 2906 e900 0000 004e 6300 0000 0000  S.)......Nc.....
 00000060: 0000 0000 0000 0000 0000 0008 0000 0043  ...............C
 00000070: 0000 0073 3200 0000 7a18 7400 a001 a100  ...s2...z.t.....
 00000080: 6400 7501 7016 7402 6a03 6401 6b02 5700  d.u.p.t.j.d.k.W.
 00000090: 5300 0400 7404 792c 0100 0100 0100 5900  S...t.y,......Y.
 000000a0: 6402 5300 3000 6400 5300 2903 4eda 0a65  d.S.0.d.S.).N..e
 000000b0: 6d73 6372 6970 7465 6e46 2905 da07 6173  mscriptenF)...as
 000000c0: 796e 6369 6f5a 0c63 7572 7265 6e74 5f74  yncioZ.current_t
 000000d0: 6173 6bda 0373 7973 da08 706c 6174 666f  ask..sys..platfo
 000000e0: 726d da0c 5275 6e74 696d 6545 7272 6f72  rm..RuntimeError
-000000f0: a900 7207 0000 0072 0700 0000 fa63 2f77  ..r....r.....c/w
+000000f0: a900 7207 0000 0072 0700 0000 fa6a 2f77  ..r....r.....j/w
 00000100: 6f72 6b73 7061 6365 732f 636f 6e74 7269  orkspaces/contri
-00000110: 6266 6c65 742f 666c 6574 2f73 646b 2f70  bflet/flet/sdk/p
-00000120: 7974 686f 6e2f 7061 636b 6167 6573 2f66  ython/packages/f
-00000130: 6c65 742d 636f 7265 2f73 7263 2f66 6c65  let-core/src/fle
-00000140: 745f 636f 7265 2f75 7469 6c73 2f63 6f6e  t_core/utils/con
-00000150: 6375 7272 656e 6379 5f75 7469 6c73 2e70  currency_utils.p
-00000160: 79da 0a69 735f 6173 796e 6369 6f05 0000  y..is_asyncio...
-00000170: 0073 0800 0000 0001 0201 1801 0c01 7209  .s............r.
-00000180: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000190: 0000 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-000001a0: 0074 006a 0164 016b 0253 0029 024e 7202  .t.j.d.k.S.).Nr.
-000001b0: 0000 0029 0272 0400 0000 7205 0000 0072  ...).r....r....r
-000001c0: 0700 0000 7207 0000 0072 0700 0000 7208  ....r....r....r.
-000001d0: 0000 00da 0a69 735f 7079 6f64 6964 650c  .....is_pyodide.
-000001e0: 0000 0073 0200 0000 0001 720a 0000 0029  ...s......r....)
-000001f0: 0472 0300 0000 7204 0000 0072 0900 0000  .r....r....r....
-00000200: 720a 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
-00000210: 0700 0000 7208 0000 00da 083c 6d6f 6475  ....r......<modu
-00000220: 6c65 3e01 0000 0073 0600 0000 0801 0803  le>....s........
-00000230: 0807                                     ..
+00000110: 6266 6c65 742f 666c 6574 636f 6e74 7269  bflet/fletcontri
+00000120: 622f 7364 6b2f 7079 7468 6f6e 2f70 6163  b/sdk/python/pac
+00000130: 6b61 6765 732f 666c 6574 2d63 6f72 652f  kages/flet-core/
+00000140: 7372 632f 666c 6574 5f63 6f72 652f 7574  src/flet_core/ut
+00000150: 696c 732f 636f 6e63 7572 7265 6e63 795f  ils/concurrency_
+00000160: 7574 696c 732e 7079 da0a 6973 5f61 7379  utils.py..is_asy
+00000170: 6e63 696f 0500 0000 7308 0000 0000 0102  ncio....s.......
+00000180: 0118 010c 0172 0900 0000 6300 0000 0000  .....r....c.....
+00000190: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+000001a0: 0000 0073 0a00 0000 7400 6a01 6401 6b02  ...s....t.j.d.k.
+000001b0: 5300 2902 4e72 0200 0000 2902 7204 0000  S.).Nr....).r...
+000001c0: 0072 0500 0000 7207 0000 0072 0700 0000  .r....r....r....
+000001d0: 7207 0000 0072 0800 0000 da0a 6973 5f70  r....r......is_p
+000001e0: 796f 6469 6465 0c00 0000 7302 0000 0000  yodide....s.....
+000001f0: 0172 0a00 0000 2904 7203 0000 0072 0400  .r....).r....r..
+00000200: 0000 7209 0000 0072 0a00 0000 7207 0000  ..r....r....r...
+00000210: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000220: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
+00000230: 0000 0008 0108 0308 07                   .........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 835 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 4303 0000  a........:)fC...
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 4303 0000  a........./fC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6401 5300 2904 e900 0000  d...Z.d.S.).....
 00000050: 004e 6303 0000 0000 0000 0000 0000 0004  .Nc.............
 00000060: 0000 0003 0000 0003 0000 0073 1400 0000  ...........s....
 00000070: 8700 8701 8702 6603 6401 6402 8408 7d03  ......f.d.d...}.
@@ -43,35 +43,35 @@
 000002a0: 7461 636b 6c65 7665 6c29 04da 0877 6172  tacklevel)...war
 000002b0: 6e69 6e67 73da 0477 6172 6eda 085f 5f6e  nings..warn..__n
 000002c0: 616d 655f 5fda 1244 6570 7265 6361 7469  ame__..Deprecati
 000002d0: 6f6e 5761 726e 696e 6729 02da 0461 7267  onWarning)...arg
 000002e0: 73da 066b 7761 7267 7329 04da 0e64 656c  s..kwargs)...del
 000002f0: 6574 655f 7665 7273 696f 6eda 0466 756e  ete_version..fun
 00000300: 63da 0672 6561 736f 6eda 0776 6572 7369  c..reason..versi
-00000310: 6f6e a900 fa5c 2f77 6f72 6b73 7061 6365  on...\/workspace
+00000310: 6f6e a900 fa63 2f77 6f72 6b73 7061 6365  on...c/workspace
 00000320: 732f 636f 6e74 7269 6266 6c65 742f 666c  s/contribflet/fl
-00000330: 6574 2f73 646b 2f70 7974 686f 6e2f 7061  et/sdk/python/pa
-00000340: 636b 6167 6573 2f66 6c65 742d 636f 7265  ckages/flet-core
-00000350: 2f73 7263 2f66 6c65 745f 636f 7265 2f75  /src/flet_core/u
-00000360: 7469 6c73 2f64 6570 7265 6361 7465 642e  tils/deprecated.
-00000370: 7079 da08 6e65 775f 6675 6e63 0f00 0000  py..new_func....
-00000380: 7314 0000 0000 0204 0110 0102 ff04 0102  s...............
-00000390: ff04 0202 0102 fc06 067a 2f64 6570 7265  .........z/depre
-000003a0: 6361 7465 642e 3c6c 6f63 616c 733e 2e64  cated.<locals>.d
-000003b0: 6563 6f72 6174 6f72 2e3c 6c6f 6361 6c73  ecorator.<locals
-000003c0: 3e2e 6e65 775f 6675 6e63 2902 da09 6675  >.new_func)...fu
-000003d0: 6e63 746f 6f6c 73da 0577 7261 7073 2902  nctools..wraps).
-000003e0: 720c 0000 0072 1100 0000 a903 720b 0000  r....r......r...
-000003f0: 0072 0d00 0000 720e 0000 0029 0172 0c00  .r....r....).r..
-00000400: 0000 7210 0000 00da 0964 6563 6f72 6174  ..r......decorat
-00000410: 6f72 0e00 0000 7306 0000 0000 0108 0114  or....s.........
-00000420: 097a 1d64 6570 7265 6361 7465 642e 3c6c  .z.deprecated.<l
-00000430: 6f63 616c 733e 2e64 6563 6f72 6174 6f72  ocals>.decorator
-00000440: 720f 0000 0029 0472 0d00 0000 720e 0000  r....).r....r...
-00000450: 0072 0b00 0000 7215 0000 0072 0f00 0000  .r....r....r....
-00000460: 7214 0000 0072 1000 0000 da0a 6465 7072  r....r......depr
-00000470: 6563 6174 6564 0500 0000 7304 0000 0000  ecated....s.....
-00000480: 0910 0d72 1600 0000 2903 7212 0000 0072  ...r....).r....r
-00000490: 0500 0000 7216 0000 0072 0f00 0000 720f  ....r....r....r.
-000004a0: 0000 0072 0f00 0000 7210 0000 00da 083c  ...r....r......<
-000004b0: 6d6f 6475 6c65 3e01 0000 0073 0400 0000  module>....s....
-000004c0: 0801 0803                                ....
+00000330: 6574 636f 6e74 7269 622f 7364 6b2f 7079  etcontrib/sdk/py
+00000340: 7468 6f6e 2f70 6163 6b61 6765 732f 666c  thon/packages/fl
+00000350: 6574 2d63 6f72 652f 7372 632f 666c 6574  et-core/src/flet
+00000360: 5f63 6f72 652f 7574 696c 732f 6465 7072  _core/utils/depr
+00000370: 6563 6174 6564 2e70 79da 086e 6577 5f66  ecated.py..new_f
+00000380: 756e 630f 0000 0073 1400 0000 0002 0401  unc....s........
+00000390: 1001 02ff 0401 02ff 0402 0201 02fc 0606  ................
+000003a0: 7a2f 6465 7072 6563 6174 6564 2e3c 6c6f  z/deprecated.<lo
+000003b0: 6361 6c73 3e2e 6465 636f 7261 746f 722e  cals>.decorator.
+000003c0: 3c6c 6f63 616c 733e 2e6e 6577 5f66 756e  <locals>.new_fun
+000003d0: 6329 02da 0966 756e 6374 6f6f 6c73 da05  c)...functools..
+000003e0: 7772 6170 7329 0272 0c00 0000 7211 0000  wraps).r....r...
+000003f0: 00a9 0372 0b00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000400: 0000 2901 720c 0000 0072 1000 0000 da09  ..).r....r......
+00000410: 6465 636f 7261 746f 720e 0000 0073 0600  decorator....s..
+00000420: 0000 0001 0801 1409 7a1d 6465 7072 6563  ........z.deprec
+00000430: 6174 6564 2e3c 6c6f 6361 6c73 3e2e 6465  ated.<locals>.de
+00000440: 636f 7261 746f 7272 0f00 0000 2904 720d  coratorr....).r.
+00000450: 0000 0072 0e00 0000 720b 0000 0072 1500  ...r....r....r..
+00000460: 0000 720f 0000 0072 1400 0000 7210 0000  ..r....r....r...
+00000470: 00da 0a64 6570 7265 6361 7465 6405 0000  ...deprecated...
+00000480: 0073 0400 0000 0009 100d 7216 0000 0029  .s........r....)
+00000490: 0372 1200 0000 7205 0000 0072 1600 0000  .r....r....r....
+000004a0: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+000004b0: 1000 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000004c0: 0000 7304 0000 0008 0108 03              ..s........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 465 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 d101 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 d101 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6502  d.l.Z.d.d.l.Z.e.
 00000040: 6502 6402 9c02 6403 6404 8404 5a03 6401  e.d...d.d...Z.d.
 00000050: 5300 2905 e900 0000 004e 2902 da05 7661  S.)......N)...va
 00000060: 6c75 65da 0672 6574 7572 6e63 0100 0000  lue..returnc....
 00000070: 0000 0000 0000 0000 0100 0000 0500 0000  ................
@@ -25,20 +25,20 @@
 00000180: 4e46 4b44 da05 6173 6369 69da 0669 676e  NFKD..ascii..ign
 00000190: 6f72 657a 085b 5e5c 775c 732d 5dda 007a  orez.[^\w\s-]..z
 000001a0: 065b 2d5c 735d 2bfa 012d 2908 da0b 756e  .[-\s]+..-)...un
 000001b0: 6963 6f64 6564 6174 615a 096e 6f72 6d61  icodedataZ.norma
 000001c0: 6c69 7a65 da06 656e 636f 6465 da06 6465  lize..encode..de
 000001d0: 636f 6465 da02 7265 da03 7375 62da 0573  code..re..sub..s
 000001e0: 7472 6970 da05 6c6f 7765 7229 0172 0200  trip..lower).r..
-000001f0: 0000 a900 720f 0000 00fa 592f 776f 726b  ....r.....Y/work
+000001f0: 0000 a900 720f 0000 00fa 602f 776f 726b  ....r.....`/work
 00000200: 7370 6163 6573 2f63 6f6e 7472 6962 666c  spaces/contribfl
-00000210: 6574 2f66 6c65 742f 7364 6b2f 7079 7468  et/flet/sdk/pyth
-00000220: 6f6e 2f70 6163 6b61 6765 732f 666c 6574  on/packages/flet
-00000230: 2d63 6f72 652f 7372 632f 666c 6574 5f63  -core/src/flet_c
-00000240: 6f72 652f 7574 696c 732f 736c 7567 6966  ore/utils/slugif
-00000250: 792e 7079 da07 736c 7567 6966 7905 0000  y.py..slugify...
-00000260: 0073 0800 0000 0006 18ff 0203 1601 7211  .s............r.
-00000270: 0000 0029 0472 0b00 0000 7208 0000 00da  ...).r....r.....
-00000280: 0373 7472 7211 0000 0072 0f00 0000 720f  .strr....r....r.
-00000290: 0000 0072 0f00 0000 7210 0000 00da 083c  ...r....r......<
-000002a0: 6d6f 6475 6c65 3e01 0000 0073 0400 0000  module>....s....
-000002b0: 0801 0803                                ....
+00000210: 6574 2f66 6c65 7463 6f6e 7472 6962 2f73  et/fletcontrib/s
+00000220: 646b 2f70 7974 686f 6e2f 7061 636b 6167  dk/python/packag
+00000230: 6573 2f66 6c65 742d 636f 7265 2f73 7263  es/flet-core/src
+00000240: 2f66 6c65 745f 636f 7265 2f75 7469 6c73  /flet_core/utils
+00000250: 2f73 6c75 6769 6679 2e70 79da 0773 6c75  /slugify.py..slu
+00000260: 6769 6679 0500 0000 7308 0000 0000 0618  gify....s.......
+00000270: ff02 0316 0172 1100 0000 2904 720b 0000  .....r....).r...
+00000280: 0072 0800 0000 da03 7374 7272 1100 0000  .r......strr....
+00000290: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+000002a0: 1000 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000002b0: 0000 7304 0000 0008 0108 03              ..s........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/strings.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/strings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 178 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 b200 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 b200 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6401 5300 2904 e900 0000  d...Z.d.S.).....
 00000050: 004e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
 00000060: 0000 0005 0000 0003 0000 0073 2800 0000  ...........s(...
 00000070: 7400 6a01 7400 6a02 1700 8900 6401 a003  t.j.t.j.....d...
@@ -10,27 +10,27 @@
 00000090: 4400 8301 a101 5300 2904 4eda 0063 0100  D.....S.).N..c..
 000000a0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 000000b0: 0000 3300 0000 7318 0000 007c 005d 107d  ..3...s....|.].}
 000000c0: 0174 00a0 0188 00a1 0156 0001 0071 0264  .t.......V...q.d
 000000d0: 0053 0029 014e 2902 da07 7365 6372 6574  .S.).N)...secret
 000000e0: 735a 0663 686f 6963 6529 02da 022e 30da  sZ.choice)....0.
 000000f0: 015f a901 5a08 616c 7068 6162 6574 a900  ._..Z.alphabet..
-00000100: fa59 2f77 6f72 6b73 7061 6365 732f 636f  .Y/workspaces/co
-00000110: 6e74 7269 6266 6c65 742f 666c 6574 2f73  ntribflet/flet/s
-00000120: 646b 2f70 7974 686f 6e2f 7061 636b 6167  dk/python/packag
-00000130: 6573 2f66 6c65 742d 636f 7265 2f73 7263  es/flet-core/src
-00000140: 2f66 6c65 745f 636f 7265 2f75 7469 6c73  /flet_core/utils
-00000150: 2f73 7472 696e 6773 2e70 79da 093c 6765  /strings.py..<ge
-00000160: 6e65 7870 723e 0700 0000 f300 0000 007a  nexpr>.........z
-00000170: 2072 616e 646f 6d5f 7374 7269 6e67 2e3c   random_string.<
-00000180: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-00000190: 3e29 05da 0673 7472 696e 67da 0d61 7363  >)...string..asc
-000001a0: 6969 5f6c 6574 7465 7273 da06 6469 6769  ii_letters..digi
-000001b0: 7473 da04 6a6f 696e da05 7261 6e67 6529  ts..join..range)
-000001c0: 01da 066c 656e 6774 6872 0700 0000 7206  ...lengthr....r.
-000001d0: 0000 0072 0800 0000 da0d 7261 6e64 6f6d  ...r......random
-000001e0: 5f73 7472 696e 6705 0000 0073 0400 0000  _string....s....
-000001f0: 0001 0c01 7211 0000 0029 0372 0300 0000  ....r....).r....
-00000200: 720b 0000 0072 1100 0000 7207 0000 0072  r....r....r....r
-00000210: 0700 0000 7207 0000 0072 0800 0000 da08  ....r....r......
-00000220: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
-00000230: 0008 0108 03                             .....
+00000100: fa60 2f77 6f72 6b73 7061 6365 732f 636f  .`/workspaces/co
+00000110: 6e74 7269 6266 6c65 742f 666c 6574 636f  ntribflet/fletco
+00000120: 6e74 7269 622f 7364 6b2f 7079 7468 6f6e  ntrib/sdk/python
+00000130: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
+00000140: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
+00000150: 652f 7574 696c 732f 7374 7269 6e67 732e  e/utils/strings.
+00000160: 7079 da09 3c67 656e 6578 7072 3e07 0000  py..<genexpr>...
+00000170: 00f3 0000 0000 7a20 7261 6e64 6f6d 5f73  ......z random_s
+00000180: 7472 696e 672e 3c6c 6f63 616c 733e 2e3c  tring.<locals>.<
+00000190: 6765 6e65 7870 723e 2905 da06 7374 7269  genexpr>)...stri
+000001a0: 6e67 da0d 6173 6369 695f 6c65 7474 6572  ng..ascii_letter
+000001b0: 73da 0664 6967 6974 73da 046a 6f69 6eda  s..digits..join.
+000001c0: 0572 616e 6765 2901 da06 6c65 6e67 7468  .range)...length
+000001d0: 7207 0000 0072 0600 0000 7208 0000 00da  r....r....r.....
+000001e0: 0d72 616e 646f 6d5f 7374 7269 6e67 0500  .random_string..
+000001f0: 0000 7304 0000 0000 010c 0172 1100 0000  ..s........r....
+00000200: 2903 7203 0000 0072 0b00 0000 7211 0000  ).r....r....r...
+00000210: 0072 0700 0000 7207 0000 0072 0700 0000  .r....r....r....
+00000220: 7208 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000230: 0000 0073 0400 0000 0801 0803            ...s........
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/__pycache__/vector.cpython-39.pyc` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/__pycache__/vector.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 16:58:02 2024 UTC, .py size: 3207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1a3a 2966 870c 0000  a........:)f....
+00000000: 610d 0d0a 0000 0000 d7d7 2f66 870c 0000  a........./f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6501 8303 5a02 6401 5300 2904 e900 0000  e...Z.d.S.).....
 00000050: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000060: 0000 0003 0000 0040 0000 0073 d200 0000  .......@...s....
 00000070: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
@@ -102,192 +102,193 @@
 00000650: 302c 2032 2e30 290a 2020 2020 67bb bdd7  0, 2.0).    g...
 00000660: d9df 7cdb 3d63 0200 0000 0000 0000 0000  ..|.=c..........
 00000670: 0000 0200 0000 0500 0000 4300 0000 7314  ..........C...s.
 00000680: 0000 0074 007c 0083 0174 01a0 027c 007c  ...t.|...t...|.|
 00000690: 01a1 0283 0153 00a9 014e 2903 da04 7479  .....S...N)...ty
 000006a0: 7065 da07 636f 6d70 6c65 78da 075f 5f61  pe..complex..__a
 000006b0: 6464 5f5f a902 da04 7365 6c66 da05 6f74  dd__....self..ot
-000006c0: 6865 72a9 0072 0a00 0000 fa58 2f77 6f72  her..r.....X/wor
+000006c0: 6865 72a9 0072 0a00 0000 fa5f 2f77 6f72  her..r....._/wor
 000006d0: 6b73 7061 6365 732f 636f 6e74 7269 6266  kspaces/contribf
-000006e0: 6c65 742f 666c 6574 2f73 646b 2f70 7974  let/flet/sdk/pyt
-000006f0: 686f 6e2f 7061 636b 6167 6573 2f66 6c65  hon/packages/fle
-00000700: 742d 636f 7265 2f73 7263 2f66 6c65 745f  t-core/src/flet_
-00000710: 636f 7265 2f75 7469 6c73 2f76 6563 746f  core/utils/vecto
-00000720: 722e 7079 da08 3c6c 616d 6264 613e 4200  r.py..<lambda>B.
-00000730: 0000 f300 0000 007a 0f56 6563 746f 722e  .......z.Vector.
-00000740: 3c6c 616d 6264 613e 6302 0000 0000 0000  <lambda>c.......
-00000750: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-00000760: 0073 1400 0000 7400 7c00 8301 7401 a002  .s....t.|...t...
-00000770: 7c00 7c01 a102 8301 5300 7203 0000 0029  |.|.....S.r....)
-00000780: 0372 0400 0000 7205 0000 00da 075f 5f73  .r....r......__s
-00000790: 7562 5f5f 7207 0000 0072 0a00 0000 720a  ub__r....r....r.
-000007a0: 0000 0072 0b00 0000 720c 0000 0043 0000  ...r....r....C..
-000007b0: 0072 0d00 0000 6302 0000 0000 0000 0000  .r....c.........
-000007c0: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-000007d0: 1400 0000 7400 7c00 8301 7401 a002 7c00  ....t.|...t...|.
-000007e0: 7c01 a102 8301 5300 7203 0000 0029 0372  |.....S.r....).r
-000007f0: 0400 0000 7205 0000 00da 075f 5f6d 756c  ....r......__mul
-00000800: 5f5f 7207 0000 0072 0a00 0000 720a 0000  __r....r....r...
-00000810: 0072 0b00 0000 720c 0000 0044 0000 0072  .r....r....D...r
-00000820: 0d00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000830: 0002 0000 0005 0000 0043 0000 0073 1400  .........C...s..
-00000840: 0000 7400 7c00 8301 7401 a002 7c00 7c01  ..t.|...t...|.|.
-00000850: a102 8301 5300 7203 0000 0029 0372 0400  ....S.r....).r..
-00000860: 0000 7205 0000 00da 0b5f 5f74 7275 6564  ..r......__trued
-00000870: 6976 5f5f 7207 0000 0072 0a00 0000 720a  iv__r....r....r.
-00000880: 0000 0072 0b00 0000 720c 0000 0045 0000  ...r....r....E..
-00000890: 0072 0d00 0000 6301 0000 0000 0000 0000  .r....c.........
-000008a0: 0000 0001 0000 0001 0000 0043 0000 0073  ...........C...s
-000008b0: 0400 0000 6401 5300 2902 4ee9 0200 0000  ....d.S.).N.....
-000008c0: 720a 0000 00a9 0172 0800 0000 720a 0000  r......r....r...
-000008d0: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-000008e0: 4600 0000 720d 0000 004e 6302 0000 0000  F...r....Nc.....
-000008f0: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
-00000900: 0000 0073 1e00 0000 7400 7c00 8301 7401  ...s....t.|...t.
-00000910: 7c00 6a02 7c01 8302 7401 7c00 6a03 7c01  |.j.|...t.|.j.|.
-00000920: 8302 8302 5300 7203 0000 0029 0472 0400  ....S.r....).r..
-00000930: 0000 da05 726f 756e 64da 0178 da01 7929  ....round..x..y)
-00000940: 0272 0800 0000 da07 6e64 6967 6974 7372  .r......ndigitsr
-00000950: 0a00 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
-00000960: 0000 0047 0000 0073 0400 0000 0601 14ff  ...G...s........
-00000970: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000980: 0005 0000 0043 0000 0073 2c00 0000 7400  .....C...s,...t.
-00000990: 6a01 7c00 6a02 7c01 6a02 7c00 6a03 6401  j.|.j.|.j.|.j.d.
-000009a0: 8d03 6f2a 7400 6a01 7c00 6a04 7c01 6a04  ..o*t.j.|.j.|.j.
-000009b0: 7c00 6a03 6401 8d03 5300 2902 4e29 01da  |.j.d...S.).N)..
-000009c0: 0761 6273 5f74 6f6c 2905 da04 6d61 7468  .abs_tol)...math
-000009d0: da07 6973 636c 6f73 6572 1400 0000 7217  ..iscloser....r.
-000009e0: 0000 0072 1500 0000 7207 0000 0072 0a00  ...r....r....r..
-000009f0: 0000 720a 0000 0072 0b00 0000 da06 5f5f  ..r....r......__
-00000a00: 6571 5f5f 4b00 0000 7306 0000 0000 011a  eq__K...s.......
-00000a10: 010c ff7a 0d56 6563 746f 722e 5f5f 6571  ...z.Vector.__eq
-00000a20: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-00000a30: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
-00000a40: 7c00 a000 7c01 a101 0c00 5300 7203 0000  |...|.....S.r...
-00000a50: 0029 0172 1a00 0000 7207 0000 0072 0a00  .).r....r....r..
-00000a60: 0000 720a 0000 0072 0b00 0000 da06 5f5f  ..r....r......__
-00000a70: 6e65 5f5f 5000 0000 7302 0000 0000 017a  ne__P...s......z
-00000a80: 0d56 6563 746f 722e 5f5f 6e65 5f5f 6301  .Vector.__ne__c.
-00000a90: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000aa0: 0000 0043 0000 0073 1000 0000 7400 7c00  ...C...s....t.|.
-00000ab0: 6a01 7c00 6a02 6702 8301 5300 7203 0000  j.|.j.g...S.r...
-00000ac0: 0029 03da 0469 7465 7272 1400 0000 7215  .)...iterr....r.
-00000ad0: 0000 0072 1200 0000 720a 0000 0072 0a00  ...r....r....r..
-00000ae0: 0000 720b 0000 00da 085f 5f69 7465 725f  ..r......__iter_
-00000af0: 5f53 0000 0073 0200 0000 0001 7a0f 5665  _S...s......z.Ve
-00000b00: 6374 6f72 2e5f 5f69 7465 725f 5f63 0100  ctor.__iter__c..
-00000b10: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000b20: 0000 4300 0000 730c 0000 0074 0074 017c  ..C...s....t.t.|
-00000b30: 0083 0183 0153 0072 0300 0000 2902 da03  .....S.r....)...
-00000b40: 7374 72da 0574 7570 6c65 7212 0000 0072  str..tupler....r
-00000b50: 0a00 0000 720a 0000 0072 0b00 0000 da07  ....r....r......
-00000b60: 5f5f 7374 725f 5f56 0000 0073 0200 0000  __str__V...s....
-00000b70: 0001 7a0e 5665 6374 6f72 2e5f 5f73 7472  ..z.Vector.__str
-00000b80: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00000b90: 0000 0003 0000 0043 0000 0073 1600 0000  .......C...s....
-00000ba0: 7400 7c00 8301 6a01 9b00 7402 7c00 8301  t.|...j...t.|...
-00000bb0: 9b00 9d02 5300 7203 0000 0029 0372 0400  ....S.r....).r..
-00000bc0: 0000 da08 5f5f 6e61 6d65 5f5f 721e 0000  ....__name__r...
-00000bd0: 0072 1200 0000 720a 0000 0072 0a00 0000  .r....r....r....
-00000be0: 720b 0000 00da 085f 5f72 6570 725f 5f59  r......__repr__Y
-00000bf0: 0000 0073 0200 0000 0001 7a0f 5665 6374  ...s......z.Vect
-00000c00: 6f72 2e5f 5f72 6570 725f 5f63 0300 0000  or.__repr__c....
-00000c10: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-00000c20: 4300 0000 732a 0000 007c 0074 0074 01a0  C...s*...|.t.t..
-00000c30: 027c 01a1 017c 0214 0064 0183 0274 0074  .|...|...d...t.t
-00000c40: 01a0 037c 01a1 017c 0214 0064 0183 0283  ...|...|...d....
-00000c50: 0253 0029 024e e90a 0000 0029 0472 1300  .S.).N.....).r..
-00000c60: 0000 7218 0000 00da 0363 6f73 da03 7369  ..r......cos..si
-00000c70: 6e29 03da 0363 6c73 da07 7261 6469 616e  n)...cls..radian
-00000c80: 73da 096d 6167 6e69 7475 6465 720a 0000  s..magnituder...
-00000c90: 0072 0a00 0000 720b 0000 00da 0570 6f6c  .r....r......pol
-00000ca0: 6172 5c00 0000 7308 0000 0000 0202 0112  ar\...s.........
-00000cb0: 0112 fe7a 0c56 6563 746f 722e 706f 6c61  ...z.Vector.pola
-00000cc0: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
-00000cd0: 0000 0200 0000 4300 0000 7308 0000 0074  ......C...s....t
-00000ce0: 007c 0083 0153 0072 0300 0000 a901 da03  .|...S.r........
-00000cf0: 6162 7372 1200 0000 720a 0000 0072 0a00  absr....r....r..
-00000d00: 0000 720b 0000 0072 2800 0000 6300 0000  ..r....r(...c...
-00000d10: 7302 0000 0000 027a 1056 6563 746f 722e  s......z.Vector.
-00000d20: 6d61 676e 6974 7564 6563 0100 0000 0000  magnitudec......
-00000d30: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000d40: 0000 730c 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
-00000d50: 0153 0072 0300 0000 2903 7218 0000 00da  .S.r....).r.....
-00000d60: 0764 6567 7265 6573 7227 0000 0072 1200  .degreesr'...r..
-00000d70: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000d80: 0072 2c00 0000 6700 0000 7302 0000 0000  .r,...g...s.....
-00000d90: 027a 0e56 6563 746f 722e 6465 6772 6565  .z.Vector.degree
-00000da0: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-00000db0: 0000 0400 0000 4300 0000 7310 0000 0074  ......C...s....t
-00000dc0: 00a0 017c 006a 027c 006a 03a1 0253 0072  ...|.j.|.j...S.r
-00000dd0: 0300 0000 2904 7218 0000 00da 0561 7461  ....).r......ata
-00000de0: 6e32 7215 0000 0072 1400 0000 7212 0000  n2r....r....r...
-00000df0: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000e00: 7227 0000 006b 0000 0073 0200 0000 0002  r'...k...s......
-00000e10: 7a0e 5665 6374 6f72 2e72 6164 6961 6e73  z.Vector.radians
-00000e20: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000e30: 0003 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
-00000e40: 7c00 8301 7c01 7c00 6a01 8302 5300 7203  |...|.|.j...S.r.
-00000e50: 0000 0029 0272 0400 0000 7215 0000 00a9  ...).r....r.....
-00000e60: 0272 0800 0000 da05 7661 6c75 6572 0a00  .r......valuer..
-00000e70: 0000 720a 0000 0072 0b00 0000 da06 7769  ..r....r......wi
-00000e80: 7468 5f78 6f00 0000 7302 0000 0000 017a  th_xo...s......z
-00000e90: 0d56 6563 746f 722e 7769 7468 5f78 6302  .Vector.with_xc.
-00000ea0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000eb0: 0000 0043 0000 0073 1000 0000 7400 7c00  ...C...s....t.|.
-00000ec0: 8301 7c00 6a01 7c01 8302 5300 7203 0000  ..|.j.|...S.r...
-00000ed0: 0029 0272 0400 0000 7214 0000 0072 2e00  .).r....r....r..
-00000ee0: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000ef0: 00da 0677 6974 685f 7972 0000 0073 0200  ...with_yr...s..
-00000f00: 0000 0001 7a0d 5665 6374 6f72 2e77 6974  ....z.Vector.wit
-00000f10: 685f 7963 0200 0000 0000 0000 0000 0000  h_yc............
-00000f20: 0200 0000 0300 0000 4300 0000 7310 0000  ........C...s...
-00000f30: 007c 007c 0114 0074 007c 0083 011b 0053  .|.|...t.|.....S
-00000f40: 0072 0300 0000 722a 0000 0072 2e00 0000  .r....r*...r....
-00000f50: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000f60: 0e77 6974 685f 6d61 676e 6974 7564 6575  .with_magnitudeu
-00000f70: 0000 0073 0200 0000 0001 7a15 5665 6374  ...s......z.Vect
-00000f80: 6f72 2e77 6974 685f 6d61 676e 6974 7564  or.with_magnitud
-00000f90: 6563 0200 0000 0000 0000 0000 0000 0300  ec..............
-00000fa0: 0000 0400 0000 4300 0000 7318 0000 0074  ......C...s....t
-00000fb0: 007c 0083 017d 0274 017c 0083 01a0 027c  .|...}.t.|.....|
-00000fc0: 017c 02a1 0253 0072 0300 0000 2903 722b  .|...S.r....).r+
-00000fd0: 0000 0072 0400 0000 7229 0000 0029 0372  ...r....r)...).r
-00000fe0: 0800 0000 722f 0000 0072 2800 0000 720a  ....r/...r(...r.
-00000ff0: 0000 0072 0a00 0000 720b 0000 00da 0c77  ...r....r......w
-00001000: 6974 685f 7261 6469 616e 7378 0000 0073  ith_radiansx...s
-00001010: 0400 0000 0001 0801 7a13 5665 6374 6f72  ........z.Vector
-00001020: 2e77 6974 685f 7261 6469 616e 7363 0200  .with_radiansc..
-00001030: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-00001040: 0000 4300 0000 7322 0000 0074 00a0 017c  ..C...s"...t...|
-00001050: 01a1 017d 0274 027c 0083 017d 0374 037c  ...}.t.|...}.t.|
-00001060: 0083 01a0 047c 027c 03a1 0253 0072 0300  .....|.|...S.r..
-00001070: 0000 2905 7218 0000 0072 2700 0000 722b  ..).r....r'...r+
-00001080: 0000 0072 0400 0000 7229 0000 0029 0472  ...r....r)...).r
-00001090: 0800 0000 722f 0000 0072 2700 0000 7228  ....r/...r'...r(
-000010a0: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
-000010b0: 0000 da0c 7769 7468 5f64 6567 7265 6573  ....with_degrees
-000010c0: 7c00 0000 7306 0000 0000 010a 0108 017a  |...s..........z
-000010d0: 1356 6563 746f 722e 7769 7468 5f64 6567  .Vector.with_deg
-000010e0: 7265 6573 2901 4e29 2072 2100 0000 da0a  rees).N) r!.....
-000010f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00001100: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00001110: 5f72 1700 0000 7205 0000 00da 0472 6561  _r....r......rea
-00001120: 6c72 1400 0000 da04 696d 6167 7215 0000  lr......imagr...
-00001130: 0072 0600 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00001140: 7210 0000 00da 075f 5f6c 656e 5f5f da09  r......__len__..
-00001150: 5f5f 726f 756e 645f 5f72 1a00 0000 721b  __round__r....r.
-00001160: 0000 0072 1d00 0000 7220 0000 0072 2200  ...r....r ...r".
-00001170: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
-00001180: 2900 0000 da08 7072 6f70 6572 7479 7228  ).....propertyr(
-00001190: 0000 0072 2c00 0000 7227 0000 0072 3000  ...r,...r'...r0.
-000011a0: 0000 7231 0000 0072 3200 0000 7233 0000  ..r1...r2...r3..
-000011b0: 0072 3400 0000 720a 0000 0072 0a00 0000  .r4...r....r....
-000011c0: 720a 0000 0072 0b00 0000 7202 0000 0004  r....r....r.....
-000011d0: 0000 0073 3800 0000 0801 0439 0402 0601  ...s8......9....
-000011e0: 0601 0801 0801 0801 0801 0801 0a04 0805  ................
-000011f0: 0803 0803 0803 0803 0201 0a06 0201 0a03  ................
-00001200: 0201 0a03 0201 0a03 0803 0803 0803 0804  ................
-00001210: 7202 0000 0029 0372 1800 0000 7205 0000  r....).r....r...
-00001220: 0072 0200 0000 720a 0000 0072 0a00 0000  .r....r....r....
-00001230: 720a 0000 0072 0b00 0000 da08 3c6d 6f64  r....r......<mod
-00001240: 756c 653e 0100 0000 7302 0000 0008 03    ule>....s......
+000006e0: 6c65 742f 666c 6574 636f 6e74 7269 622f  let/fletcontrib/
+000006f0: 7364 6b2f 7079 7468 6f6e 2f70 6163 6b61  sdk/python/packa
+00000700: 6765 732f 666c 6574 2d63 6f72 652f 7372  ges/flet-core/sr
+00000710: 632f 666c 6574 5f63 6f72 652f 7574 696c  c/flet_core/util
+00000720: 732f 7665 6374 6f72 2e70 79da 083c 6c61  s/vector.py..<la
+00000730: 6d62 6461 3e42 0000 00f3 0000 0000 7a0f  mbda>B........z.
+00000740: 5665 6374 6f72 2e3c 6c61 6d62 6461 3e63  Vector.<lambda>c
+00000750: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000760: 0500 0000 4300 0000 7314 0000 0074 007c  ....C...s....t.|
+00000770: 0083 0174 01a0 027c 007c 01a1 0283 0153  ...t...|.|.....S
+00000780: 0072 0300 0000 2903 7204 0000 0072 0500  .r....).r....r..
+00000790: 0000 da07 5f5f 7375 625f 5f72 0700 0000  ....__sub__r....
+000007a0: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+000007b0: 0c00 0000 4300 0000 720d 0000 0063 0200  ....C...r....c..
+000007c0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+000007d0: 0000 4300 0000 7314 0000 0074 007c 0083  ..C...s....t.|..
+000007e0: 0174 01a0 027c 007c 01a1 0283 0153 0072  .t...|.|.....S.r
+000007f0: 0300 0000 2903 7204 0000 0072 0500 0000  ....).r....r....
+00000800: da07 5f5f 6d75 6c5f 5f72 0700 0000 720a  ..__mul__r....r.
+00000810: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+00000820: 0000 4400 0000 720d 0000 0063 0200 0000  ..D...r....c....
+00000830: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00000840: 4300 0000 7314 0000 0074 007c 0083 0174  C...s....t.|...t
+00000850: 01a0 027c 007c 01a1 0283 0153 0072 0300  ...|.|.....S.r..
+00000860: 0000 2903 7204 0000 0072 0500 0000 da0b  ..).r....r......
+00000870: 5f5f 7472 7565 6469 765f 5f72 0700 0000  __truediv__r....
+00000880: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+00000890: 0c00 0000 4500 0000 720d 0000 0063 0100  ....E...r....c..
+000008a0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000008b0: 0000 4300 0000 7304 0000 0064 0153 0029  ..C...s....d.S.)
+000008c0: 024e e902 0000 0072 0a00 0000 a901 7208  .N.....r......r.
+000008d0: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
+000008e0: 0000 720c 0000 0046 0000 0072 0d00 0000  ..r....F...r....
+000008f0: 4e63 0200 0000 0000 0000 0000 0000 0200  Nc..............
+00000900: 0000 0500 0000 4300 0000 731e 0000 0074  ......C...s....t
+00000910: 007c 0083 0174 017c 006a 027c 0183 0274  .|...t.|.j.|...t
+00000920: 017c 006a 037c 0183 0283 0253 0072 0300  .|.j.|.....S.r..
+00000930: 0000 2904 7204 0000 00da 0572 6f75 6e64  ..).r......round
+00000940: da01 78da 0179 2902 7208 0000 00da 076e  ..x..y).r......n
+00000950: 6469 6769 7473 720a 0000 0072 0a00 0000  digitsr....r....
+00000960: 720b 0000 0072 0c00 0000 4700 0000 7304  r....r....G...s.
+00000970: 0000 0006 0114 ff63 0200 0000 0000 0000  .......c........
+00000980: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+00000990: 732c 0000 0074 006a 017c 006a 027c 016a  s,...t.j.|.j.|.j
+000009a0: 027c 006a 0364 018d 036f 2a74 006a 017c  .|.j.d...o*t.j.|
+000009b0: 006a 047c 016a 047c 006a 0364 018d 0353  .j.|.j.|.j.d...S
+000009c0: 0029 024e 2901 da07 6162 735f 746f 6c29  .).N)...abs_tol)
+000009d0: 05da 046d 6174 68da 0769 7363 6c6f 7365  ...math..isclose
+000009e0: 7214 0000 0072 1700 0000 7215 0000 0072  r....r....r....r
+000009f0: 0700 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00000a00: 0000 00da 065f 5f65 715f 5f4b 0000 0073  .....__eq__K...s
+00000a10: 0600 0000 0001 1a01 0cff 7a0d 5665 6374  ..........z.Vect
+00000a20: 6f72 2e5f 5f65 715f 5f63 0200 0000 0000  or.__eq__c......
+00000a30: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000a40: 0000 730c 0000 007c 00a0 007c 01a1 010c  ..s....|...|....
+00000a50: 0053 0072 0300 0000 2901 721a 0000 0072  .S.r....).r....r
+00000a60: 0700 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+00000a70: 0000 00da 065f 5f6e 655f 5f50 0000 0073  .....__ne__P...s
+00000a80: 0200 0000 0001 7a0d 5665 6374 6f72 2e5f  ......z.Vector._
+00000a90: 5f6e 655f 5f63 0100 0000 0000 0000 0000  _ne__c..........
+00000aa0: 0000 0100 0000 0300 0000 4300 0000 7310  ..........C...s.
+00000ab0: 0000 0074 007c 006a 017c 006a 0267 0283  ...t.|.j.|.j.g..
+00000ac0: 0153 0072 0300 0000 2903 da04 6974 6572  .S.r....)...iter
+00000ad0: 7214 0000 0072 1500 0000 7212 0000 0072  r....r....r....r
+00000ae0: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
+00000af0: 5f5f 6974 6572 5f5f 5300 0000 7302 0000  __iter__S...s...
+00000b00: 0000 017a 0f56 6563 746f 722e 5f5f 6974  ...z.Vector.__it
+00000b10: 6572 5f5f 6301 0000 0000 0000 0000 0000  er__c...........
+00000b20: 0001 0000 0003 0000 0043 0000 0073 0c00  .........C...s..
+00000b30: 0000 7400 7401 7c00 8301 8301 5300 7203  ..t.t.|.....S.r.
+00000b40: 0000 0029 02da 0373 7472 da05 7475 706c  ...)...str..tupl
+00000b50: 6572 1200 0000 720a 0000 0072 0a00 0000  er....r....r....
+00000b60: 720b 0000 00da 075f 5f73 7472 5f5f 5600  r......__str__V.
+00000b70: 0000 7302 0000 0000 017a 0e56 6563 746f  ..s......z.Vecto
+00000b80: 722e 5f5f 7374 725f 5f63 0100 0000 0000  r.__str__c......
+00000b90: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000ba0: 0000 7316 0000 0074 007c 0083 016a 019b  ..s....t.|...j..
+00000bb0: 0074 027c 0083 019b 009d 0253 0072 0300  .t.|.......S.r..
+00000bc0: 0000 2903 7204 0000 00da 085f 5f6e 616d  ..).r......__nam
+00000bd0: 655f 5f72 1e00 0000 7212 0000 0072 0a00  e__r....r....r..
+00000be0: 0000 720a 0000 0072 0b00 0000 da08 5f5f  ..r....r......__
+00000bf0: 7265 7072 5f5f 5900 0000 7302 0000 0000  repr__Y...s.....
+00000c00: 017a 0f56 6563 746f 722e 5f5f 7265 7072  .z.Vector.__repr
+00000c10: 5f5f 6303 0000 0000 0000 0000 0000 0003  __c.............
+00000c20: 0000 0006 0000 0043 0000 0073 2a00 0000  .......C...s*...
+00000c30: 7c00 7400 7401 a002 7c01 a101 7c02 1400  |.t.t...|...|...
+00000c40: 6401 8302 7400 7401 a003 7c01 a101 7c02  d...t.t...|...|.
+00000c50: 1400 6401 8302 8302 5300 2902 4ee9 0a00  ..d.....S.).N...
+00000c60: 0000 2904 7213 0000 0072 1800 0000 da03  ..).r....r......
+00000c70: 636f 73da 0373 696e 2903 da03 636c 73da  cos..sin)...cls.
+00000c80: 0772 6164 6961 6e73 da09 6d61 676e 6974  .radians..magnit
+00000c90: 7564 6572 0a00 0000 720a 0000 0072 0b00  uder....r....r..
+00000ca0: 0000 da05 706f 6c61 725c 0000 0073 0800  ....polar\...s..
+00000cb0: 0000 0002 0201 1201 12fe 7a0c 5665 6374  ..........z.Vect
+00000cc0: 6f72 2e70 6f6c 6172 6301 0000 0000 0000  or.polarc.......
+00000cd0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00000ce0: 0073 0800 0000 7400 7c00 8301 5300 7203  .s....t.|...S.r.
+00000cf0: 0000 00a9 01da 0361 6273 7212 0000 0072  .......absr....r
+00000d00: 0a00 0000 720a 0000 0072 0b00 0000 7228  ....r....r....r(
+00000d10: 0000 0063 0000 0073 0200 0000 0002 7a10  ...c...s......z.
+00000d20: 5665 6374 6f72 2e6d 6167 6e69 7475 6465  Vector.magnitude
+00000d30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000d40: 0003 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
+00000d50: a001 7c00 6a02 a101 5300 7203 0000 0029  ..|.j...S.r....)
+00000d60: 0372 1800 0000 da07 6465 6772 6565 7372  .r......degreesr
+00000d70: 2700 0000 7212 0000 0072 0a00 0000 720a  '...r....r....r.
+00000d80: 0000 0072 0b00 0000 722c 0000 0067 0000  ...r....r,...g..
+00000d90: 0073 0200 0000 0002 7a0e 5665 6374 6f72  .s......z.Vector
+00000da0: 2e64 6567 7265 6573 6301 0000 0000 0000  .degreesc.......
+00000db0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00000dc0: 0073 1000 0000 7400 a001 7c00 6a02 7c00  .s....t...|.j.|.
+00000dd0: 6a03 a102 5300 7203 0000 0029 0472 1800  j...S.r....).r..
+00000de0: 0000 da05 6174 616e 3272 1500 0000 7214  ....atan2r....r.
+00000df0: 0000 0072 1200 0000 720a 0000 0072 0a00  ...r....r....r..
+00000e00: 0000 720b 0000 0072 2700 0000 6b00 0000  ..r....r'...k...
+00000e10: 7302 0000 0000 027a 0e56 6563 746f 722e  s......z.Vector.
+00000e20: 7261 6469 616e 7363 0200 0000 0000 0000  radiansc........
+00000e30: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00000e40: 7310 0000 0074 007c 0083 017c 017c 006a  s....t.|...|.|.j
+00000e50: 0183 0253 0072 0300 0000 2902 7204 0000  ...S.r....).r...
+00000e60: 0072 1500 0000 a902 7208 0000 00da 0576  .r......r......v
+00000e70: 616c 7565 720a 0000 0072 0a00 0000 720b  aluer....r....r.
+00000e80: 0000 00da 0677 6974 685f 786f 0000 0073  .....with_xo...s
+00000e90: 0200 0000 0001 7a0d 5665 6374 6f72 2e77  ......z.Vector.w
+00000ea0: 6974 685f 7863 0200 0000 0000 0000 0000  ith_xc..........
+00000eb0: 0000 0200 0000 0300 0000 4300 0000 7310  ..........C...s.
+00000ec0: 0000 0074 007c 0083 017c 006a 017c 0183  ...t.|...|.j.|..
+00000ed0: 0253 0072 0300 0000 2902 7204 0000 0072  .S.r....).r....r
+00000ee0: 1400 0000 722e 0000 0072 0a00 0000 720a  ....r....r....r.
+00000ef0: 0000 0072 0b00 0000 da06 7769 7468 5f79  ...r......with_y
+00000f00: 7200 0000 7302 0000 0000 017a 0d56 6563  r...s......z.Vec
+00000f10: 746f 722e 7769 7468 5f79 6302 0000 0000  tor.with_yc.....
+00000f20: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000f30: 0000 0073 1000 0000 7c00 7c01 1400 7400  ...s....|.|...t.
+00000f40: 7c00 8301 1b00 5300 7203 0000 0072 2a00  |.....S.r....r*.
+00000f50: 0000 722e 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+00000f60: 0072 0b00 0000 da0e 7769 7468 5f6d 6167  .r......with_mag
+00000f70: 6e69 7475 6465 7500 0000 7302 0000 0000  nitudeu...s.....
+00000f80: 017a 1556 6563 746f 722e 7769 7468 5f6d  .z.Vector.with_m
+00000f90: 6167 6e69 7475 6465 6302 0000 0000 0000  agnitudec.......
+00000fa0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000fb0: 0073 1800 0000 7400 7c00 8301 7d02 7401  .s....t.|...}.t.
+00000fc0: 7c00 8301 a002 7c01 7c02 a102 5300 7203  |.....|.|...S.r.
+00000fd0: 0000 0029 0372 2b00 0000 7204 0000 0072  ...).r+...r....r
+00000fe0: 2900 0000 2903 7208 0000 0072 2f00 0000  )...).r....r/...
+00000ff0: 7228 0000 0072 0a00 0000 720a 0000 0072  r(...r....r....r
+00001000: 0b00 0000 da0c 7769 7468 5f72 6164 6961  ......with_radia
+00001010: 6e73 7800 0000 7304 0000 0000 0108 017a  nsx...s........z
+00001020: 1356 6563 746f 722e 7769 7468 5f72 6164  .Vector.with_rad
+00001030: 6961 6e73 6302 0000 0000 0000 0000 0000  iansc...........
+00001040: 0004 0000 0004 0000 0043 0000 0073 2200  .........C...s".
+00001050: 0000 7400 a001 7c01 a101 7d02 7402 7c00  ..t...|...}.t.|.
+00001060: 8301 7d03 7403 7c00 8301 a004 7c02 7c03  ..}.t.|.....|.|.
+00001070: a102 5300 7203 0000 0029 0572 1800 0000  ..S.r....).r....
+00001080: 7227 0000 0072 2b00 0000 7204 0000 0072  r'...r+...r....r
+00001090: 2900 0000 2904 7208 0000 0072 2f00 0000  )...).r....r/...
+000010a0: 7227 0000 0072 2800 0000 720a 0000 0072  r'...r(...r....r
+000010b0: 0a00 0000 720b 0000 00da 0c77 6974 685f  ....r......with_
+000010c0: 6465 6772 6565 737c 0000 0073 0600 0000  degrees|...s....
+000010d0: 0001 0a01 0801 7a13 5665 6374 6f72 2e77  ......z.Vector.w
+000010e0: 6974 685f 6465 6772 6565 7329 014e 2920  ith_degrees).N) 
+000010f0: 7221 0000 00da 0a5f 5f6d 6f64 756c 655f  r!.....__module_
+00001100: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00001110: 075f 5f64 6f63 5f5f 7217 0000 0072 0500  .__doc__r....r..
+00001120: 0000 da04 7265 616c 7214 0000 00da 0469  ....realr......i
+00001130: 6d61 6772 1500 0000 7206 0000 0072 0e00  magr....r....r..
+00001140: 0000 720f 0000 0072 1000 0000 da07 5f5f  ..r....r......__
+00001150: 6c65 6e5f 5fda 095f 5f72 6f75 6e64 5f5f  len__..__round__
+00001160: 721a 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
+00001170: 2000 0000 7222 0000 00da 0b63 6c61 7373   ...r".....class
+00001180: 6d65 7468 6f64 7229 0000 00da 0870 726f  methodr).....pro
+00001190: 7065 7274 7972 2800 0000 722c 0000 0072  pertyr(...r,...r
+000011a0: 2700 0000 7230 0000 0072 3100 0000 7232  '...r0...r1...r2
+000011b0: 0000 0072 3300 0000 7234 0000 0072 0a00  ...r3...r4...r..
+000011c0: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+000011d0: 0072 0200 0000 0400 0000 7338 0000 0008  .r........s8....
+000011e0: 0104 3904 0206 0106 0108 0108 0108 0108  ..9.............
+000011f0: 0108 010a 0408 0508 0308 0308 0308 0302  ................
+00001200: 010a 0602 010a 0302 010a 0302 010a 0308  ................
+00001210: 0308 0308 0308 0472 0200 0000 2903 7218  .......r....).r.
+00001220: 0000 0072 0500 0000 7202 0000 0072 0a00  ...r....r....r..
+00001230: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00001240: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001250: 0200 0000 0803                           ......
```

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/deprecated.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/utils/vector.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/utils/vector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/vertical_divider.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/video.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/video.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/view.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/webview.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/webview.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/src/flet_core/window_drag_area.py` & `flet_contrib_core-2024.5.2.1633/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.4.28.2241/PKG-INFO` & `flet_contrib_core-2024.5.2.1633/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-contrib-core
-Version: 2024.4.28.2241
+Version: 2024.5.2.1633
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

