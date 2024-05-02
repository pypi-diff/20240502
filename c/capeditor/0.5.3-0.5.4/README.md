# Comparing `tmp/capeditor-0.5.3.tar.gz` & `tmp/capeditor-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.5.3.tar", last modified: Mon Apr 29 12:44:58 2024, max compression
+gzip compressed data, was "capeditor-0.5.4.tar", last modified: Thu May  2 08:13:10 2024, max compression
```

## Comparing `capeditor-0.5.3.tar` & `capeditor-0.5.4.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-29 12:44:50.000000 capeditor-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-29 12:44:58.094514 capeditor-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-29 12:44:50.000000 capeditor-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    28279 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/cap_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/caputils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/capimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.070514 capeditor-0.5.3/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.070514 capeditor-0.5.3/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.078514 capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0002_alter_capsetting_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0003_capsetting_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0004_predefinedalertarea.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/0005_alter_capsetting_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/cap_detail_page.css
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/import_cap_preview.css
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/mapbox-gl-draw.css
--rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.082514 capeditor-0.5.3/capeditor/static/capeditor/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.090514 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.090514 capeditor-0.5.3/capeditor/static/capeditor/images/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/alert.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/area.png
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/certainty.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/extreme.png
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/minor.png
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/moderate.png
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/severe.png
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/images/urgency.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.090514 capeditor-0.5.3/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/mapbox-gl-draw.js
--rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/turf.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.074514 capeditor-0.5.3/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/load_cap_alert.html
--rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/preview_cap_alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-29 12:44:50.000000 capeditor-0.5.3/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:44:58.094514 capeditor-0.5.3/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 12:44:58.000000 capeditor-0.5.3/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 12:44:50.000000 capeditor-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-29 12:44:58.094514 capeditor-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.591057 capeditor-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 08:13:06.000000 capeditor-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-02 08:13:10.591057 capeditor-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-02 08:13:06.000000 capeditor-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.571057 capeditor-0.5.4/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/cap_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/caputils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.571057 capeditor-0.5.4/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/forms/capimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.567057 capeditor-0.5.4/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.563057 capeditor-0.5.4/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.571057 capeditor-0.5.4/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.563057 capeditor-0.5.4/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.575057 capeditor-0.5.4/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.563057 capeditor-0.5.4/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.575057 capeditor-0.5.4/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.563057 capeditor-0.5.4/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.575057 capeditor-0.5.4/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.563057 capeditor-0.5.4/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.575057 capeditor-0.5.4/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.567057 capeditor-0.5.4/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.575057 capeditor-0.5.4/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.575057 capeditor-0.5.4/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/migrations/0002_alter_capsetting_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/migrations/0003_capsetting_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/migrations/0004_predefinedalertarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/migrations/0005_alter_capsetting_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16379 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.575057 capeditor-0.5.4/capeditor/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/pubsub/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/pubsub/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.567057 capeditor-0.5.4/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.567057 capeditor-0.5.4/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.579057 capeditor-0.5.4/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/cap_detail_page.css
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/import_cap_preview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/mapbox-gl-draw.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.579057 capeditor-0.5.4/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.579057 capeditor-0.5.4/capeditor/static/capeditor/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.583057 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.583057 capeditor-0.5.4/capeditor/static/capeditor/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/area.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/certainty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/extreme.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/minor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/moderate.png
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/severe.png
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/images/urgency.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.587057 capeditor-0.5.4/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/mapbox-gl-draw.js
+-rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/turf.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.587057 capeditor-0.5.4/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.567057 capeditor-0.5.4/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.587057 capeditor-0.5.4/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.591057 capeditor-0.5.4/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/icons/cap-alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/load_cap_alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/preview_cap_alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.591057 capeditor-0.5.4/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-02 08:13:06.000000 capeditor-0.5.4/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:13:10.591057 capeditor-0.5.4/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-02 08:13:10.000000 capeditor-0.5.4/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-02 08:13:10.000000 capeditor-0.5.4/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:13:10.000000 capeditor-0.5.4/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-02 08:13:10.000000 capeditor-0.5.4/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 08:13:10.000000 capeditor-0.5.4/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 08:13:06.000000 capeditor-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-02 08:13:10.591057 capeditor-0.5.4/setup.cfg
```

### Comparing `capeditor-0.5.3/PKG-INFO` & `capeditor-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.3
+Version: 0.5.4
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.5.3/README.md` & `capeditor-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/blocks.py` & `capeditor-0.5.4/capeditor/blocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 
 import shapely
 from django import forms
 from django.contrib.gis.geos import GEOSGeometry
+from django.core.exceptions import ValidationError
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from shapely import Point, Polygon
 from shapely.geometry import shape
 from wagtail import blocks
-from wagtail.blocks import FieldBlock, StructValue
+from wagtail.blocks import FieldBlock, StructValue, StructBlockValidationError
 from wagtail.documents.blocks import DocumentChooserBlock
 from wagtail.models import Site
 from wagtailmodelchooser.blocks import ModelChooserBlock
 
 from .forms.fields import PolygonField, MultiPolygonField, BoundaryMultiPolygonField, PolygonOrMultiPolygonField
 from .forms.widgets import CircleWidget
+from .serializers import parse_tz
 from .utils import file_path_mime
 
 
 class BoundaryFieldBlock(FieldBlock):
     def __init__(self, required=True, help_text=None, srid=4326, **kwargs):
         self.field_options = {
             "required": required,
@@ -111,17 +113,17 @@
     address = blocks.TextBlock(label=_("Address"), help_text=_("Address Information of the recipient"))
 
 
 class AlertReferenceStructValue(StructValue):
     @property
     def ref_alert_identifier(self):
         alert_page = self.get("ref_alert").specific
-
-        if hasattr(alert_page, "cap_reference_id"):
-            return alert_page.cap_reference_id
+        if hasattr(alert_page, "sender") and hasattr(alert_page, "identifier") and hasattr(alert_page, "sent"):
+            sent = parse_tz(alert_page.sent.isoformat())
+            return "{},{},{}".format(alert_page.sender, alert_page.identifier, sent)
 
         return None
 
 
 class AlertReference(blocks.StructBlock):
     class Meta:
         value_class = AlertReferenceStructValue
@@ -694,14 +696,34 @@
     eventCode = blocks.ListBlock(AlertEventCode(label=_("Event Code")), label=_("Event codes"), default=[])
 
     # NOTE: web attribute is obtained from the url of the page
     class Meta:
         value_class = AlertInfoStructValue
         label_format = "({language}) {event}"
 
+    def clean(self, value):
+        result = super().clean(value)
+        effective = result.get("effective")
+        onset = result.get("onset")
+        expires = result.get("expires")
+
+        if expires:
+            if effective and expires < effective:
+                raise StructBlockValidationError(block_errors={
+                    "expires": ValidationError(
+                        _("The expiry time of the alert should be greater than the effective time"))
+                })
+
+            if onset and expires < onset:
+                raise StructBlockValidationError(block_errors={
+                    "expires": ValidationError(_("The expiry time of the alert should be greater than the onset time"))
+                })
+
+        return result
+
 
 class AudienceTypeBlock(blocks.StructBlock):
     audience = blocks.CharBlock(max_length=255, label=_("Audience"), help_text=_("Intended audience"))
 
 
 class ContactBlock(blocks.StructBlock):
     contact = blocks.CharBlock(max_length=255, label=_("Contact Detail"))
```

### Comparing `capeditor-0.5.3/capeditor/cap_settings.py` & `capeditor-0.5.4/capeditor/cap_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,16 @@
 
     @property
     def geojson(self):
         return json.loads(self.geom.geojson)
 
     panels = [
         FieldPanel("name"),
-        FieldPanel("geom", widget=PolygonDrawWidget(attrs={"resize_trigger_class": "map-resize-trigger"})),
+        FieldPanel("geom",
+                   widget=PolygonDrawWidget(attrs={"resize_trigger_selector": ".w-tabs__tab.map-resize-trigger"})),
     ]
 
 
 register_model_chooser(PredefinedAlertArea)
 
 
 def get_cap_setting():
```

### Comparing `capeditor-0.5.3/capeditor/caputils.py` & `capeditor-0.5.4/capeditor/caputils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/constants.py` & `capeditor-0.5.4/capeditor/constants.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/forms/capimporter.py` & `capeditor-0.5.4/capeditor/forms/capimporter.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/forms/fields.py` & `capeditor-0.5.4/capeditor/forms/fields.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/forms/widgets.py` & `capeditor-0.5.4/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.5.4/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.5.4/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.5.4/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.5.4/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.5.4/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.5.4/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.5.4/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.5.4/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.5.4/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.5.4/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.5.4/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.5.4/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/migrations/0001_initial.py` & `capeditor-0.5.4/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/migrations/0002_alter_capsetting_options_and_more.py` & `capeditor-0.5.4/capeditor/migrations/0002_alter_capsetting_options_and_more.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/migrations/0003_capsetting_logo.py` & `capeditor-0.5.4/capeditor/migrations/0003_capsetting_logo.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/migrations/0004_predefinedalertarea.py` & `capeditor-0.5.4/capeditor/migrations/0004_predefinedalertarea.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/models.py` & `capeditor-0.5.4/capeditor/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,14 +86,56 @@
                         label = audience_block.label or field_name
                         name = audience_block.name
                         info_field.block.child_blocks[block_type].child_blocks[field_name] = blocks.ChoiceBlock(
                             choices=audience_type_choices, required=False, help_text=AUDIENCE_HELP_TEXT)
                         info_field.block.child_blocks[block_type].child_blocks[field_name].name = name
                         info_field.block.child_blocks[block_type].child_blocks[field_name].label = label
 
+    def clean(self):
+        cleaned_data = super().clean()
+
+        # validata msgType
+        msgType = cleaned_data.get("msgType")
+        if msgType and msgType != 'Alert':
+            references = cleaned_data.get("references")
+            if not references:
+                # if the message type is not 'Alert' then references are required
+                self.add_error('references', _("You must select at least one reference alert for this message type. "
+                                               "Only 'Alert' Message Type can be saved without references."))
+            else:
+                alerts_ids = []
+                for reference in references:
+                    ref_alert_page = reference.value.get("ref_alert").specific
+                    if ref_alert_page:
+                        alerts_ids.append(ref_alert_page.identifier)
+
+                # check if the same alert is selected more than once
+                if len(alerts_ids) != len(set(alerts_ids)):
+                    self.add_error('references', _("You cannot select the same alert more than once."))
+
+        # validate dates
+        sent = cleaned_data.get("sent")
+        alert_infos = cleaned_data.get("info")
+        if alert_infos:
+            for info in alert_infos:
+                effective = info.value.get("effective")
+                onset = info.value.get("onset")
+                expires = info.value.get("expires")
+
+                if effective and sent and effective < sent:
+                    self.add_error('info', _("Effective date cannot be earlier than the alert sent date."))
+
+                if onset and sent and onset < sent:
+                    self.add_error('info', _("Onset date cannot be earlier than the alert sent date."))
+
+                if expires and sent and expires < sent:
+                    self.add_error('info', _("Expires date cannot be earlier than the alert sent date."))
+
+        return cleaned_data
+
 
 class AbstractCapAlertPage(Page):
     base_form_class = CapAlertPageForm
 
     exclude_fields_in_copy = ["identifier"]
 
     STATUS_CHOICES = (
```

### Comparing `capeditor-0.5.3/capeditor/pubsub/base.py` & `capeditor-0.5.4/capeditor/pubsub/base.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/pubsub/mqtt.py` & `capeditor-0.5.4/capeditor/pubsub/mqtt.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/pubsub/publish.py` & `capeditor-0.5.4/capeditor/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/renderers.py` & `capeditor-0.5.4/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/serializers.py` & `capeditor-0.5.4/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.5.4/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/css/import_cap_preview.css` & `capeditor-0.5.4/capeditor/static/capeditor/css/import_cap_preview.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/css/mapbox-gl-draw.css` & `capeditor-0.5.4/capeditor/static/capeditor/css/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/css/maplibre-gl.css` & `capeditor-0.5.4/capeditor/static/capeditor/css/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.5.4/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.5.4/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/fonts/mapbox-gl-draw.css` & `capeditor-0.5.4/capeditor/static/capeditor/fonts/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/alert.png` & `capeditor-0.5.4/capeditor/static/capeditor/images/alert.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/alert.svg` & `capeditor-0.5.4/capeditor/static/capeditor/images/alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/area.png` & `capeditor-0.5.4/capeditor/static/capeditor/images/area.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/certainty.png` & `capeditor-0.5.4/capeditor/static/capeditor/images/certainty.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/extreme.png` & `capeditor-0.5.4/capeditor/static/capeditor/images/extreme.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/minor.png` & `capeditor-0.5.4/capeditor/static/capeditor/images/minor.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/moderate.png` & `capeditor-0.5.4/capeditor/static/capeditor/images/moderate.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/images/severe.png` & `capeditor-0.5.4/capeditor/static/capeditor/images/severe.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/conditional_fields.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/mapbox-gl-draw.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/mapbox-gl-draw.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/maplibre-gl.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/turf.min.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/turf.min.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -109,14 +109,15 @@
     }
 
     // initialize map
     this.map = new maplibregl.Map({
         container: this.options.map_id,
         style: defaultStyle,
         doubleClickZoom: false,
+        scrollZoom: false,
     });
 
 
     this.map.addControl(
         new maplibregl.NavigationControl({
             showCompass: false,
         }), "bottom-right"
@@ -302,13 +303,20 @@
                         level
                     } = boundary
                     const name = boundary[`name_${level}`]
 
                     if (name) {
                         this.areaDescInput.val(name)
                     }
-                    this.setSourceData(feature)
+
+                    const truncatedFeature = turf.truncate(feature, {
+                        precision: 2,
+                        coordinates: 2,
+                        mutate: true
+                    })
+
+                    this.setSourceData(truncatedFeature)
                 })
             }
         }
     });
 }
```

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -130,14 +130,15 @@
     }
 
     // initialize map
     this.map = new maplibregl.Map({
         container: this.options.map_id,
         style: defaultStyle,
         doubleClickZoom: false,
+        scrollZoom: false,
     });
 
 
     this.map.addControl(
         new maplibregl.NavigationControl({
             showCompass: false,
         }), "bottom-right"
@@ -297,16 +298,14 @@
         this.setState("")
     }
 }
 
 CircleWidget.prototype.initFromState = function() {
     const circeValue = this.getState()
 
-    console.log(circeValue)
-
     if (circeValue) {
         const {
             lon,
             lat,
             radius
         } = this.parseCircleValue(circeValue) || {}
```

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-draw-widget.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/polygon-draw-widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,36 +6,34 @@
         this.map = null;
         this.ready = false;
 
         this.options = options
         this.geomInput = document.getElementById(this.options.id)
 
 
-        if (this.options.resize_trigger_class) {
-            this.resizeTriggerEls = document.getElementsByClassName(this.options.resize_trigger_class)
+        if (this.options.resize_trigger_selector) {
+            this.resizeTriggerEls = document.querySelectorAll(this.options.resize_trigger_selector)
         }
 
         this.initalValue = this.geomInput.value
         this.countriesBounds = this.geomInput.dataset.bounds ? JSON.parse(this.geomInput.dataset.bounds) : null
 
         this.createMap().then((map) => {
             this.map = map;
-
             this.fitBounds()
 
             if (this.resizeTriggerEls && this.resizeTriggerEls.length > 0) {
                 for (let i = 0; i < this.resizeTriggerEls.length; i++) {
                     const el = this.resizeTriggerEls[i];
                     el.addEventListener('click', () => {
                         this.fitBounds()
                     })
                 }
             }
 
-
             this.initDraw();
         });
 
     }
 
 
     async createMap() {
@@ -79,14 +77,15 @@
         }
 
         // initialize map
         const map = new maplibregl.Map({
             container: this.options.map_id,
             style: defaultStyle,
             doubleClickZoom: false,
+            scrollZoom: false,
         });
 
 
         map.addControl(
             new maplibregl.NavigationControl({
                 showCompass: false,
             }), "bottom-right"
@@ -144,15 +143,14 @@
 
     setValue(feature) {
         this.geomInput.value = feature;
     }
 
     initDraw() {
         const feature = this.getValue()
-
         this.draw = new MapboxDraw({
             displayControlsDefault: false,
             controls: {
                 polygon: true,
                 trash: true
             },
         });
@@ -179,14 +177,21 @@
         if (featureCollection && featureCollection.features && !!featureCollection.features.length) {
             combinedFeatures = turf.combine(featureCollection)
         }
 
         if (combinedFeatures) {
             const feature = combinedFeatures.features[0]
 
-            this.setValue(JSON.stringify(feature.geometry))
+
+            const truncatedFeature = turf.truncate(feature, {
+                precision: 2,
+                coordinates: 2,
+                mutate: true
+            })
+
+            this.setValue(JSON.stringify(truncatedFeature.geometry))
 
         } else {
             this.setValue("")
         }
     }
 }
```

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.5.4/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -161,14 +161,15 @@
     }
 
     // initialize map
     this.map = new maplibregl.Map({
         container: this.options.map_id,
         style: defaultStyle,
         doubleClickZoom: false,
+        scrollZoom: false,
     });
 
 
     this.map.addControl(
         new maplibregl.NavigationControl({
             showCompass: false,
         }), "bottom-right"
@@ -326,16 +327,24 @@
     if (this.saveCancelControl) {
         this.map.removeControl(this.saveCancelControl)
         this.saveCancelControl = null
     }
 }
 
 
-PolygonWidget.prototype.setDrawData = function(geometry) {
-    if (geometry) {
+PolygonWidget.prototype.setDrawData = function(featureGeom) {
+    if (featureGeom) {
+
+        // truncate geometry
+        const geometry = turf.truncate(featureGeom, {
+            precision: 2,
+            coordinates: 2,
+            mutate: true
+        })
+
         const bbox = turf.bbox(geometry)
         const bounds = [
             [bbox[0], bbox[1]],
             [bbox[2], bbox[3]]
         ]
 
         this.setSourceData(geometry)
```

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.5.4/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.5.4/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.5.4/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/load_cap_alert.html` & `capeditor-0.5.4/capeditor/templates/capeditor/load_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/preview_cap_alert.html` & `capeditor-0.5.4/capeditor/templates/capeditor/preview_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.5.4/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html` & `capeditor-0.5.4/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/templates/capeditor/widgets/polygon_draw_widget.html` & `capeditor-0.5.4/capeditor/templates/capeditor/widgets/polygon_draw_widget.html`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,14 @@
         {% block options %}
             var options = {
                 geom_name: '{{ geom_type }}',
                 id: '{{ id }}',
                 map_id: '{{ id }}_map',
                 map_srid: {{ map_srid|unlocalize }},
                 name: '{{ name }}',
-                resize_trigger_class: '{{ resize_trigger_class }}',
+                resize_trigger_selector: '{{ resize_trigger_selector }}',
             };
         {% endblock %}
         var {{ module }} =
         new PolygonDrawWidget(options);
     </script>
 </div>
```

### Comparing `capeditor-0.5.3/capeditor/utils.py` & `capeditor-0.5.4/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/views.py` & `capeditor-0.5.4/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor/wagtail_hooks.py` & `capeditor-0.5.4/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/capeditor.egg-info/PKG-INFO` & `capeditor-0.5.4/capeditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.3
+Version: 0.5.4
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.5.3/capeditor.egg-info/SOURCES.txt` & `capeditor-0.5.4/capeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.3/setup.cfg` & `capeditor-0.5.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.5.3
+version = 0.5.4
 description = Wagtail based CAP composer
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-composer
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
```

