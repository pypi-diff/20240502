# Comparing `tmp/pyams_app_msc-1.99.2.tar.gz` & `tmp/pyams_app_msc-1.99.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_app_msc-1.99.2.tar", last modified: Sun Apr 28 15:45:17 2024, max compression
+gzip compressed data, was "dist/pyams_app_msc-1.99.2.4.tar", last modified: Thu May  2 21:32:26 2024, max compression
```

## Comparing `pyams_app_msc-1.99.2.tar` & `pyams_app_msc-1.99.2.4.tar`

### file list

```diff
@@ -1,386 +1,386 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3201 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1664 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/booking.puml
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/classes.puml
--rw-rw-rw-   0 root         (0) root         (0)    16507 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/docs/es-mapping.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/assets/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/clock.png
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/email.png
--rw-rw-rw-   0 root         (0) root         (0)   207972 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)   117372 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)    68004 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    25452 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   419720 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)   156496 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.woff2
--rw-rw-rw-   0 root         (0) root         (0)    10832 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.ttf
--rw-rw-rw-   0 root         (0) root         (0)     4792 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.woff2
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/form.png
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/layers-2x.png
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/layers.png
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/marker-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/phone.png
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/select2-spinner.gif
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/select2.png
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/select2x2.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/assets/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/dev/
--rw-rw-rw-   0 root         (0) root         (0)   263831 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/dev/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/dist/
--rw-rw-rw-   0 root         (0) root         (0)   337917 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/dist/msc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/css/img/
--rw-rw-rw-   0 root         (0) root         (0)     2508 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/clock.png
--rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/download.svg
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/email.png
--rw-rw-rw-   0 root         (0) root         (0)     7604 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/form.png
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/link.svg
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/list-item.png
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/map.png
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/mobile-menu.png
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/phone.png
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/print.svg
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/search.png
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/css/img/social-icons.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/js/dev/
--rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js.map
--rw-rw-rw-   0 root         (0) root         (0)     4652 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    10624 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)     6409 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    19333 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
--rw-rw-rw-   0 root         (0) root         (0)    29675 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   209738 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
--rw-rw-rw-   0 root         (0) root         (0)   236865 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   182041 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
--rw-rw-rw-   0 root         (0) root         (0)   230602 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
--rw-rw-rw-   0 root         (0) root         (0)   181575 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
--rw-rw-rw-   0 root         (0) root         (0)   230045 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
--rw-rw-rw-   0 root         (0) root         (0)   174144 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
--rw-rw-rw-   0 root         (0) root         (0)   220941 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
--rw-rw-rw-   0 root         (0) root         (0)    21983 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
--rw-rw-rw-   0 root         (0) root         (0)    18395 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)    18911 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
--rw-rw-rw-   0 root         (0) root         (0)    20127 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   450498 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
--rw-rw-rw-   0 root         (0) root         (0)   569896 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)    46418 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
--rw-rw-rw-   0 root         (0) root         (0)    53162 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
--rw-rw-rw-   0 root         (0) root         (0)   153997 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
--rw-rw-rw-   0 root         (0) root         (0)   189149 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
--rw-rw-rw-   0 root         (0) root         (0)   114212 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
--rw-rw-rw-   0 root         (0) root         (0)   139871 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/pkg/js/dist/
--rw-rw-rw-   0 root         (0) root         (0)     7914 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/116.js
--rw-rw-rw-   0 root         (0) root         (0)     8340 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/137.js
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/178.js
--rw-rw-rw-   0 root         (0) root         (0)    67548 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/23.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/23.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/243.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/243.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16009 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/274.js
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/284.js
--rw-rw-rw-   0 root         (0) root         (0)    69465 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/458.js
--rw-rw-rw-   0 root         (0) root         (0)     3219 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/47.js
--rw-rw-rw-   0 root         (0) root         (0)   148911 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/481.js
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/481.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/528.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/528.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70026 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/612.js
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/612.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    16008 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/623.js
--rw-rw-rw-   0 root         (0) root         (0)    61493 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/624.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/624.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)   105878 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/660.js
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/660.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/671.js
--rw-rw-rw-   0 root         (0) root         (0)    69464 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/686.js
--rw-rw-rw-   0 root         (0) root         (0)    61491 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/698.js
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/698.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    70252 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/814.js
--rw-rw-rw-   0 root         (0) root         (0)     1457 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/814.js.LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/830.js
--rw-rw-rw-   0 root         (0) root         (0)     1859 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/854.js
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/860.js
--rw-rw-rw-   0 root         (0) root         (0)    18213 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/882.js
--rw-rw-rw-   0 root         (0) root         (0)   937336 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3871 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2428 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1828 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/
--rw-rw-rw-   0 root         (0) root         (0)    12350 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/container.py
--rw-rw-rw-   0 root         (0) root         (0)     9708 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4366 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/reminder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6130 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    36201 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15231 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/home.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/reminder.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3121 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
--rw-rw-rw-   0 root         (0) root         (0)    38087 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3332 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/
--rw-rw-rw-   0 root         (0) root         (0)     3511 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    12100 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8006 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16194 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/
--rw-rw-rw-   0 root         (0) root         (0)     3975 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7142 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/password.py
--rw-rw-rw-   0 root         (0) root         (0)    11384 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      642 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12105 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/
--rw-rw-rw-   0 root         (0) root         (0)    20552 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   167336 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)   167000 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
--rw-rw-rw-   0 root         (0) root         (0)   168644 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/
--rw-rw-rw-   0 root         (0) root         (0)    17688 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4826 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/generations/
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8674 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/include.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    62537 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
--rw-rw-rw-   0 root         (0) root         (0)   107792 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
--rw-rw-rw-   0 root         (0) root         (0)    76407 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/locales/pyams_app_msc.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5752 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3216 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2257 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/root/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/api/
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1862 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4485 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3434 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2050 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/search.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3704 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     6790 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6079 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/
--rw-rw-rw-   0 root         (0) root         (0)     8410 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4330 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/audience.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    12262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/audience.py
--rw-rw-rw-   0 root         (0) root         (0)     4080 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/price.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/room.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/page.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/price.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/room.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/session.py
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12679 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9666 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/audience.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3642 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/planning.py
--rw-rw-rw-   0 root         (0) root         (0)     3108 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/presentation.py
--rw-rw-rw-   0 root         (0) root         (0)     9318 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/price.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     9175 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/room.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     3618 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4526 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/types.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/form.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     5255 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/
--rw-rw-rw-   0 root         (0) root         (0)    11860 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_form.js
--rw-rw-rw-   0 root         (0) root         (0)     5731 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_gis.js
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_i18n.js
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_search.js
--rw-rw-rw-   0 root         (0) root         (0)     9714 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4237 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/mscapp.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_content.scss
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     3047 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_list.scss
--rw-rw-rw-   0 root         (0) root         (0)     4416 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
--rw-rw-rw-   0 root         (0) root         (0)      960 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_search.scss
--rw-rw-rw-   0 root         (0) root         (0)     4329 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/msc.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/skin/templates/select-admin-theater.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/img/
--rw-rw-rw-   0 root         (0) root         (0)     4680 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/img/pass-culture.webp
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    21353 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.js
--rw-rw-rw-   0 root         (0) root         (0)     8471 2024-04-28 15:44:49.000000 pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3201 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13305 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:45:11.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      677 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-28 15:45:17.000000 pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3489 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1950 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/booking.puml
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/classes.puml
+-rw-rw-rw-   0 root         (0) root         (0)    16507 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/docs/es-mapping.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/email.png
+-rw-rw-rw-   0 root         (0) root         (0)   207972 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   117372 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    68004 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    25452 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   419720 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   156496 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    10832 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.woff2
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/form.png
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/layers-2x.png
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/layers.png
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/marker-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/select2-spinner.gif
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/select2.png
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/select2x2.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/assets/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/dev/
+-rw-rw-rw-   0 root         (0) root         (0)   263831 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/dev/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/dist/
+-rw-rw-rw-   0 root         (0) root         (0)   337917 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/dist/msc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/css/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/clock.png
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/download.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/email.png
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/form.png
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/link.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/list-item.png
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/map.png
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/mobile-menu.png
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/phone.png
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/print.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/search.png
+-rw-rw-rw-   0 root         (0) root         (0)     7058 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/css/img/social-icons.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/
+-rw-rw-rw-   0 root         (0) root         (0)  2392493 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)  2948389 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    10624 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    19333 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    29675 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   209738 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   236865 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   182041 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js
+-rw-rw-rw-   0 root         (0) root         (0)   230602 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   181575 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js
+-rw-rw-rw-   0 root         (0) root         (0)   230045 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   174144 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js
+-rw-rw-rw-   0 root         (0) root         (0)   220941 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    21983 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    18395 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   450498 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   569896 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    46418 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js
+-rw-rw-rw-   0 root         (0) root         (0)    53162 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   153997 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   189149 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   114212 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js
+-rw-rw-rw-   0 root         (0) root         (0)   139871 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/
+-rw-rw-rw-   0 root         (0) root         (0)     7914 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/116.js
+-rw-rw-rw-   0 root         (0) root         (0)     8340 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/137.js
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/178.js
+-rw-rw-rw-   0 root         (0) root         (0)    67548 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/23.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/23.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/243.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/243.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16009 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/274.js
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/284.js
+-rw-rw-rw-   0 root         (0) root         (0)    69465 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/458.js
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/47.js
+-rw-rw-rw-   0 root         (0) root         (0)   148911 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/481.js
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/481.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/528.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/528.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70026 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/612.js
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/612.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    16008 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/623.js
+-rw-rw-rw-   0 root         (0) root         (0)    61493 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/624.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/624.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)   105878 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/660.js
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/660.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/671.js
+-rw-rw-rw-   0 root         (0) root         (0)    69464 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/686.js
+-rw-rw-rw-   0 root         (0) root         (0)    61491 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/698.js
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/698.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/814.js
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/814.js.LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/830.js
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/854.js
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/860.js
+-rw-rw-rw-   0 root         (0) root         (0)    18213 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/882.js
+-rw-rw-rw-   0 root         (0) root         (0)   937336 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3901 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2428 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/
+-rw-rw-rw-   0 root         (0) root         (0)    12350 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     9708 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4366 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/reminder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/booking-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    36201 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15562 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/home.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/reminder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8133 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3121 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt
+-rw-rw-rw-   0 root         (0) root         (0)    38087 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3464 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/
+-rw-rw-rw-   0 root         (0) root         (0)     3511 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    12100 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8006 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16194 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7142 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/password.py
+-rw-rw-rw-   0 root         (0) root         (0)    11384 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      642 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/password-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6337 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12105 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/
+-rw-rw-rw-   0 root         (0) root         (0)    20552 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   167336 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   167000 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   168644 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/
+-rw-rw-rw-   0 root         (0) root         (0)    17688 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    62537 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo
+-rw-rw-rw-   0 root         (0) root         (0)   107792 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po
+-rw-rw-rw-   0 root         (0) root         (0)    76407 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/pyams_app_msc.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     6790 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8269 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6079 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/
+-rw-rw-rw-   0 root         (0) root         (0)     8410 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4330 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/audience.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    12262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/room.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12679 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9666 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/audience.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/planning.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/presentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9318 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/price.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9175 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/room.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     3618 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4526 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5255 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)    11860 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_form.js
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_gis.js
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_i18n.js
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_search.js
+-rw-rw-rw-   0 root         (0) root         (0)     9714 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4237 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/i18n/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/mscapp.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_breadcrumbs.scss
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_content.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_layout.scss
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_list.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_misc.scss
+-rw-rw-rw-   0 root         (0) root         (0)      960 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_search.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/msc.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/templates/select-admin-theater.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/img/
+-rw-rw-rw-   0 root         (0) root         (0)     4680 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/img/pass-culture.webp
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    21353 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.js
+-rw-rw-rw-   0 root         (0) root         (0)     8471 2024-05-02 21:31:46.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3489 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13305 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:32:14.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      698 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 21:32:26.000000 pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/top_level.txt
```

### Comparing `pyams_app_msc-1.99.2/LICENSE` & `pyams_app_msc-1.99.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/PKG-INFO` & `pyams_app_msc-1.99.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_app_msc
-Version: 1.99.2
+Version: 1.99.2.4
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -44,14 +44,30 @@
 PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.2.4
+--------
+ - removed code dependency on OAuth authentication module (bis!)
+
+1.99.2.3
+--------
+ - removed code dependency on OAuth authentication module
+
+1.99.2.2
+--------
+ - updated tests requirements
+
+1.99.2.1
+--------
+ - issue #24: updated booking value getter in dashboards
+
 1.99.2
 ------
  - updated menus order
  - added paragraphs factory settings support to movie theater
  - updated booking recipient label
  - added structure type attribute to user profile
  - disable autocomplete on user profile creation form
```

### Comparing `pyams_app_msc-1.99.2/docs/HISTORY.rst` & `pyams_app_msc-1.99.2.4/docs/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changelog
 =========
 
+1.99.2.4
+--------
+ - removed code dependency on OAuth authentication module (bis!)
+
+1.99.2.3
+--------
+ - removed code dependency on OAuth authentication module
+
+1.99.2.2
+--------
+ - updated tests requirements
+
+1.99.2.1
+--------
+ - issue #24: updated booking value getter in dashboards
+
 1.99.2
 ------
  - updated menus order
  - added paragraphs factory settings support to movie theater
  - updated booking recipient label
  - added structure type attribute to user profile
  - disable autocomplete on user profile creation form
```

### Comparing `pyams_app_msc-1.99.2/docs/README.rst` & `pyams_app_msc-1.99.2.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/docs/classes.puml` & `pyams_app_msc-1.99.2.4/docs/classes.puml`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/docs/es-mapping.json` & `pyams_app_msc-1.99.2.4/docs/es-mapping.json`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/clock.png` & `pyams_app_msc-1.99.2.4/pkg/assets/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/email.png` & `pyams_app_msc-1.99.2.4/pkg/assets/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.ttf` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-brands-400.woff2` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.ttf` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-regular-400.woff2` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.ttf` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-solid-900.woff2` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.ttf` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/fa-v4compatibility.woff2` & `pyams_app_msc-1.99.2.4/pkg/assets/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/form.png` & `pyams_app_msc-1.99.2.4/pkg/assets/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/layers-2x.png` & `pyams_app_msc-1.99.2.4/pkg/assets/layers-2x.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/layers.png` & `pyams_app_msc-1.99.2.4/pkg/assets/layers.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/list-item.png` & `pyams_app_msc-1.99.2.4/pkg/assets/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/map.png` & `pyams_app_msc-1.99.2.4/pkg/assets/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/marker-icon.png` & `pyams_app_msc-1.99.2.4/pkg/assets/marker-icon.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/mobile-menu.png` & `pyams_app_msc-1.99.2.4/pkg/assets/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/phone.png` & `pyams_app_msc-1.99.2.4/pkg/assets/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/select2-spinner.gif` & `pyams_app_msc-1.99.2.4/pkg/assets/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/select2.png` & `pyams_app_msc-1.99.2.4/pkg/assets/select2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/select2x2.png` & `pyams_app_msc-1.99.2.4/pkg/assets/select2x2.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/assets/social-icons.png` & `pyams_app_msc-1.99.2.4/pkg/assets/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/dev/msc.css` & `pyams_app_msc-1.99.2.4/pkg/css/dev/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/dist/msc.css` & `pyams_app_msc-1.99.2.4/pkg/css/dist/msc.css`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/clock.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/clock.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/download.svg` & `pyams_app_msc-1.99.2.4/pkg/css/img/download.svg`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/email.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/email.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/form.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/form.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/list-item.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/list-item.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/map.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/map.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/mobile-menu.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/mobile-menu.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/phone.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/phone.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/search.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/search.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/css/img/social-icons.png` & `pyams_app_msc-1.99.2.4/pkg/css/img/social-icons.png`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/mscapp.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/mscapp.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_jquery-validation_dist_localization_messages_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js__form_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/src_pyams_app_msc_skin_resources_src_js_i18n_fr_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_inputmask_dist_inputmask_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-scrollto_out_lib-28fdf0.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-90cd1e.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_jquery-form_dist_jquery_form_min_js-node_modules_jquery-validation_dist_-f675ac.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet-gesture-handling_dist_leaflet-gesture-handling_min_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet-src_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_leaflet_dist_leaflet_css.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_select2_dist_js_select2_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map` & `pyams_app_msc-1.99.2.4/pkg/js/dev/vendors-node_modules_tempusdominus-bootstrap-4_build_js_tempusdominus-bootstrap-4_js.js.map`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/116.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/116.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/137.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/137.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/23.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/23.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/23.js.LICENSE.txt` & `pyams_app_msc-1.99.2.4/pkg/js/dist/23.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/243.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/243.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/274.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/274.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/284.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/284.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/458.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/458.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/47.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/47.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/481.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/481.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/528.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/528.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/528.js.LICENSE.txt` & `pyams_app_msc-1.99.2.4/pkg/js/dist/528.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/612.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/612.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/612.js.LICENSE.txt` & `pyams_app_msc-1.99.2.4/pkg/js/dist/612.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/623.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/623.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/624.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/624.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/660.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/660.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/686.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/686.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/698.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/698.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/814.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/814.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/814.js.LICENSE.txt` & `pyams_app_msc-1.99.2.4/pkg/js/dist/814.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/830.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/830.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/854.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/854.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/860.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/860.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/882.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/882.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js` & `pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/pkg/js/dist/mscapp.js.LICENSE.txt` & `pyams_app_msc-1.99.2.4/pkg/js/dist/mscapp.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/setup.py` & `pyams_app_msc-1.99.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.2'
+version = '1.99.2.4'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 data_dir = 'pkg'
 data_files = [(d, [os.path.join(d, f) for f in files])
               for d, folders, files in os.walk(data_dir)]
 
 tests_require = [
+    'pyams_content_themes',
     'pyramid_zcml',
     'zope.exceptions'
 ]
 
 setup(name='pyams_app_msc',
       version=version,
       description="PyAMS application for cinema reservation management",
```

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/address/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/address/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/admininfo/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/admininfo/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/banking/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/banking/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/contact/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/contact/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/schema.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/duration/zmi/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/duration/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/component/paragraph/zmi/container.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/component/paragraph/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/container.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/container.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/reminder.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/skin/templates/booking-new-header.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/task.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/dashboard.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,19 +127,22 @@
     def __acl__(self):
         return self.booking.__acl__
 
 
 def get_booking_element(booking):
     """Get booking element from booking input"""
     session = booking.session
-    entry = IWorkflowVersions(get_parent(session, ICatalogEntry)).get_last_versions()[0]
+    wf_entry = None
+    entry = get_parent(session, ICatalogEntry)
+    if entry is not None:
+        wf_entry = IWorkflowVersions(entry).get_last_versions()[0]
     return BookingElement({
         'booking': booking,
         'session': session,
-        'entry': entry
+        'entry': wf_entry
     })
 
 
 @adapter_config(required=IBookingElement,
                 provides=ICacheKeyValue)
 def booking_element_cache_key_value(context):
     """Booking element cache key value adapter"""
@@ -183,14 +186,21 @@
     i18n_header = _("Session")
     css_classes = {
         'td': 'text-nowrap'
     }
     weight = 10
 
     def get_value(self, obj):
+        if obj.entry is None:
+            label = obj.session.label
+            if label:
+                label = f'({label})'
+            else:
+                label = self.request.localizer.translate(_("Out of catalog activity"))
+            return label
         return get_object_label(obj.entry, self.request, self.table)
 
 
 @adapter_config(name='room',
                 required=(IMovieTheater, IAdminLayer, IBookingStatusTable),
                 provides=IColumn)
 class BookingStatusRoomColumn(I18nColumnMixin, GetAttrColumn):
```

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/home.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/home.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/reminder.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/reminder.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/search.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/task.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/templates/today-program.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/booking/zmi/workflow.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/booking/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/messaging/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/messaging/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,37 +20,43 @@
 
 import requests
 from pyramid.events import subscriber
 from pyramid.httpexceptions import HTTPOk
 from zope.lifecycleevent.interfaces import IObjectAddedEvent
 
 from pyams_app_msc.feature.profile import IUserProfile
-from pyams_auth_oauth.interfaces import IOAuthUser
 from pyams_zmi.interfaces.profile import IUserProfile as IZMIProfile
 
 __docformat__ = 'restructuredtext'
 
 
-@subscriber(IObjectAddedEvent, context_selector=IOAuthUser)
-def handle_new_oauth_user(event):
-    """Handle new OAuth user"""
-    folder = event.newParent
-    if folder is None:
-        return
-    user_info = event.object
-    principal_info = folder.get_principal(principal_id=f'{folder.prefix}:{user_info.user_id}', info=True)
-    if principal_info is None:
-        return
-    profile = IUserProfile(principal_info)
-    profile.firstname = user_info.first_name
-    profile.lastname = user_info.last_name
-    profile.email = user_info.email
-    if user_info.picture:
-        response = requests.get(user_info.picture)
-        if response.status_code == HTTPOk.code:
-            zmi_profile = IZMIProfile(principal_info)
-            content_type = response.headers.get('content-type')
-            if content_type:
-                filename = f'profile{mimetypes.guess_extension(content_type)}'
-            else:
-                filename = 'profile.jpg'
-            zmi_profile.avatar = (filename, response.content)
+try:
+
+    from pyams_auth_oauth.interfaces import IOAuthUser
+
+    @subscriber(IObjectAddedEvent, context_selector=IOAuthUser)
+    def handle_new_oauth_user(event):
+        """Handle new OAuth user"""
+        folder = event.newParent
+        if folder is None:
+            return
+        user_info = event.object
+        principal_info = folder.get_principal(principal_id=f'{folder.prefix}:{user_info.user_id}', info=True)
+        if principal_info is None:
+            return
+        profile = IUserProfile(principal_info)
+        profile.firstname = user_info.first_name
+        profile.lastname = user_info.last_name
+        profile.email = user_info.email
+        if user_info.picture:
+            response = requests.get(user_info.picture)
+            if response.status_code == HTTPOk.code:
+                zmi_profile = IZMIProfile(principal_info)
+                content_type = response.headers.get('content-type')
+                if content_type:
+                    filename = f'profile{mimetypes.guess_extension(content_type)}'
+                else:
+                    filename = 'profile.jpg'
+                zmi_profile.avatar = (filename, response.content)
+
+except ImportError:
+    pass
```

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/oauth/skin/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/oauth/skin/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,59 +17,64 @@
 from hypatia.catalog import CatalogQuery
 from hypatia.interfaces import ICatalog
 from hypatia.query import And, Eq, Or
 from pyramid.events import subscriber
 
 from pyams_app_msc.feature.profile import IUserProfile
 from pyams_app_msc.shared.theater import IMovieTheater
-from pyams_auth_oauth.interfaces import IOAuthAuthenticationEvent
 from pyams_catalog.query import CatalogResultSet
 from pyams_security.interfaces import LOGIN_REFERER_KEY
-from pyams_security.interfaces.base import IUnavailablePrincipalInfo
 from pyams_security.utility import get_principal
 from pyams_utils.factory import get_interface_base_name
 from pyams_utils.registry import get_utility
 from pyams_utils.url import absolute_url
 
 __docformat__ = 'restructuredtext'
 
 
-@subscriber(IOAuthAuthenticationEvent)
-def handle_oauth_authentication(event):
-    """Handle redirect on OAuth authentication"""
-    principal_id = event.principal_id
-    principal = get_principal(principal_id=principal_id)
-    profile_info = IUserProfile(principal, None)
-    if profile_info is None:
-        return
-    request = event.request
-    if not (profile_info.firstname and profile_info.lastname and
-            profile_info.email and profile_info.establishment and
-            profile_info.local_theaters):
-        event.redirect_location = absolute_url(request.root, request, 'my-profile.html')
-    else:
-        theaters_names = profile_info.local_theaters
-        if len(theaters_names) == 1:
-            theater = get_utility(IMovieTheater, name=theaters_names[0])
-            if theater is not None:
-                event.redirect_location = absolute_url(theater, request)
-                return
-        session = request.session
-        if LOGIN_REFERER_KEY in session:
-            event.redirect_location = session[LOGIN_REFERER_KEY]
-            del session[LOGIN_REFERER_KEY]
+try:
+
+    from pyams_auth_oauth.interfaces import IOAuthAuthenticationEvent
+
+    @subscriber(IOAuthAuthenticationEvent)
+    def handle_oauth_authentication(event):
+        """Handle redirect on OAuth authentication"""
+        principal_id = event.principal_id
+        principal = get_principal(principal_id=principal_id)
+        profile_info = IUserProfile(principal, None)
+        if profile_info is None:
+            return
+        request = event.request
+        if not (profile_info.firstname and profile_info.lastname and
+                profile_info.email and profile_info.establishment and
+                profile_info.local_theaters):
+            event.redirect_location = absolute_url(request.root, request, 'my-profile.html')
         else:
-            catalog = get_utility(ICatalog)
-            query = And(Eq(catalog['object_types'], get_interface_base_name(IMovieTheater)),
-                        Or(Eq(catalog['role:msc:manager'], principal_id),
-                           Eq(catalog['role:msc:operator'], principal_id),
-                           Eq(catalog['role:msc:contributor'], principal_id),
-                           Eq(catalog['role:msc:reader'], principal_id)))
-            theaters = list(CatalogResultSet(CatalogQuery(catalog).query(query)))
-            if len(theaters) == 1:
-                theater = theaters[0]
-                event.redirect_location = absolute_url(theater, request, 'admin')
-            elif len(theaters) > 1:
-                event.redirect_location = absolute_url(request.root, request,
-                                                      'select-admin-theater.html')
+            theaters_names = profile_info.local_theaters
+            if len(theaters_names) == 1:
+                theater = get_utility(IMovieTheater, name=theaters_names[0])
+                if theater is not None:
+                    event.redirect_location = absolute_url(theater, request)
+                    return
+            session = request.session
+            if LOGIN_REFERER_KEY in session:
+                event.redirect_location = session[LOGIN_REFERER_KEY]
+                del session[LOGIN_REFERER_KEY]
             else:
-                event.redirect_location = absolute_url(request.context, request)
+                catalog = get_utility(ICatalog)
+                query = And(Eq(catalog['object_types'], get_interface_base_name(IMovieTheater)),
+                            Or(Eq(catalog['role:msc:manager'], principal_id),
+                               Eq(catalog['role:msc:operator'], principal_id),
+                               Eq(catalog['role:msc:contributor'], principal_id),
+                               Eq(catalog['role:msc:reader'], principal_id)))
+                theaters = list(CatalogResultSet(CatalogQuery(catalog).query(query)))
+                if len(theaters) == 1:
+                    theater = theaters[0]
+                    event.redirect_location = absolute_url(theater, request, 'admin')
+                elif len(theaters) > 1:
+                    event.redirect_location = absolute_url(request.root, request,
+                                                          'select-admin-theater.html')
+                else:
+                    event.redirect_location = absolute_url(request.context, request)
+
+except ImportError:
+    pass
```

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/session.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/session.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/planning/zmi/templates/planning.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 #
 
 """PyAMS_*** module
 
 """
 
 from persistent import Persistent
+from pyramid.authorization import ALL_PERMISSIONS, Allow
 from pyramid.interfaces import IRequest
-from pyramid.security import ALL_PERMISSIONS, Allow
 from zope.container.contained import Contained
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_app_msc.feature.profile.interfaces import IOperatorProfile, IUserProfile, OPERATOR_PROFILE_KEY, \
     USER_PROFILE_KEY
 from pyams_app_msc.reference.structure import IStructureTypeTable
 from pyams_i18n.interfaces import II18n
```

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/password.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/password.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/register.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/register.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/password-changed.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-final.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/skin/templates/register-ok.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/task.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/task.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/templates/principal-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/profile/zmi/widget.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/profile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/quotation/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/api/schema.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/feature/tmdb/zmi/lookup.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/feature/tmdb/zmi/lookup.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/generations/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/include.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/include.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.mo`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/fr/LC_MESSAGES/pyams_app_msc.po`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/locales/pyams_app_msc.pot` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/locales/pyams_app_msc.pot`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/structure/zmi/table.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/structure/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/reference/zmi/viewlet.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/reference/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/root/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/root/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/root/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/root/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/api/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/index.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/index.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/manager.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/page.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/portlet/skin/templates/view-catalog-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/search.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/security.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/security.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/skin/templates/specificities.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/dashboard.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/catalog/zmi/workflow.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/catalog/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/common/zmi/viewlet.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/common/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/site/zmi/viewlet.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/site/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/price.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/api/schema.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/api/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/audience.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/audience.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/mail.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/price.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/interfaces/room.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/interfaces/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/mail.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/page.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/page.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/price.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/room.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/session.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/settings.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/audience.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/audience.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/interfaces.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/mail.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/planning.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/planning.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/presentation.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/presentation.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/price.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/price.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/restrictions.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/room.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/room.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/search.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/session.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/session.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/types.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/types.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/shared/theater/zmi/viewlet.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/shared/theater/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/form.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/form.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/layer.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/layer.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/login.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/login.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_form.js` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_form.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_gis.js` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_gis.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_search.js` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_search.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/_utils.js` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/_utils.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/js/app.js` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/js/app.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_content.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_content.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_footer.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_footer.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_forms.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_forms.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_layout.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_layout.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_misc.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_misc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_mobile.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/_variables.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/_variables.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/resources/src/sass/msc.scss` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/resources/src/sass/msc.scss`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/skin/templates/select-admin-theater.pt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/skin/templates/select-admin-theater.pt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/tests/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocs.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/tests/test_utilsdocstrings.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/__init__.py` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/img/pass-culture.webp` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/img/pass-culture.webp`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.js` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc/zmi/resources/js/msc.min.js` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc/zmi/resources/js/msc.min.js`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/PKG-INFO` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-app-msc
-Version: 1.99.2
+Version: 1.99.2.4
 Summary: PyAMS application for cinema reservation management
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -44,14 +44,30 @@
 PyAMS MSC application is a french web application ("Ma Séance Cinéma") which is used to manage sessions
 and bookings in movies theaters.
 
 
 Changelog
 =========
 
+1.99.2.4
+--------
+ - removed code dependency on OAuth authentication module (bis!)
+
+1.99.2.3
+--------
+ - removed code dependency on OAuth authentication module
+
+1.99.2.2
+--------
+ - updated tests requirements
+
+1.99.2.1
+--------
+ - issue #24: updated booking value getter in dashboards
+
 1.99.2
 ------
  - updated menus order
  - added paragraphs factory settings support to movie theater
  - updated booking recipient label
  - added structure type attribute to user profile
  - disable autocomplete on user profile creation form
```

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/SOURCES.txt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyams_app_msc-1.99.2/src/pyams_app_msc.egg-info/requires.txt` & `pyams_app_msc-1.99.2.4/src/pyams_app_msc.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -44,9 +44,10 @@
 zope.lifecycleevent
 zope.location
 zope.principalannotation
 zope.schema
 zope.traversing
 
 [test]
+pyams_content_themes
 pyramid_zcml
 zope.exceptions
```

