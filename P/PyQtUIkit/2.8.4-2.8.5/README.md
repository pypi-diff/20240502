# Comparing `tmp/PyQtUIkit-2.8.4.tar.gz` & `tmp/PyQtUIkit-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.8.4.tar", last modified: Tue Apr 30 08:46:41 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.8.5.tar", last modified: Thu May  2 16:47:32 2024, max compression
```

## Comparing `PyQtUIkit-2.8.4.tar` & `PyQtUIkit-2.8.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.387046 PyQtUIkit-2.8.4/
--rw-rw-rw-   0        0        0     1090 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-30 08:46:41.387046 PyQtUIkit-2.8.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.355798 PyQtUIkit-2.8.4/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3271 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.355798 PyQtUIkit-2.8.4/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.355798 PyQtUIkit-2.8.4/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.371422 PyQtUIkit-2.8.4/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.371422 PyQtUIkit-2.8.4/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     4222 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1830 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/themes/locale.py
--rw-rw-rw-   0        0        0     1470 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.387046 PyQtUIkit-2.8.4/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1734 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3304 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     8034 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2794 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    11424 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8328 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5876 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/form.py
--rw-rw-rw-   0        0        0     4350 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/grid_layout.py
--rw-rw-rw-   0        0        0     2280 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     1578 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     5436 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/layout.py
--rw-rw-rw-   0        0        0     1697 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3671 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     4253 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4948 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7145 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6805 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     4021 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    14123 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1313 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/tabs_layout.py
--rw-rw-rw-   0        0        0     4538 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    17878 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/PyQtUIkit/widgets/tree_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:46:41.355798 PyQtUIkit-2.8.4/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-30 08:46:41.000000 PyQtUIkit-2.8.4/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2024-04-30 08:46:41.000000 PyQtUIkit-2.8.4/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:46:41.000000 PyQtUIkit-2.8.4/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-04-30 08:46:41.000000 PyQtUIkit-2.8.4/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-04-30 08:46:41.000000 PyQtUIkit-2.8.4/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 08:46:41.000000 PyQtUIkit-2.8.4/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 08:46:41.387046 PyQtUIkit-2.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-04-30 08:45:47.000000 PyQtUIkit-2.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.377640 PyQtUIkit-2.8.5/
+-rw-rw-rw-   0        0        0     1090 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-05-02 16:47:32.377640 PyQtUIkit-2.8.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.330305 PyQtUIkit-2.8.5/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3271 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.345925 PyQtUIkit-2.8.5/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.345925 PyQtUIkit-2.8.5/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.362114 PyQtUIkit-2.8.5/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.362114 PyQtUIkit-2.8.5/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     4222 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1830 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/themes/locale.py
+-rw-rw-rw-   0        0        0     1470 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.377640 PyQtUIkit-2.8.5/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1734 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3304 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     8034 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2794 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    11424 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8328 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5876 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/form.py
+-rw-rw-rw-   0        0        0     4350 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/grid_layout.py
+-rw-rw-rw-   0        0        0     2280 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     1578 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     5436 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/layout.py
+-rw-rw-rw-   0        0        0     1697 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3671 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4948 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7471 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6805 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     4021 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    14123 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1313 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/tabs_layout.py
+-rw-rw-rw-   0        0        0     4538 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    17878 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/PyQtUIkit/widgets/tree_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-02 16:47:32.330305 PyQtUIkit-2.8.5/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-05-02 16:47:32.000000 PyQtUIkit-2.8.5/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2024-05-02 16:47:32.000000 PyQtUIkit-2.8.5/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 16:47:32.000000 PyQtUIkit-2.8.5/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-02 16:47:32.000000 PyQtUIkit-2.8.5/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-02 16:47:32.000000 PyQtUIkit-2.8.5/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 16:47:32.000000 PyQtUIkit-2.8.5/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 16:47:32.377640 PyQtUIkit-2.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-05-02 16:46:43.000000 PyQtUIkit-2.8.5/setup.py
```

### Comparing `PyQtUIkit-2.8.4/LICENSE` & `PyQtUIkit-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PKG-INFO` & `PyQtUIkit-2.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.8.4
+Version: 2.8.5
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/_icons.py` & `PyQtUIkit-2.8.5/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/_translate.py` & `PyQtUIkit-2.8.5/PyQtUIkit/_translate.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.8.5/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.8.5/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.8.5/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/core/font.py` & `PyQtUIkit-2.8.5/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.8.5/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.8.5/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.8.5/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.8.5/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.8.5/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.8.5/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/themes/locale.py` & `PyQtUIkit-2.8.5/PyQtUIkit/themes/locale.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.8.5/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.8.5/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/form.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/grid_layout.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/grid_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/layout.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/navigation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from PyQt6.QtCore import Qt, QPropertyAnimation, QEasingCurve, pyqtSignal
 from PyQt6.QtGui import QFontMetrics
 from PyQt6.QtWidgets import QLabel, QPushButton, QHBoxLayout, QSizePolicy
 
 from PyQtUIkit.core.icon import KitIcon
-from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty
+from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty, TextProperty
 from PyQtUIkit.widgets import KitVBoxLayout, KitIconButton, KitIconWidget
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitNavigationButton(QPushButton, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     icon = IconProperty('icon')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    text = TextProperty('text')
 
     selected = pyqtSignal()
 
     def __init__(self, text='', icon=None):
         super().__init__()
+        self._text = text
+        self._main_palette = 'Main'
         self.__widgets = []
         self._radius = 4
         self._size = 30
         self.setCheckable(True)
         self.clicked.connect(self._on_clicked)
         self.setCursor(Qt.CursorShape.PointingHandCursor)
 
@@ -31,15 +34,15 @@
         self.__layout.setSpacing(4)
         self.setLayout(self.__layout)
 
         self.__icon = KitIconWidget()
         self.__icon._use_text_only = False
         self.__layout.addWidget(self.__icon)
 
-        self.__label = QLabel(text)
+        self.__label = QLabel()
         self.__layout.addWidget(self.__label)
 
         self._icon = icon
         self._set_expanded(False)
 
     def _on_clicked(self, flag):
         if not flag:
@@ -83,14 +86,17 @@
 QPushButton::checked {{
     background-color: {self.main_palette.selected};
 }}""")
         self.__label.setStyleSheet(f"color: {self.main_palette.text}; border: none; background-color: transparent")
         if self.icon is not None:
             self.__icon.icon = self.icon
 
+    def _apply_lang(self):
+        self.__label.setText(self.text)
+
 
 class KitNavigation(KitVBoxLayout):
     button_size = IntProperty('button_size', 30)
     button_radius = IntProperty('button_radius', 4)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
@@ -191,7 +197,13 @@
         for el in self.__tabs:
             el.main_palette = self.main_palette
             el.font = self.font
             el.font_size = self.font_size
             el._size = self.button_size
             el._radius = self.button_radius
         super()._apply_theme()
+
+    def _apply_lang(self):
+        for el in self.__tabs:
+            el._apply_lang()
+        if self.__expanded:
+            self.expand()
```

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/tabs_layout.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/tabs_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.8.5/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.8.5/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.8.4
+Version: 2.8.5
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.8.4/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.8.5/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.8.4/setup.py` & `PyQtUIkit-2.8.5/setup.py`

 * *Files identical despite different names*

